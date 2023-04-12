# Comparing `tmp/airlabs-0.0.5.tar.gz` & `tmp/airlabs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlabs-0.0.5.tar", last modified: Wed Apr 12 12:41:53 2023, max compression
+gzip compressed data, was "airlabs-0.0.6.tar", last modified: Wed Apr 12 15:33:48 2023, max compression
```

## Comparing `airlabs-0.0.5.tar` & `airlabs-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 12:41:53.460006 airlabs-0.0.5/
--rw-rw-rw-   0        0        0     1087 2023-04-12 12:16:51.000000 airlabs-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       57 2023-04-12 12:16:51.000000 airlabs-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1662 2023-04-12 12:41:53.460006 airlabs-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1183 2023-04-12 12:16:51.000000 airlabs-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 12:41:53.460006 airlabs-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-04-12 12:30:56.000000 airlabs-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:41:53.359690 airlabs-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 12:41:53.397876 airlabs-0.0.5/src/airlabs/
--rw-rw-rw-   0        0        0       35 2023-04-12 12:17:23.000000 airlabs-0.0.5/src/airlabs/__init__.py
--rw-rw-rw-   0        0        0     9455 2023-04-12 12:16:51.000000 airlabs-0.0.5/src/airlabs/endpoints.py
--rw-rw-rw-   0        0        0      460 2023-04-12 12:16:51.000000 airlabs-0.0.5/src/airlabs/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:41:53.451038 airlabs-0.0.5/src/airlabs.egg-info/
--rw-rw-rw-   0        0        0     1662 2023-04-12 12:41:53.000000 airlabs-0.0.5/src/airlabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-04-12 12:41:53.000000 airlabs-0.0.5/src/airlabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 12:41:53.000000 airlabs-0.0.5/src/airlabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 12:41:53.000000 airlabs-0.0.5/src/airlabs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      168 2023-04-12 12:30:53.000000 airlabs-0.0.5/versions.md
+drwxrwxrwx   0        0        0        0 2023-04-12 15:33:48.919263 airlabs-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-12 12:16:51.000000 airlabs-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-04-12 12:16:51.000000 airlabs-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1662 2023-04-12 15:33:48.919263 airlabs-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1183 2023-04-12 15:32:24.000000 airlabs-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 15:33:48.919263 airlabs-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-04-12 15:26:26.000000 airlabs-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:33:48.761897 airlabs-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:33:48.810287 airlabs-0.0.6/src/airlabs/
+-rw-rw-rw-   0        0        0       35 2023-04-12 12:17:23.000000 airlabs-0.0.6/src/airlabs/__init__.py
+-rw-rw-rw-   0        0        0     9476 2023-04-12 15:23:54.000000 airlabs-0.0.6/src/airlabs/endpoints.py
+-rw-rw-rw-   0        0        0      460 2023-04-12 12:16:51.000000 airlabs-0.0.6/src/airlabs/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:33:48.917317 airlabs-0.0.6/src/airlabs.egg-info/
+-rw-rw-rw-   0        0        0     1662 2023-04-12 15:33:48.000000 airlabs-0.0.6/src/airlabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-12 15:33:48.000000 airlabs-0.0.6/src/airlabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:33:48.000000 airlabs-0.0.6/src/airlabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 15:33:48.000000 airlabs-0.0.6/src/airlabs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-04-12 15:27:03.000000 airlabs-0.0.6/versions.md
```

### Comparing `airlabs-0.0.5/LICENSE` & `airlabs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airlabs-0.0.5/PKG-INFO` & `airlabs-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airlabs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python wrapper for AirLabs
 Home-page: https://github.com/calebyhan/AirLabs
 Author: Caleb Han
 Author-email: calebhantech@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `airlabs-0.0.5/README.md` & `airlabs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `airlabs-0.0.5/setup.py` & `airlabs-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="airlabs",
-    version="0.0.5",
+    version="0.0.6",
     description="Python wrapper for AirLabs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/calebyhan/AirLabs",
     author="Caleb Han",
     author_email="calebhantech@gmail.com",
     license="MIT",
```

### Comparing `airlabs-0.0.5/src/airlabs/endpoints.py` & `airlabs-0.0.6/src/airlabs/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import functions
+import airlabs.functions as functions
 import requests
 
 
 class API:
     def __init__(self, api_key: str):
         """
         Instantiation to input api key.
```

### Comparing `airlabs-0.0.5/src/airlabs.egg-info/PKG-INFO` & `airlabs-0.0.6/src/airlabs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airlabs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python wrapper for AirLabs
 Home-page: https://github.com/calebyhan/AirLabs
 Author: Caleb Han
 Author-email: calebhantech@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

