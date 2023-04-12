# Comparing `tmp/openapi_markdown-0.0.4.tar.gz` & `tmp/openapi_markdown-0.0.5.tar.gz`

## Comparing `openapi_markdown-0.0.4.tar` & `openapi_markdown-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/pypi.sh
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/requirement.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/generator.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/templates/api_doc_template.md.j2
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/templates/example.md.j2
--rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/tests/openapi.json
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/tests/test.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/LICENSE
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/pypi.sh
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/src/openapi_markdown/__init__.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/src/openapi_markdown/generator.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/src/openapi_markdown/templates/api_doc_template.md.j2
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/src/openapi_markdown/templates/example.md.j2
+-rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/tests/openapi.json
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/tests/test.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/LICENSE
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 openapi_markdown-0.0.5/PKG-INFO
```

### Comparing `openapi_markdown-0.0.4/src/openapi_markdown/generator.py` & `openapi_markdown-0.0.5/src/openapi_markdown/generator.py`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.4/src/openapi_markdown/templates/api_doc_template.md.j2` & `openapi_markdown-0.0.5/src/openapi_markdown/templates/api_doc_template.md.j2`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.4/tests/openapi.json` & `openapi_markdown-0.0.5/tests/openapi.json`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.4/LICENSE` & `openapi_markdown-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.4/README.md` & `openapi_markdown-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.4/pyproject.toml` & `openapi_markdown-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openapi-markdown"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="soonoh", email="soonoh.jung@vrerv.com" },
 ]
 description = "Generates API documentation from an OpenAPI specification file"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `openapi_markdown-0.0.4/PKG-INFO` & `openapi_markdown-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-markdown
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generates API documentation from an OpenAPI specification file
 Project-URL: Homepage, https://github.com/vrerv/openapi-markdown
 Project-URL: Bug Tracker, https://github.com/vrerv/openapi-markdown/issues
 Author-email: soonoh <soonoh.jung@vrerv.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

