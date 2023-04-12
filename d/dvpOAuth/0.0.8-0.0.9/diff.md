# Comparing `tmp/dvpOAuth-0.0.8.tar.gz` & `tmp/dvpOAuth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvpOAuth-0.0.8.tar", last modified: Fri Feb 17 05:20:23 2023, max compression
+gzip compressed data, was "dvpOAuth-0.0.9.tar", last modified: Fri Feb 17 05:42:35 2023, max compression
```

## Comparing `dvpOAuth-0.0.8.tar` & `dvpOAuth-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dingli     (501) staff       (20)        0 2023-02-17 05:20:23.649337 dvpOAuth-0.0.8/
--rw-r--r--   0 dingli     (501) staff       (20)        0 2022-12-23 00:01:17.000000 dvpOAuth-0.0.8/LICENSE
--rw-r--r--   0 dingli     (501) staff       (20)      921 2023-02-17 05:20:23.649088 dvpOAuth-0.0.8/PKG-INFO
--rw-r--r--   0 dingli     (501) staff       (20)      436 2022-12-23 00:01:28.000000 dvpOAuth-0.0.8/README.md
-drwxr-xr-x   0 dingli     (501) staff       (20)        0 2023-02-17 05:20:23.648036 dvpOAuth-0.0.8/dvpOAuth/
--rw-r--r--   0 dingli     (501) staff       (20)      162 2023-02-17 05:19:36.000000 dvpOAuth-0.0.8/dvpOAuth/__init__.py
--rw-r--r--   0 dingli     (501) staff       (20)    12612 2023-02-17 05:19:22.000000 dvpOAuth-0.0.8/dvpOAuth/class_OAuth.py
--rw-r--r--   0 dingli     (501) staff       (20)      131 2022-12-23 00:02:34.000000 dvpOAuth-0.0.8/dvpOAuth/error.py
--rw-r--r--   0 dingli     (501) staff       (20)      685 2022-12-28 06:52:03.000000 dvpOAuth-0.0.8/dvpOAuth/util.py
-drwxr-xr-x   0 dingli     (501) staff       (20)        0 2023-02-17 05:20:23.648899 dvpOAuth-0.0.8/dvpOAuth.egg-info/
--rw-r--r--   0 dingli     (501) staff       (20)      921 2023-02-17 05:20:23.000000 dvpOAuth-0.0.8/dvpOAuth.egg-info/PKG-INFO
--rw-r--r--   0 dingli     (501) staff       (20)      265 2023-02-17 05:20:23.000000 dvpOAuth-0.0.8/dvpOAuth.egg-info/SOURCES.txt
--rw-r--r--   0 dingli     (501) staff       (20)        1 2023-02-17 05:20:23.000000 dvpOAuth-0.0.8/dvpOAuth.egg-info/dependency_links.txt
--rw-r--r--   0 dingli     (501) staff       (20)       24 2023-02-17 05:20:23.000000 dvpOAuth-0.0.8/dvpOAuth.egg-info/requires.txt
--rw-r--r--   0 dingli     (501) staff       (20)        9 2023-02-17 05:20:23.000000 dvpOAuth-0.0.8/dvpOAuth.egg-info/top_level.txt
--rw-r--r--   0 dingli     (501) staff       (20)       38 2023-02-17 05:20:23.649380 dvpOAuth-0.0.8/setup.cfg
--rw-r--r--   0 dingli     (501) staff       (20)     1177 2023-02-17 05:19:45.000000 dvpOAuth-0.0.8/setup.py
+drwxr-xr-x   0 dingli     (501) staff       (20)        0 2023-02-17 05:42:35.822549 dvpOAuth-0.0.9/
+-rw-r--r--   0 dingli     (501) staff       (20)        0 2022-12-23 00:01:17.000000 dvpOAuth-0.0.9/LICENSE
+-rw-r--r--   0 dingli     (501) staff       (20)      921 2023-02-17 05:42:35.822303 dvpOAuth-0.0.9/PKG-INFO
+-rw-r--r--   0 dingli     (501) staff       (20)      436 2022-12-23 00:01:28.000000 dvpOAuth-0.0.9/README.md
+drwxr-xr-x   0 dingli     (501) staff       (20)        0 2023-02-17 05:42:35.821226 dvpOAuth-0.0.9/dvpOAuth/
+-rw-r--r--   0 dingli     (501) staff       (20)      162 2023-02-17 05:42:02.000000 dvpOAuth-0.0.9/dvpOAuth/__init__.py
+-rw-r--r--   0 dingli     (501) staff       (20)    12203 2023-02-17 05:41:15.000000 dvpOAuth-0.0.9/dvpOAuth/class_OAuth.py
+-rw-r--r--   0 dingli     (501) staff       (20)      131 2022-12-23 00:02:34.000000 dvpOAuth-0.0.9/dvpOAuth/error.py
+-rw-r--r--   0 dingli     (501) staff       (20)      685 2022-12-28 06:52:03.000000 dvpOAuth-0.0.9/dvpOAuth/util.py
+drwxr-xr-x   0 dingli     (501) staff       (20)        0 2023-02-17 05:42:35.822106 dvpOAuth-0.0.9/dvpOAuth.egg-info/
+-rw-r--r--   0 dingli     (501) staff       (20)      921 2023-02-17 05:42:35.000000 dvpOAuth-0.0.9/dvpOAuth.egg-info/PKG-INFO
+-rw-r--r--   0 dingli     (501) staff       (20)      265 2023-02-17 05:42:35.000000 dvpOAuth-0.0.9/dvpOAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 dingli     (501) staff       (20)        1 2023-02-17 05:42:35.000000 dvpOAuth-0.0.9/dvpOAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 dingli     (501) staff       (20)       24 2023-02-17 05:42:35.000000 dvpOAuth-0.0.9/dvpOAuth.egg-info/requires.txt
+-rw-r--r--   0 dingli     (501) staff       (20)        9 2023-02-17 05:42:35.000000 dvpOAuth-0.0.9/dvpOAuth.egg-info/top_level.txt
+-rw-r--r--   0 dingli     (501) staff       (20)       38 2023-02-17 05:42:35.822596 dvpOAuth-0.0.9/setup.cfg
+-rw-r--r--   0 dingli     (501) staff       (20)     1177 2023-02-17 05:41:45.000000 dvpOAuth-0.0.9/setup.py
```

### Comparing `dvpOAuth-0.0.8/PKG-INFO` & `dvpOAuth-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvpOAuth
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dominion API python wrapper
 Home-page: https://github.com/achillis2/dvpOAuth
 Author: Ding Li
 Author-email: dingli@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dvpOAuth-0.0.8/dvpOAuth/class_OAuth.py` & `dvpOAuth-0.0.9/dvpOAuth/class_OAuth.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,57 +186,39 @@
             "ServiceState": data["ServiceAddressState"],
             "ServiceZipCode": data["ServiceAddressZipCode"],
             "SwitchActive": "N",
             "SwitchInstalled": "N",
         }
         return res
 
-    def soap_U_format(self):
+    def soap_U_format(self, resp=None):
         return_dict = {
             'AccountSearchSequence': {
                 'AccountSearchSequence': []
             },
             'Header': {
-                'DateTimeStamp': None,
-                'MessageText': 'Validation fails: Invalid Account Number 12345',
-                'Result': 'U',
-                'ReturnCode': None
-            },
-            'MoreData': None,
-            'RowsReturned': None
-        }
-        return return_dict
-
-    def soap_W_format(self):
-        return_dict = {
-            'AccountSearchSequence': None,
-            'Header': {
                 'DateTimeStamp': datetime.now().strftime("%Y-%m-%d-%H.%M.%S.%f"),
-                'MessageText': 'No matches found for search criteria',
-                'Result': 'W',
-                'ReturnCode': 'A0016'
+                'MessageText': resp.get('ReturnMessageText',''),
+                'Result': resp.get('InternetReturnCode', ''),
+                'ReturnCode': resp.get('ErrorCode', '')
             },
-            'MoreData': 'N',
-            'RowsReturned': '0000'
+            'MoreData': resp.get('MoreData', ''),
+            'RowsReturned': resp.get('RowsReturned', '')
         }
         return return_dict
 
-
     def convert_account_search_json_from_oauth_to_soap(
         self, status_code=None, resp=None
     ):
         """convert the search result json to the soap format"""
         if not resp["d"]["results"]:
             return None
 
         if resp['d']['results'][0]['InternetReturnCode'] == 'U':
-            return self.soap_U_format()
-
-        if resp['d']['results'][0]['InternetReturnCode'] == 'W':
-            return self.soap_W_format()
+            return self.soap_U_format(resp['d']['results'][0])
 
         resp_parent = resp["d"]["results"][0]
         data = resp_parent["ZAcctSearchNav"]["results"][0]
 
         return_dict = {
             "AccountSearchSequence": {
                 "AccountSearchSequence": [
```

### Comparing `dvpOAuth-0.0.8/dvpOAuth/util.py` & `dvpOAuth-0.0.9/dvpOAuth/util.py`

 * *Files identical despite different names*

### Comparing `dvpOAuth-0.0.8/dvpOAuth.egg-info/PKG-INFO` & `dvpOAuth-0.0.9/dvpOAuth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvpOAuth
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dominion API python wrapper
 Home-page: https://github.com/achillis2/dvpOAuth
 Author: Ding Li
 Author-email: dingli@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dvpOAuth-0.0.8/setup.py` & `dvpOAuth-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Dominion API python wrapper'
 
 setup(
     name='dvpOAuth',
     version=VERSION,    
     description=DESCRIPTION,
     url='https://github.com/achillis2/dvpOAuth',
```

