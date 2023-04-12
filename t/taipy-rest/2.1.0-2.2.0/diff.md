# Comparing `tmp/taipy-rest-2.1.0.tar.gz` & `tmp/taipy-rest-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-rest-2.1.0.tar", last modified: Tue Jan 31 11:36:43 2023, max compression
+gzip compressed data, was "taipy-rest-2.2.0.tar", last modified: Wed Apr 12 09:39:03 2023, max compression
```

## Comparing `taipy-rest-2.1.0.tar` & `taipy-rest-2.2.0.tar`

### file list

```diff
@@ -1,55 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.615615 taipy-rest-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-01-31 11:36:43.615615 taipy-rest-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 11:36:43.615615 taipy-rest-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.607615 taipy-rest-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.607615 taipy-rest-2.1.0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.607615 taipy-rest-2.1.0/src/taipy/rest/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.607615 taipy-rest-2.1.0/src/taipy/rest/api/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.611615 taipy-rest-2.1.0/src/taipy/rest/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.611615 taipy-rest-2.1.0/src/taipy/rest/api/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/middlewares/_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.611615 taipy-rest-2.1.0/src/taipy/rest/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/resources/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/resources/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/resources/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/resources/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/resources/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/resources/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.611615 taipy-rest-2.1.0/src/taipy/rest/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/schemas/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/schemas/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/schemas/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/schemas/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/schemas/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/schemas/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.611615 taipy-rest-2.1.0/src/taipy/rest/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/commons/apispec.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/commons/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/commons/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/commons/to_from_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-31 11:36:31.000000 taipy-rest-2.1.0/src/taipy/rest/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:36:43.615615 taipy-rest-2.1.0/src/taipy_rest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-01-31 11:36:43.000000 taipy-rest-2.1.0/src/taipy_rest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-31 11:36:43.000000 taipy-rest-2.1.0/src/taipy_rest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 11:36:43.000000 taipy-rest-2.1.0/src/taipy_rest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-31 11:36:43.000000 taipy-rest-2.1.0/src/taipy_rest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-31 11:36:43.000000 taipy-rest-2.1.0/src/taipy_rest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.347860 taipy-rest-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-12 09:39:03.347860 taipy-rest-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:39:03.347860 taipy-rest-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.339860 taipy-rest-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.339860 taipy-rest-2.2.0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.343860 taipy-rest-2.2.0/src/taipy/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.343860 taipy-rest-2.2.0/src/taipy/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.343860 taipy-rest-2.2.0/src/taipy/rest/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.343860 taipy-rest-2.2.0/src/taipy/rest/api/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/middlewares/_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.343860 taipy-rest-2.2.0/src/taipy/rest/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/resources/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/resources/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/resources/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/resources/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/resources/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/resources/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.343860 taipy-rest-2.2.0/src/taipy/rest/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/schemas/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/schemas/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/schemas/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/schemas/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/schemas/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.347860 taipy-rest-2.2.0/src/taipy/rest/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/commons/apispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/commons/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/commons/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/commons/to_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/src/taipy/rest/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.347860 taipy-rest-2.2.0/src/taipy_rest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-12 09:39:03.000000 taipy-rest-2.2.0/src/taipy_rest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-12 09:39:03.000000 taipy-rest-2.2.0/src/taipy_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:39:03.000000 taipy-rest-2.2.0/src/taipy_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-12 09:39:03.000000 taipy-rest-2.2.0/src/taipy_rest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:39:03.000000 taipy-rest-2.2.0/src/taipy_rest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:39:03.347860 taipy-rest-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-12 09:38:52.000000 taipy-rest-2.2.0/tests/test_task.py
```

### Comparing `taipy-rest-2.1.0/LICENSE` & `taipy-rest-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/PKG-INFO` & `taipy-rest-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-rest
-Version: 2.1.0
+Version: 2.2.0
 Summary: Library to expose taipy-core REST APIs.
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-rest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `taipy-rest-2.1.0/README.md` & `taipy-rest-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/setup.py` & `taipy-rest-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/__init__.py` & `taipy-rest-2.2.0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/__init__.py` & `taipy-rest-2.2.0/src/taipy/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/__init__.py` & `taipy-rest-2.2.0/src/taipy/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/error_handler.py` & `taipy-rest-2.2.0/src/taipy/rest/api/error_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/exceptions/__init__.py` & `taipy-rest-2.2.0/src/taipy/rest/api/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/exceptions/exceptions.py` & `taipy-rest-2.2.0/src/taipy/rest/api/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/middlewares/__init__.py` & `taipy-rest-2.2.0/src/taipy/rest/api/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/middlewares/_middleware.py` & `taipy-rest-2.2.0/src/taipy/rest/api/middlewares/_middleware.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/resources/__init__.py` & `taipy-rest-2.2.0/src/taipy/rest/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/resources/cycle.py` & `taipy-rest-2.2.0/src/taipy/rest/api/resources/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/resources/datanode.py` & `taipy-rest-2.2.0/src/taipy/rest/api/resources/datanode.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/resources/job.py` & `taipy-rest-2.2.0/src/taipy/rest/api/resources/job.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/resources/pipeline.py` & `taipy-rest-2.2.0/src/taipy/rest/api/resources/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/resources/scenario.py` & `taipy-rest-2.2.0/src/taipy/rest/api/resources/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/resources/task.py` & `taipy-rest-2.2.0/src/taipy/rest/api/resources/task.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/schemas/__init__.py` & `taipy-rest-2.2.0/src/taipy/rest/api/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/schemas/cycle.py` & `taipy-rest-2.2.0/src/taipy/rest/api/schemas/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/schemas/datanode.py` & `taipy-rest-2.2.0/src/taipy/rest/api/schemas/datanode.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/schemas/job.py` & `taipy-rest-2.2.0/src/taipy/rest/api/schemas/job.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/schemas/pipeline.py` & `taipy-rest-2.2.0/src/taipy/rest/api/schemas/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/schemas/scenario.py` & `taipy-rest-2.2.0/src/taipy/rest/api/schemas/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/schemas/task.py` & `taipy-rest-2.2.0/src/taipy/rest/api/schemas/task.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/api/views.py` & `taipy-rest-2.2.0/src/taipy/rest/api/views.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/app.py` & `taipy-rest-2.2.0/src/taipy/rest/app.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/commons/__init__.py` & `taipy-rest-2.2.0/src/taipy/rest/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/commons/apispec.py` & `taipy-rest-2.2.0/src/taipy/rest/commons/apispec.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/commons/pagination.py` & `taipy-rest-2.2.0/src/taipy/rest/commons/pagination.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/commons/to_from_model.py` & `taipy-rest-2.2.0/src/taipy/rest/commons/to_from_model.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/extensions.py` & `taipy-rest-2.2.0/src/taipy/rest/extensions.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/rest.py` & `taipy-rest-2.2.0/src/taipy/rest/rest.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy/rest/version.py` & `taipy-rest-2.2.0/src/taipy/rest/version.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.1.0/src/taipy_rest.egg-info/PKG-INFO` & `taipy-rest-2.2.0/src/taipy_rest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-rest
-Version: 2.1.0
+Version: 2.2.0
 Summary: Library to expose taipy-core REST APIs.
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-rest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

