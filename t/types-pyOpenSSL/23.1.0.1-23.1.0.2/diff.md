# Comparing `tmp/types-pyOpenSSL-23.1.0.1.tar.gz` & `tmp/types-pyOpenSSL-23.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyOpenSSL-23.1.0.1.tar", last modified: Mon Mar 27 18:25:31 2023, max compression
+gzip compressed data, was "types-pyOpenSSL-23.1.0.2.tar", last modified: Wed Apr 12 15:15:52 2023, max compression
```

## Comparing `types-pyOpenSSL-23.1.0.1.tar` & `types-pyOpenSSL-23.1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:31.371883 types-pyOpenSSL-23.1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-03-27 18:25:30.000000 types-pyOpenSSL-23.1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:25:30.000000 types-pyOpenSSL-23.1.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:31.371883 types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-27 18:25:30.000000 types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-03-27 18:21:24.000000 types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/SSL.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-03-27 18:21:24.000000 types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-27 18:21:24.000000 types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-27 18:21:24.000000 types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-27 18:25:31.371883 types-pyOpenSSL-23.1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:25:31.371883 types-pyOpenSSL-23.1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-27 18:25:30.000000 types-pyOpenSSL-23.1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:31.371883 types-pyOpenSSL-23.1.0.1/types_pyOpenSSL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-27 18:25:31.000000 types-pyOpenSSL-23.1.0.1/types_pyOpenSSL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-27 18:25:31.000000 types-pyOpenSSL-23.1.0.1/types_pyOpenSSL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:25:31.000000 types-pyOpenSSL-23.1.0.1/types_pyOpenSSL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:25:31.000000 types-pyOpenSSL-23.1.0.1/types_pyOpenSSL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-27 18:25:31.000000 types-pyOpenSSL-23.1.0.1/types_pyOpenSSL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:52.501234 types-pyOpenSSL-23.1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-12 15:15:51.000000 types-pyOpenSSL-23.1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 15:15:51.000000 types-pyOpenSSL-23.1.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:52.501234 types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-12 15:15:51.000000 types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-12 15:15:34.000000 types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/SSL.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:34.000000 types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-12 15:15:34.000000 types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-12 15:15:34.000000 types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 15:15:34.000000 types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 15:15:52.501234 types-pyOpenSSL-23.1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:15:52.501234 types-pyOpenSSL-23.1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-12 15:15:51.000000 types-pyOpenSSL-23.1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:52.501234 types-pyOpenSSL-23.1.0.2/types_pyOpenSSL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 15:15:52.000000 types-pyOpenSSL-23.1.0.2/types_pyOpenSSL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 15:15:52.000000 types-pyOpenSSL-23.1.0.2/types_pyOpenSSL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:15:52.000000 types-pyOpenSSL-23.1.0.2/types_pyOpenSSL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 15:15:52.000000 types-pyOpenSSL-23.1.0.2/types_pyOpenSSL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 15:15:52.000000 types-pyOpenSSL-23.1.0.2/types_pyOpenSSL.egg-info/top_level.txt
```

### Comparing `types-pyOpenSSL-23.1.0.1/CHANGELOG.md` & `types-pyOpenSSL-23.1.0.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 23.1.0.2 (2023-04-12)
+
+[pyOpenSSL] Fix return type of SSLeay_version (#10037)
+
+Closes: #10024
+
 ## 23.1.0.1 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 23.1.0.0 (2023-03-25)
 
 Update pyOpenSSL to 23.1.* (#9939)
```

### Comparing `types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/SSL.pyi` & `types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/SSL.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 class Error(Exception): ...
 class WantReadError(Error): ...
 class WantWriteError(Error): ...
 class WantX509LookupError(Error): ...
 class ZeroReturnError(Error): ...
 class SysCallError(Error): ...
 
-def SSLeay_version(type: int) -> str: ...
+def SSLeay_version(type: int) -> bytes: ...
 
 class Session: ...
 
 class Connection:
     def __getattr__(self, name: str) -> Any: ...  # takes attributes from `self._socket`
     def __init__(self, context: Context, socket: socket.socket | None = None) -> None: ...
     def get_context(self) -> Context: ...
```

### Comparing `types-pyOpenSSL-23.1.0.1/OpenSSL-stubs/crypto.pyi` & `types-pyOpenSSL-23.1.0.2/OpenSSL-stubs/crypto.pyi`

 * *Files identical despite different names*

### Comparing `types-pyOpenSSL-23.1.0.1/PKG-INFO` & `types-pyOpenSSL-23.1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 23.1.0.1
+Version: 23.1.0.2
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `be0ef211679fabf020dcc79cd4b5c43af0fa1839`.
```

### Comparing `types-pyOpenSSL-23.1.0.1/setup.py` & `types-pyOpenSSL-23.1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `be0ef211679fabf020dcc79cd4b5c43af0fa1839`.
 '''.lstrip()
 
 setup(name=name,
-      version="23.1.0.1",
+      version="23.1.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md",
```

### Comparing `types-pyOpenSSL-23.1.0.1/types_pyOpenSSL.egg-info/PKG-INFO` & `types-pyOpenSSL-23.1.0.2/types_pyOpenSSL.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 23.1.0.1
+Version: 23.1.0.2
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `be0ef211679fabf020dcc79cd4b5c43af0fa1839`.
```

