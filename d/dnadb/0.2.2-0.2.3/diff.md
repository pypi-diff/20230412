# Comparing `tmp/dnadb-0.2.2.tar.gz` & `tmp/dnadb-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.2.2.tar", last modified: Wed Apr 12 05:08:54 2023, max compression
+gzip compressed data, was "dnadb-0.2.3.tar", last modified: Wed Apr 12 05:32:53 2023, max compression
```

## Comparing `dnadb-0.2.2.tar` & `dnadb-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:08:54.946390 dnadb-0.2.2/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.2/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-12 05:08:54.946390 dnadb-0.2.2/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.2/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-12 05:07:54.000000 dnadb-0.2.2/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-12 05:08:54.946390 dnadb-0.2.2/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:08:54.946390 dnadb-0.2.2/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:08:54.946390 dnadb-0.2.2/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-12 05:08:06.000000 dnadb-0.2.2/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:08:54.946390 dnadb-0.2.2/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.2/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.2/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.2/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:08:54.946390 dnadb-0.2.2/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5446 2023-03-29 23:23:47.000000 dnadb-0.2.2/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.2/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      988 2023-04-12 05:07:32.000000 dnadb-0.2.2/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.2/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4786 2023-04-01 20:18:30.000000 dnadb-0.2.2/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6098 2023-04-01 22:17:05.000000 dnadb-0.2.2/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    14178 2023-04-02 01:58:16.000000 dnadb-0.2.2/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.2/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:08:54.946390 dnadb-0.2.2/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-12 05:08:54.000000 dnadb-0.2.2/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-12 05:08:54.000000 dnadb-0.2.2/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-12 05:08:54.000000 dnadb-0.2.2/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-12 05:08:54.000000 dnadb-0.2.2/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-12 05:08:54.000000 dnadb-0.2.2/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:32:53.611128 dnadb-0.2.3/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.3/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-12 05:32:53.611128 dnadb-0.2.3/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.3/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-12 05:32:22.000000 dnadb-0.2.3/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-12 05:32:53.611128 dnadb-0.2.3/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:32:53.611128 dnadb-0.2.3/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:32:53.611128 dnadb-0.2.3/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-12 05:32:19.000000 dnadb-0.2.3/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:32:53.611128 dnadb-0.2.3/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.3/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.3/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.3/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:32:53.611128 dnadb-0.2.3/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5446 2023-03-29 23:23:47.000000 dnadb-0.2.3/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.3/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.3/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.3/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4775 2023-04-12 05:31:58.000000 dnadb-0.2.3/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6098 2023-04-01 22:17:05.000000 dnadb-0.2.3/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    14178 2023-04-02 01:58:16.000000 dnadb-0.2.3/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.3/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-12 05:32:53.611128 dnadb-0.2.3/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-12 05:32:53.000000 dnadb-0.2.3/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-12 05:32:53.000000 dnadb-0.2.3/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-12 05:32:53.000000 dnadb-0.2.3/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-12 05:32:53.000000 dnadb-0.2.3/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-12 05:32:53.000000 dnadb-0.2.3/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.2.2/LICENSE` & `dnadb-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/PKG-INFO` & `dnadb-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.2.2/pyproject.toml` & `dnadb-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.2.2/src/dnadb/datasets/dataset.py` & `dnadb-0.2.3/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb/datasets/greengenes.py` & `dnadb-0.2.3/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.2.3/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.2.3/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb/db.py` & `dnadb-0.2.3/src/dnadb/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class DbFactory:
     """
     A factory for creating LMDB-backed databases of FASTA entries.
     """
     def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
         self.path = Path(path)
         if self.path.suffix != ".db":
-            self.path = str(self.path) + ".db"
-        self.db = Lmdb.open(str(path), "n", lock=True)
+            self.path = Path(str(self.path) + ".db")
+        self.db = Lmdb.open(str(self.path), "n", lock=True)
         self.buffer: dict[Union[str, bytes], bytes] = {}
         self.chunk_size = chunk_size
 
     def flush(self):
         self.db.update(self.buffer)
         self.buffer.clear()
```

### Comparing `dnadb-0.2.2/src/dnadb/dna.py` & `dnadb-0.2.3/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb/fasta.py` & `dnadb-0.2.3/src/dnadb/fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import abc
 from functools import singledispatchmethod
 from lmdbm import Lmdb
 import numpy as np
 from pathlib import Path
 from typing import Generator, Iterable, TextIO, Tuple, Union
 
 from .db import DbFactory
```

### Comparing `dnadb-0.2.2/src/dnadb/fastq.py` & `dnadb-0.2.3/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb/taxonomy.py` & `dnadb-0.2.3/src/dnadb/taxonomy.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb/utils.py` & `dnadb-0.2.3/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.2/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.2.3/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

