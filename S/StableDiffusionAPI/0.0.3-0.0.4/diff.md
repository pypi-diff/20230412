# Comparing `tmp/StableDiffusionAPI-0.0.3.tar.gz` & `tmp/StableDiffusionAPI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StableDiffusionAPI-0.0.3.tar", last modified: Wed Apr 12 07:54:07 2023, max compression
+gzip compressed data, was "StableDiffusionAPI-0.0.4.tar", last modified: Wed Apr 12 15:49:51 2023, max compression
```

## Comparing `StableDiffusionAPI-0.0.3.tar` & `StableDiffusionAPI-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:07.025546 StableDiffusionAPI-0.0.3/
--rw-rw-rw-   0        0        0     2185 2023-04-10 10:15:54.000000 StableDiffusionAPI-0.0.3/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-10 23:23:24.000000 StableDiffusionAPI-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      923 2023-04-12 07:54:07.025546 StableDiffusionAPI-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-04-12 07:52:41.000000 StableDiffusionAPI-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:07.019158 StableDiffusionAPI-0.0.3/StableDiffusionAPI/
--rw-rw-rw-   0        0        0      125 2023-04-12 07:46:30.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/SetKey.py
--rw-rw-rw-   0        0        0     4013 2023-04-12 07:45:58.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/Text2Img.py
--rw-rw-rw-   0        0        0      144 2023-04-12 07:53:33.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/__init__.py
--rw-rw-rw-   0        0        0       30 2023-04-12 07:45:34.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/__main__.py
--rw-rw-rw-   0        0        0      115 2023-04-12 07:46:13.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/key.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:07.024545 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      790 2023-04-12 07:51:03.000000 StableDiffusionAPI-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 07:54:07.025546 StableDiffusionAPI-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 15:49:51.508899 StableDiffusionAPI-0.0.4/
+-rw-rw-rw-   0        0        0     2185 2023-04-10 10:15:54.000000 StableDiffusionAPI-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-10 23:23:24.000000 StableDiffusionAPI-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      923 2023-04-12 15:49:51.508899 StableDiffusionAPI-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-04-12 07:52:41.000000 StableDiffusionAPI-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 15:49:51.503900 StableDiffusionAPI-0.0.4/StableDiffusionAPI/
+-rw-rw-rw-   0        0        0       96 2023-04-12 13:09:21.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/SetKey.py
+-rw-rw-rw-   0        0        0     5105 2023-04-12 15:43:25.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/Text2Img.py
+-rw-rw-rw-   0        0        0      144 2023-04-12 07:53:33.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-12 07:45:34.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/__main__.py
+-rw-rw-rw-   0        0        0      115 2023-04-12 07:46:13.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/key.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:49:51.507900 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      790 2023-04-12 15:49:14.000000 StableDiffusionAPI-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 15:49:51.509899 StableDiffusionAPI-0.0.4/setup.cfg
```

### Comparing `StableDiffusionAPI-0.0.3/LICENSE` & `StableDiffusionAPI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `StableDiffusionAPI-0.0.3/PKG-INFO` & `StableDiffusionAPI-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableDiffusionAPI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to interface with the StableDiffusionAPI.com API
 Author-email: Jonathan Caraveo <jon@ziawe.com>
 Project-URL: Homepage, https://StableDiffusionAPI.com
 Project-URL: GitHub, https://github.com/caraveo/SDAPI/
 Project-URL: Bug Tracker, https://github.com/Caraveo/SDAPI/issues
 Project-URL: Guide, https://www.sparkandwave.com/stablediffusionapi/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/PKG-INFO` & `StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableDiffusionAPI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to interface with the StableDiffusionAPI.com API
 Author-email: Jonathan Caraveo <jon@ziawe.com>
 Project-URL: Homepage, https://StableDiffusionAPI.com
 Project-URL: GitHub, https://github.com/caraveo/SDAPI/
 Project-URL: Bug Tracker, https://github.com/Caraveo/SDAPI/issues
 Project-URL: Guide, https://www.sparkandwave.com/stablediffusionapi/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `StableDiffusionAPI-0.0.3/pyproject.toml` & `StableDiffusionAPI-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 install_requires = ['random', 'json', 'time', 'urllib3', 'http.client']
 build-backend = "setuptools.build_meta"
 [project]
 name = "StableDiffusionAPI"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jonathan Caraveo", email="jon@ziawe.com" },
 ]
 description = "A package to interface with the StableDiffusionAPI.com API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

