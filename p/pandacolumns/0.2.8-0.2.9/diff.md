# Comparing `tmp/pandacolumns-0.2.8.tar.gz` & `tmp/pandacolumns-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.2.8.tar", last modified: Wed Apr 12 14:37:54 2023, max compression
+gzip compressed data, was "pandacolumns-0.2.9.tar", last modified: Wed Apr 12 14:40:19 2023, max compression
```

## Comparing `pandacolumns-0.2.8.tar` & `pandacolumns-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:37:54.758637 pandacolumns-0.2.8/
--rw-rw-rw-   0        0        0      171 2023-04-12 14:37:54.757633 pandacolumns-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 14:37:54.747619 pandacolumns-0.2.8/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.8/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-04-12 14:37:38.000000 pandacolumns-0.2.8/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:37:54.757633 pandacolumns-0.2.8/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 14:37:54.758637 pandacolumns-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-12 14:37:48.000000 pandacolumns-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:40:19.630605 pandacolumns-0.2.9/
+-rw-rw-rw-   0        0        0      171 2023-04-12 14:40:19.630605 pandacolumns-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 14:40:19.615994 pandacolumns-0.2.9/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.9/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-12 14:40:05.000000 pandacolumns-0.2.9/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:40:19.629592 pandacolumns-0.2.9/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-12 14:40:19.000000 pandacolumns-0.2.9/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-12 14:40:19.000000 pandacolumns-0.2.9/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:40:19.000000 pandacolumns-0.2.9/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-12 14:40:19.000000 pandacolumns-0.2.9/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 14:40:19.000000 pandacolumns-0.2.9/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:40:19.630605 pandacolumns-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-12 14:40:14.000000 pandacolumns-0.2.9/setup.py
```

### Comparing `pandacolumns-0.2.8/pandacolumns/dynamic.py` & `pandacolumns-0.2.9/pandacolumns/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 import ipywidgets as widgets
 from IPython.display import display
+import ipdb
 
 
 def pandadropper(df):  
   checkboxes = [widgets.Checkbox(value=False, description=column) for column in df.columns]
 
   for checkbox in checkboxes:
       checkbox.layout.width = 'auto'
```

