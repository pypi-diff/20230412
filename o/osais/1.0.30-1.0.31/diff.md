# Comparing `tmp/osais-1.0.30.tar.gz` & `tmp/osais-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-xnn7tmf4\osais-1.0.30.tar", last modified: Wed Apr 12 13:11:51 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-w521o5n9\osais-1.0.31.tar", last modified: Wed Apr 12 13:23:24 2023, max compression
```

## Comparing `osais-1.0.30.tar` & `osais-1.0.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:51.779500 osais-1.0.30/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.30/LICENSE
--rw-rw-rw-   0        0        0     1113 2023-04-12 13:11:51.778501 osais-1.0.30/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.30/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:51.774501 osais-1.0.30/osais/
--rw-rw-rw-   0        0        0      618 2023-04-05 19:42:46.000000 osais-1.0.30/osais/__init__.py
--rw-rw-rw-   0        0        0    40972 2023-04-12 13:11:40.000000 osais-1.0.30/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:11:51.777500 osais-1.0.30/osais.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-12 13:11:51.000000 osais-1.0.30/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-12 13:11:51.000000 osais-1.0.30/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 13:11:51.000000 osais-1.0.30/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-12 13:11:51.000000 osais-1.0.30/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 13:11:51.000000 osais-1.0.30/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.30/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 13:11:51.779500 osais-1.0.30/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-12 13:11:30.000000 osais-1.0.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:23:24.049351 osais-1.0.31/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.31/LICENSE
+-rw-rw-rw-   0        0        0     1113 2023-04-12 13:23:24.049351 osais-1.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.31/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 13:23:24.044348 osais-1.0.31/osais/
+-rw-rw-rw-   0        0        0      652 2023-04-12 13:22:01.000000 osais-1.0.31/osais/__init__.py
+-rw-rw-rw-   0        0        0    40972 2023-04-12 13:23:02.000000 osais-1.0.31/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:23:24.047349 osais-1.0.31/osais.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-12 13:23:24.000000 osais-1.0.31/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-12 13:23:24.000000 osais-1.0.31/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:23:24.000000 osais-1.0.31/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-12 13:23:24.000000 osais-1.0.31/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 13:23:24.000000 osais-1.0.31/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.31/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 13:23:24.049351 osais-1.0.31/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-04-12 13:23:14.000000 osais-1.0.31/setup.py
```

### Comparing `osais-1.0.30/LICENSE` & `osais-1.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.30/PKG-INFO` & `osais-1.0.31/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.30
+Version: 1.0.31
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.30/osais/__init__.py` & `osais-1.0.31/osais/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.29"
+__version__="1.0.31"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
+from .osais import osais_isLocal
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
 from .osais import osais_getDirectoryListing
 from .osais import osais_getInfo
 from .osais import osais_resetGateway
 from .osais import osais_authenticateAI
```

### Comparing `osais-1.0.30/osais/osais.py` & `osais-1.0.31/osais/osais.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 0d0a 5f5f 7665 7273 696f 6e5f 5f3d 2231  ..__version__="1
-00000010: 2e30 2e33 3022 0d0a 0d0a 2323 203d 3d3d  .0.30"....## ===
+00000010: 2e30 2e33 3122 0d0a 0d0a 2323 203d 3d3d  .0.31"....## ===
 00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000040: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000050: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000060: 3d3d 3d3d 3d0d 0a23 2320 0d0a 2323 2020  =====..## ..##  
 00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000080: 2020 2020 5574 696c 6974 6965 7320 7374      Utilities st
```

### Comparing `osais-1.0.30/osais.egg-info/PKG-INFO` & `osais-1.0.31/osais.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.30
+Version: 1.0.31
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.30/setup.py` & `osais-1.0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.30',
+    version='1.0.31',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

