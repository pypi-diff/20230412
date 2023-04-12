# Comparing `tmp/MLapp1-0.0.6.tar.gz` & `tmp/MLapp1-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLapp1-0.0.6.tar", last modified: Wed Apr 12 16:00:07 2023, max compression
+gzip compressed data, was "MLapp1-0.0.7.tar", last modified: Wed Apr 12 16:13:18 2023, max compression
```

## Comparing `MLapp1-0.0.6.tar` & `MLapp1-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:00:07.878664 MLapp1-0.0.6/
--rw-------   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.6/LICENSE.toml
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:00:07.878825 MLapp1-0.0.6/PKG-INFO
--rw-------   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.6/README.md
--rw-------   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.6/pyproject.toml
--rw-------   0 akshay     (503) staff       (20)      857 2023-04-12 16:00:07.879474 MLapp1-0.0.6/setup.cfg
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:00:07.857680 MLapp1-0.0.6/src/
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:00:07.866616 MLapp1-0.0.6/src/MLapp/
--rw-------   0 akshay     (503) staff       (20)      305 2023-04-12 10:51:26.000000 MLapp1-0.0.6/src/MLapp/MLapp.py
--rw-------   0 akshay     (503) staff       (20)     1035 2022-09-12 15:07:15.000000 MLapp1-0.0.6/src/MLapp/README.txt
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:00:07.876081 MLapp1-0.0.6/src/MLapp/UI/
--rw-------   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.6/src/MLapp/UI/__init__.py
--rw-------   0 akshay     (503) staff       (20)    26860 2022-09-22 15:11:18.000000 MLapp1-0.0.6/src/MLapp/UI/autoML.py
--rw-------   0 akshay     (503) staff       (20)    61898 2022-08-29 10:14:56.000000 MLapp1-0.0.6/src/MLapp/UI/classifcationAlgo.py
--rw-------   0 akshay     (503) staff       (20)    34120 2022-07-29 11:43:58.000000 MLapp1-0.0.6/src/MLapp/UI/componentIDs.py
--rw-------   0 akshay     (503) staff       (20)    28664 2022-08-29 10:15:24.000000 MLapp1-0.0.6/src/MLapp/UI/dataSampling.py
--rw-------   0 akshay     (503) staff       (20)    21241 2022-08-29 10:16:09.000000 MLapp1-0.0.6/src/MLapp/UI/featureSelection.py
--rwxr-xr-x   0 akshay     (503) staff       (20)     4731 2022-07-19 11:00:49.000000 MLapp1-0.0.6/src/MLapp/UI/layouts.py
--rw-------   0 akshay     (503) staff       (20)    23237 2022-09-12 14:20:10.000000 MLapp1-0.0.6/src/MLapp/UI/modelEvaluation.py
--rw-------   0 akshay     (503) staff       (20)    25582 2023-04-12 08:17:24.000000 MLapp1-0.0.6/src/MLapp/UI/result.py
--rw-------   0 akshay     (503) staff       (20)    19093 2022-08-29 10:16:51.000000 MLapp1-0.0.6/src/MLapp/UI/scaling.py
--rw-------   0 akshay     (503) staff       (20)     5562 2022-08-30 12:21:10.000000 MLapp1-0.0.6/src/MLapp/UI/submit.py
--rwxr-xr-x   0 akshay     (503) staff       (20)    13625 2022-09-22 15:55:06.000000 MLapp1-0.0.6/src/MLapp/UI/uploadInput.py
--rw-r--r--   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.6/src/MLapp/__init__.py
--rwxr-xr-x   0 akshay     (503) staff       (20)      485 2023-04-12 08:49:57.000000 MLapp1-0.0.6/src/MLapp/app.py
--rw-------   0 akshay     (503) staff       (20)     2556 2022-07-11 09:48:49.000000 MLapp1-0.0.6/src/MLapp/generateScript.py
--rw-------   0 akshay     (503) staff       (20)    45926 2023-04-12 07:46:30.000000 MLapp1-0.0.6/src/MLapp/helperFunctions.py
--rwxr-xr-x   0 akshay     (503) staff       (20)     3853 2023-04-12 08:51:43.000000 MLapp1-0.0.6/src/MLapp/main.py
--rw-------   0 akshay     (503) staff       (20)    13361 2022-09-13 11:45:53.000000 MLapp1-0.0.6/src/MLapp/scriptTemplate.py
--rw-------   0 akshay     (503) staff       (20)    12723 2022-09-22 10:44:47.000000 MLapp1-0.0.6/src/MLapp/subScript.py
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:00:07.878341 MLapp1-0.0.6/src/MLapp1.egg-info/
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:00:07.000000 MLapp1-0.0.6/src/MLapp1.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)      748 2023-04-12 16:00:07.000000 MLapp1-0.0.6/src/MLapp1.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 16:00:07.000000 MLapp1-0.0.6/src/MLapp1.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 16:00:07.000000 MLapp1-0.0.6/src/MLapp1.egg-info/requires.txt
--rw-r--r--   0 akshay     (503) staff       (20)        6 2023-04-12 16:00:07.000000 MLapp1-0.0.6/src/MLapp1.egg-info/top_level.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.253991 MLapp1-0.0.7/
+-rw-------   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.7/LICENSE.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:13:18.254119 MLapp1-0.0.7/PKG-INFO
+-rw-------   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.7/README.md
+-rw-------   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.7/pyproject.toml
+-rw-------   0 akshay     (503) staff       (20)      857 2023-04-12 16:13:18.254641 MLapp1-0.0.7/setup.cfg
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.243433 MLapp1-0.0.7/src/
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.248601 MLapp1-0.0.7/src/MLapp/
+-rw-------   0 akshay     (503) staff       (20)     1035 2022-09-12 15:07:15.000000 MLapp1-0.0.7/src/MLapp/README.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.252404 MLapp1-0.0.7/src/MLapp/UI/
+-rw-------   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.7/src/MLapp/UI/__init__.py
+-rw-------   0 akshay     (503) staff       (20)    26860 2022-09-22 15:11:18.000000 MLapp1-0.0.7/src/MLapp/UI/autoML.py
+-rw-------   0 akshay     (503) staff       (20)    61898 2022-08-29 10:14:56.000000 MLapp1-0.0.7/src/MLapp/UI/classifcationAlgo.py
+-rw-------   0 akshay     (503) staff       (20)    34120 2022-07-29 11:43:58.000000 MLapp1-0.0.7/src/MLapp/UI/componentIDs.py
+-rw-------   0 akshay     (503) staff       (20)    28664 2022-08-29 10:15:24.000000 MLapp1-0.0.7/src/MLapp/UI/dataSampling.py
+-rw-------   0 akshay     (503) staff       (20)    21241 2022-08-29 10:16:09.000000 MLapp1-0.0.7/src/MLapp/UI/featureSelection.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)     4731 2022-07-19 11:00:49.000000 MLapp1-0.0.7/src/MLapp/UI/layouts.py
+-rw-------   0 akshay     (503) staff       (20)    23237 2022-09-12 14:20:10.000000 MLapp1-0.0.7/src/MLapp/UI/modelEvaluation.py
+-rw-------   0 akshay     (503) staff       (20)    25582 2023-04-12 08:17:24.000000 MLapp1-0.0.7/src/MLapp/UI/result.py
+-rw-------   0 akshay     (503) staff       (20)    19093 2022-08-29 10:16:51.000000 MLapp1-0.0.7/src/MLapp/UI/scaling.py
+-rw-------   0 akshay     (503) staff       (20)     5562 2022-08-30 12:21:10.000000 MLapp1-0.0.7/src/MLapp/UI/submit.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)    13625 2022-09-22 15:55:06.000000 MLapp1-0.0.7/src/MLapp/UI/uploadInput.py
+-rw-r--r--   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.7/src/MLapp/__init__.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)      485 2023-04-12 08:49:57.000000 MLapp1-0.0.7/src/MLapp/app.py
+-rw-------   0 akshay     (503) staff       (20)     2556 2022-07-11 09:48:49.000000 MLapp1-0.0.7/src/MLapp/generateScript.py
+-rw-------   0 akshay     (503) staff       (20)    45926 2023-04-12 07:46:30.000000 MLapp1-0.0.7/src/MLapp/helperFunctions.py
+-rw-------   0 akshay     (503) staff       (20)      319 2023-04-12 16:12:15.000000 MLapp1-0.0.7/src/MLapp/launcher.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)     3853 2023-04-12 08:51:43.000000 MLapp1-0.0.7/src/MLapp/main.py
+-rw-------   0 akshay     (503) staff       (20)    13361 2022-09-13 11:45:53.000000 MLapp1-0.0.7/src/MLapp/scriptTemplate.py
+-rw-------   0 akshay     (503) staff       (20)    12723 2022-09-22 10:44:47.000000 MLapp1-0.0.7/src/MLapp/subScript.py
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.253765 MLapp1-0.0.7/src/MLapp1.egg-info/
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)      751 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/requires.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        6 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/top_level.txt
```

### Comparing `MLapp1-0.0.6/LICENSE.toml` & `MLapp1-0.0.7/LICENSE.toml`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/setup.cfg` & `MLapp1-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MLapp1
-version = 0.0.6
+version = 0.0.7
 author = Akshay
 author_email = akshaysuhag1996@gmail.com
 description = "MLapp"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FunctionalUrology/
 project_urls =
```

### Comparing `MLapp1-0.0.6/src/MLapp/README.txt` & `MLapp1-0.0.7/src/MLapp/README.txt`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/autoML.py` & `MLapp1-0.0.7/src/MLapp/UI/autoML.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/classifcationAlgo.py` & `MLapp1-0.0.7/src/MLapp/UI/classifcationAlgo.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/componentIDs.py` & `MLapp1-0.0.7/src/MLapp/UI/componentIDs.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/dataSampling.py` & `MLapp1-0.0.7/src/MLapp/UI/dataSampling.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/featureSelection.py` & `MLapp1-0.0.7/src/MLapp/UI/featureSelection.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/layouts.py` & `MLapp1-0.0.7/src/MLapp/UI/layouts.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/modelEvaluation.py` & `MLapp1-0.0.7/src/MLapp/UI/modelEvaluation.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/result.py` & `MLapp1-0.0.7/src/MLapp/UI/result.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/scaling.py` & `MLapp1-0.0.7/src/MLapp/UI/scaling.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/submit.py` & `MLapp1-0.0.7/src/MLapp/UI/submit.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/UI/uploadInput.py` & `MLapp1-0.0.7/src/MLapp/UI/uploadInput.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/generateScript.py` & `MLapp1-0.0.7/src/MLapp/generateScript.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/helperFunctions.py` & `MLapp1-0.0.7/src/MLapp/helperFunctions.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/main.py` & `MLapp1-0.0.7/src/MLapp/main.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/scriptTemplate.py` & `MLapp1-0.0.7/src/MLapp/scriptTemplate.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp/subScript.py` & `MLapp1-0.0.7/src/MLapp/subScript.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.6/src/MLapp1.egg-info/SOURCES.txt` & `MLapp1-0.0.7/src/MLapp1.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE.toml
 README.md
 pyproject.toml
 setup.cfg
-src/MLapp/MLapp.py
 src/MLapp/README.txt
 src/MLapp/__init__.py
 src/MLapp/app.py
 src/MLapp/generateScript.py
 src/MLapp/helperFunctions.py
+src/MLapp/launcher.py
 src/MLapp/main.py
 src/MLapp/scriptTemplate.py
 src/MLapp/subScript.py
 src/MLapp/UI/__init__.py
 src/MLapp/UI/autoML.py
 src/MLapp/UI/classifcationAlgo.py
 src/MLapp/UI/componentIDs.py
```

