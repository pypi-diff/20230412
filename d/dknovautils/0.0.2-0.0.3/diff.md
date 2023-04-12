# Comparing `tmp/dknovautils-0.0.2.tar.gz` & `tmp/dknovautils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.2.tar", last modified: Thu Mar  9 04:58:40 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.3.tar", last modified: Thu Mar  9 05:00:48 2023, max compression
```

## Comparing `dknovautils-0.0.2.tar` & `dknovautils-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 04:58:40.000000 dknovautils-0.0.2/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 04:58:40.000000 dknovautils-0.0.2/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      156 2023-03-09 04:55:58.000000 dknovautils-0.0.2/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-03-09 03:20:10.000000 dknovautils-0.0.2/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        2 2023-03-09 04:42:46.000000 dknovautils-0.0.2/dknovautils/files.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       49 2023-03-09 04:42:48.000000 dknovautils-0.0.2/dknovautils/test_a.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 02:42:43.000000 dknovautils-0.0.2/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 04:58:40.000000 dknovautils-0.0.2/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-03-09 04:58:40.000000 dknovautils-0.0.2/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      678 2023-03-09 04:58:40.000000 dknovautils-0.0.2/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2023-03-09 04:58:40.000000 dknovautils-0.0.2/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      313 2023-03-09 04:58:40.000000 dknovautils-0.0.2/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-03-09 04:58:40.000000 dknovautils-0.0.2/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.2/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      678 2023-03-09 04:58:40.000000 dknovautils-0.0.2/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      271 2023-03-09 04:58:34.000000 dknovautils-0.0.2/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-03-09 04:58:40.000000 dknovautils-0.0.2/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1057 2023-03-09 04:58:07.000000 dknovautils-0.0.2/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 05:00:48.000000 dknovautils-0.0.3/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      156 2023-03-09 04:55:58.000000 dknovautils-0.0.3/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-03-09 03:20:10.000000 dknovautils-0.0.3/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        2 2023-03-09 04:42:46.000000 dknovautils-0.0.3/dknovautils/files.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       49 2023-03-09 04:42:48.000000 dknovautils-0.0.3/dknovautils/test_a.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 02:42:43.000000 dknovautils-0.0.3/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      678 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      313 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.3/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      678 2023-03-09 05:00:48.000000 dknovautils-0.0.3/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      271 2023-03-09 04:58:34.000000 dknovautils-0.0.3/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-03-09 05:00:48.000000 dknovautils-0.0.3/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1075 2023-03-09 05:00:42.000000 dknovautils-0.0.3/setup.py
```

### Comparing `dknovautils-0.0.2/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.3/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.2/PKG-INFO` & `dknovautils-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.2/setup.py` & `dknovautils-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-version = "0.0.2"
+version = "0.0.03"
 
-with open("README.md", "r") as f:
+with open("README.md", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=version,
     author="dknova",
     author_email="dknova@example.com",
```

