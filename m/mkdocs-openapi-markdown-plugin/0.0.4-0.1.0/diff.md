# Comparing `tmp/mkdocs_openapi_markdown_plugin-0.0.4.tar.gz` & `tmp/mkdocs_openapi_markdown_plugin-0.1.0.tar.gz`

## Comparing `mkdocs_openapi_markdown_plugin-0.0.4.tar` & `mkdocs_openapi_markdown_plugin-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/pypi.sh
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/src/mkdocs_openapi_markdown_plugin/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/src/mkdocs_openapi_markdown_plugin/plugin.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/LICENSE
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/README.md
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/pypi.sh
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/src/mkdocs_openapi_markdown_plugin/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/src/mkdocs_openapi_markdown_plugin/plugin.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/LICENSE
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/README.md
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mkdocs_openapi_markdown_plugin-0.1.0/PKG-INFO
```

### Comparing `mkdocs_openapi_markdown_plugin-0.0.4/src/mkdocs_openapi_markdown_plugin/plugin.py` & `mkdocs_openapi_markdown_plugin-0.1.0/src/mkdocs_openapi_markdown_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_openapi_markdown_plugin-0.0.4/LICENSE` & `mkdocs_openapi_markdown_plugin-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_openapi_markdown_plugin-0.0.4/pyproject.toml` & `mkdocs_openapi_markdown_plugin-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mkdocs-openapi-markdown-plugin"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="soonoh", email="soonoh.jung@vrerv.com" },
 ]
 description = "Mkdocs plugin to generate openapi document markdown"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mkdocs_openapi_markdown_plugin-0.0.4/PKG-INFO` & `mkdocs_openapi_markdown_plugin-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mkdocs-openapi-markdown-plugin
-Version: 0.0.4
+Version: 0.1.0
 Summary: Mkdocs plugin to generate openapi document markdown
 Project-URL: Homepage, https://github.com/vrerv/mkdocs-openapi-markdown-plugin
 Project-URL: Bug Tracker, https://github.com/vrerv/mkdocs-openapi-markdown-plugin/issues
 Author-email: soonoh <soonoh.jung@vrerv.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Requires-Dist: mkdocs==1.4.2
-Requires-Dist: openapi-markdown==0.0.4
+Requires-Dist: openapi-markdown==0.1.0
 Description-Content-Type: text/markdown
 
 # MkDocs OpenApi Markdown Plugin
 
 This plugin generates markdown file from openapi spec file. (json or yaml)
```

