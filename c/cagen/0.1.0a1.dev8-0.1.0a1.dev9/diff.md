# Comparing `tmp/cagen-0.1.0a1.dev8.tar.gz` & `tmp/cagen-0.1.0a1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.1.0a1.dev8.tar", last modified: Sat Jan 14 22:39:28 2023, max compression
+gzip compressed data, was "cagen-0.1.0a1.dev9.tar", last modified: Sat Jan 14 23:02:36 2023, max compression
```

## Comparing `cagen-0.1.0a1.dev8.tar` & `cagen-0.1.0a1.dev9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 22:39:28.203232 cagen-0.1.0a1.dev8/
--rw-r--r--   0 xan       (1000) xan       (1000)    18093 2023-01-04 12:26:34.000000 cagen-0.1.0a1.dev8/LICENSE
--rw-r--r--   0 xan       (1000) xan       (1000)     3067 2023-01-14 22:39:28.203232 cagen-0.1.0a1.dev8/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     2165 2023-01-14 22:37:52.000000 cagen-0.1.0a1.dev8/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1051 2023-01-13 19:34:54.000000 cagen-0.1.0a1.dev8/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-01-14 22:39:28.203232 cagen-0.1.0a1.dev8/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 22:39:28.203232 cagen-0.1.0a1.dev8/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 22:39:28.203232 cagen-0.1.0a1.dev8/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)        0 2023-01-08 15:44:40.000000 cagen-0.1.0a1.dev8/src/cagen/__init__.py
--rwxr-xr-x   0 xan       (1000) xan       (1000)      875 2023-01-13 16:37:28.000000 cagen-0.1.0a1.dev8/src/cagen/cagen-make.py
--rwxr-xr-x   0 xan       (1000) xan       (1000)     1248 2023-01-12 21:15:09.000000 cagen-0.1.0a1.dev8/src/cagen/cagen.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4455 2023-01-13 14:39:41.000000 cagen-0.1.0a1.dev8/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 22:39:28.203232 cagen-0.1.0a1.dev8/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)        0 2023-01-08 15:45:16.000000 cagen-0.1.0a1.dev8/src/cagen/templates/__init__.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 22:39:28.203232 cagen-0.1.0a1.dev8/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     3067 2023-01-14 22:39:28.000000 cagen-0.1.0a1.dev8/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      315 2023-01-14 22:39:28.000000 cagen-0.1.0a1.dev8/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-01-14 22:39:28.000000 cagen-0.1.0a1.dev8/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-01-14 22:39:28.000000 cagen-0.1.0a1.dev8/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-01-14 22:39:28.000000 cagen-0.1.0a1.dev8/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/
+-rw-r--r--   0 xan       (1000) xan       (1000)    18093 2023-01-04 12:26:34.000000 cagen-0.1.0a1.dev9/LICENSE
+-rw-r--r--   0 xan       (1000) xan       (1000)       30 2023-01-14 23:02:30.000000 cagen-0.1.0a1.dev9/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     3067 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     2165 2023-01-14 22:37:52.000000 cagen-0.1.0a1.dev9/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1099 2023-01-14 22:53:28.000000 cagen-0.1.0a1.dev9/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.732638 cagen-0.1.0a1.dev9/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.732638 cagen-0.1.0a1.dev9/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)        0 2023-01-08 15:44:40.000000 cagen-0.1.0a1.dev9/src/cagen/__init__.py
+-rwxr-xr-x   0 xan       (1000) xan       (1000)      875 2023-01-13 16:37:28.000000 cagen-0.1.0a1.dev9/src/cagen/cagen-make.py
+-rwxr-xr-x   0 xan       (1000) xan       (1000)     1248 2023-01-12 21:15:09.000000 cagen-0.1.0a1.dev9/src/cagen/cagen.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4455 2023-01-13 14:39:41.000000 cagen-0.1.0a1.dev9/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)     1076 2023-01-13 14:43:30.000000 cagen-0.1.0a1.dev9/src/cagen/templates/schema.tmpl
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-01-14 23:02:36.735972 cagen-0.1.0a1.dev9/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     3067 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      327 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-01-14 23:02:36.000000 cagen-0.1.0a1.dev9/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.1.0a1.dev8/LICENSE` & `cagen-0.1.0a1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `cagen-0.1.0a1.dev8/PKG-INFO` & `cagen-0.1.0a1.dev9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.1.0a1.dev8
+Version: 0.1.0a1.dev9
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://sr.ht/~somenxavierb/cagen/
 Project-URL: Bug Tracker, https://todo.sr.ht/~somenxavierb/cagen-tasks
 Project-URL: Repository, https://git.sr.ht/~somenxavierb/cagen
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `cagen-0.1.0a1.dev8/README.md` & `cagen-0.1.0a1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.1.0a1.dev8/pyproject.toml` & `cagen-0.1.0a1.dev9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = true
+
 [project]
 name = "cagen"
-version = "0.1.0-alpha1-dev8"
+version = "0.1.0-alpha1-dev9"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
@@ -20,11 +23,12 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
         'Topic :: Internet :: WWW/HTTP :: Site Management']
 dependencies = [
 	"python-frontmatter>=1.0.0",
 	"pypandoc>=1.10",
 	"Mako>=1.2.4"]
+
 [project.urls]
 "Homepage" = "https://sr.ht/~somenxavierb/cagen/"
 "Bug Tracker" = "https://todo.sr.ht/~somenxavierb/cagen-tasks"
 "Repository" = "https://git.sr.ht/~somenxavierb/cagen"
```

### Comparing `cagen-0.1.0a1.dev8/src/cagen/cagen-make.py` & `cagen-0.1.0a1.dev9/src/cagen/cagen-make.py`

 * *Files identical despite different names*

### Comparing `cagen-0.1.0a1.dev8/src/cagen/cagen.py` & `cagen-0.1.0a1.dev9/src/cagen/cagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.1.0a1.dev8/src/cagen/libcagen.py` & `cagen-0.1.0a1.dev9/src/cagen/libcagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.1.0a1.dev8/src/cagen.egg-info/PKG-INFO` & `cagen-0.1.0a1.dev9/src/cagen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.1.0a1.dev8
+Version: 0.1.0a1.dev9
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://sr.ht/~somenxavierb/cagen/
 Project-URL: Bug Tracker, https://todo.sr.ht/~somenxavierb/cagen-tasks
 Project-URL: Repository, https://git.sr.ht/~somenxavierb/cagen
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

