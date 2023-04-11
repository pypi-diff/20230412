# Comparing `tmp/deep_tracking-1.0.4.tar.gz` & `tmp/deep_tracking-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_tracking-1.0.4.tar", last modified: Tue Apr 11 20:18:25 2023, max compression
+gzip compressed data, was "deep_tracking-1.0.5.tar", last modified: Tue Apr 11 23:31:36 2023, max compression
```

## Comparing `deep_tracking-1.0.4.tar` & `deep_tracking-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 20:18:25.956632 deep_tracking-1.0.4/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.4/LICENCE.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 20:18:25.956632 deep_tracking-1.0.4/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.4/README.md
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 20:18:25.952632 deep_tracking-1.0.4/deep_tracking/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 20:09:29.000000 deep_tracking-1.0.4/deep_tracking/__init__.py
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     9923 2023-04-11 19:54:01.000000 deep_tracking-1.0.4/deep_tracking/deep_tracking.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 20:18:25.952632 deep_tracking-1.0.4/deep_tracking.egg-info/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 20:18:25.000000 deep_tracking-1.0.4/deep_tracking.egg-info/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-11 20:18:25.000000 deep_tracking-1.0.4/deep_tracking.egg-info/SOURCES.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 20:18:25.000000 deep_tracking-1.0.4/deep_tracking.egg-info/dependency_links.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 20:18:25.000000 deep_tracking-1.0.4/deep_tracking.egg-info/requires.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 20:18:25.000000 deep_tracking-1.0.4/deep_tracking.egg-info/top_level.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 20:18:25.956632 deep_tracking-1.0.4/setup.cfg
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      773 2023-04-11 20:18:20.000000 deep_tracking-1.0.4/setup.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:31:36.526833 deep_tracking-1.0.5/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.5/LICENSE.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:31:36.526833 deep_tracking-1.0.5/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.5/README.md
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:31:36.522832 deep_tracking-1.0.5/deep_tracking/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 20:24:32.000000 deep_tracking-1.0.5/deep_tracking/__init__.py
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)    10202 2023-04-11 23:29:32.000000 deep_tracking-1.0.5/deep_tracking/deep_tracking.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:31:36.526833 deep_tracking-1.0.5/deep_tracking.egg-info/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:31:36.000000 deep_tracking-1.0.5/deep_tracking.egg-info/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-11 23:31:36.000000 deep_tracking-1.0.5/deep_tracking.egg-info/SOURCES.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 23:31:36.000000 deep_tracking-1.0.5/deep_tracking.egg-info/dependency_links.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:31:36.000000 deep_tracking-1.0.5/deep_tracking.egg-info/requires.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:31:36.000000 deep_tracking-1.0.5/deep_tracking.egg-info/top_level.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 23:31:36.526833 deep_tracking-1.0.5/setup.cfg
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      773 2023-04-11 23:31:22.000000 deep_tracking-1.0.5/setup.py
```

### Comparing `deep_tracking-1.0.4/LICENCE.txt` & `deep_tracking-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deep_tracking-1.0.4/PKG-INFO` & `deep_tracking-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep_tracking
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
-License-File: LICENCE.txt
+License-File: LICENSE.txt
 
 Library to track the development of data science works using the DE&P method
```

### Comparing `deep_tracking-1.0.4/deep_tracking/deep_tracking.py` & `deep_tracking-1.0.5/deep_tracking/deep_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import pandas as pd
 import inspect
 import pickle
 import os.path
 from IPython.display import clear_output
 import zipfile
-import io
+import sys
 
 class Process:
     def __init__(self, scope, action, function, description, tracked):
         self.update(scope, action, function, description, tracked)
         
     def run(self, data):
+        # get globals of the main
+        current_frame = sys._getframe()
+        name = current_frame.f_globals['__name__']
+        while name != '__main__':
+            current_frame = current_frame.f_back
+            name = current_frame.f_globals['__name__']
+
         data = data.copy()
         local = {}
-        exec(self.function, globals(), local)
+        exec(self.function, current_frame.f_globals, local)
         function = list(local.values())[0]        
         return function(data)
     
     def update(self, scope, action, function, description, tracked):
         self.scope = scope
         self.action = action
         self.function = inspect.getsource(function)
```

### Comparing `deep_tracking-1.0.4/deep_tracking.egg-info/PKG-INFO` & `deep_tracking-1.0.5/deep_tracking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep-tracking
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
-License-File: LICENCE.txt
+License-File: LICENSE.txt
 
 Library to track the development of data science works using the DE&P method
```

### Comparing `deep_tracking-1.0.4/setup.py` & `deep_tracking-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='deep_tracking',
-    version='1.0.4',
+    version='1.0.5',
     description='Library to track the development of data science works using the DE&P method',
     long_description = 'Library to track the development of data science works using the DE&P method',
     author='Gabriel Nuernberg Biazoto',
     author_email='biazotogabriel@gmail.com',
     url='https://github.com/biazotogabriel/deep_tracking',
     packages=['deep_tracking'],
     license = 'MIT',
```

