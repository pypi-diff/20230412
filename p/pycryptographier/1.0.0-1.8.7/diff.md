# Comparing `tmp/pycryptographier-1.0.0.tar.gz` & `tmp/pycryptographier-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptographier-1.0.0.tar", last modified: Wed Apr 12 16:04:39 2023, max compression
+gzip compressed data, was "pycryptographier-1.8.7.tar", last modified: Wed Apr 12 18:58:15 2023, max compression
```

## Comparing `pycryptographier-1.0.0.tar` & `pycryptographier-1.8.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:04:39.933563 pycryptographier-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-12 16:04:39.929563 pycryptographier-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:04:39.929563 pycryptographier-1.0.0/pycryptographier/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 16:04:39.000000 pycryptographier-1.0.0/pycryptographier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:04:39.929563 pycryptographier-1.0.0/pycryptographier.egg-info/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-12 16:04:39.000000 pycryptographier-1.0.0/pycryptographier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-12 16:04:39.000000 pycryptographier-1.0.0/pycryptographier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:04:39.000000 pycryptographier-1.0.0/pycryptographier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 16:04:39.000000 pycryptographier-1.0.0/pycryptographier.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 16:04:39.933563 pycryptographier-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      537 2023-04-12 16:04:38.000000 pycryptographier-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 18:58:15.858151 pycryptographier-1.8.7/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-04-12 18:58:15.858151 pycryptographier-1.8.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 18:58:15.858151 pycryptographier-1.8.7/pycryptographier/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-12 18:58:15.000000 pycryptographier-1.8.7/pycryptographier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 18:58:15.858151 pycryptographier-1.8.7/pycryptographier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-04-12 18:58:15.000000 pycryptographier-1.8.7/pycryptographier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-12 18:58:15.000000 pycryptographier-1.8.7/pycryptographier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 18:58:15.000000 pycryptographier-1.8.7/pycryptographier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 18:58:15.000000 pycryptographier-1.8.7/pycryptographier.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 18:58:15.858151 pycryptographier-1.8.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      555 2023-04-12 18:58:14.000000 pycryptographier-1.8.7/setup.py
```

### Comparing `pycryptographier-1.0.0/setup.py` & `pycryptographier-1.8.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '1.8.7'
+DESCRIPTION = "Cryptography package"
+LONG_DESCRIPTION = "Cryptography package"
 
 # Setting up
 setup(
     name="pycryptographier",
     version=VERSION,
     author="NHJonas",
     author_email="nick.faltermeier@gmx.de",
```

