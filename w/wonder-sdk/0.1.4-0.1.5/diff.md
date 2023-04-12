# Comparing `tmp/wonder-sdk-0.1.4.tar.gz` & `tmp/wonder-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.4.tar", last modified: Wed Apr 12 12:13:11 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.5.tar", last modified: Wed Apr 12 13:14:38 2023, max compression
```

## Comparing `wonder-sdk-0.1.4.tar` & `wonder-sdk-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:13:11.768364 wonder-sdk-0.1.4/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.4/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:13:11.768246 wonder-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 12:13:11.768410 wonder-sdk-0.1.4/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 12:13:07.000000 wonder-sdk-0.1.4/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:13:11.767530 wonder-sdk-0.1.4/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     4481 2023-04-12 12:13:02.000000 wonder-sdk-0.1.4/wonder_sdk/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)     1044 2023-04-12 12:03:33.000000 wonder-sdk-0.1.4/wonder_sdk/config.py
--rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.4/wonder_sdk/health.py
--rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.4/wonder_sdk/logger.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:13:11.768086 wonder-sdk-0.1.4/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 13:14:38.190318 wonder-sdk-0.1.5/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.5/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 13:14:38.190204 wonder-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 13:14:38.190363 wonder-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 13:14:17.000000 wonder-sdk-0.1.5/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 13:14:38.189509 wonder-sdk-0.1.5/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     4533 2023-04-12 13:13:59.000000 wonder-sdk-0.1.5/wonder_sdk/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)     1044 2023-04-12 12:03:33.000000 wonder-sdk-0.1.5/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      593 2023-04-12 13:13:21.000000 wonder-sdk-0.1.5/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.5/wonder_sdk/logger.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 13:14:38.190059 wonder-sdk-0.1.5/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 13:14:38.000000 wonder-sdk-0.1.5/wonder_sdk.egg-info/top_level.txt
```

### Comparing `wonder-sdk-0.1.4/LICENCE` & `wonder-sdk-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.4/wonder_sdk/__init__.py` & `wonder-sdk-0.1.5/wonder_sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import firebase_admin
 from firebase_admin import credentials, firestore
 from google.cloud import storage, pubsub_v1, translate_v2
 
 from .config import WonderSdkConfig
-from .health import start_health_check
+from .health import start_health_check, set_health_to_false
 from .logger import setup_logger
 
 class WonderSdk:
     def __init__(self, config: WonderSdkConfig, app_credentials=None):
         self._config = config
 
         start_health_check()
@@ -61,14 +61,16 @@
             try:
                 # When `timeout` is not set, result() will block indefinitely, unless an exception is encountered first.
                 streaming_pull_future.result(timeout=timeout)
             except Exception as e:
                 streaming_pull_future.cancel() # Trigger the shutdown.
                 streaming_pull_future.result() # Block until the shutdown is complete.
 
+        set_health_to_false()
+
     # TRANSLATION
     def _get_translate_client(self):
         if not hasattr(self, 'translate_client'):
             self.translate_client = translate_v2.Client()
 
         return self.translate_client
```

### Comparing `wonder-sdk-0.1.4/wonder_sdk/config.py` & `wonder-sdk-0.1.5/wonder_sdk/config.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.4/wonder_sdk/logger.py` & `wonder-sdk-0.1.5/wonder_sdk/logger.py`

 * *Files identical despite different names*

