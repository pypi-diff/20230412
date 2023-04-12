# Comparing `tmp/TapisCL-ICICLE-0.0.21.tar.gz` & `tmp/TapisCL-ICICLE-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.21.tar", last modified: Wed Apr 12 21:44:19 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.22.tar", last modified: Wed Apr 12 21:51:32 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.21.tar` & `TapisCL-ICICLE-0.0.22.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:44:19.118909 TapisCL-ICICLE-0.0.21/
--rw-rw-rw-   0        0        0    35823 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.21/LICENSE
--rw-rw-rw-   0        0        0    43024 2023-04-12 21:44:19.117914 TapisCL-ICICLE-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-04-12 05:02:25.000000 TapisCL-ICICLE-0.0.21/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 21:44:19.111932 TapisCL-ICICLE-0.0.21/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 18:30:28.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1408 2023-04-12 20:12:15.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    11151 2023-04-12 21:12:56.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     6873 2023-04-12 21:08:42.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     4985 2023-04-12 20:49:51.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     1049 2023-04-12 16:16:32.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10512 2023-04-12 21:18:32.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-12 17:45:30.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    16274 2023-04-12 21:21:11.000000 TapisCL-ICICLE-0.0.21/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:44:19.116916 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43024 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 21:44:19.000000 TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      983 2023-04-12 21:43:40.000000 TapisCL-ICICLE-0.0.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 21:44:19.118909 TapisCL-ICICLE-0.0.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 21:51:32.605950 TapisCL-ICICLE-0.0.22/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.22/LICENSE
+-rw-rw-rw-   0        0        0    43024 2023-04-12 21:51:32.605950 TapisCL-ICICLE-0.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-04-12 05:02:25.000000 TapisCL-ICICLE-0.0.22/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 21:51:32.595952 TapisCL-ICICLE-0.0.22/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 18:30:28.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1408 2023-04-12 20:12:15.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    11151 2023-04-12 21:12:56.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     6873 2023-04-12 21:08:42.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     4985 2023-04-12 20:49:51.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     1049 2023-04-12 16:16:32.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10512 2023-04-12 21:18:32.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-12 17:45:30.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    16274 2023-04-12 21:21:11.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:51:32.603957 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43024 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-12 21:50:58.000000 TapisCL-ICICLE-0.0.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 21:51:32.605950 TapisCL-ICICLE-0.0.22/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.21/LICENSE` & `TapisCL-ICICLE-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/PKG-INFO` & `TapisCL-ICICLE-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.21
+Version: 0.0.22
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.21/README.md` & `TapisCL-ICICLE-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/helpers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.22/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.21/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.21
+Version: 0.0.22
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.21/pyproject.toml` & `TapisCL-ICICLE-0.0.22/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.21"
+version = "0.0.22"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
@@ -27,7 +27,10 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE"
+
+[project.entry-points."TapisCLICICLE.__main__"]
+tomatoes = "TapisCLICICLE:__main__"
```

