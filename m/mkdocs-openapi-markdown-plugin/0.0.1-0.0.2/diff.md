# Comparing `tmp/mkdocs_openapi_markdown_plugin-0.0.1.tar.gz` & `tmp/mkdocs_openapi_markdown_plugin-0.0.2.tar.gz`

## Comparing `mkdocs_openapi_markdown_plugin-0.0.1.tar` & `mkdocs_openapi_markdown_plugin-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/pypi.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/requirement.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/src/mkdocs_openapi_markdown_plugin/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/src/mkdocs_openapi_markdown_plugin/plugin.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/LICENSE
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/pypi.sh
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/requirement.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/src/mkdocs_openapi_markdown_plugin/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/src/mkdocs_openapi_markdown_plugin/plugin.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/LICENSE
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.2/PKG-INFO
```

### Comparing `mkdocs_openapi_markdown_plugin-0.0.1/src/mkdocs_openapi_markdown_plugin/plugin.py` & `mkdocs_openapi_markdown_plugin-0.0.2/src/mkdocs_openapi_markdown_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_openapi_markdown_plugin-0.0.1/LICENSE` & `mkdocs_openapi_markdown_plugin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_openapi_markdown_plugin-0.0.1/pyproject.toml` & `mkdocs_openapi_markdown_plugin-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mkdocs-openapi-markdown-plugin"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="soonoh", email="soonoh.jung@vrerv.com" },
 ]
 description = "Mkdocs plugin to generate openapi document markdown"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mkdocs_openapi_markdown_plugin-0.0.1/PKG-INFO` & `mkdocs_openapi_markdown_plugin-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-openapi-markdown-plugin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mkdocs plugin to generate openapi document markdown
 Project-URL: Homepage, https://github.com/vrerv/mkdocs-openapi-markdown-plugin
 Project-URL: Bug Tracker, https://github.com/vrerv/mkdocs-openapi-markdown-plugin/issues
 Author-email: soonoh <soonoh.jung@vrerv.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

