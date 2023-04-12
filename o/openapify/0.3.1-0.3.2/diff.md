# Comparing `tmp/openapify-0.3.1.tar.gz` & `tmp/openapify-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.1.tar", last modified: Tue Apr 11 15:15:12 2023, max compression
+gzip compressed data, was "openapify-0.3.2.tar", last modified: Wed Apr 12 11:49:54 2023, max compression
```

## Comparing `openapify-0.3.1.tar` & `openapify-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.415802 openapify-0.3.1/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-04-11 15:10:01.000000 openapify-0.3.1/LICENSE
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    30080 2023-04-11 15:15:12.415659 openapify-0.3.1/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    29266 2023-04-11 15:00:22.000000 openapify-0.3.1/README.md
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.412589 openapify-0.3.1/openapify/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      282 2023-04-09 19:40:13.000000 openapify-0.3.1/openapify/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.414555 openapify-0.3.1/openapify/core/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3.1/openapify/core/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    14737 2023-04-11 12:57:05.000000 openapify-0.3.1/openapify/core/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       92 2023-03-20 20:50:13.000000 openapify-0.3.1/openapify/core/const.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2002 2023-04-11 12:57:05.000000 openapify-0.3.1/openapify/core/document.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3.1/openapify/core/jsonschema.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3.1/openapify/core/models.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.414871 openapify-0.3.1/openapify/core/openapi/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3.1/openapify/core/openapi/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5270 2023-04-09 09:42:43.000000 openapify-0.3.1/openapify/core/openapi/models.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5208 2023-04-10 17:45:46.000000 openapify-0.3.1/openapify/decorators.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.415108 openapify-0.3.1/openapify/ext/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3.1/openapify/ext/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.415281 openapify-0.3.1/openapify/ext/web/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3.1/openapify/ext/web/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3.1/openapify/ext/web/aiohttp.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3.1/openapify/py.typed
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.413301 openapify-0.3.1/openapify.egg-info/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    30080 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      613 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3.1/openapify.egg-info/not-zip-safe
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/requires.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/top_level.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3.1/pyproject.toml
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-11 15:15:12.415840 openapify-0.3.1/setup.cfg
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1249 2023-04-11 15:11:19.000000 openapify-0.3.1/setup.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.547030 openapify-0.3.2/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.2/LICENSE
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30129 2023-04-12 11:49:54.546880 openapify-0.3.2/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29266 2023-04-11 22:14:24.000000 openapify-0.3.2/README.md
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.543689 openapify-0.3.2/openapify/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      282 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.545651 openapify-0.3.2/openapify/core/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    14772 2023-04-12 11:49:41.000000 openapify-0.3.2/openapify/core/builder.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       92 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/const.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2002 2023-04-11 22:14:24.000000 openapify-0.3.2/openapify/core/document.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1630 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/jsonschema.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1748 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/models.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.546039 openapify-0.3.2/openapify/core/openapi/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/openapi/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5270 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/openapi/models.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5208 2023-04-11 22:14:24.000000 openapify-0.3.2/openapify/decorators.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.546335 openapify-0.3.2/openapify/ext/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/ext/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.546526 openapify-0.3.2/openapify/ext/web/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/ext/web/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.2/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/py.typed
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.544514 openapify-0.3.2/openapify.egg-info/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30129 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.2/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/requires.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/top_level.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.2/pyproject.toml
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-12 11:49:54.547066 openapify-0.3.2/setup.cfg
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-12 11:49:09.000000 openapify-0.3.2/setup.py
```

### Comparing `openapify-0.3.1/LICENSE` & `openapify-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/PKG-INFO` & `openapify-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
+Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -299,15 +300,15 @@
 The documentation for [aiohttp](https://github.com/aio-libs/aiohttp)
 web-application can be built in three ways:
 
 * Using an already existing [`aiohttp.web.Application`](https://docs.aiohttp.org/en/stable/web_reference.html#application) object
 * Using a set of [`aiohttp.web.RouteDef`](https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.RouteDef) objects
 * Using a set of objects implementing [`AioHttpRouteDef`](https://github.com/Fatal1ty/openapify/blob/2bbf2e99c06b31fa2f1465f2ebc118884ce2bb95/openapify/ext/web/aiohttp.py#L43-L46) protocol
 
-All we need is to pass either an application, or a set or route defs to
+All we need is to pass either an application, or a set of route defs to
 modified `build_spec` function. See the example:
 ```python
 from aiohttp import web
 from openapify import request_schema, response_schema
 from openapify.ext.web.aiohttp import build_spec
 
 routes = web.RouteTableDef()
@@ -1036,24 +1037,24 @@
 def secure_operation():
     ...
 ```
 
 And the generated specification document will look like this:
 
 ```yaml
+openapi: 3.1.0
+info:
+  title: API
+  version: 1.0.0
 paths:
   /secure_path:
     get:
       responses: {}
       security:
       - x-auth-token: []
-info:
-  title: API
-  version: 1.0.0
-openapi: 3.1.0
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
       location: header
 ```
```

### Comparing `openapify-0.3.1/README.md` & `openapify-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 The documentation for [aiohttp](https://github.com/aio-libs/aiohttp)
 web-application can be built in three ways:
 
 * Using an already existing [`aiohttp.web.Application`](https://docs.aiohttp.org/en/stable/web_reference.html#application) object
 * Using a set of [`aiohttp.web.RouteDef`](https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.RouteDef) objects
 * Using a set of objects implementing [`AioHttpRouteDef`](https://github.com/Fatal1ty/openapify/blob/2bbf2e99c06b31fa2f1465f2ebc118884ce2bb95/openapify/ext/web/aiohttp.py#L43-L46) protocol
 
-All we need is to pass either an application, or a set or route defs to
+All we need is to pass either an application, or a set of route defs to
 modified `build_spec` function. See the example:
 ```python
 from aiohttp import web
 from openapify import request_schema, response_schema
 from openapify.ext.web.aiohttp import build_spec
 
 routes = web.RouteTableDef()
@@ -1014,24 +1014,24 @@
 def secure_operation():
     ...
 ```
 
 And the generated specification document will look like this:
 
 ```yaml
+openapi: 3.1.0
+info:
+  title: API
+  version: 1.0.0
 paths:
   /secure_path:
     get:
       responses: {}
       security:
       - x-auth-token: []
-info:
-  title: API
-  version: 1.0.0
-openapi: 3.1.0
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
       location: header
 ```
```

### Comparing `openapify-0.3.1/openapify/core/builder.py` & `openapify-0.3.2/openapify/core/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
                 http_code = args.pop("http_code")
                 body_value_type = args.pop("body")
                 if body_value_type is not None:
                     code_responses[http_code] = self._build_response(
                         body=body_value_type, **args
                     )
             elif args_type == "path_docs":
+                args = args.copy()
                 summary = args.get("summary")
                 description = args.get("description")
                 tags.extend(args.get("tags") or [])
                 # _merge_parameters(parameters, args.get("parameters") or {})
                 external_docs = self._build_external_docs(
                     args.get("external_docs")
                 )
```

### Comparing `openapify-0.3.1/openapify/core/document.py` & `openapify-0.3.2/openapify/core/document.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/openapify/core/jsonschema.py` & `openapify-0.3.2/openapify/core/jsonschema.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/openapify/core/models.py` & `openapify-0.3.2/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/openapify/core/openapi/models.py` & `openapify-0.3.2/openapify/core/openapi/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/openapify/decorators.py` & `openapify-0.3.2/openapify/decorators.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/openapify/ext/web/aiohttp.py` & `openapify-0.3.2/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/openapify.egg-info/PKG-INFO` & `openapify-0.3.2/openapify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
+Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -299,15 +300,15 @@
 The documentation for [aiohttp](https://github.com/aio-libs/aiohttp)
 web-application can be built in three ways:
 
 * Using an already existing [`aiohttp.web.Application`](https://docs.aiohttp.org/en/stable/web_reference.html#application) object
 * Using a set of [`aiohttp.web.RouteDef`](https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.RouteDef) objects
 * Using a set of objects implementing [`AioHttpRouteDef`](https://github.com/Fatal1ty/openapify/blob/2bbf2e99c06b31fa2f1465f2ebc118884ce2bb95/openapify/ext/web/aiohttp.py#L43-L46) protocol
 
-All we need is to pass either an application, or a set or route defs to
+All we need is to pass either an application, or a set of route defs to
 modified `build_spec` function. See the example:
 ```python
 from aiohttp import web
 from openapify import request_schema, response_schema
 from openapify.ext.web.aiohttp import build_spec
 
 routes = web.RouteTableDef()
@@ -1036,24 +1037,24 @@
 def secure_operation():
     ...
 ```
 
 And the generated specification document will look like this:
 
 ```yaml
+openapi: 3.1.0
+info:
+  title: API
+  version: 1.0.0
 paths:
   /secure_path:
     get:
       responses: {}
       security:
       - x-auth-token: []
-info:
-  title: API
-  version: 1.0.0
-openapi: 3.1.0
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
       location: header
 ```
```

### Comparing `openapify-0.3.1/openapify.egg-info/SOURCES.txt` & `openapify-0.3.2/openapify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapify-0.3.1/setup.py` & `openapify-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.3.1",
+    version="0.3.2",
     description=(
         "Framework agnostic OpenAPI Specification generation for code lovers"
     ),
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
@@ -21,14 +21,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Development Status :: 3 - Alpha",
     ],
     license="Apache License, Version 2.0",
     author="Alexander Tikhonov",
     author_email="random.gauss@gmail.com",
+    url="https://github.com/Fatal1ty/openapify",
     packages=find_packages(include=("openapify", "openapify.*")),
     package_data={"openapify": ["py.typed"]},
     python_requires=">=3.7",
     install_requires=[
         "apispec",
         "mashumaro>=3.6",
     ],
```

