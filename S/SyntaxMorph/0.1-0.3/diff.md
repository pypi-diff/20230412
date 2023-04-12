# Comparing `tmp/SyntaxMorph-0.1.tar.gz` & `tmp/SyntaxMorph-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SyntaxMorph-0.1.tar", last modified: Wed Apr 12 18:30:48 2023, max compression
+gzip compressed data, was "SyntaxMorph-0.3.tar", last modified: Wed Apr 12 18:44:40 2023, max compression
```

## Comparing `SyntaxMorph-0.1.tar` & `SyntaxMorph-0.3.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxrwxr-x   0 marijua   (1000) marijua   (1000)        0 2023-04-12 18:30:48.015631 SyntaxMorph-0.1/
--rw-rw-r--   0 marijua   (1000) marijua   (1000)     1235 2023-04-12 18:30:48.015631 SyntaxMorph-0.1/PKG-INFO
-drwxrwxr-x   0 marijua   (1000) marijua   (1000)        0 2023-04-12 18:30:48.015631 SyntaxMorph-0.1/SyntaxMorph.egg-info/
--rw-rw-r--   0 marijua   (1000) marijua   (1000)     1235 2023-04-12 18:30:47.000000 SyntaxMorph-0.1/SyntaxMorph.egg-info/PKG-INFO
--rw-rw-r--   0 marijua   (1000) marijua   (1000)      182 2023-04-12 18:30:47.000000 SyntaxMorph-0.1/SyntaxMorph.egg-info/SOURCES.txt
--rw-rw-r--   0 marijua   (1000) marijua   (1000)        1 2023-04-12 18:30:47.000000 SyntaxMorph-0.1/SyntaxMorph.egg-info/dependency_links.txt
--rw-rw-r--   0 marijua   (1000) marijua   (1000)       13 2023-04-12 18:30:47.000000 SyntaxMorph-0.1/SyntaxMorph.egg-info/requires.txt
--rw-rw-r--   0 marijua   (1000) marijua   (1000)        1 2023-04-12 18:30:47.000000 SyntaxMorph-0.1/SyntaxMorph.egg-info/top_level.txt
--rw-rw-r--   0 marijua   (1000) marijua   (1000)       38 2023-04-12 18:30:48.015631 SyntaxMorph-0.1/setup.cfg
--rw-rw-r--   0 marijua   (1000) marijua   (1000)     1441 2023-04-12 18:29:12.000000 SyntaxMorph-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 18:44:40.229956 SyntaxMorph-0.3/
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-04-12 18:44:40.225956 SyntaxMorph-0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 18:44:40.225956 SyntaxMorph-0.3/SyntaxMorph.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     1235 2023-04-12 18:44:40.000000 SyntaxMorph-0.3/SyntaxMorph.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-04-12 18:44:40.000000 SyntaxMorph-0.3/SyntaxMorph.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-12 18:44:40.000000 SyntaxMorph-0.3/SyntaxMorph.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-04-12 18:44:40.000000 SyntaxMorph-0.3/SyntaxMorph.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-04-12 18:44:40.000000 SyntaxMorph-0.3/SyntaxMorph.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 18:44:40.225956 SyntaxMorph-0.3/morph/
+-rw-rw-r--   0 root         (0) root         (0)     2249 2023-04-12 18:29:35.000000 SyntaxMorph-0.3/morph/columDetect.py
+-rw-rw-r--   0 root         (0) root         (0)     1995 2023-04-12 18:13:50.000000 SyntaxMorph-0.3/morph/formatCode.py
+-rw-rw-r--   0 root         (0) root         (0)     3639 2023-04-12 18:29:54.000000 SyntaxMorph-0.3/morph/languageDetect.py
+-rw-rw-r--   0 root         (0) root         (0)      808 2023-04-12 18:39:46.000000 SyntaxMorph-0.3/morph/main.py
+-rw-rw-r--   0 root         (0) root         (0)     5999 2023-04-12 18:29:42.000000 SyntaxMorph-0.3/morph/translate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 18:44:40.229956 SyntaxMorph-0.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1408 2023-04-12 18:42:45.000000 SyntaxMorph-0.3/setup.py
```

### Comparing `SyntaxMorph-0.1/PKG-INFO` & `SyntaxMorph-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SyntaxMorph
-Version: 0.1
+Version: 0.3
 Summary: SyntaxMorph is a Python module that enables code conversion between different programming languages
 Home-page: https://github.com/Enderjua/SyntaxMorph
 Author: Marijua
 Author-email: enderjua@gmail.com
 License: UNKNOWN
 Description: 
         SyntaxMorph is a Python module that enables code conversion between different programming languages using the OpenAI API. It uses advanced deep learning algorithms to ensure that the functionality and structural integrity of the code are preserved during the conversion process. Users simply need to provide the source code and the target programming language to SyntaxMorph, and it automatically analyzes and converts the code to the target language.
```

### Comparing `SyntaxMorph-0.1/SyntaxMorph.egg-info/PKG-INFO` & `SyntaxMorph-0.3/SyntaxMorph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SyntaxMorph
-Version: 0.1
+Version: 0.3
 Summary: SyntaxMorph is a Python module that enables code conversion between different programming languages
 Home-page: https://github.com/Enderjua/SyntaxMorph
 Author: Marijua
 Author-email: enderjua@gmail.com
 License: UNKNOWN
 Description: 
         SyntaxMorph is a Python module that enables code conversion between different programming languages using the OpenAI API. It uses advanced deep learning algorithms to ensure that the functionality and structural integrity of the code are preserved during the conversion process. Users simply need to provide the source code and the target programming language to SyntaxMorph, and it automatically analyzes and converts the code to the target language.
```

### Comparing `SyntaxMorph-0.1/setup.py` & `SyntaxMorph-0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup
-import setuptools
 
 long_description = """
 SyntaxMorph is a Python module that enables code conversion between different programming languages using the OpenAI API. It uses advanced deep learning algorithms to ensure that the functionality and structural integrity of the code are preserved during the conversion process. Users simply need to provide the source code and the target programming language to SyntaxMorph, and it automatically analyzes and converts the code to the target language.
 
 SyntaxMorph offers developers a significant advantage in terms of speeding up the code conversion process between different programming languages. With this module, developers can complete their projects more efficiently and effectively."""
 
 
 setup(
     name="SyntaxMorph",
-    version="0.1",
+    version="0.3",
     author="Marijua",
     author_email="enderjua@gmail.com",
     description="SyntaxMorph is a Python module that enables code conversion between different programming languages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Enderjua/SyntaxMorph",
-    packages=setuptools.find_packages(),
+    packages = ['morph'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
```

