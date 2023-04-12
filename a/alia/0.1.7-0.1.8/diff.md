# Comparing `tmp/alia-0.1.7.tar.gz` & `tmp/alia-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.1.7.tar", last modified: Wed Apr 12 16:24:04 2023, max compression
+gzip compressed data, was "alia-0.1.8.tar", last modified: Wed Apr 12 19:03:17 2023, max compression
```

## Comparing `alia-0.1.7.tar` & `alia-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 16:24:04.306466 alia-0.1.7/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.7/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 16:24:04.306137 alia-0.1.7/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.7/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 16:24:04.303892 alia-0.1.7/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.7/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.7/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.7/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    25525 2023-04-12 16:23:41.000000 alia-0.1.7/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 16:24:04.305750 alia-0.1.7/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-12 16:24:04.306564 alia-0.1.7/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-12 16:24:01.000000 alia-0.1.7/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 19:03:17.708780 alia-0.1.8/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.8/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 19:03:17.708439 alia-0.1.8/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.8/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 19:03:17.705915 alia-0.1.8/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.8/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.8/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.8/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    25979 2023-04-12 19:02:55.000000 alia-0.1.8/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 19:03:17.707835 alia-0.1.8/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-12 19:03:17.000000 alia-0.1.8/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-12 19:03:17.708866 alia-0.1.8/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-12 19:02:55.000000 alia-0.1.8/setup.py
```

### Comparing `alia-0.1.7/LICENSE` & `alia-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.1.7/alia/colors.py` & `alia-0.1.8/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.7/alia/df_tools.py` & `alia-0.1.8/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.7/alia/tools.py` & `alia-0.1.8/alia/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import calendar
 import difflib
 import os
 import pickle
 from datetime import datetime, date, timedelta
 
 import pandas as pd
@@ -51,14 +52,29 @@
         An un-pickled object."""
     with open(filename, "rb") as f:
         obj = pickle.load(f)
 
     return obj
 
 
+def b64encode(obj, encoding="utf-8"):
+    """Encodes an object using the base64 library.
+
+    Args:
+        obj (any type): Object to encode
+        encoding (str): Encoding to use (utf-8 by default)
+
+    Returns:
+        An encoded string representing the given object."""
+    if isinstance(obj, str):
+        return base64.b64encode(bytes(obj, encoding)).decode(encoding)
+    else:
+        return base64.b64encode(obj).decode(encoding)
+
+
 def tformat(date_obj, style=None):
     """Formats a date or datetime object as a string with the given style.
     When style=None default datetime format is %Y-%m-%d %H:%M:%S and default date format is %Y-%m-%d.
 
     Args:
         date_obj (date, datetime): Date or datetime object to format
         style (str): Desired datetime format (i.e. %Y-%m-%d)
```

### Comparing `alia-0.1.7/setup.py` & `alia-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.1.7",
+    version="0.1.8",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
```

