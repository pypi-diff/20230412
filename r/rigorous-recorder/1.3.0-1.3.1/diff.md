# Comparing `tmp/rigorous_recorder-1.3.0.tar.gz` & `tmp/rigorous_recorder-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigorous_recorder-1.3.0.tar", last modified: Sun Mar 19 14:34:25 2023, max compression
+gzip compressed data, was "rigorous_recorder-1.3.1.tar", last modified: Wed Apr 12 13:55:06 2023, max compression
```

## Comparing `rigorous_recorder-1.3.0.tar` & `rigorous_recorder-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-03-19 14:34:25.943583 rigorous_recorder-1.3.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-03-19 14:34:25.943451 rigorous_recorder-1.3.0/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-03-19 14:34:25.942621 rigorous_recorder-1.3.0/rigorous_recorder/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       36 2023-03-19 13:33:17.000000 rigorous_recorder-1.3.0/rigorous_recorder/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    34454 2023-03-19 14:29:57.000000 rigorous_recorder-1.3.0/rigorous_recorder/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-03-19 14:34:25.943283 rigorous_recorder-1.3.0/rigorous_recorder.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-03-19 14:34:25.000000 rigorous_recorder-1.3.0/rigorous_recorder.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      268 2023-03-19 14:34:25.000000 rigorous_recorder-1.3.0/rigorous_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-03-19 14:34:25.000000 rigorous_recorder-1.3.0/rigorous_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       59 2023-03-19 14:34:25.000000 rigorous_recorder-1.3.0/rigorous_recorder.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-03-19 14:34:25.000000 rigorous_recorder-1.3.0/rigorous_recorder.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-03-19 14:34:25.943625 rigorous_recorder-1.3.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-03-19 13:50:47.000000 rigorous_recorder-1.3.0/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:55:06.052296 rigorous_recorder-1.3.1/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:55:06.052157 rigorous_recorder-1.3.1/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:55:06.051372 rigorous_recorder-1.3.1/rigorous_recorder/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       36 2023-03-19 13:33:17.000000 rigorous_recorder-1.3.1/rigorous_recorder/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    34454 2023-03-19 14:29:57.000000 rigorous_recorder-1.3.1/rigorous_recorder/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:55:06.051996 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      268 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       59 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-04-12 13:55:05.000000 rigorous_recorder-1.3.1/rigorous_recorder.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-12 13:55:06.052337 rigorous_recorder-1.3.1/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-03-19 13:50:47.000000 rigorous_recorder-1.3.1/setup.py
```

### Comparing `rigorous_recorder-1.3.0/PKG-INFO` & `rigorous_recorder-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous_recorder
-Version: 1.3.0
+Version: 1.3.1
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.3.0/rigorous_recorder/main.py` & `rigorous_recorder-1.3.1/rigorous_recorder/main.py`

 * *Files identical despite different names*

### Comparing `rigorous_recorder-1.3.0/rigorous_recorder.egg-info/PKG-INFO` & `rigorous_recorder-1.3.1/rigorous_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous-recorder
-Version: 1.3.0
+Version: 1.3.1
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.3.0/setup.py` & `rigorous_recorder-1.3.1/setup.py`

 * *Files identical despite different names*

