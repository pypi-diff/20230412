# Comparing `tmp/RXL-0.0.2.tar.gz` & `tmp/RXL-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RXL-0.0.2.tar", last modified: Mon Apr 10 19:45:53 2023, max compression
+gzip compressed data, was "RXL-0.0.3.tar", last modified: Tue Apr 11 23:09:52 2023, max compression
```

## Comparing `RXL-0.0.2.tar` & `RXL-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 19:45:53.077176 RXL-0.0.2/
--rw-rw-rw-   0        0        0     7815 2022-12-20 17:30:11.000000 RXL-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      350 2023-04-10 19:45:53.074614 RXL-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-10 19:45:27.000000 RXL-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 19:45:53.063930 RXL-0.0.2/RXL/
--rw-rw-rw-   0        0        0     3629 2023-04-09 19:38:27.000000 RXL-0.0.2/RXL/Errors.py
--rw-rw-rw-   0        0        0    32483 2023-04-09 19:38:27.000000 RXL-0.0.2/RXL/Grammar.py
--rw-rw-rw-   0        0        0    19597 2023-04-09 19:38:27.000000 RXL-0.0.2/RXL/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:45:53.073617 RXL-0.0.2/RXL.egg-info/
--rw-rw-rw-   0        0        0      350 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 19:45:53.077176 RXL-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-04-10 19:45:01.000000 RXL-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:09:52.902279 RXL-0.0.3/
+-rw-rw-rw-   0        0        0     7815 2022-12-20 17:30:11.000000 RXL-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-04-11 23:09:52.900247 RXL-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-10 19:45:27.000000 RXL-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 23:09:52.877237 RXL-0.0.3/RXL/
+-rw-rw-rw-   0        0        0     3632 2023-04-11 22:42:18.000000 RXL-0.0.3/RXL/Errors.py
+-rw-rw-rw-   0        0        0    32539 2023-04-11 23:00:13.000000 RXL-0.0.3/RXL/Grammar.py
+-rw-rw-rw-   0        0        0    19603 2023-04-11 22:45:21.000000 RXL-0.0.3/RXL/Lib.py
+-rw-rw-rw-   0        0        0    10491 2023-04-11 23:07:12.000000 RXL-0.0.3/RXL/RXL.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 22:34:21.000000 RXL-0.0.3/RXL/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:09:52.888207 RXL-0.0.3/RXL.egg-info/
+-rw-rw-rw-   0        0        0      334 2023-04-11 23:09:52.000000 RXL-0.0.3/RXL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-11 23:09:52.000000 RXL-0.0.3/RXL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 23:09:52.000000 RXL-0.0.3/RXL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-11 23:09:52.000000 RXL-0.0.3/RXL.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-04-11 23:09:52.000000 RXL-0.0.3/RXL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 23:09:52.902279 RXL-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-11 23:09:50.000000 RXL-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:09:52.889205 RXL-0.0.3/tests/
+-rw-rw-rw-   0        0        0       22 2023-04-11 22:49:41.000000 RXL-0.0.3/tests/test.py
```

### Comparing `RXL-0.0.2/LICENSE` & `RXL-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RXL-0.0.2/RXL/Errors.py` & `RXL-0.0.3/RXL/Errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from . import *
+from .lib import *
 
 Error = rx.style.log_error
 
 
 
 #< List of all errors >#
 class RaiseError(Exception):
```

### Comparing `RXL-0.0.2/RXL/Grammar.py` & `RXL-0.0.3/RXL/Grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from . import *
+from .lib import *
 from . import Errors as ERRORS
 
 CLASSES = (
            ['Files'   , 'System', 'Random'    , 'Record', 'Style'   ,
             'Terminal', 'Tuple' , 'Decorator' , 'IO'    , 'Internet',
             'Date_Time'],
            ['files'   , 'system', 'random'    , 'record', 'style'   ,
@@ -253,15 +253,16 @@
     STRING.append(f"std = rx = {MODULE_SHORTCUT};std.RXL = __import__('RXL')")
     STRING.append(f"print = {MODULE_SHORTCUT+'.style.print' if PRINT_TYPE=='stylized' else 'print'}")
     #] Direct Attributes
     STRING.append(F"input = {MODULE_SHORTCUT}.Input")
     STRING.append(f"Check_Type = {MODULE_SHORTCUT}.Check_Type")
     #] Other ones
     if not map_defd:
-        STRING.append("apply = __builtins__['map'] ; map = None")
+        # STRING.append("apply = __builtins__['map'] ; map = None")
+        STRING.append("apply = map ; map = None")
     for key,value in INFO.items():
         STRING.append(f"setattr(std,'{key}','{value}')")
 
     if len(Changeable):
         for line in Changeable:
             if line == Changeable[-1]:
                 SOURCE[line] = ';'.join(STRING)
```

### Comparing `RXL-0.0.2/RXL/__init__.py` & `RXL-0.0.3/RXL/Lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 def convert_file_name(file):
     return '_'+os.path.basename(file)+'_'
     #'‎'+FILE+'‎' THERE IS INVISIBLE CHAR IN QUOTES
 
 
+
 class rx:
     @staticmethod
     def cls():
         os.system('cls')
 
 
     class record:
@@ -36,16 +37,16 @@
             return (self.lap(False)-self.laps[-1]) if self.laps else self.lap(False)
     Record = record
 
 
     class Terminal:
         run = os.system
         getoutput = __import__('subprocess').getoutput
-        set_title = __import__('win32api').SetConsoleTitle
-        get_title = __import__('win32api').GetConsoleTitle
+        # set_title = __import__('win32api').SetConsoleTitle
+        # get_title = __import__('win32api').GetConsoleTitle
     terminal = Terminal
 
 
     class style:
         def __init__(self,text,color='default',BG='black'):
             try:
                 color= color.lower()
```

### Comparing `RXL-0.0.2/setup.py` & `RXL-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_descriptions = fh.read()
 
 s = setup(
     name = "RXL",
-    version = "0.0.2",
-    license = "LGPL",
     description = "RXL Features",
-    url = "https://github.com/Ramin-RX7/RX-Language/tree/master/RXL/",
+    version = "0.0.3",
+    license = "LGPL",
+    url = "https://github.com/Ramin-RX7/RX-Language/",
+    author = "Ramin RX7",
+    author_email = "rawmin.rx@gmail.com",
+
     packages = find_packages(),
     install_requires = [],
     python_requires = ">= 3.8",
-    author = "Ramin RX7",
-    author_email = "rawmin.rx@gmail.com",
+
     classifiers = [
         'Programming Language :: Python :: 3',
     ],
+
     long_description = long_descriptions,
     long_description_content_type = "text/markdown",
-    )
+
+    entry_points={
+        'console_scripts': [
+            'RXL = RXL.RXL:main',
+        ],
+    },
+)
```

