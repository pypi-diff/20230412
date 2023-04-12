# Comparing `tmp/baselog-2.0.0.tar.gz` & `tmp/baselog-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baselog-2.0.0.tar", last modified: Tue Apr 11 20:19:24 2023, max compression
+gzip compressed data, was "baselog-2.0.1.tar", last modified: Wed Apr 12 08:20:08 2023, max compression
```

## Comparing `baselog-2.0.0.tar` & `baselog-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.427564 baselog-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-11 20:19:00.000000 baselog-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-11 20:19:24.427564 baselog-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-11 20:19:00.000000 baselog-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-11 20:19:00.000000 baselog-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:19:24.427564 baselog-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.423564 baselog-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.423564 baselog-2.0.0/src/baselog/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 20:19:00.000000 baselog-2.0.0/src/baselog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-04-11 20:19:00.000000 baselog-2.0.0/src/baselog/baselog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.423564 baselog-2.0.0/src/baselog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:20:08.915731 baselog-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-12 08:19:45.000000 baselog-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-12 08:20:08.915731 baselog-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-12 08:19:45.000000 baselog-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-12 08:19:45.000000 baselog-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:20:08.915731 baselog-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:20:08.915731 baselog-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:20:08.915731 baselog-2.0.1/src/baselog/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 08:19:45.000000 baselog-2.0.1/src/baselog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-04-12 08:19:45.000000 baselog-2.0.1/src/baselog/baselog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:20:08.915731 baselog-2.0.1/src/baselog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-12 08:20:08.000000 baselog-2.0.1/src/baselog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 08:20:08.000000 baselog-2.0.1/src/baselog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:20:08.000000 baselog-2.0.1/src/baselog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 08:20:08.000000 baselog-2.0.1/src/baselog.egg-info/top_level.txt
```

### Comparing `baselog-2.0.0/LICENSE` & `baselog-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `baselog-2.0.0/PKG-INFO` & `baselog-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: baselog
-Version: 2.0.0
-Summary: typed 12-factor app configuration helper
+Version: 2.0.1
+Summary: helper for log initialization
 Author-email: Ben Burke <actualben@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/edencehealth/baselog
 Project-URL: Bug Tracker, https://github.com/edencehealth/baselog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -64,15 +64,15 @@
 
 A `sys.excepthook` is set by `BaseLog`, so in the case of an uncaught exception, the exception and traceback are logged to the console and log files:
 
 ```log
 2023-04-11T20:06:59+0000 - logdemo - INFO - starting a thing
 2023-04-11T20:06:59+0000 - logdemo.util - WARNING - Things may be happening
 2023-04-11T20:06:59+0000 - logdemo.other.funcs - INFO - Things aren't happening yet
-2023-04-11T20:06:59+0000 - logdemo - CRITICAL - uncaught exception: RuntimeError; What the crap!
+2023-04-11T20:06:59+0000 - logdemo - CRITICAL - uncaught exception: RuntimeError; What the heck?!
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-000: Traceback (most recent call last):
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-001:   File "<frozen runpy>", line 198, in _run_module_as_main
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-002:   File "<frozen runpy>", line 88, in _run_code
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-003:   File "/app/logdemo/__main__.py", line 21, in <module>
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-004:     main()
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-005:   File "/app/logdemo/__main__.py", line 17, in main
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-006:     whatsit()
```

### Comparing `baselog-2.0.0/README.md` & `baselog-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 A `sys.excepthook` is set by `BaseLog`, so in the case of an uncaught exception, the exception and traceback are logged to the console and log files:
 
 ```log
 2023-04-11T20:06:59+0000 - logdemo - INFO - starting a thing
 2023-04-11T20:06:59+0000 - logdemo.util - WARNING - Things may be happening
 2023-04-11T20:06:59+0000 - logdemo.other.funcs - INFO - Things aren't happening yet
-2023-04-11T20:06:59+0000 - logdemo - CRITICAL - uncaught exception: RuntimeError; What the crap!
+2023-04-11T20:06:59+0000 - logdemo - CRITICAL - uncaught exception: RuntimeError; What the heck?!
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-000: Traceback (most recent call last):
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-001:   File "<frozen runpy>", line 198, in _run_module_as_main
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-002:   File "<frozen runpy>", line 88, in _run_code
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-003:   File "/app/logdemo/__main__.py", line 21, in <module>
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-004:     main()
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-005:   File "/app/logdemo/__main__.py", line 17, in main
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-006:     whatsit()
```

### Comparing `baselog-2.0.0/pyproject.toml` & `baselog-2.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "baselog"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Ben Burke", email="actualben@users.noreply.github.com" },
 ]
-description = "typed 12-factor app configuration helper"
+description = "helper for log initialization"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `baselog-2.0.0/src/baselog/baselog.py` & `baselog-2.0.1/src/baselog/baselog.py`

 * *Files identical despite different names*

### Comparing `baselog-2.0.0/src/baselog.egg-info/PKG-INFO` & `baselog-2.0.1/src/baselog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: baselog
-Version: 2.0.0
-Summary: typed 12-factor app configuration helper
+Version: 2.0.1
+Summary: helper for log initialization
 Author-email: Ben Burke <actualben@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/edencehealth/baselog
 Project-URL: Bug Tracker, https://github.com/edencehealth/baselog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -64,15 +64,15 @@
 
 A `sys.excepthook` is set by `BaseLog`, so in the case of an uncaught exception, the exception and traceback are logged to the console and log files:
 
 ```log
 2023-04-11T20:06:59+0000 - logdemo - INFO - starting a thing
 2023-04-11T20:06:59+0000 - logdemo.util - WARNING - Things may be happening
 2023-04-11T20:06:59+0000 - logdemo.other.funcs - INFO - Things aren't happening yet
-2023-04-11T20:06:59+0000 - logdemo - CRITICAL - uncaught exception: RuntimeError; What the crap!
+2023-04-11T20:06:59+0000 - logdemo - CRITICAL - uncaught exception: RuntimeError; What the heck?!
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-000: Traceback (most recent call last):
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-001:   File "<frozen runpy>", line 198, in _run_module_as_main
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-002:   File "<frozen runpy>", line 88, in _run_code
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-003:   File "/app/logdemo/__main__.py", line 21, in <module>
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-004:     main()
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-005:   File "/app/logdemo/__main__.py", line 17, in main
 2023-04-11T20:06:59+0000 - logdemo - CRITICAL - traceback-006:     whatsit()
```

