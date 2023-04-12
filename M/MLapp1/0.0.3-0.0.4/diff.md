# Comparing `tmp/MLapp1-0.0.3.tar.gz` & `tmp/MLapp1-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLapp1-0.0.3.tar", last modified: Wed Apr 12 11:19:05 2023, max compression
+gzip compressed data, was "MLapp1-0.0.4.tar", last modified: Wed Apr 12 11:22:18 2023, max compression
```

## Comparing `MLapp1-0.0.3.tar` & `MLapp1-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:19:05.905063 MLapp1-0.0.3/
--rw-r--r--   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.3/LICENSE.toml
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:19:05.905134 MLapp1-0.0.3/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.3/README.md
--rw-r--r--   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.3/pyproject.toml
--rw-r--r--   0 akshay     (503) staff       (20)      872 2023-04-12 11:19:05.905917 MLapp1-0.0.3/setup.cfg
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:19:05.901466 MLapp1-0.0.3/src/
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:19:05.904903 MLapp1-0.0.3/src/MLapp1.egg-info/
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:19:05.000000 MLapp1-0.0.3/src/MLapp1.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)      216 2023-04-12 11:19:05.000000 MLapp1-0.0.3/src/MLapp1.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:19:05.000000 MLapp1-0.0.3/src/MLapp1.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (503) staff       (20)      199 2023-04-12 11:19:05.000000 MLapp1-0.0.3/src/MLapp1.egg-info/requires.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:19:05.000000 MLapp1-0.0.3/src/MLapp1.egg-info/top_level.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:22:18.061326 MLapp1-0.0.4/
+-rw-r--r--   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.4/LICENSE.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:22:18.061408 MLapp1-0.0.4/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.4/README.md
+-rw-r--r--   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.4/pyproject.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      860 2023-04-12 11:22:18.062173 MLapp1-0.0.4/setup.cfg
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:22:18.057674 MLapp1-0.0.4/src/
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:22:18.061152 MLapp1-0.0.4/src/MLapp1.egg-info/
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)      216 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/requires.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:22:18.000000 MLapp1-0.0.4/src/MLapp1.egg-info/top_level.txt
```

### Comparing `MLapp1-0.0.3/LICENSE.toml` & `MLapp1-0.0.4/LICENSE.toml`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.3/setup.cfg` & `MLapp1-0.0.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MLapp1
-version = 0.0.3
+version = 0.0.4
 author = Akshay
 author_email = akshaysuhag1996@gmail.com
 description = "MLapp"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FunctionalUrology/
 project_urls = 
@@ -23,15 +23,14 @@
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	dash
 	dash_bootstrap_components
 	dash_table
 	subprocess.run
-	webbrowser
 	pickle4
 	numpy
 	zipfile36
 	pandas
 	scikit-learn
 	collections2
 	colorlover
```

