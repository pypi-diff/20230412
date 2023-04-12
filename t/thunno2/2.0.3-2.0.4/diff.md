# Comparing `tmp/thunno2-2.0.3.tar.gz` & `tmp/thunno2-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.0.3.tar", last modified: Wed Apr 12 10:07:26 2023, max compression
+gzip compressed data, was "thunno2-2.0.4.tar", last modified: Wed Apr 12 13:46:20 2023, max compression
```

## Comparing `thunno2-2.0.3.tar` & `thunno2-2.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 10:07:26.799659 thunno2-2.0.3/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 10:07:26.799519 thunno2-2.0.3/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-12 10:07:26.799701 thunno2-2.0.3/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.3/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 10:07:26.798676 thunno2-2.0.3/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.3/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.3/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    39327 2023-04-11 16:50:16.000000 thunno2-2.0.3/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.3/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   244557 2023-04-08 16:04:36.000000 thunno2-2.0.3/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     2896 2023-04-12 09:58:27.000000 thunno2-2.0.3/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    40904 2023-04-11 19:11:59.000000 thunno2-2.0.3/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    18356 2023-04-11 14:03:07.000000 thunno2-2.0.3/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    14374 2023-04-11 14:03:07.000000 thunno2-2.0.3/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:05:20.000000 thunno2-2.0.3/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    55521 2023-04-11 17:00:38.000000 thunno2-2.0.3/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.3/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-12 10:06:44.000000 thunno2-2.0.3/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 10:07:26.799255 thunno2-2.0.3/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 13:46:20.327935 thunno2-2.0.4/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 13:46:20.327818 thunno2-2.0.4/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-12 13:46:20.327971 thunno2-2.0.4/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.4/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 13:46:20.327125 thunno2-2.0.4/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.4/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.4/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    39327 2023-04-11 16:50:16.000000 thunno2-2.0.4/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.4/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   244557 2023-04-08 16:04:36.000000 thunno2-2.0.4/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4239 2023-04-12 13:31:45.000000 thunno2-2.0.4/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    40904 2023-04-11 19:11:59.000000 thunno2-2.0.4/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    18356 2023-04-11 14:03:07.000000 thunno2-2.0.4/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    14374 2023-04-11 14:03:07.000000 thunno2-2.0.4/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.4/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    55521 2023-04-11 17:00:38.000000 thunno2-2.0.4/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.4/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-12 13:33:49.000000 thunno2-2.0.4/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 13:46:20.327650 thunno2-2.0.4/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 13:46:20.000000 thunno2-2.0.4/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-12 13:46:20.000000 thunno2-2.0.4/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-12 13:46:20.000000 thunno2-2.0.4/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-12 13:46:20.000000 thunno2-2.0.4/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-12 13:46:20.000000 thunno2-2.0.4/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.0.3/PKG-INFO` & `thunno2-2.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.3
+Version: 2.0.4
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.3.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.4.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.0.3/setup.py` & `thunno2-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/codepage.py` & `thunno2-2.0.4/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/commands.py` & `thunno2-2.0.4/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/constants.py` & `thunno2-2.0.4/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/dictionary.py` & `thunno2-2.0.4/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/flags.py` & `thunno2-2.0.4/thunno2/flags.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 from thunno2 import interpreter, commands, helpers
 
 
 def process_input_flags(flags, inputs):
 
+    if 'w' in flags:
+        commands.ctx.warnings = True
+
     if 'W' in flags:
         inputs = [inputs]
     else:
         inputs = inputs.splitlines()
 
     if 'E' not in flags:
         new_input = []
         for inp in inputs:
             try:
-                new_input.append(eval(inp))
+                x = eval(inp)
+                if type(x) in (int, float, str, list):
+                    new_input.append(x)
+                elif isinstance(x, bool):
+                    new_input.append(int(x))
+                elif isinstance(x, (set, tuple)):
+                    new_input.append(list(x))
+                elif isinstance(x, dict):
+                    new_input.append(list(map(list, x.items())))
+                else:
+                    new_input.append(inp)
             except:
                 new_input.append(inp)
         inputs = new_input[:]
 
     for flag in flags:
         if flag == 'Z':
             commands.ctx.stack.push(0)
@@ -85,17 +98,42 @@
 
         if 'L' == flag:
             commands.ctx.stack.push(commands.commands['l']()[0])
 
         if 'l' == flag:
             commands.ctx.stack.push(len(commands.ctx.stack))
 
+        if 'h' == flag:
+            commands.ctx.stack.push(commands.commands['h']()[0])
+
+        if 't' == flag:
+            commands.ctx.stack.push(commands.commands['t']()[0])
+
     if (commands.ctx.implicit_print or ('O' in flags)) and not ('o' in flags):
         print(next(commands.ctx.stack.rmv(1)))
 
 
 def run(flags, code, inputs):
+
+    if 'V' in flags:
+        new_flags = ''.join(f for f in flags if f != 'V')
+        for line in inputs:
+            try:
+                x = eval(line)
+                if isinstance(x, tuple):
+                    new_inputs = process_input_flags(new_flags, '\n'.join(map(repr, x)))
+                else:
+                    new_inputs = [x]
+            except:
+                new_inputs = [line]
+            commands.ctx.og_input_list = new_inputs.copy()
+            commands.ctx.other_il = new_inputs.copy()
+            print(line, '--> ')
+            interpreter.run(code, n=0, iteration_index=0)
+            process_output_flags(new_flags)
+        return None
+
     inputs = process_input_flags(flags, inputs)
     commands.ctx.og_input_list = inputs.copy()
     commands.ctx.other_il = inputs.copy()
     interpreter.run(code, n=0, iteration_index=0)
     process_output_flags(flags)
```

### Comparing `thunno2-2.0.3/thunno2/helpers.py` & `thunno2-2.0.4/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/interpreter.py` & `thunno2-2.0.4/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/lexer.py` & `thunno2-2.0.4/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/run.py` & `thunno2-2.0.4/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/tests.py` & `thunno2-2.0.4/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2/tokens.py` & `thunno2-2.0.4/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.3/thunno2.egg-info/PKG-INFO` & `thunno2-2.0.4/thunno2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.3
+Version: 2.0.4
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.3.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.4.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

