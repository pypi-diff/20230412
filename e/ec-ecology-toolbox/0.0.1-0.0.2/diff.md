# Comparing `tmp/ec_ecology_toolbox-0.0.1.tar.gz` & `tmp/ec_ecology_toolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec_ecology_toolbox-0.0.1.tar", last modified: Wed Apr 12 02:34:48 2023, max compression
+gzip compressed data, was "ec_ecology_toolbox-0.0.2.tar", last modified: Wed Apr 12 03:25:44 2023, max compression
```

## Comparing `ec_ecology_toolbox-0.0.1.tar` & `ec_ecology_toolbox-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 emily     (1000) emily     (1000)        0 2023-04-12 02:34:48.799641 ec_ecology_toolbox-0.0.1/
--rw-rw-r--   0 emily     (1000) emily     (1000)     1083 2022-12-16 06:07:00.000000 ec_ecology_toolbox-0.0.1/LICENSE
--rw-rw-r--   0 emily     (1000) emily     (1000)      369 2023-04-12 02:34:48.799641 ec_ecology_toolbox-0.0.1/PKG-INFO
--rw-rw-r--   0 emily     (1000) emily     (1000)      355 2023-02-27 06:44:18.000000 ec_ecology_toolbox-0.0.1/README.md
-drwxrwxr-x   0 emily     (1000) emily     (1000)        0 2023-04-12 02:34:48.799641 ec_ecology_toolbox-0.0.1/ec_ecology_toolbox.egg-info/
--rw-rw-r--   0 emily     (1000) emily     (1000)      369 2023-04-12 02:34:48.000000 ec_ecology_toolbox-0.0.1/ec_ecology_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 emily     (1000) emily     (1000)      331 2023-04-12 02:34:48.000000 ec_ecology_toolbox-0.0.1/ec_ecology_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 emily     (1000) emily     (1000)        1 2023-04-12 02:34:48.000000 ec_ecology_toolbox-0.0.1/ec_ecology_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 emily     (1000) emily     (1000)        1 2023-04-11 20:06:59.000000 ec_ecology_toolbox-0.0.1/ec_ecology_toolbox.egg-info/not-zip-safe
--rw-rw-r--   0 emily     (1000) emily     (1000)       15 2023-04-12 02:34:48.000000 ec_ecology_toolbox-0.0.1/ec_ecology_toolbox.egg-info/requires.txt
--rw-rw-r--   0 emily     (1000) emily     (1000)       19 2023-04-12 02:34:48.000000 ec_ecology_toolbox-0.0.1/ec_ecology_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 emily     (1000) emily     (1000)      265 2023-04-12 02:18:06.000000 ec_ecology_toolbox-0.0.1/pyproject.toml
--rw-rw-r--   0 emily     (1000) emily     (1000)       38 2023-04-12 02:34:48.799641 ec_ecology_toolbox-0.0.1/setup.cfg
--rw-rw-r--   0 emily     (1000) emily     (1000)     1438 2023-04-12 02:30:22.000000 ec_ecology_toolbox-0.0.1/setup.py
-drwxrwxr-x   0 emily     (1000) emily     (1000)        0 2023-04-12 02:34:48.799641 ec_ecology_toolbox-0.0.1/source/
--rw-rw-r--   0 emily     (1000) emily     (1000)      482 2023-04-12 02:27:53.000000 ec_ecology_toolbox-0.0.1/source/wrapper.cc
-drwxrwxr-x   0 emily     (1000) emily     (1000)        0 2023-04-12 02:34:48.799641 ec_ecology_toolbox-0.0.1/tests/
--rw-rw-r--   0 emily     (1000) emily     (1000)       95 2023-04-11 20:10:09.000000 ec_ecology_toolbox-0.0.1/tests/test_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:25:44.896501 ec_ecology_toolbox-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-12 03:25:28.000000 ec_ecology_toolbox-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 03:25:44.896501 ec_ecology_toolbox-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 03:25:28.000000 ec_ecology_toolbox-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:25:44.896501 ec_ecology_toolbox-0.0.2/ec_ecology_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 03:25:44.000000 ec_ecology_toolbox-0.0.2/ec_ecology_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-12 03:25:44.000000 ec_ecology_toolbox-0.0.2/ec_ecology_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:25:44.000000 ec_ecology_toolbox-0.0.2/ec_ecology_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:25:44.000000 ec_ecology_toolbox-0.0.2/ec_ecology_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 03:25:44.000000 ec_ecology_toolbox-0.0.2/ec_ecology_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 03:25:44.000000 ec_ecology_toolbox-0.0.2/ec_ecology_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-12 03:25:28.000000 ec_ecology_toolbox-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-12 03:25:44.896501 ec_ecology_toolbox-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-12 03:25:28.000000 ec_ecology_toolbox-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:25:44.896501 ec_ecology_toolbox-0.0.2/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 03:25:28.000000 ec_ecology_toolbox-0.0.2/source/wrapper.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:25:44.896501 ec_ecology_toolbox-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 03:25:28.000000 ec_ecology_toolbox-0.0.2/tests/test_toolbox.py
```

### Comparing `ec_ecology_toolbox-0.0.1/LICENSE` & `ec_ecology_toolbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ec_ecology_toolbox-0.0.1/setup.py` & `ec_ecology_toolbox-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

