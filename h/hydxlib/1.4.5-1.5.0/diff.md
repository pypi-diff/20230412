# Comparing `tmp/hydxlib-1.4.5.tar.gz` & `tmp/hydxlib-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydxlib-1.4.5.tar", last modified: Fri Mar 31 11:58:22 2023, max compression
+gzip compressed data, was "hydxlib-1.5.0.tar", last modified: Wed Apr 12 07:20:37 2023, max compression
```

## Comparing `hydxlib-1.4.5.tar` & `hydxlib-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:58:22.565195 hydxlib-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-03-31 11:58:19.000000 hydxlib-1.4.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-31 11:58:19.000000 hydxlib-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-31 11:58:19.000000 hydxlib-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-31 11:58:22.565195 hydxlib-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-31 11:58:19.000000 hydxlib-1.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:58:22.565195 hydxlib-1.4.5/hydxlib/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/hydx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:58:22.565195 hydxlib-1.4.5/hydxlib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/tests/test_hydx.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/tests/test_threedi.py
--rw-r--r--   0 runner    (1001) docker     (123)    31610 2023-03-31 11:58:19.000000 hydxlib-1.4.5/hydxlib/threedi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:58:22.565195 hydxlib-1.4.5/hydxlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-31 11:58:22.000000 hydxlib-1.4.5/hydxlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-31 11:58:22.000000 hydxlib-1.4.5/hydxlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:58:22.000000 hydxlib-1.4.5/hydxlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-31 11:58:22.000000 hydxlib-1.4.5/hydxlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:58:22.000000 hydxlib-1.4.5/hydxlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-31 11:58:22.000000 hydxlib-1.4.5/hydxlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 11:58:22.000000 hydxlib-1.4.5/hydxlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-31 11:58:22.565195 hydxlib-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-31 11:58:19.000000 hydxlib-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.335319 hydxlib-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-12 07:20:34.000000 hydxlib-1.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-12 07:20:34.000000 hydxlib-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 07:20:34.000000 hydxlib-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-12 07:20:37.335319 hydxlib-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 07:20:34.000000 hydxlib-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.331319 hydxlib-1.5.0/hydxlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/hydx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.335319 hydxlib-1.5.0/hydxlib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_hydx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_threedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31610 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/threedi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.335319 hydxlib-1.5.0/hydxlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 07:20:37.335319 hydxlib-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-12 07:20:34.000000 hydxlib-1.5.0/setup.py
```

### Comparing `hydxlib-1.4.5/CHANGES.rst` & `hydxlib-1.5.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog of hydxlib
 ===================================================
 
+1.5.0 (2023-04-12)
+------------------
+
+- Extra release to signal updated requirements.
+
+
 1.4.5 (2023-03-31)
 ------------------
 
 - Make exporter work with SQLAlchemy 2.*
 
 - Updated required threedi-schema version to 0.216.*
```

### Comparing `hydxlib-1.4.5/LICENSE` & `hydxlib-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/PKG-INFO` & `hydxlib-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydxlib
-Version: 1.4.5
+Version: 1.5.0
 Summary: Importer and Exporter for GWSW
 Home-page: https://github.com/nens/hydxlib
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
@@ -83,14 +83,20 @@
 
   $ pre-commit install
 
 
 Changelog of hydxlib
 ===================================================
 
+1.5.0 (2023-04-12)
+------------------
+
+- Extra release to signal updated requirements.
+
+
 1.4.5 (2023-03-31)
 ------------------
 
 - Make exporter work with SQLAlchemy 2.*
 
 - Updated required threedi-schema version to 0.216.*
```

### Comparing `hydxlib-1.4.5/README.rst` & `hydxlib-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/exporter.py` & `hydxlib-1.5.0/hydxlib/exporter.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/hydx.py` & `hydxlib-1.5.0/hydxlib/hydx.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/importer.py` & `hydxlib-1.5.0/hydxlib/importer.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/scripts.py` & `hydxlib-1.5.0/hydxlib/scripts.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/tests/conftest.py` & `hydxlib-1.5.0/hydxlib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/tests/test_exporter.py` & `hydxlib-1.5.0/hydxlib/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/tests/test_hydx.py` & `hydxlib-1.5.0/hydxlib/tests/test_hydx.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/tests/test_importer.py` & `hydxlib-1.5.0/hydxlib/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/tests/test_scripts.py` & `hydxlib-1.5.0/hydxlib/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/tests/test_threedi.py` & `hydxlib-1.5.0/hydxlib/tests/test_threedi.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib/threedi.py` & `hydxlib-1.5.0/hydxlib/threedi.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/hydxlib.egg-info/PKG-INFO` & `hydxlib-1.5.0/hydxlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydxlib
-Version: 1.4.5
+Version: 1.5.0
 Summary: Importer and Exporter for GWSW
 Home-page: https://github.com/nens/hydxlib
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
@@ -83,14 +83,20 @@
 
   $ pre-commit install
 
 
 Changelog of hydxlib
 ===================================================
 
+1.5.0 (2023-04-12)
+------------------
+
+- Extra release to signal updated requirements.
+
+
 1.4.5 (2023-03-31)
 ------------------
 
 - Make exporter work with SQLAlchemy 2.*
 
 - Updated required threedi-schema version to 0.216.*
```

### Comparing `hydxlib-1.4.5/hydxlib.egg-info/SOURCES.txt` & `hydxlib-1.5.0/hydxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydxlib-1.4.5/setup.py` & `hydxlib-1.5.0/setup.py`

 * *Files identical despite different names*

