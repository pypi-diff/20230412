# Comparing `tmp/cryptographylib-1.0.0.tar.gz` & `tmp/cryptographylib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographylib-1.0.0.tar", last modified: Wed Apr 12 16:06:34 2023, max compression
+gzip compressed data, was "cryptographylib-1.2.0.tar", last modified: Wed Apr 12 19:45:46 2023, max compression
```

## Comparing `cryptographylib-1.0.0.tar` & `cryptographylib-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:06:34.012557 cryptographylib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-12 16:06:34.012557 cryptographylib-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:06:34.008557 cryptographylib-1.0.0/cryptographylib/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 16:06:33.000000 cryptographylib-1.0.0/cryptographylib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:06:34.012557 cryptographylib-1.0.0/cryptographylib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-12 16:06:33.000000 cryptographylib-1.0.0/cryptographylib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-04-12 16:06:33.000000 cryptographylib-1.0.0/cryptographylib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:06:33.000000 cryptographylib-1.0.0/cryptographylib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-12 16:06:33.000000 cryptographylib-1.0.0/cryptographylib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 16:06:34.012557 cryptographylib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      536 2023-04-12 16:06:32.000000 cryptographylib-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:45:46.766715 cryptographylib-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-04-12 19:45:46.766715 cryptographylib-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:45:46.766715 cryptographylib-1.2.0/cryptographylib/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-12 19:45:46.000000 cryptographylib-1.2.0/cryptographylib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:45:46.766715 cryptographylib-1.2.0/cryptographylib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-04-12 19:45:46.000000 cryptographylib-1.2.0/cryptographylib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-12 19:45:46.000000 cryptographylib-1.2.0/cryptographylib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:45:46.000000 cryptographylib-1.2.0/cryptographylib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-12 19:45:46.000000 cryptographylib-1.2.0/cryptographylib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 19:45:46.766715 cryptographylib-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-12 19:45:44.000000 cryptographylib-1.2.0/setup.py
```

### Comparing `cryptographylib-1.0.0/setup.py` & `cryptographylib-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '1.2.0'
+DESCRIPTION = "Crypto Package"
+LONG_DESCRIPTION = "Crypto Package"
 
 # Setting up
 setup(
     name="cryptographylib",
     version=VERSION,
     author="NHJonas",
     author_email="nick.faltermeier@gmx.de",
```

