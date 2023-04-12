# Comparing `tmp/stathub-0.1.4-py3-none-any.whl.zip` & `tmp/stathub-0.1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2042 bytes, number of entries: 5
+Zip file size: 2089 bytes, number of entries: 5
 -rw-rw-rw-  2.0 fat     1536 b- defN 23-Apr-12 08:33 stathub/stathub.py
--rw-rw-rw-  2.0 fat      673 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      371 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/RECORD
-5 files, 2680 bytes uncompressed, 1348 bytes compressed:  49.7%
+-rw-rw-rw-  2.0 fat      716 b- defN 23-Apr-12 08:46 stathub-0.1.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 08:46 stathub-0.1.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-12 08:46 stathub-0.1.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      379 b- defN 23-Apr-12 08:46 stathub-0.1.4.1.dist-info/RECORD
+5 files, 2731 bytes uncompressed, 1379 bytes compressed:  49.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: stathub/stathub.py
 Comment: 
 
-Filename: stathub-0.1.4.dist-info/METADATA
+Filename: stathub-0.1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: stathub-0.1.4.dist-info/WHEEL
+Filename: stathub-0.1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: stathub-0.1.4.dist-info/top_level.txt
+Filename: stathub-0.1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: stathub-0.1.4.dist-info/RECORD
+Filename: stathub-0.1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stathub-0.1.4.dist-info/METADATA` & `stathub-0.1.4.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: stathub
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: A python package used for getting data from Statistics Sharing Hub.
 Home-page: https://pypi.org/project/stathub
 Author: Government Strategic Information Center​
 Author-email: sdmx.tnso@gmail.com
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: openpyxl
 
 This python package can be used for accessing and getting datasets from Statistics Sharing Hub (stathub.nso.go.th) maintained by Government Strategic Information Center​, National Statistical Office of Thailand.
 
 # Prerequisite Packages
```

