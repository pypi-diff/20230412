# Comparing `tmp/mammoth-analytics-sdk-1.6.2.tar.gz` & `tmp/mammoth-analytics-sdk-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammoth-analytics-sdk-1.6.2.tar", last modified: Tue Mar 28 06:55:50 2023, max compression
+gzip compressed data, was "mammoth-analytics-sdk-1.6.3.tar", last modified: Wed Apr 12 06:37:31 2023, max compression
```

## Comparing `mammoth-analytics-sdk-1.6.2.tar` & `mammoth-analytics-sdk-1.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 prajna    (1000) prajna    (1000)        0 2023-03-28 06:55:50.465001 mammoth-analytics-sdk-1.6.2/
-drwxrwxr-x   0 prajna    (1000) prajna    (1000)        0 2023-03-28 06:55:50.465001 mammoth-analytics-sdk-1.6.2/MammothAnalytics/
--rw-rw-r--   0 prajna    (1000) prajna    (1000)        0 2022-10-07 05:27:16.000000 mammoth-analytics-sdk-1.6.2/MammothAnalytics/__init__.py
--rw-rw-r--   0 prajna    (1000) prajna    (1000)     2199 2023-03-16 06:02:22.000000 mammoth-analytics-sdk-1.6.2/MammothAnalytics/const.py
--rw-rw-r--   0 prajna    (1000) prajna    (1000)      933 2022-10-07 05:27:16.000000 mammoth-analytics-sdk-1.6.2/MammothAnalytics/errors.py
--rw-rw-r--   0 prajna    (1000) prajna    (1000)    79258 2023-03-28 06:51:23.000000 mammoth-analytics-sdk-1.6.2/MammothAnalytics/mammoth.py
--rw-rw-r--   0 prajna    (1000) prajna    (1000)      294 2022-10-07 05:27:16.000000 mammoth-analytics-sdk-1.6.2/MammothAnalytics/urls.py
--rw-rw-r--   0 prajna    (1000) prajna    (1000)       89 2022-10-07 05:27:16.000000 mammoth-analytics-sdk-1.6.2/MammothAnalytics/utils.py
--rw-rw-r--   0 prajna    (1000) prajna    (1000)     1350 2023-03-28 06:55:50.465001 mammoth-analytics-sdk-1.6.2/PKG-INFO
-drwxrwxr-x   0 prajna    (1000) prajna    (1000)        0 2023-03-28 06:55:50.465001 mammoth-analytics-sdk-1.6.2/mammoth_analytics_sdk.egg-info/
--rw-rw-r--   0 prajna    (1000) prajna    (1000)     1350 2023-03-28 06:55:50.000000 mammoth-analytics-sdk-1.6.2/mammoth_analytics_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 prajna    (1000) prajna    (1000)      393 2023-03-28 06:55:50.000000 mammoth-analytics-sdk-1.6.2/mammoth_analytics_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 prajna    (1000) prajna    (1000)        1 2023-03-28 06:55:50.000000 mammoth-analytics-sdk-1.6.2/mammoth_analytics_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 prajna    (1000) prajna    (1000)       29 2023-03-28 06:55:50.000000 mammoth-analytics-sdk-1.6.2/mammoth_analytics_sdk.egg-info/requires.txt
--rw-rw-r--   0 prajna    (1000) prajna    (1000)       17 2023-03-28 06:55:50.000000 mammoth-analytics-sdk-1.6.2/mammoth_analytics_sdk.egg-info/top_level.txt
--rw-rw-r--   0 prajna    (1000) prajna    (1000)       38 2023-03-28 06:55:50.465001 mammoth-analytics-sdk-1.6.2/setup.cfg
--rw-rw-r--   0 prajna    (1000) prajna    (1000)     1532 2023-03-28 06:51:23.000000 mammoth-analytics-sdk-1.6.2/setup.py
+drwxrwxr-x   0 virendra  (1000) virendra  (1000)        0 2023-04-12 06:37:31.089794 mammoth-analytics-sdk-1.6.3/
+drwxrwxr-x   0 virendra  (1000) virendra  (1000)        0 2023-04-12 06:37:31.089794 mammoth-analytics-sdk-1.6.3/MammothAnalytics/
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)        0 2023-02-07 10:52:15.000000 mammoth-analytics-sdk-1.6.3/MammothAnalytics/__init__.py
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)     2199 2023-02-07 10:52:15.000000 mammoth-analytics-sdk-1.6.3/MammothAnalytics/const.py
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)      933 2023-02-07 10:52:15.000000 mammoth-analytics-sdk-1.6.3/MammothAnalytics/errors.py
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)    79258 2023-04-12 06:34:06.000000 mammoth-analytics-sdk-1.6.3/MammothAnalytics/mammoth.py
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)      294 2023-02-07 10:52:15.000000 mammoth-analytics-sdk-1.6.3/MammothAnalytics/urls.py
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)       89 2023-02-07 10:52:15.000000 mammoth-analytics-sdk-1.6.3/MammothAnalytics/utils.py
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)     1350 2023-04-12 06:37:31.089794 mammoth-analytics-sdk-1.6.3/PKG-INFO
+drwxrwxr-x   0 virendra  (1000) virendra  (1000)        0 2023-04-12 06:37:31.089794 mammoth-analytics-sdk-1.6.3/mammoth_analytics_sdk.egg-info/
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)     1350 2023-04-12 06:37:31.000000 mammoth-analytics-sdk-1.6.3/mammoth_analytics_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)      393 2023-04-12 06:37:31.000000 mammoth-analytics-sdk-1.6.3/mammoth_analytics_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)        1 2023-04-12 06:37:31.000000 mammoth-analytics-sdk-1.6.3/mammoth_analytics_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)       36 2023-04-12 06:37:31.000000 mammoth-analytics-sdk-1.6.3/mammoth_analytics_sdk.egg-info/requires.txt
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)       17 2023-04-12 06:37:31.000000 mammoth-analytics-sdk-1.6.3/mammoth_analytics_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)       38 2023-04-12 06:37:31.089794 mammoth-analytics-sdk-1.6.3/setup.cfg
+-rw-rw-r--   0 virendra  (1000) virendra  (1000)     1539 2023-04-12 06:34:32.000000 mammoth-analytics-sdk-1.6.3/setup.py
```

### Comparing `mammoth-analytics-sdk-1.6.2/MammothAnalytics/const.py` & `mammoth-analytics-sdk-1.6.3/MammothAnalytics/const.py`

 * *Files identical despite different names*

### Comparing `mammoth-analytics-sdk-1.6.2/MammothAnalytics/errors.py` & `mammoth-analytics-sdk-1.6.3/MammothAnalytics/errors.py`

 * *Files identical despite different names*

### Comparing `mammoth-analytics-sdk-1.6.2/MammothAnalytics/mammoth.py` & `mammoth-analytics-sdk-1.6.3/MammothAnalytics/mammoth.py`

 * *Files identical despite different names*

### Comparing `mammoth-analytics-sdk-1.6.2/PKG-INFO` & `mammoth-analytics-sdk-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: mammoth-analytics-sdk
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python client for Mammoth Analytics (https://mammoth.io)
 Home-page: UNKNOWN
 Author: Mammoth developer
 Author-email: developer@mammoth.io
 License: UNKNOWN
 Description: 
         Mammoth is a data management platform that allows you to take your data from its raw state to insights with all the steps in between. More specifically Mammoth allows you to:
```

### Comparing `mammoth-analytics-sdk-1.6.2/mammoth_analytics_sdk.egg-info/PKG-INFO` & `mammoth-analytics-sdk-1.6.3/mammoth_analytics_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: mammoth-analytics-sdk
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python client for Mammoth Analytics (https://mammoth.io)
 Home-page: UNKNOWN
 Author: Mammoth developer
 Author-email: developer@mammoth.io
 License: UNKNOWN
 Description: 
         Mammoth is a data management platform that allows you to take your data from its raw state to insights with all the steps in between. More specifically Mammoth allows you to:
```

### Comparing `mammoth-analytics-sdk-1.6.2/setup.py` & `mammoth-analytics-sdk-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 """
 
 config = {
     'description': 'Python client for Mammoth Analytics (https://mammoth.io)',
     'long_description': docs_test,
     'author': 'Mammoth developer',
     'author_email': 'developer@mammoth.io',
-    'version': '1.6.2',
+    'version': '1.6.3',
     'packages': ['MammothAnalytics'],
     'scripts': [],
     'name': 'mammoth-analytics-sdk',
     'install_requires': [
         'requests',
         'pytest',
         'names',
-        'pydash'
+        'pydash==6.0.2'
     ]
 }
 
 setup(**config)
```

