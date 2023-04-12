# Comparing `tmp/PyLanguageEasy-1.0.0.tar.gz` & `tmp/PyLanguageEasy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLanguageEasy-1.0.0.tar", last modified: Tue Apr 11 12:14:08 2023, max compression
+gzip compressed data, was "PyLanguageEasy-1.0.1.tar", last modified: Wed Apr 12 09:14:06 2023, max compression
```

## Comparing `PyLanguageEasy-1.0.0.tar` & `PyLanguageEasy-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:14:08.829280 PyLanguageEasy-1.0.0/
--rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 PyLanguageEasy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1242 2023-04-11 12:14:08.829280 PyLanguageEasy-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 12:14:08.803838 PyLanguageEasy-1.0.0/PyLanguageEasy/
--rw-rw-rw-   0        0        0    21065 2023-04-11 11:53:52.000000 PyLanguageEasy-1.0.0/PyLanguageEasy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:14:08.822272 PyLanguageEasy-1.0.0/PyLanguageEasy.egg-info/
--rw-rw-rw-   0        0        0     1242 2023-04-11 12:14:08.000000 PyLanguageEasy-1.0.0/PyLanguageEasy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-11 12:14:08.000000 PyLanguageEasy-1.0.0/PyLanguageEasy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:14:08.000000 PyLanguageEasy-1.0.0/PyLanguageEasy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-11 12:14:08.000000 PyLanguageEasy-1.0.0/PyLanguageEasy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 12:14:08.000000 PyLanguageEasy-1.0.0/PyLanguageEasy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 PyLanguageEasy-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 12:14:08.829280 PyLanguageEasy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1596 2023-04-11 12:13:00.000000 PyLanguageEasy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:14:06.479663 PyLanguageEasy-1.0.1/
+-rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 PyLanguageEasy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1242 2023-04-12 09:14:06.476649 PyLanguageEasy-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 09:14:06.460469 PyLanguageEasy-1.0.1/PyLanguageEasy/
+-rw-rw-rw-   0        0        0    21065 2023-04-12 09:13:19.000000 PyLanguageEasy-1.0.1/PyLanguageEasy/Pylan.py
+-rw-rw-rw-   0        0        0    21065 2023-04-11 11:53:52.000000 PyLanguageEasy-1.0.1/PyLanguageEasy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:14:06.472362 PyLanguageEasy-1.0.1/PyLanguageEasy.egg-info/
+-rw-rw-rw-   0        0        0     1242 2023-04-12 09:14:06.000000 PyLanguageEasy-1.0.1/PyLanguageEasy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-04-12 09:14:06.000000 PyLanguageEasy-1.0.1/PyLanguageEasy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:14:06.000000 PyLanguageEasy-1.0.1/PyLanguageEasy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-12 09:14:06.000000 PyLanguageEasy-1.0.1/PyLanguageEasy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 09:14:06.000000 PyLanguageEasy-1.0.1/PyLanguageEasy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 PyLanguageEasy-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:14:06.479663 PyLanguageEasy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1596 2023-04-12 09:13:19.000000 PyLanguageEasy-1.0.1/setup.py
```

### Comparing `PyLanguageEasy-1.0.0/LICENSE` & `PyLanguageEasy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLanguageEasy-1.0.0/PKG-INFO` & `PyLanguageEasy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLanguageEasy
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyLanguageEasy
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan,pygame,game,image
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyLanguageEasy-1.0.0/PyLanguageEasy/__init__.py` & `PyLanguageEasy-1.0.1/PyLanguageEasy/Pylan.py`

 * *Files identical despite different names*

### Comparing `PyLanguageEasy-1.0.0/PyLanguageEasy.egg-info/PKG-INFO` & `PyLanguageEasy-1.0.1/PyLanguageEasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLanguageEasy
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyLanguageEasy
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan,pygame,game,image
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyLanguageEasy-1.0.0/README.md` & `PyLanguageEasy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PyLanguageEasy-1.0.0/setup.py` & `PyLanguageEasy-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'PyLanguageEasy'
 LONG_DESCRIPTION = """
 Easy Python Language
 
 Helps you to make python easier and more understandable
 
 some example:
@@ -36,16 +36,16 @@
     version=VERSION,
     author="Developer HelloUsers",
     author_email="duartesaopedrocat1@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=["pygame", "Pillow", "pyttsx3", "SpeechRecognition", "datetime", "keyboard", "termcolor"],
-    keywords=['python', 'Pylan', 'pylan', 'EasyPython', 'EasyPyLan', "easypylan", "pygame", "game", "image"],
+    install_requires=['pygame', 'Pillow', 'pyttsx3', 'SpeechRecognition', 'datetime', 'keyboard', 'termcolor'],
+    keywords=['python', 'Pylan', 'pylan', 'EasyPython', 'EasyPyLan', 'easypylan', 'pygame', 'game', 'image'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

