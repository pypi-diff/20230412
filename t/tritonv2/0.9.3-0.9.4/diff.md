# Comparing `tmp/tritonv2-0.9.3.tar.gz` & `tmp/tritonv2-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritonv2-0.9.3.tar", last modified: Sun Apr  9 16:31:38 2023, max compression
+gzip compressed data, was "tritonv2-0.9.4.tar", last modified: Wed Apr 12 16:38:26 2023, max compression
```

## Comparing `tritonv2-0.9.3.tar` & `tritonv2-0.9.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-09 16:31:38.884566 tritonv2-0.9.3/
--rw-r--r--   0 jojo       (501) staff       (20)     2468 2023-04-09 16:31:38.884651 tritonv2-0.9.3/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1882 2023-04-09 16:31:38.000000 tritonv2-0.9.3/README.md
--rw-r--r--   0 jojo       (501) staff       (20)      767 2023-04-09 16:31:38.885080 tritonv2-0.9.3/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-09 16:31:38.000000 tritonv2-0.9.3/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-09 16:31:38.883486 tritonv2-0.9.3/tritonv2/
--rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      332 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     5923 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/client_factory.py
--rw-r--r--   0 jojo       (501) staff       (20)      653 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)    16365 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/grpc_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    13778 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/grpc_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    19189 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/http_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    18307 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/http_client.py
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-04-09 08:19:04.000000 tritonv2-0.9.3/tritonv2/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-09 16:31:38.884413 tritonv2-0.9.3/tritonv2.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)     2468 2023-04-09 16:31:38.000000 tritonv2-0.9.3/tritonv2.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      470 2023-04-09 16:31:38.000000 tritonv2-0.9.3/tritonv2.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-09 16:31:38.000000 tritonv2-0.9.3/tritonv2.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-09 16:31:38.000000 tritonv2-0.9.3/tritonv2.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       65 2023-04-09 16:31:38.000000 tritonv2-0.9.3/tritonv2.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        9 2023-04-09 16:31:38.000000 tritonv2-0.9.3/tritonv2.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:38:26.794211 tritonv2-0.9.4/
+-rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-04-12 16:38:26.794298 tritonv2-0.9.4/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1882 2023-04-12 16:38:26.000000 tritonv2-0.9.4/README.md
+-rw-r--r--   0 jojo       (501) staff       (20)      713 2023-04-12 16:38:26.794707 tritonv2-0.9.4/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 16:38:26.000000 tritonv2-0.9.4/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:38:26.793222 tritonv2-0.9.4/tritonv2/
+-rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      332 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5923 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/client_factory.py
+-rw-r--r--   0 jojo       (501) staff       (20)      653 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)    16365 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/grpc_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    13778 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/grpc_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    19189 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/http_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    18307 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/http_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:38:26.794066 tritonv2-0.9.4/tritonv2.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      470 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       73 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        9 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/top_level.txt
```

### Comparing `tritonv2-0.9.3/PKG-INFO` & `tritonv2-0.9.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.3
+Version: 0.9.4
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
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.3
+pip install tritonv2==0.9.4
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.3/README.md` & `tritonv2-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.3
+pip install tritonv2==0.9.4
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.3/setup.cfg` & `tritonv2-0.9.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [metadata]
 name = tritonv2
 author = zhoubohan
-author_email = zhoubohan@baidu.com
-version = 0.9.3
+author_email = zhoubohan.pro@gmail.com
+version = 0.9.4
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
 
 [options]
 packages = find:
 install_requires = 
-	numpy
+	numpy>=1.23.5
 	tenacity>=8.1.0
 	tritonclient[all]>=2.25.0
 	pydantic>=1.10.2
 python_requires = >=3.7
 include_package_data = True
 zip_safe = False
```

### Comparing `tritonv2-0.9.3/tritonv2/client_factory.py` & `tritonv2-0.9.4/tritonv2/client_factory.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.3/tritonv2/constants.py` & `tritonv2-0.9.4/tritonv2/constants.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.3/tritonv2/grpc_aio_client.py` & `tritonv2-0.9.4/tritonv2/grpc_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.3/tritonv2/grpc_client.py` & `tritonv2-0.9.4/tritonv2/grpc_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.3/tritonv2/http_aio_client.py` & `tritonv2-0.9.4/tritonv2/http_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.3/tritonv2/http_client.py` & `tritonv2-0.9.4/tritonv2/http_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.3/tritonv2/utils.py` & `tritonv2-0.9.4/tritonv2/utils.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.3/tritonv2.egg-info/PKG-INFO` & `tritonv2-0.9.4/tritonv2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.3
+Version: 0.9.4
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
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.3
+pip install tritonv2==0.9.4
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

