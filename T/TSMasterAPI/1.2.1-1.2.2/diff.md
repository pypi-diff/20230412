# Comparing `tmp/TSMasterAPI-1.2.1.tar.gz` & `tmp/TSMasterAPI-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-1.2.1.tar", last modified: Wed Apr 12 07:40:57 2023, max compression
+gzip compressed data, was "TSMasterAPI-1.2.2.tar", last modified: Wed Apr 12 08:18:27 2023, max compression
```

## Comparing `TSMasterAPI-1.2.1.tar` & `TSMasterAPI-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:40:57.939405 TSMasterAPI-1.2.1/
--rw-rw-rw-   0        0        0     1048 2023-04-12 07:40:57.928114 TSMasterAPI-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 07:40:57.917161 TSMasterAPI-1.2.1/TSMasterAPI/
--rw-rw-rw-   0        0        0   151849 2023-04-12 07:38:26.000000 TSMasterAPI-1.2.1/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.1/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:40:57.926807 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1048 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 07:40:57.000000 TSMasterAPI-1.2.1/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 07:40:57.939405 TSMasterAPI-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-04-12 07:40:55.000000 TSMasterAPI-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:18:27.706061 TSMasterAPI-1.2.2/
+-rw-rw-rw-   0        0        0     1024 2023-04-12 08:18:27.706061 TSMasterAPI-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 08:18:27.691775 TSMasterAPI-1.2.2/TSMasterAPI/
+-rw-rw-rw-   0        0        0   151846 2023-04-12 08:18:03.000000 TSMasterAPI-1.2.2/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.2/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:18:27.705009 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 08:18:27.000000 TSMasterAPI-1.2.2/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 08:18:27.706061 TSMasterAPI-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-04-12 08:18:17.000000 TSMasterAPI-1.2.2/setup.py
```

### Comparing `TSMasterAPI-1.2.1/PKG-INFO` & `TSMasterAPI-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.1
+Version: 1.2.2
 Summary: Use TSMaster hardware
-Home-page: UNKNOWN
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
@@ -26,9 +25,7 @@
 This is the TSMaster python library
 
 Can only be used by WIN32 Python
 
 [联系作者](865762826@qq.com)
 
 to write your content.
-
-
```

### Comparing `TSMasterAPI-1.2.1/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-1.2.2/TSMasterAPI/TSMasterAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-06 16:36:32
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 15:38:26
+LastEditTime: 2023-04-12 16:17:50
 github:https://github.com/sy950915/TSMasterAPI.git
 ''' 
 from ctypes import *
 from enum import Enum
 import copy
 import os
 from sys import getsizeof
@@ -2816,27 +2816,27 @@
         except:
             AComment = ''
         return ADBIndex,AFrameCount,ASignalCount,AECUCount,ASupportedChannelMask,string_at(AName).decode('utf8'),AComment
     print(tsapp_get_error_description(ret))
     return AECUCount,AFrameCount,ASignalCount,ASupportedChannelMask,string_at(AName),AComment     
 
 # 通过索引获取数据库属性信息
-def tsdb_get_flexray_db_properties_by_indexx_verbose(ADBIndex:c_int32):
+def tsdb_get_flexray_db_properties_by_index_verbose(ADBIndex:c_int32):
     '''
     db_msg =  app.db_get_flexray_database_properties_by_address(0)
     print(db_msg)
     '''
     AFrameCount = c_int32(0)
     ASignalCount = c_int32(0)
     AECUCount = c_int32(0)
     ASupportedChannelMask = c_int64(0)
     AName = POINTER(POINTER(c_char))()
     AComment = POINTER(POINTER(c_char))()
 
-    ret = dll.tsdb_get_flexray_db_properties_by_indexx_verbose(ADBIndex,byref(ASignalCount),byref(AFrameCount),byref(AECUCount),byref(ASupportedChannelMask),byref(AName),byref(AComment))
+    ret = dll.tsdb_get_flexray_db_properties_by_index_verbose(ADBIndex,byref(ASignalCount),byref(AFrameCount),byref(AECUCount),byref(ASupportedChannelMask),byref(AName),byref(AComment))
 
     if ret ==0:
         try:
             AComment = string_at(AComment).decode('utf8')
         except:
             AComment = ''
         return AECUCount,AFrameCount,ASignalCount,ASupportedChannelMask,string_at(AName),AComment
@@ -4025,15 +4025,15 @@
     example:
         db_ecu_frame_signal = TDBSignalProperties()
         tsdb_get_lin_db_signal_properties_by_frame_index(0,0,0,db_ecu_frame_signal)
     """
     return dll.tsdb_get_lin_db_signal_properties_by_frame_index(AIdxDB,Frameidx,AIndex,byref(Avalue))
 # def flexray_db_parse(index):
 #     ecu_list = {}
-#     ecuCount, fmeCount, sgnCount, supportedChannelMask, sName, sComment = tsdb_get_flexray_db_properties_by_indexx_verbose(index)
+#     ecuCount, fmeCount, sgnCount, supportedChannelMask, sName, sComment = tsdb_get_flexray_db_properties_by_index_verbose(index)
 #     for idxECU in range(ecuCount.value):
 #         message_list = []
 #         ATxFrameCount, ARxFrameCount, ecuName, sComment = tsdb_get_flexray_ecu_properties_by_index_verbose(index, idxECU)
 #         # print("ECUName = ",ecuName)
 #         for idxFme in range(ATxFrameCount.value):
 #             chnMask, baseCycle, cycleRep, isStartup, slotId, cycleMask, sgnCount, AFRDLC,sName, sComment= ret = tsdb_get_flexray_frame_properties_by_index_verbose(index, idxECU, idxFme, True)
 #             # print('Tx Frame', sName, ', comment:', sComment, ', base cycle:', baseCycle, ', cycle repetition:', cycleRep, ', slot Id:', slotId, ', cycle mask:', hex(cycleMask.value), ', signal count:', sgnCount)
```

### Comparing `TSMasterAPI-1.2.1/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-1.2.2/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.2.1
+Version: 1.2.2
 Summary: Use TSMaster hardware
-Home-page: UNKNOWN
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
@@ -26,9 +25,7 @@
 This is the TSMaster python library
 
 Can only be used by WIN32 Python
 
 [联系作者](865762826@qq.com)
 
 to write your content.
-
-
```

### Comparing `TSMasterAPI-1.2.1/license.txt` & `TSMasterAPI-1.2.2/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-1.2.1/setup.py` & `TSMasterAPI-1.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-04-12 15:40:45
+LastEditTime: 2023-04-12 16:18:17
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='1.2.1',  # 版本号
+      version='1.2.2',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

