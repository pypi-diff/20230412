# Comparing `tmp/prevert-1.0.1.tar.gz` & `tmp/prevert-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prevert-1.0.1.tar", last modified: Tue Apr 11 14:29:07 2023, max compression
+gzip compressed data, was "prevert-1.0.2.tar", last modified: Wed Apr 12 06:22:16 2023, max compression
```

## Comparing `prevert-1.0.1.tar` & `prevert-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/
--rw-rw-r--   0 peter     (1000) peter     (1000)    11558 2023-04-11 13:32:00.000000 prevert-1.0.1/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)       31 2023-04-11 13:47:00.000000 prevert-1.0.1/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)    14555 2023-04-11 14:29:07.324228 prevert-1.0.1/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     1107 2023-04-11 14:28:49.000000 prevert-1.0.1/README.md
--rw-rw-r--   0 peter     (1000) peter     (1000)      756 2023-04-11 14:27:36.000000 prevert-1.0.1/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-04-11 14:29:07.324228 prevert-1.0.1/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/src/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/src/prevert/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1910 2023-04-11 14:26:32.000000 prevert-1.0.1/src/prevert/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/src/prevert.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)    14555 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      242 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-12 06:22:16.467231 prevert-1.0.2/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11558 2023-04-11 13:32:00.000000 prevert-1.0.2/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)       31 2023-04-11 13:47:00.000000 prevert-1.0.2/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)    14555 2023-04-12 06:22:16.467231 prevert-1.0.2/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1107 2023-04-11 14:28:49.000000 prevert-1.0.2/README.md
+-rw-rw-r--   0 peter     (1000) peter     (1000)      756 2023-04-12 06:21:38.000000 prevert-1.0.2/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-04-12 06:22:16.467231 prevert-1.0.2/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-12 06:22:16.463231 prevert-1.0.2/src/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-12 06:22:16.463231 prevert-1.0.2/src/prevert/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1910 2023-04-11 14:26:32.000000 prevert-1.0.2/src/prevert/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-12 06:22:16.467231 prevert-1.0.2/src/prevert.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    14555 2023-04-12 06:22:16.000000 prevert-1.0.2/src/prevert.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      264 2023-04-12 06:22:16.000000 prevert-1.0.2/src/prevert.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-04-12 06:22:16.000000 prevert-1.0.2/src/prevert.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-04-12 06:22:16.000000 prevert-1.0.2/src/prevert.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-04-12 06:22:16.000000 prevert-1.0.2/src/prevert.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-12 06:22:16.467231 prevert-1.0.2/tests/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      597 2023-04-12 06:14:44.000000 prevert-1.0.2/tests/test_reading.py
```

### Comparing `prevert-1.0.1/LICENSE` & `prevert-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prevert-1.0.1/PKG-INFO` & `prevert-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prevert
-Version: 1.0.1
+Version: 1.0.2
 Summary: Iterator for prevert files
 Author-email: Peter Rupnik <peter.rupnik@ijs.si>, Nikola Ljubešić <nikola.ljubesic@ijs.si>, Taja Kuzman <taja.kuzman@ijs.si>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `prevert-1.0.1/README.md` & `prevert-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `prevert-1.0.1/pyproject.toml` & `prevert-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prevert"
-version = "1.0.1"
+version = "1.0.2"
 description = "Iterator for prevert files"
 readme = "README.md"
 authors = [
 { name = "Peter Rupnik", email = "peter.rupnik@ijs.si" },
 { name = "Nikola Ljubešić", email = "nikola.ljubesic@ijs.si" },
 { name = "Taja Kuzman", email = "taja.kuzman@ijs.si" },
 ]
```

### Comparing `prevert-1.0.1/src/prevert/__init__.py` & `prevert-1.0.2/src/prevert/__init__.py`

 * *Files identical despite different names*

### Comparing `prevert-1.0.1/src/prevert.egg-info/PKG-INFO` & `prevert-1.0.2/src/prevert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prevert
-Version: 1.0.1
+Version: 1.0.2
 Summary: Iterator for prevert files
 Author-email: Peter Rupnik <peter.rupnik@ijs.si>, Nikola Ljubešić <nikola.ljubesic@ijs.si>, Taja Kuzman <taja.kuzman@ijs.si>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

