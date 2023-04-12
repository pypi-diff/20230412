# Comparing `tmp/meilisearch_tui-0.6.0.tar.gz` & `tmp/meilisearch_tui-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_tui-0.6.0.tar", max compression
+gzip compressed data, was "meilisearch_tui-0.6.1.tar", max compression
```

## Comparing `meilisearch_tui-0.6.0.tar` & `meilisearch_tui-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-04-08 00:40:02.889690 meilisearch_tui-0.6.0/LICENSE
--rw-r--r--   0        0        0     2045 2023-04-08 00:40:02.889690 meilisearch_tui-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/__init__.py
--rw-r--r--   0        0        0     2776 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/__main__.py
--rw-r--r--   0        0        0      608 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/client.py
--rw-r--r--   0        0        0     3226 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/config.py
--rw-r--r--   0        0        0       86 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/errors.py
--rw-r--r--   0        0        0     1855 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/meilisearch.css
--rw-r--r--   0        0        0        0 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/py.typed
--rw-r--r--   0        0        0        0 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/screens/__init__.py
--rw-r--r--   0        0        0     4548 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/screens/configuration.py
--rw-r--r--   0        0        0    29002 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/screens/indexes.py
--rw-r--r--   0        0        0     3173 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/screens/meilisearch_settings.py
--rw-r--r--   0        0        0     6208 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/screens/search.py
--rw-r--r--   0        0        0      897 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/utils.py
--rw-r--r--   0        0        0        0 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/widgets/__init__.py
--rw-r--r--   0        0        0      844 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/widgets/index.py
--rw-r--r--   0        0        0     1543 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/widgets/index_sidebar.py
--rw-r--r--   0        0        0     1730 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/widgets/input.py
--rw-r--r--   0        0        0      709 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/meilisearch_tui/widgets/messages.py
--rw-r--r--   0        0        0     1985 2023-04-08 00:40:02.893690 meilisearch_tui-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 meilisearch_tui-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2045 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/__init__.py
+-rw-r--r--   0        0        0     2776 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/__main__.py
+-rw-r--r--   0        0        0      608 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/client.py
+-rw-r--r--   0        0        0     3226 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/config.py
+-rw-r--r--   0        0        0       86 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/errors.py
+-rw-r--r--   0        0        0     1909 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/meilisearch.css
+-rw-r--r--   0        0        0        0 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/py.typed
+-rw-r--r--   0        0        0        0 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/screens/__init__.py
+-rw-r--r--   0        0        0     4548 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/screens/configuration.py
+-rw-r--r--   0        0        0    29002 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/screens/indexes.py
+-rw-r--r--   0        0        0     3173 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/screens/meilisearch_settings.py
+-rw-r--r--   0        0        0     6208 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/screens/search.py
+-rw-r--r--   0        0        0      897 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/__init__.py
+-rw-r--r--   0        0        0      844 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/index.py
+-rw-r--r--   0        0        0     1543 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/index_sidebar.py
+-rw-r--r--   0        0        0     1730 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/input.py
+-rw-r--r--   0        0        0      709 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/messages.py
+-rw-r--r--   0        0        0     1985 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 meilisearch_tui-0.6.1/PKG-INFO
```

### Comparing `meilisearch_tui-0.6.0/LICENSE` & `meilisearch_tui-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/README.md` & `meilisearch_tui-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/__main__.py` & `meilisearch_tui-0.6.1/meilisearch_tui/__main__.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/client.py` & `meilisearch_tui-0.6.1/meilisearch_tui/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/config.py` & `meilisearch_tui-0.6.1/meilisearch_tui/config.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/meilisearch.css` & `meilisearch_tui-0.6.1/meilisearch_tui/meilisearch.css`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,18 @@
   background: $primary-lighten-1;
 }
 
 ListView:focus > ListItem.--highlight {
   background: $secondary;
 }
 
+Underline > .underline--bar {
+  color: $secondary;
+}
+
 #tree-view {
   scrollbar-gutter: stable;
   overflow: auto;
   width: auto;
   height: 100%;
   dock: left;
   margin-right: 2;
```

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/screens/configuration.py` & `meilisearch_tui-0.6.1/meilisearch_tui/screens/configuration.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/screens/indexes.py` & `meilisearch_tui-0.6.1/meilisearch_tui/screens/indexes.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/screens/meilisearch_settings.py` & `meilisearch_tui-0.6.1/meilisearch_tui/screens/meilisearch_settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/screens/search.py` & `meilisearch_tui-0.6.1/meilisearch_tui/screens/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/utils.py` & `meilisearch_tui-0.6.1/meilisearch_tui/utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/widgets/index.py` & `meilisearch_tui-0.6.1/meilisearch_tui/widgets/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/widgets/index_sidebar.py` & `meilisearch_tui-0.6.1/meilisearch_tui/widgets/index_sidebar.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/widgets/input.py` & `meilisearch_tui-0.6.1/meilisearch_tui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/meilisearch_tui/widgets/messages.py` & `meilisearch_tui-0.6.1/meilisearch_tui/widgets/messages.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.0/pyproject.toml` & `meilisearch_tui-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-tui"
-version = "0.6.0"
+version = "0.6.1"
 description = "A TUI for Managing and Searching with Meilisearch"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-tui"
 homepage = "https://github.com/sanders41/meilisearch-tui"
 documentation = "https://github.com/sanders41/meilisearch-tui"
@@ -18,25 +18,25 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 meilisearch-python-async = "1.1.1"
-textual = "0.19.0"
+textual = "0.19.1"
 uvloop = {version = "0.17.0", markers = "sys_platform != 'win32'"}
 
 [tool.poetry.group.dev.dependencies]
 aiohttp = "3.8.4"
 black = "23.3.0"
 click = "8.1.3"
 msgpack = "1.0.5"
 mypy = "1.2.0"
 pre-commit = "3.2.2"
-pytest = "7.2.2"
+pytest = "7.3.0"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.0.0"
 ruff = "0.0.261"
 tox = "4.4.11"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `meilisearch_tui-0.6.0/PKG-INFO` & `meilisearch_tui-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-tui
-Version: 0.6.0
+Version: 0.6.1
 Summary: A TUI for Managing and Searching with Meilisearch
 Home-page: https://github.com/sanders41/meilisearch-tui
 License: MIT
 Keywords: meilisearch,tui
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: meilisearch-python-async (==1.1.1)
-Requires-Dist: textual (==0.19.0)
+Requires-Dist: textual (==0.19.1)
 Requires-Dist: uvloop (==0.17.0) ; sys_platform != "win32"
 Project-URL: Documentation, https://github.com/sanders41/meilisearch-tui
 Project-URL: Repository, https://github.com/sanders41/meilisearch-tui
 Description-Content-Type: text/markdown
 
 # Meilisearch TUI
```

