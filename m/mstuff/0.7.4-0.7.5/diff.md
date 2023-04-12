# Comparing `tmp/mstuff-0.7.4.tar.gz` & `tmp/mstuff-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mstuff-0.7.4.tar", last modified: Wed Apr 12 03:54:50 2023, max compression
+gzip compressed data, was "mstuff-0.7.5.tar", last modified: Wed Apr 12 03:56:55 2023, max compression
```

## Comparing `mstuff-0.7.4.tar` & `mstuff-0.7.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:54:50.308722 mstuff-0.7.4/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-04-12 03:54:50.308564 mstuff-0.7.4/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:02.000000 mstuff-0.7.4/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:54:50.307695 mstuff-0.7.4/mstuff/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      163 2023-03-08 18:10:18.000000 mstuff-0.7.4/mstuff/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     3837 2023-03-18 01:39:41.000000 mstuff-0.7.4/mstuff/http.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     3615 2023-03-15 21:27:41.000000 mstuff-0.7.4/mstuff/mstuff.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:54:50.308401 mstuff-0.7.4/mstuff.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-04-12 03:54:50.000000 mstuff-0.7.4/mstuff.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      225 2023-04-12 03:54:50.000000 mstuff-0.7.4/mstuff.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-04-12 03:54:50.000000 mstuff-0.7.4/mstuff.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       17 2023-04-12 03:54:50.000000 mstuff-0.7.4/mstuff.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        7 2023-04-12 03:54:50.000000 mstuff-0.7.4/mstuff.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      186 2023-04-12 03:54:46.000000 mstuff-0.7.4/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-04-12 03:54:50.308770 mstuff-0.7.4/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:56:55.359119 mstuff-0.7.5/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-04-12 03:56:55.358971 mstuff-0.7.5/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:02.000000 mstuff-0.7.5/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:56:55.358108 mstuff-0.7.5/mstuff/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      163 2023-03-08 18:10:18.000000 mstuff-0.7.5/mstuff/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     3837 2023-03-18 01:39:41.000000 mstuff-0.7.5/mstuff/http.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     3615 2023-03-15 21:27:41.000000 mstuff-0.7.5/mstuff/mstuff.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:56:55.358808 mstuff-0.7.5/mstuff.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-04-12 03:56:55.000000 mstuff-0.7.5/mstuff.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      225 2023-04-12 03:56:55.000000 mstuff-0.7.5/mstuff.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-04-12 03:56:55.000000 mstuff-0.7.5/mstuff.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       17 2023-04-12 03:56:55.000000 mstuff-0.7.5/mstuff.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        7 2023-04-12 03:56:55.000000 mstuff-0.7.5/mstuff.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      186 2023-04-12 03:56:51.000000 mstuff-0.7.5/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-04-12 03:56:55.359157 mstuff-0.7.5/setup.cfg
```

### Comparing `mstuff-0.7.4/mstuff/http.py` & `mstuff-0.7.5/mstuff/http.py`

 * *Files identical despite different names*

### Comparing `mstuff-0.7.4/mstuff/mstuff.py` & `mstuff-0.7.5/mstuff/mstuff.py`

 * *Files identical despite different names*

