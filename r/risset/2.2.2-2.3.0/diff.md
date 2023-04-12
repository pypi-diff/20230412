# Comparing `tmp/risset-2.2.2.tar.gz` & `tmp/risset-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.2.2.tar", last modified: Wed Apr 12 10:24:53 2023, max compression
+gzip compressed data, was "risset-2.3.0.tar", last modified: Wed Apr 12 12:17:47 2023, max compression
```

## Comparing `risset-2.2.2.tar` & `risset-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 10:24:53.687569 risset-2.2.2/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 10:24:53.687569 risset-2.2.2/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.2.2/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 10:24:53.686569 risset-2.2.2/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   107792 2023-04-12 10:24:42.000000 risset-2.2.2/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-12 10:24:53.687569 risset-2.2.2/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-10 12:28:18.000000 risset-2.2.2/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 12:17:47.432653 risset-2.3.0/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 12:17:47.432653 risset-2.3.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.3.0/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 12:17:47.431653 risset-2.3.0/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 12:17:47.000000 risset-2.3.0/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-12 12:17:47.000000 risset-2.3.0/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-12 12:17:47.000000 risset-2.3.0/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-12 12:17:47.000000 risset-2.3.0/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-12 12:17:47.000000 risset-2.3.0/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-12 12:17:47.000000 risset-2.3.0/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   107792 2023-04-12 12:16:55.000000 risset-2.3.0/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-12 12:17:47.432653 risset-2.3.0/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.3.0/setup.py
```

### Comparing `risset-2.2.2/PKG-INFO` & `risset-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.2.2
+Version: 2.3.0
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.2.2/README.md` & `risset-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `risset-2.2.2/risset.egg-info/PKG-INFO` & `risset-2.3.0/risset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.2.2
+Version: 2.3.0
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.2.2/risset.py` & `risset-2.3.0/risset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.2.2"
+__version__ = "2.3.0"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
```

### Comparing `risset-2.2.2/setup.py` & `risset-2.3.0/setup.py`

 * *Files identical despite different names*

