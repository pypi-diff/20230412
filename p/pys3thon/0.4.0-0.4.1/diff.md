# Comparing `tmp/pys3thon-0.4.0.tar.gz` & `tmp/pys3thon-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pys3thon-0.4.0.tar", last modified: Wed Jan 11 13:15:04 2023, max compression
+gzip compressed data, was "pys3thon-0.4.1.tar", last modified: Wed Apr 12 03:04:54 2023, max compression
```

## Comparing `pys3thon-0.4.0.tar` & `pys3thon-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 13:15:04.291236 pys3thon-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-01-11 13:14:22.000000 pys3thon-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-01-11 13:15:04.291236 pys3thon-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-01-11 13:14:22.000000 pys3thon-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-01-11 13:14:22.000000 pys3thon-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 13:15:04.291236 pys3thon-0.4.0/pys3thon/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-11 13:15:01.000000 pys3thon-0.4.0/pys3thon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9597 2023-01-11 13:14:22.000000 pys3thon-0.4.0/pys3thon/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-01-11 13:14:22.000000 pys3thon-0.4.0/pys3thon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 13:15:04.291236 pys3thon-0.4.0/pys3thon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-01-11 13:15:04.000000 pys3thon-0.4.0/pys3thon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-01-11 13:15:04.000000 pys3thon-0.4.0/pys3thon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-11 13:15:04.000000 pys3thon-0.4.0/pys3thon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-01-11 13:15:04.000000 pys3thon-0.4.0/pys3thon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-01-11 13:15:04.000000 pys3thon-0.4.0/pys3thon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-01-11 13:15:04.291236 pys3thon-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-01-11 13:14:22.000000 pys3thon-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:04:54.776760 pys3thon-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-04-12 03:04:10.000000 pys3thon-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-04-12 03:04:54.776760 pys3thon-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-12 03:04:10.000000 pys3thon-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-04-12 03:04:10.000000 pys3thon-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:04:54.776760 pys3thon-0.4.1/pys3thon/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-12 03:04:53.000000 pys3thon-0.4.1/pys3thon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9965 2023-04-12 03:04:10.000000 pys3thon-0.4.1/pys3thon/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-04-12 03:04:10.000000 pys3thon-0.4.1/pys3thon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:04:54.776760 pys3thon-0.4.1/pys3thon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-04-12 03:04:54.000000 pys3thon-0.4.1/pys3thon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-12 03:04:54.000000 pys3thon-0.4.1/pys3thon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 03:04:54.000000 pys3thon-0.4.1/pys3thon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-12 03:04:54.000000 pys3thon-0.4.1/pys3thon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-12 03:04:54.000000 pys3thon-0.4.1/pys3thon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-12 03:04:54.776760 pys3thon-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-12 03:04:10.000000 pys3thon-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:04:54.776760 pys3thon-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2091 2023-04-12 03:04:10.000000 pys3thon-0.4.1/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-04-12 03:04:10.000000 pys3thon-0.4.1/tests/test_delete_directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4444 2023-04-12 03:04:10.000000 pys3thon-0.4.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5552 2023-04-12 03:04:10.000000 pys3thon-0.4.1/tests/test_get_directories_for_bucket_with_prefix_recursively.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-12 03:04:10.000000 pys3thon-0.4.1/tests/test_get_files_for_bucket_with_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-12 03:04:10.000000 pys3thon-0.4.1/tests/test_upload_directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-04-12 03:04:10.000000 pys3thon-0.4.1/tests/test_upload_file.py
```

### Comparing `pys3thon-0.4.0/LICENSE` & `pys3thon-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pys3thon-0.4.0/pys3thon/client.py` & `pys3thon-0.4.1/pys3thon/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from contextlib import contextmanager
 from pathlib import Path
-from tempfile import NamedTemporaryFile
-from urllib.parse import unquote
+from tempfile import TemporaryDirectory
 
 import boto3
+from boto3.s3.transfer import TransferConfig
 from botocore.client import Config
 from botocore.exceptions import ClientError
 from tqdm import tqdm
 
 from .utils import run_shell_command
 
 
@@ -28,52 +28,64 @@
         self.client = boto3.session.Session(**session_kwargs).client(
             "s3", **client_kwargs
         )
         self.profile_name = profile_name
         self.endpoint_url = endpoint_url
 
     @contextmanager
-    def download_to_temporary_file(self, bucket, key, show_progress=False):
+    def download_to_temporary_file(
+        self, bucket, key, file_name=None, show_progress=False
+    ):
         try:
-            temp_file = NamedTemporaryFile()
-            self.download(bucket, key, temp_file.name, show_progress)
-            yield temp_file.name
+            temp_directory = TemporaryDirectory()
+            if file_name is None:
+                file_name = key.split("/")[-1]
+            save_path = Path(temp_directory.name) / file_name
+            self.download(bucket, key, str(save_path), show_progress)
+            yield save_path
         finally:
-            pass
+            temp_directory.cleanup()
 
-    def download(self, bucket, key, save_prefix, show_progress=False):
+    def download(
+        self,
+        bucket,
+        key,
+        save_prefix,
+        show_progress=False,
+        Config=TransferConfig(),
+    ):
         save_prefix = str(save_prefix)
 
         if show_progress:
 
             def hook(t):
                 def inner(bytes_amount):
                     t.update(bytes_amount)
 
                 return inner
 
             file_size = float(
-                self.client.head_object(Bucket=bucket, Key=unquote(key))[
+                self.client.head_object(Bucket=bucket, Key=key)[
                     "ContentLength"
                 ]
             )
             with tqdm(
                 total=file_size, unit="B", unit_scale=True, desc=save_prefix
             ) as t:
                 self.client.download_file(
-                    bucket, unquote(key), save_prefix, Callback=hook(t)
+                    bucket, key, save_prefix, Callback=hook(t), Config=Config
                 )
         else:
-            self.client.download_file(bucket, unquote(key), save_prefix)
+            self.client.download_file(bucket, key, save_prefix, Config=Config)
 
-    def upload_file(self, path, bucket, key):
-        self.client.upload_file(path, bucket, key)
+    def upload_file(self, path, bucket, key, Config=TransferConfig()):
+        self.client.upload_file(path, bucket, key, Config=Config)
 
-    def upload_fileobj(self, fileobj, bucket, key):
-        self.client.upload_fileobj(fileobj, bucket, key)
+    def upload_fileobj(self, fileobj, bucket, key, Config=TransferConfig()):
+        self.client.upload_fileobj(fileobj, bucket, key, Config=Config)
 
     def copy(self, source_bucket, source_key, dst_bucket, dst_key):
         self.client.copy(
             {"Bucket": source_bucket, "Key": source_key}, dst_bucket, dst_key
         )
 
     def check_if_exists_in_s3(self, bucket, key):
```

### Comparing `pys3thon-0.4.0/pys3thon/utils.py` & `pys3thon-0.4.1/pys3thon/utils.py`

 * *Files identical despite different names*

### Comparing `pys3thon-0.4.0/setup.py` & `pys3thon-0.4.1/setup.py`

 * *Files identical despite different names*

