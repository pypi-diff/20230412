# Comparing `tmp/mango_pycore-0.1.0.tar.gz` & `tmp/mango_pycore-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_pycore-0.1.0.tar", max compression
+gzip compressed data, was "mango_pycore-0.1.1.tar", max compression
```

## Comparing `mango_pycore-0.1.0.tar` & `mango_pycore-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      193 2023-04-11 21:58:06.906084 mango_pycore-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-11 15:48:26.224000 mango_pycore-0.1.0/mango_pycore/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 15:48:41.881000 mango_pycore-0.1.0/mango_pycore/api/__init__.py
--rw-r--r--   0        0        0     3067 2023-04-11 17:08:02.850000 mango_pycore-0.1.0/mango_pycore/api/base_api.py
--rw-r--r--   0        0        0      290 2023-02-27 21:01:16.440000 mango_pycore-0.1.0/mango_pycore/api/exceptions.py
--rw-r--r--   0        0        0     2089 2023-04-11 18:55:16.155000 mango_pycore-0.1.0/mango_pycore/api/http_api.py
--rw-r--r--   0        0        0     4945 2023-04-11 17:08:02.842000 mango_pycore-0.1.0/mango_pycore/api/request.py
--rw-r--r--   0        0        0      627 2023-04-11 17:08:02.862000 mango_pycore-0.1.0/mango_pycore/api/response.py
--rw-r--r--   0        0        0     2089 2023-04-11 17:44:59.674000 mango_pycore-0.1.0/mango_pycore/api/rest_api.py
--rw-r--r--   0        0        0     2710 2023-04-11 16:31:27.655000 mango_pycore-0.1.0/mango_pycore/api/websocket_api.py
--rw-r--r--   0        0        0        0 2023-04-11 15:48:48.597000 mango_pycore-0.1.0/mango_pycore/stream/__init__.py
--rw-r--r--   0        0        0     3965 2023-04-11 16:25:24.868000 mango_pycore-0.1.0/mango_pycore/stream/dynamo.py
--rw-r--r--   0        0        0        0 2023-04-11 16:12:38.138000 mango_pycore-0.1.0/mango_pycore/tools/__init__.py
--rw-r--r--   0        0        0      175 2023-04-11 16:25:24.860000 mango_pycore-0.1.0/mango_pycore/tools/utils.py
--rw-r--r--   0        0        0        0 2023-04-11 15:48:57.665000 mango_pycore-0.1.0/mango_pycore/websocket/__init__.py
--rw-r--r--   0        0        0      348 2023-04-11 21:53:29.153854 mango_pycore-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 mango_pycore-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-04-11 21:58:06.906084 mango_pycore-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 15:48:26.224000 mango_pycore-0.1.1/mango_pycore/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:48:41.881000 mango_pycore-0.1.1/mango_pycore/api/__init__.py
+-rw-r--r--   0        0        0     3067 2023-04-11 17:08:02.850000 mango_pycore-0.1.1/mango_pycore/api/base_api.py
+-rw-r--r--   0        0        0      290 2023-02-27 21:01:16.440000 mango_pycore-0.1.1/mango_pycore/api/exceptions.py
+-rw-r--r--   0        0        0     2089 2023-04-11 18:55:16.155000 mango_pycore-0.1.1/mango_pycore/api/http_api.py
+-rw-r--r--   0        0        0     4945 2023-04-11 17:08:02.842000 mango_pycore-0.1.1/mango_pycore/api/request.py
+-rw-r--r--   0        0        0      627 2023-04-11 17:08:02.862000 mango_pycore-0.1.1/mango_pycore/api/response.py
+-rw-r--r--   0        0        0     2089 2023-04-11 17:44:59.674000 mango_pycore-0.1.1/mango_pycore/api/rest_api.py
+-rw-r--r--   0        0        0     2710 2023-04-11 16:31:27.655000 mango_pycore-0.1.1/mango_pycore/api/websocket_api.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:48:48.597000 mango_pycore-0.1.1/mango_pycore/stream/__init__.py
+-rw-r--r--   0        0        0     3965 2023-04-11 16:25:24.868000 mango_pycore-0.1.1/mango_pycore/stream/dynamo.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:12:38.138000 mango_pycore-0.1.1/mango_pycore/tools/__init__.py
+-rw-r--r--   0        0        0      175 2023-04-11 16:25:24.860000 mango_pycore-0.1.1/mango_pycore/tools/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 15:48:57.665000 mango_pycore-0.1.1/mango_pycore/websocket/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-11 22:20:34.178135 mango_pycore-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 mango_pycore-0.1.1/PKG-INFO
```

### Comparing `mango_pycore-0.1.0/mango_pycore/api/base_api.py` & `mango_pycore-0.1.1/mango_pycore/api/base_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.0/mango_pycore/api/http_api.py` & `mango_pycore-0.1.1/mango_pycore/api/http_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.0/mango_pycore/api/request.py` & `mango_pycore-0.1.1/mango_pycore/api/request.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.0/mango_pycore/api/response.py` & `mango_pycore-0.1.1/mango_pycore/api/response.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.0/mango_pycore/api/rest_api.py` & `mango_pycore-0.1.1/mango_pycore/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.0/mango_pycore/api/websocket_api.py` & `mango_pycore-0.1.1/mango_pycore/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.0/mango_pycore/stream/dynamo.py` & `mango_pycore-0.1.1/mango_pycore/stream/dynamo.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.0/PKG-INFO` & `mango_pycore-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-pycore
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Ernesto Licea Martin
 Author-email: ernesto.licea@mango-soft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

