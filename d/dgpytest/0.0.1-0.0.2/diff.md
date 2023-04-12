# Comparing `tmp/dgpytest-0.0.1.tar.gz` & `tmp/dgpytest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgpytest-0.0.1.tar", max compression
+gzip compressed data, was "dgpytest-0.0.2.tar", max compression
```

## Comparing `dgpytest-0.0.1.tar` & `dgpytest-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      743 2023-04-12 18:23:21.340274 dgpytest-0.0.1/dgpytest/__init__.py
--rw-r--r--   0        0        0      477 2023-04-12 18:23:21.340274 dgpytest-0.0.1/dgpytest/__main__.py
--rw-r--r--   0        0        0      292 2023-04-12 18:23:21.340274 dgpytest-0.0.1/dgpytest/_meta.py
--rw-r--r--   0        0        0      454 2023-04-12 18:23:21.341271 dgpytest-0.0.1/dgpytest/hooks.py
--rw-r--r--   0        0        0     2583 2023-04-12 18:23:21.341271 dgpytest-0.0.1/dgpytest/plugin.py
--rw-r--r--   0        0        0        0 2023-04-12 18:23:21.341271 dgpytest-0.0.1/dgpytest/py.typed
--rw-r--r--   0        0        0     1056 2023-04-12 18:23:21.339264 dgpytest-0.0.1/LICENSE
--rw-r--r--   0        0        0     2160 2023-04-12 18:23:21.342273 dgpytest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      813 2023-04-12 18:23:21.339264 dgpytest-0.0.1/README.md
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 dgpytest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      743 2023-04-12 18:54:12.719143 dgpytest-0.0.2/dgpytest/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-12 18:54:12.719143 dgpytest-0.0.2/dgpytest/__main__.py
+-rw-r--r--   0        0        0      292 2023-04-12 18:54:12.720143 dgpytest-0.0.2/dgpytest/_meta.py
+-rw-r--r--   0        0        0      454 2023-04-12 18:54:12.720143 dgpytest-0.0.2/dgpytest/hooks.py
+-rw-r--r--   0        0        0     2583 2023-04-12 18:54:12.720143 dgpytest-0.0.2/dgpytest/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:54:12.720143 dgpytest-0.0.2/dgpytest/py.typed
+-rw-r--r--   0        0        0     1056 2023-04-12 18:54:12.718144 dgpytest-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2157 2023-04-12 18:54:12.722145 dgpytest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      813 2023-04-12 18:54:12.718144 dgpytest-0.0.2/README.md
+-rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 dgpytest-0.0.2/PKG-INFO
```

### Comparing `dgpytest-0.0.1/dgpytest/__init__.py` & `dgpytest-0.0.2/dgpytest/__init__.py`

 * *Files identical despite different names*

### Comparing `dgpytest-0.0.1/dgpytest/plugin.py` & `dgpytest-0.0.2/dgpytest/plugin.py`

 * *Files identical despite different names*

### Comparing `dgpytest-0.0.1/LICENSE` & `dgpytest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dgpytest-0.0.1/pyproject.toml` & `dgpytest-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dgpytest"
-version = "0.0.1"
+version = "0.0.2"
 description = "dgpytest = dgpy + pytest"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/dgpytest"
 readme = 'README.md'
 packages = [
@@ -30,15 +30,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest = ">=7.2.2"
 pytest-asyncio = "^0.21.0"
 
 [tool.poetry.plugins.pytest11]
-cool_plugin = "dgpytest.plugin"
+dgpytest = "dgpytest.plugin"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `dgpytest-0.0.1/README.md` & `dgpytest-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dgpytest-0.0.1/PKG-INFO` & `dgpytest-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgpytest
-Version: 0.0.1
+Version: 0.0.2
 Summary: dgpytest = dgpy + pytest
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/dgpytest
 License: MIT
 Keywords: pytest,dgpy,typed,plugin
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dgpytest Version: 0.0.1 Summary: dgpytest = dgpy +
+Metadata-Version: 2.1 Name: dgpytest Version: 0.0.2 Summary: dgpytest = dgpy +
 pytest Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/
 libs/dgpytest License: MIT Keywords: pytest,dgpy,typed,plugin Author: jesse
 Author-email: jesse@dgi.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

