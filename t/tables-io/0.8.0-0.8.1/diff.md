# Comparing `tmp/tables_io-0.8.0.tar.gz` & `tmp/tables_io-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tables_io-0.8.0.tar", last modified: Wed Apr 12 16:42:25 2023, max compression
+gzip compressed data, was "tables_io-0.8.1.tar", last modified: Wed Apr 12 20:05:53 2023, max compression
```

## Comparing `tables_io-0.8.0.tar` & `tables_io-0.8.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-12 16:42:07.000000 tables_io-0.8.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-12 16:42:07.000000 tables_io-0.8.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-04-12 16:42:07.000000 tables_io-0.8.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-12 16:42:07.000000 tables_io-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-12 16:42:07.000000 tables_io-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-12 16:42:25.368535 tables_io-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-12 16:42:07.000000 tables_io-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4944 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/tables_io.rst
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-12 16:42:07.000000 tables_io-0.8.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/nb/
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/hdf5_iter_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/multipleWriteHdf5_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5885 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/singleTable_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8213 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/tableDict_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-04-12 16:42:07.000000 tables_io-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 16:42:25.368535 tables_io-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-12 16:42:07.000000 tables_io-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/src/tables_io/
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-12 16:42:24.000000 tables_io-0.8.0/src/tables_io/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/arrayUtils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9925 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/convUtils.py
--rw-r--r--   0 runner    (1001) docker     (122)    31624 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/ioUtils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/lazy_modules.py
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/tableDict.py
--rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/testUtils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5328 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/src/tables_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)     8272 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/data/no_groupname_test.hdf5
--rw-r--r--   0 runner    (1001) docker     (122)     9104 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/data/pandas_test_hdf5.h5
--rw-r--r--   0 runner    (1001) docker     (122)    10172 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/data/parquet_test.parquet
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     5176 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_table_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.918478 tables_io-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-12 20:05:30.000000 tables_io-0.8.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.914477 tables_io-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.914477 tables_io-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-12 20:05:30.000000 tables_io-0.8.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-04-12 20:05:30.000000 tables_io-0.8.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-12 20:05:30.000000 tables_io-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-12 20:05:30.000000 tables_io-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-12 20:05:53.918478 tables_io-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-12 20:05:30.000000 tables_io-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.914477 tables_io-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-12 20:05:30.000000 tables_io-0.8.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-04-12 20:05:30.000000 tables_io-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-04-12 20:05:30.000000 tables_io-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4944 2023-04-12 20:05:30.000000 tables_io-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-12 20:05:30.000000 tables_io-0.8.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-04-12 20:05:30.000000 tables_io-0.8.1/docs/tables_io.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-12 20:05:30.000000 tables_io-0.8.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.918478 tables_io-0.8.1/nb/
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-12 20:05:30.000000 tables_io-0.8.1/nb/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-04-12 20:05:30.000000 tables_io-0.8.1/nb/hdf5_iter_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-04-12 20:05:30.000000 tables_io-0.8.1/nb/multipleWriteHdf5_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     5885 2023-04-12 20:05:30.000000 tables_io-0.8.1/nb/singleTable_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8213 2023-04-12 20:05:30.000000 tables_io-0.8.1/nb/tableDict_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-04-12 20:05:30.000000 tables_io-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 20:05:53.918478 tables_io-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-12 20:05:30.000000 tables_io-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.914477 tables_io-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.918478 tables_io-0.8.1/src/tables_io/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-12 20:05:52.000000 tables_io-0.8.1/src/tables_io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/arrayUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9925 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/convUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31624 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/ioUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/lazy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/tableDict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/testUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5328 2023-04-12 20:05:30.000000 tables_io-0.8.1/src/tables_io/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.918478 tables_io-0.8.1/src/tables_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-12 20:05:53.000000 tables_io-0.8.1/src/tables_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-12 20:05:53.000000 tables_io-0.8.1/src/tables_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 20:05:53.000000 tables_io-0.8.1/src/tables_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-04-12 20:05:53.000000 tables_io-0.8.1/src/tables_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 20:05:53.000000 tables_io-0.8.1/src/tables_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.918478 tables_io-0.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:05:53.918478 tables_io-0.8.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     8272 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/data/no_groupname_test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (122)     9104 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/data/pandas_test_hdf5.h5
+-rw-r--r--   0 runner    (1001) docker     (122)    10172 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/data/parquet_test.parquet
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5176 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/test_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/test_table_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-04-12 20:05:30.000000 tables_io-0.8.1/tests/test_utils.py
```

### Comparing `tables_io-0.8.0/.github/workflows/pypi.yaml` & `tables_io-0.8.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/.github/workflows/python-package.yml` & `tables_io-0.8.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/.gitignore` & `tables_io-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/LICENSE` & `tables_io-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/PKG-INFO` & `tables_io-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tables_io
-Version: 0.8.0
+Version: 0.8.1
 Summary: Input/output and conversion functions for tabular data
 Author-email: Eric Charles <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2021 Eric Charles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: io
+Provides-Extra: full
 Provides-Extra: dev
 License-File: LICENSE
 
 # tables_io
 
 Input/output and conversion interfaces for tabular data formats.
```

### Comparing `tables_io-0.8.0/docs/.gitignore` & `tables_io-0.8.1/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/docs/Makefile` & `tables_io-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/docs/conf.py` & `tables_io-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/docs/index.rst` & `tables_io-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/docs/tables_io.rst` & `tables_io-0.8.1/docs/tables_io.rst`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/nb/.gitignore` & `tables_io-0.8.1/nb/.gitignore`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/nb/hdf5_iter_example.ipynb` & `tables_io-0.8.1/nb/hdf5_iter_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/nb/multipleWriteHdf5_example.ipynb` & `tables_io-0.8.1/nb/multipleWriteHdf5_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/nb/singleTable_example.ipynb` & `tables_io-0.8.1/nb/singleTable_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/nb/tableDict_example.ipynb` & `tables_io-0.8.1/nb/tableDict_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/pyproject.toml` & `tables_io-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ]
 dynamic = ["version"]
 dependencies = [
     "numpy>=1.21.0",
 ]
 
 [project.optional-dependencies]
-io = [
+full = [
     "astropy",
     "tables",
     "h5py>=2.9",
     "pandas",
     "pyarrow",
 ]
 dev = [
```

### Comparing `tables_io-0.8.0/src/tables_io/__init__.py` & `tables_io-0.8.1/src/tables_io/__init__.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io/arrayUtils.py` & `tables_io-0.8.1/src/tables_io/arrayUtils.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io/convUtils.py` & `tables_io-0.8.1/src/tables_io/convUtils.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io/ioUtils.py` & `tables_io-0.8.1/src/tables_io/ioUtils.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io/lazy_modules.py` & `tables_io-0.8.1/src/tables_io/lazy_modules.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io/tableDict.py` & `tables_io-0.8.1/src/tables_io/tableDict.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io/testUtils.py` & `tables_io-0.8.1/src/tables_io/testUtils.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io/types.py` & `tables_io-0.8.1/src/tables_io/types.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/src/tables_io.egg-info/PKG-INFO` & `tables_io-0.8.1/src/tables_io.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tables-io
-Version: 0.8.0
+Version: 0.8.1
 Summary: Input/output and conversion functions for tabular data
 Author-email: Eric Charles <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2021 Eric Charles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: io
+Provides-Extra: full
 Provides-Extra: dev
 License-File: LICENSE
 
 # tables_io
 
 Input/output and conversion interfaces for tabular data formats.
```

### Comparing `tables_io-0.8.0/src/tables_io.egg-info/SOURCES.txt` & `tables_io-0.8.1/src/tables_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/data/no_groupname_test.hdf5` & `tables_io-0.8.1/tests/data/no_groupname_test.hdf5`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/data/pandas_test_hdf5.h5` & `tables_io-0.8.1/tests/data/pandas_test_hdf5.h5`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/data/parquet_test.parquet` & `tables_io-0.8.1/tests/data/parquet_test.parquet`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/test_conv.py` & `tables_io-0.8.1/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/test_fileIO.py` & `tables_io-0.8.1/tests/test_fileIO.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/test_io.py` & `tables_io-0.8.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/test_table_dict.py` & `tables_io-0.8.1/tests/test_table_dict.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.8.0/tests/test_utils.py` & `tables_io-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

