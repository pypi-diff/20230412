# Comparing `tmp/halo-reader-0.0.7.tar.gz` & `tmp/halo-reader-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halo-reader-0.0.7.tar", last modified: Mon Apr  3 09:42:24 2023, max compression
+gzip compressed data, was "halo-reader-0.0.8.tar", last modified: Wed Apr 12 11:30:47 2023, max compression
```

## Comparing `halo-reader-0.0.7.tar` & `halo-reader-0.0.8.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:24.003299 halo-reader-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-03 09:42:02.000000 halo-reader-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-03 09:42:02.000000 halo-reader-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-03 09:42:24.003299 halo-reader-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-03 09:42:02.000000 halo-reader-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-03 09:42:02.000000 halo-reader-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 09:42:24.003299 halo-reader-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-03 09:42:02.000000 halo-reader-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.995299 halo-reader-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.995299 halo-reader-0.0.7/src/halo_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/halo_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/halo_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/halo_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/halo_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/halo_reader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/halo_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/halo_reader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.995299 halo-reader-0.0.7/src/haloboard/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloboard/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.995299 halo-reader-0.0.7/src/haloboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloboard/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloboard/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.995299 halo-reader-0.0.7/src/haloboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloboard/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.999299 halo-reader-0.0.7/src/halodata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/halodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/halodata/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.999299 halo-reader-0.0.7/src/haloreader/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/attenuated_backscatter_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/background_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:23.999299 halo-reader-0.0.7/src/haloreader/background_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-03 09:42:22.000000 halo-reader-0.0.7/src/haloreader/background_reader/background_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/background_reader/background_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:24.003299 halo-reader-0.0.7/src/haloreader/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-03 09:42:23.000000 halo-reader-0.0.7/src/haloreader/data_reader/data_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/data_reader/data_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/grammar_header.lark
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/halo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/read.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/type_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 09:42:02.000000 halo-reader-0.0.7/src/haloreader/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:42:24.003299 halo-reader-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-03 09:42:02.000000 halo-reader-0.0.7/tests/test_halo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 11:30:24.000000 halo-reader-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 11:30:24.000000 halo-reader-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 11:30:47.855285 halo-reader-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-12 11:30:24.000000 halo-reader-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-12 11:30:24.000000 halo-reader-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:30:47.855285 halo-reader-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 11:30:24.000000 halo-reader-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.843284 halo-reader-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/halo_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/haloboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/haloboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/haloboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/halodata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/halodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/halodata/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.851285 halo-reader-0.0.8/src/haloreader/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/attenuated_backscatter_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/background_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/src/haloreader/background_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-12 11:30:45.000000 halo-reader-0.0.8/src/haloreader/background_reader/background_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/background_reader/background_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/src/haloreader/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-12 11:30:46.000000 halo-reader-0.0.8/src/haloreader/data_reader/data_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/data_reader/data_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/grammar_header.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/halo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/type_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-12 11:30:24.000000 halo-reader-0.0.8/tests/test_halo_reader.py
```

### Comparing `halo-reader-0.0.7/LICENSE` & `halo-reader-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/PKG-INFO` & `halo-reader-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.0.7
+Version: 0.0.8
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.0.7/README.md` & `halo-reader-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/pyproject.toml` & `halo-reader-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/setup.py` & `halo-reader-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/halo_reader.egg-info/PKG-INFO` & `halo-reader-0.0.8/src/halo_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.0.7
+Version: 0.0.8
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.0.7/src/halo_reader.egg-info/SOURCES.txt` & `halo-reader-0.0.8/src/halo_reader.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/haloreader/exceptions.py
 src/haloreader/grammar_header.lark
 src/haloreader/halo.py
 src/haloreader/metadata.py
 src/haloreader/py.typed
 src/haloreader/read.py
 src/haloreader/scantype.py
+src/haloreader/screen.py
 src/haloreader/transformer.py
 src/haloreader/type_guards.py
 src/haloreader/utils.py
 src/haloreader/variable.py
 src/haloreader/version.py
 src/haloreader/background_reader/background_reader.c
 src/haloreader/background_reader/background_reader.pyx
```

### Comparing `halo-reader-0.0.7/src/haloboard/app.py` & `halo-reader-0.0.8/src/haloboard/app.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloboard/static/favicon.ico` & `halo-reader-0.0.8/src/haloboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloboard/static/style.css` & `halo-reader-0.0.8/src/haloboard/static/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 main {
   display: flex;
   justify-content: center;
 }
 .container {
   display: flex;
   flex-direction: column;
-  width: min(100vw, 1200px);
+  width: min(100vw, 1800px);
 
 }
 .input-filter {
   display: flex;
   justify-content: center;
 }
 .input-filter input {
```

### Comparing `halo-reader-0.0.7/src/haloboard/templates/index.html` & `halo-reader-0.0.8/src/haloboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/halodata/datasets.py` & `halo-reader-0.0.8/src/halodata/datasets.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/attenuated_backscatter_coefficient.py` & `halo-reader-0.0.8/src/haloreader/attenuated_backscatter_coefficient.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,22 @@
         optical frequency
     h
         planc's constant
     c
         speed of light
     B
         reveiver bandwidth
+
+    References
+    ----------
+    Methodology for deriving the telescope focus function and
+    its uncertainty for a heterodyne pulsed Doppler lidar
+        authors:  Pyry Pentikäinen, Ewan James O'Connor,
+            Antti Juhani Manninen, and Pablo Ortiz-Amezcua
+        doi: https://doi.org/10.5194/amt-13-2849-2020
     """
     if not is_ndarray(intensity.data):
         raise TypeError
     if not is_ndarray(range_.data):
         raise TypeError
 
     r = range_.data
@@ -51,16 +59,18 @@
     B = 5e7
     A_e = compute_effective_receiver_energy(range_, focus, lambda_)
     snr = intensity.data - 1
     # ref: https://doi.org/10.5194/amt-13-2849-2020
     beta = 2 * h * nu * B * r**2 * snr / (eta * c * E * A_e)
     return Variable(
         name="beta",
-        long_name="Attenuated backscatter coefficient",
-        comment="Computed using placeholder values. Do not use this variable",
+        long_name="attenuated backscatter coefficient",
+        comment=(
+            "Experimental variable. Computed using uncalibrated/placeholder values."
+        ),
         units="m-1 sr-1",
         dimensions=intensity.dimensions,
         data=beta,
     )
 
 
 def compute_effective_receiver_energy(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `halo-reader-0.0.7/src/haloreader/attribute.py` & `halo-reader-0.0.8/src/haloreader/attribute.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,21 +10,33 @@
 
 
 @dataclass(slots=True)
 class Attribute:
     name: str
     value: str | ScanType | list[str]
 
-    def nc_write(self, nc: netCDF4.Dataset) -> None:
+    def nc_write(
+        self,
+        nc: netCDF4.Dataset,
+        nc_map: dict[str, dict] | None = None,
+        nc_exclude: dict[str, set] | None = None,
+    ) -> None:
+        nc_exclude_attr = (
+            nc_exclude.get("attributes", set()) if nc_exclude is not None else set()
+        )
+        if self.name in nc_exclude_attr:
+            return
+        nc_map_attr = nc_map.get("attributes", {}) if nc_map is not None else {}
+        name = nc_map_attr.get(self.name, self.name)
         if isinstance(self.value, str):
-            setattr(nc, self.name, self.value)
+            setattr(nc, name, self.value)
         elif isinstance(self.value, ScanType):
-            setattr(nc, self.name, str(self.value))
+            setattr(nc, name, str(self.value))
         elif is_str_list(self.value):
-            setattr(nc, self.name, "\n".join(self.value))
+            setattr(nc, name, "\n".join(self.value))
 
     @classmethod
     def is_attribute_list(cls, val: list[Any]) -> TypeGuard[list[Attribute]]:
         return all(isinstance(x, Attribute) for x in val)
 
     @classmethod
     def merge(cls, attributes: list[Attribute]) -> Attribute | None:
```

### Comparing `halo-reader-0.0.7/src/haloreader/background_correction.py` & `halo-reader-0.0.8/src/haloreader/background_correction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 import numpy as np
-from scipy.ndimage import gaussian_filter  # mypy:
+from scipy.ndimage import gaussian_filter
 from scipy.signal import medfilt2d
 
+from haloreader.exceptions import BackgroundCorrectionError
 from haloreader.type_guards import is_ndarray
 from haloreader.variable import Variable
 
 
 def background_measurement_correction(
     time: Variable,
     intensity: Variable,
     time_bg: Variable,
     bg: Variable,
     p_amp: Variable,
 ) -> Variable:
-    # ref: https://doi.org/10.5194/amt-12-839-2019
+    """
+    References
+    ----------
+    A novel post-processing algorithm for Halo Doppler lidars
+        authors:  Ville Vakkari, Antti J. Manninen, Ewan J. O'Connor,
+            Jan H. Schween, Pieter G. van Zyl, and Eleni Marinou
+        doi: https://doi.org/10.5194/amt-12-839-2019
+    """
     if not is_ndarray(time.data):
         raise TypeError
     if not is_ndarray(intensity.data):
         raise TypeError
     if not is_ndarray(time_bg.data):
         raise TypeError
     if not is_ndarray(bg.data):
         raise TypeError
     if not is_ndarray(p_amp.data):
         raise TypeError
-    intensity_index2bg_index = _previous_measurement_map(time.data, time_bg.data)
+    try:
+        intensity_index2bg_index = _previous_measurement_map(time.data, time_bg.data)
+    except ValueError as err:
+        raise BackgroundCorrectionError(
+            "Cannot find matching background measurement for all profiles"
+        ) from err
     relevant_bg_indeces = sorted(list(set(intensity_index2bg_index)))
     relevant_bg_indeces_map = {v: i for i, v in enumerate(relevant_bg_indeces)}
     intensity_index2relevant_bg_index = np.array(
         [relevant_bg_indeces_map[i] for i in intensity_index2bg_index]
     )
     bg_relevant = bg.take(relevant_bg_indeces)
     if not is_ndarray(bg_relevant.data):
```

### Comparing `halo-reader-0.0.7/src/haloreader/background_reader/background_reader.c` & `halo-reader-0.0.8/src/haloreader/background_reader/background_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/background_reader/background_reader.pyx` & `halo-reader-0.0.8/src/haloreader/background_reader/background_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/cli.py` & `halo-reader-0.0.8/src/haloreader/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,28 +31,35 @@
         return
     if halobg is None:
         raise TypeError
     log.info("Correct background")
     halo.correct_background(halobg)
     log.info("Compute beta")
     halo.compute_beta()
+    log.info("Compute noise screen")
+    screen = halo.compute_noise_screen()
+    log.info("Compute screened beta")
+    halo.compute_beta_screened(screen)
+    log.info("Compute screened doppler velocity")
+    halo.compute_doppler_velocity_screened(screen)
     log.info("Convert timeunits")
     halo.convert_time_unit2cloudnet_time()
     log.info("Create netCDF")
     nc_buff = halo.to_nc()
     with open(f"halo_{args.site}_{args.date}.nc", "wb") as f:
         f.write(nc_buff)
     if args.plot:
         log.info("Create plots")
         writer = Writer()
         fig, ax = plt.subplots(3, 1, figsize=(24, 16))
         halo.intensity_raw.plot(ax[0])
         halo.doppler_velocity.plot(ax[1])
         if halo.intensity is not None:
             halo.intensity.plot(ax[2])
+
         writer.add_figure(f"halo_{args.site}_{args.date}", fig)
 
 
 def _from_raw(args: argparse.Namespace) -> None:
     halo_src = [src for src in args.src if src.name.endswith(".hpl")]
     bg_src = [
         src
```

### Comparing `halo-reader-0.0.7/src/haloreader/data_reader/data_reader.c` & `halo-reader-0.0.8/src/haloreader/data_reader/data_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/data_reader/data_reader.pyx` & `halo-reader-0.0.8/src/haloreader/data_reader/data_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/grammar_header.lark` & `halo-reader-0.0.8/src/haloreader/grammar_header.lark`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/halo.py` & `halo-reader-0.0.8/src/haloreader/halo.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Protocol, TypeGuard, runtime_checkable
 
 import netCDF4
 import numpy as np
 
 import haloreader.attenuated_backscatter_coefficient
 import haloreader.background_correction
+import haloreader.screen
 from haloreader.metadata import Metadata
 from haloreader.type_guards import is_fancy_index, is_ndarray, is_none_list
 from haloreader.utils import CLOUDNET_TIME_UNIT_FMT, UNIX_TIME_FMT, UNIX_TIME_UNIT
 from haloreader.variable import Variable, VariableWithNumpyData
 
 log = logging.getLogger(__name__)
 
@@ -30,23 +31,27 @@
     roll: Variable
     doppler_velocity: Variable
     intensity_raw: Variable
     beta_raw: Variable
     spectral_width: Variable | None = None
     intensity: Variable | None = None
     beta: Variable | None = None
+    beta_screened: Variable | None = None
+    doppler_velocity_screened: Variable | None = None
 
-    def to_nc(self) -> memoryview:
+    def to_nc(
+        self,
+        nc_map: dict[str, dict] | None = None,
+        nc_exclude: dict[str, set] | None = None,
+    ) -> memoryview:
         nc = netCDF4.Dataset("inmemory.nc", "w", memory=1028)
-        self.time.nc_create_dimension(nc)
-        self.range.nc_create_dimension(nc)
         for attr_name in self.__dataclass_fields__.keys():
             halo_attr = getattr(self, attr_name)
             if halo_attr is not None:
-                halo_attr.nc_write(nc)
+                halo_attr.nc_write(nc, nc_map=nc_map, nc_exclude=nc_exclude)
         nc_buf = nc.close()
         if isinstance(nc_buf, memoryview):
             return nc_buf
         raise TypeError
 
     @classmethod
     def merge(cls, halos: list[Halo]) -> Halo | None:
@@ -123,27 +128,50 @@
         self.intensity = haloreader.background_correction.snr_correction(
             intensity_step1, signalmask
         )
 
     def compute_beta(self) -> None:
         if not isinstance(self.intensity, Variable):
             raise TypeError
-        beta = haloreader.attenuated_backscatter_coefficient.compute_beta(
+        log.warning("beta is computed using placeholder values")
+        self.beta = haloreader.attenuated_backscatter_coefficient.compute_beta(
             self.intensity, self.range, self.metadata.focus_range
         )
-        if not is_ndarray(self.beta_raw.data) or not is_ndarray(beta.data):
+
+    def compute_noise_screen(self) -> Variable:
+        if not isinstance(self.intensity, Variable):
+            raise TypeError
+        return haloreader.screen.compute_noise_screen(
+            self.intensity, self.doppler_velocity
+        )
+
+    def compute_beta_screened(self, screen: Variable) -> None:
+        if not isinstance(self.beta, Variable):
+            raise TypeError
+        self.beta_screened = Variable(
+            name="beta_screened",
+            long_name="screened attenuated backscatter coefficient",
+            comment=(
+                "Experimental variable. Computed using uncalibrated/placeholder values."
+            ),
+            units="m-1 sr-1",
+            dimensions=self.beta.dimensions,
+            data=np.ma.masked_array(self.beta.data, mask=screen.data),
+        )
+
+    def compute_doppler_velocity_screened(self, screen: Variable) -> None:
+        if not isinstance(self.beta, Variable):
             raise TypeError
-        placeholder_scale = self.beta_raw.data.mean() / beta.data.mean()
-        log.warning(
-            "beta is computed using placeholder values"
-            "and then scaled by %0.3f to match values from raw beta",
-            placeholder_scale,
+        self.doppler_velocity_screened = Variable(
+            name="doppler_velocity_screened",
+            long_name="screened radial velocity (positive away from lidar)",
+            units=self.doppler_velocity.units,
+            dimensions=self.doppler_velocity.dimensions,
+            data=np.ma.masked_array(self.doppler_velocity.data, mask=screen.data),
         )
-        beta.data = placeholder_scale * beta.data
-        self.beta = beta
 
 
 def _convert_timevar_unit2cloudnet_time(var: Variable) -> None:
     """Converts time variable to cloudnet format.
 
     Format is: hours since [beginning of the day of the first
     measurement]
```

### Comparing `halo-reader-0.0.7/src/haloreader/metadata.py` & `halo-reader-0.0.8/src/haloreader/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,39 +23,49 @@
     scantype: Attribute
     focus_range: Variable
     start_time: Variable
     resolution: Variable
     nrays: Variable | None = None
     nwaypoints: Variable | None = None
     instrument_spectral_width: Variable | None = None
+    wavelength: Variable | None = field(
+        default_factory=lambda: Variable(
+            name="wavelength",
+            standard_name="radiation_wavelength",
+            units="m",
+            data=1.5e-6,
+        )
+    )
     haloreader_version: Attribute = field(
         default_factory=lambda: Attribute(name="haloreader_version", value=pkgversion)
     )
     conventions: Attribute = field(
         default_factory=lambda: Attribute(name="Conventions", value="CF-1.8")
     )
 
-    def nc_write(self, nc: netCDF4.Dataset) -> None:
-        # nc_meta = nc.createGroup("metadata")
-        nc_meta = nc
+    def nc_write(
+        self,
+        nc: netCDF4.Dataset,
+        nc_map: dict[str, dict] | None = None,
+        nc_exclude: dict[str, set] | None = None,
+    ) -> None:
         for attr_name in self.__dataclass_fields__.keys():
             metadata_attr = getattr(self, attr_name)
             if metadata_attr is not None:
-                metadata_attr.nc_write(nc_meta)
+                metadata_attr.nc_write(nc, nc_map=nc_map, nc_exclude=nc_exclude)
 
     @classmethod
     def merge(cls, metadata_list: list[Metadata]) -> Metadata | None:
         if len(metadata_list) == 0:
             return None
         if len(metadata_list) == 1:
             return metadata_list[0]
         metadata_attrs: dict[str, Any] = {}
         for attr_name in cls.__dataclass_fields__.keys():
             metadata_attr_list = [getattr(md, attr_name) for md in metadata_list]
-
             if Attribute.is_attribute_list(metadata_attr_list):
                 metadata_attrs[attr_name] = Attribute.merge(metadata_attr_list)
             elif Variable.is_variable_list(metadata_attr_list):
                 metadata_attrs[attr_name] = Variable.merge(metadata_attr_list)
             elif is_none_list(metadata_attr_list):
                 metadata_attrs[attr_name] = None
             else:
```

### Comparing `halo-reader-0.0.7/src/haloreader/read.py` & `halo-reader-0.0.8/src/haloreader/read.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/scantype.py` & `halo-reader-0.0.8/src/haloreader/scantype.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/transformer.py` & `halo-reader-0.0.8/src/haloreader/transformer.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/type_guards.py` & `halo-reader-0.0.8/src/haloreader/type_guards.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/utils.py` & `halo-reader-0.0.8/src/haloreader/utils.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.7/src/haloreader/variable.py` & `halo-reader-0.0.8/src/haloreader/variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,21 +33,34 @@
     @classmethod
     def is_variable_list(cls, val: list[Any]) -> TypeGuard[list[Variable]]:
         return all(isinstance(x, Variable) for x in val)
 
     def nc_create_dimension(self, nc: netCDF4.Dataset) -> None:
         nc.createDimension(self.name, None)
 
-    def nc_write(self, nc: netCDF4.Dataset) -> None:
+    def nc_write(
+        self,
+        nc: netCDF4.Dataset,
+        nc_map: dict[str, dict] | None = None,
+        nc_exclude: dict[str, set] | None = None,
+    ) -> None:
+        nc_exclude_var = (
+            nc_exclude.get("variables", set()) if nc_exclude is not None else set()
+        )
+        if self.name in nc_exclude_var:
+            return
+        nc_map_var = nc_map.get("variables", {}) if nc_map is not None else {}
+        var_name = nc_map_var.get(self.name, self.name)
         nc_dtype = _choose_nc_dtype(self)
         dimensions = self.dimensions if self.dimensions is not None else ()
-        for dim in dimensions:
+        mapped_dimensions = tuple((nc_map_var.get(dim, dim) for dim in dimensions))
+        for dim in mapped_dimensions:
             if not _dimension_exists(nc, dim):
                 nc.createDimension(dim, None)
-        nc_var = nc.createVariable(self.name, nc_dtype, dimensions, zlib=True)
+        nc_var = nc.createVariable(var_name, nc_dtype, mapped_dimensions, zlib=True)
         nc_var[:] = self.data if self.data is not None else []
         for attr_name in set(self.__dataclass_fields__.keys()) - {
             "name",
             "dimensions",
             "data",
         }:
             attr_val = getattr(self, attr_name)
@@ -56,15 +69,14 @@
 
     @classmethod
     def like(
         cls,
         var: Variable,
         data: DataType,
     ) -> Variable:
-        # pylint: disable=too-many-arguments
         return Variable(
             **{
                 attr_name: getattr(var, attr_name)
                 for attr_name in set(var.__dataclass_fields__.keys()) - {"data"}
             },
             data=data,
         )
@@ -184,19 +196,19 @@
     if dim in nc.dimensions:
         return True
     return _dimension_exists(nc.parent, dim)
 
 
 def _choose_nc_dtype(var: Variable) -> str:
     if var.data is None:
-        return "f8"
+        return "f4"
     if isinstance(var.data, float):
-        return "f8"
+        return "f4"
     if isinstance(var.data, int):
-        return "i8"
+        return "i4"
     if isinstance(var.data, np.ndarray):
         if var.name == "time" and var.data.dtype.kind == "f":
             return "f8"
         if var.data.dtype.kind == "f":
             return "f4"
         if var.data.dtype.kind == "i":
             return "i4"
```

### Comparing `halo-reader-0.0.7/tests/test_halo_reader.py` & `halo-reader-0.0.8/tests/test_halo_reader.py`

 * *Files identical despite different names*

