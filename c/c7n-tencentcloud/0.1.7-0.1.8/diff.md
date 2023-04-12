# Comparing `tmp/c7n_tencentcloud-0.1.7-py3-none-any.whl.zip` & `tmp/c7n_tencentcloud-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 45409 bytes, number of entries: 33
+Zip file size: 45405 bytes, number of entries: 33
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 c7n_tencentcloud/__init__.py
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 c7n_tencentcloud/actions/__init__.py
 -rw-r--r--  2.0 unx      819 b- defN 80-Jan-01 00:00 c7n_tencentcloud/actions/core.py
 -rw-r--r--  2.0 unx    10845 b- defN 80-Jan-01 00:00 c7n_tencentcloud/actions/tags.py
 -rw-r--r--  2.0 unx     7239 b- defN 80-Jan-01 00:00 c7n_tencentcloud/client.py
 -rw-r--r--  2.0 unx      329 b- defN 80-Jan-01 00:00 c7n_tencentcloud/entry.py
 -rw-r--r--  2.0 unx      116 b- defN 80-Jan-01 00:00 c7n_tencentcloud/filters/__init__.py
@@ -25,11 +25,11 @@
 -rw-r--r--  2.0 unx     2151 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/nat_gateway.py
 -rw-r--r--  2.0 unx     1253 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/resource_map.py
 -rw-r--r--  2.0 unx     9155 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/security_group.py
 -rw-r--r--  2.0 unx     1399 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/tag.py
 -rw-r--r--  2.0 unx     3179 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/tcr.py
 -rw-r--r--  2.0 unx     3138 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/vpc.py
 -rw-r--r--  2.0 unx     1252 b- defN 80-Jan-01 00:00 c7n_tencentcloud/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_tencentcloud-0.1.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4207 b- defN 16-Jan-01 00:00 c7n_tencentcloud-0.1.7.dist-info/METADATA
-?rw-------  2.0 unx     2948 b- defN 23-Apr-11 08:33 c7n_tencentcloud-0.1.7.dist-info/RECORD
-33 files, 133647 bytes uncompressed, 40621 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_tencentcloud-0.1.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4207 b- defN 16-Jan-01 00:00 c7n_tencentcloud-0.1.8.dist-info/METADATA
+?rw-------  2.0 unx     2948 b- defN 23-Apr-12 11:00 c7n_tencentcloud-0.1.8.dist-info/RECORD
+33 files, 133647 bytes uncompressed, 40617 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -84,17 +84,17 @@
 
 Filename: c7n_tencentcloud/resources/vpc.py
 Comment: 
 
 Filename: c7n_tencentcloud/utils.py
 Comment: 
 
-Filename: c7n_tencentcloud-0.1.7.dist-info/WHEEL
+Filename: c7n_tencentcloud-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_tencentcloud-0.1.7.dist-info/METADATA
+Filename: c7n_tencentcloud-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: c7n_tencentcloud-0.1.7.dist-info/RECORD
+Filename: c7n_tencentcloud-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_tencentcloud-0.1.7.dist-info/METADATA` & `c7n_tencentcloud-0.1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: c7n-tencentcloud
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cloud Custodian - Tencent Cloud Provider
 Home-page: https://cloudcustodian.io
 License: Apache-2.0
 Author: Tencent Cloud
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: c7n (==0.9.25) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: c7n (==0.9.26) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: boto3 (==1.26.109) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: jsonschema (==4.17.3) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: argcomplete (==3.0.5) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: python-dateutil (==2.8.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pyyaml (==6.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: tabulate (==0.9.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: importlib-metadata (==5.2.0) ; python_version >= "3.7" and python_version < "4.0"
```

## Comparing `c7n_tencentcloud-0.1.7.dist-info/RECORD` & `c7n_tencentcloud-0.1.8.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 c7n_tencentcloud/resources/nat_gateway.py,sha256=b3DhZKC8x92paORrZQ3FbX2sWEit0Iweketn1rK7qqs,2151
 c7n_tencentcloud/resources/resource_map.py,sha256=dm-1PqUUgdyQW5Q2hsfstP4Gw1Z77UFMv_T94pOg2PM,1253
 c7n_tencentcloud/resources/security_group.py,sha256=CvMaWS6NJLVg-syICYt63igheQ0DcT-WYQjAMhAiJ3k,9155
 c7n_tencentcloud/resources/tag.py,sha256=3WiuN-y4Dm36Bk7i7CwLrVYPn3xh7a5K4gyCVBhpFC0,1399
 c7n_tencentcloud/resources/tcr.py,sha256=RKf13xKcEt9ZHiJGSKPaUzfda3h2bcVArEaq82IGMmg,3179
 c7n_tencentcloud/resources/vpc.py,sha256=TkPc6bYtK6m7wEj5qqRWoYUFDD8rL6zFRNLFJZcZDRo,3138
 c7n_tencentcloud/utils.py,sha256=6Nr5ZbebrexDRLCANUyN3mp8vO67d-hNkhsX5dN06QU,1252
-c7n_tencentcloud-0.1.7.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
-c7n_tencentcloud-0.1.7.dist-info/RECORD,,
-c7n_tencentcloud-0.1.7.dist-info/METADATA,sha256=oAJa-0qDnEWu2NbLR5yKhEIQQDrE10ZKHN8IdqoiTUQ,4207
+c7n_tencentcloud-0.1.8.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
+c7n_tencentcloud-0.1.8.dist-info/RECORD,,
+c7n_tencentcloud-0.1.8.dist-info/METADATA,sha256=3gRUSzE6AjYh0VoOl2l_gdAD75R1kr4Waf6Nf_4rMNQ,4207
```

