# Comparing `tmp/macrometa-target-collection-0.0.47.tar.gz` & `tmp/macrometa-target-collection-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.47.tar", last modified: Thu Apr  6 17:23:30 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.48.tar", last modified: Wed Apr 12 14:55:22 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.47.tar` & `macrometa-target-collection-0.0.48.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:23:30.386081 macrometa-target-collection-0.0.47/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-06 17:23:09.000000 macrometa-target-collection-0.0.47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-06 17:23:30.386081 macrometa-target-collection-0.0.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-06 17:23:09.000000 macrometa-target-collection-0.0.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:23:30.386081 macrometa-target-collection-0.0.47/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-06 17:23:09.000000 macrometa-target-collection-0.0.47/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13048 2023-04-06 17:23:09.000000 macrometa-target-collection-0.0.47/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:23:30.386081 macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-06 17:23:30.000000 macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-06 17:23:30.000000 macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 17:23:30.000000 macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 17:23:30.000000 macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-06 17:23:30.000000 macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 17:23:30.000000 macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-06 17:23:09.000000 macrometa-target-collection-0.0.47/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-06 17:23:30.386081 macrometa-target-collection-0.0.47/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.790713 macrometa-target-collection-0.0.48/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 14:55:01.000000 macrometa-target-collection-0.0.48/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 14:55:22.790713 macrometa-target-collection-0.0.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 14:55:01.000000 macrometa-target-collection-0.0.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.790713 macrometa-target-collection-0.0.48/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 14:55:01.000000 macrometa-target-collection-0.0.48/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13050 2023-04-12 14:55:01.000000 macrometa-target-collection-0.0.48/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.790713 macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 14:55:22.000000 macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 14:55:22.000000 macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:55:22.000000 macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 14:55:22.000000 macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 14:55:22.000000 macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 14:55:22.000000 macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 14:55:01.000000 macrometa-target-collection-0.0.48/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 14:55:22.790713 macrometa-target-collection-0.0.48/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.47/LICENSE` & `macrometa-target-collection-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.47/PKG-INFO` & `macrometa-target-collection-0.0.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.47
+Version: 0.0.48
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.47/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.48/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.47/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.48/macrometa_target_collection/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 # Increment ingest_errors metric
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 logger.error(f"Failed parsing the json schema for stream: {stream}.")
                 raise e
 
             try:
                 rec = o['record']
-                if o["time_extracted"]:
+                if 'time_extracted' in o:
                     rec["time_extracted"] = o["time_extracted"]
                 else:
                     rec["time_extracted"] = record_batch.last_executed_time
                 try:
                     kps = key_properties.get(stream)
                     _key = None
                     # Appending _ to keys inorder for preserving values of reserved keys in source data
```

### Comparing `macrometa-target-collection-0.0.47/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.48/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.47
+Version: 0.0.48
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.47/pyproject.toml` & `macrometa-target-collection-0.0.48/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.47"
+version = "0.0.48"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

