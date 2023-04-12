# Comparing `tmp/dataroid-0.0.1.tar.gz` & `tmp/dataroid-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataroid-0.0.1.tar", last modified: Wed Apr 12 13:06:19 2023, max compression
+gzip compressed data, was "dataroid-0.0.2.tar", last modified: Wed Apr 12 14:09:08 2023, max compression
```

## Comparing `dataroid-0.0.1.tar` & `dataroid-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 13:06:19.035990 dataroid-0.0.1/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      578 2023-04-12 13:06:19.035990 dataroid-0.0.1/PKG-INFO
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 13:06:19.031989 dataroid-0.0.1/dataroid/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       29 2023-04-11 19:54:23.000000 dataroid-0.0.1/dataroid/__init__.py
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1172 2023-04-12 13:02:55.000000 dataroid-0.0.1/dataroid/dataroid.py
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 13:06:19.031989 dataroid-0.0.1/dataroid.egg-info/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      578 2023-04-12 13:06:19.000000 dataroid-0.0.1/dataroid.egg-info/PKG-INFO
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      209 2023-04-12 13:06:19.000000 dataroid-0.0.1/dataroid.egg-info/SOURCES.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        1 2023-04-12 13:06:19.000000 dataroid-0.0.1/dataroid.egg-info/dependency_links.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       13 2023-04-12 13:06:19.000000 dataroid-0.0.1/dataroid.egg-info/requires.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        9 2023-04-12 13:06:19.000000 dataroid-0.0.1/dataroid.egg-info/top_level.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       38 2023-04-12 13:06:19.035990 dataroid-0.0.1/setup.cfg
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      774 2023-04-12 13:06:11.000000 dataroid-0.0.1/setup.py
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:09:08.263484 dataroid-0.0.2/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      581 2023-04-12 14:09:08.263484 dataroid-0.0.2/PKG-INFO
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:09:08.263484 dataroid-0.0.2/dataroid/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:03:59.000000 dataroid-0.0.2/dataroid/__init__.py
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1172 2023-04-12 13:02:55.000000 dataroid-0.0.2/dataroid/dataroid.py
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:09:08.263484 dataroid-0.0.2/dataroid.egg-info/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      581 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/PKG-INFO
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      209 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/SOURCES.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        1 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/dependency_links.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       27 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/requires.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        9 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/top_level.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       38 2023-04-12 14:09:08.263484 dataroid-0.0.2/setup.cfg
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      791 2023-04-12 14:08:48.000000 dataroid-0.0.2/setup.py
```

### Comparing `dataroid-0.0.1/PKG-INFO` & `dataroid-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dataroid
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Simple Wrapper For Synthetic Data Generation
 Home-page: UNKNOWN
 Author: torchd3v (Burak Egeli)
-Author-email: <mail@neuralnine.com>
+Author-email: <burak96egeli@gmail.com>
 License: UNKNOWN
 Keywords: python,data,generate,synthetic,deep learning,model
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `dataroid-0.0.1/dataroid/dataroid.py` & `dataroid-0.0.2/dataroid/dataroid.py`

 * *Files identical despite different names*

### Comparing `dataroid-0.0.1/dataroid.egg-info/PKG-INFO` & `dataroid-0.0.2/dataroid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dataroid
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Simple Wrapper For Synthetic Data Generation
 Home-page: UNKNOWN
 Author: torchd3v (Burak Egeli)
-Author-email: <mail@neuralnine.com>
+Author-email: <burak96egeli@gmail.com>
 License: UNKNOWN
 Keywords: python,data,generate,synthetic,deep learning,model
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `dataroid-0.0.1/setup.py` & `dataroid-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A Simple Wrapper For Synthetic Data Generation'
 
 # Setting up
 setup(
     name="dataroid",
     version=VERSION,
     author="torchd3v (Burak Egeli)",
-    author_email="<mail@neuralnine.com>",
+    author_email="<burak96egeli@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['pandas', 'ctgan'],
+    install_requires=['pandas==1.5.3', 'ctgan==0.7.1'],
     keywords=['python', 'data', 'generate', 'synthetic', 'deep learning', 'model'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

