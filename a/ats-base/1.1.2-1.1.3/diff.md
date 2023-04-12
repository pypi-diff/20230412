# Comparing `tmp/ats_base-1.1.2.tar.gz` & `tmp/ats_base-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_base-1.1.2.tar", last modified: Wed Apr 12 01:15:08 2023, max compression
+gzip compressed data, was "ats_base-1.1.3.tar", last modified: Wed Apr 12 02:34:45 2023, max compression
```

## Comparing `ats_base-1.1.2.tar` & `ats_base-1.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:08.635730 ats_base-1.1.2/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_base-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      305 2023-04-08 10:09:46.000000 ats_base-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-12 01:15:08.631740 ats_base-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_base-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:07.466855 ats_base-1.1.2/ats_base/
--rw-rw-rw-   0        0        0        0 2022-09-15 08:20:17.000000 ats_base-1.1.2/ats_base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:07.782011 ats_base-1.1.2/ats_base/base/
--rw-rw-rw-   0        0        0        0 2022-09-15 08:27:28.000000 ats_base-1.1.2/ats_base/base/__init__.py
--rw-rw-rw-   0        0        0      868 2022-10-08 05:21:17.000000 ats_base-1.1.2/ats_base/base/entrance.py
--rw-rw-rw-   0        0        0     1739 2023-04-07 00:56:47.000000 ats_base-1.1.2/ats_base/base/req.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:08.220840 ats_base-1.1.2/ats_base/common/
--rw-rw-rw-   0        0        0        0 2022-05-30 03:34:10.000000 ats_base-1.1.2/ats_base/common/__init__.py
--rw-rw-rw-   0        0        0     3706 2023-04-12 01:13:01.000000 ats_base-1.1.2/ats_base/common/func.py
--rw-rw-rw-   0        0        0      656 2022-10-11 06:12:32.000000 ats_base-1.1.2/ats_base/common/resp.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:08.371437 ats_base-1.1.2/ats_base/config/
--rw-rw-rw-   0        0        0        0 2022-05-26 08:20:18.000000 ats_base-1.1.2/ats_base/config/__init__.py
--rw-rw-rw-   0        0        0      401 2023-04-07 01:00:41.000000 ats_base-1.1.2/ats_base/config/config.ini
--rw-rw-rw-   0        0        0      251 2022-05-30 01:53:51.000000 ats_base-1.1.2/ats_base/config/configure.py
--rw-rw-rw-   0        0        0     1108 2022-12-22 02:31:24.000000 ats_base-1.1.2/ats_base/config/rewrite_config.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:08.402354 ats_base-1.1.2/ats_base/log/
--rw-rw-rw-   0        0        0        0 2022-09-20 00:58:33.000000 ats_base-1.1.2/ats_base/log/__init__.py
--rw-rw-rw-   0        0        0     3449 2023-04-12 01:14:31.000000 ats_base-1.1.2/ats_base/log/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:08.597831 ats_base-1.1.2/ats_base/service/
--rw-rw-rw-   0        0        0        0 2022-05-26 08:20:27.000000 ats_base-1.1.2/ats_base/service/__init__.py
--rw-rw-rw-   0        0        0      225 2022-09-16 06:07:59.000000 ats_base-1.1.2/ats_base/service/app.py
--rw-rw-rw-   0        0        0     1691 2022-10-08 06:47:45.000000 ats_base-1.1.2/ats_base/service/db.py
--rw-rw-rw-   0        0        0      432 2023-04-11 01:28:00.000000 ats_base-1.1.2/ats_base/service/em.py
--rw-rw-rw-   0        0        0     8729 2022-10-26 00:59:06.000000 ats_base-1.1.2/ats_base/service/mm.py
--rw-rw-rw-   0        0        0      957 2022-10-09 01:12:00.000000 ats_base-1.1.2/ats_base/service/pro.py
--rw-rw-rw-   0        0        0     1236 2023-04-07 01:08:33.000000 ats_base-1.1.2/ats_base/service/udm.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:15:07.658341 ats_base-1.1.2/ats_base.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-12 01:15:06.000000 ats_base-1.1.2/ats_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-04-12 01:15:07.000000 ats_base-1.1.2/ats_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 01:15:06.000000 ats_base-1.1.2/ats_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-12 01:15:06.000000 ats_base-1.1.2/ats_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 01:15:06.000000 ats_base-1.1.2/ats_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 01:15:08.635730 ats_base-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      947 2023-04-12 01:14:50.000000 ats_base-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:45.544259 ats_base-1.1.3/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_base-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      305 2023-04-08 10:09:46.000000 ats_base-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-12 02:34:45.542274 ats_base-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_base-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:44.773146 ats_base-1.1.3/ats_base/
+-rw-rw-rw-   0        0        0        0 2022-09-15 08:20:17.000000 ats_base-1.1.3/ats_base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:44.986387 ats_base-1.1.3/ats_base/base/
+-rw-rw-rw-   0        0        0        0 2022-09-15 08:27:28.000000 ats_base-1.1.3/ats_base/base/__init__.py
+-rw-rw-rw-   0        0        0      868 2022-10-08 05:21:17.000000 ats_base-1.1.3/ats_base/base/entrance.py
+-rw-rw-rw-   0        0        0     1739 2023-04-07 00:56:47.000000 ats_base-1.1.3/ats_base/base/req.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:45.069163 ats_base-1.1.3/ats_base/common/
+-rw-rw-rw-   0        0        0        0 2022-05-30 03:34:10.000000 ats_base-1.1.3/ats_base/common/__init__.py
+-rw-rw-rw-   0        0        0     3778 2023-04-12 02:34:23.000000 ats_base-1.1.3/ats_base/common/func.py
+-rw-rw-rw-   0        0        0      656 2022-10-11 06:12:32.000000 ats_base-1.1.3/ats_base/common/resp.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:45.171889 ats_base-1.1.3/ats_base/config/
+-rw-rw-rw-   0        0        0        0 2022-05-26 08:20:18.000000 ats_base-1.1.3/ats_base/config/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-04-07 01:00:41.000000 ats_base-1.1.3/ats_base/config/config.ini
+-rw-rw-rw-   0        0        0      251 2022-05-30 01:53:51.000000 ats_base-1.1.3/ats_base/config/configure.py
+-rw-rw-rw-   0        0        0     1108 2022-12-22 02:31:24.000000 ats_base-1.1.3/ats_base/config/rewrite_config.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:45.267002 ats_base-1.1.3/ats_base/log/
+-rw-rw-rw-   0        0        0        0 2022-09-20 00:58:33.000000 ats_base-1.1.3/ats_base/log/__init__.py
+-rw-rw-rw-   0        0        0     3449 2023-04-12 01:14:31.000000 ats_base-1.1.3/ats_base/log/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:45.503368 ats_base-1.1.3/ats_base/service/
+-rw-rw-rw-   0        0        0        0 2022-05-26 08:20:27.000000 ats_base-1.1.3/ats_base/service/__init__.py
+-rw-rw-rw-   0        0        0      225 2022-09-16 06:07:59.000000 ats_base-1.1.3/ats_base/service/app.py
+-rw-rw-rw-   0        0        0     1691 2022-10-08 06:47:45.000000 ats_base-1.1.3/ats_base/service/db.py
+-rw-rw-rw-   0        0        0      432 2023-04-11 01:28:00.000000 ats_base-1.1.3/ats_base/service/em.py
+-rw-rw-rw-   0        0        0     8729 2022-10-26 00:59:06.000000 ats_base-1.1.3/ats_base/service/mm.py
+-rw-rw-rw-   0        0        0      957 2022-10-09 01:12:00.000000 ats_base-1.1.3/ats_base/service/pro.py
+-rw-rw-rw-   0        0        0     1236 2023-04-07 01:08:33.000000 ats_base-1.1.3/ats_base/service/udm.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:34:44.881666 ats_base-1.1.3/ats_base.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-12 02:34:44.000000 ats_base-1.1.3/ats_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-04-12 02:34:44.000000 ats_base-1.1.3/ats_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:34:44.000000 ats_base-1.1.3/ats_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-12 02:34:44.000000 ats_base-1.1.3/ats_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 02:34:44.000000 ats_base-1.1.3/ats_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:34:45.545257 ats_base-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      947 2023-04-12 02:34:39.000000 ats_base-1.1.3/setup.py
```

### Comparing `ats_base-1.1.2/PKG-INFO` & `ats_base-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_base
-Version: 1.1.2
+Version: 1.1.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_base
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_base-1.1.2/README.md` & `ats_base-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/base/entrance.py` & `ats_base-1.1.3/ats_base/base/entrance.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/base/req.py` & `ats_base-1.1.3/ats_base/base/req.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/common/func.py` & `ats_base-1.1.3/ats_base/common/func.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 from dateutil import parser
 from dateutil.relativedelta import relativedelta
 
 SERVICE = 'API'
 
 
 def project_dir():
-    return os.getenv('PROJECT_DIR')
+    root = os.getenv('PROJECT_DIR')
+    if root is None:
+        return '/service/app'
+
+    return root
 
 
 def to_dict(**kwargs):
     """
     转化为dict类型数据
     :param kwargs:
     :return:
```

### Comparing `ats_base-1.1.2/ats_base/common/resp.py` & `ats_base-1.1.3/ats_base/common/resp.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/config/rewrite_config.py` & `ats_base-1.1.3/ats_base/config/rewrite_config.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/log/logger.py` & `ats_base-1.1.3/ats_base/log/logger.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/service/db.py` & `ats_base-1.1.3/ats_base/service/db.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/service/mm.py` & `ats_base-1.1.3/ats_base/service/mm.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/service/pro.py` & `ats_base-1.1.3/ats_base/service/pro.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base/service/udm.py` & `ats_base-1.1.3/ats_base/service/udm.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/ats_base.egg-info/PKG-INFO` & `ats_base-1.1.3/ats_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-base
-Version: 1.1.2
+Version: 1.1.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_base
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_base-1.1.2/ats_base.egg-info/SOURCES.txt` & `ats_base-1.1.3/ats_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.2/setup.py` & `ats_base-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_base",
-    version="1.1.2",
+    version="1.1.3",
     py_modules=['ats_base'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_base",
```

