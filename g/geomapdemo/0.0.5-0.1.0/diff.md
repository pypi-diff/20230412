# Comparing `tmp/geomapdemo-0.0.5.tar.gz` & `tmp/geomapdemo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.0.5.tar", last modified: Tue Apr 11 21:41:08 2023, max compression
+gzip compressed data, was "geomapdemo-0.1.0.tar", last modified: Tue Apr 11 22:12:55 2023, max compression
```

## Comparing `geomapdemo-0.0.5.tar` & `geomapdemo-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/setup.py
```

### Comparing `geomapdemo-0.0.5/LICENSE` & `geomapdemo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.0.5/PKG-INFO` & `geomapdemo-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.0.5
+Version: 0.1.0
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.0.5/README.md` & `geomapdemo-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.0.5/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.1.0/geomapdemo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.0.5
+Version: 0.1.0
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.0.5/setup.py` & `geomapdemo-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.0.5',
+    version='0.1.0',
     zip_safe=False,
 )
```

