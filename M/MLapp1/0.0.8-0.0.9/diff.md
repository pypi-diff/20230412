# Comparing `tmp/MLapp1-0.0.8.tar.gz` & `tmp/MLapp1-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLapp1-0.0.8.tar", last modified: Wed Apr 12 16:26:56 2023, max compression
+gzip compressed data, was "MLapp1-0.0.9.tar", last modified: Wed Apr 12 16:28:29 2023, max compression
```

## Comparing `MLapp1-0.0.8.tar` & `MLapp1-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.168928 MLapp1-0.0.8/
--rw-------   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.8/LICENSE.toml
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:26:56.169009 MLapp1-0.0.8/PKG-INFO
--rw-------   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.8/README.md
--rw-------   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.8/pyproject.toml
--rw-------   0 akshay     (503) staff       (20)      857 2023-04-12 16:26:56.169455 MLapp1-0.0.8/setup.cfg
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.159786 MLapp1-0.0.8/src/
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.164239 MLapp1-0.0.8/src/MLapp/
--rw-------   0 akshay     (503) staff       (20)     1035 2022-09-12 15:07:15.000000 MLapp1-0.0.8/src/MLapp/README.txt
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.167605 MLapp1-0.0.8/src/MLapp/UI/
--rw-------   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.8/src/MLapp/UI/__init__.py
--rw-------   0 akshay     (503) staff       (20)    26863 2023-04-12 16:23:12.000000 MLapp1-0.0.8/src/MLapp/UI/autoML.py
--rw-------   0 akshay     (503) staff       (20)    61901 2023-04-12 16:24:56.000000 MLapp1-0.0.8/src/MLapp/UI/classifcationAlgo.py
--rw-------   0 akshay     (503) staff       (20)    34120 2022-07-29 11:43:58.000000 MLapp1-0.0.8/src/MLapp/UI/componentIDs.py
--rw-------   0 akshay     (503) staff       (20)    28666 2023-04-12 16:24:48.000000 MLapp1-0.0.8/src/MLapp/UI/dataSampling.py
--rw-------   0 akshay     (503) staff       (20)    21244 2023-04-12 16:23:57.000000 MLapp1-0.0.8/src/MLapp/UI/featureSelection.py
--rwxr-xr-x   0 akshay     (503) staff       (20)     4731 2022-07-19 11:00:49.000000 MLapp1-0.0.8/src/MLapp/UI/layouts.py
--rw-------   0 akshay     (503) staff       (20)    23240 2023-04-12 16:23:20.000000 MLapp1-0.0.8/src/MLapp/UI/modelEvaluation.py
--rw-------   0 akshay     (503) staff       (20)    25583 2023-04-12 16:22:45.000000 MLapp1-0.0.8/src/MLapp/UI/result.py
--rw-------   0 akshay     (503) staff       (20)    19094 2023-04-12 16:23:48.000000 MLapp1-0.0.8/src/MLapp/UI/scaling.py
--rw-------   0 akshay     (503) staff       (20)     5565 2023-04-12 16:23:39.000000 MLapp1-0.0.8/src/MLapp/UI/submit.py
--rwxr-xr-x   0 akshay     (503) staff       (20)    13628 2023-04-12 16:23:03.000000 MLapp1-0.0.8/src/MLapp/UI/uploadInput.py
--rw-r--r--   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.8/src/MLapp/__init__.py
--rwxr-xr-x   0 akshay     (503) staff       (20)      485 2023-04-12 08:49:57.000000 MLapp1-0.0.8/src/MLapp/app.py
--rw-------   0 akshay     (503) staff       (20)     2558 2023-04-12 16:16:15.000000 MLapp1-0.0.8/src/MLapp/generateScript.py
--rw-------   0 akshay     (503) staff       (20)    45927 2023-04-12 16:25:43.000000 MLapp1-0.0.8/src/MLapp/helperFunctions.py
--rw-------   0 akshay     (503) staff       (20)      319 2023-04-12 16:12:15.000000 MLapp1-0.0.8/src/MLapp/launcher.py
--rwxr-xr-x   0 akshay     (503) staff       (20)     3861 2023-04-12 16:15:34.000000 MLapp1-0.0.8/src/MLapp/main.py
--rw-------   0 akshay     (503) staff       (20)    13361 2022-09-13 11:45:53.000000 MLapp1-0.0.8/src/MLapp/scriptTemplate.py
--rw-------   0 akshay     (503) staff       (20)    12723 2022-09-22 10:44:47.000000 MLapp1-0.0.8/src/MLapp/subScript.py
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.168766 MLapp1-0.0.8/src/MLapp1.egg-info/
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)      751 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/requires.txt
--rw-r--r--   0 akshay     (503) staff       (20)        6 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/top_level.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:28:29.140278 MLapp1-0.0.9/
+-rw-------   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.9/LICENSE.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:28:29.140512 MLapp1-0.0.9/PKG-INFO
+-rw-------   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.9/README.md
+-rw-------   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.9/pyproject.toml
+-rw-------   0 akshay     (503) staff       (20)      857 2023-04-12 16:28:29.141610 MLapp1-0.0.9/setup.cfg
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:28:29.123003 MLapp1-0.0.9/src/
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:28:29.129855 MLapp1-0.0.9/src/MLapp/
+-rw-------   0 akshay     (503) staff       (20)     1035 2022-09-12 15:07:15.000000 MLapp1-0.0.9/src/MLapp/README.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:28:29.136934 MLapp1-0.0.9/src/MLapp/UI/
+-rw-------   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.9/src/MLapp/UI/__init__.py
+-rw-------   0 akshay     (503) staff       (20)    26863 2023-04-12 16:23:12.000000 MLapp1-0.0.9/src/MLapp/UI/autoML.py
+-rw-------   0 akshay     (503) staff       (20)    61901 2023-04-12 16:24:56.000000 MLapp1-0.0.9/src/MLapp/UI/classifcationAlgo.py
+-rw-------   0 akshay     (503) staff       (20)    34120 2022-07-29 11:43:58.000000 MLapp1-0.0.9/src/MLapp/UI/componentIDs.py
+-rw-------   0 akshay     (503) staff       (20)    28666 2023-04-12 16:24:48.000000 MLapp1-0.0.9/src/MLapp/UI/dataSampling.py
+-rw-------   0 akshay     (503) staff       (20)    21244 2023-04-12 16:23:57.000000 MLapp1-0.0.9/src/MLapp/UI/featureSelection.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)     4732 2023-04-12 16:27:58.000000 MLapp1-0.0.9/src/MLapp/UI/layouts.py
+-rw-------   0 akshay     (503) staff       (20)    23240 2023-04-12 16:23:20.000000 MLapp1-0.0.9/src/MLapp/UI/modelEvaluation.py
+-rw-------   0 akshay     (503) staff       (20)    25583 2023-04-12 16:22:45.000000 MLapp1-0.0.9/src/MLapp/UI/result.py
+-rw-------   0 akshay     (503) staff       (20)    19094 2023-04-12 16:23:48.000000 MLapp1-0.0.9/src/MLapp/UI/scaling.py
+-rw-------   0 akshay     (503) staff       (20)     5565 2023-04-12 16:23:39.000000 MLapp1-0.0.9/src/MLapp/UI/submit.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)    13628 2023-04-12 16:23:03.000000 MLapp1-0.0.9/src/MLapp/UI/uploadInput.py
+-rw-r--r--   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.9/src/MLapp/__init__.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)      485 2023-04-12 08:49:57.000000 MLapp1-0.0.9/src/MLapp/app.py
+-rw-------   0 akshay     (503) staff       (20)     2558 2023-04-12 16:16:15.000000 MLapp1-0.0.9/src/MLapp/generateScript.py
+-rw-------   0 akshay     (503) staff       (20)    45927 2023-04-12 16:25:43.000000 MLapp1-0.0.9/src/MLapp/helperFunctions.py
+-rw-------   0 akshay     (503) staff       (20)      319 2023-04-12 16:12:15.000000 MLapp1-0.0.9/src/MLapp/launcher.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)     3861 2023-04-12 16:15:34.000000 MLapp1-0.0.9/src/MLapp/main.py
+-rw-------   0 akshay     (503) staff       (20)    13361 2022-09-13 11:45:53.000000 MLapp1-0.0.9/src/MLapp/scriptTemplate.py
+-rw-------   0 akshay     (503) staff       (20)    12723 2022-09-22 10:44:47.000000 MLapp1-0.0.9/src/MLapp/subScript.py
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:28:29.139822 MLapp1-0.0.9/src/MLapp1.egg-info/
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:28:29.000000 MLapp1-0.0.9/src/MLapp1.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)      751 2023-04-12 16:28:29.000000 MLapp1-0.0.9/src/MLapp1.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 16:28:29.000000 MLapp1-0.0.9/src/MLapp1.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 16:28:29.000000 MLapp1-0.0.9/src/MLapp1.egg-info/requires.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        6 2023-04-12 16:28:29.000000 MLapp1-0.0.9/src/MLapp1.egg-info/top_level.txt
```

### Comparing `MLapp1-0.0.8/LICENSE.toml` & `MLapp1-0.0.9/LICENSE.toml`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/setup.cfg` & `MLapp1-0.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MLapp1
-version = 0.0.8
+version = 0.0.9
 author = Akshay
 author_email = akshaysuhag1996@gmail.com
 description = "MLapp"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FunctionalUrology/
 project_urls =
```

### Comparing `MLapp1-0.0.8/src/MLapp/README.txt` & `MLapp1-0.0.9/src/MLapp/README.txt`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/autoML.py` & `MLapp1-0.0.9/src/MLapp/UI/autoML.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/classifcationAlgo.py` & `MLapp1-0.0.9/src/MLapp/UI/classifcationAlgo.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/componentIDs.py` & `MLapp1-0.0.9/src/MLapp/UI/componentIDs.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/dataSampling.py` & `MLapp1-0.0.9/src/MLapp/UI/dataSampling.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/featureSelection.py` & `MLapp1-0.0.9/src/MLapp/UI/featureSelection.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/layouts.py` & `MLapp1-0.0.9/src/MLapp/UI/layouts.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on Thu Sep  9 17:17:20 2021
 
 @author: akshay
 """
 
 from dash import dcc,html
 import dash_bootstrap_components as dbc
-from app import app
+from .app import app
 from dash.dependencies import Input, Output,State
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! 
 # =============================================================================
 # preprocessing data tab
 # 
 # =============================================================================
```

### Comparing `MLapp1-0.0.8/src/MLapp/UI/modelEvaluation.py` & `MLapp1-0.0.9/src/MLapp/UI/modelEvaluation.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/result.py` & `MLapp1-0.0.9/src/MLapp/UI/result.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/scaling.py` & `MLapp1-0.0.9/src/MLapp/UI/scaling.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/submit.py` & `MLapp1-0.0.9/src/MLapp/UI/submit.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/UI/uploadInput.py` & `MLapp1-0.0.9/src/MLapp/UI/uploadInput.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/generateScript.py` & `MLapp1-0.0.9/src/MLapp/generateScript.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/helperFunctions.py` & `MLapp1-0.0.9/src/MLapp/helperFunctions.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/main.py` & `MLapp1-0.0.9/src/MLapp/main.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/scriptTemplate.py` & `MLapp1-0.0.9/src/MLapp/scriptTemplate.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp/subScript.py` & `MLapp1-0.0.9/src/MLapp/subScript.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.8/src/MLapp1.egg-info/SOURCES.txt` & `MLapp1-0.0.9/src/MLapp1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

