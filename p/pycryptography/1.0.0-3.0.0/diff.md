# Comparing `tmp/pycryptography-1.0.0.tar.gz` & `tmp/pycryptography-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptography-1.0.0.tar", last modified: Wed Apr 12 13:43:31 2023, max compression
+gzip compressed data, was "pycryptography-3.0.0.tar", last modified: Wed Apr 12 15:59:44 2023, max compression
```

## Comparing `pycryptography-1.0.0.tar` & `pycryptography-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:43:31.851159 pycryptography-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-12 13:43:31.851159 pycryptography-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:43:31.851159 pycryptography-1.0.0/pycryptography/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 13:43:31.000000 pycryptography-1.0.0/pycryptography/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:43:31.851159 pycryptography-1.0.0/pycryptography.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-12 13:43:31.000000 pycryptography-1.0.0/pycryptography.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-04-12 13:43:31.000000 pycryptography-1.0.0/pycryptography.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 13:43:31.000000 pycryptography-1.0.0/pycryptography.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-12 13:43:31.000000 pycryptography-1.0.0/pycryptography.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 13:43:31.851159 pycryptography-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      535 2023-04-12 13:43:30.000000 pycryptography-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:59:44.388139 pycryptography-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      405 2023-04-12 15:59:44.388139 pycryptography-3.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:59:44.384139 pycryptography-3.0.0/pycryptography/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-12 15:59:43.000000 pycryptography-3.0.0/pycryptography/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:59:44.388139 pycryptography-3.0.0/pycryptography.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2023-04-12 15:59:44.000000 pycryptography-3.0.0/pycryptography.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-04-12 15:59:44.000000 pycryptography-3.0.0/pycryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 15:59:44.000000 pycryptography-3.0.0/pycryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-12 15:59:44.000000 pycryptography-3.0.0/pycryptography.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 15:59:44.388139 pycryptography-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-12 15:59:43.000000 pycryptography-3.0.0/setup.py
```

### Comparing `pycryptography-1.0.0/setup.py` & `pycryptography-3.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '3.0.0'
+DESCRIPTION = "A Python package to encrypt complex data in Python3"
+LONG_DESCRIPTION = "A Python package to encrypt complex data in Python3"
 
 # Setting up
 setup(
     name="pycryptography",
     version=VERSION,
-    author="NHJonas",
+    author="knwnLegend",
     author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
```

