# Comparing `tmp/TapisCL-ICICLE-0.0.2.tar.gz` & `tmp/TapisCL-ICICLE-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.2.tar", last modified: Wed Apr 12 21:32:36 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.21.tar", last modified: Wed Apr 12 21:44:19 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.2.tar` & `TapisCL-ICICLE-0.0.21.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:32:36.540827 TapisCL-ICICLE-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    43023 2023-04-12 21:32:36.539829 TapisCL-ICICLE-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-04-12 05:02:25.000000 TapisCL-ICICLE-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 21:32:36.532332 TapisCL-ICICLE-0.0.2/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-04-12 20:12:15.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    11151 2023-04-12 21:12:56.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     6873 2023-04-12 21:08:42.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     4985 2023-04-12 20:49:51.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     1049 2023-04-12 16:16:32.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10512 2023-04-12 21:18:32.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-12 17:45:30.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    16274 2023-04-12 21:21:11.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:32:36.538816 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43023 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      982 2023-04-12 21:29:55.000000 TapisCL-ICICLE-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 21:32:36.540827 TapisCL-ICICLE-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 21:44:19.118909 TapisCL-ICICLE-0.0.21/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.21/LICENSE
+-rw-rw-rw-   0        0        0    43024 2023-04-12 21:44:19.117914 TapisCL-ICICLE-0.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-04-12 05:02:25.000000 TapisCL-ICICLE-0.0.21/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 21:44:19.111932 TapisCL-ICICLE-0.0.21/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 18:30:28.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1408 2023-04-12 20:12:15.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    11151 2023-04-12 21:12:56.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     6873 2023-04-12 21:08:42.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     4985 2023-04-12 20:49:51.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     1049 2023-04-12 16:16:32.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10512 2023-04-12 21:18:32.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-12 17:45:30.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    16274 2023-04-12 21:21:11.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:44:19.116916 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43024 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      983 2023-04-12 21:43:40.000000 TapisCL-ICICLE-0.0.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 21:44:19.118909 TapisCL-ICICLE-0.0.21/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.2/LICENSE` & `TapisCL-ICICLE-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/PKG-INFO` & `TapisCL-ICICLE-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.2
+Version: 0.0.21
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.2/README.md` & `TapisCL-ICICLE-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/helpers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.21/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.2
+Version: 0.0.21
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.2/pyproject.toml` & `TapisCL-ICICLE-0.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.2"
+version = "0.0.21"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

