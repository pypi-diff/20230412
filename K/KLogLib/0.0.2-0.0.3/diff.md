# Comparing `tmp/KLogLib-0.0.2.tar.gz` & `tmp/KLogLib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KLogLib-0.0.2.tar", last modified: Wed Apr 12 10:53:48 2023, max compression
+gzip compressed data, was "KLogLib-0.0.3.tar", last modified: Wed Apr 12 11:02:52 2023, max compression
```

## Comparing `KLogLib-0.0.2.tar` & `KLogLib-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 10:53:48.213812 KLogLib-0.0.2/
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 10:53:48.213221 KLogLib-0.0.2/Handlers/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.2/Handlers/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)      264 2023-04-12 09:40:54.000000 KLogLib-0.0.2/Handlers/byte.py
--rw-r--r--   0 javier     (501) staff       (20)     2774 2023-04-12 09:40:54.000000 KLogLib-0.0.2/Handlers/files_handler.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 10:53:48.213701 KLogLib-0.0.2/KLogLib.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      106 2023-04-12 10:53:48.000000 KLogLib-0.0.2/KLogLib.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      224 2023-04-12 10:53:48.000000 KLogLib-0.0.2/KLogLib.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 10:53:48.000000 KLogLib-0.0.2/KLogLib.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)        9 2023-04-12 10:53:48.000000 KLogLib-0.0.2/KLogLib.egg-info/top_level.txt
--rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.2/LICENSE
--rw-r--r--   0 javier     (501) staff       (20)      106 2023-04-12 10:53:48.213862 KLogLib-0.0.2/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)       41 2023-04-12 09:40:54.000000 KLogLib-0.0.2/README.md
--rw-r--r--   0 javier     (501) staff       (20)       81 2023-04-12 10:53:48.214049 KLogLib-0.0.2/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      763 2023-04-12 10:53:22.000000 KLogLib-0.0.2/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.547098 KLogLib-0.0.3/
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.546045 KLogLib-0.0.3/Handlers/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.3/Handlers/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)      264 2023-04-12 09:40:54.000000 KLogLib-0.0.3/Handlers/byte.py
+-rw-r--r--   0 javier     (501) staff       (20)     2774 2023-04-12 09:40:54.000000 KLogLib-0.0.3/Handlers/files_handler.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.546541 KLogLib-0.0.3/KLog/
+-rw-r--r--   0 javier     (501) staff       (20)     1832 2023-04-12 10:31:12.000000 KLogLib-0.0.3/KLog/KLog.py
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.3/KLog/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.546986 KLogLib-0.0.3/KLogLib.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/top_level.txt
+-rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.3/LICENSE
+-rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 11:02:52.547160 KLogLib-0.0.3/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)       41 2023-04-12 09:40:54.000000 KLogLib-0.0.3/README.md
+-rw-r--r--   0 javier     (501) staff       (20)       81 2023-04-12 11:02:52.547422 KLogLib-0.0.3/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      740 2023-04-12 11:02:46.000000 KLogLib-0.0.3/setup.py
```

### Comparing `KLogLib-0.0.2/Handlers/files_handler.py` & `KLogLib-0.0.3/Handlers/files_handler.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.2/LICENSE` & `KLogLib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.2/setup.py` & `KLogLib-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 PACKAGE_NAME =  'KLogLib'
 AUTHOR = 'Javier Frias Jimenez'
 AUTHOR_EMAIL = 'javifriasj@gmail.com'
-URL = 'https://javifriasj.es' #https://github.com/javifriasj/KLog/releases/tag/0.0.1
+URL = 'https://github.com/javifriasj/KLog/releases/tag/0.0.3'
 LICENSE = 'MIT license'
 DESCRIPTION = 'Simple Log library'
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
 LONG_DESC_TYPE = "text/markdown"
 INSTALL_REQUIRES = [
 
 ]
```

