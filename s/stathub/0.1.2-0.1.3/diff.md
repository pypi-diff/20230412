# Comparing `tmp/stathub-0.1.2-py3-none-any.whl.zip` & `tmp/stathub-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1906 bytes, number of entries: 5
+Zip file size: 1907 bytes, number of entries: 5
 -rw-rw-rw-  2.0 fat     1120 b- defN 23-Apr-12 04:16 stathub/stathub.py
--rw-rw-rw-  2.0 fat      661 b- defN 23-Apr-12 06:46 stathub-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 06:46 stathub-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-12 06:46 stathub-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      371 b- defN 23-Apr-12 06:46 stathub-0.1.2.dist-info/RECORD
-5 files, 2252 bytes uncompressed, 1212 bytes compressed:  46.2%
+-rw-rw-rw-  2.0 fat      667 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      371 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/RECORD
+5 files, 2258 bytes uncompressed, 1213 bytes compressed:  46.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: stathub/stathub.py
 Comment: 
 
-Filename: stathub-0.1.2.dist-info/METADATA
+Filename: stathub-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: stathub-0.1.2.dist-info/WHEEL
+Filename: stathub-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: stathub-0.1.2.dist-info/top_level.txt
+Filename: stathub-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: stathub-0.1.2.dist-info/RECORD
+Filename: stathub-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stathub-0.1.2.dist-info/METADATA` & `stathub-0.1.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: stathub
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package used for getting data from Statistics Sharing Hub
 Home-page: https://pypi.org/project/stathub
 Author: Government Strategic Information Center​
 Author-email: sdmx.tnso@gmail.com
 Requires-Python: >=3.8
 Requires-Dist: pandas
 Requires-Dist: requests
 
 ## Project Description
+
 This python package can be used for accessing and getting datasets from Statistics Sharing Hub (stathub.nso.go.th) maintained by Government Strategic Information Center​, National Statistical Office of Thailand.
 
 ## Prerequisite Packages
+
 - pandas
 - requests
 
 ## Contact
+
 sdmx.tnso@gmail.com
```

