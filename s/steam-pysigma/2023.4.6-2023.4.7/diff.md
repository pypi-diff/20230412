# Comparing `tmp/steam-pysigma-2023.4.6.tar.gz` & `tmp/steam-pysigma-2023.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.4.6.tar", last modified: Thu Apr  6 09:06:49 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.4.7.tar", last modified: Wed Apr 12 08:24:29 2023, max compression
```

## Comparing `steam-pysigma-2023.4.6.tar` & `steam-pysigma-2023.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 09:06:49.882294 steam-pysigma-2023.4.6/
--rw-rw-rw-   0        0        0     1030 2023-04-06 09:06:49.881294 steam-pysigma-2023.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 09:06:49.882294 steam-pysigma-2023.4.6/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-04-06 09:06:44.000000 steam-pysigma-2023.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 09:06:49.872293 steam-pysigma-2023.4.6/steam_pysigma/
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.4.6/steam_pysigma/__init__.py
--rw-rw-rw-   0        0        0    10881 2023-04-05 08:23:05.000000 steam-pysigma-2023.4.6/steam_pysigma/helpers.py
--rw-rw-rw-   0        0        0     8355 2023-04-05 08:56:51.000000 steam-pysigma-2023.4.6/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-04-06 09:06:49.880293 steam-pysigma-2023.4.6/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-04-06 09:06:46.000000 steam-pysigma-2023.4.6/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-06 09:06:46.000000 steam-pysigma-2023.4.6/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 09:06:46.000000 steam-pysigma-2023.4.6/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-04-06 09:06:46.000000 steam-pysigma-2023.4.6/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-06 09:06:46.000000 steam-pysigma-2023.4.6/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 08:24:29.961576 steam-pysigma-2023.4.7/
+-rw-rw-rw-   0        0        0     1030 2023-04-12 08:24:29.955576 steam-pysigma-2023.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 08:24:29.962577 steam-pysigma-2023.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-04-12 08:13:33.000000 steam-pysigma-2023.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:24:29.907576 steam-pysigma-2023.4.7/steam_pysigma/
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.4.7/steam_pysigma/__init__.py
+-rw-rw-rw-   0        0        0    10881 2023-04-05 08:23:05.000000 steam-pysigma-2023.4.7/steam_pysigma/helpers.py
+-rw-rw-rw-   0        0        0     8355 2023-04-05 08:56:51.000000 steam-pysigma-2023.4.7/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:24:29.952576 steam-pysigma-2023.4.7/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.4.6/PKG-INFO` & `steam-pysigma-2023.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.4.6
+Version: 2023.4.7
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: STEAM,CERN,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.4.6/README.md` & `steam-pysigma-2023.4.7/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.4.6/setup.py` & `steam-pysigma-2023.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.4.6",
+    version="2023.4.7",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.4.6/steam_pysigma/helpers.py` & `steam-pysigma-2023.4.7/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.4.6/steam_pysigma/pysigma.py` & `steam-pysigma-2023.4.7/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.4.6/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.4.7/steam_pysigma.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.4.6
+Version: 2023.4.7
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: STEAM,CERN,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

