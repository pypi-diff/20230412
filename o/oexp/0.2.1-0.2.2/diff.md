# Comparing `tmp/oexp-0.2.1.tar.gz` & `tmp/oexp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.2.1.tar", last modified: Wed Apr 12 03:55:29 2023, max compression
+gzip compressed data, was "oexp-0.2.2.tar", last modified: Wed Apr 12 04:06:24 2023, max compression
```

## Comparing `oexp-0.2.1.tar` & `oexp-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:55:29.269041 oexp-0.2.1/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-04-12 03:55:29.268878 oexp-0.2.1/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.2.1/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:55:29.268032 oexp-0.2.1/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      127 2023-03-14 19:30:00.000000 oexp-0.2.1/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)      399 2023-03-18 02:41:19.000000 oexp-0.2.1/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     7596 2023-03-31 14:49:58.000000 oexp-0.2.1/oexp/oexp.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 03:55:29.268717 oexp-0.2.1/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-04-12 03:55:29.000000 oexp-0.2.1/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      206 2023-04-12 03:55:29.000000 oexp-0.2.1/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-04-12 03:55:29.000000 oexp-0.2.1/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-04-12 03:55:29.000000 oexp-0.2.1/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-04-12 03:55:29.000000 oexp-0.2.1/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-04-12 03:55:25.000000 oexp-0.2.1/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-04-12 03:55:29.269093 oexp-0.2.1/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:06:24.622341 oexp-0.2.2/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-04-12 04:06:24.622179 oexp-0.2.2/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.2.2/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:06:24.621272 oexp-0.2.2/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      127 2023-03-14 19:30:00.000000 oexp-0.2.2/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)      399 2023-03-18 02:41:19.000000 oexp-0.2.2/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     7596 2023-03-31 14:49:58.000000 oexp-0.2.2/oexp/oexp.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:06:24.622013 oexp-0.2.2/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      206 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-04-12 04:06:20.000000 oexp-0.2.2/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-04-12 04:06:24.622382 oexp-0.2.2/setup.cfg
```

### Comparing `oexp-0.2.1/oexp/oexp.py` & `oexp-0.2.2/oexp/oexp.py`

 * *Files identical despite different names*

