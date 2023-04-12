# Comparing `tmp/rigorous_recorder-1.3.1.tar.gz` & `tmp/rigorous_recorder-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigorous_recorder-1.3.1.tar", last modified: Wed Apr 12 13:55:06 2023, max compression
+gzip compressed data, was "rigorous_recorder-1.3.2.tar", last modified: Wed Apr 12 13:57:53 2023, max compression
```

## Comparing `rigorous_recorder-1.3.1.tar` & `rigorous_recorder-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:55:06.052296 rigorous_recorder-1.3.1/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:55:06.052157 rigorous_recorder-1.3.1/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:55:06.051372 rigorous_recorder-1.3.1/rigorous_recorder/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       36 2023-03-19 13:33:17.000000 rigorous_recorder-1.3.1/rigorous_recorder/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    34454 2023-03-19 14:29:57.000000 rigorous_recorder-1.3.1/rigorous_recorder/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:55:06.051996 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      268 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       59 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-12 13:55:06.052337 rigorous_recorder-1.3.1/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-03-19 13:50:47.000000 rigorous_recorder-1.3.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:57:53.680174 rigorous_recorder-1.3.2/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:57:53.680045 rigorous_recorder-1.3.2/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:57:53.679099 rigorous_recorder-1.3.2/rigorous_recorder/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       36 2023-03-19 13:33:17.000000 rigorous_recorder-1.3.2/rigorous_recorder/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    34494 2023-04-12 13:57:30.000000 rigorous_recorder-1.3.2/rigorous_recorder/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:57:53.679861 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      268 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       59 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-12 13:57:53.680215 rigorous_recorder-1.3.2/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-03-19 13:50:47.000000 rigorous_recorder-1.3.2/setup.py
```

### Comparing `rigorous_recorder-1.3.1/PKG-INFO` & `rigorous_recorder-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous_recorder
-Version: 1.3.1
+Version: 1.3.2
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.3.1/rigorous_recorder/main.py` & `rigorous_recorder-1.3.2/rigorous_recorder/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,18 +660,19 @@
         # fallback case first
         representer = attempt(lambda: indent(representer.__repr__()), default=self.local_data)
         # ideal case
         representer = attempt(lambda: indent(json.dumps(self.local_data, indent=4)), default=representer)
         # parent data
         all_parents = []
         parent_data = "    {"
-        for each_key, each_value in self.parent.items():
-            parent_data += f'\n        "{each_key}":' + indent(
-                attempt(lambda: json.dumps(each_value, indent=4), default=f"{each_value}")
-            )
+        if self.parent:
+            for each_key, each_value in self.parent.items():
+                parent_data += f'\n        "{each_key}":' + indent(
+                    attempt(lambda: json.dumps(each_value, indent=4), default=f"{each_value}")
+                )
         parent_data += "\n    }"
         
         return f"""{'{'}\n    number_of_records: {size},\n    records: [ ... ],\n    local_data: {representer},\n    parent_data:{parent_data}\n{'}'}"""
     
     def __getitem__(self, key):
         # numerical acts like array of local records 
         if isinstance(key, (int, slice)):
```

### Comparing `rigorous_recorder-1.3.1/rigorous_recorder.egg-info/PKG-INFO` & `rigorous_recorder-1.3.2/rigorous_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous-recorder
-Version: 1.3.1
+Version: 1.3.2
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.3.1/setup.py` & `rigorous_recorder-1.3.2/setup.py`

 * *Files identical despite different names*

