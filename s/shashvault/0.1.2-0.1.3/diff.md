# Comparing `tmp/shashvault-0.1.2-py3-none-any.whl.zip` & `tmp/shashvault-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4619 bytes, number of entries: 8
--rw-r--r--  2.0 unx       36 b- defN 23-Apr-12 09:40 shashvault/__init__.py
--rw-r--r--  2.0 unx     4349 b- defN 23-Apr-12 11:19 shashvault/main.py
--rw-rw-rw-  2.0 unx     1336 b- defN 23-Apr-12 11:20 shashvault-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1540 b- defN 23-Apr-12 11:20 shashvault-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 11:20 shashvault-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 11:20 shashvault-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 11:20 shashvault-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 11:20 shashvault-0.1.2.dist-info/RECORD
-8 files, 8066 bytes uncompressed, 3475 bytes compressed:  56.9%
+Zip file size: 4641 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       36 b- defN 23-Apr-12 14:45 shashvault/__init__.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-Apr-12 14:45 shashvault/main.py
+-rw-rw-rw-  2.0 unx     1336 b- defN 23-Apr-12 14:45 shashvault-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1559 b- defN 23-Apr-12 14:45 shashvault-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 14:45 shashvault-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 14:45 shashvault-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 14:45 shashvault-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 14:45 shashvault-0.1.3.dist-info/RECORD
+8 files, 8101 bytes uncompressed, 3497 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: shashvault/__init__.py
 Comment: 
 
 Filename: shashvault/main.py
 Comment: 
 
-Filename: shashvault-0.1.2.dist-info/LICENSE
+Filename: shashvault-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: shashvault-0.1.2.dist-info/METADATA
+Filename: shashvault-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: shashvault-0.1.2.dist-info/WHEEL
+Filename: shashvault-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: shashvault-0.1.2.dist-info/entry_points.txt
+Filename: shashvault-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: shashvault-0.1.2.dist-info/top_level.txt
+Filename: shashvault-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: shashvault-0.1.2.dist-info/RECORD
+Filename: shashvault-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shashvault/main.py

```diff
@@ -53,15 +53,15 @@
                     vault_token,
                     kv_path,
                     vault_skip_verify,
                     search_path,
                     f"{current_path}/{key.strip('/')}",
                 )
             )
-        elif search_path in key:
+        elif search_path.lower() in key.lower():
             matching_paths.append(f"{current_path}/{key}".strip("/"))
 
     subpaths = await asyncio.gather(*tasks)
     for subpath in subpaths:
         matching_paths.extend(subpath)
 
     return matching_paths
```

## Comparing `shashvault-0.1.2.dist-info/LICENSE` & `shashvault-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shashvault-0.1.2.dist-info/METADATA` & `shashvault-0.1.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shashvault
-Version: 0.1.2
+Version: 0.1.3
 Summary: search Hashicorp vault path and secret
 Home-page: https://gitlab.esss.lu.se/ics-infrastructure/shashvault
 Author: Remy Mudingay
 Author-email: remy.mudingay@ess.eu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp (~=3.8.4)
 Requires-Dist: requests (~=2.28.1)
 
 # Vault search
 
-This script provides the functionality to search secret paths that match a string and also display k/v when specifying a path.
+This script provides the functionality to search secret paths that match a string (case insensitive) and also display k/v when specifying a path.
 
 ## Dependancies
 
 ### Requirements
 ```
 pip install requests aiohttp
 ```
```

## Comparing `shashvault-0.1.2.dist-info/RECORD` & `shashvault-0.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 shashvault/__init__.py,sha256=BgKbBh7aubvQHftiaEqNjeP4iPviOR-JvJgoLrDkD6I,36
-shashvault/main.py,sha256=e_kkFyXl7Z6jrbnpxiDiOaqQCTU_RBGdYHcmkEHlPc4,4349
-shashvault-0.1.2.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
-shashvault-0.1.2.dist-info/METADATA,sha256=10SOBNyKqjEebfLcOkaC_P-q-EF5MRGeAcQzbBnnUfY,1540
-shashvault-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-shashvault-0.1.2.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
-shashvault-0.1.2.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
-shashvault-0.1.2.dist-info/RECORD,,
+shashvault/main.py,sha256=qFGTfw4WhbIPXVI1kv_DYdIFznMX8xaK7vkhVvqludY,4365
+shashvault-0.1.3.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
+shashvault-0.1.3.dist-info/METADATA,sha256=X2UpbdKPBRmFFoStA9sSw9LODInMsHZo6ear1Akjpv4,1559
+shashvault-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+shashvault-0.1.3.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
+shashvault-0.1.3.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
+shashvault-0.1.3.dist-info/RECORD,,
```

