# Comparing `tmp/peakrdl-systemrdl-0.2.0.tar.gz` & `tmp/peakrdl-systemrdl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-systemrdl-0.2.0.tar", last modified: Sun Mar 12 06:26:50 2023, max compression
+gzip compressed data, was "peakrdl-systemrdl-0.3.0.tar", last modified: Wed Apr 12 04:34:17 2023, max compression
```

## Comparing `peakrdl-systemrdl-0.2.0.tar` & `peakrdl-systemrdl-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:26:50.618251 peakrdl-systemrdl-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-12 06:26:50.618251 peakrdl-systemrdl-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 06:26:50.618251 peakrdl-systemrdl-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:26:50.614251 peakrdl-systemrdl-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:26:50.614251 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/definition_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/rdl_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-12 06:26:49.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:26:50.614251 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-12 06:26:50.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-12 06:26:50.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 06:26:50.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-12 06:26:50.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-12 06:26:50.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-12 06:26:50.000000 peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:17.772326 peakrdl-systemrdl-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-12 04:34:17.772326 peakrdl-systemrdl-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:34:17.772326 peakrdl-systemrdl-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:17.768326 peakrdl-systemrdl-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:17.772326 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/definition_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/rdl_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-12 04:34:15.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:17.772326 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-12 04:34:17.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-12 04:34:17.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:34:17.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 04:34:17.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 04:34:17.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 04:34:17.000000 peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/top_level.txt
```

### Comparing `peakrdl-systemrdl-0.2.0/LICENSE` & `peakrdl-systemrdl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-systemrdl-0.2.0/PKG-INFO` & `peakrdl-systemrdl-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-systemrdl
-Version: 0.2.0
+Version: 0.3.0
 Summary: Write a register model to a SystemRDL file
 Home-page: https://github.com/SystemRDL/PeakRDL-systemrdl
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/SystemRDL/PeakRDL-systemrdl
 Project-URL: Tracker, https://github.com/SystemRDL/PeakRDL-systemrdl/issues
```

### Comparing `peakrdl-systemrdl-0.2.0/README.md` & `peakrdl-systemrdl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl-systemrdl-0.2.0/setup.py` & `peakrdl-systemrdl-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/__peakrdl__.py` & `peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/definition_generator.py` & `peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/definition_generator.py`

 * *Files identical despite different names*

### Comparing `peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/exporter.py` & `peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/exporter.py`

 * *Files identical despite different names*

### Comparing `peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/rdl_generator.py` & `peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/rdl_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Type
 
 from systemrdl.walker import RDLListener, RDLWalker
+from systemrdl import rdltypes
 
 from .definition_generator import DefinitionGenerator
 from .stringify import stringify_rdl_value
 
 if TYPE_CHECKING:
     from systemrdl.node import AddressableNode
     from systemrdl.node import AddrmapNode, RegfileNode, RegNode, FieldNode, Node, MemNode, SignalNode
@@ -33,14 +34,29 @@
             value = node.get_property(prop_name)
             if prop_name == "reset" and isinstance(value, int):
                 continue
 
             value_s = stringify_rdl_value(value)
             self.add_content(f"{prop_name} = {value_s};")
 
+    def define_enum(self, enum: Type[rdltypes.UserEnum])-> None:
+        self.push(f"enum {enum.type_name}", "")
+        for identifier, member in enum.members.items():
+            if member.rdl_name or member.rdl_desc:
+                self.add_content(f"{identifier} = {member.value} {{")
+                if member.rdl_name:
+                    self.add_content(f"    name = {stringify_rdl_value(member.rdl_name)};")
+                if member.rdl_desc:
+                    self.add_content(f"    desc = {stringify_rdl_value(member.rdl_desc)};")
+                self.add_content("};")
+            else:
+                self.add_content(f"{identifier} = {member.value};")
+        self.pop()
+
+
     def get_addressable_assignment(self, node: 'AddressableNode') -> str:
         a = f" @ 0x{node.raw_address_offset:X}"
         if node.is_array:
             a += f" += 0x{node.array_stride:X}"
         return a
 
     def enter_Addrmap(self, node: 'AddrmapNode') -> None:
@@ -66,14 +82,19 @@
     def enter_Field(self, node: 'FieldNode') -> None:
         suffix = f"[{node.msb}:{node.lsb}]"
         reset = node.get_property('reset')
         if isinstance(reset, int):
             suffix += f" = 0x{reset:X}"
 
         self.push("field", node.inst_name, suffix=suffix, is_external=node.external)
+
+        encode = node.get_property('encode')
+        if encode is not None:
+            self.define_enum(encode)
+
         self.assign_properties(node)
 
     def enter_Signal(self, node: 'SignalNode') -> None:
         self.push("signal", node.inst_name)
         self.assign_properties(node)
 
     def exit_Component(self, node: 'Node') -> None:
```

### Comparing `peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl/stringify.py` & `peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl/stringify.py`

 * *Files identical despite different names*

### Comparing `peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/PKG-INFO` & `peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-systemrdl
-Version: 0.2.0
+Version: 0.3.0
 Summary: Write a register model to a SystemRDL file
 Home-page: https://github.com/SystemRDL/PeakRDL-systemrdl
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/SystemRDL/PeakRDL-systemrdl
 Project-URL: Tracker, https://github.com/SystemRDL/PeakRDL-systemrdl/issues
```

### Comparing `peakrdl-systemrdl-0.2.0/src/peakrdl_systemrdl.egg-info/SOURCES.txt` & `peakrdl-systemrdl-0.3.0/src/peakrdl_systemrdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

