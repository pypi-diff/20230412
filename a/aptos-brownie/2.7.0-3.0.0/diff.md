# Comparing `tmp/aptos_brownie-2.7.0-py3-none-any.whl.zip` & `tmp/aptos_brownie-3.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7370 bytes, number of entries: 5
--rw-r--r--  2.0 unx    33233 b- defN 23-Apr-08 14:34 aptos_brownie.py
--rw-r--r--  2.0 unx      911 b- defN 23-Apr-08 14:35 aptos_brownie-2.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 14:35 aptos_brownie-2.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-08 14:35 aptos_brownie-2.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-08 14:35 aptos_brownie-2.7.0.dist-info/RECORD
-5 files, 34645 bytes uncompressed, 6632 bytes compressed:  80.9%
+Zip file size: 7462 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    33691 b- defN 23-Apr-12 05:13 aptos_brownie.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/RECORD
+5 files, 35083 bytes uncompressed, 6724 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aptos_brownie.py
 Comment: 
 
-Filename: aptos_brownie-2.7.0.dist-info/METADATA
+Filename: aptos_brownie-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: aptos_brownie-2.7.0.dist-info/WHEEL
+Filename: aptos_brownie-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: aptos_brownie-2.7.0.dist-info/top_level.txt
+Filename: aptos_brownie-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aptos_brownie-2.7.0.dist-info/RECORD
+Filename: aptos_brownie-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aptos_brownie.py

```diff
@@ -825,7 +825,18 @@
             url = f"{self.rest_client.base_url}/accounts/{address}/events/{event_handle}/{field_name}?limit={limit}"
         else:
             url = f"{self.rest_client.base_url}/accounts/{address}/events/{event_handle}/{field_name}"
         response = self.rest_client.client.get(url)
         if response.status_code >= 400:
             raise ApiError(response.text, response.status_code)
         return response.json()
+
+
+def get_account_balance(node_url, account_address, coin_type):
+    rest_client = RestClient(node_url)
+    resource_type = f"0x1::coin::CoinStore<{coin_type}>"
+    response = rest_client.client.get(
+        f"{node_url}/accounts/{account_address}/resource/{resource_type}"
+    )
+    if response.status_code >= 400:
+        raise ApiError(f"{response.text} - {account_address}", response.status_code)
+    return int(response.json()["data"]["coin"]["value"])
```

## Comparing `aptos_brownie-2.7.0.dist-info/METADATA` & `aptos_brownie-3.0.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: aptos-brownie
-Version: 2.7.0
+Version: 3.0.0
 Summary: Aptos Package Tool
 Home-page: https://github.com/OmniBTC/OmniSwap/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -20,9 +19,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Requires-Dist: aptos-sdk
 Requires-Dist: pyyaml
 Requires-Dist: toml
 
 This is an aptos python tool to quickly implement aptos calls
-
-
```

