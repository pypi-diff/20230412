# Comparing `tmp/microllama-0.4.6.tar.gz` & `tmp/microllama-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microllama-0.4.6.tar", last modified: Mon Mar 20 18:00:23 2023, max compression
+gzip compressed data, was "microllama-0.4.7.tar", last modified: Wed Apr 12 13:03:48 2023, max compression
```

## Comparing `microllama-0.4.6.tar` & `microllama-0.4.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       60 2023-03-13 12:38:15.340959 microllama-0.4.6/.dockerignore
--rw-r--r--   0        0        0     3119 2023-03-13 12:38:15.341062 microllama-0.4.6/.gitignore
--rw-r--r--   0        0        0     1066 2023-03-13 12:38:15.341213 microllama-0.4.6/LICENSE
--rw-r--r--   0        0        0     3559 2023-03-19 21:29:23.436615 microllama-0.4.6/README.md
--rw-r--r--   0        0        0      262 2023-03-19 21:29:23.437372 microllama-0.4.6/microllama/Dockerfile
--rw-r--r--   0        0        0     7763 2023-03-20 17:55:11.913136 microllama-0.4.6/microllama/__init__.py
--rw-r--r--   0        0        0    19314 2023-03-14 13:05:44.551702 microllama-0.4.6/microllama/example.source.json
--rw-r--r--   0        0        0     4092 2023-03-20 17:59:23.179760 microllama-0.4.6/microllama/index.html
--rw-r--r--   0        0        0      583 2023-03-19 22:11:32.820944 microllama-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     4024 1970-01-01 00:00:00.000000 microllama-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-03-13 12:38:15.340959 microllama-0.4.7/.dockerignore
+-rw-r--r--   0        0        0     3127 2023-03-21 15:46:26.361821 microllama-0.4.7/.gitignore
+-rw-r--r--   0        0        0     1066 2023-03-13 12:38:15.341213 microllama-0.4.7/LICENSE
+-rw-r--r--   0        0        0     3559 2023-03-19 21:29:23.436615 microllama-0.4.7/README.md
+-rw-r--r--   0        0        0      262 2023-03-19 21:29:23.437372 microllama-0.4.7/microllama/Dockerfile
+-rw-r--r--   0        0        0     7763 2023-04-12 13:03:32.635581 microllama-0.4.7/microllama/__init__.py
+-rw-r--r--   0        0        0    19314 2023-03-14 13:05:44.551702 microllama-0.4.7/microllama/example.source.json
+-rw-r--r--   0        0        0     4092 2023-03-20 17:59:23.179760 microllama-0.4.7/microllama/index.html
+-rw-r--r--   0        0        0      599 2023-04-12 12:59:15.537398 microllama-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 microllama-0.4.7/PKG-INFO
```

### Comparing `microllama-0.4.6/.gitignore` & `microllama-0.4.7/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 __pycache__/
 *.py[cod]
 *$py.class
 fly.toml
 # source.json
 faiss_index/
 ig-*
+.vscode
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `microllama-0.4.6/LICENSE` & `microllama-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `microllama-0.4.6/README.md` & `microllama-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `microllama-0.4.6/microllama/__init__.py` & `microllama-0.4.7/microllama/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The smallest possible LLM API"""
 
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 import inspect
 import json
 import os
 import sys
 from functools import lru_cache
 from typing import Optional, Union
```

### Comparing `microllama-0.4.6/microllama/example.source.json` & `microllama-0.4.7/microllama/example.source.json`

 * *Files identical despite different names*

### Comparing `microllama-0.4.6/microllama/index.html` & `microllama-0.4.7/microllama/index.html`

 * *Files identical despite different names*

### Comparing `microllama-0.4.6/pyproject.toml` & `microllama-0.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 authors = [{name = "Tom Dyson", email = "tom@torchbox.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
     "langchain", 
+    "tiktoken",
     "faiss-cpu",
     "openai",
     "fastapi",
     "uvicorn[standard]",
     "sse-starlette",
     "typer"
 ]
```

### Comparing `microllama-0.4.6/PKG-INFO` & `microllama-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: microllama
-Version: 0.4.6
+Version: 0.4.7
 Summary: The smallest possible LLM API
 Author-email: Tom Dyson <tom@torchbox.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: langchain
+Requires-Dist: tiktoken
 Requires-Dist: faiss-cpu
 Requires-Dist: openai
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 Requires-Dist: sse-starlette
 Requires-Dist: typer
 Project-URL: Home, https://github.com/tomdyson/microllama
```

