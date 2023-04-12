# Comparing `tmp/symbolicmode-0.9.7.tar.gz` & `tmp/symbolicmode-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicmode-0.9.7.tar", last modified: Mon Apr 10 04:11:21 2023, max compression
+gzip compressed data, was "symbolicmode-1.0.tar", last modified: Wed Apr 12 15:00:54 2023, max compression
```

## Comparing `symbolicmode-0.9.7.tar` & `symbolicmode-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-10 04:11:14.000000 symbolicmode-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.536718 symbolicmode-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.536718 symbolicmode-0.9.7/src/symbolicmode/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/src/symbolicmode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/src/symbolicmode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 04:11:21.000000 symbolicmode-0.9.7/src/symbolicmode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:11:21.540717 symbolicmode-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/tests/test_chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-10 04:11:08.000000 symbolicmode-0.9.7/tests/test_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.685901 symbolicmode-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-12 15:00:44.000000 symbolicmode-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-12 15:00:54.685901 symbolicmode-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-12 15:00:44.000000 symbolicmode-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 15:00:47.000000 symbolicmode-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:00:54.685901 symbolicmode-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.681902 symbolicmode-1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.681902 symbolicmode-1.0/src/symbolicmode/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-04-12 15:00:44.000000 symbolicmode-1.0/src/symbolicmode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.685901 symbolicmode-1.0/src/symbolicmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.685901 symbolicmode-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-12 15:00:44.000000 symbolicmode-1.0/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-12 15:00:44.000000 symbolicmode-1.0/tests/test_modes.py
```

### Comparing `symbolicmode-0.9.7/LICENSE` & `symbolicmode-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.7/PKG-INFO` & `symbolicmode-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.7
+Version: 1.0
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.7/README.md` & `symbolicmode-1.0/README.md`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.7/pyproject.toml` & `symbolicmode-1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
 name = "symbolicmode"
-version = "0.9.7"
+version = "1.0"
 authors = [
   { name="Sean Reifschneider", email="jafo00@gmail.com" },
 ]
 description = "Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symbolicmode-0.9.7/src/symbolicmode/__init__.py` & `symbolicmode-1.0/src/symbolicmode/__init__.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.7/src/symbolicmode.egg-info/PKG-INFO` & `symbolicmode-1.0/src/symbolicmode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.7
+Version: 1.0
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.7/tests/test_chmod.py` & `symbolicmode-1.0/tests/test_chmod.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.7/tests/test_modes.py` & `symbolicmode-1.0/tests/test_modes.py`

 * *Files identical despite different names*

