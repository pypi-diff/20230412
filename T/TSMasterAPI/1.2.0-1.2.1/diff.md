# Comparing `tmp/TSMasterAPI-1.2.0.tar.gz` & `tmp/TSMasterAPI-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-1.2.0.tar", last modified: Wed Apr 12 03:59:44 2023, max compression
+gzip compressed data, was "TSMasterAPI-1.2.1.tar", last modified: Wed Apr 12 07:40:57 2023, max compression
```

## Comparing `TSMasterAPI-1.2.0.tar` & `TSMasterAPI-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 03:59:44.569959 TSMasterAPI-1.2.0/
--rw-rw-rw-   0        0        0     1024 2023-04-12 03:59:44.569959 TSMasterAPI-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 03:59:44.561445 TSMasterAPI-1.2.0/TSMasterAPI/
--rw-rw-rw-   0        0        0   152596 2023-04-12 02:44:50.000000 TSMasterAPI-1.2.0/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.0/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:59:44.568957 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 03:59:44.570957 TSMasterAPI-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-04-12 03:59:42.000000 TSMasterAPI-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:40:57.939405 TSMasterAPI-1.2.1/
+-rw-rw-rw-   0        0        0     1048 2023-04-12 07:40:57.928114 TSMasterAPI-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 07:40:57.917161 TSMasterAPI-1.2.1/TSMasterAPI/
+-rw-rw-rw-   0        0        0   151849 2023-04-12 07:38:26.000000 TSMasterAPI-1.2.1/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.1/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:40:57.926807 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1048 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 07:40:57.939405 TSMasterAPI-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-04-12 07:40:55.000000 TSMasterAPI-1.2.1/setup.py
```

### Comparing `TSMasterAPI-1.2.0/PKG-INFO` & `TSMasterAPI-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.0
+Version: 1.2.1
 Summary: Use TSMaster hardware
+Home-page: UNKNOWN
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
@@ -25,7 +26,9 @@
 This is the TSMaster python library
 
 Can only be used by WIN32 Python
 
 [联系作者](865762826@qq.com)
 
 to write your content.
+
+
```

### Comparing `TSMasterAPI-1.2.0/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-1.2.1/TSMasterAPI/TSMasterAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-06 16:36:32
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 10:23:45
+LastEditTime: 2023-04-12 15:38:26
 github:https://github.com/sy950915/TSMasterAPI.git
 ''' 
 from ctypes import *
 from enum import Enum
 import copy
 import os
 from sys import getsizeof
@@ -400,35 +400,15 @@
         datalen = len(data)
         if datalen>self.FActualPayloadLength:
             datalen = self.FActualPayloadLength
         for i in range(datalen):
             self.FData[i] = data[i]
 
 
-class TFlexRaySignal(Structure):
-    '''
-    获取信号在数据库中的定义 通过该结构体 可获取对报文中该信号值以及设置对应报文该信号值
-    相关函数：
-    tscom_flexray_get_signal_definition
-    tscom_flexray_set_signal_value_in_raw_frame
-    tscom_flexray_get_signal_value_in_raw_frame
-    函数使用示例可在Flexray_demo中找到
-    '''
-    _pack_ =1
-    _fields_ = [
-                ("FFRSgnType",c_uint8),
-                ("FCompuMethod",c_uint8),
-                ("FReserved",c_uint8),
-                ("FIsIntel",c_bool),
-                ("FStartBit",c_int32),
-                ("FUpdateBit",c_int32),
-                ("FLength",c_int32),
-                ("FFactor",c_double),
-                ("FOffset",c_double),
-                ]
+
 
 class TLibFlexray_controller_config(Structure):
     """
     Flexray controller config结构体
     作用:在配置flexray时,需要对硬件参数进行配置
     字段来源:数据库中可获取
     注:在使用该库时,可直接TSMaster加载工程,跳过复杂参数的配置
@@ -602,23 +582,14 @@
                 ("FDeviceIndex", c_int32),
                 ("FVendorName", c_char * 32),
                 ("FDeviceName", c_char * 32),
                 ("FSerialString", c_char * 64),
                 ]
     
 DATABASE_STR_LEN = 512    
-class TDBProperties(Structure):
-    _pack_ = 1
-    _fields_ = [("FCANSgnType", c_uint8),
-                ("FIsIntel", c_bool),
-                ("FStartBit", c_int32),
-                ("FLength", c_int32),
-                ("FFactor", c_double),
-                ("FOffset", c_double),
-                ]
 
 class TCANSignal(Structure):
     _pack_ = 1
     _fields_ = [("FCANSgnType", c_uint8),
                 ("FIsIntel", c_bool),
                 ("FStartBit", c_int32),
                 ("FLength", c_int32),
@@ -633,25 +604,34 @@
                 ("FStartBit", c_int32),
                 ("FLength", c_int32),
                 ("FFactor", c_double),
                 ("FOffset", c_double),
                 ]
     
 class TFlexRaySignal(Structure):
-    _pack_ = 1
-    _fields_ = [("FCANSgnType", c_uint8),
-                ("FCompuMethod", c_uint8),
-                ("FReserved", c_uint8),
-                ("FIsIntel", c_bool),
-                ("FStartBit", c_int32),
-                ("FUpdateBit", c_int32),
-                ("FLength", c_int32),
-                ("FFactor", c_double),
-                ("FOffset", c_double),
-                ]  
+    '''
+    获取信号在数据库中的定义 通过该结构体 可获取对报文中该信号值以及设置对应报文该信号值
+    相关函数：
+    tscom_flexray_get_signal_definition
+    tscom_flexray_set_signal_value_in_raw_frame
+    tscom_flexray_get_signal_value_in_raw_frame
+    函数使用示例可在Flexray_demo中找到
+    '''
+    _pack_ =1
+    _fields_ = [
+                ("FFRSgnType",c_uint8),
+                ("FCompuMethod",c_uint8),
+                ("FReserved",c_uint8),
+                ("FIsIntel",c_bool),
+                ("FStartBit",c_int32),
+                ("FUpdateBit",c_int32),
+                ("FLength",c_int32),
+                ("FFactor",c_double),
+                ("FOffset",c_double),
+                ] 
 class TDBProperties(Structure):
     _pack_ = 1
     _fields_ = [("FDBIndex", c_int32),
                 ("FSignalCount", c_int32),
                 ("FFrameCount", c_int32),
                 ("FECUCount", c_int32),
                 ("FSupportedChannelMask", c_uint64),
```

### Comparing `TSMasterAPI-1.2.0/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-1.2.1/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.0
+Version: 1.2.1
 Summary: Use TSMaster hardware
+Home-page: UNKNOWN
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
@@ -25,7 +26,9 @@
 This is the TSMaster python library
 
 Can only be used by WIN32 Python
 
 [联系作者](865762826@qq.com)
 
 to write your content.
+
+
```

### Comparing `TSMasterAPI-1.2.0/license.txt` & `TSMasterAPI-1.2.1/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-1.2.0/setup.py` & `TSMasterAPI-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 11:59:42
+LastEditTime: 2023-04-12 15:40:45
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='1.2.0',  # 版本号
+      version='1.2.1',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

