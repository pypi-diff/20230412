# Comparing `tmp/bodo_platform_utils-0.0.6.tar.gz` & `tmp/bodo_platform_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodo_platform_utils-0.0.6.tar", last modified: Fri Sep 16 13:43:57 2022, max compression
+gzip compressed data, was "bodo_platform_utils-0.0.7.tar", last modified: Wed Apr 12 19:38:18 2023, max compression
```

## Comparing `bodo_platform_utils-0.0.6.tar` & `bodo_platform_utils-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 13:43:57.199482 bodo_platform_utils-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-16 13:43:57.199482 bodo_platform_utils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 13:43:57.199482 bodo_platform_utils-0.0.6/bodo_platform_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/bodo_platform_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-16 13:43:57.199482 bodo_platform_utils-0.0.6/bodo_platform_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/bodo_platform_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/bodo_platform_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/bodo_platform_utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/bodo_platform_utils/utils_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 13:43:57.199482 bodo_platform_utils-0.0.6/bodo_platform_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-16 13:43:57.000000 bodo_platform_utils-0.0.6/bodo_platform_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-16 13:43:57.000000 bodo_platform_utils-0.0.6/bodo_platform_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 13:43:57.000000 bodo_platform_utils-0.0.6/bodo_platform_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-16 13:43:57.000000 bodo_platform_utils-0.0.6/bodo_platform_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-16 13:43:57.000000 bodo_platform_utils-0.0.6/bodo_platform_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-09-16 13:43:57.199482 bodo_platform_utils-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    81180 2022-09-16 13:42:12.000000 bodo_platform_utils-0.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/bodo_platform_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/bodo_platform_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/utils_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/versioneer.py
```

### Comparing `bodo_platform_utils-0.0.6/LICENSE` & `bodo_platform_utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.6/PKG-INFO` & `bodo_platform_utils-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodo_platform_utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.0.6/bodo_platform_utils/config.py` & `bodo_platform_utils-0.0.7/bodo_platform_utils/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from bodo_platform_utils.utils_types import CloudProvider
 
 WORKSPACE_UUID = os.environ.get("BODO_PLATFORM_WORKSPACE_UUID")
 REGION = os.environ.get("BODO_PLATFORM_WORKSPACE_REGION")
-# Default to AWS for now.
 CLOUD_PROVIDER = CloudProvider(
-    os.environ.get("BODO_PLATFORM_WORKSPACE_CLOUD_PROVIDER", "AWS")
+    os.environ.get("BODO_PLATFORM_CLOUD_PROVIDER")
 )
 
 # This is related to Snowflake Partner Connect, we use the same constant in the backend
 # to store the data coming from Partner Connect.
 SNOWFLAKE_PC_CATALOG_NAME = 'snowflake_pc'
 
 CATALOG_PREFIX = "catalog-secret"
```

### Comparing `bodo_platform_utils-0.0.6/bodo_platform_utils.egg-info/PKG-INFO` & `bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodo-platform-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.0.6/setup.py` & `bodo_platform_utils-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.6/versioneer.py` & `bodo_platform_utils-0.0.7/versioneer.py`

 * *Files identical despite different names*

