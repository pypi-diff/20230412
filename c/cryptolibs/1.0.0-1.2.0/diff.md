# Comparing `tmp/cryptolibs-1.0.0.tar.gz` & `tmp/cryptolibs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptolibs-1.0.0.tar", last modified: Wed Apr 12 16:07:45 2023, max compression
+gzip compressed data, was "cryptolibs-1.2.0.tar", last modified: Wed Apr 12 20:23:31 2023, max compression
```

## Comparing `cryptolibs-1.0.0.tar` & `cryptolibs-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:07:45.219928 cryptolibs-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-12 16:07:45.219928 cryptolibs-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:07:45.219928 cryptolibs-1.0.0/cryptolibs/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 16:07:44.000000 cryptolibs-1.0.0/cryptolibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:07:45.219928 cryptolibs-1.0.0/cryptolibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-12 16:07:45.000000 cryptolibs-1.0.0/cryptolibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-12 16:07:45.000000 cryptolibs-1.0.0/cryptolibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:07:45.000000 cryptolibs-1.0.0/cryptolibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-12 16:07:45.000000 cryptolibs-1.0.0/cryptolibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 16:07:45.219928 cryptolibs-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-12 16:07:43.000000 cryptolibs-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:23:31.238925 cryptolibs-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-12 20:23:31.238925 cryptolibs-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:23:31.234925 cryptolibs-1.2.0/cryptolibs/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-12 20:23:30.000000 cryptolibs-1.2.0/cryptolibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:23:31.234925 cryptolibs-1.2.0/cryptolibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-12 20:23:31.000000 cryptolibs-1.2.0/cryptolibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-12 20:23:31.000000 cryptolibs-1.2.0/cryptolibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:23:31.000000 cryptolibs-1.2.0/cryptolibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-12 20:23:31.000000 cryptolibs-1.2.0/cryptolibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:23:31.238925 cryptolibs-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      585 2023-04-12 20:23:30.000000 cryptolibs-1.2.0/setup.py
```

### Comparing `cryptolibs-1.0.0/setup.py` & `cryptolibs-1.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '1.2.0'
+DESCRIPTION = "Package that helps with crypto libarys"
+LONG_DESCRIPTION = "Package that helps with crypto libarys"
 
 # Setting up
 setup(
     name="cryptolibs",
     version=VERSION,
     author="NHJonas",
     author_email="nick.faltermeier@gmx.de",
```

