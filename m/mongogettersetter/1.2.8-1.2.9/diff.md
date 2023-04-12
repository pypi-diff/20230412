# Comparing `tmp/mongogettersetter-1.2.8.tar.gz` & `tmp/mongogettersetter-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.2.8.tar", last modified: Tue Mar 28 19:13:52 2023, max compression
+gzip compressed data, was "mongogettersetter-1.2.9.tar", last modified: Wed Apr 12 10:53:43 2023, max compression
```

## Comparing `mongogettersetter-1.2.8.tar` & `mongogettersetter-1.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-03-28 19:13:52.083770 mongogettersetter-1.2.8/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28884 2023-03-28 19:13:52.083770 mongogettersetter-1.2.8/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28287 2023-03-28 19:08:59.000000 mongogettersetter-1.2.8/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-03-28 19:13:52.083770 mongogettersetter-1.2.8/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24192 2023-03-28 19:13:22.000000 mongogettersetter-1.2.8/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-03-28 19:13:52.083770 mongogettersetter-1.2.8/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28884 2023-03-28 19:13:52.000000 mongogettersetter-1.2.8/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-03-28 19:13:52.000000 mongogettersetter-1.2.8/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-03-28 19:13:52.000000 mongogettersetter-1.2.8/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-03-28 19:13:52.000000 mongogettersetter-1.2.8/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-03-28 19:13:52.000000 mongogettersetter-1.2.8/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-03-28 19:13:52.083770 mongogettersetter-1.2.8/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-03-28 19:13:29.000000 mongogettersetter-1.2.8/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 10:53:43.167938 mongogettersetter-1.2.9/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28851 2023-04-12 10:53:43.167938 mongogettersetter-1.2.9/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28254 2023-04-12 10:51:51.000000 mongogettersetter-1.2.9/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 10:53:43.163938 mongogettersetter-1.2.9/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24177 2023-03-29 06:06:12.000000 mongogettersetter-1.2.9/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 10:53:43.163938 mongogettersetter-1.2.9/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    28851 2023-04-12 10:53:42.000000 mongogettersetter-1.2.9/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-04-12 10:53:42.000000 mongogettersetter-1.2.9/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-04-12 10:53:42.000000 mongogettersetter-1.2.9/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-04-12 10:53:42.000000 mongogettersetter-1.2.9/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-04-12 10:53:42.000000 mongogettersetter-1.2.9/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-04-12 10:53:43.167938 mongogettersetter-1.2.9/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-04-12 10:53:18.000000 mongogettersetter-1.2.9/setup.py
```

### Comparing `mongogettersetter-1.2.8/PKG-INFO` & `mongogettersetter-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.2.8
+Version: 1.2.9
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -44,15 +44,15 @@
     def __init__(self, _id):
     self._filter_query = {"id": _id} # or the ObjectID, at your convinence
     self._collection = collection # Should be a pymongo.MongoClient[database].collection
 
     # if the document doesn't exist, we could create it here
     try:
         self._id # if the document doesn't exist, self._id will raise Attribute Error
-    except AttributeError or KeyError:
+    except TypeError:
         self._collection.insert_one(self._filter_query)
 
 ```
 
 Now, save the above code in a file named `employee.py` and run the following command in the same directory:
 
 ```
@@ -344,14 +344,15 @@
 - `clear(self)`: Overrides the base `dict` method to remove all key-value pairs from the MongoDB document.
 
 - `__len__(self)`: Overrides the base `dict` method to return the number of key-value pairs in the MongoDB document.
 
 - `__str__(self)`: Overrides the base `dict` method to return a string representation of the MongoDB document.
 
 - `__repr__(self)`: Overrides the base `dict` method to return a string representation of the MongoDB document.
+
 ## Examples
 
 To provide a more detailed example, let's assume you have a MongoDB collection named `people` with the following documents:
 
 ```
 [
     {
@@ -411,15 +412,15 @@
 class People(metaclass=MongoGetterSetter):
     def __init__(self, _id):
         self._filter_query = {"id": _id}  # or the ObjectID, at your convenience
         self._collection = people_collection  # Should be a pymongo.MongoClient[database].collection
 
         try:
             self._id # if the document doesn't exist, self._id will raise Attribute Error
-        except AttributeError or KeyError:
+        except TypeError:
             self._collection.insert_one({
                 "id": _id
             })
 ```
```

### Comparing `mongogettersetter-1.2.8/README.md` & `mongogettersetter-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(self, _id):
     self._filter_query = {"id": _id} # or the ObjectID, at your convinence
     self._collection = collection # Should be a pymongo.MongoClient[database].collection
 
     # if the document doesn't exist, we could create it here
     try:
         self._id # if the document doesn't exist, self._id will raise Attribute Error
-    except AttributeError or KeyError:
+    except TypeError:
         self._collection.insert_one(self._filter_query)
 
 ```
 
 Now, save the above code in a file named `employee.py` and run the following command in the same directory:
 
 ```
@@ -328,14 +328,15 @@
 - `clear(self)`: Overrides the base `dict` method to remove all key-value pairs from the MongoDB document.
 
 - `__len__(self)`: Overrides the base `dict` method to return the number of key-value pairs in the MongoDB document.
 
 - `__str__(self)`: Overrides the base `dict` method to return a string representation of the MongoDB document.
 
 - `__repr__(self)`: Overrides the base `dict` method to return a string representation of the MongoDB document.
+
 ## Examples
 
 To provide a more detailed example, let's assume you have a MongoDB collection named `people` with the following documents:
 
 ```
 [
     {
@@ -395,15 +396,15 @@
 class People(metaclass=MongoGetterSetter):
     def __init__(self, _id):
         self._filter_query = {"id": _id}  # or the ObjectID, at your convenience
         self._collection = people_collection  # Should be a pymongo.MongoClient[database].collection
 
         try:
             self._id # if the document doesn't exist, self._id will raise Attribute Error
-        except AttributeError or KeyError:
+        except TypeError:
             self._collection.insert_one({
                 "id": _id
             })
 ```
```

### Comparing `mongogettersetter-1.2.8/mongogettersetter/__init__.py` & `mongogettersetter-1.2.9/mongogettersetter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # import sys
 import json
-import inspect
 
 # sys.(64)setrecursionlimit
 
 
 class MongoDictWrapper(dict):
     """
     MongoDictWrapper is a wrapper around the dictionary object to provide the functionality of updating the database when the dictionary is updated. It is used to wrap the dictionary object in the MongoGetterSetter class. It is not meant to be used directly.
```

### Comparing `mongogettersetter-1.2.8/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.2.9/mongogettersetter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.2.8
+Version: 1.2.9
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -44,15 +44,15 @@
     def __init__(self, _id):
     self._filter_query = {"id": _id} # or the ObjectID, at your convinence
     self._collection = collection # Should be a pymongo.MongoClient[database].collection
 
     # if the document doesn't exist, we could create it here
     try:
         self._id # if the document doesn't exist, self._id will raise Attribute Error
-    except AttributeError or KeyError:
+    except TypeError:
         self._collection.insert_one(self._filter_query)
 
 ```
 
 Now, save the above code in a file named `employee.py` and run the following command in the same directory:
 
 ```
@@ -344,14 +344,15 @@
 - `clear(self)`: Overrides the base `dict` method to remove all key-value pairs from the MongoDB document.
 
 - `__len__(self)`: Overrides the base `dict` method to return the number of key-value pairs in the MongoDB document.
 
 - `__str__(self)`: Overrides the base `dict` method to return a string representation of the MongoDB document.
 
 - `__repr__(self)`: Overrides the base `dict` method to return a string representation of the MongoDB document.
+
 ## Examples
 
 To provide a more detailed example, let's assume you have a MongoDB collection named `people` with the following documents:
 
 ```
 [
     {
@@ -411,15 +412,15 @@
 class People(metaclass=MongoGetterSetter):
     def __init__(self, _id):
         self._filter_query = {"id": _id}  # or the ObjectID, at your convenience
         self._collection = people_collection  # Should be a pymongo.MongoClient[database].collection
 
         try:
             self._id # if the document doesn't exist, self._id will raise Attribute Error
-        except AttributeError or KeyError:
+        except TypeError:
             self._collection.insert_one({
                 "id": _id
             })
 ```
```

### Comparing `mongogettersetter-1.2.8/setup.py` & `mongogettersetter-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.2.8',
+    version='1.2.9',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

