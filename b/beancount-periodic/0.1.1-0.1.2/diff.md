# Comparing `tmp/beancount-periodic-0.1.1.tar.gz` & `tmp/beancount-periodic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount-periodic-0.1.1.tar", last modified: Tue Apr 12 07:38:45 2022, max compression
+gzip compressed data, was "beancount-periodic-0.1.2.tar", last modified: Wed Apr 12 03:12:08 2023, max compression
```

## Comparing `beancount-periodic-0.1.1.tar` & `beancount-periodic-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-04-12 07:38:45.208485 beancount-periodic-0.1.1/
--rw-rw-rw-   0        0        0       24 2021-10-19 09:56:03.000000 beancount-periodic-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5974 2022-04-12 07:38:45.207486 beancount-periodic-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5332 2022-04-12 07:11:32.000000 beancount-periodic-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-04-12 07:38:45.188537 beancount-periodic-0.1.1/beancount_periodic/
--rw-rw-rw-   0        0        0        0 2022-04-12 07:35:15.000000 beancount-periodic-0.1.1/beancount_periodic/__init__.py
--rw-rw-rw-   0        0        0     3118 2021-10-25 10:15:28.000000 beancount-periodic-0.1.1/beancount_periodic/amortize.py
-drwxrwxrwx   0        0        0        0 2022-04-12 07:38:45.206490 beancount-periodic-0.1.1/beancount_periodic/common/
--rw-rw-rw-   0        0        0      458 2021-10-25 08:42:10.000000 beancount-periodic-0.1.1/beancount_periodic/common/__init__.py
--rw-rw-rw-   0        0        0    10429 2021-10-25 08:56:54.000000 beancount-periodic-0.1.1/beancount_periodic/common/config.py
--rw-rw-rw-   0        0        0     3241 2021-10-25 07:22:53.000000 beancount-periodic-0.1.1/beancount_periodic/common/config_test.py
--rw-rw-rw-   0        0        0      561 2021-10-25 02:39:55.000000 beancount-periodic-0.1.1/beancount_periodic/common/number.py
--rw-rw-rw-   0        0        0      434 2021-10-22 10:30:00.000000 beancount-periodic-0.1.1/beancount_periodic/common/number_test.py
--rw-rw-rw-   0        0        0      289 2021-10-22 06:36:33.000000 beancount-periodic-0.1.1/beancount_periodic/common/plugin_utils.py
--rw-rw-rw-   0        0        0     7687 2021-10-25 10:53:13.000000 beancount-periodic-0.1.1/beancount_periodic/common/utils.py
--rw-rw-rw-   0        0        0     1689 2021-10-25 10:15:14.000000 beancount-periodic-0.1.1/beancount_periodic/depreciate.py
--rw-rw-rw-   0        0        0     2199 2022-04-12 06:51:25.000000 beancount-periodic-0.1.1/beancount_periodic/recur.py
-drwxrwxrwx   0        0        0        0 2022-04-12 07:38:45.198511 beancount-periodic-0.1.1/beancount_periodic.egg-info/
--rw-rw-rw-   0        0        0     5974 2022-04-12 07:38:45.000000 beancount-periodic-0.1.1/beancount_periodic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2022-04-12 07:38:45.000000 beancount-periodic-0.1.1/beancount_periodic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-12 07:38:45.000000 beancount-periodic-0.1.1/beancount_periodic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-04-12 07:38:45.000000 beancount-periodic-0.1.1/beancount_periodic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-04-12 07:38:45.000000 beancount-periodic-0.1.1/beancount_periodic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       40 2022-04-12 05:59:44.000000 beancount-periodic-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-04-12 07:38:45.208485 beancount-periodic-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1081 2022-04-12 07:38:41.000000 beancount-periodic-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:08.788400 beancount-periodic-0.1.2/
+-rw-rw-rw-   0        0        0       24 2021-10-19 09:56:03.000000 beancount-periodic-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5974 2023-04-12 03:12:08.786405 beancount-periodic-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5332 2022-04-12 07:11:32.000000 beancount-periodic-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:08.750501 beancount-periodic-0.1.2/beancount_periodic/
+-rw-rw-rw-   0        0        0        0 2022-04-12 07:35:15.000000 beancount-periodic-0.1.2/beancount_periodic/__init__.py
+-rw-rw-rw-   0        0        0     3118 2021-10-25 10:15:28.000000 beancount-periodic-0.1.2/beancount_periodic/amortize.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:08.783413 beancount-periodic-0.1.2/beancount_periodic/common/
+-rw-rw-rw-   0        0        0      458 2021-10-25 08:42:10.000000 beancount-periodic-0.1.2/beancount_periodic/common/__init__.py
+-rw-rw-rw-   0        0        0    10429 2021-10-25 08:56:54.000000 beancount-periodic-0.1.2/beancount_periodic/common/config.py
+-rw-rw-rw-   0        0        0     3241 2021-10-25 07:22:53.000000 beancount-periodic-0.1.2/beancount_periodic/common/config_test.py
+-rw-rw-rw-   0        0        0      678 2023-04-12 03:03:24.000000 beancount-periodic-0.1.2/beancount_periodic/common/number.py
+-rw-rw-rw-   0        0        0      434 2021-10-22 10:30:00.000000 beancount-periodic-0.1.2/beancount_periodic/common/number_test.py
+-rw-rw-rw-   0        0        0      289 2021-10-22 06:36:33.000000 beancount-periodic-0.1.2/beancount_periodic/common/plugin_utils.py
+-rw-rw-rw-   0        0        0     7687 2021-10-25 10:53:13.000000 beancount-periodic-0.1.2/beancount_periodic/common/utils.py
+-rw-rw-rw-   0        0        0     1689 2021-10-25 10:15:14.000000 beancount-periodic-0.1.2/beancount_periodic/depreciate.py
+-rw-rw-rw-   0        0        0     2199 2022-04-12 06:51:25.000000 beancount-periodic-0.1.2/beancount_periodic/recur.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:12:08.766458 beancount-periodic-0.1.2/beancount_periodic.egg-info/
+-rw-rw-rw-   0        0        0     5974 2023-04-12 03:12:08.000000 beancount-periodic-0.1.2/beancount_periodic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-04-12 03:12:08.000000 beancount-periodic-0.1.2/beancount_periodic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 03:12:08.000000 beancount-periodic-0.1.2/beancount_periodic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-12 03:12:08.000000 beancount-periodic-0.1.2/beancount_periodic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-12 03:12:08.000000 beancount-periodic-0.1.2/beancount_periodic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       40 2022-04-12 05:59:44.000000 beancount-periodic-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 03:12:08.788400 beancount-periodic-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-04-12 03:05:54.000000 beancount-periodic-0.1.2/setup.py
```

### Comparing `beancount-periodic-0.1.1/PKG-INFO` & `beancount-periodic-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-periodic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Beancount plugin to generate periodic transactions #Amortize #Depreciate #Recur
 Home-page: https://github.com/dallaslu/beancount-periodic
 Author: Dallas Lu
 Author-email: 914202+dallaslu@users.noreply.github.com
 License: UNKNOWN
 Project-URL: Issue tracker, https://github.com/dallaslu/beancount-periodic/issues
 Platform: UNKNOWN
```

### Comparing `beancount-periodic-0.1.1/README.md` & `beancount-periodic-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/beancount_periodic/amortize.py` & `beancount-periodic-0.1.2/beancount_periodic/amortize.py`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/beancount_periodic/common/config.py` & `beancount-periodic-0.1.2/beancount_periodic/common/config.py`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/beancount_periodic/common/config_test.py` & `beancount-periodic-0.1.2/beancount_periodic/common/config_test.py`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/beancount_periodic/common/utils.py` & `beancount-periodic-0.1.2/beancount_periodic/common/utils.py`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/beancount_periodic/depreciate.py` & `beancount-periodic-0.1.2/beancount_periodic/depreciate.py`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/beancount_periodic/recur.py` & `beancount-periodic-0.1.2/beancount_periodic/recur.py`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/beancount_periodic.egg-info/PKG-INFO` & `beancount-periodic-0.1.2/beancount_periodic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-periodic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Beancount plugin to generate periodic transactions #Amortize #Depreciate #Recur
 Home-page: https://github.com/dallaslu/beancount-periodic
 Author: Dallas Lu
 Author-email: 914202+dallaslu@users.noreply.github.com
 License: UNKNOWN
 Project-URL: Issue tracker, https://github.com/dallaslu/beancount-periodic/issues
 Platform: UNKNOWN
```

### Comparing `beancount-periodic-0.1.1/beancount_periodic.egg-info/SOURCES.txt` & `beancount-periodic-0.1.2/beancount_periodic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beancount-periodic-0.1.1/setup.py` & `beancount-periodic-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 with open('README.md', 'r', encoding='UTF-8') as f:
     LONG_DESCRIPTION = f.read()
 
 with open('requirements.txt', 'r') as f:
     REQUIREMENTS = list(filter(None, f.read().split('\n')))
```

