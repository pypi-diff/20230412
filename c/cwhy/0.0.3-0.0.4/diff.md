# Comparing `tmp/cwhy-0.0.3.tar.gz` & `tmp/cwhy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwhy-0.0.3.tar", last modified: Wed Apr  5 13:11:45 2023, max compression
+gzip compressed data, was "cwhy-0.0.4.tar", last modified: Wed Apr 12 18:34:07 2023, max compression
```

## Comparing `cwhy-0.0.3.tar` & `cwhy-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-05 13:11:45.978577 cwhy-0.0.3/
--rw-r--r--   0 emery      (504) staff       (20)    11357 2023-04-04 16:20:04.000000 cwhy-0.0.3/LICENSE
--rw-r--r--   0 emery      (504) staff       (20)     5588 2023-04-05 13:11:45.978443 cwhy-0.0.3/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)     4973 2023-04-04 22:06:48.000000 cwhy-0.0.3/README.md
--rw-r--r--   0 emery      (504) staff       (20)      887 2023-04-04 21:39:34.000000 cwhy-0.0.3/pyproject.toml
--rw-r--r--   0 emery      (504) staff       (20)       38 2023-04-05 13:11:45.978611 cwhy-0.0.3/setup.cfg
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-05 13:11:45.976003 cwhy-0.0.3/src/
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-05 13:11:45.977414 cwhy-0.0.3/src/cwhy/
--rw-r--r--   0 emery      (504) staff       (20)        0 2023-04-04 21:38:32.000000 cwhy-0.0.3/src/cwhy/__init__.py
--rwxr-xr-x   0 emery      (504) staff       (20)      445 2023-04-04 23:26:57.000000 cwhy-0.0.3/src/cwhy/__main__.py
--rwxr-xr-x   0 emery      (504) staff       (20)     6115 2023-04-04 23:26:57.000000 cwhy-0.0.3/src/cwhy/cwhy.py
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-05 13:11:45.978297 cwhy-0.0.3/src/cwhy.egg-info/
--rw-r--r--   0 emery      (504) staff       (20)     5588 2023-04-05 13:11:45.000000 cwhy-0.0.3/src/cwhy.egg-info/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)      285 2023-04-05 13:11:45.000000 cwhy-0.0.3/src/cwhy.egg-info/SOURCES.txt
--rw-r--r--   0 emery      (504) staff       (20)        1 2023-04-05 13:11:45.000000 cwhy-0.0.3/src/cwhy.egg-info/dependency_links.txt
--rw-r--r--   0 emery      (504) staff       (20)       44 2023-04-05 13:11:45.000000 cwhy-0.0.3/src/cwhy.egg-info/entry_points.txt
--rw-r--r--   0 emery      (504) staff       (20)       81 2023-04-05 13:11:45.000000 cwhy-0.0.3/src/cwhy.egg-info/requires.txt
--rw-r--r--   0 emery      (504) staff       (20)        5 2023-04-05 13:11:45.000000 cwhy-0.0.3/src/cwhy.egg-info/top_level.txt
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.473870 cwhy-0.0.4/
+-rw-r--r--   0 emery      (504) staff       (20)    11357 2023-04-04 16:20:04.000000 cwhy-0.0.4/LICENSE
+-rw-r--r--   0 emery      (504) staff       (20)    11083 2023-04-12 18:34:07.473717 cwhy-0.0.4/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)    10468 2023-04-11 21:33:44.000000 cwhy-0.0.4/README.md
+-rw-r--r--   0 emery      (504) staff       (20)      904 2023-04-12 18:33:53.000000 cwhy-0.0.4/pyproject.toml
+-rw-r--r--   0 emery      (504) staff       (20)       38 2023-04-12 18:34:07.473901 cwhy-0.0.4/setup.cfg
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.472376 cwhy-0.0.4/src/
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.472967 cwhy-0.0.4/src/cwhy/
+-rw-r--r--   0 emery      (504) staff       (20)        0 2023-04-12 18:32:27.000000 cwhy-0.0.4/src/cwhy/__init__.py
+-rwxr-xr-x   0 emery      (504) staff       (20)     1954 2023-04-12 18:33:36.000000 cwhy-0.0.4/src/cwhy/__main__.py
+-rwxr-xr-x   0 emery      (504) staff       (20)     7774 2023-04-12 18:20:17.000000 cwhy-0.0.4/src/cwhy/cwhy.py
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.473586 cwhy-0.0.4/src/cwhy.egg-info/
+-rw-r--r--   0 emery      (504) staff       (20)    11083 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)      285 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/SOURCES.txt
+-rw-r--r--   0 emery      (504) staff       (20)        1 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/dependency_links.txt
+-rw-r--r--   0 emery      (504) staff       (20)       44 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/entry_points.txt
+-rw-r--r--   0 emery      (504) staff       (20)       95 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/requires.txt
+-rw-r--r--   0 emery      (504) staff       (20)        5 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/top_level.txt
```

### Comparing `cwhy-0.0.3/LICENSE` & `cwhy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cwhy-0.0.3/pyproject.toml` & `cwhy-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cwhy"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
   { name="Nicolas van Kempen", email="nvankemp@gmail.com" },
   { name="Bryce Adelstein Lelbach", email="brycelelbach@gmail.com" }
 ]
-dependencies = ["openai>=0.27.0", "openai_async>=0.0.3", "rich>=12.4.4", "ast-comments>=1.0.0", "click>=8.1.3"]
+dependencies = ["openai>=0.27.0", "openai_async>=0.0.3", "rich>=12.4.4", "ast-comments>=1.0.0", "click>=8.1.3", "httpx>=0.23.3"]
 description = "Explains and proposes fixes for C/C++/Rust compiler errors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

