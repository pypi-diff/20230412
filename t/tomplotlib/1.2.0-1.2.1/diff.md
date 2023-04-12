# Comparing `tmp/tomplotlib-1.2.0.tar.gz` & `tmp/tomplotlib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomplotlib-1.2.0.tar", last modified: Wed Apr 12 13:58:42 2023, max compression
+gzip compressed data, was "tomplotlib-1.2.1.tar", last modified: Wed Apr 12 14:02:42 2023, max compression
```

## Comparing `tomplotlib-1.2.0.tar` & `tomplotlib-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 13:58:42.186925 tomplotlib-1.2.0/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-12 13:58:42.186762 tomplotlib-1.2.0/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2436 2023-04-12 13:44:36.000000 tomplotlib-1.2.0/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       38 2023-04-12 13:58:42.186971 tomplotlib-1.2.0/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)      757 2023-04-12 13:41:35.000000 tomplotlib-1.2.0/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 13:58:42.185330 tomplotlib-1.2.0/tomplotlib/
--rw-r--r--   0 tomgeorge   (501) staff       (20)       82 2023-04-12 13:40:52.000000 tomplotlib-1.2.0/tomplotlib/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7892 2023-04-12 13:53:34.000000 tomplotlib-1.2.0/tomplotlib/tpl.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 13:58:42.186227 tomplotlib-1.2.0/tomplotlib.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-12 13:58:42.000000 tomplotlib-1.2.0/tomplotlib.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      228 2023-04-12 13:58:42.000000 tomplotlib-1.2.0/tomplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-12 13:58:42.000000 tomplotlib-1.2.0/tomplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       17 2023-04-12 13:58:42.000000 tomplotlib-1.2.0/tomplotlib.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       11 2023-04-12 13:58:42.000000 tomplotlib-1.2.0/tomplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 14:02:42.578047 tomplotlib-1.2.1/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-12 14:02:42.577866 tomplotlib-1.2.1/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2436 2023-04-12 13:44:36.000000 tomplotlib-1.2.1/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       38 2023-04-12 14:02:42.578101 tomplotlib-1.2.1/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      757 2023-04-12 14:02:39.000000 tomplotlib-1.2.1/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 14:02:42.576787 tomplotlib-1.2.1/tomplotlib/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       43 2023-04-12 14:02:30.000000 tomplotlib-1.2.1/tomplotlib/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7854 2023-04-12 14:02:34.000000 tomplotlib-1.2.1/tomplotlib/tpl.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 14:02:42.577542 tomplotlib-1.2.1/tomplotlib.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      228 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       17 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       11 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/top_level.txt
```

### Comparing `tomplotlib-1.2.0/PKG-INFO` & `tomplotlib-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomplotlib
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package which formats matplotlib plots and contains some other useful functions
 Home-page: https://github.com/TomGeorge1234/tomplotlib
 Author: Tom George
 Author-email: tom.george.20@ucl.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tomplotlib-1.2.0/README.md` & `tomplotlib-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tomplotlib-1.2.0/setup.py` & `tomplotlib-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tomplotlib",
-    version="1.2.0",
+    version="1.2.1",
     scripts=["tomplotlib/tpl.py"],
     author="Tom George",
     author_email="tom.george.20@ucl.ac.uk",
     description="A package which formats matplotlib plots and contains some other useful functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TomGeorge1234/tomplotlib",
```

### Comparing `tomplotlib-1.2.0/tomplotlib/tpl.py` & `tomplotlib-1.2.1/tomplotlib/tpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 The function of this is to set rcParams and define a bunch of functions which make figure plotting easy and consistent
 """
-print("importing tomplotlib package")
 import tomplotlib
 
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import rcParams, rc
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from cycler import cycler
```

### Comparing `tomplotlib-1.2.0/tomplotlib.egg-info/PKG-INFO` & `tomplotlib-1.2.1/tomplotlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomplotlib
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package which formats matplotlib plots and contains some other useful functions
 Home-page: https://github.com/TomGeorge1234/tomplotlib
 Author: Tom George
 Author-email: tom.george.20@ucl.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

