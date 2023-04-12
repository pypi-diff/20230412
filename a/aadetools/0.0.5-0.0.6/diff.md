# Comparing `tmp/aadetools-0.0.5.tar.gz` & `tmp/aadetools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aadetools-0.0.5.tar", last modified: Wed Apr 12 19:36:24 2023, max compression
+gzip compressed data, was "aadetools-0.0.6.tar", last modified: Wed Apr 12 20:14:10 2023, max compression
```

## Comparing `aadetools-0.0.5.tar` & `aadetools-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 19:36:24.318328 aadetools-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       35 2023-03-19 10:52:53.000000 aadetools-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      521 2023-04-12 19:36:24.318328 aadetools-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 19:36:24.294769 aadetools-0.0.5/aadetools.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-12 19:36:24.000000 aadetools-0.0.5/aadetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-04-12 19:36:24.000000 aadetools-0.0.5/aadetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 19:36:24.000000 aadetools-0.0.5/aadetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-04-12 19:36:24.000000 aadetools-0.0.5/aadetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 19:36:24.000000 aadetools-0.0.5/aadetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 19:36:24.318328 aadetools-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1787 2023-04-12 19:35:08.000000 aadetools-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 19:36:24.276514 aadetools-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 19:36:24.306425 aadetools-0.0.5/src/morph/
--rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 aadetools-0.0.5/src/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 aadetools-0.0.5/src/morph/charsets.py
--rw-rw-rw-   0        0        0     2765 2023-04-11 20:43:08.000000 aadetools-0.0.5/src/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     7774 2023-04-12 18:50:43.000000 aadetools-0.0.5/src/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 aadetools-0.0.5/src/morph/settings.py
--rw-rw-rw-   0        0        0      574 2023-04-11 20:44:33.000000 aadetools-0.0.5/src/morph/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-12 19:36:24.314731 aadetools-0.0.5/src/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 aadetools-0.0.5/src/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 aadetools-0.0.5/src/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.636325 aadetools-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       35 2023-03-19 10:52:53.000000 aadetools-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      521 2023-04-12 20:14:10.633856 aadetools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.587211 aadetools-0.0.6/aadetools.egg-info/
+-rw-rw-rw-   0        0        0      521 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 20:14:10.637317 aadetools-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-04-12 20:13:56.000000 aadetools-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.563139 aadetools-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.622895 aadetools-0.0.6/src/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 aadetools-0.0.6/src/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 aadetools-0.0.6/src/morph/charsets.py
+-rw-rw-rw-   0        0        0     2765 2023-04-11 20:43:08.000000 aadetools-0.0.6/src/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     7774 2023-04-12 18:50:43.000000 aadetools-0.0.6/src/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 aadetools-0.0.6/src/morph/settings.py
+-rw-rw-rw-   0        0        0      574 2023-04-11 20:44:33.000000 aadetools-0.0.6/src/morph/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.630565 aadetools-0.0.6/src/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 aadetools-0.0.6/src/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 aadetools-0.0.6/src/parse/parser.py
```

### Comparing `aadetools-0.0.5/LICENSE.txt` & `aadetools-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.5/PKG-INFO` & `aadetools-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.0.5/aadetools.egg-info/PKG-INFO` & `aadetools-0.0.6/aadetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.0.5/setup.py` & `aadetools-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 requirements = [
-    'setuptools',
-    'pip==19.2.3',
-    'bump2version==0.5.11',
-    'wheel==0.33.6',
-    'watchdog==0.9.0',
-    'flake8==3.7.8',
-    'tox==3.14.0',
-    'coverage==4.5.4',
-    'Sphinx==6.1.3',
-    'twine==4.0.2',
     'six==1.16.0',
     'farasapy==0.0.14',
     'tqdm==4.62.2',
     'requests==2.25.1',
     'regex==2021.4.4'
 ]
 
 setup(
     name="aadetools",                     # This is the name of the package
-    version="0.0.5",                        # The initial release version
+    version="0.0.6",                        # The initial release version
     url="",                                  #
     author_email="alaa.omer2009@gmail.com",   #
     author="Alaa' Omar",                     # Full name of the author
     description="Test Package Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=find_packages(include=['src.*']),    # List of all python modules to be installed
```

### Comparing `aadetools-0.0.5/src/morph/charsets.py` & `aadetools-0.0.6/src/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.5/src/morph/lemmatizeSentence.py` & `aadetools-0.0.6/src/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.5/src/morph/morph_tagger.py` & `aadetools-0.0.6/src/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.5/src/morph/tokenizers_words.py` & `aadetools-0.0.6/src/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.5/src/parse/parser.py` & `aadetools-0.0.6/src/parse/parser.py`

 * *Files identical despite different names*

