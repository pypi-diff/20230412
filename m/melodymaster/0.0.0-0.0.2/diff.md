# Comparing `tmp/melodymaster-0.0.0.tar.gz` & `tmp/melodymaster-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melodymaster-0.0.0.tar", last modified: Wed Apr 12 10:01:45 2023, max compression
+gzip compressed data, was "melodymaster-0.0.2.tar", last modified: Wed Apr 12 10:29:42 2023, max compression
```

## Comparing `melodymaster-0.0.0.tar` & `melodymaster-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:01:45.842771 melodymaster-0.0.0/
--rw-rw-rw-   0        0        0     1088 2023-04-12 09:53:17.000000 melodymaster-0.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-12 10:01:45.816343 melodymaster-0.0.0/MelodyMaster/
--rw-rw-rw-   0        0        0       26 2023-04-12 09:42:14.000000 melodymaster-0.0.0/MelodyMaster/__init__.py
--rw-rw-rw-   0        0        0     5070 2023-04-12 09:40:34.000000 melodymaster-0.0.0/MelodyMaster/music.py
--rw-rw-rw-   0        0        0      470 2023-04-12 10:01:45.838883 melodymaster-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-12 09:52:56.000000 melodymaster-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:01:45.838883 melodymaster-0.0.0/melodymaster.egg-info/
--rw-rw-rw-   0        0        0      470 2023-04-12 10:01:45.000000 melodymaster-0.0.0/melodymaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-12 10:01:45.000000 melodymaster-0.0.0/melodymaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:01:45.000000 melodymaster-0.0.0/melodymaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-12 10:01:45.000000 melodymaster-0.0.0/melodymaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 10:01:45.000000 melodymaster-0.0.0/melodymaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 10:01:45.842771 melodymaster-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      869 2023-04-12 10:00:38.000000 melodymaster-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:29:42.530410 melodymaster-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-04-12 09:53:17.000000 melodymaster-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-04-12 10:29:42.501144 melodymaster-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-12 09:52:56.000000 melodymaster-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 10:29:42.462401 melodymaster-0.0.2/melodymaster/
+-rw-rw-rw-   0        0        0     5070 2023-04-12 10:17:22.000000 melodymaster-0.0.2/melodymaster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:29:42.494838 melodymaster-0.0.2/melodymaster.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-04-12 10:29:42.000000 melodymaster-0.0.2/melodymaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-12 10:29:42.000000 melodymaster-0.0.2/melodymaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:29:42.000000 melodymaster-0.0.2/melodymaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:29:42.000000 melodymaster-0.0.2/melodymaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 10:29:42.000000 melodymaster-0.0.2/melodymaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:29:42.530410 melodymaster-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-04-12 10:29:27.000000 melodymaster-0.0.2/setup.py
```

### Comparing `melodymaster-0.0.0/LICENSE` & `melodymaster-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `melodymaster-0.0.0/MelodyMaster/music.py` & `melodymaster-0.0.2/melodymaster/__init__.py`

 * *Files identical despite different names*

### Comparing `melodymaster-0.0.0/setup.py` & `melodymaster-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
-import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Downloads your favourite music'
 LONG_DESCRIPTION = 'A package that allows to download your favourite music'
 
 # Setting up
 setup(
     name="melodymaster",
+    version=VERSION,
     author="Vikranth",
     author_email="<vikrantht32@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['pytube', 'pywhatkit', 'requests', 'moviepy', 'spotipy', 'webbrowser', 'time', 'urllib'],
+    install_requires=['pytube', 'pywhatkit', 'requests', 'moviepy', 'spotipy'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

