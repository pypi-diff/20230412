# Comparing `tmp/MLapp1-0.0.4.tar.gz` & `tmp/MLapp1-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLapp1-0.0.4.tar", last modified: Wed Apr 12 11:22:18 2023, max compression
+gzip compressed data, was "MLapp1-0.0.5.tar", last modified: Wed Apr 12 15:55:27 2023, max compression
```

## Comparing `MLapp1-0.0.4.tar` & `MLapp1-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:22:18.061326 MLapp1-0.0.4/
--rw-r--r--   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.4/LICENSE.toml
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:22:18.061408 MLapp1-0.0.4/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.4/README.md
--rw-r--r--   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.4/pyproject.toml
--rw-r--r--   0 akshay     (503) staff       (20)      860 2023-04-12 11:22:18.062173 MLapp1-0.0.4/setup.cfg
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:22:18.057674 MLapp1-0.0.4/src/
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:22:18.061152 MLapp1-0.0.4/src/MLapp1.egg-info/
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)      216 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/requires.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/top_level.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 15:55:27.947318 MLapp1-0.0.5/
+-rw-------   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.5/LICENSE.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 15:55:27.947399 MLapp1-0.0.5/PKG-INFO
+-rw-------   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.5/README.md
+-rw-------   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.5/pyproject.toml
+-rw-------   0 akshay     (503) staff       (20)      857 2023-04-12 15:55:27.947980 MLapp1-0.0.5/setup.cfg
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 15:55:27.943550 MLapp1-0.0.5/src/
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 15:55:27.947158 MLapp1-0.0.5/src/MLapp1.egg-info/
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 15:55:27.000000 MLapp1-0.0.5/src/MLapp1.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)      216 2023-04-12 15:55:27.000000 MLapp1-0.0.5/src/MLapp1.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 15:55:27.000000 MLapp1-0.0.5/src/MLapp1.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 15:55:27.000000 MLapp1-0.0.5/src/MLapp1.egg-info/requires.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 15:55:27.000000 MLapp1-0.0.5/src/MLapp1.egg-info/top_level.txt
```

### Comparing `MLapp1-0.0.4/LICENSE.toml` & `MLapp1-0.0.5/LICENSE.toml`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.4/setup.cfg` & `MLapp1-0.0.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = MLapp1
-version = 0.0.4
+version = 0.0.5
 author = Akshay
 author_email = akshaysuhag1996@gmail.com
 description = "MLapp"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FunctionalUrology/
 project_urls = 
 	Bug Tracker = https://github.com/FunctionalUrology/
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options.package_data]
-* = *.csv, *.pickle
+* = *.csv, *.txt
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires =
```

