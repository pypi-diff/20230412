# Comparing `tmp/xia_engine-0.6.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine-0.6.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1116271 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1401 b- defN 23-Mar-12 08:09 xia_engine/__init__.py
--rw-r--r--  2.0 unx   390144 b- defN 23-Mar-12 08:37 xia_engine/acl.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   548864 b- defN 23-Mar-12 08:36 xia_engine/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   637952 b- defN 23-Mar-12 08:41 xia_engine/document.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   566272 b- defN 23-Mar-12 08:40 xia_engine/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   262144 b- defN 23-Mar-12 08:42 xia_engine/exception.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   493568 b- defN 23-Mar-12 08:38 xia_engine/fields.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-12 08:42 xia_engine-0.6.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      745 b- defN 23-Mar-12 08:42 xia_engine-0.6.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-12 08:42 xia_engine-0.6.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-12 08:42 xia_engine-0.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1052 b- defN 23-Mar-12 08:42 xia_engine-0.6.8.dist-info/RECORD
-12 files, 2902404 bytes uncompressed, 1114505 bytes compressed:  61.6%
+Zip file size: 1118485 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1401 b- defN 23-Mar-15 11:41 xia_engine/__init__.py
+-rw-r--r--  2.0 unx   390144 b- defN 23-Mar-15 11:46 xia_engine/acl.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   548864 b- defN 23-Mar-15 11:44 xia_engine/base.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   645632 b- defN 23-Mar-15 11:50 xia_engine/document.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   566272 b- defN 23-Mar-15 11:48 xia_engine/engine.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   262144 b- defN 23-Mar-15 11:51 xia_engine/exception.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   493568 b- defN 23-Mar-15 11:47 xia_engine/fields.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-15 11:51 xia_engine-0.6.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      745 b- defN 23-Mar-15 11:51 xia_engine-0.6.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Mar-15 11:51 xia_engine-0.6.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Mar-15 11:51 xia_engine-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1052 b- defN 23-Mar-15 11:51 xia_engine-0.6.9.dist-info/RECORD
+12 files, 2910084 bytes uncompressed, 1116719 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_engine/exception.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_engine/fields.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine-0.6.8.dist-info/LICENSE.txt
+Filename: xia_engine-0.6.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine-0.6.8.dist-info/METADATA
+Filename: xia_engine-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine-0.6.8.dist-info/WHEEL
+Filename: xia_engine-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine-0.6.8.dist-info/top_level.txt
+Filename: xia_engine-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine-0.6.8.dist-info/RECORD
+Filename: xia_engine-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine/__init__.py

```diff
@@ -20,8 +20,8 @@
     "MetaEngine", "MetaRamEngine", "MetaCache",
     "Acl", "AclItem",
     "XiaError", 'AuthorizationError', 'AuthenticationError', "OutOfScopeError",
     'NotFoundError', 'ConflictError', 'BadRequestError', "UnprocessableError",
     "ServerError"
 ]
 
-__version__ = "0.6.8"
+__version__ = "0.6.9"
```

## Comparing `xia_engine-0.6.8.dist-info/METADATA` & `xia_engine-0.6.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine
-Version: 0.6.8
+Version: 0.6.9
 Summary: X-I-A Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine/0.6.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine/0.6.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

