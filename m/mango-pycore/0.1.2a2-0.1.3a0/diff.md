# Comparing `tmp/mango_pycore-0.1.2a2.tar.gz` & `tmp/mango_pycore-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_pycore-0.1.2a2.tar", max compression
+gzip compressed data, was "mango_pycore-0.1.3a0.tar", max compression
```

## Comparing `mango_pycore-0.1.2a2.tar` & `mango_pycore-0.1.3a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      193 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/__init__.py
--rw-r--r--   0        0        0     3067 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/base_api.py
--rw-r--r--   0        0        0      290 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/exceptions.py
--rw-r--r--   0        0        0     2089 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/http_api.py
--rw-r--r--   0        0        0     4945 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/request.py
--rw-r--r--   0        0        0      627 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/response.py
--rw-r--r--   0        0        0     2089 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/rest_api.py
--rw-r--r--   0        0        0     2710 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/api/websocket_api.py
--rw-r--r--   0        0        0        0 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/stream/__init__.py
--rw-r--r--   0        0        0     3965 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/stream/dynamo.py
--rw-r--r--   0        0        0        0 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/tools/__init__.py
--rw-r--r--   0        0        0      175 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/tools/utils.py
--rw-r--r--   0        0        0        0 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/mango_pycore/websocket/__init__.py
--rw-r--r--   0        0        0      350 2023-04-12 04:33:22.435484 mango_pycore-0.1.2a2/pyproject.toml
--rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 mango_pycore-0.1.2a2/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/__init__.py
+-rw-r--r--   0        0        0     3067 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/base_api.py
+-rw-r--r--   0        0        0      290 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/exceptions.py
+-rw-r--r--   0        0        0     2089 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/http_api.py
+-rw-r--r--   0        0        0     4945 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/request.py
+-rw-r--r--   0        0        0      627 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/response.py
+-rw-r--r--   0        0        0     2089 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/rest_api.py
+-rw-r--r--   0        0        0     2710 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/api/websocket_api.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/stream/__init__.py
+-rw-r--r--   0        0        0     3965 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/stream/dynamo.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/tools/__init__.py
+-rw-r--r--   0        0        0      175 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/tools/utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/mango_pycore/websocket/__init__.py
+-rw-r--r--   0        0        0      350 2023-04-12 05:21:54.943405 mango_pycore-0.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 mango_pycore-0.1.3a0/PKG-INFO
```

### Comparing `mango_pycore-0.1.2a2/mango_pycore/api/base_api.py` & `mango_pycore-0.1.3a0/mango_pycore/api/base_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.2a2/mango_pycore/api/http_api.py` & `mango_pycore-0.1.3a0/mango_pycore/api/http_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.2a2/mango_pycore/api/request.py` & `mango_pycore-0.1.3a0/mango_pycore/api/request.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.2a2/mango_pycore/api/response.py` & `mango_pycore-0.1.3a0/mango_pycore/api/response.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.2a2/mango_pycore/api/rest_api.py` & `mango_pycore-0.1.3a0/mango_pycore/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.2a2/mango_pycore/api/websocket_api.py` & `mango_pycore-0.1.3a0/mango_pycore/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.2a2/mango_pycore/stream/dynamo.py` & `mango_pycore-0.1.3a0/mango_pycore/stream/dynamo.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.2a2/PKG-INFO` & `mango_pycore-0.1.3a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-pycore
-Version: 0.1.2a2
+Version: 0.1.3a0
 Summary: 
 Author: Ernesto Licea Martin
 Author-email: ernesto.licea@mango-soft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,9 +16,9 @@
 ## Mango Pycore
 
 An implementation of common features for all SAM backend project for [Mango Soft Inc](http://www.mango-soft.com)
 
 ### How to install
 
 ```bash
-    $ pip install mango_pycore
+    $ pip install mango-pycore
 ```
```
