# Comparing `tmp/wonder-sdk-0.1.6.tar.gz` & `tmp/wonder-sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.6.tar", last modified: Wed Apr 12 14:44:17 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.7.tar", last modified: Wed Apr 12 14:56:48 2023, max compression
```

## Comparing `wonder-sdk-0.1.6.tar` & `wonder-sdk-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:44:17.568424 wonder-sdk-0.1.6/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.6/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:44:17.568267 wonder-sdk-0.1.6/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 14:44:17.568469 wonder-sdk-0.1.6/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 14:43:58.000000 wonder-sdk-0.1.6/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:44:17.567544 wonder-sdk-0.1.6/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     4533 2023-04-12 14:43:40.000000 wonder-sdk-0.1.6/wonder_sdk/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)     1049 2023-04-12 14:36:42.000000 wonder-sdk-0.1.6/wonder_sdk/config.py
--rw-r--r--   0 basri      (501) staff       (20)      593 2023-04-12 13:13:21.000000 wonder-sdk-0.1.6/wonder_sdk/health.py
--rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.6/wonder_sdk/logger.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:44:17.568096 wonder-sdk-0.1.6/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 14:44:17.000000 wonder-sdk-0.1.6/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:56:48.295271 wonder-sdk-0.1.7/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.7/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:56:48.295103 wonder-sdk-0.1.7/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 14:56:48.295327 wonder-sdk-0.1.7/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 14:56:42.000000 wonder-sdk-0.1.7/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:56:48.294382 wonder-sdk-0.1.7/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     4732 2023-04-12 14:56:27.000000 wonder-sdk-0.1.7/wonder_sdk/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)     1049 2023-04-12 14:36:42.000000 wonder-sdk-0.1.7/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      593 2023-04-12 13:13:21.000000 wonder-sdk-0.1.7/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.7/wonder_sdk/logger.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:56:48.294955 wonder-sdk-0.1.7/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/top_level.txt
```

### Comparing `wonder-sdk-0.1.6/LICENCE` & `wonder-sdk-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.6/wonder_sdk/__init__.py` & `wonder-sdk-0.1.7/wonder_sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,21 @@
         start_health_check()
         self.logger = setup_logger()
 
         self._firebase_cred = credentials.Certificate(app_credentials) if app_credentials else credentials.ApplicationDefault()
         firebase_admin.initialize_app(self._firebase_cred, {
             'projectId': self._config.project_id
         })
+    
+    # ENVIRONMENT VARIABLE GETTERS
+    def get_process_count(self):
+        return self._config.process_count
+
+    def get_subscription_name(self):
+        return self._config.subscription_name
 
     # FIRESTORE
     def get_firestore_client(self):
         if not hasattr(self, 'db'):
             self.db = firestore.client()
 
         return self.db
```

### Comparing `wonder-sdk-0.1.6/wonder_sdk/config.py` & `wonder-sdk-0.1.7/wonder_sdk/config.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.6/wonder_sdk/health.py` & `wonder-sdk-0.1.7/wonder_sdk/health.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.6/wonder_sdk/logger.py` & `wonder-sdk-0.1.7/wonder_sdk/logger.py`

 * *Files identical despite different names*

