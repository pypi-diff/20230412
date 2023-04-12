# Comparing `tmp/data_collect-0.8.1.tar.gz` & `tmp/data_collect-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_collect-0.8.1.tar", last modified: Thu Apr  6 11:21:57 2023, max compression
+gzip compressed data, was "data_collect-0.8.2.tar", last modified: Wed Apr 12 16:36:19 2023, max compression
```

## Comparing `data_collect-0.8.1.tar` & `data_collect-0.8.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-06 11:21:57.704063 data_collect-0.8.1/
--rw-r--r--   0 jojo       (501) staff       (20)      597 2023-04-06 11:21:57.704134 data_collect-0.8.1/PKG-INFO
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-06 11:21:57.702280 data_collect-0.8.1/data_collect/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-03-23 09:10:26.000000 data_collect-0.8.1/data_collect/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    12198 2023-04-06 11:20:37.000000 data_collect-0.8.1/data_collect/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-03 06:37:00.000000 data_collect-0.8.1/data_collect/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      283 2023-03-23 09:10:26.000000 data_collect-0.8.1/data_collect/correlation_id.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-06 11:21:57.703910 data_collect-0.8.1/data_collect/data_types/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-03-23 09:10:26.000000 data_collect-0.8.1/data_collect/data_types/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      544 2023-03-23 09:10:26.000000 data_collect-0.8.1/data_collect/data_types/blob.py
--rw-r--r--   0 jojo       (501) staff       (20)     3316 2023-03-29 14:36:52.000000 data_collect-0.8.1/data_collect/data_types/image.py
--rw-r--r--   0 jojo       (501) staff       (20)      394 2023-03-23 09:10:26.000000 data_collect-0.8.1/data_collect/data_types/text.py
--rw-r--r--   0 jojo       (501) staff       (20)     5286 2023-04-06 11:18:52.000000 data_collect-0.8.1/data_collect/logger.py
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-03-28 12:28:58.000000 data_collect-0.8.1/data_collect/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-03-23 09:10:26.000000 data_collect-0.8.1/data_collect/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-06 11:21:57.703196 data_collect-0.8.1/data_collect.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      597 2023-04-06 11:21:57.000000 data_collect-0.8.1/data_collect.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      537 2023-04-06 11:21:57.000000 data_collect-0.8.1/data_collect.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-06 11:21:57.000000 data_collect-0.8.1/data_collect.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-06 11:21:57.000000 data_collect-0.8.1/data_collect.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       75 2023-04-06 11:21:57.000000 data_collect-0.8.1/data_collect.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       13 2023-04-06 11:21:57.000000 data_collect-0.8.1/data_collect.egg-info/top_level.txt
--rw-r--r--   0 jojo       (501) staff       (20)      782 2023-04-06 11:21:57.704551 data_collect-0.8.1/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-06 11:21:57.000000 data_collect-0.8.1/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.617018 data_collect-0.8.2/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-04-12 16:36:19.617104 data_collect-0.8.2/PKG-INFO
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.615233 data_collect-0.8.2/data_collect/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)    12320 2023-04-12 15:33:55.000000 data_collect-0.8.2/data_collect/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/correlation_id.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.616886 data_collect-0.8.2/data_collect/data_types/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/data_types/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      544 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/data_types/blob.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3438 2023-04-12 16:26:19.000000 data_collect-0.8.2/data_collect/data_types/image.py
+-rw-r--r--   0 jojo       (501) staff       (20)      394 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/data_types/text.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7470 2023-04-12 16:30:39.000000 data_collect-0.8.2/data_collect/logger.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-04-12 16:33:14.000000 data_collect-0.8.2/data_collect/queue.py
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.2/data_collect/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-04-12 16:34:49.000000 data_collect-0.8.2/data_collect/thread.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.2/data_collect/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:36:19.616268 data_collect-0.8.2/data_collect.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      582 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       75 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       13 2023-04-12 16:36:19.000000 data_collect-0.8.2/data_collect.egg-info/top_level.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      720 2023-04-12 16:36:19.617562 data_collect-0.8.2/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 16:36:19.000000 data_collect-0.8.2/setup.py
```

### Comparing `data_collect-0.8.1/PKG-INFO` & `data_collect-0.8.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: data_collect
-Version: 0.8.1
+Version: 0.8.2
 Summary: project descriptions here
-Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/themis/windmill-endpoint/tree/master
+Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
-Author-email: zhoubohan@baidu.com
+Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `data_collect-0.8.1/data_collect/client.py` & `data_collect-0.8.2/data_collect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,8 +303,13 @@
         content_type = metadata.get("content_type", "application/octet-stream") \
             if metadata is not None else "application/octet-stream"
         ext = mimetypes.guess_extension(content_type)
         extension = ext if ext is not None else "bin"
         file_name = correlation_id
         if metadata.get('sub_name'):
             file_name = f"{file_name}_{metadata.get('sub_name')}"
-        return f"{dir_name}/{file_name}.{extension}"
+        return f"{dir_name}/{file_name}{extension}"
+    
+    def close(self):
+        self._image_logger.close()
+        self._blob_logger.close()
+        self._logger.close()
```

### Comparing `data_collect-0.8.1/data_collect/constants.py` & `data_collect-0.8.2/data_collect/constants.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.1/data_collect/data_types/blob.py` & `data_collect-0.8.2/data_collect/data_types/blob.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.1/data_collect/data_types/image.py` & `data_collect-0.8.2/data_collect/data_types/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,22 +81,28 @@
     def _normalize_to_uint8(self):
         # Based on: https://github.com/matplotlib/matplotlib/blob/06567e021f21be046b6d6dcf00380c1cb9adaf3c/lib
         # /matplotlib/image.py#L684
         is_int = np.issubdtype(self.data.dtype, np.integer)
         low = 0
         high = 255 if is_int else 1
         if self.data.min() < low or self.data.max() > high:
-            x = np.clip(self.data, low, high)
+            self.data = np.clip(self.data, low, high)
 
         # float or bool
         if not is_int:
             self.data = self.data * 255
 
         self.data = self.data.astype(np.uint8)
 
+    def is_bytes(self):
+        """
+        is bytes
+        """
+        return isinstance(self.data, bytes)
+    
     def is_p_mode(self):
         """
         is p mode
         """
         return PIL.Image.fromarray(self.data).mode == 'P'
 
     def is_pillow_image(self):
```

### Comparing `data_collect-0.8.1/data_collect/utils.py` & `data_collect-0.8.2/data_collect/utils.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.1/data_collect.egg-info/PKG-INFO` & `data_collect-0.8.2/data_collect.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: data-collect
-Version: 0.8.1
+Version: 0.8.2
 Summary: project descriptions here
-Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/themis/windmill-endpoint/tree/master
+Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
-Author-email: zhoubohan@baidu.com
+Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `data_collect-0.8.1/data_collect.egg-info/SOURCES.txt` & `data_collect-0.8.2/data_collect.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 setup.cfg
 setup.py
 data_collect/__init__.py
 data_collect/client.py
 data_collect/constants.py
 data_collect/correlation_id.py
 data_collect/logger.py
+data_collect/queue.py
 data_collect/setup.py
+data_collect/thread.py
 data_collect/utils.py
 data_collect.egg-info/PKG-INFO
 data_collect.egg-info/SOURCES.txt
 data_collect.egg-info/dependency_links.txt
 data_collect.egg-info/not-zip-safe
 data_collect.egg-info/requires.txt
 data_collect.egg-info/top_level.txt
```

### Comparing `data_collect-0.8.1/setup.cfg` & `data_collect-0.8.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = data_collect
 author = zhoubohan
-author_email = zhoubohan@baidu.com
-version = 0.8.1
+author_email = zhoubohan.pro@gmail.com
+version = 0.8.2
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
-home_page = https://console.cloud.baidu-int.com/devops/icode/repos/baidu/themis/windmill-endpoint/tree/master
+home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

