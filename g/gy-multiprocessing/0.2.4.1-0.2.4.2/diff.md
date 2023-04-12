# Comparing `tmp/gy_multiprocessing-0.2.4.1.tar.gz` & `tmp/gy_multiprocessing-0.2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gy_multiprocessing-0.2.4.1.tar", last modified: Wed Apr 12 09:25:36 2023, max compression
+gzip compressed data, was "gy_multiprocessing-0.2.4.2.tar", last modified: Wed Apr 12 10:20:43 2023, max compression
```

## Comparing `gy_multiprocessing-0.2.4.1.tar` & `gy_multiprocessing-0.2.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.506688 gy_multiprocessing-0.2.4.1/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6427 2023-04-12 09:25:36.506567 gy_multiprocessing-0.2.4.1/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6007 2023-04-12 09:25:12.000000 gy_multiprocessing-0.2.4.1/README.md
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.505523 gy_multiprocessing-0.2.4.1/gy_multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)      138 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/__init__.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.506183 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)       61 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     7090 2023-04-12 09:23:13.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/multi_process.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.506401 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/
--rw-r--r--   0 guangyuhe   (501) staff       (20)       59 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/multi_thread.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.505954 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6427 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/top_level.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-04-12 09:25:36.506723 gy_multiprocessing-0.2.4.1/setup.cfg
--rw-r--r--   0 guangyuhe   (501) staff       (20)      792 2023-04-12 09:24:19.000000 gy_multiprocessing-0.2.4.1/setup.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543997 gy_multiprocessing-0.2.4.2/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6438 2023-04-12 10:20:43.543877 gy_multiprocessing-0.2.4.2/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6018 2023-04-12 10:20:23.000000 gy_multiprocessing-0.2.4.2/README.md
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.542547 gy_multiprocessing-0.2.4.2/gy_multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      138 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/__init__.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543430 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       61 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     7090 2023-04-12 09:23:13.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/multi_process.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543688 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       59 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/multi_thread.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543168 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6438 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/top_level.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-04-12 10:20:43.544032 gy_multiprocessing-0.2.4.2/setup.cfg
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      826 2023-04-12 10:20:16.000000 gy_multiprocessing-0.2.4.2/setup.py
```

### Comparing `gy_multiprocessing-0.2.4.1/PKG-INFO` & `gy_multiprocessing-0.2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gy_multiprocessing
-Version: 0.2.4.1
+Version: 0.2.4.2
 Summary: Run function in multiple processes
 Home-page: https://github.com/guangyu-he/gy-multiprocessing
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -228,15 +228,15 @@
 
 #### feature
 
 - a silent mode is added to multiprocessing which is possible not showing messages in console
 - solved multiprocessing not going to the end when there are internal error exceptions in input function
 - solved multiprocessing not going to the end when there are missing queue.put() method in input function
 
-### v0.2.4.1
+### v0.2.4.1 & v0.2.4.2
 
 #### bug fix
 
 - fixed an issue from readme long desc causing installation error
 
 #### improvement
```

### Comparing `gy_multiprocessing-0.2.4.1/README.md` & `gy_multiprocessing-0.2.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
 #### feature
 
 - a silent mode is added to multiprocessing which is possible not showing messages in console
 - solved multiprocessing not going to the end when there are internal error exceptions in input function
 - solved multiprocessing not going to the end when there are missing queue.put() method in input function
 
-### v0.2.4.1
+### v0.2.4.1 & v0.2.4.2
 
 #### bug fix
 
 - fixed an issue from readme long desc causing installation error
 
 #### improvement
```

### Comparing `gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/multi_process.py` & `gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/multi_process.py`

 * *Files identical despite different names*

### Comparing `gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/multi_thread.py` & `gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/multi_thread.py`

 * *Files identical despite different names*

### Comparing `gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/PKG-INFO` & `gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gy-multiprocessing
-Version: 0.2.4.1
+Version: 0.2.4.2
 Summary: Run function in multiple processes
 Home-page: https://github.com/guangyu-he/gy-multiprocessing
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -228,15 +228,15 @@
 
 #### feature
 
 - a silent mode is added to multiprocessing which is possible not showing messages in console
 - solved multiprocessing not going to the end when there are internal error exceptions in input function
 - solved multiprocessing not going to the end when there are missing queue.put() method in input function
 
-### v0.2.4.1
+### v0.2.4.1 & v0.2.4.2
 
 #### bug fix
 
 - fixed an issue from readme long desc causing installation error
 
 #### improvement
```

