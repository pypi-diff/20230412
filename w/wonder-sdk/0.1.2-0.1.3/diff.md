# Comparing `tmp/wonder-sdk-0.1.2.tar.gz` & `tmp/wonder-sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.2.tar", last modified: Wed Apr 12 11:55:34 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.3.tar", last modified: Wed Apr 12 12:05:29 2023, max compression
```

## Comparing `wonder-sdk-0.1.2.tar` & `wonder-sdk-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:55:34.195343 wonder-sdk-0.1.2/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.2/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 11:55:34.195223 wonder-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 11:55:34.195385 wonder-sdk-0.1.2/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 11:55:31.000000 wonder-sdk-0.1.2/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:55:34.194528 wonder-sdk-0.1.2/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     4231 2023-04-12 11:55:01.000000 wonder-sdk-0.1.2/wonder_sdk/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      742 2023-04-12 11:37:03.000000 wonder-sdk-0.1.2/wonder_sdk/config.py
--rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.2/wonder_sdk/health.py
--rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.2/wonder_sdk/logger.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:55:34.195074 wonder-sdk-0.1.2/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:05:29.012332 wonder-sdk-0.1.3/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.3/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:05:29.012205 wonder-sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 12:05:29.012375 wonder-sdk-0.1.3/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 12:05:13.000000 wonder-sdk-0.1.3/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:05:29.011471 wonder-sdk-0.1.3/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     4433 2023-04-12 12:04:56.000000 wonder-sdk-0.1.3/wonder_sdk/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)     1044 2023-04-12 12:03:33.000000 wonder-sdk-0.1.3/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.3/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.3/wonder_sdk/logger.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:05:29.012052 wonder-sdk-0.1.3/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/top_level.txt
```

### Comparing `wonder-sdk-0.1.2/LICENCE` & `wonder-sdk-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.2/wonder_sdk/__init__.py` & `wonder-sdk-0.1.3/wonder_sdk/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,20 +21,24 @@
     # FIRESTORE
     def get_firestore_client(self):
         if not hasattr(self, 'db'):
             self.db = firestore.client()
 
         return self.db
 
-    def set_firestore_data(self, collection_name, document_name, data):
+    def set_firestore_data(self, document_name, data, collection_name=None):
+        collection_name = collection_name if collection_name else self._config.collection_name
+
         db = self.get_firestore_client()
         doc_ref = db.collection(collection_name).document(document_name)
         doc_ref.set(data)
 
-    def get_firestore_data(self, collection_name, document_name):
+    def get_firestore_data(self, document_name, collection_name=None):
+        collection_name = collection_name if collection_name else self._config.collection_name
+
         db = self.get_firestore_client()
         doc_ref = db.collection(collection_name).document(document_name)
         doc = doc_ref.get()
         return doc.to_dict()
 
     # PUB/SUB
     def subscribe_to_pubsub(self, max_messages: int, callback, timeout=None):
```

### Comparing `wonder-sdk-0.1.2/wonder_sdk/config.py` & `wonder-sdk-0.1.3/wonder_sdk/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 import os
 
 class EnvironmentTypes:
     production = 'production'
     staging = 'staging'
 
 class WonderSdkConfig:
-    def __init__(self, environment=None, project_id=None, subscription_name=None, process_count=None) -> None:
+    def __init__(
+            self,
+            environment=None,
+            project_id=None,
+            subscription_name=None,
+            process_count=None,
+            production_collection_name=None,
+            staging_collection_name=None
+        ) -> None:
         self.environment_types = EnvironmentTypes()
 
         self.environment = environment if environment else os.environ.get('ENVIRONMENT', self.environment_types.staging)
 
         self.project_id = project_id if project_id else os.environ.get('PROJECT_ID', default=None)
         
         self.subscription_name = subscription_name if subscription_name else os.environ.get('SUBSCRIPTION_NAME', default=None)
 
-        self.process_count = process_count if process_count else os.environ.get('PROCESS_COUNT', default=1)
+        self.process_count = process_count if process_count else os.environ.get('PROCESS_COUNT', default=1)
+
+        self.collection_name = production_collection_name if self.environment == self.environment_types.production else staging_collection_name
```

### Comparing `wonder-sdk-0.1.2/wonder_sdk/health.py` & `wonder-sdk-0.1.3/wonder_sdk/health.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.2/wonder_sdk/logger.py` & `wonder-sdk-0.1.3/wonder_sdk/logger.py`

 * *Files identical despite different names*

