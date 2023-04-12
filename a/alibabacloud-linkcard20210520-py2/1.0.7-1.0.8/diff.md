# Comparing `tmp/alibabacloud_linkcard20210520_py2-1.0.7.tar.gz` & `tmp/alibabacloud_linkcard20210520_py2-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkcard20210520_py2-1.0.7.tar", last modified: Tue Mar 14 07:23:11 2023, max compression
+gzip compressed data, was "dist/alibabacloud_linkcard20210520_py2-1.0.8.tar", last modified: Wed Apr 12 07:08:09 2023, max compression
```

## Comparing `alibabacloud_linkcard20210520_py2-1.0.7.tar` & `alibabacloud_linkcard20210520_py2-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      475 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42043 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520/client.py
--rw-r--r--   0 root         (0) root         (0)   237751 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-03-14 07:23:11.000000 alibabacloud_linkcard20210520_py2-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42160 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/client.py
+-rw-r--r--   0 root         (0) root         (0)   238312 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/setup.py
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/LICENSE` & `alibabacloud_linkcard20210520_py2-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/PKG-INFO` & `alibabacloud_linkcard20210520_py2-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkcard20210520_py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Linkcard (20210520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/README-CN.md` & `alibabacloud_linkcard20210520_py2-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/README.md` & `alibabacloud_linkcard20210520_py2-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520/client.py` & `alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,14 +770,16 @@
     def list_directional_detail(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_directional_detail_with_options(request, runtime)
 
     def list_order_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.credential_no):
+            query['CredentialNo'] = request.credential_no
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.order_id):
             query['OrderId'] = request.order_id
         if not UtilClient.is_unset(request.order_status):
             query['OrderStatus'] = request.order_status
         if not UtilClient.is_unset(request.order_type):
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520/models.py` & `alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3341,38 +3341,43 @@
             self.res_id = m.get('ResId')
         if m.get('SerialNo') is not None:
             self.serial_no = m.get('SerialNo')
         return self
 
 
 class GetOperateResultResponseBodyData(TeaModel):
-    def __init__(self, operate_type=None, result=None, status=None):
+    def __init__(self, execute_result=None, operate_type=None, result=None, status=None):
+        self.execute_result = execute_result  # type: str
         self.operate_type = operate_type  # type: str
         self.result = result  # type: bool
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetOperateResultResponseBodyData, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.execute_result is not None:
+            result['ExecuteResult'] = self.execute_result
         if self.operate_type is not None:
             result['OperateType'] = self.operate_type
         if self.result is not None:
             result['Result'] = self.result
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('ExecuteResult') is not None:
+            self.execute_result = m.get('ExecuteResult')
         if m.get('OperateType') is not None:
             self.operate_type = m.get('OperateType')
         if m.get('Result') is not None:
             self.result = m.get('Result')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
@@ -4824,16 +4829,17 @@
         if m.get('body') is not None:
             temp_model = ListDirectionalDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOrderRequest(TeaModel):
-    def __init__(self, end_date=None, order_id=None, order_status=None, order_type=None, page_no=None,
-                 page_size=None, start_date=None):
+    def __init__(self, credential_no=None, end_date=None, order_id=None, order_status=None, order_type=None,
+                 page_no=None, page_size=None, start_date=None):
+        self.credential_no = credential_no  # type: str
         self.end_date = end_date  # type: str
         self.order_id = order_id  # type: str
         self.order_status = order_status  # type: str
         self.order_type = order_type  # type: str
         self.page_no = page_no  # type: int
         self.page_size = page_size  # type: int
         self.start_date = start_date  # type: str
@@ -4843,14 +4849,16 @@
 
     def to_map(self):
         _map = super(ListOrderRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.credential_no is not None:
+            result['CredentialNo'] = self.credential_no
         if self.end_date is not None:
             result['EndDate'] = self.end_date
         if self.order_id is not None:
             result['OrderId'] = self.order_id
         if self.order_status is not None:
             result['OrderStatus'] = self.order_status
         if self.order_type is not None:
@@ -4861,14 +4869,16 @@
             result['PageSize'] = self.page_size
         if self.start_date is not None:
             result['StartDate'] = self.start_date
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('CredentialNo') is not None:
+            self.credential_no = m.get('CredentialNo')
         if m.get('EndDate') is not None:
             self.end_date = m.get('EndDate')
         if m.get('OrderId') is not None:
             self.order_id = m.get('OrderId')
         if m.get('OrderStatus') is not None:
             self.order_status = m.get('OrderStatus')
         if m.get('OrderType') is not None:
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO` & `alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkcard20210520-py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Linkcard (20210520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.7/setup.py` & `alibabacloud_linkcard20210520_py2-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkcard20210520_py2.
 
-Created on 14/03/2023
+Created on 12/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkcard20210520"
 NAME = "alibabacloud_linkcard20210520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Linkcard (20210520) SDK Library for Python2"
```

