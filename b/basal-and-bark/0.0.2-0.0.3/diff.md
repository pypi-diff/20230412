# Comparing `tmp/basal_and_bark-0.0.2.tar.gz` & `tmp/basal_and_bark-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basal_and_bark-0.0.2.tar", last modified: Wed Apr  5 17:50:59 2023, max compression
+gzip compressed data, was "basal_and_bark-0.0.3.tar", last modified: Wed Apr 12 16:41:41 2023, max compression
```

## Comparing `basal_and_bark-0.0.2.tar` & `basal_and_bark-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:50:59.068290 basal_and_bark-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-05 17:50:48.000000 basal_and_bark-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-05 17:50:48.000000 basal_and_bark-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-05 17:50:59.068290 basal_and_bark-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-05 17:50:48.000000 basal_and_bark-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:50:59.064290 basal_and_bark-0.0.2/basal_and_bark/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 17:50:48.000000 basal_and_bark-0.0.2/basal_and_bark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-05 17:50:48.000000 basal_and_bark-0.0.2/basal_and_bark/basal_and_bark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:50:59.068290 basal_and_bark-0.0.2/basal_and_bark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-05 17:50:59.000000 basal_and_bark-0.0.2/basal_and_bark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-05 17:50:59.000000 basal_and_bark-0.0.2/basal_and_bark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-05 17:50:59.000000 basal_and_bark-0.0.2/basal_and_bark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:50:59.000000 basal_and_bark-0.0.2/basal_and_bark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-05 17:50:59.000000 basal_and_bark-0.0.2/basal_and_bark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 17:50:59.000000 basal_and_bark-0.0.2/basal_and_bark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 17:50:48.000000 basal_and_bark-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-05 17:50:59.068290 basal_and_bark-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-05 17:50:48.000000 basal_and_bark-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:41:41.121163 basal_and_bark-0.0.3/basal_and_bark/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/basal_and_bark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/basal_and_bark/basal_and_bark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/basal_and_bark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/setup.py
```

### Comparing `basal_and_bark-0.0.2/LICENSE` & `basal_and_bark-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.2/PKG-INFO` & `basal_and_bark-0.0.3/basal_and_bark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: basal_and_bark
-Version: 0.0.2
+Name: basal-and-bark
+Version: 0.0.3
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.2/README.md` & `basal_and_bark-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.2/basal_and_bark.egg-info/PKG-INFO` & `basal_and_bark-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: basal-and-bark
-Version: 0.0.2
+Name: basal_and_bark
+Version: 0.0.3
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.2/setup.py` & `basal_and_bark-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='basal_and_bark',
     name='basal_and_bark',
     packages=find_packages(include=['basal_and_bark', 'basal_and_bark.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZachDorm/basal_and_bark',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

