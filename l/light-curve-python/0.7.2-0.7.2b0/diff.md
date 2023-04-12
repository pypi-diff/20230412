# Comparing `tmp/light-curve-python-0.7.2.tar.gz` & `tmp/light-curve-python-0.7.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light-curve-python-0.7.2.tar", last modified: Wed Apr 12 16:14:09 2023, max compression
+gzip compressed data, was "light-curve-python-0.7.2b0.tar", last modified: Fri Apr  7 22:27:38 2023, max compression
```

## Comparing `light-curve-python-0.7.2.tar` & `light-curve-python-0.7.2b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:14:09.426984 light-curve-python-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-04-12 16:14:02.000000 light-curve-python-0.7.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-12 16:14:02.000000 light-curve-python-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-04-12 16:14:09.426984 light-curve-python-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-12 16:14:02.000000 light-curve-python-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:14:09.426984 light-curve-python-0.7.2/light_curve_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-04-12 16:14:09.000000 light-curve-python-0.7.2/light_curve_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-12 16:14:09.000000 light-curve-python-0.7.2/light_curve_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 16:14:09.000000 light-curve-python-0.7.2/light_curve_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-12 16:14:09.000000 light-curve-python-0.7.2/light_curve_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 16:14:09.000000 light-curve-python-0.7.2/light_curve_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-04-12 16:14:02.000000 light-curve-python-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-04-12 16:14:09.426984 light-curve-python-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-12 16:14:02.000000 light-curve-python-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/light_curve_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/setup.py
```

### Comparing `light-curve-python-0.7.2/Cargo.toml` & `light-curve-python-0.7.2b0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "light-curve-python"
-version = "0.7.2"
+version = "0.7.2-beta.0"
 authors = ["Konstantin Malanchev <hombit@gmail.com>", "Anastasia Lavrukhina <lavrukhina.ad@gmail.com>"]
 description = "Feature extractor from noisy time series"
 readme = "README.md"
 repository = "https://github.com/light-curve/light-curve-python"
 license = "GPL-3.0-or-later"
 edition = "2021"
 rust-version = "1.62"
```

### Comparing `light-curve-python-0.7.2/PKG-INFO` & `light-curve-python-0.7.2b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-curve-python
-Version: 0.7.2
+Version: 0.7.2b0
 Summary: An alias to light-curve package
 Home-page: http://github.com/hombit/light-curve
 Author: Konstantin Malanchev
 Author-email: hombit@gmail.com
 License: MIT
 Keywords: science,astrophysics
 Classifier: Intended Audience :: Science/Research
```

### Comparing `light-curve-python-0.7.2/light_curve_python.egg-info/PKG-INFO` & `light-curve-python-0.7.2b0/light_curve_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-curve-python
-Version: 0.7.2
+Version: 0.7.2b0
 Summary: An alias to light-curve package
 Home-page: http://github.com/hombit/light-curve
 Author: Konstantin Malanchev
 Author-email: hombit@gmail.com
 License: MIT
 Keywords: science,astrophysics
 Classifier: Intended Audience :: Science/Research
```

### Comparing `light-curve-python-0.7.2/setup.cfg` & `light-curve-python-0.7.2b0/setup.cfg`

 * *Files identical despite different names*

