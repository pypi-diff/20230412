# Comparing `tmp/mongomancy-0.0.4.tar.gz` & `tmp/mongomancy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.0.4.tar", last modified: Tue Apr  4 11:42:03 2023, max compression
+gzip compressed data, was "mongomancy-0.0.5.tar", last modified: Wed Apr 12 12:27:09 2023, max compression
```

## Comparing `mongomancy-0.0.4.tar` & `mongomancy-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-04 11:42:03.424055 mongomancy-0.0.4/
--rw-r--r--   0 trval     (1000) trval     (1000)      942 2023-04-04 11:41:42.000000 mongomancy-0.0.4/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.0.4/LICENSE
--rw-rw-r--   0 trval     (1000) trval     (1000)       27 2022-09-02 08:46:36.000000 mongomancy-0.0.4/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-04-04 11:42:03.424055 mongomancy-0.0.4/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.0.4/README.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1243 2022-09-02 08:41:18.000000 mongomancy-0.0.4/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.0.4/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-04-04 11:42:03.424055 mongomancy-0.0.4/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-04 11:42:03.420721 mongomancy-0.0.4/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-04 11:42:03.424055 mongomancy-0.0.4/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-04-04 11:41:42.000000 mongomancy-0.0.4/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13857 2023-04-04 08:06:59.000000 mongomancy-0.0.4/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.0.4/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)    12666 2023-04-04 11:41:42.000000 mongomancy-0.0.4/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     5687 2023-04-04 08:06:59.000000 mongomancy-0.0.4/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-04 11:42:03.424055 mongomancy-0.0.4/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-04-04 11:42:03.000000 mongomancy-0.0.4/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      411 2023-04-04 11:42:03.000000 mongomancy-0.0.4/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-04-04 11:42:03.000000 mongomancy-0.0.4/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-04-04 11:42:03.000000 mongomancy-0.0.4/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-04-04 11:42:03.000000 mongomancy-0.0.4/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.646882 mongomancy-0.0.5/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1027 2023-04-12 12:22:43.000000 mongomancy-0.0.5/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.0.5/LICENSE
+-rw-rw-r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:09:27.000000 mongomancy-0.0.5/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-04-12 12:27:09.646882 mongomancy-0.0.5/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.0.5/README.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:26:56.000000 mongomancy-0.0.5/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.0.5/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-04-12 12:27:09.646882 mongomancy-0.0.5/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.643549 mongomancy-0.0.5/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.643549 mongomancy-0.0.5/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-04-12 12:22:43.000000 mongomancy-0.0.5/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    13857 2023-04-04 08:06:59.000000 mongomancy-0.0.5/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.0.5/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:06:01.000000 mongomancy-0.0.5/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    12666 2023-04-04 11:41:42.000000 mongomancy-0.0.5/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     5687 2023-04-04 08:06:59.000000 mongomancy-0.0.5/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-12 12:27:09.646882 mongomancy-0.0.5/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-04-12 12:27:09.000000 mongomancy-0.0.5/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.0.4/CHANGELOG.md` & `mongomancy-0.0.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.0.5] - 2023-04-12
+
+### Added
+
+- Include `py.typed` for python typing support.
+
 ## [0.0.4] - 2023-04-04
 
 ### Fixed
 
 - Collection aggregate return type set to pymongo CommandCursor.
 
 ## [0.0.3] - 2023-04-04
```

### Comparing `mongomancy-0.0.4/CONTRIBUTING.md` & `mongomancy-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.4/LICENSE` & `mongomancy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.4/PKG-INFO` & `mongomancy-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.0.4/README.md` & `mongomancy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.4/pyproject.toml` & `mongomancy-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -37,19 +37,29 @@
 "Bug Tracker" = "https://github.com/Ryu-CZ/mongomancy/issues"
 
 [options]
 test_suite = "tests"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
-packages = ["mongomancy", ]
+packages = [
+    "mongomancy",
+]
+
+
+[tool.setuptools.package-data]
+"mongomancy" = ["py.typed"]
 
 [tool.setuptools.dynamic]
 version = {attr = "mongomancy.__version__"}
 
+[tool.black]
+line_length = 120
+target_version = ["py310"]
+
 [coverage.run]
 branch = true
 source = [
     "src/mongomancy",
     "tests",
 ]
```

### Comparing `mongomancy-0.0.4/src/mongomancy/engine.py` & `mongomancy-0.0.5/src/mongomancy/engine.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.4/src/mongomancy/mongo_errors.py` & `mongomancy-0.0.5/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.4/src/mongomancy/schema.py` & `mongomancy-0.0.5/src/mongomancy/schema.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.4/src/mongomancy/types.py` & `mongomancy-0.0.5/src/mongomancy/types.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.4/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.0.5/src/mongomancy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

