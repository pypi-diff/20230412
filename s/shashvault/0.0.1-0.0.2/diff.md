# Comparing `tmp/shashvault-0.0.1-py3-none-any.whl.zip` & `tmp/shashvault-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4464 bytes, number of entries: 8
+Zip file size: 4485 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 08:20 shashvault/__init__.py
--rw-r--r--  2.0 unx     4085 b- defN 23-Apr-12 08:12 shashvault/main.py
--rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 08:25 shashvault-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1450 b- defN 23-Apr-12 08:25 shashvault-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:25 shashvault-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Apr-12 08:25 shashvault-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 08:25 shashvault-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-12 08:25 shashvault-0.0.1.dist-info/RECORD
-8 files, 7676 bytes uncompressed, 3320 bytes compressed:  56.7%
+-rw-r--r--  2.0 unx     4144 b- defN 23-Apr-12 08:46 shashvault/main.py
+-rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1450 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-12 08:47 shashvault-0.0.2.dist-info/RECORD
+8 files, 7734 bytes uncompressed, 3341 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: shashvault/__init__.py
 Comment: 
 
 Filename: shashvault/main.py
 Comment: 
 
-Filename: shashvault-0.0.1.dist-info/LICENSE
+Filename: shashvault-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: shashvault-0.0.1.dist-info/METADATA
+Filename: shashvault-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: shashvault-0.0.1.dist-info/WHEEL
+Filename: shashvault-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: shashvault-0.0.1.dist-info/entry_points.txt
+Filename: shashvault-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: shashvault-0.0.1.dist-info/top_level.txt
+Filename: shashvault-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: shashvault-0.0.1.dist-info/RECORD
+Filename: shashvault-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shashvault/main.py

```diff
@@ -128,7 +128,12 @@
             VAULT_KV_PATH,
             VAULT_SKIP_VERIFY,
             args.search_secret,
         )
         print("Secret data:")
         for key, value in secret_data.items():
             print(f"{key}: {value}")
+
+
+def run():
+    if __name__ == "__main__":
+        main()
```

## Comparing `shashvault-0.0.1.dist-info/LICENSE` & `shashvault-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shashvault-0.0.1.dist-info/METADATA` & `shashvault-0.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shashvault
-Version: 0.0.1
+Version: 0.0.2
 Summary: search Hashicorp vault path and secret
 Home-page: https://gitlab.esss.lu.se/remymudingay/my_scripts/shashvault.git
 Author: Remy Mudingay
 Author-email: remy.mudingay@ess.eu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

