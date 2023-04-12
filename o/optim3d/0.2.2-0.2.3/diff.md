# Comparing `tmp/optim3d-0.2.2.tar.gz` & `tmp/optim3d-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\optim3d-0.2.2.tar", last modified: Wed Apr 12 14:18:22 2023, max compression
+gzip compressed data, was "dist\optim3d-0.2.3.tar", last modified: Wed Apr 12 14:25:44 2023, max compression
```

## Comparing `optim3d-0.2.2.tar` & `optim3d-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:18:22.000000 optim3d-0.2.2/
--rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.2/COPYING
--rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-12 14:18:22.000000 optim3d-0.2.2/optim3d.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-12 14:18:22.000000 optim3d-0.2.2/optim3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-12 14:18:22.000000 optim3d-0.2.2/optim3d.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    14778 2023-04-12 14:18:22.000000 optim3d-0.2.2/optim3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-12 14:18:22.000000 optim3d-0.2.2/optim3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0      222 2023-04-12 14:18:22.000000 optim3d-0.2.2/optim3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 14:18:22.000000 optim3d-0.2.2/optim3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14778 2023-04-12 14:18:22.000000 optim3d-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    13741 2023-04-12 14:06:45.000000 optim3d-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 14:18:22.000000 optim3d-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-04-12 14:17:44.000000 optim3d-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:25:44.000000 optim3d-0.2.3/
+-rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.3/COPYING
+-rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-12 14:25:44.000000 optim3d-0.2.3/optim3d.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:25:44.000000 optim3d-0.2.3/optim3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-12 14:25:44.000000 optim3d-0.2.3/optim3d.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    14779 2023-04-12 14:25:44.000000 optim3d-0.2.3/optim3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-12 14:25:44.000000 optim3d-0.2.3/optim3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      222 2023-04-12 14:25:44.000000 optim3d-0.2.3/optim3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:25:44.000000 optim3d-0.2.3/optim3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14779 2023-04-12 14:25:44.000000 optim3d-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13741 2023-04-12 14:06:45.000000 optim3d-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:25:44.000000 optim3d-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      775 2023-04-12 14:25:31.000000 optim3d-0.2.3/setup.py
```

### Comparing `optim3d-0.2.2/COPYING` & `optim3d-0.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.2/LICENSE` & `optim3d-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.2/optim3d.egg-info/PKG-INFO` & `optim3d-0.2.3/optim3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.2
-Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models
+Version: 0.2.3
+Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optim3d-0.2.2/PKG-INFO` & `optim3d-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.2
-Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models
+Version: 0.2.3
+Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optim3d-0.2.2/README.md` & `optim3d-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.2/setup.py` & `optim3d-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="optim3d",
-    version='0.2.2',
-    description="CLI application for efficient and optimized reconstruction of large-scale 3D building models",
+    version='0.2.3',
+    description="CLI application for efficient and optimized reconstruction of large-scale 3D building models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author = 'Anass Yarroudh',
     author_email = 'ayarroudh@uliege.be',
     url = 'https://github.com/Yarroudh/Optim3D',
     packages=find_packages(),
-    py_modules=["optim3d"],
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "optim3d=optim3d.main:cli"
         ]
     },
      package_data={
```

