# Comparing `tmp/shashvault-0.1.0-py3-none-any.whl.zip` & `tmp/shashvault-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4522 bytes, number of entries: 8
+Zip file size: 4603 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       36 b- defN 23-Apr-12 09:07 shashvault/__init__.py
--rw-r--r--  2.0 unx     4108 b- defN 23-Apr-12 09:01 shashvault/main.py
--rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1465 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/RECORD
-8 files, 7750 bytes uncompressed, 3378 bytes compressed:  56.4%
+-rw-r--r--  2.0 unx     4349 b- defN 23-Apr-12 11:05 shashvault/main.py
+-rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 11:08 shashvault-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1465 b- defN 23-Apr-12 11:08 shashvault-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 11:08 shashvault-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 11:08 shashvault-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 11:08 shashvault-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 11:08 shashvault-0.1.1.dist-info/RECORD
+8 files, 7991 bytes uncompressed, 3459 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: shashvault/__init__.py
 Comment: 
 
 Filename: shashvault/main.py
 Comment: 
 
-Filename: shashvault-0.1.0.dist-info/LICENSE
+Filename: shashvault-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: shashvault-0.1.0.dist-info/METADATA
+Filename: shashvault-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: shashvault-0.1.0.dist-info/WHEEL
+Filename: shashvault-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: shashvault-0.1.0.dist-info/entry_points.txt
+Filename: shashvault-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: shashvault-0.1.0.dist-info/top_level.txt
+Filename: shashvault-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: shashvault-0.1.0.dist-info/RECORD
+Filename: shashvault-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shashvault/main.py

```diff
@@ -27,18 +27,25 @@
 async def get_paths_async(
     vault_addr, vault_token, kv_path, vault_skip_verify, search_path, current_path=""
 ):
     headers = {"X-Vault-Token": vault_token}
     url = f"{vault_addr}/v1/{kv_path}/metadata{current_path}?list=true"
 
     async with aiohttp.ClientSession(headers=headers) as session:
-        async with session.get(url, verify_ssl=not vault_skip_verify) as response:
-            response.raise_for_status()
-            json_response = await response.json()
-            keys = json_response["data"]["keys"]
+        # exception handling reported by SA due to permissions
+        try:
+            async with session.get(url, verify_ssl=not vault_skip_verify) as response:
+                response.raise_for_status()
+                json_response = await response.json()
+                keys = json_response["data"]["keys"]
+        except aiohttp.ClientResponseError as e:
+            if e.status == 403:
+                return []
+            else:
+                raise e
 
     matching_paths = []
     tasks = []
     for key in keys:
         if key.endswith("/"):
             tasks.append(
                 get_paths_async(
```

## Comparing `shashvault-0.1.0.dist-info/LICENSE` & `shashvault-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shashvault-0.1.0.dist-info/METADATA` & `shashvault-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shashvault
-Version: 0.1.0
+Version: 0.1.1
 Summary: search Hashicorp vault path and secret
 Home-page: https://gitlab.esss.lu.se/ics-infrastructure/shashvault
 Author: Remy Mudingay
 Author-email: remy.mudingay@ess.eu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

