# Comparing `tmp/data_collect-0.8.2.tar.gz` & `tmp/data_collect-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_collect-0.8.2.tar", last modified: Wed Apr 12 16:36:19 2023, max compression
+gzip compressed data, was "data_collect-0.8.3.tar", last modified: Wed Apr 12 16:43:36 2023, max compression
```

## Comparing `data_collect-0.8.2.tar` & `data_collect-0.8.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.617018 data_collect-0.8.2/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-04-12 16:36:19.617104 data_collect-0.8.2/PKG-INFO
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.615233 data_collect-0.8.2/data_collect/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    12320 2023-04-12 15:33:55.000000 data_collect-0.8.2/data_collect/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/correlation_id.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.616886 data_collect-0.8.2/data_collect/data_types/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/data_types/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      544 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/data_types/blob.py
--rw-r--r--   0 jojo       (501) staff       (20)     3438 2023-04-12 16:26:19.000000 data_collect-0.8.2/data_collect/data_types/image.py
--rw-r--r--   0 jojo       (501) staff       (20)      394 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/data_types/text.py
--rw-r--r--   0 jojo       (501) staff       (20)     7470 2023-04-12 16:30:39.000000 data_collect-0.8.2/data_collect/logger.py
--rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-04-12 16:33:14.000000 data_collect-0.8.2/data_collect/queue.py
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.2/data_collect/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-04-12 16:34:49.000000 data_collect-0.8.2/data_collect/thread.py
--rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.616268 data_collect-0.8.2/data_collect.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      582 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       75 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       13 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/top_level.txt
--rw-r--r--   0 jojo       (501) staff       (20)      720 2023-04-12 16:36:19.617562 data_collect-0.8.2/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 16:36:19.000000 data_collect-0.8.2/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:43:36.410892 data_collect-0.8.3/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-04-12 16:43:36.410974 data_collect-0.8.3/PKG-INFO
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:43:36.409069 data_collect-0.8.3/data_collect/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.3/data_collect/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)    12291 2023-04-12 16:43:21.000000 data_collect-0.8.3/data_collect/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.3/data_collect/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.3/data_collect/correlation_id.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:43:36.410752 data_collect-0.8.3/data_collect/data_types/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.3/data_collect/data_types/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      544 2023-04-11 15:51:48.000000 data_collect-0.8.3/data_collect/data_types/blob.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3438 2023-04-12 16:26:19.000000 data_collect-0.8.3/data_collect/data_types/image.py
+-rw-r--r--   0 jojo       (501) staff       (20)      394 2023-04-11 15:51:48.000000 data_collect-0.8.3/data_collect/data_types/text.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7470 2023-04-12 16:30:39.000000 data_collect-0.8.3/data_collect/logger.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-04-12 16:33:14.000000 data_collect-0.8.3/data_collect/queue.py
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.3/data_collect/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-04-12 16:34:49.000000 data_collect-0.8.3/data_collect/thread.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.3/data_collect/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:43:36.410091 data_collect-0.8.3/data_collect.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-04-12 16:43:36.000000 data_collect-0.8.3/data_collect.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      582 2023-04-12 16:43:36.000000 data_collect-0.8.3/data_collect.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:43:36.000000 data_collect-0.8.3/data_collect.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:43:36.000000 data_collect-0.8.3/data_collect.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       75 2023-04-12 16:43:36.000000 data_collect-0.8.3/data_collect.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       13 2023-04-12 16:43:36.000000 data_collect-0.8.3/data_collect.egg-info/top_level.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      720 2023-04-12 16:43:36.411408 data_collect-0.8.3/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 16:43:35.000000 data_collect-0.8.3/setup.py
```

### Comparing `data_collect-0.8.2/PKG-INFO` & `data_collect-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_collect
-Version: 0.8.2
+Version: 0.8.3
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.2/data_collect/client.py` & `data_collect-0.8.3/data_collect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,9 +307,8 @@
         file_name = correlation_id
         if metadata.get('sub_name'):
             file_name = f"{file_name}_{metadata.get('sub_name')}"
         return f"{dir_name}/{file_name}{extension}"
     
     def close(self):
         self._image_logger.close()
-        self._blob_logger.close()
-        self._logger.close()
+        self._blob_logger.close()
```

### Comparing `data_collect-0.8.2/data_collect/constants.py` & `data_collect-0.8.3/data_collect/constants.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/data_collect/data_types/blob.py` & `data_collect-0.8.3/data_collect/data_types/blob.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/data_collect/data_types/image.py` & `data_collect-0.8.3/data_collect/data_types/image.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/data_collect/logger.py` & `data_collect-0.8.3/data_collect/logger.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/data_collect/queue.py` & `data_collect-0.8.3/data_collect/queue.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/data_collect/thread.py` & `data_collect-0.8.3/data_collect/thread.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/data_collect/utils.py` & `data_collect-0.8.3/data_collect/utils.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/data_collect.egg-info/PKG-INFO` & `data_collect-0.8.3/data_collect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-collect
-Version: 0.8.2
+Version: 0.8.3
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.2/data_collect.egg-info/SOURCES.txt` & `data_collect-0.8.3/data_collect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.2/setup.cfg` & `data_collect-0.8.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = data_collect
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.8.2
+version = 0.8.3
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

