# Comparing `tmp/ler-0.1.0.tar.gz` & `tmp/ler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ler-0.1.0.tar", last modified: Tue Apr 11 06:51:05 2023, max compression
+gzip compressed data, was "ler-0.1.1.tar", last modified: Wed Apr 12 05:31:39 2023, max compression
```

## Comparing `ler-0.1.0.tar` & `ler-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-11 06:51:05.753222 ler-0.1.0/
--rw-r--r--   0 hemantaph   (501) staff       (20)      210 2023-04-11 06:51:05.752932 ler-0.1.0/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)      241 2023-04-09 00:19:21.000000 ler-0.1.0/README.md
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-11 06:51:05.750805 ler-0.1.0/ler/
--rw-r--r--   0 hemantaph   (501) staff       (20)      248 2023-04-09 00:20:02.000000 ler-0.1.0/ler/__init__.py
--rw-r--r--   0 hemantaph   (501) staff       (20)     7651 2023-04-09 00:20:55.000000 ler-0.1.0/ler/helperroutines.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    28242 2023-04-09 00:20:55.000000 ler-0.1.0/ler/lens_galaxy_population.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    17424 2023-04-09 00:20:55.000000 ler-0.1.0/ler/ler.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    53400 2023-04-09 00:20:02.000000 ler-0.1.0/ler/ler_old1.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    18973 2023-04-09 00:20:02.000000 ler-0.1.0/ler/ler_old2.py
--rw-r--r--   0 hemantaph   (501) staff       (20)     5759 2023-04-09 00:20:55.000000 ler-0.1.0/ler/solve_lens_equation.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    11812 2023-04-09 00:20:55.000000 ler-0.1.0/ler/source_population.py
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-11 06:51:05.752562 ler-0.1.0/ler.egg-info/
--rw-r--r--   0 hemantaph   (501) staff       (20)      210 2023-04-11 06:51:05.000000 ler-0.1.0/ler.egg-info/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)      315 2023-04-11 06:51:05.000000 ler-0.1.0/ler.egg-info/SOURCES.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-04-11 06:51:05.000000 ler-0.1.0/ler.egg-info/dependency_links.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)      133 2023-04-11 06:51:05.000000 ler-0.1.0/ler.egg-info/requires.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        4 2023-04-11 06:51:05.000000 ler-0.1.0/ler.egg-info/top_level.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-04-11 06:51:05.753306 ler-0.1.0/setup.cfg
--rw-r--r--   0 hemantaph   (501) staff       (20)      612 2023-04-11 06:50:56.000000 ler-0.1.0/setup.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-12 05:31:39.248831 ler-0.1.1/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-12 05:31:39.248533 ler-0.1.1/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)       50 2023-04-12 04:14:44.000000 ler-0.1.1/README.md
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-12 05:31:39.246292 ler-0.1.1/ler/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      248 2023-04-09 00:20:02.000000 ler-0.1.1/ler/__init__.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)     7651 2023-04-09 00:20:55.000000 ler-0.1.1/ler/helperroutines.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    28242 2023-04-09 00:20:55.000000 ler-0.1.1/ler/lens_galaxy_population.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    17424 2023-04-09 00:20:55.000000 ler-0.1.1/ler/ler.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    53400 2023-04-09 00:20:02.000000 ler-0.1.1/ler/ler_old1.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    18973 2023-04-09 00:20:02.000000 ler-0.1.1/ler/ler_old2.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)     5759 2023-04-09 00:20:55.000000 ler-0.1.1/ler/solve_lens_equation.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    11812 2023-04-09 00:20:55.000000 ler-0.1.1/ler/source_population.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-12 05:31:39.248149 ler-0.1.1/ler.egg-info/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)      315 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/SOURCES.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/dependency_links.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)      131 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/requires.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        4 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/top_level.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-04-12 05:31:39.248930 ler-0.1.1/setup.cfg
+-rw-r--r--   0 hemantaph   (501) staff       (20)      592 2023-04-12 05:31:26.000000 ler-0.1.1/setup.py
```

### Comparing `ler-0.1.0/ler/helperroutines.py` & `ler-0.1.1/ler/helperroutines.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.0/ler/lens_galaxy_population.py` & `ler-0.1.1/ler/lens_galaxy_population.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.0/ler/ler.py` & `ler-0.1.1/ler/ler.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.0/ler/ler_old1.py` & `ler-0.1.1/ler/ler_old1.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.0/ler/ler_old2.py` & `ler-0.1.1/ler/ler_old2.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.0/ler/solve_lens_equation.py` & `ler-0.1.1/ler/solve_lens_equation.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.0/ler/source_population.py` & `ler-0.1.1/ler/source_population.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.0/setup.py` & `ler-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 setup(name='ler',
-      version='0.1.0',
-      description='LEnsing Rates',
+      version='0.1.1',
+      description='Lensing Rates',
       author='Hemantakumar',
       license="MIT",
       author_email='hemantaphurailatpam@gmail.com',
-      url='https://git.ligo.org/hemantakumar.phurailatpam/ler',
+      url='https://github.com/hemantaph/ler',
       packages=find_packages(),
       install_requires=[
         "setuptools>=61.1.0",
         "numpy>=1.18",
         "bilby>=1.0.2",
         "pycbc>=2.0.4",
         "quintet>=0.1",
         "scipy>=1.9.0",
-        "lenstronomy>='1.10.4'",
+        "lenstronomy>=1.10.4",
         "astropy>=5.1",
         "gwcosmo>=1.0.0",
       ]
      )
```

