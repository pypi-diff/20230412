# Comparing `tmp/alibabacloud_resourcedirectorymaster20220419_py2-1.0.0.tar.gz` & `tmp/alibabacloud_resourcedirectorymaster20220419_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419_py2-1.0.0.tar", last modified: Thu Feb 16 09:45:54 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419_py2-1.0.1.tar", last modified: Wed Apr 12 09:30:51 2023, max compression
```

## Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0.tar` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2592 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1093 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64652 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419/client.py
--rw-r--r--   0 root         (0) root         (0)   294585 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2592 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3003 2023-02-16 09:45:54.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104716 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419/client.py
+-rw-r--r--   0 root         (0) root         (0)   401384 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3003 2023-04-12 09:30:51.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/LICENSE` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcedirectorymaster20220419_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/README-CN.md` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/README.md` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcedirectorymaster20220419-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

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

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.0/setup.py` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcedirectorymaster20220419_py2.
 
-Created on 16/02/2023
+Created on 12/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcedirectorymaster20220419"
 NAME = "alibabacloud_resourcedirectorymaster20220419_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python2"
```

