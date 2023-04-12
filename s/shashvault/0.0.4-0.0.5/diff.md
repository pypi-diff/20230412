# Comparing `tmp/shashvault-0.0.4-py3-none-any.whl.zip` & `tmp/shashvault-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4500 bytes, number of entries: 8
+Zip file size: 4504 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       22 b- defN 23-Apr-12 08:56 shashvault/__init__.py
--rw-r--r--  2.0 unx     4107 b- defN 23-Apr-12 08:55 shashvault/main.py
--rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1450 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 08:57 shashvault-0.0.4.dist-info/RECORD
-8 files, 7720 bytes uncompressed, 3356 bytes compressed:  56.5%
+-rw-r--r--  2.0 unx     4108 b- defN 23-Apr-12 09:01 shashvault/main.py
+-rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 09:02 shashvault-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1450 b- defN 23-Apr-12 09:02 shashvault-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 09:02 shashvault-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 09:02 shashvault-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 09:02 shashvault-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 09:02 shashvault-0.0.5.dist-info/RECORD
+8 files, 7721 bytes uncompressed, 3360 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: shashvault/__init__.py
 Comment: 
 
 Filename: shashvault/main.py
 Comment: 
 
-Filename: shashvault-0.0.4.dist-info/LICENSE
+Filename: shashvault-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: shashvault-0.0.4.dist-info/METADATA
+Filename: shashvault-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: shashvault-0.0.4.dist-info/WHEEL
+Filename: shashvault-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: shashvault-0.0.4.dist-info/entry_points.txt
+Filename: shashvault-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: shashvault-0.0.4.dist-info/top_level.txt
+Filename: shashvault-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: shashvault-0.0.4.dist-info/RECORD
+Filename: shashvault-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shashvault/main.py

```diff
@@ -74,15 +74,15 @@
     url = f"{vault_addr}/v1/{kv_path}/data/{search_secret}"
     response = requests.get(url, headers=headers, verify=not VAULT_SKIP_VERIFY)
     response.raise_for_status()
     secret_data = response.json()["data"]["data"]
     return secret_data
 
 
-def run()
+def run():
     parser = argparse.ArgumentParser(
         description="Search and display secrets in HashiCorp Vault"
     )
     parser.add_argument(
         "-sp",
         "--search-path",
         dest="search_path",
```

## Comparing `shashvault-0.0.4.dist-info/LICENSE` & `shashvault-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shashvault-0.0.4.dist-info/METADATA` & `shashvault-0.0.5.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shashvault
-Version: 0.0.4
+Version: 0.0.5
 Summary: search Hashicorp vault path and secret
 Home-page: https://gitlab.esss.lu.se/remymudingay/my_scripts/shashvault.git
 Author: Remy Mudingay
 Author-email: remy.mudingay@ess.eu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

## Comparing `shashvault-0.0.4.dist-info/RECORD` & `shashvault-0.0.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 shashvault/__init__.py,sha256=QXzW3aVbiEqgw207VQEY_0uPknbiS3bW8f6jOz-j3vQ,22
-shashvault/main.py,sha256=BZCXGg9XAw5t4QvWKNJjh9tHAnm78ibtOzk6t9Hj5oI,4107
-shashvault-0.0.4.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
-shashvault-0.0.4.dist-info/METADATA,sha256=E31NBBHLvBgBv-BsUgWnHRLf9WPWlQP67aJ11dOLP7k,1450
-shashvault-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-shashvault-0.0.4.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
-shashvault-0.0.4.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
-shashvault-0.0.4.dist-info/RECORD,,
+shashvault/main.py,sha256=cTlhhAVr427bfasr8Sx6v0XrE1DdT5WtWe_JBkpTYjA,4108
+shashvault-0.0.5.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
+shashvault-0.0.5.dist-info/METADATA,sha256=qzlSc4JBVYhHPH_tSTsX0FUchY7f3W4_mCeDsg7doE8,1450
+shashvault-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+shashvault-0.0.5.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
+shashvault-0.0.5.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
+shashvault-0.0.5.dist-info/RECORD,,
```

