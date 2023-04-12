# Comparing `tmp/MLapp1-0.0.1.tar.gz` & `tmp/MLapp1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLapp1-0.0.1.tar", last modified: Wed Apr 12 10:47:16 2023, max compression
+gzip compressed data, was "MLapp1-0.0.2.tar", last modified: Wed Apr 12 11:15:46 2023, max compression
```

## Comparing `MLapp1-0.0.1.tar` & `MLapp1-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 10:47:16.292210 MLapp1-0.0.1/
--rw-r--r--   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.1/LICENSE.toml
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 10:47:16.292281 MLapp1-0.0.1/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.1/README.md
--rw-r--r--   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.1/pyproject.toml
--rw-r--r--   0 akshay     (503) staff       (20)      726 2023-04-12 10:47:16.292908 MLapp1-0.0.1/setup.cfg
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 10:47:16.289448 MLapp1-0.0.1/src/
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 10:47:16.292056 MLapp1-0.0.1/src/MLapp1.egg-info/
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 10:47:16.000000 MLapp1-0.0.1/src/MLapp1.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)      216 2023-04-12 10:47:16.000000 MLapp1-0.0.1/src/MLapp1.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 10:47:16.000000 MLapp1-0.0.1/src/MLapp1.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (503) staff       (20)       64 2023-04-12 10:47:16.000000 MLapp1-0.0.1/src/MLapp1.egg-info/requires.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 10:47:16.000000 MLapp1-0.0.1/src/MLapp1.egg-info/top_level.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:15:46.369190 MLapp1-0.0.2/
+-rw-r--r--   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.2/LICENSE.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:15:46.369337 MLapp1-0.0.2/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.2/README.md
+-rw-r--r--   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.2/pyproject.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      871 2023-04-12 11:15:46.369964 MLapp1-0.0.2/setup.cfg
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:15:46.364957 MLapp1-0.0.2/src/
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 11:15:46.368849 MLapp1-0.0.2/src/MLapp1.egg-info/
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 11:15:46.000000 MLapp1-0.0.2/src/MLapp1.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)      216 2023-04-12 11:15:46.000000 MLapp1-0.0.2/src/MLapp1.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:15:46.000000 MLapp1-0.0.2/src/MLapp1.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (503) staff       (20)      198 2023-04-12 11:15:46.000000 MLapp1-0.0.2/src/MLapp1.egg-info/requires.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 11:15:46.000000 MLapp1-0.0.2/src/MLapp1.egg-info/top_level.txt
```

### Comparing `MLapp1-0.0.1/LICENSE.toml` & `MLapp1-0.0.2/LICENSE.toml`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.1/setup.cfg` & `MLapp1-0.0.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MLapp1
-version = 0.0.1
+version = 0.0.2
 author = Akshay
 author_email = akshaysuhag1996@gmail.com
 description = "MLapp"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FunctionalUrology/
 project_urls = 
@@ -17,22 +17,33 @@
 [options.package_data]
 * = *.csv, *.pickle
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.9
 install_requires = 
+	dash
+	dash_bootstrap_components
+	dash_table
 	subprocess.run
+	webbrowser
+	pickle
+	numpy
+	zipfile36
 	pandas
 	scikit-learn
-	imbalanced-learn
+	collections2
+	colorlover
 	plotly
-	dash
+	bokeh
+	imbalanced-learn
+	matplotlib
+	dash-loading-spinners
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

