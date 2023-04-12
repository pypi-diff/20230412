# Comparing `tmp/labelf-api-0.1.0.tar.gz` & `tmp/labelf-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelf-api-0.1.0.tar", last modified: Wed Apr 12 15:28:45 2023, max compression
+gzip compressed data, was "labelf-api-0.1.1.tar", last modified: Wed Apr 12 20:00:46 2023, max compression
```

## Comparing `labelf-api-0.1.0.tar` & `labelf-api-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 15:28:45.629266 labelf-api-0.1.0/
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      615 2023-04-12 15:28:45.629266 labelf-api-0.1.0/PKG-INFO
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      878 2023-04-12 14:18:21.000000 labelf-api-0.1.0/README.md
-drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 15:28:45.629266 labelf-api-0.1.0/labelf_api/
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      231 2023-04-12 14:20:13.000000 labelf-api-0.1.0/labelf_api/__init__.py
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)     2830 2023-04-12 15:03:44.000000 labelf-api-0.1.0/labelf_api/client.py
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      247 2023-04-12 13:16:30.000000 labelf-api-0.1.0/labelf_api/exceptions.py
-drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 15:28:45.629266 labelf-api-0.1.0/labelf_api.egg-info/
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      615 2023-04-12 15:28:45.000000 labelf-api-0.1.0/labelf_api.egg-info/PKG-INFO
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      320 2023-04-12 15:28:45.000000 labelf-api-0.1.0/labelf_api.egg-info/SOURCES.txt
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)        1 2023-04-12 15:28:45.000000 labelf-api-0.1.0/labelf_api.egg-info/dependency_links.txt
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)       24 2023-04-12 15:28:45.000000 labelf-api-0.1.0/labelf_api.egg-info/requires.txt
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)       17 2023-04-12 15:28:45.000000 labelf-api-0.1.0/labelf_api.egg-info/top_level.txt
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)       59 2023-04-12 15:27:53.000000 labelf-api-0.1.0/pyproject.toml
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      698 2023-04-12 15:28:45.633266 labelf-api-0.1.0/setup.cfg
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      627 2023-04-12 14:18:19.000000 labelf-api-0.1.0/setup.py
-drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 15:28:45.629266 labelf-api-0.1.0/tests/
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 13:10:10.000000 labelf-api-0.1.0/tests/__init__.py
--rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      982 2023-04-12 14:18:17.000000 labelf-api-0.1.0/tests/test_client.py
+drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 20:00:46.483469 labelf-api-0.1.1/
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      666 2023-04-12 20:00:46.483469 labelf-api-0.1.1/PKG-INFO
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      878 2023-04-12 14:18:21.000000 labelf-api-0.1.1/README.md
+drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 20:00:46.483469 labelf-api-0.1.1/labelf_api/
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      231 2023-04-12 14:20:13.000000 labelf-api-0.1.1/labelf_api/__init__.py
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)     7344 2023-04-12 19:53:47.000000 labelf-api-0.1.1/labelf_api/client.py
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      247 2023-04-12 13:16:30.000000 labelf-api-0.1.1/labelf_api/exceptions.py
+drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 20:00:46.483469 labelf-api-0.1.1/labelf_api.egg-info/
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      666 2023-04-12 20:00:46.000000 labelf-api-0.1.1/labelf_api.egg-info/PKG-INFO
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      311 2023-04-12 20:00:46.000000 labelf-api-0.1.1/labelf_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)        1 2023-04-12 20:00:46.000000 labelf-api-0.1.1/labelf_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)       24 2023-04-12 20:00:46.000000 labelf-api-0.1.1/labelf_api.egg-info/requires.txt
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)       17 2023-04-12 20:00:46.000000 labelf-api-0.1.1/labelf_api.egg-info/top_level.txt
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)       59 2023-04-12 15:27:53.000000 labelf-api-0.1.1/pyproject.toml
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      698 2023-04-12 20:00:46.483469 labelf-api-0.1.1/setup.cfg
+drwxrwxr-x   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 20:00:46.483469 labelf-api-0.1.1/tests/
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)        0 2023-04-12 13:10:10.000000 labelf-api-0.1.1/tests/__init__.py
+-rw-rw-r--   0 viktoralm  (1000) viktoralm  (1000)      982 2023-04-12 14:18:17.000000 labelf-api-0.1.1/tests/test_client.py
```

### Comparing `labelf-api-0.1.0/PKG-INFO` & `labelf-api-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: labelf-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for interacting with the Labelf API
 Author: Viktor Alm
 Author-email: viktor@labelf.ai
 License: MIT
 Keywords: labelf,api,client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: test
```

### Comparing `labelf-api-0.1.0/README.md` & `labelf-api-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `labelf-api-0.1.0/labelf_api.egg-info/PKG-INFO` & `labelf-api-0.1.1/labelf_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: labelf-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for interacting with the Labelf API
 Author: Viktor Alm
 Author-email: viktor@labelf.ai
 License: MIT
 Keywords: labelf,api,client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: test
```

### Comparing `labelf-api-0.1.0/setup.cfg` & `labelf-api-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = labelf-api
-version = 0.1.0
+version = 0.1.1
 description = A Python package for interacting with the Labelf API
 author = Viktor Alm
 author_email = viktor@labelf.ai
 license = MIT
 keywords = labelf, api, client
 classifiers = 
 	Development Status :: 3 - Alpha
```

### Comparing `labelf-api-0.1.0/tests/test_client.py` & `labelf-api-0.1.1/tests/test_client.py`

 * *Files identical despite different names*

