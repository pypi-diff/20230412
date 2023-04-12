# Comparing `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.0.tar.gz` & `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.0.tar", last modified: Thu Feb 16 09:46:08 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.1.tar", last modified: Wed Apr 12 09:31:31 2023, max compression
```

## Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0.tar` & `alibabacloud_resourcedirectorymaster20220419-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2448 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1082 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1167 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   170153 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419/client.py
--rw-r--r--   0 root         (0) root         (0)   291489 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2448 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2710 2023-02-16 09:46:08.000000 alibabacloud_resourcedirectorymaster20220419-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259967 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/client.py
+-rw-r--r--   0 root         (0) root         (0)   397637 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-04-12 09:31:31.000000 alibabacloud_resourcedirectorymaster20220419-1.0.1/setup.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0/LICENSE` & `alibabacloud_resourcedirectorymaster20220419-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcedirectorymaster20220419
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0/README-CN.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0/README.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcedirectorymaster20220419
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt` & `alibabacloud_resourcedirectorymaster20220419-1.0.1/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+ChangeLog.md
 LICENSE
 MANIFEST.in
 README-CN.md
 README.md
 setup.cfg
 setup.py
 alibabacloud_resourcedirectorymaster20220419/__init__.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.0/setup.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcedirectorymaster20220419.
 
-Created on 16/02/2023
+Created on 12/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcedirectorymaster20220419"
 NAME = "alibabacloud_resourcedirectorymaster20220419" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python"
```

