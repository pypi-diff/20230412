# Comparing `tmp/shashvault-0.0.8-py3-none-any.whl.zip` & `tmp/shashvault-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4529 bytes, number of entries: 8
+Zip file size: 4522 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       36 b- defN 23-Apr-12 09:07 shashvault/__init__.py
 -rw-r--r--  2.0 unx     4108 b- defN 23-Apr-12 09:01 shashvault/main.py
--rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 09:10 shashvault-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1464 b- defN 23-Apr-12 09:10 shashvault-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 09:10 shashvault-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 09:10 shashvault-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 09:10 shashvault-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 09:10 shashvault-0.0.8.dist-info/RECORD
-8 files, 7749 bytes uncompressed, 3385 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx     1336 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1465 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-12 09:40 shashvault-0.1.0.dist-info/RECORD
+8 files, 7750 bytes uncompressed, 3378 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: shashvault/__init__.py
 Comment: 
 
 Filename: shashvault/main.py
 Comment: 
 
-Filename: shashvault-0.0.8.dist-info/LICENSE
+Filename: shashvault-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: shashvault-0.0.8.dist-info/METADATA
+Filename: shashvault-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: shashvault-0.0.8.dist-info/WHEEL
+Filename: shashvault-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: shashvault-0.0.8.dist-info/entry_points.txt
+Filename: shashvault-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: shashvault-0.0.8.dist-info/top_level.txt
+Filename: shashvault-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: shashvault-0.0.8.dist-info/RECORD
+Filename: shashvault-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `shashvault-0.0.8.dist-info/LICENSE` & `shashvault-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shashvault-0.0.8.dist-info/METADATA` & `shashvault-0.1.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shashvault
-Version: 0.0.8
+Version: 0.1.0
 Summary: search Hashicorp vault path and secret
 Home-page: https://gitlab.esss.lu.se/ics-infrastructure/shashvault
 Author: Remy Mudingay
 Author-email: remy.mudingay@ess.eu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -34,15 +34,15 @@
 
 For example:
 ```
 cat ~/.vaultenv
 export VAULT_ADDR=https://hashicorp-vault.local.com:8200
 export VAULT_SKIP_VERIFY=1
 export VAULT_TOKEN=eqw.f8-example-token-2hinwin
-export VAULT_KV_PAT=secret
+export VAULT_KV_PATH=secret
 ```
 ### Usage
 ```
 usage: shashvault [-h] [-sp SEARCH_PATH] [-ss SECRET_PATH]
 
 Search and display secrets in HashiCorp Vault
```

## Comparing `shashvault-0.0.8.dist-info/RECORD` & `shashvault-0.1.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 shashvault/__init__.py,sha256=BgKbBh7aubvQHftiaEqNjeP4iPviOR-JvJgoLrDkD6I,36
 shashvault/main.py,sha256=cTlhhAVr427bfasr8Sx6v0XrE1DdT5WtWe_JBkpTYjA,4108
-shashvault-0.0.8.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
-shashvault-0.0.8.dist-info/METADATA,sha256=THjAE4SL4cmGKYfRPSVarPCkQF1Fwn_KaGGaocRMEQw,1464
-shashvault-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-shashvault-0.0.8.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
-shashvault-0.0.8.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
-shashvault-0.0.8.dist-info/RECORD,,
+shashvault-0.1.0.dist-info/LICENSE,sha256=dF2Y3lQP-nEUvREYnUEJwLGPyMKtm5icbH2kNwPJB3g,1336
+shashvault-0.1.0.dist-info/METADATA,sha256=2Zp47SL_0hUK-QaWpnxLDtbIGAdUkPdWYDjFN2BqhGs,1465
+shashvault-0.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+shashvault-0.1.0.dist-info/entry_points.txt,sha256=RVBfwNsZ2ixZGlenOCZzAGrTG7f1G3hR2lYGHmQjMcs,51
+shashvault-0.1.0.dist-info/top_level.txt,sha256=ZPxarLINYufIg6fyHNxqDkknBVmHah2fy9qhpQjbJ_w,11
+shashvault-0.1.0.dist-info/RECORD,,
```

