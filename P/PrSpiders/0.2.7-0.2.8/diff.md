# Comparing `tmp/PrSpiders-0.2.7.tar.gz` & `tmp/PrSpiders-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.2.7.tar", last modified: Mon Apr 10 14:07:26 2023, max compression
+gzip compressed data, was "PrSpiders-0.2.8.tar", last modified: Wed Apr 12 08:13:45 2023, max compression
```

## Comparing `PrSpiders-0.2.7.tar` & `PrSpiders-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.300608 PrSpiders-0.2.7/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0     4469 2023-04-10 14:07:26.296610 PrSpiders-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.228608 PrSpiders-0.2.7/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.2.7/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.2.7/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    10988 2023-04-07 07:28:46.000000 PrSpiders-0.2.7/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3995 2023-04-07 07:28:46.000000 PrSpiders-0.2.7/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.7/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.260610 PrSpiders-0.2.7/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4469 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-04-10 14:07:26.000000 PrSpiders-0.2.7/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-04-10 14:07:25.000000 PrSpiders-0.2.7/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3957 2023-04-10 01:15:21.000000 PrSpiders-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.274610 PrSpiders-0.2.7/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.2.7/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.2.7/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.2.7/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.7/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-04-10 14:07:26.300608 PrSpiders-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-04-10 14:06:53.000000 PrSpiders-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:07:26.293612 PrSpiders-0.2.7/table_parse/
--rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.2.7/table_parse/T.py
--rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.2.7/table_parse/__init__.py
--rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.2.7/table_parse/tb_parse.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.125501 PrSpiders-0.2.8/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     4469 2023-04-12 08:13:45.123929 PrSpiders-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 08:13:44.966773 PrSpiders-0.2.8/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.2.8/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.2.8/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    10988 2023-04-07 07:28:46.000000 PrSpiders-0.2.8/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3995 2023-04-07 07:28:46.000000 PrSpiders-0.2.8/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.8/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:13:44.997774 PrSpiders-0.2.8/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4469 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3957 2023-04-10 01:15:21.000000 PrSpiders-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.003774 PrSpiders-0.2.8/pkg/
+-rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.2.8/pkg/__init.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 08:12:31.000000 PrSpiders-0.2.8/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.018772 PrSpiders-0.2.8/pkg/prspider/
+-rw-rw-rw-   0        0        0     1160 2023-04-12 08:12:59.000000 PrSpiders-0.2.8/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      259 2023-03-31 06:17:29.000000 PrSpiders-0.2.8/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.2.8/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-31 06:15:13.000000 PrSpiders-0.2.8/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.093775 PrSpiders-0.2.8/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.2.8/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.2.8/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.2.8/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.8/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 08:13:45.126520 PrSpiders-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-04-12 08:12:59.000000 PrSpiders-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.109776 PrSpiders-0.2.8/table_parse/
+-rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.2.8/table_parse/T.py
+-rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.2.8/table_parse/__init__.py
+-rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.2.8/table_parse/tb_parse.py
```

### Comparing `PrSpiders-0.2.7/LICENSE.txt` & `PrSpiders-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/PKG-INFO` & `PrSpiders-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.7
+Version: 0.2.8
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.2.7/PrSpider/PrSpiders.py` & `PrSpiders-0.2.8/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/PrSpider/pxpath.py` & `PrSpiders-0.2.8/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/PrSpider/requestXpath.py` & `PrSpiders-0.2.8/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/PrSpider/useragent.py` & `PrSpiders-0.2.8/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.2.8/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.7
+Version: 0.2.8
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.2.7/README.md` & `PrSpiders-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/requestXpath/__init__.py` & `PrSpiders-0.2.8/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/requestXpath/pxpath.py` & `PrSpiders-0.2.8/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/requestXpath/requestXpath.py` & `PrSpiders-0.2.8/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/requestXpath/useragent.py` & `PrSpiders-0.2.8/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/setup.py` & `PrSpiders-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

### Comparing `PrSpiders-0.2.7/table_parse/T.py` & `PrSpiders-0.2.8/table_parse/T.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.7/table_parse/tb_parse.py` & `PrSpiders-0.2.8/table_parse/tb_parse.py`

 * *Files identical despite different names*

