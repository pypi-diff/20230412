# Comparing `tmp/pochas-geoutils-0.1.2.tar.gz` & `tmp/pochas-geoutils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pochas-geoutils-0.1.2.tar", last modified: Wed Mar  8 13:34:20 2023, max compression
+gzip compressed data, was "pochas-geoutils-0.1.3.tar", last modified: Wed Apr 12 12:48:20 2023, max compression
```

## Comparing `pochas-geoutils-0.1.2.tar` & `pochas-geoutils-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:34:20.881240 pochas-geoutils-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-08 13:34:20.881240 pochas-geoutils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:34:20.881240 pochas-geoutils-0.1.2/geoutils/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/LandsatGLAD.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/dataClean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/dataExtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/modisAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/geoutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:34:20.881240 pochas-geoutils-0.1.2/pochas_geoutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-08 13:34:20.000000 pochas-geoutils-0.1.2/pochas_geoutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-08 13:34:20.000000 pochas-geoutils-0.1.2/pochas_geoutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 13:34:20.000000 pochas-geoutils-0.1.2/pochas_geoutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-08 13:34:20.000000 pochas-geoutils-0.1.2/pochas_geoutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-08 13:34:20.000000 pochas-geoutils-0.1.2/pochas_geoutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-08 13:34:20.000000 pochas-geoutils-0.1.2/pochas_geoutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 13:34:20.881240 pochas-geoutils-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-08 13:34:11.000000 pochas-geoutils-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:48:20.224086 pochas-geoutils-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-12 12:48:20.224086 pochas-geoutils-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:48:20.224086 pochas-geoutils-0.1.3/geoutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/LandsatGLAD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/dataClean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/dataExtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/modisAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/geoutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:48:20.224086 pochas-geoutils-0.1.3/pochas_geoutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-12 12:48:20.000000 pochas-geoutils-0.1.3/pochas_geoutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-12 12:48:20.000000 pochas-geoutils-0.1.3/pochas_geoutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:48:20.000000 pochas-geoutils-0.1.3/pochas_geoutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 12:48:20.000000 pochas-geoutils-0.1.3/pochas_geoutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 12:48:20.000000 pochas-geoutils-0.1.3/pochas_geoutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 12:48:20.000000 pochas-geoutils-0.1.3/pochas_geoutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:48:20.224086 pochas-geoutils-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-12 12:48:08.000000 pochas-geoutils-0.1.3/setup.py
```

### Comparing `pochas-geoutils-0.1.2/LICENSE` & `pochas-geoutils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/PKG-INFO` & `pochas-geoutils-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-Metadata-Version: 2.1
-Name: pochas-geoutils
-Version: 0.1.2
-Summary: A Python package includes geo-utils for PoCHAS project
-Home-page: https://github.com/behzad89/pochas-geoutils
-Author: Behzad Valipour Sh.
-Author-email: behzad.valipour@swisstph.ch
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/pochas-geoutils/badge/?version=latest)](https://pochas-geoutils.readthedocs.io/en/latest/?badge=latest)
 [![image](https://img.shields.io/pypi/v/pochas-geoutils)](https://pypi.org/project/pochas-geoutils/)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![](https://github.com/behzad89/pochas-geoutils/workflows/deploy_pypi/badge.svg)
-# pochas-geoutils Python Package
+#  pochas-geoutils Python Package
+
+📦 This Python package provides spatial data handling tools 🛠️ to facilitate the input of data to machine learning algorithms🤖. All functionalities have been developed to enable user-friendly 👨‍💻 geo-data processing in [**POCHAS project**](https://www.swisstph.ch/fr/projects/project-detail/project/effects-of-airborne-pollen-on-cardiorespiratory-health-and-allergic-symptoms)
 
-A Python package is offering tools for spatial data handling to feed to machine learning Algorithms. All functionalities was applied or user-friendly geo data processing in [**POCHAS project**](https://www.swisstph.ch/fr/projects/project-detail/project/effects-of-airborne-pollen-on-cardiorespiratory-health-and-allergic-symptoms)
+🌍 This package is especially useful for working with geospatial data in various applications such as environmental monitoring, transportation, and location-based services.
 
 # Documentation
 
-A description of pochas-geoutils's functionality can be found [here](https://pochas-geoutils.readthedocs.io/en/latest/?badge=latest#).
+📚 For more information on how to use this package, check out the [documentation](https://pochas-geoutils.readthedocs.io/en/latest/?badge=latest#).
 
 # Installation
 
 - _GitHUB_:
-  `pip install git+https://github.com/behzad89/pochas-geoutils.git`
+  `pip install git+https://github.com/SwissTPH/pochas-geoutils.git`
 - _pip_:
   `pip install pochas-geoutils`
 
 # Tutorial
 
-A jupyter notebook and test data are available [here](https://github.com/behzad89/pochas-geoutils/tree/Tutorials/Tutorials).
+🎓 A jupyter notebook and test data are available [here](https://github.com/SwissTPH/pochas-geoutils/tree/Tutorials/Tutorials).
 
 # Dockerfile
 
-The Dockerimage to setup the **python container** is provided on the **ubuntu:20.04** environment [here](https://github.com/behzad89/pochas-geoutils/tree/main/src).
+The Dockerfile 🐳 to setup the **python container** 🐍 is provided on the **ubuntu:20.04** environment [here](https://github.com/behzad89/pochas-geoutils/tree/main/src).
+
+# Contributions
+👷‍♂️ Contributions and feedback are always welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
+# License
+📝 This package is released under the [MIT](./LICENSE)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pochas-geoutils-0.1.2/geoutils/LandsatGLAD.py` & `pochas-geoutils-0.1.3/geoutils/LandsatGLAD.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/cube.py` & `pochas-geoutils-0.1.3/geoutils/cube.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/dataClean.py` & `pochas-geoutils-0.1.3/geoutils/dataClean.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/dataExtraction.py` & `pochas-geoutils-0.1.3/geoutils/dataExtraction.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/grid.py` & `pochas-geoutils-0.1.3/geoutils/grid.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/image.py` & `pochas-geoutils-0.1.3/geoutils/image.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/modeling.py` & `pochas-geoutils-0.1.3/geoutils/modeling.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/modisAPI.py` & `pochas-geoutils-0.1.3/geoutils/modisAPI.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/geoutils/utils.py` & `pochas-geoutils-0.1.3/geoutils/utils.py`

 * *Files identical despite different names*

### Comparing `pochas-geoutils-0.1.2/setup.py` & `pochas-geoutils-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open("README.md") as f:
         README = f.read()
     return README
 
 
 setup(
     name="pochas-geoutils",
-    version="0.1.2",
+    version="0.1.3",
     description="A Python package includes geo-utils for PoCHAS project",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/behzad89/pochas-geoutils",
     author="Behzad Valipour Sh.",
     author_email="behzad.valipour@swisstph.ch",
     license="MIT",
```

