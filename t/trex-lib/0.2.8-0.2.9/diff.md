# Comparing `tmp/trex-lib-0.2.8.tar.gz` & `tmp/trex-lib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-lib-0.2.8.tar", last modified: Wed Feb  3 02:45:15 2021, max compression
+gzip compressed data, was "dist/trex-lib-0.2.9.tar", last modified: Thu Feb  4 01:33:21 2021, max compression
```

## Comparing `trex-lib-0.2.8.tar` & `trex-lib-0.2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.193062 trex-lib-0.2.8/
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-0.2.8/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2021-02-03 02:45:15.193273 trex-lib-0.2.8/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-0.2.8/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2021-02-03 02:45:15.194105 trex-lib-0.2.8/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      877 2021-02-03 02:44:58.000000 trex-lib-0.2.8/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.178233 trex-lib-0.2.8/trex_lib.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2021-02-03 02:45:14.000000 trex-lib-0.2.8/trex_lib.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)      957 2021-02-03 02:45:14.000000 trex-lib-0.2.8/trex_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2021-02-03 02:45:14.000000 trex-lib-0.2.8/trex_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)      103 2021-02-03 02:45:14.000000 trex-lib-0.2.8/trex_lib.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       14 2021-02-03 02:45:14.000000 trex-lib-0.2.8/trex_lib.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.178586 trex-lib-0.2.8/trexlib/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-0.2.8/trexlib/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4200 2021-01-21 09:42:37.000000 trex-lib-0.2.8/trexlib/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.179204 trex-lib-0.2.8/trexlib/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-0.2.8/trexlib/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.179596 trex-lib-0.2.8/trexlib/libs/flask_wtf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-0.2.8/trexlib/libs/flask_wtf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-0.2.8/trexlib/libs/flask_wtf/crsf_ext.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.183067 trex-lib-0.2.8/trexlib/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-0.2.8/trexlib/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.190263 trex-lib-0.2.8/trexlib/utils/common/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-0.2.8/trexlib/utils/common/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      428 2020-09-03 08:42:39.000000 trex-lib-0.2.8/trexlib/utils/common/cache_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3168 2020-09-10 04:55:42.000000 trex-lib-0.2.8/trexlib/utils/common/common_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-0.2.8/trexlib/utils/common/conftest.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-0.2.8/trexlib/utils/common/crm_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2345 2020-09-01 10:20:51.000000 trex-lib-0.2.8/trexlib/utils/common/date_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-0.2.8/trexlib/utils/common/float_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-0.2.8/trexlib/utils/common/pagination_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1361 2020-09-04 07:32:41.000000 trex-lib-0.2.8/trexlib/utils/common/phone_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      823 2020-09-04 07:16:17.000000 trex-lib-0.2.8/trexlib/utils/common/user_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      808 2020-11-09 09:40:17.000000 trex-lib-0.2.8/trexlib/utils/crypto_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-03 02:45:15.192445 trex-lib-0.2.8/trexlib/utils/google/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-0.2.8/trexlib/utils/google/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12742 2021-01-26 10:05:22.000000 trex-lib-0.2.8/trexlib/utils/google/bigquery_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3477 2021-01-22 08:40:12.000000 trex-lib-0.2.8/trexlib/utils/google/cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-0.2.8/trexlib/utils/log_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3140 2021-01-22 09:14:05.000000 trex-lib-0.2.8/trexlib/utils/security_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4739 2021-01-06 06:55:12.000000 trex-lib-0.2.8/trexlib/utils/string_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-0.2.8/trexlib/utils/url_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.275596 trex-lib-0.2.9/
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-0.2.9/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2021-02-04 01:33:21.275773 trex-lib-0.2.9/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-0.2.9/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2021-02-04 01:33:21.276412 trex-lib-0.2.9/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      877 2021-02-04 01:32:47.000000 trex-lib-0.2.9/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.259700 trex-lib-0.2.9/trex_lib.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)      957 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)      103 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       14 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.260193 trex-lib-0.2.9/trexlib/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-0.2.9/trexlib/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4200 2021-01-21 09:42:37.000000 trex-lib-0.2.9/trexlib/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.261058 trex-lib-0.2.9/trexlib/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-0.2.9/trexlib/libs/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.261673 trex-lib-0.2.9/trexlib/libs/flask_wtf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-0.2.9/trexlib/libs/flask_wtf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-0.2.9/trexlib/libs/flask_wtf/crsf_ext.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.266218 trex-lib-0.2.9/trexlib/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-0.2.9/trexlib/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.273120 trex-lib-0.2.9/trexlib/utils/common/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-0.2.9/trexlib/utils/common/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      428 2020-09-03 08:42:39.000000 trex-lib-0.2.9/trexlib/utils/common/cache_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3162 2021-02-03 09:11:17.000000 trex-lib-0.2.9/trexlib/utils/common/common_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-0.2.9/trexlib/utils/common/conftest.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-0.2.9/trexlib/utils/common/crm_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2345 2020-09-01 10:20:51.000000 trex-lib-0.2.9/trexlib/utils/common/date_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-0.2.9/trexlib/utils/common/float_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-0.2.9/trexlib/utils/common/pagination_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1361 2020-09-04 07:32:41.000000 trex-lib-0.2.9/trexlib/utils/common/phone_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      823 2020-09-04 07:16:17.000000 trex-lib-0.2.9/trexlib/utils/common/user_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      808 2020-11-09 09:40:17.000000 trex-lib-0.2.9/trexlib/utils/crypto_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.274738 trex-lib-0.2.9/trexlib/utils/google/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-0.2.9/trexlib/utils/google/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12742 2021-01-26 10:05:22.000000 trex-lib-0.2.9/trexlib/utils/google/bigquery_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3477 2021-01-22 08:40:12.000000 trex-lib-0.2.9/trexlib/utils/google/cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-0.2.9/trexlib/utils/log_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3140 2021-01-22 09:14:05.000000 trex-lib-0.2.9/trexlib/utils/security_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4739 2021-01-06 06:55:12.000000 trex-lib-0.2.9/trexlib/utils/string_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-0.2.9/trexlib/utils/url_util.py
```

### Comparing `trex-lib-0.2.8/setup.py` & `trex-lib-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-lib',  
-     version='0.2.8',
+     version='0.2.9',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-lib",
      packages=setuptools.find_packages(),
```

### Comparing `trex-lib-0.2.8/trex_lib.egg-info/SOURCES.txt` & `trex-lib-0.2.9/trex_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/conf.py` & `trex-lib-0.2.9/trexlib/conf.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/common/common_util.py` & `trex-lib-0.2.9/trexlib/utils/common/common_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,33 +74,33 @@
     if sorting_list:
         logging.debug('sort_attr_name=%s', sort_attr_name)
         new_list = sort_list_by_condition(sorting_list, 
                                           condition=lambda x: getattr(x, sort_attr_name), 
                                           reverse_order=reverse_order)
         return new_list
     else:
-        return list
+        return []
 
 def sort_dict_list(sorting_list, sort_attr_name=None, reverse_order=False):
     if sorting_list:
         logging.debug('sort_attr_name=%s', sort_attr_name)
         new_list = sort_list_by_condition(sorting_list, 
                                           condition=lambda x: x.get(sort_attr_name), 
                                           reverse_order=reverse_order)
         return new_list
     else:
-        return list
+        return []
 
 
 def sort_list_by_condition(list, condition=None, reverse_order=False):
     if list:
         new_list = sorted(list, key=condition, reverse=reverse_order)
         return new_list
     else:
-        return list
+        return []
 
 
 def sizeof_fmt(num):
     """Human friendly file size"""
     if isinstance(num, str):
         num = float(num)
```

### Comparing `trex-lib-0.2.8/trexlib/utils/common/crm_util.py` & `trex-lib-0.2.9/trexlib/utils/common/crm_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/common/date_util.py` & `trex-lib-0.2.9/trexlib/utils/common/date_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/common/pagination_util.py` & `trex-lib-0.2.9/trexlib/utils/common/pagination_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/common/phone_util.py` & `trex-lib-0.2.9/trexlib/utils/common/phone_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/common/user_util.py` & `trex-lib-0.2.9/trexlib/utils/common/user_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/crypto_util.py` & `trex-lib-0.2.9/trexlib/utils/crypto_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/google/bigquery_util.py` & `trex-lib-0.2.9/trexlib/utils/google/bigquery_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/google/cloud_tasks_util.py` & `trex-lib-0.2.9/trexlib/utils/google/cloud_tasks_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/security_util.py` & `trex-lib-0.2.9/trexlib/utils/security_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/string_util.py` & `trex-lib-0.2.9/trexlib/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.8/trexlib/utils/url_util.py` & `trex-lib-0.2.9/trexlib/utils/url_util.py`

 * *Files identical despite different names*

