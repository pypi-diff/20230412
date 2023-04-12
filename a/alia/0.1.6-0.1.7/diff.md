# Comparing `tmp/alia-0.1.6.tar.gz` & `tmp/alia-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.1.6.tar", last modified: Mon Apr 10 19:00:52 2023, max compression
+gzip compressed data, was "alia-0.1.7.tar", last modified: Wed Apr 12 16:24:04 2023, max compression
```

## Comparing `alia-0.1.6.tar` & `alia-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-10 19:00:52.189440 alia-0.1.6/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.6/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-10 19:00:52.188971 alia-0.1.6/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.6/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-10 19:00:52.186562 alia-0.1.6/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.6/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.6/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.6/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    24886 2023-04-10 19:00:16.000000 alia-0.1.6/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-10 19:00:52.188545 alia-0.1.6/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-10 19:00:52.189572 alia-0.1.6/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-10 19:00:43.000000 alia-0.1.6/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 16:24:04.306466 alia-0.1.7/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.7/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 16:24:04.306137 alia-0.1.7/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.7/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 16:24:04.303892 alia-0.1.7/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.7/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.7/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.7/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    25525 2023-04-12 16:23:41.000000 alia-0.1.7/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-12 16:24:04.305750 alia-0.1.7/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-12 16:24:04.000000 alia-0.1.7/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-12 16:24:04.306564 alia-0.1.7/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-12 16:24:01.000000 alia-0.1.7/setup.py
```

### Comparing `alia-0.1.6/LICENSE` & `alia-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.1.6/alia/colors.py` & `alia-0.1.7/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.6/alia/df_tools.py` & `alia-0.1.7/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.6/alia/tools.py` & `alia-0.1.7/alia/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,64 @@
 import calendar
 import difflib
 import os
+import pickle
 from datetime import datetime, date, timedelta
 
 import pandas as pd
 import pyperclip
 from dateutil.parser import parse
-from dotenv import load_dotenv, dotenv_values
 
 from .colors import *
 
 
 def clipboard(string):
     """Copies text to clipboard so it can be pasted anywhere.
 
     Args:
         string (str): String to copy
 
     Returns:
-        Nothing"""
+        Nothing."""
     pyperclip.copy(string)
     green("Copied to clipboard", ts=False)
 
 
+def save_obj(obj, filename):
+    """Saves an object to a file by pickling it.
+
+    Args:
+        obj (any type): Object to save
+        filename (str): Filename to save the object as
+
+    Returns:
+        Nothing."""
+    if ".pkl" not in filename:
+        filename = f"{filename.strip()}.pkl"
+
+    with open(filename, "wb") as f:
+        pickle.dump(obj, f)
+
+    green(f"Object saved as {filename}", ts=False)
+
+
+def load_obj(filename):
+    """Loads a saved pickled object.
+
+    Args:
+        filename (str): Filename of the pickled object
+
+    Returns:
+        An un-pickled object."""
+    with open(filename, "rb") as f:
+        obj = pickle.load(f)
+
+    return obj
+
+
 def tformat(date_obj, style=None):
     """Formats a date or datetime object as a string with the given style.
     When style=None default datetime format is %Y-%m-%d %H:%M:%S and default date format is %Y-%m-%d.
 
     Args:
         date_obj (date, datetime): Date or datetime object to format
         style (str): Desired datetime format (i.e. %Y-%m-%d)
@@ -472,14 +504,15 @@
     unique_words = []
     for word in words:
         if word not in unique_words:
             unique_words.append(word)
 
     return " ".join(unique_words)
 
+
 def str_remove(txt, rplc_strs):
     """Removes passed strings from a string.
 
     Args:
         txt (str): String to clean
         rplc_strs (list): Strings to remove from the passed txt string
```

### Comparing `alia-0.1.6/setup.py` & `alia-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.1.6",
+    version="0.1.7",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
```

