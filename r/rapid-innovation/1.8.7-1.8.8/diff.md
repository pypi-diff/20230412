# Comparing `tmp/rapid_innovation-1.8.7.tar.gz` & `tmp/rapid_innovation-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapid_innovation-1.8.7.tar", last modified: Thu Apr  6 10:36:51 2023, max compression
+gzip compressed data, was "rapid_innovation-1.8.8.tar", last modified: Wed Apr 12 04:52:35 2023, max compression
```

## Comparing `rapid_innovation-1.8.7.tar` & `rapid_innovation-1.8.8.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-06 10:36:51.107250 rapid_innovation-1.8.7/
--rw-r--r--   0 abhisheknegi   (501) staff       (20)     1069 2023-04-03 08:08:45.000000 rapid_innovation-1.8.7/LICENSE
--rw-r--r--   0 abhisheknegi   (501) staff       (20)     1361 2023-04-06 10:36:51.107079 rapid_innovation-1.8.7/PKG-INFO
--rw-r--r--   0 abhisheknegi   (501) staff       (20)      886 2023-04-06 10:33:58.000000 rapid_innovation-1.8.7/README.md
-drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-06 10:36:51.106057 rapid_innovation-1.8.7/rapid/
--rw-r--r--   0 abhisheknegi   (501) staff       (20)        0 2023-04-03 08:10:44.000000 rapid_innovation-1.8.7/rapid/__init__.py
--rw-r--r--   0 abhisheknegi   (501) staff       (20)     4715 2023-04-06 10:26:52.000000 rapid_innovation-1.8.7/rapid/email.py
-drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-06 10:36:51.106863 rapid_innovation-1.8.7/rapid_innovation.egg-info/
--rw-r--r--   0 abhisheknegi   (501) staff       (20)     1361 2023-04-06 10:36:51.000000 rapid_innovation-1.8.7/rapid_innovation.egg-info/PKG-INFO
--rw-r--r--   0 abhisheknegi   (501) staff       (20)      219 2023-04-06 10:36:51.000000 rapid_innovation-1.8.7/rapid_innovation.egg-info/SOURCES.txt
--rw-r--r--   0 abhisheknegi   (501) staff       (20)        1 2023-04-06 10:36:51.000000 rapid_innovation-1.8.7/rapid_innovation.egg-info/dependency_links.txt
--rw-r--r--   0 abhisheknegi   (501) staff       (20)        6 2023-04-06 10:36:51.000000 rapid_innovation-1.8.7/rapid_innovation.egg-info/top_level.txt
--rw-r--r--   0 abhisheknegi   (501) staff       (20)       38 2023-04-06 10:36:51.107308 rapid_innovation-1.8.7/setup.cfg
--rw-r--r--   0 abhisheknegi   (501) staff       (20)     1024 2023-04-06 10:34:46.000000 rapid_innovation-1.8.7/setup.py
+drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-12 04:52:35.912436 rapid_innovation-1.8.8/
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)     1069 2023-04-03 08:08:45.000000 rapid_innovation-1.8.8/LICENSE
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)       85 2023-04-12 04:51:18.000000 rapid_innovation-1.8.8/MANIFEST.in
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)     1362 2023-04-12 04:52:35.912274 rapid_innovation-1.8.8/PKG-INFO
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)      888 2023-04-06 10:41:13.000000 rapid_innovation-1.8.8/README.md
+drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-12 04:52:35.910594 rapid_innovation-1.8.8/rapid/
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)        0 2023-04-03 08:10:44.000000 rapid_innovation-1.8.8/rapid/__init__.py
+drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-12 04:52:35.909441 rapid_innovation-1.8.8/rapid/app/
+drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-12 04:52:35.910981 rapid_innovation-1.8.8/rapid/app/exceptions/
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)        0 2023-04-03 08:11:50.000000 rapid_innovation-1.8.8/rapid/app/exceptions/__init__.py
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)      725 2023-04-06 09:40:49.000000 rapid_innovation-1.8.8/rapid/app/exceptions/email_exception.py
+drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-12 04:52:35.911343 rapid_innovation-1.8.8/rapid/app/helpers/
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)        0 2023-04-03 08:12:01.000000 rapid_innovation-1.8.8/rapid/app/helpers/__init__.py
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)      388 2023-04-06 09:43:08.000000 rapid_innovation-1.8.8/rapid/app/helpers/validator.py
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)     4715 2023-04-06 10:26:52.000000 rapid_innovation-1.8.8/rapid/email.py
+drwxr-xr-x   0 abhisheknegi   (501) staff       (20)        0 2023-04-12 04:52:35.912066 rapid_innovation-1.8.8/rapid_innovation.egg-info/
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)     1362 2023-04-12 04:52:35.000000 rapid_innovation-1.8.8/rapid_innovation.egg-info/PKG-INFO
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)      365 2023-04-12 04:52:35.000000 rapid_innovation-1.8.8/rapid_innovation.egg-info/SOURCES.txt
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)        1 2023-04-12 04:52:35.000000 rapid_innovation-1.8.8/rapid_innovation.egg-info/dependency_links.txt
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)        6 2023-04-12 04:52:35.000000 rapid_innovation-1.8.8/rapid_innovation.egg-info/top_level.txt
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)       38 2023-04-12 04:52:35.912490 rapid_innovation-1.8.8/setup.cfg
+-rw-r--r--   0 abhisheknegi   (501) staff       (20)     1024 2023-04-12 04:52:33.000000 rapid_innovation-1.8.8/setup.py
```

### Comparing `rapid_innovation-1.8.7/LICENSE` & `rapid_innovation-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rapid_innovation-1.8.7/PKG-INFO` & `rapid_innovation-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid_innovation
-Version: 1.8.7
+Version: 1.8.8
 Summary: Rapid Innovation package
 Home-page: https://github.com/Rapid-Python/python-package-rapid
 Author: Abhishek Negi
 Author-email: abhisheknegi@rapidinnovation.dev
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -42,7 +42,8 @@
         renstmp.send_email(to, subject, content)
 
 
 
 ## License
 
 Rapid Innovation is released under the MIT License.
+
```

### Comparing `rapid_innovation-1.8.7/README.md` & `rapid_innovation-1.8.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,8 +26,9 @@
         
         renstmp.send_email(to, subject, content)
 
 
 
 ## License
 
-Rapid Innovation is released under the MIT License.
+Rapid Innovation is released under the MIT License.
+
```

### Comparing `rapid_innovation-1.8.7/rapid/email.py` & `rapid_innovation-1.8.8/rapid/email.py`

 * *Files identical despite different names*

### Comparing `rapid_innovation-1.8.7/rapid_innovation.egg-info/PKG-INFO` & `rapid_innovation-1.8.8/rapid_innovation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-innovation
-Version: 1.8.7
+Version: 1.8.8
 Summary: Rapid Innovation package
 Home-page: https://github.com/Rapid-Python/python-package-rapid
 Author: Abhishek Negi
 Author-email: abhisheknegi@rapidinnovation.dev
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -42,7 +42,8 @@
         renstmp.send_email(to, subject, content)
 
 
 
 ## License
 
 Rapid Innovation is released under the MIT License.
+
```

### Comparing `rapid_innovation-1.8.7/setup.py` & `rapid_innovation-1.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 # Define the package metadata
 metadata = {
     "name": "rapid_innovation",
-    "version": "1.8.7",
+    "version": "1.8.8",
     "description": "Rapid Innovation package",
     "long_description": open("README.md", "r").read(),
     "long_description_content_type": "text/markdown",
     "url": "https://github.com/Rapid-Python/python-package-rapid",
     "author": "Abhishek Negi",
     "author_email": "abhisheknegi@rapidinnovation.dev",
     "license": "MIT",
```

