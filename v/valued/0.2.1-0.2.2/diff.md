# Comparing `tmp/valued-0.2.1.tar.gz` & `tmp/valued-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valued-0.2.1.tar", max compression
+gzip compressed data, was "valued-0.2.2.tar", max compression
```

## Comparing `valued-0.2.1.tar` & `valued-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1935 2023-03-31 00:03:08.558125 valued-0.2.1/README.md
--rw-r--r--   0        0        0     1259 2023-03-31 00:03:45.163186 valued-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7115 2023-03-31 00:03:08.558125 valued-0.2.1/src/valued/__init__.py
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 valued-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1935 2023-04-12 00:41:19.996569 valued-0.2.2/README.md
+-rw-r--r--   0        0        0     1269 2023-04-12 00:41:51.144636 valued-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7115 2023-04-12 00:41:20.000569 valued-0.2.2/src/valued/__init__.py
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 valued-0.2.2/PKG-INFO
```

### Comparing `valued-0.2.1/README.md` & `valued-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `valued-0.2.1/pyproject.toml` & `valued-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "valued"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Support <hello@valued.app>"]
 readme = "README.md"
-packages = [{include = "src/valued"}]
+packages = [{include = "valued", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
```

### Comparing `valued-0.2.1/src/valued/__init__.py` & `valued-0.2.2/src/valued/__init__.py`

 * *Files identical despite different names*

### Comparing `valued-0.2.1/PKG-INFO` & `valued-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valued
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Support
 Author-email: hello@valued.app
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

