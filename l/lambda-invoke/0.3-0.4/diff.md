# Comparing `tmp/lambda-invoke-0.3.tar.gz` & `tmp/lambda-invoke-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda-invoke-0.3.tar", last modified: Sat Dec 18 23:27:37 2021, max compression
+gzip compressed data, was "lambda-invoke-0.4.tar", last modified: Wed Apr 12 03:35:06 2023, max compression
```

## Comparing `lambda-invoke-0.3.tar` & `lambda-invoke-0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-18 23:27:37.612650 lambda-invoke-0.3/
--rw-r--r--   0 root         (0) root         (0)      156 2021-12-18 23:27:33.000000 lambda-invoke-0.3/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2021-12-18 23:27:33.000000 lambda-invoke-0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1114 2021-12-18 23:27:37.612650 lambda-invoke-0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2021-12-18 23:27:33.000000 lambda-invoke-0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-18 23:27:37.612650 lambda-invoke-0.3/lambda_invoke/
--rw-r--r--   0 root         (0) root         (0)       70 2021-12-18 23:27:33.000000 lambda-invoke-0.3/lambda_invoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4183 2021-12-18 23:27:33.000000 lambda-invoke-0.3/lambda_invoke/simple_proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-18 23:27:37.612650 lambda-invoke-0.3/lambda_invoke.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1114 2021-12-18 23:27:37.000000 lambda-invoke-0.3/lambda_invoke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2021-12-18 23:27:37.000000 lambda-invoke-0.3/lambda_invoke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-18 23:27:37.000000 lambda-invoke-0.3/lambda_invoke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-18 23:27:37.000000 lambda-invoke-0.3/lambda_invoke.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       99 2021-12-18 23:27:37.000000 lambda-invoke-0.3/lambda_invoke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-12-18 23:27:37.000000 lambda-invoke-0.3/lambda_invoke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2021-12-18 23:27:33.000000 lambda-invoke-0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1014 2021-12-18 23:27:37.612650 lambda-invoke-0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 03:35:00.000000 lambda-invoke-0.4/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-04-12 03:35:00.000000 lambda-invoke-0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-12 03:35:06.289003 lambda-invoke-0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      471 2023-04-12 03:35:00.000000 lambda-invoke-0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/lambda_invoke/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-12 03:35:00.000000 lambda-invoke-0.4/lambda_invoke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-04-12 03:35:00.000000 lambda-invoke-0.4/lambda_invoke/simple_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/lambda_invoke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      358 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-12 03:35:06.000000 lambda-invoke-0.4/lambda_invoke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-12 03:35:00.000000 lambda-invoke-0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-12 03:35:06.293003 lambda-invoke-0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 03:35:06.289003 lambda-invoke-0.4/tests/
+-rw-r--r--   0 root         (0) root         (0)     5545 2023-04-12 03:35:00.000000 lambda-invoke-0.4/tests/test_simple_proxy.py
```

### Comparing `lambda-invoke-0.3/LICENSE` & `lambda-invoke-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda-invoke-0.3/PKG-INFO` & `lambda-invoke-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: lambda-invoke
-Version: 0.3
-Summary: Conviniently invoke lambda mimicking a proxy invocation
+Version: 0.4
+Summary: Conveniently invoke lambda mimicking a proxy invocation
 Home-page: https://github.com/IlyaSukhanov/lambda-invoke
 Author: Ilya Sukhanov
 Author-email: ilya@sukhanov.net
 License: MIT license
 Keywords: aws,lambda-invoke
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
@@ -40,9 +39,7 @@
 
     pip intall lambda-invoke
 
 Examples
 ````````
 
 For usage examples refer to lambda-request or lambda-httpx.
-
-
```

### Comparing `lambda-invoke-0.3/lambda_invoke/simple_proxy.py` & `lambda-invoke-0.4/lambda_invoke/simple_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,18 @@
         self.method = method
         self.url = urlparse(url)
         self.headers = headers
         self.body = body
 
     @property
     def function_name(self):
-        return self.url.hostname
+        host_parts = self.url.hostname.split(".")
+        if len(host_parts) > 1:
+            return f"{host_parts[-1]}:{host_parts[-2]}"
+        return host_parts[0]
 
     @property
     def request_query_string(self):
         return {key: value[0] for key, value in parse_qs(self.url.query).items()}
 
     @property
     def request_body(self):
```

### Comparing `lambda-invoke-0.3/lambda_invoke.egg-info/PKG-INFO` & `lambda-invoke-0.4/lambda_invoke.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: lambda-invoke
-Version: 0.3
-Summary: Conviniently invoke lambda mimicking a proxy invocation
+Version: 0.4
+Summary: Conveniently invoke lambda mimicking a proxy invocation
 Home-page: https://github.com/IlyaSukhanov/lambda-invoke
 Author: Ilya Sukhanov
 Author-email: ilya@sukhanov.net
 License: MIT license
 Keywords: aws,lambda-invoke
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
@@ -40,9 +39,7 @@
 
     pip intall lambda-invoke
 
 Examples
 ````````
 
 For usage examples refer to lambda-request or lambda-httpx.
-
-
```

### Comparing `lambda-invoke-0.3/setup.cfg` & `lambda-invoke-0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = lambda-invoke
-version = 0.3
+version = 0.4
 author = Ilya Sukhanov
 author_email = ilya@sukhanov.net
 license = MIT license
-description = Conviniently invoke lambda mimicking a proxy invocation
+description = Conveniently invoke lambda mimicking a proxy invocation
 keywords = 
 	aws
 	lambda-invoke
 url = https://github.com/IlyaSukhanov/lambda-invoke
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers =
```

