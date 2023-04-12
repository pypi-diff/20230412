# Comparing `tmp/TSMasterAPI-1.1.0.tar.gz` & `tmp/TSMasterAPI-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-1.1.0.tar", last modified: Mon Mar 27 03:57:20 2023, max compression
+gzip compressed data, was "TSMasterAPI-1.2.0.tar", last modified: Wed Apr 12 03:59:44 2023, max compression
```

## Comparing `TSMasterAPI-1.1.0.tar` & `TSMasterAPI-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 03:57:20.706848 TSMasterAPI-1.1.0/
--rw-rw-rw-   0        0        0     1024 2023-03-27 03:57:20.706848 TSMasterAPI-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-27 03:57:20.688771 TSMasterAPI-1.1.0/TSMasterAPI/
--rw-rw-rw-   0        0        0   130238 2023-03-27 03:56:08.000000 TSMasterAPI-1.1.0/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.1.0/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 03:57:20.705820 TSMasterAPI-1.1.0/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-03-27 03:57:20.000000 TSMasterAPI-1.1.0/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-03-27 03:57:20.000000 TSMasterAPI-1.1.0/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 03:57:20.000000 TSMasterAPI-1.1.0/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-03-27 03:57:20.000000 TSMasterAPI-1.1.0/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.1.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 03:57:20.706848 TSMasterAPI-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-03-27 03:56:30.000000 TSMasterAPI-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:59:44.569959 TSMasterAPI-1.2.0/
+-rw-rw-rw-   0        0        0     1024 2023-04-12 03:59:44.569959 TSMasterAPI-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 03:59:44.561445 TSMasterAPI-1.2.0/TSMasterAPI/
+-rw-rw-rw-   0        0        0   152596 2023-04-12 02:44:50.000000 TSMasterAPI-1.2.0/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0       26 2023-03-24 01:21:03.000000 TSMasterAPI-1.2.0/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:59:44.568957 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 03:59:44.000000 TSMasterAPI-1.2.0/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-1.2.0/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 03:59:44.570957 TSMasterAPI-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-04-12 03:59:42.000000 TSMasterAPI-1.2.0/setup.py
```

### Comparing `TSMasterAPI-1.1.0/PKG-INFO` & `TSMasterAPI-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.1.0
+Version: 1.2.0
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-1.1.0/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-1.2.0/TSMasterAPI/TSMasterAPI.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-06 16:36:32
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-03-27 11:54:01
+LastEditTime: 2023-04-12 10:23:45
 github:https://github.com/sy950915/TSMasterAPI.git
 ''' 
 from ctypes import *
 from enum import Enum
 import copy
 import os
 from sys import getsizeof
@@ -600,14 +600,131 @@
     _pack_ = 1
     _fields_ = [("FDeviceType", c_int32),
                 ("FDeviceIndex", c_int32),
                 ("FVendorName", c_char * 32),
                 ("FDeviceName", c_char * 32),
                 ("FSerialString", c_char * 64),
                 ]
+    
+DATABASE_STR_LEN = 512    
+class TDBProperties(Structure):
+    _pack_ = 1
+    _fields_ = [("FCANSgnType", c_uint8),
+                ("FIsIntel", c_bool),
+                ("FStartBit", c_int32),
+                ("FLength", c_int32),
+                ("FFactor", c_double),
+                ("FOffset", c_double),
+                ]
+
+class TCANSignal(Structure):
+    _pack_ = 1
+    _fields_ = [("FCANSgnType", c_uint8),
+                ("FIsIntel", c_bool),
+                ("FStartBit", c_int32),
+                ("FLength", c_int32),
+                ("FFactor", c_double),
+                ("FOffset", c_double),
+                ]
+    
+class TLINSignal(Structure):
+    _pack_ = 1
+    _fields_ = [("FLINSgnType", c_uint8),
+                ("FIsIntel", c_bool),
+                ("FStartBit", c_int32),
+                ("FLength", c_int32),
+                ("FFactor", c_double),
+                ("FOffset", c_double),
+                ]
+    
+class TFlexRaySignal(Structure):
+    _pack_ = 1
+    _fields_ = [("FCANSgnType", c_uint8),
+                ("FCompuMethod", c_uint8),
+                ("FReserved", c_uint8),
+                ("FIsIntel", c_bool),
+                ("FStartBit", c_int32),
+                ("FUpdateBit", c_int32),
+                ("FLength", c_int32),
+                ("FFactor", c_double),
+                ("FOffset", c_double),
+                ]  
+class TDBProperties(Structure):
+    _pack_ = 1
+    _fields_ = [("FDBIndex", c_int32),
+                ("FSignalCount", c_int32),
+                ("FFrameCount", c_int32),
+                ("FECUCount", c_int32),
+                ("FSupportedChannelMask", c_uint64),
+                ("FName", c_char * DATABASE_STR_LEN),
+                ("FComment", c_char * DATABASE_STR_LEN),
+                ]
+class TDBECUProperties(Structure):
+    _pack_ = 1
+    _fields_ = [("FDBIndex", c_int32),
+                ("FECUIndex", c_int32),
+                ("FTxFrameCount", c_int32),
+                ("FRxFrameCount", c_int32),
+                ("FName", c_char * DATABASE_STR_LEN),
+                ("FComment", c_char * DATABASE_STR_LEN),
+                ] 
+class TDBFrameProperties(Structure):
+    _pack_ = 1
+    _fields_ = [("FDBIndex", c_int32),
+                ("FECUIndex", c_int32),
+                ("FFrameIndex", c_int32),
+                ("FIsTx", c_uint8),
+                ("FReserved1", c_uint8),
+                ("FReserved2", c_uint8),
+                ("FReserved3", c_uint8),
+                ("FFrameType", c_int32),
+                # CAN
+                ("FCANIsDataFrame", c_uint8),
+                ("FCANIsStdFrame", c_uint8),
+                ("FCANIsEdl", c_uint8),
+                ("FCANIsBrs", c_uint8),
+                ("FCANIdentifier", c_int32),
+                ("FCANDLC", c_int32),
+                ("FCANDataBytes", c_int32),
+                #LIN
+                ("FLINIdentifier", c_int32),
+                ("FLINDLC", c_int32),
+                #FLEXRAY
+                ("FFRChannelMask", c_uint8),
+                ("FFRBaseCycle", c_uint8),
+                ("FFRCycleRepetition", c_uint8),
+                ("FFRIsStartupFrame", c_uint8),
+                ("FFRSlotId", c_uint16),
+                ("FFRDLC", c_uint16),
+                ("FFRCycleMask", c_uint64),
+                ("FSignalCount", c_int32),
+                ("FName", c_char * DATABASE_STR_LEN),
+                ("FComment", c_char * DATABASE_STR_LEN),
+                ] 
+class TDBSignalProperties(Structure):
+    _pack_ = 1
+    _fields_ = [("FDBIndex", c_int32),
+                ("FECUIndex", c_int32),
+                ("FFrameIndex", c_int32),
+                ("FSignalIndex", c_int32),
+                ("FIsTx", c_uint8),
+                ("FReserved1", c_uint8),
+                ("FReserved2", c_uint8),
+                ("FReserved3", c_uint8),
+                ("FSignalType", c_int32),
+                ("FCANSignal", TCANSignal),
+                ("FLINSignal", TLINSignal),
+                ("FFlexRaySignal", TFlexRaySignal),
+                ("FParentFrameId", c_int32),
+                ("FInitValue", c_double),
+                ("FName", c_char * DATABASE_STR_LEN),
+                ("FComment", c_char * DATABASE_STR_LEN),
+                ] 
+
+
 #回调函数
 PCANFD = POINTER(TLIBCANFD)
 OnTx_RxFUNC_CANFD = WINFUNCTYPE(None, POINTER(c_int32), PCANFD)
 
 PCAN = POINTER(TLIBCAN)
 OnTx_RxFUNC_CAN = WINFUNCTYPE(None, POINTER(c_int32), PCAN)
 
@@ -1854,54 +1971,15 @@
     """
     if isinstance(AValue,int) or isinstance(AValue,float):
         AValue = c_int32(AValue)
     r = dll.tsdb_set_signal_value_canfd(byref(ACANFD), AMsgName, ASgnName, AValue)
     return r
 
 
-# 加载dbc并绑定通道 注意idDBC 必须是c_uint32类型
-def tsdb_load_can_db(DBC_ADDRESS:bytes, ASupportedChannelsBased:bytes, idDBC: c_uint32):
-    """
-    id1 = c_int32(0)
-    tsdb_load_can_db(b"C:/1.dbc", b"0,1", id1)
-    """
-    if isinstance(idDBC,int) or isinstance(idDBC,float):
-        idDBC = c_int32(idDBC)
-    r = dll.tsdb_load_can_db(DBC_ADDRESS, ASupportedChannelsBased, byref(idDBC))
-    return r
-
-
-# 解绑所有dbc
-def tsdb_unload_can_dbs():
-    r = dll.tsdb_unload_can_dbs()
-    return r
-
-
-# 获取dbc数量
-def tsdb_get_can_db_count(ACount: c_uint32):
-    """
-    ACount = c_uint32(0)
-    tsdb_get_can_db_count(ACount)
-    print(ACount)
-    """
-    if isinstance(ACount,int) or isinstance(ACount,float):
-        ACount = c_uint32(ACount)
-    r = dll.tsdb_get_can_db_count(byref(ACount))
-    return r
-
 
-# 获取dbc AId
-def tsdb_get_can_db_id(AIndex: c_int32, AId: c_uint32):
-    """
-    ACount = c_uint32(0)
-    tsdb_get_can_db_id(0,ACount)
-    print(ACount)
-    """
-    r = dll.tsdb_get_can_db_id(AIndex, byref(AId))
-    return r
 
 
 # 获取dbc信息
 def tsdb_get_can_db_info(ADatabaseId: c_int32, AType: c_int32, AIndex: c_int32, ASubIndex: c_int32):
     AValue = POINTER(POINTER(c_char))()
     r = dll.tsdb_get_can_db_info(ADatabaseId, c_int32(AType), c_int32(AIndex), c_uint32(ASubIndex), byref(AValue))
     AValue = string_at(AValue).decode("utf8")
@@ -2729,59 +2807,17 @@
     chn = CHANNEL_INDEX.CHN1
     tsflexray_wakeup_pattern(chn,c_int32(1000))
     """
     return dll.tsflexray_wakeup_pattern(AChnIdx,ATimeout)
 
 #tsdb_Flexray api
 
-# 载入flexray数据库
-def tsdb_load_flexray_db(AFliepath:str,ASupportedChannels:str,AId:c_int32):
-    """
-    AId = c_int32(0)
-    tsdb_load_flexray_db(b"C:/1.xml",b'0,1',AId)
-    """
-    if not isinstance(AFliepath,bytes):
-        AFliepath = bytes(AFliepath)
-    if not isinstance(ASupportedChannels,bytes):
-        ASupportedChannels = bytes(ASupportedChannels)
-    ret = dll.tsdb_load_flexray_db(AFliepath,ASupportedChannels,byref(AId))
-    # if ret == 0:
-    #     try:
-    #         ret = flexray_db_parse((AId.value-1)) 
-    #     except:
-    #         return ret  
-    return ret
-
-# 卸载flexray数据库
-def tsdb_unload_flexray_db(AId:c_int32):
-    """
-    AId = c_int32(0)
-    tsdb_load_flexray_db(b"C:/1.xml",b'0,1',AId)
-    tsdb_unload_flexray_db(AId)
-    """
-    return dll.tsdb_unload_flexray_db(AId)
-
-# 卸载所有flexray数据库 
-def tsdb_unload_flexray_dbs():
-    """
-    AId = c_int32(0)
-    tsdb_load_flexray_db(b"C:/1.xml",b'0,1',AId)
-    tsdb_unload_flexray_dbs()
-    """
-    return dll.tsdb_unload_flexray_dbs()
 
-# 获取加载的flexray数据库数量
-def tsdb_get_flexray_db_count(Acount:c_int32):
-    """
-    Acount = c_int32(0)
-    tsdb_get_flexray_db_count(Acount)
-    """
-    return dll.tsdb_get_flexray_db_count(byref(Acount))
 
-# 通过地址获取flexray数据库属性信息
+# 通过地址获取数据库属性信息
 def tsdb_get_flexray_db_properties_by_address_verbose(AAddr:str):
     '''
     db_msg =  app.db_get_flexray_database_properties_by_address(b"0/network1")
     print(db_msg)
     '''
     if not isinstance(AAddr,bytes):
         AAddr = bytes(AAddr)
@@ -2799,28 +2835,28 @@
             AComment = string_at(AComment).decode('utf8')
         except:
             AComment = ''
         return ADBIndex,AFrameCount,ASignalCount,AECUCount,ASupportedChannelMask,string_at(AName).decode('utf8'),AComment
     print(tsapp_get_error_description(ret))
     return AECUCount,AFrameCount,ASignalCount,ASupportedChannelMask,string_at(AName),AComment     
 
-# 通过索引获取flexray数据库属性信息
-def tsdb_get_flexray_db_properties_by_index_verbose(ADBIndex:c_int32):
+# 通过索引获取数据库属性信息
+def tsdb_get_flexray_db_properties_by_indexx_verbose(ADBIndex:c_int32):
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
 
-    ret = dll.tsdb_get_flexray_db_properties_by_index_verbose(ADBIndex,byref(ASignalCount),byref(AFrameCount),byref(AECUCount),byref(ASupportedChannelMask),byref(AName),byref(AComment))
+    ret = dll.tsdb_get_flexray_db_properties_by_indexx_verbose(ADBIndex,byref(ASignalCount),byref(AFrameCount),byref(AECUCount),byref(ASupportedChannelMask),byref(AName),byref(AComment))
 
     if ret ==0:
         try:
             AComment = string_at(AComment).decode('utf8')
         except:
             AComment = ''
         return AECUCount,AFrameCount,ASignalCount,ASupportedChannelMask,string_at(AName),AComment
@@ -2996,24 +3032,15 @@
         # AName = ''
         # print(AName)
     if ret ==0:
         return ASignalType,ACompuMethod,AIsIntel,AStartBit,AUpdateBit,ALength,AFactor,AOffset,AInitValue,string_at(AName).decode('utf8'),AComment
     print(tsapp_get_error_description(ret))
     return ASignalType,ACompuMethod,AIsIntel,AStartBit,AUpdateBit,ALength,AFactor,AOffset,AInitValue,AName,AComment
 
-# 通过索引获取数据库id
-def tsdb_get_flexray_db_id(AIndex:c_int32):
-    '''
-    print(tsdb_get_flexray_db_id(0))
-    '''
-    Aid = c_int32(0)
-    ret = dll.tsdb_get_flexray_db_id(AIndex,byref(Aid))
-    if ret == 0 :
-        return Aid
-    return tsapp_get_error_description(ret)
+
 
 # 启动flexray rbs
 def tscom_flexray_rbs_start():
     return dll.tscom_flexray_rbs_start()
 
 # 停止flexray rbs
 def tscom_flexray_rbs_stop():
@@ -3322,15 +3349,15 @@
         pass
     On_Flexray = OnTx_RxFUNC_Flexray(Flexray_RX)
     tsapp_register_pretx_event_flexray(obj,On_Flexray)
     tsapp_unregister_pretx_events_flexray(obj)
     """
     return dll.tsapp_unregister_pretx_events_flexray(byref(obj))
 
-# 获取flexray数据库中信号定义
+# 获取数据库中信号定义
 def tscom_flexray_get_signal_definition(ASignalAddress:bytes):
     """
     TSignal_ = tscom_flexray_get_signal_definition(b'0/PowerTrain/BSC/BackLightInfo/BrakeLight')
     print(TSignal_)
     """
     ASignalDef=TFlexRaySignal()
     ret = dll.tscom_flexray_get_signal_definition(ASignalAddress,byref(ASignalDef))
@@ -3359,17 +3386,674 @@
     # 设置flexray信号值
     TSignal_ = tscom_flexray_get_signal_definition(b'0/PowerTrain/BSC/BackLightInfo/BrakeLight')
     value= c_double(1.0)
     tscom_flexray_set_signal_value_in_raw_frame(TSignal_,bytes(AFlexray.contents.FData),value)
     '''
     return dll.tscom_flexray_set_signal_value_in_raw_frame(byref(AFlexRaySignal),AData,AValue)
 
+# Flexray db info 
+# 载入数据库
+def tsdb_load_flexray_db(AFliepath:str,ASupportedChannels:str,AId:c_int32):
+    """
+    AId = c_int32(0)
+    tsdb_load_flexray_db(b"C:/1.xml",b'0,1',AId)
+    """
+    if not isinstance(AFliepath,bytes):
+        AFliepath = bytes(AFliepath)
+    if not isinstance(ASupportedChannels,bytes):
+        ASupportedChannels = bytes(ASupportedChannels)
+    ret = dll.tsdb_load_flexray_db(AFliepath,ASupportedChannels,byref(AId))
+    # if ret == 0:
+    #     try:
+    #         ret = flexray_db_parse((AId.value-1)) 
+    #     except:
+    #         return ret  
+    return ret
+
+# 卸载数据库
+def tsdb_unload_flexray_db(AId:c_int32):
+    """
+    AId = c_int32(0)
+    tsdb_load_flexray_db(b"C:/1.xml",b'0,1',AId)
+    tsdb_unload_flexray_db(AId)
+    """
+    return dll.tsdb_unload_flexray_db(AId)
+
+# 卸载所有数据库 
+def tsdb_unload_flexray_dbs():
+    """
+    AId = c_int32(0)
+    tsdb_load_flexray_db(b"C:/1.xml",b'0,1',AId)
+    tsdb_unload_flexray_dbs()
+    """
+    return dll.tsdb_unload_flexray_dbs()
+
+# 获取加载的数据库数量
+def tsdb_get_flexray_db_count(Acount:c_int32):
+    """
+    Acount = c_int32(0)
+    tsdb_get_flexray_db_count(Acount)
+    """
+    return dll.tsdb_get_flexray_db_count(byref(Acount))
+
+# 通过索引获取数据库id
+def tsdb_get_flexray_db_id(AIndex:c_int32):
+    """
+    Args:
+        获取AIndex数据库的ID
+
+    Returns:
+        DBID  or  error description
+    
+    example:
+        Acount = c_int32(0)
+        tsdb_get_flexray_db_count(Acount)
+        for i in range(0,Acount.value):
+            dbid = tsdb_get_flexray_db_id(i)
+
+    """
+    Aid = c_int32(0)
+    ret = dll.tsdb_get_flexray_db_id(AIndex,byref(Aid))
+    if ret == 0 :
+        return Aid
+    return tsapp_get_error_description(ret)
+
+def tsdb_get_flexray_db_properties_by_address(AAddr:bytes,Avalue:TDBProperties):
+    """
+    Args:
+        获取数据库信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db = TDBProperties()
+        tsdb_get_flexray_db_properties_by_address(b'0/network1',db)
+
+    """
+    return dll.tsdb_get_flexray_db_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_flexray_db_properties_by_index(Avalue:TDBProperties):
+    """
+    Args:
+        获取数据库信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db = TDBProperties()
+        db.FDBIndex = 0
+        tsdb_get_flexray_db_properties_by_index(db)
+    """
+    return dll.tsdb_get_flexray_db_properties_by_index(byref(Avalue))
+
+def tsdb_get_flexray_db_ecu_properties_by_address(AAddr:bytes,Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库ecu信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu = TDBECUProperties()
+        tsdb_get_flexray_db_ecu_properties_by_address(b"0/network1/ecu1",db_ecu)
+    """
+    return dll.tsdb_get_flexray_db_ecu_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_flexray_db_ecu_properties_by_index(Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库ecu信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu = TDBECUProperties()
+        db_ecu.FDBIndex = 0
+        db_ecu.FECUIndex = 0
+        tsdb_get_flexray_db_ecu_properties_by_index(db_ecu)
+    """
+    return dll.tsdb_get_flexray_db_ecu_properties_by_index(byref(Avalue))
+
+def tsdb_get_flexray_db_frame_properties_by_address(AAddr:bytes,Avalue:TDBFrameProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        tsdb_get_flexray_db_frame_properties_by_address(b"0/network1/ecu1/frame1",db_ecu_frame)
+    """
+    return dll.tsdb_get_flexray_db_frame_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_flexray_db_frame_properties_by_index(Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        db_ecu_frame.FDBIndex = 0
+        db_ecu_frame.FECUIndex = 0
+        db_ecu_frame.FFrameIndex = 0
+        db_ecu_frame.FIsTx = 1
+        tsdb_get_flexray_db_frame_properties_by_index(db_ecu_frame)
+    """
+    return dll.tsdb_get_flexray_db_frame_properties_by_index(byref(Avalue))
+
+def tsdb_get_flexray_db_frame_properties_by_db_index(AIdxDB:c_int32,AIndex:c_int32,Avalue:TDBFrameProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        tsdb_get_flexray_db_frame_properties_by_db_index(0,0,db_ecu_frame)
+    """
+    return dll.tsdb_get_flexray_db_frame_properties_by_db_index(AIdxDB,AIndex,byref(Avalue))
+
+
+def tsdb_get_flexray_db_signal_properties_by_address(AAddr:bytes,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库signal信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_flexray_db_signal_properties_by_address(b"0/network1/ecu1/frame1/signal1",db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_flexray_db_signal_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_flexray_db_signal_properties_by_index(Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库signal信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        db_ecu_frame_signal.FDBIndex = 0
+        db_ecu_frame_signal.FECUIndex = 0
+        db_ecu_frame_signal.FFrameIndex = 0
+        db_ecu_frame_signal.FSignalIndex = 0
+        db_ecu_frame_signal.FIsTx = 1
+        tsdb_get_flexray_db_signal_properties_by_index(db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_flexray_db_signal_properties_by_index(byref(Avalue))
+
+def tsdb_get_flexray_db_signal_properties_by_db_index(AIdxDB:c_int32,AIndex:c_int32,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_flexray_db_signal_properties_by_db_index(0,0,db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_flexray_db_signal_properties_by_db_index(AIdxDB,AIndex,byref(Avalue))
+
+def tsdb_get_flexray_db_signal_properties_by_frame_index(AIdxDB:c_int32,Frameidx:c_int32,AIndex:c_int32,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_flexray_db_signal_properties_by_frame_index(0,0,0,db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_flexray_db_signal_properties_by_frame_index(AIdxDB,Frameidx,AIndex,byref(Avalue))
+
+# can db info
+
+# 加载dbc并绑定通道 注意idDBC 必须是c_uint32类型
+def tsdb_load_can_db(AFliepath:str,ASupportedChannels:str,AId:c_int32):
+    """
+    AId = c_int32(0)
+    tsdb_load_can_db(b"C:/1.xml",b'0,1',AId)
+    """
+    if not isinstance(AFliepath,bytes):
+        AFliepath = bytes(AFliepath)
+    if not isinstance(ASupportedChannels,bytes):
+        ASupportedChannels = bytes(ASupportedChannels)
+    ret = dll.tsdb_load_can_db(AFliepath,ASupportedChannels,byref(AId))
+    # if ret == 0:
+    #     try:
+    #         ret = flexray_db_parse((AId.value-1)) 
+    #     except:
+    #         return ret  
+    return ret
+
+# 卸载数据库
+def tsdb_unload_can_db(AId:c_int32):
+    """
+    AId = c_int32(0)
+    tsdb_load_can_db(b"C:/1.xml",b'0,1',AId)
+    tsdb_unload_can_db(AId)
+    """
+    return dll.tsdb_unload_can_db(AId)
+
+# 卸载所有数据库 
+def tsdb_unload_can_dbs():
+    """
+    AId = c_int32(0)
+    tsdb_load_can_db(b"C:/1.xml",b'0,1',AId)
+    tsdb_unload_can_dbs()
+    """
+    return dll.tsdb_unload_can_dbs()
+
+# 获取加载的数据库数量
+def tsdb_get_can_db_count(Acount:c_int32):
+    """
+    Acount = c_int32(0)
+    tsdb_get_can_db_count(Acount)
+    """
+    return dll.tsdb_get_can_db_count(byref(Acount))
+
+# 通过索引获取数据库id
+def tsdb_get_can_db_id(AIndex:c_int32):
+    """
+    Args:
+        获取AIndex数据库的ID
+
+    Returns:
+        DBID  or  error description
+    
+    example:
+        Acount = c_int32(0)
+        tsdb_get_can_db_count(Acount)
+        for i in range(0,Acount.value):
+            dbid = tsdb_get_can_db_id(i)
+
+    """
+    Aid = c_int32(0)
+    ret = dll.tsdb_get_can_db_id(AIndex,byref(Aid))
+    if ret == 0 :
+        return Aid
+    return tsapp_get_error_description(ret)
+
+def tsdb_get_can_db_properties_by_address(AAddr:bytes,Avalue:TDBProperties):
+    """
+    Args:
+        获取数据库信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db = TDBProperties()
+        tsdb_get_can_db_properties_by_address(b'0/network1',db)
+
+    """
+    return dll.tsdb_get_can_db_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_can_db_properties_by_index(Avalue:TDBProperties):
+    """
+    Args:
+        获取数据库信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db = TDBProperties()
+        db.FDBIndex = 0
+        tsdb_get_can_db_properties_by_index(db)
+    """
+    return dll.tsdb_get_can_db_properties_by_index(byref(Avalue))
+
+def tsdb_get_can_db_ecu_properties_by_address(AAddr:bytes,Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库ecu信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu = TDBECUProperties()
+        tsdb_get_can_db_ecu_properties_by_address(b"0/network1/ecu1",db_ecu)
+    """
+    return dll.tsdb_get_can_db_ecu_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_can_db_ecu_properties_by_index(Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库ecu信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu = TDBECUProperties()
+        db_ecu.FDBIndex = 0
+        db_ecu.FECUIndex = 0
+        tsdb_get_can_db_ecu_properties_by_index(db_ecu)
+    """
+    return dll.tsdb_get_can_db_ecu_properties_by_index(byref(Avalue))
+
+def tsdb_get_can_db_frame_properties_by_address(AAddr:bytes,Avalue:TDBFrameProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        tsdb_get_can_db_frame_properties_by_address(b"0/network1/ecu1/frame1",db_ecu_frame)
+    """
+    return dll.tsdb_get_can_db_frame_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_can_db_frame_properties_by_index(Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        db_ecu_frame.FDBIndex = 0
+        db_ecu_frame.FECUIndex = 0
+        db_ecu_frame.FFrameIndex = 0
+        db_ecu_frame.FIsTx = 1
+        tsdb_get_can_db_frame_properties_by_index(db_ecu_frame)
+    """
+    return dll.tsdb_get_can_db_frame_properties_by_index(byref(Avalue))
+
+def tsdb_get_can_db_frame_properties_by_db_index(AIdxDB:c_int32,AIndex:c_int32,Avalue:TDBFrameProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        tsdb_get_can_db_frame_properties_by_db_index(0,0,db_ecu_frame)
+    """
+    return dll.tsdb_get_can_db_frame_properties_by_db_index(AIdxDB,AIndex,byref(Avalue))
+
+
+def tsdb_get_can_db_signal_properties_by_address(AAddr:bytes,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库signal信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_can_db_signal_properties_by_address(b"0/network1/ecu1/frame1/signal1",db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_can_db_signal_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_can_db_signal_properties_by_index(Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库signal信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        db_ecu_frame_signal.FDBIndex = 0
+        db_ecu_frame_signal.FECUIndex = 0
+        db_ecu_frame_signal.FFrameIndex = 0
+        db_ecu_frame_signal.FSignalIndex = 0
+        db_ecu_frame_signal.FIsTx = 1
+        tsdb_get_can_db_signal_properties_by_index(db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_can_db_signal_properties_by_index(byref(Avalue))
+
+def tsdb_get_can_db_signal_properties_by_db_index(AIdxDB:c_int32,AIndex:c_int32,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_can_db_signal_properties_by_db_index(0,0,db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_can_db_signal_properties_by_db_index(AIdxDB,AIndex,byref(Avalue))
+
+def tsdb_get_can_db_signal_properties_by_frame_index(AIdxDB:c_int32,Frameidx:c_int32,AIndex:c_int32,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_can_db_signal_properties_by_frame_index(0,0,0,db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_can_db_signal_properties_by_frame_index(AIdxDB,Frameidx,AIndex,byref(Avalue))
+
+# lin db info
+def tsdb_load_lin_db(AFliepath:str,ASupportedChannels:str,AId:c_int32):
+    """
+    AId = c_int32(0)
+    tsdb_load_lin_db(b"C:/1.xml",b'0,1',AId)
+    """
+    if not isinstance(AFliepath,bytes):
+        AFliepat数h = bytes(AFliepath)
+    if not isinstance(ASupportedChannels,bytes):
+        ASupportedChannels = bytes(ASupportedChannels)
+    ret = dll.tsdb_load_lin_db(AFliepath,ASupportedChannels,byref(AId))
+    return ret
+
+# 卸载数据库
+def tsdb_unload_lin_db(AId:c_int32):
+    """
+    AId = c_int32(0)
+    tsdb_load_lin_db(b"C:/1.xml",b'0,1',AId)
+    tsdb_unload_lin_db(AId)
+    """
+    return dll.tsdb_unload_lin_db(AId)
+
+# 卸载所有数据库 
+def tsdb_unload_lin_dbs():
+    """
+    AId = c_int32(0)
+    tsdb_load_lin_db(b"C:/1.xml",b'0,1',AId)
+    tsdb_unload_lin_dbs()
+    """
+    return dll.tsdb_unload_lin_dbs()
+
+# 获取加载的数据库数量
+def tsdb_get_lin_db_count(Acount:c_int32):
+    """
+    Acount = c_int32(0)
+    tsdb_get_lin_db_count(Acount)
+    """
+    return dll.tsdb_get_lin_db_count(byref(Acount))
+
+# 通过索引获取数据库id
+def tsdb_get_lin_db_id(AIndex:c_int32):
+    """
+    Args:
+        获取AIndex数据库的ID
+
+    Returns:
+        DBID  or  error description
+    
+    example:
+        Acount = c_int32(0)
+        tsdb_get_lin_db_count(Acount)
+        for i in range(0,Acount.value):
+            dbid = tsdb_get_lin_db_id(i)
+
+    """
+    Aid = c_int32(0)
+    ret = dll.tsdb_get_lin_db_id(AIndex,byref(Aid))
+    if ret == 0 :
+        return Aid
+    return tsapp_get_error_description(ret)
+
+def tsdb_get_lin_db_properties_by_address(AAddr:bytes,Avalue:TDBProperties):
+    """
+    Args:
+        获取数据库信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db = TDBProperties()
+        tsdb_get_lin_db_properties_by_address(b'0/network1',db)
+
+    """
+    return dll.tsdb_get_lin_db_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_lin_db_properties_by_index(Avalue:TDBProperties):
+    """
+    Args:
+        获取数据库信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db = TDBProperties()
+        db.FDBIndex = 0
+        tsdb_get_lin_db_properties_by_index(db)
+    """
+    return dll.tsdb_get_lin_db_properties_by_index(byref(Avalue))
+
+def tsdb_get_lin_db_ecu_properties_by_address(AAddr:bytes,Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库ecu信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu = TDBECUProperties()
+        tsdb_get_lin_db_ecu_properties_by_address(b"0/network1/ecu1",db_ecu)
+    """
+    return dll.tsdb_get_lin_db_ecu_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_lin_db_ecu_properties_by_index(Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库ecu信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu = TDBECUProperties()
+        db_ecu.FDBIndex = 0
+        db_ecu.FECUIndex = 0
+        tsdb_get_lin_db_ecu_properties_by_index(db_ecu)
+    """
+    return dll.tsdb_get_lin_db_ecu_properties_by_index(byref(Avalue))
+
+def tsdb_get_lin_db_frame_properties_by_address(AAddr:bytes,Avalue:TDBFrameProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        tsdb_get_lin_db_frame_properties_by_address(b"0/network1/ecu1/frame1",db_ecu_frame)
+    """
+    return dll.tsdb_get_lin_db_frame_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_lin_db_frame_properties_by_index(Avalue:TDBECUProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        db_ecu_frame.FDBIndex = 0
+        db_ecu_frame.FECUIndex = 0
+        db_ecu_frame.FFrameIndex = 0
+        db_ecu_frame.FIsTx = 1
+        tsdb_get_lin_db_frame_properties_by_index(db_ecu_frame)
+    """
+    return dll.tsdb_get_lin_db_frame_properties_by_index(byref(Avalue))
+
+def tsdb_get_lin_db_frame_properties_by_db_index(AIdxDB:c_int32,AIndex:c_int32,Avalue:TDBFrameProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame = TDBFrameProperties()
+        tsdb_get_lin_db_frame_properties_by_db_index(0,0,db_ecu_frame)
+    """
+    return dll.tsdb_get_lin_db_frame_properties_by_db_index(AIdxDB,AIndex,byref(Avalue))
+
+
+def tsdb_get_lin_db_signal_properties_by_address(AAddr:bytes,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库signal信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_lin_db_signal_properties_by_address(b"0/network1/ecu1/frame1/signal1",db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_lin_db_signal_properties_by_address(AAddr,byref(Avalue))
+
+def tsdb_get_lin_db_signal_properties_by_index(Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库signal信息
+    Returns:
+        error code  0:ok  other:error
+    
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        db_ecu_frame_signal.FDBIndex = 0
+        db_ecu_frame_signal.FECUIndex = 0
+        db_ecu_frame_signal.FFrameIndex = 0
+        db_ecu_frame_signal.FSignalIndex = 0
+        db_ecu_frame_signal.FIsTx = 1
+        tsdb_get_lin_db_signal_properties_by_index(db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_lin_db_signal_properties_by_index(byref(Avalue))
+
+def tsdb_get_lin_db_signal_properties_by_db_index(AIdxDB:c_int32,AIndex:c_int32,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_lin_db_signal_properties_by_db_index(0,0,db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_lin_db_signal_properties_by_db_index(AIdxDB,AIndex,byref(Avalue))
+
+def tsdb_get_lin_db_signal_properties_by_frame_index(AIdxDB:c_int32,Frameidx:c_int32,AIndex:c_int32,Avalue:TDBSignalProperties):
+    """
+    Args:
+        获取数据库frame信息
+    Returns:
+        error code  0:ok  other:error
+    example:
+        db_ecu_frame_signal = TDBSignalProperties()
+        tsdb_get_lin_db_signal_properties_by_frame_index(0,0,0,db_ecu_frame_signal)
+    """
+    return dll.tsdb_get_lin_db_signal_properties_by_frame_index(AIdxDB,Frameidx,AIndex,byref(Avalue))
 # def flexray_db_parse(index):
 #     ecu_list = {}
-#     ecuCount, fmeCount, sgnCount, supportedChannelMask, sName, sComment = tsdb_get_flexray_db_properties_by_index_verbose(index)
+#     ecuCount, fmeCount, sgnCount, supportedChannelMask, sName, sComment = tsdb_get_flexray_db_properties_by_indexx_verbose(index)
 #     for idxECU in range(ecuCount.value):
 #         message_list = []
 #         ATxFrameCount, ARxFrameCount, ecuName, sComment = tsdb_get_flexray_ecu_properties_by_index_verbose(index, idxECU)
 #         # print("ECUName = ",ecuName)
 #         for idxFme in range(ATxFrameCount.value):
 #             chnMask, baseCycle, cycleRep, isStartup, slotId, cycleMask, sgnCount, AFRDLC,sName, sComment= ret = tsdb_get_flexray_frame_properties_by_index_verbose(index, idxECU, idxFme, True)
 #             # print('Tx Frame', sName, ', comment:', sComment, ', base cycle:', baseCycle, ', cycle repetition:', cycleRep, ', slot Id:', slotId, ', cycle mask:', hex(cycleMask.value), ', signal count:', sgnCount)
```

### Comparing `TSMasterAPI-1.1.0/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-1.2.0/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 1.1.0
+Version: 1.2.0
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-1.1.0/license.txt` & `TSMasterAPI-1.2.0/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-1.1.0/setup.py` & `TSMasterAPI-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-03-27 11:56:30
+LastEditTime: 2023-04-12 11:59:42
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
-
+# 
 setup(name='TSMasterAPI',  # 包名
-      version='1.1.0',  # 版本号
+      version='1.2.0',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

