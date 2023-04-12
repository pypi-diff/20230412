# Comparing `tmp/airlabs-0.0.3.tar.gz` & `tmp/airlabs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlabs-0.0.3.tar", last modified: Wed Apr 12 00:21:21 2023, max compression
+gzip compressed data, was "airlabs-0.0.4.tar", last modified: Wed Apr 12 12:21:05 2023, max compression
```

## Comparing `airlabs-0.0.3.tar` & `airlabs-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.981094 airlabs-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-04-11 20:29:40.000000 airlabs-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       57 2023-04-11 20:29:40.000000 airlabs-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1419 2023-04-12 00:21:21.980097 airlabs-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      943 2023-04-12 00:20:26.000000 airlabs-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 00:21:21.981094 airlabs-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-04-12 00:20:39.000000 airlabs-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.971121 airlabs-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.977105 airlabs-0.0.3/src/airlabs/
--rw-rw-rw-   0        0        0       27 2023-04-11 20:29:40.000000 airlabs-0.0.3/src/airlabs/__init__.py
--rw-rw-rw-   0        0        0     9455 2023-04-11 23:44:56.000000 airlabs-0.0.3/src/airlabs/endpoints.py
--rw-rw-rw-   0        0        0      460 2023-04-11 23:30:26.000000 airlabs-0.0.3/src/airlabs/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.979099 airlabs-0.0.3/src/airlabs.egg-info/
--rw-rw-rw-   0        0        0     1419 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      109 2023-04-12 00:20:51.000000 airlabs-0.0.3/versions.md
+drwxrwxrwx   0        0        0        0 2023-04-12 12:21:05.906831 airlabs-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-12 12:16:51.000000 airlabs-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-04-12 12:16:51.000000 airlabs-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1662 2023-04-12 12:21:05.904611 airlabs-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1183 2023-04-12 12:16:51.000000 airlabs-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 12:21:05.906831 airlabs-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-04-12 12:17:55.000000 airlabs-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:21:05.808922 airlabs-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 12:21:05.849318 airlabs-0.0.4/src/airlabs/
+-rw-rw-rw-   0        0        0       35 2023-04-12 12:17:23.000000 airlabs-0.0.4/src/airlabs/__init__.py
+-rw-rw-rw-   0        0        0     9455 2023-04-12 12:16:51.000000 airlabs-0.0.4/src/airlabs/endpoints.py
+-rw-rw-rw-   0        0        0      460 2023-04-12 12:16:51.000000 airlabs-0.0.4/src/airlabs/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:21:05.901591 airlabs-0.0.4/src/airlabs.egg-info/
+-rw-rw-rw-   0        0        0     1662 2023-04-12 12:21:05.000000 airlabs-0.0.4/src/airlabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-12 12:21:05.000000 airlabs-0.0.4/src/airlabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 12:21:05.000000 airlabs-0.0.4/src/airlabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 12:21:05.000000 airlabs-0.0.4/src/airlabs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-04-12 12:17:52.000000 airlabs-0.0.4/versions.md
```

### Comparing `airlabs-0.0.3/LICENSE` & `airlabs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airlabs-0.0.3/PKG-INFO` & `airlabs-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: airlabs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for AirLabs
 Home-page: https://github.com/calebyhan/AirLabs
 Author: Caleb Han
 Author-email: calebhantech@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **Project Portfolio: https://github.com/calebyhan/CalebHan**
 
+[![PyPI version](https://badge.fury.io/py/airlabs.svg)](https://badge.fury.io/py/airlabs)
+[![Documentation Status](https://readthedocs.org/projects/airlabs/badge/?version=latest)](https://airlabs.readthedocs.io/en/latest/?badge=latest)
+
 # airlabs
 
 Python wrapper for [AirLabs](https://airlabs.co/).
 
 
 ## Installation
 ----------------------
```

### Comparing `airlabs-0.0.3/README.md` & `airlabs-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 **Project Portfolio: https://github.com/calebyhan/CalebHan**
 
+[![PyPI version](https://badge.fury.io/py/airlabs.svg)](https://badge.fury.io/py/airlabs)
+[![Documentation Status](https://readthedocs.org/projects/airlabs/badge/?version=latest)](https://airlabs.readthedocs.io/en/latest/?badge=latest)
+
 # airlabs
 
 Python wrapper for [AirLabs](https://airlabs.co/).
 
 
 ## Installation
 ----------------------
```

### Comparing `airlabs-0.0.3/setup.py` & `airlabs-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="airlabs",
-    version="0.0.3",
+    version="0.0.4",
     description="Python wrapper for AirLabs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/calebyhan/AirLabs",
     author="Caleb Han",
     author_email="calebhantech@gmail.com",
     license="MIT",
```

### Comparing `airlabs-0.0.3/src/airlabs/endpoints.py` & `airlabs-0.0.4/src/airlabs/endpoints.py`

 * *Files identical despite different names*

### Comparing `airlabs-0.0.3/src/airlabs.egg-info/PKG-INFO` & `airlabs-0.0.4/src/airlabs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: airlabs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for AirLabs
 Home-page: https://github.com/calebyhan/AirLabs
 Author: Caleb Han
 Author-email: calebhantech@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **Project Portfolio: https://github.com/calebyhan/CalebHan**
 
+[![PyPI version](https://badge.fury.io/py/airlabs.svg)](https://badge.fury.io/py/airlabs)
+[![Documentation Status](https://readthedocs.org/projects/airlabs/badge/?version=latest)](https://airlabs.readthedocs.io/en/latest/?badge=latest)
+
 # airlabs
 
 Python wrapper for [AirLabs](https://airlabs.co/).
 
 
 ## Installation
 ----------------------
```

