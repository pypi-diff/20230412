# Comparing `tmp/shashvault-0.0.2-py3-none-any.whl.zip` & `tmp/shashvault-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4485 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 08:20 shashvault/__init__.py
--rw-r--r--  2.0 unx     4144 b- defN 23-Apr-12 08:46 shashvault/main.py
--rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1450 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/RECORD
-8 files, 7734 bytes uncompressed, 3341 bytes compressed:  56.8%
+Zip file size: 4500 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-12 08:56 shashvault/__init__.py
+-rw-r--r--  2.0 unx     4107 b- defN 23-Apr-12 08:55 shashvault/main.py
+-rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1450 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/RECORD
+8 files, 7720 bytes uncompressed, 3356 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: shashvault/__init__.py
 Comment: 
 
 Filename: shashvault/main.py
 Comment: 
 
-Filename: shashvault-0.0.2.dist-info/LICENSE
+Filename: shashvault-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: shashvault-0.0.2.dist-info/METADATA
+Filename: shashvault-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: shashvault-0.0.2.dist-info/WHEEL
+Filename: shashvault-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: shashvault-0.0.2.dist-info/entry_points.txt
+Filename: shashvault-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: shashvault-0.0.2.dist-info/top_level.txt
+Filename: shashvault-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: shashvault-0.0.2.dist-info/RECORD
+Filename: shashvault-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shashvault/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 6d61 696e 2069 6d70 6f72  from .main impor
+00000010: 7420 7275 6e0a                           t run.
```

## shashvault/main.py

```diff
@@ -74,15 +74,15 @@
     url = f"{vault_addr}/v1/{kv_path}/data/{search_secret}"
     response = requests.get(url, headers=headers, verify=not VAULT_SKIP_VERIFY)
     response.raise_for_status()
     secret_data = response.json()["data"]["data"]
     return secret_data
 
 
-if __name__ == "__main__":
+def run()
     parser = argparse.ArgumentParser(
         description="Search and display secrets in HashiCorp Vault"
     )
     parser.add_argument(
         "-sp",
         "--search-path",
         dest="search_path",
@@ -130,10 +130,9 @@
             args.search_secret,
         )
         print("Secret data:")
         for key, value in secret_data.items():
             print(f"{key}: {value}")
 
 
-def run():
-    if __name__ == "__main__":
-        main()
+if __name__ == "__main__":
+    run()
```

## Comparing `shashvault-0.0.2.dist-info/LICENSE` & `shashvault-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shashvault-0.0.2.dist-info/METADATA` & `shashvault-0.0.4.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shashvault
-Version: 0.0.2
+Version: 0.0.4
 Summary: search Hashicorp vault path and secret
 Home-page: https://gitlab.esss.lu.se/remymudingay/my_scripts/shashvault.git
 Author: Remy Mudingay
 Author-email: remy.mudingay@ess.eu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

## Comparing `shashvault-0.0.2.dist-info/RECORD` & `shashvault-0.0.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-shashvault/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-shashvault/main.py,sha256=oGX7u_9eumz63Qu4JlhvFV1ha9k16kQTb65ZZLv68_g,4144
-shashvault-0.0.2.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
-shashvault-0.0.2.dist-info/METADATA,sha256=131z2CuXyi63IhwqUI0_sh1bcej4PexM_gAPGOAtSMc,1450
-shashvault-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-shashvault-0.0.2.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
-shashvault-0.0.2.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
-shashvault-0.0.2.dist-info/RECORD,,
+shashvault/__init__.py,sha256=QXzW3aVbiEqgw207VQEY_0uPknbiS3bW8f6jOz-j3vQ,22
+shashvault/main.py,sha256=BZCXGg9XAw5t4QvWKNJjh9tHAnm78ibtOzk6t9Hj5oI,4107
+shashvault-0.0.4.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
+shashvault-0.0.4.dist-info/METADATA,sha256=E31NBBHLvBgBv-BsUgWnHRLf9WPWlQP67aJ11dOLP7k,1450
+shashvault-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+shashvault-0.0.4.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
+shashvault-0.0.4.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
+shashvault-0.0.4.dist-info/RECORD,,
```

