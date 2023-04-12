# Comparing `tmp/nyanlang-1.6.0.tar.gz` & `tmp/nyanlang-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyanlang-1.6.0.tar", max compression
+gzip compressed data, was "nyanlang-1.6.1.tar", max compression
```

## Comparing `nyanlang-1.6.0.tar` & `nyanlang-1.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11342 2023-03-30 11:49:13.955098 nyanlang-1.6.0/LICENSE
--rw-r--r--   0        0        0      529 2023-04-01 06:11:32.522384 nyanlang-1.6.0/README.md
--rw-r--r--   0        0        0     1094 2023-03-30 10:43:06.836493 nyanlang-1.6.0/nyanlang/__init__.py
--rw-r--r--   0        0        0     1216 2023-03-29 08:52:28.005299 nyanlang-1.6.0/nyanlang/helper.py
--rw-r--r--   0        0        0    14418 2023-04-04 14:01:03.995477 nyanlang-1.6.0/nyanlang/nyan.py
--rw-r--r--   0        0        0      338 2023-04-04 13:39:21.463323 nyanlang-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 nyanlang-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-03-30 11:49:13.955098 nyanlang-1.6.1/LICENSE
+-rw-r--r--   0        0        0      529 2023-04-01 06:11:32.522384 nyanlang-1.6.1/README.md
+-rw-r--r--   0        0        0     1105 2023-04-12 08:44:48.257994 nyanlang-1.6.1/nyanlang/__init__.py
+-rw-r--r--   0        0        0     1216 2023-03-29 08:52:28.005299 nyanlang-1.6.1/nyanlang/helper.py
+-rw-r--r--   0        0        0    12610 2023-04-12 09:45:06.941720 nyanlang-1.6.1/nyanlang/nyan.py
+-rw-r--r--   0        0        0      338 2023-04-12 09:25:58.503787 nyanlang-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 nyanlang-1.6.1/PKG-INFO
```

### Comparing `nyanlang-1.6.0/LICENSE` & `nyanlang-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nyanlang-1.6.0/README.md` & `nyanlang-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nyanlang-1.6.0/nyanlang/__init__.py` & `nyanlang-1.6.1/nyanlang/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .nyan import Nyan, NyanEngine
+from .nyan import NyanInterpreter, NyanEngine
 
 from .helper import Param, ParamItem
 from .helper import Helper
 
 import sys
 import pathlib
```

### Comparing `nyanlang-1.6.0/nyanlang/helper.py` & `nyanlang-1.6.1/nyanlang/helper.py`

 * *Files identical despite different names*

### Comparing `nyanlang-1.6.0/nyanlang/nyan.py` & `nyanlang-1.6.1/nyanlang/nyan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 from pathlib import Path
 import re
 import sys
 import logging
-import time
 
 logging.basicConfig(level=logging.ERROR)
 
 _logger = logging.getLogger("NyanEngine")
 
 
 # @dataclass
@@ -55,47 +54,100 @@
             return self.nyan_b
         elif nyan == self.nyan_b:
             return self.nyan_a
         else:
             raise ValueError("Invalid nyan")
 
 
-class CommunitySignal:
-    SEND_WAKE = 0
-    RECEIVE_WAKE = 1
+class Signals:
+    PAUSE = 0
     MAIN_EOF = 2
     SUB_EOF = 3
+    KEEP_GOING = 4
 
 
-class Nyan:
-    global_custom_keywords = {}
+class Pointer:
+    def __init__(self, initial: int = None):
+        if initial is None:
+            initial = 0
+        self._v = initial
 
+    def increase(self):
+        self._v += 1
+
+    def decrease(self):
+        self._v -= 1
+
+    def set(self, value: int):
+        self._v = value
+
+    def get(self):
+        return self._v
+
+
+class Memory:
+    def __init__(self, initial: dict = None):
+        if initial is None:
+            initial = {}
+        self.memory = initial
+
+    def increase(self, pointer: Pointer):
+        self.memory[pointer.get()] = self.memory.get(pointer.get(), 0) + 1
+
+    def decrease(self, pointer: Pointer):
+        self.memory[pointer.get()] = self.memory.get(pointer.get(), 0) - 1
+
+    def set(self, pointer: Pointer, value: int):
+        self.memory[pointer.get()] = value
+
+    def get(self, pointer: Pointer):
+        return self.memory.get(pointer.get(), 0)
+
+
+class NyanInterpreter:
     def __init__(self, filename: Path, subprocess=False, debug=False):
         self.filename = filename
         if not os.path.exists(filename):
             raise FileNotFoundError(f"File \"{filename}\" not found")
         self.initialized = False
 
         self.program = None
         self.debug = debug
 
         self.cursor = 0
-        self.memory = {}
-        self.pointer = 0
-        self.module_pointer = 0
+        self.memory = Memory()
+        self.pointer = Pointer()
+        self.module_pointer = Pointer()
         self.pointing_parents = False
         self.children = {}
         self.parents = {}
 
         self.jump_points = {}
         self.next_points = {}
 
-        self.sub = subprocess
+        self.keywords = {
+            "?": lambda o: o.pointer.increase(),
+            "!": lambda o: o.pointer.decrease(),
+            "냥": lambda o: o.memory.increase(o.pointer),
+            "냐": lambda o: o.memory.decrease(o.pointer),
+            "먕": lambda o: o.module_pointer.increase(),
+            "먀": lambda o: o.module_pointer.decrease(),
+            ";": ...,
+            ":": ...,
+            ".": lambda o: print(chr(o.memory.get(o.pointer)), end=""),
+            ",": lambda o: o.memory.set(o.pointer, ord(i) if (i := sys.stdin.read(1)) else 0),
+            "뀨": lambda o: print("{"+str(o.memory.get(o.pointer))+"}", end=""),
+        }
+        self.module_write()
+        self.module_read()
+        self.module_control()
+        self.jumper_end()
+        self.jumper_start()
 
-        self._instance_custom_keywords = {}
+        self.sub = subprocess
 
     def init(self):
         self.parse_program()
         self.parse_loop_points()
         self.initialized = True
         _logger.debug(f"Nyan \"{self.filename.stem}\" initialized.")
         return self
@@ -104,20 +156,18 @@
         self.cursor = 0
         self.memory = {}
         self.pointer = 0
         self.module_pointer = 0
         self.pointing_parents = False
         _logger.debug(f"Nyan \"{self.filename.stem}\" initialized.")
 
-    def add_local_keyword(self, keyword: str, handler: callable):
-        self._instance_custom_keywords[keyword] = handler
-
-    @staticmethod
-    def add_keyword(keyword: str, handler: callable):
-        Nyan.global_custom_keywords[keyword] = handler
+    def add_keyword(self, keyword: str):
+        def wrapper(handler: callable):
+            self.keywords[keyword] = handler
+        return wrapper
 
     def add_parent(self, parent: Communicator, pos: int):
         if pos in self.parents:
             raise ValueError("Parent cat already exists")
         self.parents[pos] = parent
 
     def add_child(self, child: Communicator, pos: int):
@@ -157,256 +207,165 @@
 
     def start_of_loop(self):
         ...
 
     def end_of_loop(self):
         ...
 
-    def pointer_plus_handler(self):
-        self.pointer += 1
-
-    def pointer_minus_handler(self):
-        self.pointer -= 1
-
-    def memory_plus_handler(self):
-        self.memory[self.pointer] = self.memory.get(self.pointer, 0) + 1
-
-    def memory_minus_handler(self):
-        self.memory[self.pointer] = self.memory.get(self.pointer, 0) - 1
-
-    def module_plus_handler(self):
-        self.module_pointer += 1
-
-    def module_minus_handler(self):
-        self.module_pointer -= 1
-
-    def module_read_handler(self):
-        if self.pointing_parents:
-            if self.module_pointer in self.parents:
-                _received = self.parents[self.module_pointer].receive(self)
-                if not _received:
-                    return CommunitySignal.RECEIVE_WAKE, self.pointing_parents, self.module_pointer
-                self.memory[self.pointer] = _received
-            else:
-                raise ValueError("Parent cat does not exist")
-        else:
-            if self.module_pointer in self.children:
-                _received = self.children[self.module_pointer].receive(self)
-                if not _received:
-                    return CommunitySignal.RECEIVE_WAKE, self.pointing_parents, self.module_pointer
-                self.memory[self.pointer] = _received
+    def module_read(self):
+        def wrapper(o):
+            if o.pointing_parents:
+                if o.module_pointer.get() in o.parents:
+                    _received = o.parents[o.module_pointer.get()].receive(o)
+                    if not _received:
+                        return Signals.PAUSE, o.pointing_parents, o.module_pointer.get()
+                    o.memory.set(o.pointer, _received)
+                else:
+                    raise ValueError("Parent cat does not exist")
             else:
-                raise ValueError("Child cat does not exist")
+                if o.module_pointer.get() in o.children:
+                    _received = o.children[o.module_pointer.get()].receive(o)
+                    if not _received:
+                        return Signals.PAUSE, o.pointing_parents, o.module_pointer.get()
+                    o.memory.set(o.pointer, _received)
+                else:
+                    raise ValueError("Child cat does not exist")
+        self.add_keyword(":")(wrapper)
 
-    def module_write_handler(self):
-        if self.pointing_parents:
-            if self.module_pointer in self.parents:
-                self.parents[self.module_pointer].send(self, self.memory.get(self.pointer, 0))
-                self.cursor += 1
-                return CommunitySignal.SEND_WAKE, self.pointing_parents, self.module_pointer
-            else:
-                raise ValueError("Parent cat does not exist")
-        else:
-            if self.module_pointer in self.children:
-                self.children[self.module_pointer].send(self, self.memory.get(self.pointer, 0))
-                self.cursor += 1
-                return CommunitySignal.SEND_WAKE, self.pointing_parents, self.module_pointer
+    def module_write(self):
+        def wrapper(o):
+            if o.pointing_parents:
+                if o.module_pointer.get() in o.parents:
+                    o.parents[o.module_pointer.get()].send(o, o.memory.get(o.pointer))
+                    o.cursor += 1
+                    return Signals.PAUSE, o.pointing_parents, o.module_pointer.get()
+                else:
+                    raise ValueError("Parent cat does not exist")
             else:
-                raise ValueError("Child cat does not exist")
-
-    def std_in_handler(self):
-        self.memory[self.pointer] = ord(i) if (i := sys.stdin.read(1)) else 0
-
-    def std_out_handler(self):
-        if self.debug:
-            print("{" + str(self.memory.get(self.pointer, 0)) + "}", end="")
-        else:
-            print(chr(self.memory.get(self.pointer, 0)), end="")
+                if o.module_pointer.get() in o.children:
+                    o.children[o.module_pointer.get()].send(o, o.memory.get(o.pointer))
+                    o.cursor += 1
+                    return Signals.PAUSE, o.pointing_parents, o.module_pointer.get()
+                else:
+                    raise ValueError("Child cat does not exist")
+        self.add_keyword(";")(wrapper)
 
     def jumper_start(self):
-        if self.memory.get(self.pointer, 0) == 0:
-            self.cursor = self.next_points[self.cursor]
+        def wrapper(o):
+            if o.memory.get(o.pointer) == 0:
+                o.cursor = o.next_points[o.cursor]
+        self.add_keyword("~")(wrapper)
 
     def jumper_end(self):
-        if self.memory.get(self.pointer, 0) != 0:
-            self.cursor = self.jump_points[self.cursor]
-
-    def debug_handler(self):
-        print("{" + str(self.memory.get(self.pointer, 0)) + "}", end="")
-
-    def module_control_handler(self):
-        self.pointing_parents = not self.pointing_parents
+        def wrapper(o):
+            if o.memory.get(o.pointer) != 0:
+                o.cursor = o.jump_points[o.cursor]
+        self.add_keyword("-")(wrapper)
+
+    def module_control(self):
+        def wrapper(o):
+            o.pointing_parents = not o.pointing_parents
+        self.add_keyword("'")(wrapper)
 
     def run(self):
         self.before_run()
         while True:
             self.start_of_loop()
             char = self.program[self.cursor]
             if char == " ":
                 if not self.sub:
                     print("\n")
                 break
-            match char:
-                case "?":
-                    self.pointer_plus_handler()
-                case "!":
-                    self.pointer_minus_handler()
-                case "냥":
-                    self.memory_plus_handler()
-                case "냐":
-                    self.memory_minus_handler()
-                case "먕":
-                    self.module_plus_handler()
-                case "먀":
-                    self.module_minus_handler()
-                case ";":
-                    return self.module_write_handler()
-                case ":":
-                    _read = self.module_read_handler()
-                    if _read:
-                        return _read
-                case ".":
-                    self.std_out_handler()
-                case ",":
-                    self.std_in_handler()
-                case "~":
-                    self.jumper_start()
-                case "-":
-                    self.jumper_end()
-                case "뀨":
-                    self.debug_handler()
-                case "'":
-                    self.module_control_handler()
-                case char:
-                    if char in self._instance_custom_keywords:
-                        self._instance_custom_keywords[char]()
-                    elif char in self.global_custom_keywords:
-                        self.global_custom_keywords[char]()
-                    else:
-                        raise ValueError(f"Invalid character {char} in file {self.filename}")
+            if char in self.keywords:
+                raw_response = self.keywords[char](self)
+                if type(raw_response) == tuple:
+                    return raw_response
+            else:
+                raise SyntaxError(f"Invalid character {char}")
 
             self.cursor += 1
             self.end_of_loop()
         if self.sub:
-            return CommunitySignal.SUB_EOF, self.pointing_parents, self.module_pointer
-        return CommunitySignal.MAIN_EOF, self.pointing_parents, self.module_pointer
-
-
-class TimeSleepNyan(Nyan):
-    def __init__(self, debug=False):
-        self.filename = Path("time.sleep")
-        self.debug = debug
-        self.parents = {}
-
-    def init(self):
-        return self
-
-    def run(self):
-        for c in self.parents:
-            r = self.parents[c].receive(self)
-            if r:
-                _logger.debug(f"Sleeping for {r} ms")
-                time.sleep(r/1000)
-                return CommunitySignal.SUB_EOF, True, c
-
-
-exts = {
-    "time.sleep": TimeSleepNyan
-}
+            return Signals.SUB_EOF, self.pointing_parents, self.module_pointer
+        return Signals.MAIN_EOF, self.pointing_parents, self.module_pointer
 
 
 class NyanEngine:
     def __init__(self, root_name: str, *, debug=False):
         self.debug = debug
         if self.debug:
             logging.basicConfig(level=logging.DEBUG)
             _logger.level = logging.DEBUG
 
-        self.root = Nyan(Path(root_name).absolute(), debug=self.debug).init()
+        self.root = NyanInterpreter(Path(root_name).absolute(), debug=self.debug).init()
         self.nodetree = []
         self.references = {}
 
         self.nyans = [self.root]
 
         self.find_mouse_info()
 
-    @staticmethod
-    def add_keyword(keyword: str, handler: callable):
-        Nyan.add_keyword(keyword, handler)
-
-    def find_mouse_info(self, nyan: Nyan | None = None):
+    def find_mouse_info(self, nyan: NyanInterpreter | None = None):
         if not nyan:
             _mpath = os.path.join(self.root.filename.parent, self.root.filename.stem + ".mouse")
         else:
             _mpath = os.path.join(nyan.filename.parent, nyan.filename.stem + ".mouse")
         if not os.path.exists(_mpath):
             return
         with open(_mpath, "r", encoding="utf-8") as _f:
             for index, line in enumerate(_f.readlines()):
-                is_child_ext = False
                 mobj = re.match(r"(?P<position>-?\d+)->(?P<target_pos>-?\d+):\s*(?P<filename>.*)\n?", line)
                 if mobj:
                     try:
                         _pos = int(mobj.group("position"))
                         _tpos = int(mobj.group("target_pos"))
                     except ValueError:
                         raise ValueError(f"Invalid mouse position in line {index} - "
                                          f"{mobj.group('position')} or {mobj.group('target_pos')}")
-                    if mobj.group("filename") in exts.keys():
-                        is_child_ext = True
-                        if mobj.group("filename") not in self.references:
-                            _child = exts[mobj.group("filename")](debug=self.debug).init()
-                            self.references[mobj.group("filename")] = _child
-                        else:
-                            _child = self.references[mobj.group("filename")]
+                    new_path = Path(
+                        os.path.join(
+                            (self.root.filename.parent if not nyan else nyan.filename.parent),
+                            Path(mobj.group("filename"))
+                        )
+                    ).absolute()
+                    if new_path not in self.references:
+                        _child = NyanInterpreter(new_path, subprocess=True, debug=self.debug).init()
+                        self.references[new_path] = _child
+                        self.nyans.append(_child)
                     else:
-                        new_path = Path(
-                            os.path.join(
-                                (self.root.filename.parent if not nyan else nyan.filename.parent),
-                                Path(mobj.group("filename"))
-                            )
-                        ).absolute()
-                        if new_path not in self.references:
-                            _child = Nyan(new_path, subprocess=True, debug=self.debug).init()
-                            self.references[new_path] = _child
-                            self.nyans.append(_child)
-                        else:
-                            _child = self.references[new_path]
+                        _child = self.references[new_path]
                     if not nyan:
                         _comm = Communicator(self.root, _child)
                         self.root.add_child(_comm, _pos)
                     else:
                         _comm = Communicator(nyan, _child)
                         nyan.add_child(_comm, _pos)
                     _child.add_parent(_comm, _tpos)
-                    if not is_child_ext:
-                        self.find_mouse_info(_child)
+                    self.find_mouse_info(_child)
                 else:
                     raise SyntaxError(f"Invalid mouse info: line {index}")
 
     def run(self):
         while True:
             if not self.nodetree:
                 nyan = self.root
             else:
                 nyan = self.nodetree[-1]
             _logger.debug(f"Running {nyan.filename.stem}")
             signal, parent_mode, mouse_pointer = nyan.run()
             match signal:
-                case CommunitySignal.SEND_WAKE | CommunitySignal.RECEIVE_WAKE:
-                    _logger.debug(f"WAKE {'SEND' if signal == CommunitySignal.SEND_WAKE else 'RECEIVE'} SIGNAL SENT "
-                                  f"FROM {nyan.filename.stem}")
+                case Signals.PAUSE:
                     if parent_mode:
                         points = nyan.parents[mouse_pointer].get_nyan(nyan)
                     else:
                         points = nyan.children[mouse_pointer].get_nyan(nyan)
                     if len(self.nodetree) >= 2 and self.nodetree[-2] == points:
                         self.nodetree = self.nodetree[:-1]
                         continue
                     self.nodetree.append(points)
                     continue
-                case CommunitySignal.SUB_EOF:
+                case Signals.SUB_EOF:
                     nyan.reset()
                     self.nodetree = self.nodetree[:-1]
                     continue
-                case CommunitySignal.MAIN_EOF:
+                case Signals.MAIN_EOF:
                     return
```

### Comparing `nyanlang-1.6.0/PKG-INFO` & `nyanlang-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyanlang
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Cutest Programming Language
 Author: sserve-kr
 Author-email: personal@sserve.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nyanlang Version: 1.6.0 Summary: A Cutest
+Metadata-Version: 2.1 Name: nyanlang Version: 1.6.1 Summary: A Cutest
 Programming Language Author: sserve-kr Author-email: personal@sserve.me
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown
  [https://user-images.githubusercontent.com/61446372/228822639-f126e6a3-5bcb-
                           4e04-80ed-1cb6325314bf.png]
                              ****** ë¥ë­ ******
```

