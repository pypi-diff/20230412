# Comparing `tmp/mongogettersetter-1.3.0.tar.gz` & `tmp/mongogettersetter-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.3.0.tar", last modified: Wed Apr 12 10:55:19 2023, max compression
+gzip compressed data, was "mongogettersetter-1.3.1.tar", last modified: Wed Apr 12 13:31:02 2023, max compression
```

## Comparing `mongogettersetter-1.3.0.tar` & `mongogettersetter-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 10:55:19.139999 mongogettersetter-1.3.0/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28839 2023-04-12 10:55:19.139999 mongogettersetter-1.3.0/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28242 2023-04-12 10:55:04.000000 mongogettersetter-1.3.0/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 10:55:19.136000 mongogettersetter-1.3.0/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24177 2023-03-29 06:06:12.000000 mongogettersetter-1.3.0/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 10:55:19.139999 mongogettersetter-1.3.0/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28839 2023-04-12 10:55:19.000000 mongogettersetter-1.3.0/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-04-12 10:55:19.000000 mongogettersetter-1.3.0/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-04-12 10:55:19.000000 mongogettersetter-1.3.0/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-04-12 10:55:19.000000 mongogettersetter-1.3.0/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-04-12 10:55:19.000000 mongogettersetter-1.3.0/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-04-12 10:55:19.139999 mongogettersetter-1.3.0/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-04-12 10:55:12.000000 mongogettersetter-1.3.0/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 13:31:02.965840 mongogettersetter-1.3.1/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29494 2023-04-12 13:31:02.965840 mongogettersetter-1.3.1/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28897 2023-04-12 13:28:49.000000 mongogettersetter-1.3.1/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 13:31:02.965840 mongogettersetter-1.3.1/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24177 2023-04-12 12:58:33.000000 mongogettersetter-1.3.1/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 13:31:02.965840 mongogettersetter-1.3.1/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29494 2023-04-12 13:31:02.000000 mongogettersetter-1.3.1/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-04-12 13:31:02.000000 mongogettersetter-1.3.1/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-04-12 13:31:02.000000 mongogettersetter-1.3.1/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-04-12 13:31:02.000000 mongogettersetter-1.3.1/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-04-12 13:31:02.000000 mongogettersetter-1.3.1/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-04-12 13:31:02.965840 mongogettersetter-1.3.1/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-04-12 13:20:48.000000 mongogettersetter-1.3.1/setup.py
```

### Comparing `mongogettersetter-1.3.0/PKG-INFO` & `mongogettersetter-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.0
+Version: 1.3.1
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -23,37 +23,46 @@
 [![Downloads](https://pepy.tech/badge/mongogettersetter/week)](https://pepy.tech/project/mongogettersetter/week)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 
 The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and other datatypes like `int`, `bool` `float` and `list` are all handled by `MongoDataWrapper`.
 
-Here, we initialize `Employee` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
+Here, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
 
 
 ### Usage of `MongoGetterSetter` metaclass
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
 # Connect to the MongoDB database and collection
 
 client = MongoClient("mongodb://localhost:27017/")
 db = client["example_db"]
 collection = db["employee"]
-class Employee(metaclass=MongoGetterSetter):
+
+# Wrapper for MongoDB Collection with metaclass, use this inside your actual class.
+class EmployeeClass(metaclass=MongoGetterSetter):
     def __init__(self, _id):
-    self._filter_query = {"id": _id} # or the ObjectID, at your convinence
-    self._collection = collection # Should be a pymongo.MongoClient[database].collection
+        self._filter_query = {"id": _id} # or the ObjectID, at your convinence
+        self._collection = collection # Should be a pymongo.MongoClient[database].collection
 
-    # if the document doesn't exist, we could create it here
-    try:
-        self._id # if the document doesn't exist, self._id will raise TypeError
-    except TypeError:
-        self._collection.insert_one(self._filter_query)
+class Employee:
+    def __init__(self, _id):
+        self._filter_query = {"id": _id}
+        self._collection = collection
+        self.collection = EmployeeCollection(_id)
+
+        # Create a new document if it doesn't exist
+        if self.collection.get() is None:
+            self._collection.insert_one(self._filter_query)
+    
+    def someOtherOperation(self):
+        self.collection.hello = "Hello World"  
 
 ```
 
 Now, save the above code in a file named `employee.py` and run the following command in the same directory:
 
 ```
 $ python3 -i employee.py
@@ -61,26 +70,26 @@
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 ```
 
-This can be accessed by creating an instance of `Employee` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
+This can be accessed by creating an instance of `EmployeeClass` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
 
 For example:
 
 ```
->>> e = Employee(4051)
+>>> e = EmployeeCollection(4051)
 ```
 
-Now this `e` object is an instance of `Employee` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
+Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
 
 ```
->>> e = Employee(4051)
+>>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
 >>> e.id.get()
 4051
 >>> e.name
@@ -182,15 +191,15 @@
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
 
     Example:
     ```
-    obj = Employee(_id)
+    obj = EmployeeClass(_id)
     result = obj.some_key
     ```
 - `__getitem__(self, key, value)`: Gets the value of the specified `key` from the MongoDB document.
 
     Example:
 
     ```
@@ -394,43 +403,48 @@
                 "status": "in progress"
             }
         ]
     }
 ]
 ```
 
-Now, let's create a class called `People` with `MongoGetterSetter` as its metaclass.
+Now, let's create a class called `People` and `PeopleCollection` with `MongoGetterSetter` as its metaclass.
 
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
 # Connect to the MongoDB database and collection
 client = MongoClient("mongodb://localhost:27017/")
 db = client["example_db"]
 people_collection = db["people"]
 
-class People(metaclass=MongoGetterSetter):
+# Wrapper for MongoDB Collection with metaclass, use this inside your actual class.
+class PeopleCollection(metaclass=MongoGetterSetter):
     def __init__(self, _id):
         self._filter_query = {"id": _id}  # or the ObjectID, at your convenience
         self._collection = people_collection  # Should be a pymongo.MongoClient[database].collection
 
-        try:
-            self._id # if the document doesn't exist, self._id will raise TypeError
-        except TypeError:
-            self._collection.insert_one({
-                "id": _id
-            })
+class People():
+    def __init__(self, _id):
+        self.collection = PeopleCollection(_id)
+        self._filter_query = {"id": _id}
+        self._collection = people_collection
+        if self.collection.get() is None:
+            self._collection.insert_one(self._filter_query)
+    
+    def someOtherOperation(self):
+        self.collection.hello = "Hello World"       
 ```
 
 
 
-Create a People object for Alice with `id = 1`
+Create a PeopleCollection object for Alice with `id = 1`
 ```
-alice = People(1)
+alice = PeopleCollection(1)
 ```
 
 Access and modify Alice's name
 ```
 print(alice.name)  # Output: 'Alice'
 alice.name = "Alice Johnson"
 print(alice.name)  # Output: 'Alice Johnson'
```

### Comparing `mongogettersetter-1.3.0/README.md` & `mongogettersetter-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,46 @@
 [![Downloads](https://pepy.tech/badge/mongogettersetter/week)](https://pepy.tech/project/mongogettersetter/week)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 
 The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and other datatypes like `int`, `bool` `float` and `list` are all handled by `MongoDataWrapper`.
 
-Here, we initialize `Employee` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
+Here, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
 
 
 ### Usage of `MongoGetterSetter` metaclass
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
 # Connect to the MongoDB database and collection
 
 client = MongoClient("mongodb://localhost:27017/")
 db = client["example_db"]
 collection = db["employee"]
-class Employee(metaclass=MongoGetterSetter):
+
+# Wrapper for MongoDB Collection with metaclass, use this inside your actual class.
+class EmployeeClass(metaclass=MongoGetterSetter):
     def __init__(self, _id):
-    self._filter_query = {"id": _id} # or the ObjectID, at your convinence
-    self._collection = collection # Should be a pymongo.MongoClient[database].collection
+        self._filter_query = {"id": _id} # or the ObjectID, at your convinence
+        self._collection = collection # Should be a pymongo.MongoClient[database].collection
 
-    # if the document doesn't exist, we could create it here
-    try:
-        self._id # if the document doesn't exist, self._id will raise TypeError
-    except TypeError:
-        self._collection.insert_one(self._filter_query)
+class Employee:
+    def __init__(self, _id):
+        self._filter_query = {"id": _id}
+        self._collection = collection
+        self.collection = EmployeeCollection(_id)
+
+        # Create a new document if it doesn't exist
+        if self.collection.get() is None:
+            self._collection.insert_one(self._filter_query)
+    
+    def someOtherOperation(self):
+        self.collection.hello = "Hello World"  
 
 ```
 
 Now, save the above code in a file named `employee.py` and run the following command in the same directory:
 
 ```
 $ python3 -i employee.py
@@ -45,26 +54,26 @@
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 ```
 
-This can be accessed by creating an instance of `Employee` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
+This can be accessed by creating an instance of `EmployeeClass` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
 
 For example:
 
 ```
->>> e = Employee(4051)
+>>> e = EmployeeCollection(4051)
 ```
 
-Now this `e` object is an instance of `Employee` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
+Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
 
 ```
->>> e = Employee(4051)
+>>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
 >>> e.id.get()
 4051
 >>> e.name
@@ -166,15 +175,15 @@
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
 
     Example:
     ```
-    obj = Employee(_id)
+    obj = EmployeeClass(_id)
     result = obj.some_key
     ```
 - `__getitem__(self, key, value)`: Gets the value of the specified `key` from the MongoDB document.
 
     Example:
 
     ```
@@ -378,43 +387,48 @@
                 "status": "in progress"
             }
         ]
     }
 ]
 ```
 
-Now, let's create a class called `People` with `MongoGetterSetter` as its metaclass.
+Now, let's create a class called `People` and `PeopleCollection` with `MongoGetterSetter` as its metaclass.
 
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
 # Connect to the MongoDB database and collection
 client = MongoClient("mongodb://localhost:27017/")
 db = client["example_db"]
 people_collection = db["people"]
 
-class People(metaclass=MongoGetterSetter):
+# Wrapper for MongoDB Collection with metaclass, use this inside your actual class.
+class PeopleCollection(metaclass=MongoGetterSetter):
     def __init__(self, _id):
         self._filter_query = {"id": _id}  # or the ObjectID, at your convenience
         self._collection = people_collection  # Should be a pymongo.MongoClient[database].collection
 
-        try:
-            self._id # if the document doesn't exist, self._id will raise TypeError
-        except TypeError:
-            self._collection.insert_one({
-                "id": _id
-            })
+class People():
+    def __init__(self, _id):
+        self.collection = PeopleCollection(_id)
+        self._filter_query = {"id": _id}
+        self._collection = people_collection
+        if self.collection.get() is None:
+            self._collection.insert_one(self._filter_query)
+    
+    def someOtherOperation(self):
+        self.collection.hello = "Hello World"       
 ```
 
 
 
-Create a People object for Alice with `id = 1`
+Create a PeopleCollection object for Alice with `id = 1`
 ```
-alice = People(1)
+alice = PeopleCollection(1)
 ```
 
 Access and modify Alice's name
 ```
 print(alice.name)  # Output: 'Alice'
 alice.name = "Alice Johnson"
 print(alice.name)  # Output: 'Alice Johnson'
```

### Comparing `mongogettersetter-1.3.0/mongogettersetter/__init__.py` & `mongogettersetter-1.3.1/mongogettersetter/__init__.py`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.3.0/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.3.1/mongogettersetter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.0
+Version: 1.3.1
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -23,37 +23,46 @@
 [![Downloads](https://pepy.tech/badge/mongogettersetter/week)](https://pepy.tech/project/mongogettersetter/week)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 
 The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and other datatypes like `int`, `bool` `float` and `list` are all handled by `MongoDataWrapper`.
 
-Here, we initialize `Employee` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
+Here, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
 
 
 ### Usage of `MongoGetterSetter` metaclass
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
 # Connect to the MongoDB database and collection
 
 client = MongoClient("mongodb://localhost:27017/")
 db = client["example_db"]
 collection = db["employee"]
-class Employee(metaclass=MongoGetterSetter):
+
+# Wrapper for MongoDB Collection with metaclass, use this inside your actual class.
+class EmployeeClass(metaclass=MongoGetterSetter):
     def __init__(self, _id):
-    self._filter_query = {"id": _id} # or the ObjectID, at your convinence
-    self._collection = collection # Should be a pymongo.MongoClient[database].collection
+        self._filter_query = {"id": _id} # or the ObjectID, at your convinence
+        self._collection = collection # Should be a pymongo.MongoClient[database].collection
 
-    # if the document doesn't exist, we could create it here
-    try:
-        self._id # if the document doesn't exist, self._id will raise TypeError
-    except TypeError:
-        self._collection.insert_one(self._filter_query)
+class Employee:
+    def __init__(self, _id):
+        self._filter_query = {"id": _id}
+        self._collection = collection
+        self.collection = EmployeeCollection(_id)
+
+        # Create a new document if it doesn't exist
+        if self.collection.get() is None:
+            self._collection.insert_one(self._filter_query)
+    
+    def someOtherOperation(self):
+        self.collection.hello = "Hello World"  
 
 ```
 
 Now, save the above code in a file named `employee.py` and run the following command in the same directory:
 
 ```
 $ python3 -i employee.py
@@ -61,26 +70,26 @@
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 ```
 
-This can be accessed by creating an instance of `Employee` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
+This can be accessed by creating an instance of `EmployeeClass` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, it will create a new document with the given `id`.
 
 For example:
 
 ```
->>> e = Employee(4051)
+>>> e = EmployeeCollection(4051)
 ```
 
-Now this `e` object is an instance of `Employee` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
+Now this `e` object is an instance of `EmployeeCollection` class, which is a subclass of `MongoGetterSetter` metaclass. This object is a wrapper around the MongoDB document, which is fetched from the MongoDB collection using the `self._filter_query` from the `self._collection` attribute. You can access the MongoDB document and do CURD essential operations just by accessing this object's attributes/indexes. For the available methods, see the `MongoDataWrapper` and `MongoDictWrapper` methods. For example:
 
 ```
->>> e = Employee(4051)
+>>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
 >>> e.id.get()
 4051
 >>> e.name
@@ -182,15 +191,15 @@
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
 
     Example:
     ```
-    obj = Employee(_id)
+    obj = EmployeeClass(_id)
     result = obj.some_key
     ```
 - `__getitem__(self, key, value)`: Gets the value of the specified `key` from the MongoDB document.
 
     Example:
 
     ```
@@ -394,43 +403,48 @@
                 "status": "in progress"
             }
         ]
     }
 ]
 ```
 
-Now, let's create a class called `People` with `MongoGetterSetter` as its metaclass.
+Now, let's create a class called `People` and `PeopleCollection` with `MongoGetterSetter` as its metaclass.
 
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
 # Connect to the MongoDB database and collection
 client = MongoClient("mongodb://localhost:27017/")
 db = client["example_db"]
 people_collection = db["people"]
 
-class People(metaclass=MongoGetterSetter):
+# Wrapper for MongoDB Collection with metaclass, use this inside your actual class.
+class PeopleCollection(metaclass=MongoGetterSetter):
     def __init__(self, _id):
         self._filter_query = {"id": _id}  # or the ObjectID, at your convenience
         self._collection = people_collection  # Should be a pymongo.MongoClient[database].collection
 
-        try:
-            self._id # if the document doesn't exist, self._id will raise TypeError
-        except TypeError:
-            self._collection.insert_one({
-                "id": _id
-            })
+class People():
+    def __init__(self, _id):
+        self.collection = PeopleCollection(_id)
+        self._filter_query = {"id": _id}
+        self._collection = people_collection
+        if self.collection.get() is None:
+            self._collection.insert_one(self._filter_query)
+    
+    def someOtherOperation(self):
+        self.collection.hello = "Hello World"       
 ```
 
 
 
-Create a People object for Alice with `id = 1`
+Create a PeopleCollection object for Alice with `id = 1`
 ```
-alice = People(1)
+alice = PeopleCollection(1)
 ```
 
 Access and modify Alice's name
 ```
 print(alice.name)  # Output: 'Alice'
 alice.name = "Alice Johnson"
 print(alice.name)  # Output: 'Alice Johnson'
```

### Comparing `mongogettersetter-1.3.0/setup.py` & `mongogettersetter-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.3.0',
+    version='1.3.1',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

