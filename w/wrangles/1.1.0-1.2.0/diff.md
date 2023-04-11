# Comparing `tmp/wrangles-1.1.0.tar.gz` & `tmp/wrangles-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrangles-1.1.0.tar", last modified: Thu Mar 30 20:48:00 2023, max compression
+gzip compressed data, was "wrangles-1.2.0.tar", last modified: Tue Apr 11 22:32:34 2023, max compression
```

## Comparing `wrangles-1.1.0.tar` & `wrangles-1.2.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 20:48:00.611900 wrangles-1.1.0/
--rw-rw-rw-   0        0        0     3615 2023-03-30 20:48:00.612897 wrangles-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 20:48:00.591958 wrangles-1.1.0/Wrangles.egg-info/
--rw-rw-rw-   0        0        0     3615 2023-03-30 20:48:00.000000 wrangles-1.1.0/Wrangles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1508 2023-03-30 20:48:00.000000 wrangles-1.1.0/Wrangles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 20:48:00.000000 wrangles-1.1.0/Wrangles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-03-30 20:48:00.000000 wrangles-1.1.0/Wrangles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2023-03-30 20:48:00.000000 wrangles-1.1.0/Wrangles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-30 20:48:00.000000 wrangles-1.1.0/Wrangles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-30 20:48:00.613895 wrangles-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-03-30 20:43:12.000000 wrangles-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 20:48:00.590956 wrangles-1.1.0/wrangles/
--rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.1.0/wrangles/__init__.py
--rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/auth.py
--rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/batching.py
--rw-rw-rw-   0        0        0     2069 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/classify.py
--rw-rw-rw-   0        0        0      559 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/config.py
-drwxrwxrwx   0        0        0        0 2023-03-30 20:48:00.605915 wrangles-1.1.0/wrangles/connectors/
--rw-rw-rw-   0        0        0      427 2023-03-30 14:19:22.000000 wrangles-1.1.0/wrangles/connectors/__init__.py
--rw-rw-rw-   0        0        0    11023 2023-03-30 14:19:22.000000 wrangles-1.1.0/wrangles/connectors/ckan.py
--rw-rw-rw-   0        0        0     7811 2023-03-30 19:56:39.000000 wrangles-1.1.0/wrangles/connectors/file.py
--rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/connectors/http.py
--rw-rw-rw-   0        0        0     1883 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/connectors/jinja.py
--rw-rw-rw-   0        0        0     4537 2022-08-10 19:07:21.000000 wrangles-1.1.0/wrangles/connectors/mongodb.py
--rw-rw-rw-   0        0        0     6136 2022-08-10 19:07:21.000000 wrangles-1.1.0/wrangles/connectors/mssql.py
--rw-rw-rw-   0        0        0     4372 2022-08-10 19:07:21.000000 wrangles-1.1.0/wrangles/connectors/mysql.py
--rw-rw-rw-   0        0        0     6328 2023-03-30 19:57:06.000000 wrangles-1.1.0/wrangles/connectors/notification.py
--rw-rw-rw-   0        0        0     5892 2022-06-23 19:42:00.000000 wrangles-1.1.0/wrangles/connectors/postgres.py
--rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/connectors/pricefx.py
--rw-rw-rw-   0        0        0     4534 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/connectors/recipe.py
--rw-rw-rw-   0        0        0     8530 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/connectors/s3.py
--rw-rw-rw-   0        0        0     4756 2022-08-10 19:07:21.000000 wrangles-1.1.0/wrangles/connectors/salesforce.py
--rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.1.0/wrangles/connectors/sftp.py
--rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.1.0/wrangles/connectors/ssh.py
--rw-rw-rw-   0        0        0     5651 2023-03-30 20:18:43.000000 wrangles-1.1.0/wrangles/connectors/test.py
--rw-rw-rw-   0        0        0     8040 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/connectors/train.py
--rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/console.py
--rw-rw-rw-   0        0        0     1592 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/data.py
--rw-rw-rw-   0        0        0    10063 2023-03-30 19:49:25.000000 wrangles-1.1.0/wrangles/extract.py
--rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/format.py
--rw-rw-rw-   0        0        0    19601 2023-03-30 19:09:34.000000 wrangles-1.1.0/wrangles/recipe.py
-drwxrwxrwx   0        0        0        0 2023-03-30 20:48:00.611900 wrangles-1.1.0/wrangles/recipe_wrangles/
--rw-rw-rw-   0        0        0      562 2022-06-23 19:42:00.000000 wrangles-1.1.0/wrangles/recipe_wrangles/__init__.py
--rw-rw-rw-   0        0        0     6878 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/convert.py
--rw-rw-rw-   0        0        0     8232 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/create.py
--rw-rw-rw-   0        0        0    18689 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/extract.py
--rw-rw-rw-   0        0        0     7692 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/format.py
--rw-rw-rw-   0        0        0    27378 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/main.py
--rw-rw-rw-   0        0        0     8585 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/merge.py
--rw-rw-rw-   0        0        0     7650 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/select.py
--rw-rw-rw-   0        0        0     6361 2023-03-30 18:35:01.000000 wrangles-1.1.0/wrangles/recipe_wrangles/split.py
--rw-rw-rw-   0        0        0     1875 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/select.py
--rw-rw-rw-   0        0        0     2099 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/standardize.py
--rw-rw-rw-   0        0        0     6100 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/train.py
--rw-rw-rw-   0        0        0     1778 2022-12-21 19:41:28.000000 wrangles-1.1.0/wrangles/translate.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.840601 wrangles-1.2.0/
+-rw-rw-rw-   0        0        0     3615 2023-04-11 22:32:34.840601 wrangles-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.816665 wrangles-1.2.0/Wrangles.egg-info/
+-rw-rw-rw-   0        0        0     3615 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1538 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-11 22:32:34.848579 wrangles-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-04-11 22:14:24.000000 wrangles-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.814672 wrangles-1.2.0/wrangles/
+-rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.2.0/wrangles/__init__.py
+-rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/auth.py
+-rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/batching.py
+-rw-rw-rw-   0        0        0     2069 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/classify.py
+-rw-rw-rw-   0        0        0      559 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/config.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.831625 wrangles-1.2.0/wrangles/connectors/
+-rw-rw-rw-   0        0        0      449 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7100 2023-04-11 22:29:27.000000 wrangles-1.2.0/wrangles/connectors/akeneo.py
+-rw-rw-rw-   0        0        0    11023 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/ckan.py
+-rw-rw-rw-   0        0        0     7811 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/file.py
+-rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/http.py
+-rw-rw-rw-   0        0        0     1883 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/jinja.py
+-rw-rw-rw-   0        0        0     4537 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/mongodb.py
+-rw-rw-rw-   0        0        0     6136 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4372 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/mysql.py
+-rw-rw-rw-   0        0        0     6328 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/notification.py
+-rw-rw-rw-   0        0        0     5892 2022-06-23 19:42:00.000000 wrangles-1.2.0/wrangles/connectors/postgres.py
+-rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/pricefx.py
+-rw-rw-rw-   0        0        0     4534 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/recipe.py
+-rw-rw-rw-   0        0        0     8530 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/s3.py
+-rw-rw-rw-   0        0        0     4756 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/salesforce.py
+-rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/sftp.py
+-rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/ssh.py
+-rw-rw-rw-   0        0        0     5651 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/test.py
+-rw-rw-rw-   0        0        0     8040 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/train.py
+-rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/console.py
+-rw-rw-rw-   0        0        0     1592 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/data.py
+-rw-rw-rw-   0        0        0    10183 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/extract.py
+-rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/format.py
+-rw-rw-rw-   0        0        0    19601 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/recipe.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.839603 wrangles-1.2.0/wrangles/recipe_wrangles/
+-rw-rw-rw-   0        0        0      562 2022-06-23 19:42:00.000000 wrangles-1.2.0/wrangles/recipe_wrangles/__init__.py
+-rw-rw-rw-   0        0        0     6878 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/recipe_wrangles/convert.py
+-rw-rw-rw-   0        0        0     8582 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/recipe_wrangles/create.py
+-rw-rw-rw-   0        0        0    19584 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/recipe_wrangles/extract.py
+-rw-rw-rw-   0        0        0     8055 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/format.py
+-rw-rw-rw-   0        0        0    26422 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/recipe_wrangles/main.py
+-rw-rw-rw-   0        0        0     8570 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/merge.py
+-rw-rw-rw-   0        0        0     7681 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/select.py
+-rw-rw-rw-   0        0        0     6435 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/split.py
+-rw-rw-rw-   0        0        0     1875 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/select.py
+-rw-rw-rw-   0        0        0     2099 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/standardize.py
+-rw-rw-rw-   0        0        0     6100 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/train.py
+-rw-rw-rw-   0        0        0     3502 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/translate.py
```

### Comparing `wrangles-1.1.0/PKG-INFO` & `wrangles-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.1.0
+Version: 1.2.0
 Summary: Wrangle your data into shape with machine learning
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Keywords: data,wrangling
 Platform: UNKNOWN
```

### Comparing `wrangles-1.1.0/README.md` & `wrangles-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/Wrangles.egg-info/PKG-INFO` & `wrangles-1.2.0/Wrangles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.1.0
+Version: 1.2.0
 Summary: Wrangle your data into shape with machine learning
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Keywords: data,wrangling
 Platform: UNKNOWN
```

### Comparing `wrangles-1.1.0/Wrangles.egg-info/SOURCES.txt` & `wrangles-1.2.0/Wrangles.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 wrangles.egg-info/PKG-INFO
 wrangles.egg-info/SOURCES.txt
 wrangles.egg-info/dependency_links.txt
 wrangles.egg-info/entry_points.txt
 wrangles.egg-info/requires.txt
 wrangles.egg-info/top_level.txt
 wrangles/connectors/__init__.py
+wrangles/connectors/akeneo.py
 wrangles/connectors/ckan.py
 wrangles/connectors/file.py
 wrangles/connectors/http.py
 wrangles/connectors/jinja.py
 wrangles/connectors/mongodb.py
 wrangles/connectors/mssql.py
 wrangles/connectors/mysql.py
```

### Comparing `wrangles-1.1.0/setup.py` & `wrangles-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     license_files = ('LICENSE.txt',),
     license = 'Apache License 2.0',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
-    version = '1.1.0',
+    version = '1.2.0',
     url = 'https://github.com/wrangleworks/WranglesPy',
     author = 'WrangleWorks',
     author_email = 'chris@wrangleworks.com',
     keywords = ['data','wrangling'],
     install_requires = requirements,
     entry_points ={
         'console_scripts': ['wrangles.recipe = wrangles.console:recipe']
```

### Comparing `wrangles-1.1.0/wrangles/__init__.py` & `wrangles-1.2.0/wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/auth.py` & `wrangles-1.2.0/wrangles/auth.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/batching.py` & `wrangles-1.2.0/wrangles/batching.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/classify.py` & `wrangles-1.2.0/wrangles/classify.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/config.py` & `wrangles-1.2.0/wrangles/config.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/ckan.py` & `wrangles-1.2.0/wrangles/connectors/ckan.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/file.py` & `wrangles-1.2.0/wrangles/connectors/file.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/http.py` & `wrangles-1.2.0/wrangles/connectors/http.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/jinja.py` & `wrangles-1.2.0/wrangles/connectors/jinja.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/mongodb.py` & `wrangles-1.2.0/wrangles/connectors/mongodb.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/mssql.py` & `wrangles-1.2.0/wrangles/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/mysql.py` & `wrangles-1.2.0/wrangles/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/notification.py` & `wrangles-1.2.0/wrangles/connectors/notification.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/postgres.py` & `wrangles-1.2.0/wrangles/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/pricefx.py` & `wrangles-1.2.0/wrangles/connectors/pricefx.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/recipe.py` & `wrangles-1.2.0/wrangles/connectors/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/s3.py` & `wrangles-1.2.0/wrangles/connectors/s3.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/salesforce.py` & `wrangles-1.2.0/wrangles/connectors/salesforce.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/sftp.py` & `wrangles-1.2.0/wrangles/connectors/sftp.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/ssh.py` & `wrangles-1.2.0/wrangles/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/test.py` & `wrangles-1.2.0/wrangles/connectors/test.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/connectors/train.py` & `wrangles-1.2.0/wrangles/connectors/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/console.py` & `wrangles-1.2.0/wrangles/console.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/data.py` & `wrangles-1.2.0/wrangles/data.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/extract.py` & `wrangles-1.2.0/wrangles/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     results = _batching.batch_api_calls(url, params, json_data, batch_size)
 
     if isinstance(input, str): results = results[0]
     
     return results
 
 
-def custom(input: _Union[str, list], model_id: str) -> list:
+def custom(input: _Union[str, list], model_id: str, first_element: bool = False) -> list:
     """
     Extract entities using a custom model.
     Requires WrangleWorks Account and Subscription.
 
     :param input: A string or list of strings to searched for information.
     :param model_id: The model to be used to search for information.
     :return: A list of entities found.
@@ -138,14 +138,17 @@
     # Using model_id in wrong function
     purpose = model_properties['purpose']
     if purpose != 'extract':
         raise ValueError(f'Using {purpose} model_id in an extract function.')
     
     results = _batching.batch_api_calls(url, params, json_data, batch_size)
 
+    if first_element:
+        results = [x[0] if len(x) >= 1 else "" for x in results]
+
     if isinstance(input, str): results = results[0]
     
     return results
 
 
 def html(input: _Union[str, list], dataType: str) -> list:
     """
```

### Comparing `wrangles-1.1.0/wrangles/format.py` & `wrangles-1.2.0/wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/recipe.py` & `wrangles-1.2.0/wrangles/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/__init__.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/convert.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/convert.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/create.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -164,34 +164,38 @@
     # Loop through and create incremental index
     for output_column in output:
         df[output_column] = _np.arange(start, len(df) * step + start, step=step)
 
     return df
 
 
-def jinja(df: _pd.DataFrame, template: dict, output: list, input: str = None) -> _pd.DataFrame:
+def jinja(df: _pd.DataFrame, template: dict, output: _Union[str, list], input: str = None) -> _pd.DataFrame:
     """
     type: object
     description: Output text using a jinja template
     additionalProperties: false
     required:
       - output
       - template
     properties:
       input:
         type: string
         description: |
           Specify a name of column containing a dictionary of elements to be used in jinja template.
           Otherwise, the column headers will be used as keys.
       output:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the column to be output to.
       template:
         type: object
-        description: A dictionary which defines the template/location as well as the form which the template is input
+        description: |
+          A dictionary which defines the template/location as well as the form which the template is input.
+          If any keys use a space, it must be replaced with an underscore.
         additionalProperties: false
         properties:
           file:
             type: string
             description: A .jinja file containing the template
           column:
             type: string
@@ -205,14 +209,23 @@
     
     if input:
         input = input[0]
         input_list = df[input]
     else:
         input_list = df.to_dict(orient='records')
 
+    # Replace any spaces in keys with underscores
+    input_list = [
+        {
+            key.replace(' ', '_'): val
+            for key, val in row.items()
+        }
+        for row in input_list
+    ]
+
     if len(template) > 1:
         raise Exception('Template must have only one key specified')
 
     # Template input as a file
     if 'file' in template:
         environment = _Environment(loader=_FileSystemLoader(''),trim_blocks=True, lstrip_blocks=True)
         desc_template = environment.get_template(template['file'])
```

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/extract.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 import re as _re
 from collections import OrderedDict as _OrderedDict
 import pandas as _pd
 from .. import extract as _extract
 from .. import format as _format
 
 
-def address(df: _pd.DataFrame, input: str, output: str, dataType: str) -> _pd.DataFrame:
+def address(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], dataType: str) -> _pd.DataFrame:
     """
     type: object
     description: Extract parts of addresses. Requires WrangleWorks Account.
     additionalProperties: false
     required:
       - input
       - output
+      - dataType
     properties:
       input:
         type:
           - string
           - array
         description: Name of the input column.
       output:
@@ -50,15 +51,15 @@
   
     for input_column, output_column in zip(input, output):
         df[output_column] = _extract.address(df[input_column].astype(str).tolist(), dataType)
   
     return df
 
 
-def attributes(df: _pd.DataFrame, input: str, output: str, responseContent: str = 'span', attribute_type: str = None, desired_unit: str = None, bound: str = 'mid') -> _pd.DataFrame:
+def attributes(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], responseContent: str = 'span', attribute_type: str = None, desired_unit: str = None, bound: str = 'mid') -> _pd.DataFrame:
     """
     type: object
     description: Extract numeric attributes from the input such as weights or lengths. Requires WrangleWorks Account.
     additionalProperties: false
     required:
       - input
       - output
@@ -134,15 +135,15 @@
             desired_unit,
             bound
         )
         
     return df
 
 
-def brackets(df: _pd.DataFrame, input: str, output: str) -> _pd.DataFrame:
+def brackets(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
     description: Extract text properties in brackets from the input
     additionalProperties: false
     required:
       - input
       - output
@@ -213,70 +214,77 @@
         # Loop through and apply for all columns
         for input_column, output_column in zip(input, output):
             df[output_column] = _extract.codes(df[input_column].astype(str).tolist())
 
     return df
 
 
-def custom(df: _pd.DataFrame, input: list, output: _Union[str, list], model_id: _Union[str, list], use_labels: bool = False) -> _pd.DataFrame:
+def custom(df: _pd.DataFrame, input: _Union[str, list], model_id: _Union[str, list], output: _Union[str, list] = None, use_labels: bool = False, first_element: bool = False) -> _pd.DataFrame:
     """
     type: object
     description: Extract data from the input using a DIY or bespoke extraction wrangle. Requires WrangleWorks Account and Subscription.
-    additionalProperties: true
+    additionalProperties: false
     required:
       - input
-      - output
       - model_id
     properties:
       input:
         type:
           - string
           - array
         description: Name or list of input columns.
       output:
         type:
           - string
           - array
         description: Name or list of output columns
       model_id:
-        type: string
+        type:
+          - string
+          - array
         description: The ID of the wrangle to use
+      use_labels:
+        type: boolean
+        description: Use Labels in the extract output {label: value}
+      first_element:
+        type: boolean
+        description: Get the first element from results
     """
-    if not output:
-        output = input
-
-    if not isinstance(output, list):
-        output = [output]
-
-    if not isinstance(model_id, list):
-        # If a list of inputs is provided, ensure the list of outputs is the same length
-        if len(input) != len(output):
-            if len(output) == 1:
-                df[output[0]] = _extract.custom(_format.concatenate(df[input].astype(str).values.tolist(), ' '), model_id=model_id)
-            else:
-                raise ValueError('If providing a list of inputs, a corresponding list of outputs must also be provided.')
-        else:
-            for input_column, output_column in zip(input, output):
-                df[output_column] = _extract.custom(df[input_column].astype(str).tolist(), model_id=model_id)
-                
-    # Multiple different custom wrangles at the same time
-    else:
-        for in_col, out_col, mod_id in zip(input, output, model_id):
-            df[out_col] = _extract.custom(df[in_col].astype(str).tolist(),model_id=mod_id)
+    if output is None: output = input
     
-    if use_labels:
-        if len(output) > 1:
-            raise ValueError("'use_labels' can only be used with a single output")
-        
-        output = output[0]
+    # If a string provided, convert to list
+    if not isinstance(input, list): input = [input]
+    if not isinstance(output, list): output = [output]
+    if not isinstance(model_id, list): model_id = [model_id]
+    
+    if len(input) == len(output) and len(model_id) == 1:
+        # if one model_id, then use that model for all columns inputs and outputs
+        model_id = [model_id[0] for _ in range(len(input))]
+        for in_col, out_col, model in zip(input, output, model_id):
+            df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element)
+    
+    elif len(input) > 1 and len(output) == 1 and len(model_id) == 1:
+        # if there are multiple inputs and one output and one model_id. concatenate the inputs
+        df[output[0]] = _extract.custom(_format.concatenate(df[input].astype(str).values.tolist(), ' '), model_id=model_id, first_element=first_element)
+    
+    else:
+        # Iterate through the inputs, outputs and model_ids
+        for in_col, out_col, model in zip(input, output, model_id):
+            df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element)
 
+    # if use_labels is true and output is only one column
+    if (use_labels and len(output) == 1):
+        
+        # if first_element is checked, then the output must be converted to lists
+        if first_element: df[output[0]] = [[x] for x in df[output[0]]]
+        
         # Run the custom dictionary maker after normal operation from extract
         # This will be triggered only if a parameter is set
         result = []
-        for out_row in df[output]:
+        for out_row in df[output[0]]:
         
             dict_output = {'Unlabeled': []}
             # Iterating over the results
             for item in out_row:
                 
                 try:
                     item = item.strip()
@@ -288,23 +296,27 @@
                 except:
                     dict_output['Unlabeled'].append(item)
                     
             tmp_unlabeled = dict_output['Unlabeled']
             del dict_output['Unlabeled']
             output_dict = _OrderedDict(dict_output)
             output_dict['Unlabeled'] = tmp_unlabeled
-                
+            
+            # check if the Unlabeled key is empty if yes, delete the key
+            if len(output_dict['Unlabeled']) == 0:
+                del output_dict['Unlabeled']
+                            
             result.append(dict(output_dict))
             
-        df[output] = result
+        df[output[0]] = result
         
     return df
 
 
-def date_properties(df: _pd.DataFrame, input: _pd.Timestamp, property: str, output: str = None) -> _pd.DataFrame:
+def date_properties(df: _pd.DataFrame, input: _pd.Timestamp, property: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Extract date properties from a date (day, month, year, etc...)
     additionalProperties: false
     required:
       - input
       - property
@@ -372,15 +384,14 @@
     type: object
     description: Extract date range frequency from two dates
     additionalProperties: false
     required:
       - start_time
       - end_time
       - output
-      - range
     properties:
       start_time:
         type: string
         description: Name of the start date column
       end_time:
         type: string
         description: Name of the end date column
@@ -453,15 +464,14 @@
 def html(df: _pd.DataFrame, input: _Union[str, list], data_type: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Extract elements from strings containing html. Requires WrangleWorks Account.
     additionalProperties: false
     required:
       - input
-      - output
       - data_type
     properties:
       input:
         type:
           - string
           - array
         description: Name or list of input columns.
@@ -548,24 +558,25 @@
     """
     type: object
     description: Extract single values using regex
     additionalProperties: false
     required:
       - input
       - output
+      - find
     properties:
       input:
         type: string
         description: Name of the input column.
     output:
       type: string
       description: Name of the output column.
-      find:
-        type: string
-        description: Pattern to find using regex
+    find:
+      type: string
+      description: Pattern to find using regex
     """
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
```

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/format.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 Functions to re-format data
 """
 from typing import Union as _Union
 import pandas as _pd
 from .. import format as _format
 
 
-def dates(df: _pd.DataFrame, input: str, format: str, output: str = None) -> _pd.DataFrame:
+def dates(df: _pd.DataFrame, input: _Union[str, list], format: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Format a date
     additionalProperties: false
     required:
       - input
       - format
     properties:
       input:
         type:
           - string
+          - array
         description: Name of the input column
       output:
         type:
           - string
+          - array
         description: Name of the output column
       format:
         type:
           - string
         description: String pattern to format date
     """
     # If output is not specified, overwrite input columns in place
@@ -43,15 +45,15 @@
     for input_column, output_column in zip(input, output):
         # convert the column to timestamp type and format date
         df[output_column] = _pd.to_datetime(df[input_column]).dt.strftime(format)
     
     return df
     
     
-def pad(df: _pd.DataFrame, input: _Union[str, list], pad_length: int, side: str, char: str, output =  None) -> _pd.DataFrame:
+def pad(df: _pd.DataFrame, input: _Union[str, list], pad_length: int, side: str, char: _Union[str, int], output: _Union[str, list] =  None) -> _pd.DataFrame:
     """
     type: object
     description: Pad a string to a fixed length
     additionalProperties: false
     required:
       - input
       - pad_length
@@ -72,17 +74,22 @@
         type:
           - number
         description: Length for the output
       side:
         type:
           - string
         description:  Side from which to fill resulting string
+        enum:
+          - left
+          - right
+          - both
       char:
         type:
           - string
+          - int
         description: The character to pad the input with
   """
     char = str(char)
     # If the output is not specified, overwrite input columns in place
     if output is None: output = input
     
     # If the input is a string
@@ -95,15 +102,15 @@
   
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].astype(str).str.pad(pad_length, side, char)
     
     return df
 
 
-def prefix(df: _pd.DataFrame, input: str, value: str, output: str = None) -> _pd.DataFrame:
+def prefix(df: _pd.DataFrame, input: _Union[str, list], value: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Add a prefix to a column
     additionalProperties: false
     required:
       - input
       - value
@@ -137,27 +144,31 @@
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = value + df[input_column].astype(str)
 
     return df
 
 
-def remove_duplicates(df: _pd.DataFrame, input: str, output: str = None) -> _pd.DataFrame:
+def remove_duplicates(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Remove duplicates from a list. Preserves input order.
     additionalProperties: false
     required:
       - input
     properties:
       input:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the input column
       output:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the output column
     """
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
@@ -170,15 +181,15 @@
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] =  _format.remove_duplicates(df[input_column].values.tolist())
 
     return df
 
 
-def suffix(df: _pd.DataFrame, input: str, value: str, output: str = None) -> _pd.DataFrame:
+def suffix(df: _pd.DataFrame, input: _Union[str, list], value: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Add a suffix to a column
     additionalProperties: false
     required:
         - input
         - value
@@ -211,15 +222,15 @@
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].astype(str) + value
   
     return df
 
 
-def trim(df: _pd.DataFrame, input: str, output: str = None) -> _pd.DataFrame:
+def trim(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Remove excess whitespace at the start and end of text.
     additionalProperties: false
     required:
       - input
     properties:
```

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/main.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import types as _types
 import logging as _logging
 from typing import Union as _Union
 import sqlite3 as _sqlite3
 import re as _re
 import numexpr as _ne
+import requests as _requests
 import pandas as _pd
 import wrangles as _wrangles
 import yaml as _yaml
 from ..classify import classify as _classify
 from ..standardize import standardize as _standardize
 from ..translate import translate as _translate
 from .. import extract as _extract
@@ -68,16 +69,14 @@
 def date_calculator(df: _pd.DataFrame, input: _Union[str, _pd.Timestamp], operation: str = 'add', output: _Union[str, _pd.Timestamp] = None, time_unit: str = None, time_value: float = None) -> _pd.DataFrame:
     """
     type: object
     description: Add or Subtract time from a date
     additionalProperties: false
     required:
       - input
-      - operation
-      - kwargs
     properties:
       input:
         type: string
         description: Name of the dates column
       operation:
         type: string
         description: Date operation
@@ -284,15 +283,81 @@
             df = df[~df[input_column].str.contains(not_contains, na=False, **kwargs)]
         
         if is_null == True:
             df = df[df[input_column].isnull()]
         
         if is_null == False:
             df = df[df[input_column].notnull()]
-     
+
+    df = df.reset_index(drop=True)
+
+    return df
+
+
+def huggingface(
+    df: _pd.DataFrame,
+    input: _Union[str, list],
+    api_token: str,
+    model: str,
+    output: _Union[str, list] = None,
+    parameters = None
+):
+    """
+    type: object
+    description: Use a model from huggingface
+    required:
+      - input
+      - api_token
+      - model
+    properties:
+      input:
+        type:
+          - string
+          - array
+        description: Name of the input column.
+      output:
+        type:
+          - string
+          - array
+        description: >
+          Name of the output column.
+          If not provided, will overwrite the input column
+      model:
+        type: string
+        description: Name of the model to use. e.g. facebook/bart-large-cnn
+      api_token:
+        type: string
+        description: Huggingface API Token
+      parameters:
+        type: object
+        description: Optionally, provide additional parameters to define the model behaviour
+    """
+    if not output: output = input
+    if not isinstance(output, list): output = [output]
+    if not isinstance(input, list): input = [input]
+
+    json_base = {}
+    if parameters:
+        json_base['parameters'] = parameters
+
+    for input_col, output_col in zip(input, output):
+        df[output_col] = [
+            _requests.post(
+                f"https://api-inference.huggingface.co/models/{model}",
+                headers={
+                    "Authorization": f"Bearer {api_token}"
+                },
+                json={
+                    **json_base,
+                    **{"inputs": row}
+                }
+            ).json()
+            for row in df[input_col].values
+        ]
+
     return df
 
 
 def log(df: _pd.DataFrame, columns: list = None, write: list = None):
     """
     type: object
     description: Log the current status of the dataframe.
@@ -416,34 +481,35 @@
         df = df_temp
     else:
         df = original_df.merge(df_temp[output_columns], how='left', left_index=True, right_index=True)
         
     return df
 
 
-def remove_words(df: _pd.DataFrame, input: str, to_remove: str, output: str = None, tokenize_to_remove: bool = False, ignore_case: bool = True) -> _pd.DataFrame:
+def remove_words(df: _pd.DataFrame, input: _Union[str, list], to_remove: _Union[str, list], output: _Union[str, list] = None, tokenize_to_remove: bool = False, ignore_case: bool = True) -> _pd.DataFrame:
     """
     type: object
     description: Remove all the elements that occur in one list from another.
     additionalProperties: false
     required:
       - input
       - to_remove
-      - output
     properties:
       input:
         type: 
           - string
           - array
         description: Name of column to remove words from
       to_remove:
         type: array
         description: Column or list of columns with a list of words to be removed
       output:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the output columns
       tokenize_to_remove:
         type: boolean
         description: Tokenize all to_remove inputs
       ignore_case:
         type: boolean
         description: Ignore input and to_remove case
@@ -504,22 +570,21 @@
         
         # Otherwise create a dict from input and output columns
         rename_dict = dict(zip(input, output))
 
     return df.rename(columns=rename_dict)
 
 
-def replace(df: _pd.DataFrame, input: str, output: str, find: str, replace: str) -> _pd.DataFrame:
+def replace(df: _pd.DataFrame, input: _Union[str, list], find: str, replace: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Quick find and replace for simple values. Can use regex in the find field.
     additionalProperties: false
     required:
       - input
-      - output
       - find
       - replace
     properties:
       input:
         type:
           - string
           - array
@@ -625,22 +690,14 @@
           - array
         description: Name or list of output columns
       model_id:
         type:
           - string
           - array
         description: The ID of the wrangle to use (do not include 'find' and 'replace')
-      find:
-        type:
-          - string
-        description: Pattern to find using regex (do not include model_id)
-      replace:
-        type:
-          - string
-        description: Value to replace the pattern found (do not include model_id)
     """
     # If user hasn't specified an output column, overwrite the input
     if output is None: output = input
 
     # If user provides a single string, convert all the arguments to lists for consistency
     if isinstance(input, str): input = [input]
     if isinstance(output, str): output = [output]
@@ -650,15 +707,15 @@
         for input_column, output_column in zip(input, output):
             df[output_column] = _standardize(df[input_column].astype(str).tolist(), model)
 
 
     return df
 
 
-def translate(df: _pd.DataFrame, input: str, output: str, target_language: str, source_language: str = 'AUTO', case: str = None) -> _pd.DataFrame:
+def translate(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], target_language: str, source_language: str = 'AUTO', case: str = None) -> _pd.DataFrame:
     """
     type: object
     description: Translate the input to a different language. Requires WrangleWorks Account and DeepL API Key (A free account for up to 500,000 characters per month is available).
     additionalProperties: false
     required:
       - input
       - output
@@ -670,14 +727,22 @@
           - array
         description: Name of the column to translate
       output:
         type:
           - string
           - array
         description: Name of the output column
+      case:
+        type: string
+        description: Allow changing the case of the input prior to translation. lower, upper or title
+        enum:
+          - lower
+          - upper
+          - title
+          - sentence
       target_language:
         type: string
         description: Code of the language to translate to
         enum:
           - Bulgarian
           - Chinese
           - Czech
@@ -731,79 +796,14 @@
           - Russian
           - Slovak
           - Slovenian
           - Spanish
           - Swedish
     """
     
-    # Convert Language to DeepL Code
-    source_dict = [
-        { 'key': 'AUTO', 'text': 'Auto'},
-        { 'key': 'BG', 'text': 'Bulgarian' },
-        { 'key': 'ZH', 'text': 'Chinese' },
-        { 'key': 'CS', 'text': 'Czech' },
-        { 'key': 'DA', 'text': 'Danish' },
-        { 'key': 'NL', 'text': 'Dutch' },
-        { 'key': 'EN', 'text': 'English' },
-        { 'key': 'ET', 'text': 'Estonian' },
-        { 'key': 'FI', 'text': 'Finnish' },
-        { 'key': 'FR', 'text': 'French' },
-        { 'key': 'DE', 'text': 'German' },
-        { 'key': 'EL', 'text': 'Greek' },
-        { 'key': 'HU', 'text': 'Hungarian' },
-        { 'key': 'IT', 'text': 'Italian' },
-        { 'key': 'JA', 'text': 'Japanese' },
-        { 'key': 'LV', 'text': 'Latvian' },
-        { 'key': 'LT', 'text': 'Lithuanian' },
-        { 'key': 'PL', 'text': 'Polish' },
-        { 'key': 'PT', 'text': 'Portuguese' },
-        { 'key': 'RO', 'text': 'Romanian' },
-        { 'key': 'RU', 'text': 'Russian' },
-        { 'key': 'SK', 'text': 'Slovak' },
-        { 'key': 'SL', 'text': 'Slovenian' },
-        { 'key': 'ES', 'text': 'Spanish' },
-        { 'key': 'SV', 'text': 'Swedish' },
-    ]
-    
-    target_dict = [
-        { 'key': 'BG', 'text': 'Bulgarian' },
-        { 'key': 'ZH', 'text': 'Chinese' },
-        { 'key': 'CS', 'text': 'Czech' },
-        { 'key': 'DA', 'text': 'Danish' },
-        { 'key': 'NL', 'text': 'Dutch' },
-        { 'key': 'EN-US', 'text': 'English (American)' },
-        { 'key': 'EN-GB', 'text': 'English (British)' },
-        { 'key': 'ET', 'text': 'Estonian' },
-        { 'key': 'FI', 'text': 'Finnish' },
-        { 'key': 'FR', 'text': 'French' },
-        { 'key': 'DE', 'text': 'German' },
-        { 'key': 'EL', 'text': 'Greek' },
-        { 'key': 'HU', 'text': 'Hungarian' },
-        { 'key': 'IT', 'text': 'Italian' },
-        { 'key': 'JA', 'text': 'Japanese' },
-        { 'key': 'LV', 'text': 'Latvian' },
-        { 'key': 'LT', 'text': 'Lithuanian' },
-        { 'key': 'PL', 'text': 'Polish' },
-        { 'key': 'PT-PT', 'text': 'Portuguese' },
-        { 'key': 'PT-BR', 'text': 'Portuguese (Brazilian)' },
-        { 'key': 'RO', 'text': 'Romanian' },
-        { 'key': 'RU', 'text': 'Russian' },
-        { 'key': 'SK', 'text': 'Slovak' },
-        { 'key': 'SL', 'text': 'Slovenian' },
-        { 'key': 'ES', 'text': 'Spanish' },
-        { 'key': 'SV', 'text': 'Swedish' },
-    ]
-    # Source Language code
-    try:
-        if target_language == 'English': target_language = 'English (British)'
-        source_language = [x['key'] for x in source_dict if x['text'] == source_language][0]
-        target_language = [x['key'] for x in target_dict if x['text'] == target_language][0]
-    except:
-        pass
-
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
```

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/merge.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     """
     type: object
     description: Concatenate a list of columns or a list within a single column.
     additionalProperties: false
     required:
       - input
       - output
-      - char
     properties:
       input:
         type: 
           - array
           - string
         description: Either a single column name or list of columns
       output:
@@ -71,15 +70,15 @@
     description: Take dictionaries in multiple columns and merge them to a single dictionary.
     additionalProperties: false
     required:
       - input
       - output
     properties:
       input:
-        type: object
+        type: array
         description: list of input columns
       output:
         type: string
         description: Name of the output column    
     """
     output_list = []
     for row in df[input].values.tolist():
```

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/select.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/select.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 def dictionary_element(df: _pd.DataFrame, input: _Union[str, list], element: str, output: _Union[str, list] = None,) -> _pd.DataFrame:
     """
     type: object
     description: Select a named element of a dictionary.
     additionalProperties: false
     required:
       - input
-      - output
       - element
     properties:
       input:
         type: string
         description: Name of the input column
       output:
         type: string
@@ -37,15 +36,15 @@
     
     for in_col, out_col in zip(input, output):
         df[out_col] = _select.dict_element(df[in_col].tolist(), element)
     
     return df
 
 
-def highest_confidence(df: _pd.DataFrame, input: list, output: str) -> _pd.DataFrame:
+def highest_confidence(df: _pd.DataFrame, input: list, output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
     description: Select the option with the highest confidence from multiple columns. Inputs are expected to be of the form [<<value>>, <<confidence_score>>].
     additionalProperties: false
     required:
       - input
       - output
@@ -104,22 +103,24 @@
 def list_element(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None, element: int = 0) -> _pd.DataFrame:
     """
     type: object
     description: Select a numbered element of a list (zero indexed).
     additionalProperties: false
     required:
       - input
-      - output
-      - element
     properties:
       input:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the input column
       output:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the output column
       element:
         type: integer
         description: The numbered element of the list to select. Starts from zero
     """
     if output is None: output = input
```

### Comparing `wrangles-1.1.0/wrangles/recipe_wrangles/split.py` & `wrangles-1.2.0/wrangles/recipe_wrangles/split.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         description: Name of the column to be split
     """
     exploded_df = _pd.json_normalize(df[input], max_level=1).fillna('')
     df[exploded_df.columns] = exploded_df
     return df
 
     
-def list(df: _pd.DataFrame, input: str, output: list) -> _pd.DataFrame:
+def list(df: _pd.DataFrame, input: str, output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
     description: Split a list in a single column to multiple columns.
     additionalProperties: false
     required:
       - input
       - output
@@ -142,30 +142,32 @@
     elif isinstance(element, str):
         slice_values = [int(x) for x in element.split(':')]
         df[output] = df[output].apply(lambda x: x[slice_values[0]:slice_values[1]])
         
     return df
 
 
-def tokenize(df: _pd.DataFrame, input: str, output: str = None) -> _pd.DataFrame:
+def tokenize(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Tokenize elements in a list into individual tokens.
     additionalProperties: false
     required:
       - input
       - output
     properties:
       input:
         type:
           - string
           - array
         description: list in column to split
       output:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the output column
     """
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, _list): input = [input]
     if not isinstance(output, _list): output = [output]
```

### Comparing `wrangles-1.1.0/wrangles/select.py` & `wrangles-1.2.0/wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/standardize.py` & `wrangles-1.2.0/wrangles/standardize.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.1.0/wrangles/train.py` & `wrangles-1.2.0/wrangles/train.py`

 * *Files identical despite different names*

