# Comparing `tmp/TSMasterAPI-1.2.2.tar.gz` & `tmp/TSMasterAPI-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-1.2.2.tar", last modified: Wed Apr 12 08:18:27 2023, max compression
+gzip compressed data, was "TSMasterAPI-1.2.3.tar", last modified: Wed Apr 12 10:00:57 2023, max compression
```

## Comparing `TSMasterAPI-1.2.2.tar` & `TSMasterAPI-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 08:18:27.706061 TSMasterAPI-1.2.2/
--rw-rw-rw-   0        0        0     1024 2023-04-12 08:18:27.706061 TSMasterAPI-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 08:18:27.691775 TSMasterAPI-1.2.2/TSMasterAPI/
--rw-rw-rw-   0        0        0   151846 2023-04-12 08:18:03.000000 TSMasterAPI-1.2.2/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.2/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:18:27.705009 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 08:18:27.706061 TSMasterAPI-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-04-12 08:18:17.000000 TSMasterAPI-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:00:57.062585 TSMasterAPI-1.2.3/
+-rw-rw-rw-   0        0        0     1024 2023-04-12 10:00:57.055643 TSMasterAPI-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 10:00:57.046611 TSMasterAPI-1.2.3/TSMasterAPI/
+-rw-rw-rw-   0        0        0   151843 2023-04-12 09:54:48.000000 TSMasterAPI-1.2.3/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.3/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:00:57.054138 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-04-12 10:00:56.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-12 10:00:57.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:00:56.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 10:00:56.000000 TSMasterAPI-1.2.3/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.3/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:00:57.063087 TSMasterAPI-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-04-12 10:00:55.000000 TSMasterAPI-1.2.3/setup.py
```

### Comparing `TSMasterAPI-1.2.2/PKG-INFO` & `TSMasterAPI-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.2
+Version: 1.2.3
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-1.2.2/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-1.2.3/TSMasterAPI/TSMasterAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-06 16:36:32
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 16:17:50
+LastEditTime: 2023-04-12 17:52:14
 github:https://github.com/sy950915/TSMasterAPI.git
 ''' 
 from ctypes import *
 from enum import Enum
 import copy
 import os
 from sys import getsizeof
@@ -3816,15 +3816,15 @@
 # lin db info
 def tsdb_load_lin_db(AFliepath:str,ASupportedChannels:str,AId:c_int32):
     """
     AId = c_int32(0)
     tsdb_load_lin_db(b"C:/1.xml",b'0,1',AId)
     """
     if not isinstance(AFliepath,bytes):
-        AFliepat数h = bytes(AFliepath)
+        AFliepath = bytes(AFliepath)
     if not isinstance(ASupportedChannels,bytes):
         ASupportedChannels = bytes(ASupportedChannels)
     ret = dll.tsdb_load_lin_db(AFliepath,ASupportedChannels,byref(AId))
     return ret
 
 # 卸载数据库
 def tsdb_unload_lin_db(AId:c_int32):
```

### Comparing `TSMasterAPI-1.2.2/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-1.2.3/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.2
+Version: 1.2.3
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-1.2.2/license.txt` & `TSMasterAPI-1.2.3/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-1.2.2/setup.py` & `TSMasterAPI-1.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 16:18:17
+LastEditTime: 2023-04-12 18:00:55
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='1.2.2',  # 版本号
+      version='1.2.3',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

