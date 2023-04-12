# Comparing `tmp/wonder-sdk-0.1.5.tar.gz` & `tmp/wonder-sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.5.tar", last modified: Wed Apr 12 13:14:38 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.6.tar", last modified: Wed Apr 12 14:44:17 2023, max compression
```

## Comparing `wonder-sdk-0.1.5.tar` & `wonder-sdk-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 13:14:38.190318 wonder-sdk-0.1.5/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.5/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 13:14:38.190204 wonder-sdk-0.1.5/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 13:14:38.190363 wonder-sdk-0.1.5/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 13:14:17.000000 wonder-sdk-0.1.5/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 13:14:38.189509 wonder-sdk-0.1.5/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     4533 2023-04-12 13:13:59.000000 wonder-sdk-0.1.5/wonder_sdk/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)     1044 2023-04-12 12:03:33.000000 wonder-sdk-0.1.5/wonder_sdk/config.py
--rw-r--r--   0 basri      (501) staff       (20)      593 2023-04-12 13:13:21.000000 wonder-sdk-0.1.5/wonder_sdk/health.py
--rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.5/wonder_sdk/logger.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 13:14:38.190059 wonder-sdk-0.1.5/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:44:17.568424 wonder-sdk-0.1.6/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.6/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:44:17.568267 wonder-sdk-0.1.6/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 14:44:17.568469 wonder-sdk-0.1.6/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 14:43:58.000000 wonder-sdk-0.1.6/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:44:17.567544 wonder-sdk-0.1.6/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     4533 2023-04-12 14:43:40.000000 wonder-sdk-0.1.6/wonder_sdk/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)     1049 2023-04-12 14:36:42.000000 wonder-sdk-0.1.6/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      593 2023-04-12 13:13:21.000000 wonder-sdk-0.1.6/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.6/wonder_sdk/logger.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:44:17.568096 wonder-sdk-0.1.6/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/top_level.txt
```

### Comparing `wonder-sdk-0.1.5/LICENCE` & `wonder-sdk-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.5/wonder_sdk/__init__.py` & `wonder-sdk-0.1.6/wonder_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.5/wonder_sdk/config.py` & `wonder-sdk-0.1.6/wonder_sdk/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
         self.environment = environment if environment else os.environ.get('ENVIRONMENT', self.environment_types.staging)
 
         self.project_id = project_id if project_id else os.environ.get('PROJECT_ID', default=None)
         
         self.subscription_name = subscription_name if subscription_name else os.environ.get('SUBSCRIPTION_NAME', default=None)
 
-        self.process_count = process_count if process_count else os.environ.get('PROCESS_COUNT', default=1)
+        self.process_count = process_count if process_count else int(os.environ.get('PROCESS_COUNT', default=1))
 
         self.collection_name = production_collection_name if self.environment == self.environment_types.production else staging_collection_name
```

### Comparing `wonder-sdk-0.1.5/wonder_sdk/health.py` & `wonder-sdk-0.1.6/wonder_sdk/health.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.5/wonder_sdk/logger.py` & `wonder-sdk-0.1.6/wonder_sdk/logger.py`

 * *Files identical despite different names*

