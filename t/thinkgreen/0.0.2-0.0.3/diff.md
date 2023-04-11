# Comparing `tmp/thinkgreen-0.0.2.tar.gz` & `tmp/thinkgreen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkgreen-0.0.2.tar", last modified: Tue Apr  4 19:02:47 2023, max compression
+gzip compressed data, was "thinkgreen-0.0.3.tar", last modified: Tue Apr 11 23:22:59 2023, max compression
```

## Comparing `thinkgreen-0.0.2.tar` & `thinkgreen-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:02:47.223574 thinkgreen-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 19:02:37.000000 thinkgreen-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-04 19:02:37.000000 thinkgreen-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-04 19:02:47.223574 thinkgreen-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-04 19:02:37.000000 thinkgreen-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 19:02:37.000000 thinkgreen-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-04 19:02:47.223574 thinkgreen-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-04 19:02:37.000000 thinkgreen-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:02:47.223574 thinkgreen-0.0.2/thinkgreen/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-04 19:02:37.000000 thinkgreen-0.0.2/thinkgreen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-04 19:02:37.000000 thinkgreen-0.0.2/thinkgreen/thinkgreen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:02:47.223574 thinkgreen-0.0.2/thinkgreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-04 19:02:47.000000 thinkgreen-0.0.2/thinkgreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-04 19:02:47.000000 thinkgreen-0.0.2/thinkgreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 19:02:47.000000 thinkgreen-0.0.2/thinkgreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:02:47.000000 thinkgreen-0.0.2/thinkgreen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 19:02:47.000000 thinkgreen-0.0.2/thinkgreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 19:02:47.000000 thinkgreen-0.0.2/thinkgreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:22:59.137228 thinkgreen-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 23:22:49.000000 thinkgreen-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 23:22:49.000000 thinkgreen-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-11 23:22:59.137228 thinkgreen-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-11 23:22:49.000000 thinkgreen-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 23:22:49.000000 thinkgreen-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 23:22:59.137228 thinkgreen-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-11 23:22:49.000000 thinkgreen-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:22:59.133228 thinkgreen-0.0.3/thinkgreen/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 23:22:49.000000 thinkgreen-0.0.3/thinkgreen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-04-11 23:22:49.000000 thinkgreen-0.0.3/thinkgreen/thinkgreen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:22:59.137228 thinkgreen-0.0.3/thinkgreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-11 23:22:59.000000 thinkgreen-0.0.3/thinkgreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-11 23:22:59.000000 thinkgreen-0.0.3/thinkgreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 23:22:59.000000 thinkgreen-0.0.3/thinkgreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:22:59.000000 thinkgreen-0.0.3/thinkgreen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 23:22:59.000000 thinkgreen-0.0.3/thinkgreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 23:22:59.000000 thinkgreen-0.0.3/thinkgreen.egg-info/top_level.txt
```

### Comparing `thinkgreen-0.0.2/LICENSE` & `thinkgreen-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thinkgreen-0.0.2/PKG-INFO` & `thinkgreen-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinkgreen
-Version: 0.0.2
+Version: 0.0.3
 Summary: python package final project
 Home-page: https://github.com/olilamm/thinkgreen
 Author: Olivia Lamm
 Author-email: olamm@vols.utk.edu
 License: MIT license
 Keywords: thinkgreen
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `thinkgreen-0.0.2/README.md` & `thinkgreen-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `thinkgreen-0.0.2/setup.py` & `thinkgreen-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='thinkgreen',
     name='thinkgreen',
     packages=find_packages(include=['thinkgreen', 'thinkgreen.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/olilamm/thinkgreen',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

### Comparing `thinkgreen-0.0.2/thinkgreen.egg-info/PKG-INFO` & `thinkgreen-0.0.3/thinkgreen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinkgreen
-Version: 0.0.2
+Version: 0.0.3
 Summary: python package final project
 Home-page: https://github.com/olilamm/thinkgreen
 Author: Olivia Lamm
 Author-email: olamm@vols.utk.edu
 License: MIT license
 Keywords: thinkgreen
 Classifier: Development Status :: 2 - Pre-Alpha
```

