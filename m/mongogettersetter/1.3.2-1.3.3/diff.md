# Comparing `tmp/mongogettersetter-1.3.2.tar.gz` & `tmp/mongogettersetter-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.3.2.tar", last modified: Wed Apr 12 14:18:20 2023, max compression
+gzip compressed data, was "mongogettersetter-1.3.3.tar", last modified: Wed Apr 12 16:07:35 2023, max compression
```

## Comparing `mongogettersetter-1.3.2.tar` & `mongogettersetter-1.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 14:18:20.839585 mongogettersetter-1.3.2/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29533 2023-04-12 14:18:20.839585 mongogettersetter-1.3.2/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28936 2023-04-12 14:17:32.000000 mongogettersetter-1.3.2/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 14:18:20.835585 mongogettersetter-1.3.2/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24177 2023-04-12 12:58:33.000000 mongogettersetter-1.3.2/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 14:18:20.839585 mongogettersetter-1.3.2/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29533 2023-04-12 14:18:20.000000 mongogettersetter-1.3.2/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-04-12 14:18:20.000000 mongogettersetter-1.3.2/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-04-12 14:18:20.000000 mongogettersetter-1.3.2/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-04-12 14:18:20.000000 mongogettersetter-1.3.2/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-04-12 14:18:20.000000 mongogettersetter-1.3.2/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-04-12 14:18:20.839585 mongogettersetter-1.3.2/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-04-12 14:17:53.000000 mongogettersetter-1.3.2/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.3/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24177 2023-04-12 12:58:33.000000 mongogettersetter-1.3.3/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-04-12 16:07:31.000000 mongogettersetter-1.3.3/setup.py
```

### Comparing `mongogettersetter-1.3.2/PKG-INFO` & `mongogettersetter-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.2
+Version: 1.3.3
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -70,23 +70,23 @@
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `EmployeeCollection` in `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 ```
 
-This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
+This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, `Employee` class will create a new document with the given `id` when initialized. `EmployeeCollection` is designed to replace your MongoDB collection object, so you can use it as a drop-in replacement for your MongoDB collection object inside any class, and perform operations in it according to this documentation.
 
 For example:
 
 ```
 >>> e = EmployeeCollection(4051)
 ```
 
-Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
+Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. When inside `Employee` class, it can be accessed like `self.collection`. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
 
 ```
 >>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
```

### Comparing `mongogettersetter-1.3.2/README.md` & `mongogettersetter-1.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `EmployeeCollection` in `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 ```
 
-This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
+This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, `Employee` class will create a new document with the given `id` when initialized. `EmployeeCollection` is designed to replace your MongoDB collection object, so you can use it as a drop-in replacement for your MongoDB collection object inside any class, and perform operations in it according to this documentation.
 
 For example:
 
 ```
 >>> e = EmployeeCollection(4051)
 ```
 
-Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
+Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. When inside `Employee` class, it can be accessed like `self.collection`. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
 
 ```
 >>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
```

### Comparing `mongogettersetter-1.3.2/mongogettersetter/__init__.py` & `mongogettersetter-1.3.3/mongogettersetter/__init__.py`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.3.2/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.3.3/mongogettersetter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.2
+Version: 1.3.3
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -70,23 +70,23 @@
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `EmployeeCollection` in `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 ```
 
-This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
+This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, `Employee` class will create a new document with the given `id` when initialized. `EmployeeCollection` is designed to replace your MongoDB collection object, so you can use it as a drop-in replacement for your MongoDB collection object inside any class, and perform operations in it according to this documentation.
 
 For example:
 
 ```
 >>> e = EmployeeCollection(4051)
 ```
 
-Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
+Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. When inside `Employee` class, it can be accessed like `self.collection`. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
 
 ```
 >>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
```

### Comparing `mongogettersetter-1.3.2/setup.py` & `mongogettersetter-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.3.2',
+    version='1.3.3',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

