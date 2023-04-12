# Comparing `tmp/astro_hh-0.0.3.tar.gz` & `tmp/astro_hh-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_hh-0.0.3.tar", last modified: Wed Apr 12 11:22:34 2023, max compression
+gzip compressed data, was "astro_hh-0.0.4.tar", last modified: Wed Apr 12 11:26:20 2023, max compression
```

## Comparing `astro_hh-0.0.3.tar` & `astro_hh-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 11:22:34.978635 astro_hh-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-12 08:42:42.000000 astro_hh-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      416 2023-04-12 11:22:34.977635 astro_hh-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-12 08:41:29.000000 astro_hh-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 11:22:34.972634 astro_hh-0.0.3/astro_hh/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:19:40.000000 astro_hh-0.0.3/astro_hh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:22:34.976636 astro_hh-0.0.3/astro_hh/ccd/
--rw-rw-rw-   0        0        0       49 2023-04-12 09:43:00.000000 astro_hh-0.0.3/astro_hh/ccd/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-07 08:39:02.000000 astro_hh-0.0.3/astro_hh/ccd/ccd_io.py
--rw-rw-rw-   0        0        0     2863 2023-04-11 14:18:16.000000 astro_hh-0.0.3/astro_hh/ccd/ccd_process.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:22:34.975635 astro_hh-0.0.3/astro_hh.egg-info/
--rw-rw-rw-   0        0        0      416 2023-04-12 11:22:34.000000 astro_hh-0.0.3/astro_hh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-12 11:22:34.000000 astro_hh-0.0.3/astro_hh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 11:22:34.000000 astro_hh-0.0.3/astro_hh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 11:22:34.000000 astro_hh-0.0.3/astro_hh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 11:22:34.978635 astro_hh-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-04-12 10:44:45.000000 astro_hh-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:26:20.389129 astro_hh-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-12 08:42:42.000000 astro_hh-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      416 2023-04-12 11:26:20.388130 astro_hh-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-12 08:41:29.000000 astro_hh-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 11:26:20.384127 astro_hh-0.0.4/astro_hh/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:19:40.000000 astro_hh-0.0.4/astro_hh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:26:20.388130 astro_hh-0.0.4/astro_hh/ccd/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:25:22.000000 astro_hh-0.0.4/astro_hh/ccd/__init__.py
+-rw-rw-rw-   0        0        0      312 2023-04-07 08:39:02.000000 astro_hh-0.0.4/astro_hh/ccd/ccd_io.py
+-rw-rw-rw-   0        0        0     2863 2023-04-11 14:18:16.000000 astro_hh-0.0.4/astro_hh/ccd/ccd_process.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:26:20.386130 astro_hh-0.0.4/astro_hh.egg-info/
+-rw-rw-rw-   0        0        0      416 2023-04-12 11:26:20.000000 astro_hh-0.0.4/astro_hh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-12 11:26:20.000000 astro_hh-0.0.4/astro_hh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 11:26:20.000000 astro_hh-0.0.4/astro_hh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 11:26:20.000000 astro_hh-0.0.4/astro_hh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 11:26:20.389129 astro_hh-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-04-12 11:26:11.000000 astro_hh-0.0.4/setup.py
```

### Comparing `astro_hh-0.0.3/LICENSE` & `astro_hh-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_hh-0.0.3/astro_hh/ccd/ccd_process.py` & `astro_hh-0.0.4/astro_hh/ccd/ccd_process.py`

 * *Files identical despite different names*

### Comparing `astro_hh-0.0.3/setup.py` & `astro_hh-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="astro_hh",
-  version="0.0.3",
+  version="0.0.4",
   author="HuangHao",
   author_email="ironlionwg@outlook.com",
   description="A small example package",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=find_packages(".\\"),
```

