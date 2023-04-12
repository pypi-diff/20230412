# Comparing `tmp/appwrite-1.2.0.tar.gz` & `tmp/appwrite-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appwrite-1.2.0.tar", last modified: Tue Dec 27 23:08:29 2022, max compression
+gzip compressed data, was "appwrite-2.0.0.tar", last modified: Wed Apr 12 10:01:29 2023, max compression
```

## Comparing `appwrite-1.2.0.tar` & `appwrite-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-12-27 23:08:29.331156 appwrite-1.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2022-12-27 23:08:11.000000 appwrite-1.2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2022-12-27 23:08:29.331156 appwrite-1.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4238 2022-12-27 23:08:11.000000 appwrite-1.2.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-12-27 23:08:29.327154 appwrite-1.2.0/appwrite/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6745 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/id.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      593 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/input_file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/permission.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1856 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-12-27 23:08:29.331156 appwrite-1.2.0/appwrite/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8488 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/avatars.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26454 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/databases.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13016 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      996 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/graphql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/health.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1875 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/locale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9352 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/storage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6764 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/teams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16087 2022-12-27 23:08:11.000000 appwrite-1.2.0/appwrite/services/users.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-12-27 23:08:29.331156 appwrite-1.2.0/appwrite.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2022-12-27 23:08:29.000000 appwrite-1.2.0/appwrite.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      691 2022-12-27 23:08:29.000000 appwrite-1.2.0/appwrite.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-12-27 23:08:29.000000 appwrite-1.2.0/appwrite.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2022-12-27 23:08:29.000000 appwrite-1.2.0/appwrite.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2022-12-27 23:08:29.000000 appwrite-1.2.0/appwrite.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2022-12-27 23:08:29.331156 appwrite-1.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2022-12-27 23:08:11.000000 appwrite-1.2.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.126136 appwrite-2.0.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2023-04-12 10:01:09.000000 appwrite-2.0.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-04-12 10:01:29.126136 appwrite-2.0.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4238 2023-04-12 10:01:09.000000 appwrite-2.0.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.122136 appwrite-2.0.0/appwrite/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6745 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      128 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/id.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      593 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/input_file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/permission.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/role.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/service.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.126136 appwrite-2.0.0/appwrite/services/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8488 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/avatars.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39693 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/databases.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12818 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      996 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/graphql.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/health.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1875 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/locale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9352 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7733 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/teams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16087 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/users.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.122136 appwrite-2.0.0/appwrite.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      691 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-04-12 10:01:29.126136 appwrite-2.0.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2023-04-12 10:01:09.000000 appwrite-2.0.0/setup.py
```

### Comparing `appwrite-1.2.0/LICENSE` & `appwrite-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Appwrite (https://appwrite.io) and individual contributors.
+Copyright (c) 2023 Appwrite (https://appwrite.io) and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
     2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `appwrite-1.2.0/PKG-INFO` & `appwrite-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 1.2.0
+Version: 2.0.0
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/1.2.0.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.0.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,20 +21,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.2.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.3.0-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
-**This SDK is compatible with Appwrite server version 1.2.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
+**This SDK is compatible with Appwrite server version 1.3.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
 
 ![Appwrite](https://appwrite.io/images/github.png)
 
 ## Installation
```

### Comparing `appwrite-1.2.0/README.md` & `appwrite-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.2.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.3.0-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
-**This SDK is compatible with Appwrite server version 1.2.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
+**This SDK is compatible with Appwrite server version 1.3.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
 
 ![Appwrite](https://appwrite.io/images/github.png)
 
 ## Installation
```

### Comparing `appwrite-1.2.0/appwrite/client.py` & `appwrite-2.0.0/appwrite/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._self_signed = False
         self._endpoint = 'https://HOSTNAME/v1'
         self._global_headers = {
             'content-type': '',
             'x-sdk-name': 'Python',
             'x-sdk-platform': 'server',
             'x-sdk-language': 'python',
-            'x-sdk-version': '1.2.0',
+            'x-sdk-version': '2.0.0',
             'X-Appwrite-Response-Format' : '1.0.0',
         }
 
     def set_self_signed(self, status=True):
         self._self_signed = status
         return self
```

### Comparing `appwrite-1.2.0/appwrite/input_file.py` & `appwrite-2.0.0/appwrite/input_file.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/query.py` & `appwrite-2.0.0/appwrite/query.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,86 @@
 class Query:
     @staticmethod
     def equal(attribute, value):
-        return Query.addQuery(attribute, "equal", value)
+        return Query.add_query(attribute, "equal", value)
 
     @staticmethod
-    def notEqual(attribute, value):
-        return Query.addQuery(attribute, "notEqual", value)
+    def not_equal(attribute, value):
+        return Query.add_query(attribute, "notEqual", value)
     
     @staticmethod
-    def lessThan(attribute, value):
-        return Query.addQuery(attribute, "lessThan", value)
+    def less_than(attribute, value):
+        return Query.add_query(attribute, "lessThan", value)
     
     @staticmethod
-    def lessThanEqual(attribute, value):
-        return Query.addQuery(attribute, "lessThanEqual", value)
+    def less_than_equal(attribute, value):
+        return Query.add_query(attribute, "lessThanEqual", value)
     
     @staticmethod
-    def greaterThan(attribute, value):
-        return Query.addQuery(attribute, "greaterThan", value)
+    def greater_than(attribute, value):
+        return Query.add_query(attribute, "greaterThan", value)
     
     @staticmethod
-    def greaterThanEqual(attribute, value):
-        return Query.addQuery(attribute, "greaterThanEqual", value)
+    def greater_than_equal(attribute, value):
+        return Query.add_query(attribute, "greaterThanEqual", value)
+
+    @staticmethod
+    def is_null(attribute):
+        return f'isNull("{attribute}")'
+
+    @staticmethod
+    def is_not_null(attribute):
+        return f'isNotNull("{attribute}")'
+
+    @staticmethod
+    def between(attribute, start, end):
+        return Query.add_query(attribute, "between", [start, end])
+
+    @staticmethod
+    def starts_with(attribute, value):
+        return Query.add_query(attribute, "startsWith", value)
+
+    @staticmethod
+    def ends_with(attribute, value):
+        return Query.add_query(attribute, "endsWith", value)
+
+    @staticmethod
+    def select(attributes):
+        return f'select([{",".join(map(Query.parseValues, attributes))}])'
 
     @staticmethod
     def search(attribute, value):
-        return Query.addQuery(attribute, "search", value)
+        return Query.add_query(attribute, "search", value)
 
     @staticmethod
-    def orderAsc(attribute):
+    def order_asc(attribute):
         return f'orderAsc("{attribute}")'
 
     @staticmethod
-    def orderDesc(attribute):
+    def order_desc(attribute):
         return f'orderDesc("{attribute}")'
 
     @staticmethod
-    def cursorBefore(id):
+    def cursor_before(id):
         return f'cursorBefore("{id}")'
 
     @staticmethod
-    def cursorAfter(id):
+    def cursor_after(id):
         return f'cursorAfter("{id}")'
 
     @staticmethod
     def limit(limit):
         return f'limit({limit})'
 
     @staticmethod
     def offset(offset):
         return f'offset({offset})'
 
     @staticmethod
-    def addQuery(attribute, method, value):
+    def add_query(attribute, method, value):
         if type(value) == list:
             return f'{method}("{attribute}", [{",".join(map(Query.parseValues, value))}])'
         else:
             return f'{method}("{attribute}", [{Query.parseValues(value)}])'
 
     @staticmethod
     def parseValues(value):
```

### Comparing `appwrite-1.2.0/appwrite/role.py` & `appwrite-2.0.0/appwrite/role.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/services/account.py` & `appwrite-2.0.0/appwrite/services/account.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/services/avatars.py` & `appwrite-2.0.0/appwrite/services/avatars.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/services/databases.py` & `appwrite-2.0.0/appwrite/services/databases.py`

 * *Files 17% similar despite different names*

```diff
@@ -249,14 +249,46 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_boolean_attribute(self, database_id, collection_id, key, required, default):
+        """Update Boolean Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/boolean/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_datetime_attribute(self, database_id, collection_id, key, required, default = None, array = None):
         """Create DateTime Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/datetime'
         params = {}
         if database_id is None:
@@ -279,14 +311,46 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_datetime_attribute(self, database_id, collection_id, key, required, default):
+        """Update DateTime Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/datetime/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_email_attribute(self, database_id, collection_id, key, required, default = None, array = None):
         """Create Email Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/email'
         params = {}
         if database_id is None:
@@ -309,14 +373,46 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_email_attribute(self, database_id, collection_id, key, required, default):
+        """Update Email Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/email/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_enum_attribute(self, database_id, collection_id, key, elements, required, default = None, array = None):
         """Create Enum Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/enum'
         params = {}
         if database_id is None:
@@ -343,14 +439,50 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_enum_attribute(self, database_id, collection_id, key, elements, required, default):
+        """Update Enum Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/enum/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if elements is None:
+            raise AppwriteException('Missing required parameter: "elements"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['elements'] = elements
+        params['required'] = required
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_float_attribute(self, database_id, collection_id, key, required, min = None, max = None, default = None, array = None):
         """Create Float Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/float'
         params = {}
         if database_id is None:
@@ -375,14 +507,54 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_float_attribute(self, database_id, collection_id, key, required, min, max, default):
+        """Update Float Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/float/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if min is None:
+            raise AppwriteException('Missing required parameter: "min"')
+
+        if max is None:
+            raise AppwriteException('Missing required parameter: "max"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['min'] = min
+        params['max'] = max
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_integer_attribute(self, database_id, collection_id, key, required, min = None, max = None, default = None, array = None):
         """Create Integer Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/integer'
         params = {}
         if database_id is None:
@@ -407,14 +579,54 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_integer_attribute(self, database_id, collection_id, key, required, min, max, default):
+        """Update Integer Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/integer/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if min is None:
+            raise AppwriteException('Missing required parameter: "min"')
+
+        if max is None:
+            raise AppwriteException('Missing required parameter: "max"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['min'] = min
+        params['max'] = max
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_ip_attribute(self, database_id, collection_id, key, required, default = None, array = None):
         """Create IP Address Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/ip'
         params = {}
         if database_id is None:
@@ -437,14 +649,78 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_ip_attribute(self, database_id, collection_id, key, required, default):
+        """Update IP Address Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/ip/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
+    def create_relationship_attribute(self, database_id, collection_id, related_collection_id, type, two_way = None, key = None, two_way_key = None, on_delete = None):
+        """Create Relationship Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/relationship'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if related_collection_id is None:
+            raise AppwriteException('Missing required parameter: "related_collection_id"')
+
+        if type is None:
+            raise AppwriteException('Missing required parameter: "type"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+
+        params['relatedCollectionId'] = related_collection_id
+        params['type'] = type
+        params['twoWay'] = two_way
+        params['key'] = key
+        params['twoWayKey'] = two_way_key
+        params['onDelete'] = on_delete
+
+        return self.client.call('post', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_string_attribute(self, database_id, collection_id, key, size, required, default = None, array = None):
         """Create String Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/string'
         params = {}
         if database_id is None:
@@ -471,14 +747,46 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_string_attribute(self, database_id, collection_id, key, required, default):
+        """Update String Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/string/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def create_url_attribute(self, database_id, collection_id, key, required, default = None, array = None):
         """Create URL Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/url'
         params = {}
         if database_id is None:
@@ -501,14 +809,46 @@
         params['default'] = default
         params['array'] = array
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_url_attribute(self, database_id, collection_id, key, required, default):
+        """Update URL Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/url/{key}'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        if required is None:
+            raise AppwriteException('Missing required parameter: "required"')
+
+        if default is None:
+            raise AppwriteException('Missing required parameter: "default"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['required'] = required
+        params['default'] = default
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def get_attribute(self, database_id, collection_id, key):
         """Get Attribute"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/attributes/{key}'
         params = {}
         if database_id is None:
@@ -549,14 +889,39 @@
         path = path.replace('{key}', key)
 
 
         return self.client.call('delete', path, {
             'content-type': 'application/json',
         }, params)
 
+    def update_relationship_attribute(self, database_id, collection_id, key, on_delete = None):
+        """Update Relationship Attribute"""
+
+        
+        path = '/databases/{databaseId}/collections/{collectionId}/attributes/{key}/relationship'
+        params = {}
+        if database_id is None:
+            raise AppwriteException('Missing required parameter: "database_id"')
+
+        if collection_id is None:
+            raise AppwriteException('Missing required parameter: "collection_id"')
+
+        if key is None:
+            raise AppwriteException('Missing required parameter: "key"')
+
+        path = path.replace('{databaseId}', database_id)
+        path = path.replace('{collectionId}', collection_id)
+        path = path.replace('{key}', key)
+
+        params['onDelete'] = on_delete
+
+        return self.client.call('patch', path, {
+            'content-type': 'application/json',
+        }, params)
+
     def list_documents(self, database_id, collection_id, queries = None):
         """List Documents"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/documents'
         params = {}
         if database_id is None:
@@ -599,15 +964,15 @@
         params['data'] = data
         params['permissions'] = permissions
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
 
-    def get_document(self, database_id, collection_id, document_id):
+    def get_document(self, database_id, collection_id, document_id, queries = None):
         """Get Document"""
 
         
         path = '/databases/{databaseId}/collections/{collectionId}/documents/{documentId}'
         params = {}
         if database_id is None:
             raise AppwriteException('Missing required parameter: "database_id"')
@@ -618,14 +983,15 @@
         if document_id is None:
             raise AppwriteException('Missing required parameter: "document_id"')
 
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{documentId}', document_id)
 
+        params['queries'] = queries
 
         return self.client.call('get', path, {
             'content-type': 'application/json',
         }, params)
 
     def update_document(self, database_id, collection_id, document_id, data = None, permissions = None):
         """Update Document"""
```

### Comparing `appwrite-1.2.0/appwrite/services/functions.py` & `appwrite-2.0.0/appwrite/services/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,26 @@
         params['queries'] = queries
         params['search'] = search
 
         return self.client.call('get', path, {
             'content-type': 'application/json',
         }, params)
 
-    def create(self, function_id, name, execute, runtime, events = None, schedule = None, timeout = None, enabled = None):
+    def create(self, function_id, name, runtime, execute = None, events = None, schedule = None, timeout = None, enabled = None):
         """Create Function"""
 
         
         path = '/functions'
         params = {}
         if function_id is None:
             raise AppwriteException('Missing required parameter: "function_id"')
 
         if name is None:
             raise AppwriteException('Missing required parameter: "name"')
 
-        if execute is None:
-            raise AppwriteException('Missing required parameter: "execute"')
-
         if runtime is None:
             raise AppwriteException('Missing required parameter: "runtime"')
 
 
         params['functionId'] = function_id
         params['name'] = name
         params['execute'] = execute
@@ -75,29 +72,26 @@
         path = path.replace('{functionId}', function_id)
 
 
         return self.client.call('get', path, {
             'content-type': 'application/json',
         }, params)
 
-    def update(self, function_id, name, execute, events = None, schedule = None, timeout = None, enabled = None):
+    def update(self, function_id, name, execute = None, events = None, schedule = None, timeout = None, enabled = None):
         """Update Function"""
 
         
         path = '/functions/{functionId}'
         params = {}
         if function_id is None:
             raise AppwriteException('Missing required parameter: "function_id"')
 
         if name is None:
             raise AppwriteException('Missing required parameter: "name"')
 
-        if execute is None:
-            raise AppwriteException('Missing required parameter: "execute"')
-
         path = path.replace('{functionId}', function_id)
 
         params['name'] = name
         params['execute'] = execute
         params['events'] = events
         params['schedule'] = schedule
         params['timeout'] = timeout
```

### Comparing `appwrite-1.2.0/appwrite/services/graphql.py` & `appwrite-2.0.0/appwrite/services/graphql.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/services/health.py` & `appwrite-2.0.0/appwrite/services/health.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/services/locale.py` & `appwrite-2.0.0/appwrite/services/locale.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/services/storage.py` & `appwrite-2.0.0/appwrite/services/storage.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite/services/teams.py` & `appwrite-2.0.0/appwrite/services/teams.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         path = path.replace('{teamId}', team_id)
 
 
         return self.client.call('get', path, {
             'content-type': 'application/json',
         }, params)
 
-    def update(self, team_id, name):
-        """Update Team"""
+    def update_name(self, team_id, name):
+        """Update Name"""
 
         
         path = '/teams/{teamId}'
         params = {}
         if team_id is None:
             raise AppwriteException('Missing required parameter: "team_id"')
 
@@ -107,35 +107,34 @@
         params['queries'] = queries
         params['search'] = search
 
         return self.client.call('get', path, {
             'content-type': 'application/json',
         }, params)
 
-    def create_membership(self, team_id, email, roles, url, name = None):
+    def create_membership(self, team_id, roles, url, email = None, user_id = None, phone = None, name = None):
         """Create Team Membership"""
 
         
         path = '/teams/{teamId}/memberships'
         params = {}
         if team_id is None:
             raise AppwriteException('Missing required parameter: "team_id"')
 
-        if email is None:
-            raise AppwriteException('Missing required parameter: "email"')
-
         if roles is None:
             raise AppwriteException('Missing required parameter: "roles"')
 
         if url is None:
             raise AppwriteException('Missing required parameter: "url"')
 
         path = path.replace('{teamId}', team_id)
 
         params['email'] = email
+        params['userId'] = user_id
+        params['phone'] = phone
         params['roles'] = roles
         params['url'] = url
         params['name'] = name
 
         return self.client.call('post', path, {
             'content-type': 'application/json',
         }, params)
@@ -227,7 +226,43 @@
 
         params['userId'] = user_id
         params['secret'] = secret
 
         return self.client.call('patch', path, {
             'content-type': 'application/json',
         }, params)
+
+    def get_prefs(self, team_id):
+        """Get Team Preferences"""
+
+        
+        path = '/teams/{teamId}/prefs'
+        params = {}
+        if team_id is None:
+            raise AppwriteException('Missing required parameter: "team_id"')
+
+        path = path.replace('{teamId}', team_id)
+
+
+        return self.client.call('get', path, {
+            'content-type': 'application/json',
+        }, params)
+
+    def update_prefs(self, team_id, prefs):
+        """Update Preferences"""
+
+        
+        path = '/teams/{teamId}/prefs'
+        params = {}
+        if team_id is None:
+            raise AppwriteException('Missing required parameter: "team_id"')
+
+        if prefs is None:
+            raise AppwriteException('Missing required parameter: "prefs"')
+
+        path = path.replace('{teamId}', team_id)
+
+        params['prefs'] = prefs
+
+        return self.client.call('put', path, {
+            'content-type': 'application/json',
+        }, params)
```

### Comparing `appwrite-1.2.0/appwrite/services/users.py` & `appwrite-2.0.0/appwrite/services/users.py`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/appwrite.egg-info/PKG-INFO` & `appwrite-2.0.0/appwrite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 1.2.0
+Version: 2.0.0
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/1.2.0.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.0.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,20 +21,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.2.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.3.0-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
-**This SDK is compatible with Appwrite server version 1.2.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
+**This SDK is compatible with Appwrite server version 1.3.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
 
 ![Appwrite](https://appwrite.io/images/github.png)
 
 ## Installation
```

### Comparing `appwrite-1.2.0/appwrite.egg-info/SOURCES.txt` & `appwrite-2.0.0/appwrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appwrite-1.2.0/setup.py` & `appwrite-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 with open("README.md", "r", encoding="utf-8") as readme_file_desc:
     long_description = readme_file_desc.read()
     
 setuptools.setup(
   name = 'appwrite',
   packages = ['appwrite', 'appwrite/services'],
-  version = '1.2.0',
+  version = '2.0.0',
   license='BSD-3-Clause',
   description = 'Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Appwrite Team',
   author_email = 'team@appwrite.io',
   maintainer = 'Appwrite Team',
   maintainer_email = 'team@appwrite.io',
   url = 'https://appwrite.io/support',
-  download_url='https://github.com/appwrite/sdk-for-python/archive/1.2.0.tar.gz',
+  download_url='https://github.com/appwrite/sdk-for-python/archive/2.0.0.tar.gz',
   # keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],
   install_requires=[
           'requests',
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
```

