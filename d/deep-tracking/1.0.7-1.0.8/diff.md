# Comparing `tmp/deep_tracking-1.0.7.tar.gz` & `tmp/deep_tracking-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_tracking-1.0.7.tar", last modified: Tue Apr 11 23:40:55 2023, max compression
+gzip compressed data, was "deep_tracking-1.0.8.tar", last modified: Tue Apr 11 23:50:49 2023, max compression
```

## Comparing `deep_tracking-1.0.7.tar` & `deep_tracking-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:40:55.389616 deep_tracking-1.0.7/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.7/LICENSE.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:40:55.389616 deep_tracking-1.0.7/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.7/README.md
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:40:55.385615 deep_tracking-1.0.7/deep_tracking/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 20:24:32.000000 deep_tracking-1.0.7/deep_tracking/__init__.py
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)    10182 2023-04-11 23:40:14.000000 deep_tracking-1.0.7/deep_tracking/deep_tracking.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:40:55.389616 deep_tracking-1.0.7/deep_tracking.egg-info/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:40:55.000000 deep_tracking-1.0.7/deep_tracking.egg-info/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-11 23:40:55.000000 deep_tracking-1.0.7/deep_tracking.egg-info/SOURCES.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 23:40:55.000000 deep_tracking-1.0.7/deep_tracking.egg-info/dependency_links.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:40:55.000000 deep_tracking-1.0.7/deep_tracking.egg-info/requires.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:40:55.000000 deep_tracking-1.0.7/deep_tracking.egg-info/top_level.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 23:40:55.389616 deep_tracking-1.0.7/setup.cfg
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      773 2023-04-11 23:40:40.000000 deep_tracking-1.0.7/setup.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.8/LICENSE.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.8/README.md
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:50:49.450373 deep_tracking-1.0.8/deep_tracking/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 20:24:32.000000 deep_tracking-1.0.8/deep_tracking/__init__.py
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)    10283 2023-04-11 23:50:32.000000 deep_tracking-1.0.8/deep_tracking/deep_tracking.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/deep_tracking.egg-info/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/SOURCES.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/dependency_links.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/requires.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/top_level.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/setup.cfg
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      773 2023-04-11 23:50:39.000000 deep_tracking-1.0.8/setup.py
```

### Comparing `deep_tracking-1.0.7/LICENSE.txt` & `deep_tracking-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deep_tracking-1.0.7/PKG-INFO` & `deep_tracking-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_tracking
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deep_tracking-1.0.7/deep_tracking/deep_tracking.py` & `deep_tracking-1.0.8/deep_tracking/deep_tracking.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,39 +2,14 @@
 import inspect
 import pickle
 import os.path
 from IPython.display import clear_output
 import zipfile
 import sys
 
-class Process:
-    def __init__(self, scope, action, function, description, tracked):
-        self.update(scope, action, function, description, tracked)
-        
-    def run(self, data):
-        # get globals of the main
-        current_frame = sys._getframe()
-        name = current_frame.f_globals['__name__']
-        while name != '__main__':
-            current_frame = current_frame.f_back
-            name = current_frame.f_globals['__name__']
-
-        data = data.copy()
-        local = {}
-        exec(self.function, current_frame.f_globals, local)
-        function = list(local.values())[0]        
-        return function(data)
-    
-    def update(self, scope, action, function, description, tracked):
-        self.scope = scope
-        self.action = action
-        self.function = inspect.getsource(function) 
-        self.description = description
-        self.tracked = tracked
-
 class Tracker: 
     
     def __init__(self, data=None):
         self.__last_consolidated = -1
         self.__processes = []
         self.__backups = {}
         self.__data = data
@@ -105,15 +80,15 @@
             return False
         return True
 
     def add_process(self, scope, action, function, description, tracked=True):
         if self.process_exists(scope, action):
             self.update_process(scope, action, function, description, tracked)
         else:
-            process = Process(scope, action, function, description, tracked)
+            process = self.Process(scope, action, function, description, tracked)
             self.__processes.append(process)
             self.consolidate()
         return None
     
     def update_process(self, scope, action, function, description, tracked=True):
         order = self.get_process_order(scope, action)
         already_consolidated = self.__last_consolidated >= order
@@ -237,8 +212,33 @@
             
         backups_list = [key for key in self.__backups.keys() if eval(f'key {method} {order}')]
         if backups_list:
             if method in ('=','<=', '<'):
                 return max(backups_list)
             else:
                 return min(backups_list)
-        return None
+        return None
+    
+    class Process:
+        def __init__(self, scope, action, function, description, tracked):
+            self.update(scope, action, function, description, tracked)
+            
+        def run(self, data):
+            # get globals of the main
+            current_frame = sys._getframe()
+            name = current_frame.f_globals['__name__']
+            while name != '__main__':
+                current_frame = current_frame.f_back
+                name = current_frame.f_globals['__name__']
+
+            data = data.copy()
+            local = {}
+            exec(self.function, current_frame.f_globals, local)
+            function = list(local.values())[0]        
+            return function(data)
+        
+        def update(self, scope, action, function, description, tracked):
+            self.scope = scope
+            self.action = action
+            self.function = inspect.getsource(function) 
+            self.description = description
+            self.tracked = tracked
```

### Comparing `deep_tracking-1.0.7/deep_tracking.egg-info/PKG-INFO` & `deep_tracking-1.0.8/deep_tracking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-tracking
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deep_tracking-1.0.7/setup.py` & `deep_tracking-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='deep_tracking',
-    version='1.0.7',
+    version='1.0.8',
     description='Library to track the development of data science works using the DE&P method',
     long_description = 'Library to track the development of data science works using the DE&P method',
     author='Gabriel Nuernberg Biazoto',
     author_email='biazotogabriel@gmail.com',
     url='https://github.com/biazotogabriel/deep_tracking',
     packages=['deep_tracking'],
     license = 'MIT',
```

