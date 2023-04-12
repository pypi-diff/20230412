# Comparing `tmp/zarr_checksum-0.2.8.tar.gz` & `tmp/zarr_checksum-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarr_checksum-0.2.8.tar", max compression
+gzip compressed data, was "zarr_checksum-0.2.9.tar", max compression
```

## Comparing `zarr_checksum-0.2.8.tar` & `zarr_checksum-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/LICENSE
--rw-r--r--   0        0        0     1215 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/README.md
--rw-r--r--   0        0        0     1946 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      538 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/__init__.py
--rw-r--r--   0        0        0     2910 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/checksum.py
--rw-r--r--   0        0        0     1053 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/cli.py
--rw-r--r--   0        0        0     3518 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/generators.py
--rw-r--r--   0        0        0     1173 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/tests/test_checksum.py
--rw-r--r--   0        0        0     1469 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/tests/test_generators.py
--rw-r--r--   0        0        0     1161 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/tests/test_tree.py
--rw-r--r--   0        0        0     3092 2023-02-01 22:26:47.556352 zarr_checksum-0.2.8/zarr_checksum/tree.py
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 zarr_checksum-0.2.8/setup.py
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 zarr_checksum-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1215 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/README.md
+-rw-r--r--   0        0        0     1946 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      538 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/checksum.py
+-rw-r--r--   0        0        0     1053 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/cli.py
+-rw-r--r--   0        0        0     3518 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/generators.py
+-rw-r--r--   0        0        0     1173 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/tests/test_checksum.py
+-rw-r--r--   0        0        0     1469 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/tests/test_generators.py
+-rw-r--r--   0        0        0     1161 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/tests/test_tree.py
+-rw-r--r--   0        0        0     3092 2023-04-12 15:12:16.536365 zarr_checksum-0.2.9/zarr_checksum/tree.py
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 zarr_checksum-0.2.9/PKG-INFO
```

### Comparing `zarr_checksum-0.2.8/LICENSE` & `zarr_checksum-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/README.md` & `zarr_checksum-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/pyproject.toml` & `zarr_checksum-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "zarr-checksum"
-version = "0.2.8"
+version = "0.2.9"
 description = "Checksum support for zarrs stored in various backends"
 readme="README.md"
 homepage="https://github.com/dandi/zarr_checksum"
 repository="https://github.com/dandi/zarr_checksum"
 authors = ["Kitware, Inc. <kitware@kitware.com>"]
 license = "Apache 2.0"
 
 [tool.poetry.scripts]
 zarrsum = "zarr_checksum.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-boto3 = "~1.24"
+boto3 = "^1.24"
 zarr = "^2.12"
 click = "^8.1.3"
 tqdm = "^4.64.1"
 pydantic = "^1.10.2"
 
 # Optional
-boto3-stubs = {version = "~1.24", extras = ["s3"], optional = true}
+boto3-stubs = {version = "^1.24", extras = ["s3"], optional = true}
 black = {version = "^22.12.0", optional = true}
 isort = {version = "^5.11.4", optional = true}
 flake8 = {version = "^5.0.4", optional = true}
 flake8-black = {version = "^0.3.6", optional = true}
 flake8-bugbear = {version = "^23.1.20", optional = true}
 flake8-docstrings = {version = "^1.7.0", optional = true}
 flake8-isort = {version = "^6.0.0", optional = true}
```

### Comparing `zarr_checksum-0.2.8/zarr_checksum/__init__.py` & `zarr_checksum-0.2.9/zarr_checksum/__init__.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/zarr_checksum/checksum.py` & `zarr_checksum-0.2.9/zarr_checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/zarr_checksum/cli.py` & `zarr_checksum-0.2.9/zarr_checksum/cli.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/zarr_checksum/generators.py` & `zarr_checksum-0.2.9/zarr_checksum/generators.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/zarr_checksum/tests/test_checksum.py` & `zarr_checksum-0.2.9/zarr_checksum/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/zarr_checksum/tests/test_generators.py` & `zarr_checksum-0.2.9/zarr_checksum/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/zarr_checksum/tests/test_tree.py` & `zarr_checksum-0.2.9/zarr_checksum/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/zarr_checksum/tree.py` & `zarr_checksum-0.2.9/zarr_checksum/tree.py`

 * *Files identical despite different names*

### Comparing `zarr_checksum-0.2.8/PKG-INFO` & `zarr_checksum-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarr-checksum
-Version: 0.2.8
+Version: 0.2.9
 Summary: Checksum support for zarrs stored in various backends
 Home-page: https://github.com/dandi/zarr_checksum
 License: Apache 2.0
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Provides-Extra: format
 Provides-Extra: lint
 Provides-Extra: test
 Requires-Dist: black (>=22.12.0,<23.0.0) ; extra == "format" or extra == "dev"
-Requires-Dist: boto3 (>=1.24,<1.25)
-Requires-Dist: boto3-stubs[s3] (>=1.24,<1.25) ; extra == "dev"
+Requires-Dist: boto3 (>=1.24,<2.0)
+Requires-Dist: boto3-stubs[s3] (>=1.24,<2.0) ; extra == "dev"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: flake8 (>=5.0.4,<6.0.0) ; extra == "lint" or extra == "dev"
 Requires-Dist: flake8-black (>=0.3.6,<0.4.0) ; extra == "lint" or extra == "dev"
 Requires-Dist: flake8-bugbear (>=23.1.20,<24.0.0) ; extra == "lint" or extra == "dev"
 Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0) ; extra == "lint" or extra == "dev"
 Requires-Dist: flake8-isort (>=6.0.0,<7.0.0) ; extra == "lint" or extra == "dev"
 Requires-Dist: flake8-quotes (>=3.3.2,<4.0.0) ; extra == "lint" or extra == "dev"
```

