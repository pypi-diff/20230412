# Comparing `tmp/crimpy-0.0.2.tar.gz` & `tmp/crimpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crimpy-0.0.2.tar", last modified: Tue Apr  4 15:52:50 2023, max compression
+gzip compressed data, was "crimpy-0.0.4.tar", last modified: Wed Apr 12 15:59:33 2023, max compression
```

## Comparing `crimpy-0.0.2.tar` & `crimpy-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:52:50.208113 crimpy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-04 15:52:31.000000 crimpy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-04 15:52:31.000000 crimpy-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-04 15:52:50.208113 crimpy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-04 15:52:31.000000 crimpy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:52:50.208113 crimpy-0.0.2/crimpy/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-04 15:52:31.000000 crimpy-0.0.2/crimpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-04 15:52:31.000000 crimpy-0.0.2/crimpy/crimpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:52:50.208113 crimpy-0.0.2/crimpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-04 15:52:50.000000 crimpy-0.0.2/crimpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-04 15:52:50.000000 crimpy-0.0.2/crimpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 15:52:50.000000 crimpy-0.0.2/crimpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:52:50.000000 crimpy-0.0.2/crimpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 15:52:50.000000 crimpy-0.0.2/crimpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 15:52:50.000000 crimpy-0.0.2/crimpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-04 15:52:31.000000 crimpy-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-04 15:52:50.208113 crimpy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-04 15:52:31.000000 crimpy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:59:33.941785 crimpy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 15:59:23.000000 crimpy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 15:59:23.000000 crimpy-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-12 15:59:33.941785 crimpy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 15:59:23.000000 crimpy-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:59:33.941785 crimpy-0.0.4/crimpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 15:59:23.000000 crimpy-0.0.4/crimpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-12 15:59:23.000000 crimpy-0.0.4/crimpy/crimpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-12 15:59:23.000000 crimpy-0.0.4/crimpy/folium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:59:33.941785 crimpy-0.0.4/crimpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-12 15:59:33.000000 crimpy-0.0.4/crimpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 15:59:33.000000 crimpy-0.0.4/crimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 15:59:33.000000 crimpy-0.0.4/crimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:59:33.000000 crimpy-0.0.4/crimpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 15:59:33.000000 crimpy-0.0.4/crimpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 15:59:33.000000 crimpy-0.0.4/crimpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 15:59:23.000000 crimpy-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-12 15:59:33.941785 crimpy-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-12 15:59:23.000000 crimpy-0.0.4/setup.py
```

### Comparing `crimpy-0.0.2/LICENSE` & `crimpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crimpy-0.0.2/PKG-INFO` & `crimpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crimpy
-Version: 0.0.2
+Version: 0.0.4
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/statenandrea33/crimpy
 Author: Andrea Staten
 Author-email: statenandrea33@gmail.com
 License: MIT license
 Keywords: crimpy
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `crimpy-0.0.2/README.md` & `crimpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `crimpy-0.0.2/crimpy.egg-info/PKG-INFO` & `crimpy-0.0.4/crimpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crimpy
-Version: 0.0.2
+Version: 0.0.4
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/statenandrea33/crimpy
 Author: Andrea Staten
 Author-email: statenandrea33@gmail.com
 License: MIT license
 Keywords: crimpy
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `crimpy-0.0.2/setup.py` & `crimpy-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='crimpy',
     name='crimpy',
     packages=find_packages(include=['crimpy', 'crimpy.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/statenandrea33/crimpy',
-    version='0.0.2',
+    version='0.0.4',
     zip_safe=False,
 )
```

