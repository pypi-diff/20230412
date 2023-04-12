# Comparing `tmp/wonder-sdk-0.1.7.tar.gz` & `tmp/wonder-sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.7.tar", last modified: Wed Apr 12 14:56:48 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.8.tar", last modified: Wed Apr 12 15:35:17 2023, max compression
```

## Comparing `wonder-sdk-0.1.7.tar` & `wonder-sdk-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:56:48.295271 wonder-sdk-0.1.7/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.7/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:56:48.295103 wonder-sdk-0.1.7/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 14:56:48.295327 wonder-sdk-0.1.7/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 14:56:42.000000 wonder-sdk-0.1.7/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:56:48.294382 wonder-sdk-0.1.7/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     4732 2023-04-12 14:56:27.000000 wonder-sdk-0.1.7/wonder_sdk/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)     1049 2023-04-12 14:36:42.000000 wonder-sdk-0.1.7/wonder_sdk/config.py
--rw-r--r--   0 basri      (501) staff       (20)      593 2023-04-12 13:13:21.000000 wonder-sdk-0.1.7/wonder_sdk/health.py
--rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.7/wonder_sdk/logger.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 14:56:48.294955 wonder-sdk-0.1.7/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 14:56:48.000000 wonder-sdk-0.1.7/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 15:35:17.220667 wonder-sdk-0.1.8/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.8/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 15:35:17.220532 wonder-sdk-0.1.8/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 15:35:17.220713 wonder-sdk-0.1.8/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 15:34:16.000000 wonder-sdk-0.1.8/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 15:35:17.219768 wonder-sdk-0.1.8/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     4728 2023-04-12 15:28:37.000000 wonder-sdk-0.1.8/wonder_sdk/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)     1049 2023-04-12 15:05:49.000000 wonder-sdk-0.1.8/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      593 2023-04-12 13:13:21.000000 wonder-sdk-0.1.8/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.8/wonder_sdk/logger.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 15:35:17.220345 wonder-sdk-0.1.8/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 15:35:17.000000 wonder-sdk-0.1.8/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 15:35:17.000000 wonder-sdk-0.1.8/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 15:35:17.000000 wonder-sdk-0.1.8/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 15:35:17.000000 wonder-sdk-0.1.8/wonder_sdk.egg-info/top_level.txt
```

### Comparing `wonder-sdk-0.1.7/LICENCE` & `wonder-sdk-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.7/wonder_sdk/__init__.py` & `wonder-sdk-0.1.8/wonder_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,26 +92,26 @@
     # STORAGE
     def _get_storage_client(self):
         if not hasattr('storage_client'):
             self.storage_client = storage.Client()
         
         return self.storage_client
 
-    def upload_from_filename(self, bucket_name, destination_blob_name, source_file_path=None, source_file=None, source_string=None):
+    def upload_to_bucket(self, bucket_name, destination_blob_name, source_file_path=None, source_file=None, source_string=None):
         client = self._get_storage_client()
         bucket = client.bucket(bucket_name)
         blob = bucket.blob(destination_blob_name)
         if source_file_path:
             blob.upload_from_filename(source_file_path)
         elif source_file:
             blob.upload_from_file(source_file)
         elif source_string:
             blob.upload_from_string(source_string)
 
-    def download_to_filename(self, bucket_name, source_blob_name, destination_file_path=None, download_as_text=False, download_as_bytes=False):
+    def download_from_bucket(self, bucket_name, source_blob_name, destination_file_path=None, download_as_text=False, download_as_bytes=False):
         storage_client = storage.Client()
         bucket = storage_client.bucket(bucket_name)
         blob = bucket.blob(source_blob_name)
         if destination_file_path:
             blob.download_to_filename(destination_file_path)
             return destination_file_path
         elif download_as_text:
```

### Comparing `wonder-sdk-0.1.7/wonder_sdk/config.py` & `wonder-sdk-0.1.8/wonder_sdk/config.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.7/wonder_sdk/health.py` & `wonder-sdk-0.1.8/wonder_sdk/health.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.7/wonder_sdk/logger.py` & `wonder-sdk-0.1.8/wonder_sdk/logger.py`

 * *Files identical despite different names*

