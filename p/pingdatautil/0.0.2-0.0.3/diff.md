# Comparing `tmp/pingdatautil-0.0.2.tar.gz` & `tmp/pingdatautil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingdatautil-0.0.2.tar", last modified: Sun Apr  9 11:00:54 2023, max compression
+gzip compressed data, was "pingdatautil-0.0.3.tar", last modified: Wed Apr 12 03:12:21 2023, max compression
```

## Comparing `pingdatautil-0.0.2.tar` & `pingdatautil-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.501476 pingdatautil-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-04-02 15:02:53.000000 pingdatautil-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      231 2023-04-02 15:26:23.000000 pingdatautil-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      142 2023-04-09 11:00:54.501476 pingdatautil-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-04-02 15:02:53.000000 pingdatautil-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.487476 pingdatautil-0.0.2/pingdatautil/
--rw-rw-rw-   0        0        0     6939 2023-04-02 17:34:55.000000 pingdatautil-0.0.2/pingdatautil/AzureStorage.py
--rw-rw-rw-   0        0        0     6272 2023-04-09 09:04:38.000000 pingdatautil-0.0.2/pingdatautil/DataConnection.py
--rw-rw-rw-   0        0        0    20872 2023-04-09 10:39:11.000000 pingdatautil-0.0.2/pingdatautil/DataExport.py
--rw-rw-rw-   0        0        0     2294 2023-04-02 15:51:17.000000 pingdatautil-0.0.2/pingdatautil/EngineHelper.py
--rw-rw-rw-   0        0        0     7118 2023-04-09 10:55:36.000000 pingdatautil-0.0.2/pingdatautil/ExcelFormatter.py
--rw-rw-rw-   0        0        0     6294 2023-04-02 16:21:41.000000 pingdatautil-0.0.2/pingdatautil/GoogleDrive.py
--rw-rw-rw-   0        0        0     5602 2023-04-02 16:20:58.000000 pingdatautil-0.0.2/pingdatautil/GoogleSheet.py
--rw-rw-rw-   0        0        0    22769 2023-04-07 07:52:34.000000 pingdatautil-0.0.2/pingdatautil/HyperClass.py
--rw-rw-rw-   0        0        0     8710 2023-04-02 17:03:36.000000 pingdatautil-0.0.2/pingdatautil/JDBCExport.py
--rw-rw-rw-   0        0        0     4187 2023-04-02 16:59:49.000000 pingdatautil-0.0.2/pingdatautil/JDBCHelper.py
--rw-rw-rw-   0        0        0     2291 2023-04-02 15:47:17.000000 pingdatautil-0.0.2/pingdatautil/LineNotify.py
--rw-rw-rw-   0        0        0     4087 2023-04-02 15:47:31.000000 pingdatautil-0.0.2/pingdatautil/Logger.py
--rw-rw-rw-   0        0        0    15750 2023-04-02 16:44:54.000000 pingdatautil-0.0.2/pingdatautil/ODBCExport.py
--rw-rw-rw-   0        0        0     3756 2023-04-09 08:31:37.000000 pingdatautil-0.0.2/pingdatautil/ODBCHelper.py
--rw-rw-rw-   0        0        0      524 2023-04-09 08:49:40.000000 pingdatautil-0.0.2/pingdatautil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.491476 pingdatautil-0.0.2/pingdatautil.egg-info/
--rw-rw-rw-   0        0        0      142 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 11:00:54.501476 pingdatautil-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-04-09 11:00:06.000000 pingdatautil-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.500475 pingdatautil-0.0.2/test/
--rw-rw-rw-   0        0        0      903 2023-04-09 08:49:13.000000 pingdatautil-0.0.2/test/test-data-connection.py
--rw-rw-rw-   0        0        0      503 2023-04-09 09:58:44.000000 pingdatautil-0.0.2/test/test-data-export-2.py
--rw-rw-rw-   0        0        0     1246 2023-04-09 09:55:34.000000 pingdatautil-0.0.2/test/test-data-export.py
--rw-rw-rw-   0        0        0      542 2023-04-09 10:56:13.000000 pingdatautil-0.0.2/test/test-excel-format.py
--rw-rw-rw-   0        0        0      414 2023-04-07 07:38:37.000000 pingdatautil-0.0.2/test/test-hyper1.py
--rw-rw-rw-   0        0        0      958 2023-04-02 17:22:59.000000 pingdatautil-0.0.2/test/test-hyper2.py
--rw-rw-rw-   0        0        0      756 2023-04-05 07:30:16.000000 pingdatautil-0.0.2/test/test1.py
--rw-rw-rw-   0        0        0      356 2023-04-07 02:52:52.000000 pingdatautil-0.0.2/test/test1a.py
--rw-rw-rw-   0        0        0      779 2023-04-03 04:07:43.000000 pingdatautil-0.0.2/test/test2.py
--rw-rw-rw-   0        0        0     1375 2023-04-02 17:35:00.000000 pingdatautil-0.0.2/test/test3.py
--rw-rw-rw-   0        0        0      276 2023-04-05 07:30:30.000000 pingdatautil-0.0.2/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.235404 pingdatautil-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-02 15:02:53.000000 pingdatautil-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      331 2023-04-12 03:11:58.000000 pingdatautil-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      142 2023-04-12 03:12:21.234404 pingdatautil-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2023-04-12 03:04:56.000000 pingdatautil-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.219642 pingdatautil-0.0.3/pingdatautil/
+-rw-rw-rw-   0        0        0     6939 2023-04-02 17:34:55.000000 pingdatautil-0.0.3/pingdatautil/AzureStorage.py
+-rw-rw-rw-   0        0        0     6272 2023-04-09 09:04:38.000000 pingdatautil-0.0.3/pingdatautil/DataConnection.py
+-rw-rw-rw-   0        0        0    20872 2023-04-09 10:39:11.000000 pingdatautil-0.0.3/pingdatautil/DataExport.py
+-rw-rw-rw-   0        0        0     2294 2023-04-02 15:51:17.000000 pingdatautil-0.0.3/pingdatautil/EngineHelper.py
+-rw-rw-rw-   0        0        0     7118 2023-04-09 10:55:36.000000 pingdatautil-0.0.3/pingdatautil/ExcelFormatter.py
+-rw-rw-rw-   0        0        0     6294 2023-04-02 16:21:41.000000 pingdatautil-0.0.3/pingdatautil/GoogleDrive.py
+-rw-rw-rw-   0        0        0     5602 2023-04-02 16:20:58.000000 pingdatautil-0.0.3/pingdatautil/GoogleSheet.py
+-rw-rw-rw-   0        0        0    22769 2023-04-07 07:52:34.000000 pingdatautil-0.0.3/pingdatautil/HyperClass.py
+-rw-rw-rw-   0        0        0     8710 2023-04-02 17:03:36.000000 pingdatautil-0.0.3/pingdatautil/JDBCExport.py
+-rw-rw-rw-   0        0        0     4187 2023-04-02 16:59:49.000000 pingdatautil-0.0.3/pingdatautil/JDBCHelper.py
+-rw-rw-rw-   0        0        0     2291 2023-04-02 15:47:17.000000 pingdatautil-0.0.3/pingdatautil/LineNotify.py
+-rw-rw-rw-   0        0        0     4087 2023-04-02 15:47:31.000000 pingdatautil-0.0.3/pingdatautil/Logger.py
+-rw-rw-rw-   0        0        0    15750 2023-04-02 16:44:54.000000 pingdatautil-0.0.3/pingdatautil/ODBCExport.py
+-rw-rw-rw-   0        0        0     3756 2023-04-09 08:31:37.000000 pingdatautil-0.0.3/pingdatautil/ODBCHelper.py
+-rw-rw-rw-   0        0        0     3835 2023-04-10 02:37:54.000000 pingdatautil-0.0.3/pingdatautil/ODBCHelper1.py
+-rw-rw-rw-   0        0        0    14299 2023-04-11 09:13:14.000000 pingdatautil-0.0.3/pingdatautil/UnitTest.py
+-rw-rw-rw-   0        0        0      484 2023-04-10 02:36:27.000000 pingdatautil-0.0.3/pingdatautil/_LogUtil.py
+-rw-rw-rw-   0        0        0      566 2023-04-11 07:58:05.000000 pingdatautil-0.0.3/pingdatautil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.224926 pingdatautil-0.0.3/pingdatautil.egg-info/
+-rw-rw-rw-   0        0        0      142 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 03:12:21.235404 pingdatautil-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      365 2023-04-12 03:09:33.000000 pingdatautil-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.233399 pingdatautil-0.0.3/test/
+-rw-rw-rw-   0        0        0      903 2023-04-09 08:49:13.000000 pingdatautil-0.0.3/test/test-data-connection.py
+-rw-rw-rw-   0        0        0      503 2023-04-09 09:58:44.000000 pingdatautil-0.0.3/test/test-data-export-2.py
+-rw-rw-rw-   0        0        0      661 2023-04-11 03:47:54.000000 pingdatautil-0.0.3/test/test-data-export-jdbc.py
+-rw-rw-rw-   0        0        0     1246 2023-04-10 04:00:25.000000 pingdatautil-0.0.3/test/test-data-export.py
+-rw-rw-rw-   0        0        0      557 2023-04-11 03:48:18.000000 pingdatautil-0.0.3/test/test-excel-format.py
+-rw-rw-rw-   0        0        0      414 2023-04-07 07:38:37.000000 pingdatautil-0.0.3/test/test-hyper1.py
+-rw-rw-rw-   0        0        0      958 2023-04-02 17:22:59.000000 pingdatautil-0.0.3/test/test-hyper2.py
+-rw-rw-rw-   0        0        0      756 2023-04-05 07:30:16.000000 pingdatautil-0.0.3/test/test1.py
+-rw-rw-rw-   0        0        0      356 2023-04-07 02:52:52.000000 pingdatautil-0.0.3/test/test1a.py
+-rw-rw-rw-   0        0        0      428 2023-04-09 11:53:27.000000 pingdatautil-0.0.3/test/test1m.py
+-rw-rw-rw-   0        0        0      779 2023-04-03 04:07:43.000000 pingdatautil-0.0.3/test/test2.py
+-rw-rw-rw-   0        0        0     1375 2023-04-02 17:35:00.000000 pingdatautil-0.0.3/test/test3.py
+-rw-rw-rw-   0        0        0      276 2023-04-05 07:30:30.000000 pingdatautil-0.0.3/test/test4.py
+-rw-rw-rw-   0        0        0      123 2023-04-10 02:30:50.000000 pingdatautil-0.0.3/test/test5.py
```

### Comparing `pingdatautil-0.0.2/LICENSE` & `pingdatautil-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/AzureStorage.py` & `pingdatautil-0.0.3/pingdatautil/AzureStorage.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/DataConnection.py` & `pingdatautil-0.0.3/pingdatautil/DataConnection.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/DataExport.py` & `pingdatautil-0.0.3/pingdatautil/DataExport.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/EngineHelper.py` & `pingdatautil-0.0.3/pingdatautil/EngineHelper.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/ExcelFormatter.py` & `pingdatautil-0.0.3/pingdatautil/ExcelFormatter.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/GoogleDrive.py` & `pingdatautil-0.0.3/pingdatautil/GoogleDrive.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/GoogleSheet.py` & `pingdatautil-0.0.3/pingdatautil/GoogleSheet.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/HyperClass.py` & `pingdatautil-0.0.3/pingdatautil/HyperClass.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/JDBCExport.py` & `pingdatautil-0.0.3/pingdatautil/JDBCExport.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/JDBCHelper.py` & `pingdatautil-0.0.3/pingdatautil/JDBCHelper.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/LineNotify.py` & `pingdatautil-0.0.3/pingdatautil/LineNotify.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/Logger.py` & `pingdatautil-0.0.3/pingdatautil/Logger.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/ODBCExport.py` & `pingdatautil-0.0.3/pingdatautil/ODBCExport.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/ODBCHelper.py` & `pingdatautil-0.0.3/pingdatautil/ODBCHelper.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/pingdatautil/__init__.py` & `pingdatautil-0.0.3/pingdatautil/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .Logger import Logger
 from .LineNotify import LineNotify
-from .EngineHelper import EngineHelper
 from .DataConnection import DataConnection
 from .DataExport import DataExport
 from .ODBCHelper import ODBCHelper
 from .ODBCExport import ODBCExport
 from .JDBCHelper import JDBCHelper
 from .JDBCExport import JDBCExport
-from .GoogleSheet import GoogleSheet
-from .GoogleDrive import GoogleDrive
-from .HyperClass import HyperClass
-from .AzureStorage import AzureStorage
 from .ExcelFormatter import ExcelFormatter
+from .UnitTest import UnitTest
+# from .EngineHelper import EngineHelper
+# from .GoogleSheet import GoogleSheet
+# from .GoogleDrive import GoogleDrive
+# from .HyperClass import HyperClass
+# from .AzureStorage import AzureStorage
```

### Comparing `pingdatautil-0.0.2/pingdatautil.egg-info/SOURCES.txt` & `pingdatautil-0.0.3/pingdatautil.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 pingdatautil/HyperClass.py
 pingdatautil/JDBCExport.py
 pingdatautil/JDBCHelper.py
 pingdatautil/LineNotify.py
 pingdatautil/Logger.py
 pingdatautil/ODBCExport.py
 pingdatautil/ODBCHelper.py
+pingdatautil/ODBCHelper1.py
+pingdatautil/UnitTest.py
+pingdatautil/_LogUtil.py
 pingdatautil/__init__.py
 pingdatautil.egg-info/PKG-INFO
 pingdatautil.egg-info/SOURCES.txt
 pingdatautil.egg-info/dependency_links.txt
+pingdatautil.egg-info/requires.txt
 pingdatautil.egg-info/top_level.txt
 test/test-data-connection.py
 test/test-data-export-2.py
+test/test-data-export-jdbc.py
 test/test-data-export.py
 test/test-excel-format.py
 test/test-hyper1.py
 test/test-hyper2.py
 test/test1.py
 test/test1a.py
+test/test1m.py
 test/test2.py
 test/test3.py
-test/test4.py
+test/test4.py
+test/test5.py
```

### Comparing `pingdatautil-0.0.2/test/test-data-connection.py` & `pingdatautil-0.0.3/test/test-data-connection.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/test/test-data-export.py` & `pingdatautil-0.0.3/test/test-data-export.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/test/test-excel-format.py` & `pingdatautil-0.0.3/test/test-excel-format.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 import pingdatautil
 
 logger = pingdatautil.Logger()
 
 dc = pingdatautil.DataConnection(logger=logger)
-cs = f"DRIVER=ODBC Driver 17 for SQL Server;SERVER=localhost;PORT=1433;DATABASE=TEST;UID=sa;PWD=P@ssw0rd;"
+cs = f"DRIVER=ODBC Driver 17 for SQL Server;SERVER=localhost;PORT=1433;DATABASE=DEMO_DATA;UID=sa;PWD=P@ssw0rd;"
 dc.connect(cs, mode="odbc")
 
 ex = pingdatautil.ExcelFormatter(logger=logger)
 
-df = pd.read_sql("SELECT * FROM BNK48_MEMBER", con=dc.conn)
+df = pd.read_sql("SELECT TOP 1000 * FROM DEMO_SALES_1M", con=dc.conn)
 
-file_name = "D:\\TEMP\\BNK.xlsx"
-sheet_name = "BNK48"
+file_name = "D:\\TEMP\\DATA.xlsx"
+sheet_name = "DATA"
 
 ex.set_config({"font-family": "Tahoma", "font-size": 10})
 
 ex.df_to_excel(df, file_name, sheet_name)
```

### Comparing `pingdatautil-0.0.2/test/test-hyper2.py` & `pingdatautil-0.0.3/test/test-hyper2.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/test/test1.py` & `pingdatautil-0.0.3/test/test1.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/test/test2.py` & `pingdatautil-0.0.3/test/test2.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.2/test/test3.py` & `pingdatautil-0.0.3/test/test3.py`

 * *Files identical despite different names*

