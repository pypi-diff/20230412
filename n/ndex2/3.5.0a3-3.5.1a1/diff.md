# Comparing `tmp/ndex2-3.5.0a3.tar.gz` & `tmp/ndex2-3.5.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndex2-3.5.0a3.tar", last modified: Tue Jun 28 17:50:39 2022, max compression
+gzip compressed data, was "dist/ndex2-3.5.1a1.tar", last modified: Tue Apr 11 22:48:15 2023, max compression
```

## Comparing `ndex2-3.5.0a3.tar` & `ndex2-3.5.1a1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.308690 ndex2-3.5.0a3/
--rw-r--r--   0 churas     (504) staff       (20)     9092 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1526 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/LICENSE.txt
--rw-r--r--   0 churas     (504) staff       (20)      237 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     2477 2021-04-01 21:50:41.000000 ndex2-3.5.0a3/Makefile
--rw-r--r--   0 churas     (504) staff       (20)    14372 2022-06-28 17:50:39.308930 ndex2-3.5.0a3/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     2103 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.284586 ndex2-3.5.0a3/docs/
--rw-r--r--   0 churas     (504) staff       (20)      606 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.276676 ndex2-3.5.0a3/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.276766 ndex2-3.5.0a3/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.286227 ndex2-3.5.0a3/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2022-02-15 21:42:18.000000 ndex2-3.5.0a3/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 ndex2-3.5.0a3/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 ndex2-3.5.0a3/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)     9473 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)     1067 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/convertnicecx.rst
--rw-r--r--   0 churas     (504) staff       (20)      520 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/createnicecx.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      241 2021-04-01 21:50:41.000000 ndex2-3.5.0a3/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1062 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)       46 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/docs/license.rst
--rw-r--r--   0 churas     (504) staff       (20)      581 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/miscref.rst
--rw-r--r--   0 churas     (504) staff       (20)      545 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     2769 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/ndex2.rst
--rw-r--r--   0 churas     (504) staff       (20)     1949 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/ndex2client.rst
--rw-r--r--   0 churas     (504) staff       (20)     7395 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/docs/quicktutorial.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.291081 ndex2-3.5.0a3/ndex2/
--rw-r--r--   0 churas     (504) staff       (20)    28035 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)    87630 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2/client.py
--rw-r--r--   0 churas     (504) staff       (20)     2635 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2/constants.py
--rw-r--r--   0 churas     (504) staff       (20)      955 2021-04-01 21:50:41.000000 ndex2-3.5.0a3/ndex2/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    20507 2021-04-01 21:50:41.000000 ndex2-3.5.0a3/ndex2/niceCxInterface.py
--rw-r--r--   0 churas     (504) staff       (20)   106528 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2/nice_cx_network.py
--rw-r--r--   0 churas     (504) staff       (20)     6120 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2/util.py
--rw-r--r--   0 churas     (504) staff       (20)       24 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2/version.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.292592 ndex2-3.5.0a3/ndex2.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)    14372 2022-06-28 17:50:39.000000 ndex2-3.5.0a3/ndex2.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1425 2022-06-28 17:50:39.000000 ndex2-3.5.0a3/ndex2.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2022-06-28 17:50:39.000000 ndex2-3.5.0a3/ndex2.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)      167 2022-06-28 17:50:39.000000 ndex2-3.5.0a3/ndex2.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       14 2022-06-28 17:50:39.000000 ndex2-3.5.0a3/ndex2.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.294012 ndex2-3.5.0a3/ndex2cx/
--rw-r--r--   0 churas     (504) staff       (20)      697 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2cx/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)    18328 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/ndex2cx/nice_cx_builder.py
--rw-r--r--   0 churas     (504) staff       (20)      255 2021-04-01 21:50:41.000000 ndex2-3.5.0a3/ndex2cx/parallelCX.py
--rw-r--r--   0 churas     (504) staff       (20)      295 2022-06-28 17:50:39.309480 ndex2-3.5.0a3/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     3578 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.304366 ndex2-3.5.0a3/tests/
--rw-r--r--   0 churas     (504) staff       (20)     6148 2022-06-14 21:58:22.000000 ndex2-3.5.0a3/tests/.DS_Store
--rw-r--r--   0 churas     (504) staff       (20)       60 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2022-06-28 17:50:39.308045 ndex2-3.5.0a3/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)   108653 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/tests/data/darkthemefinal.cx
--rw-r--r--   0 churas     (504) staff       (20)   218291 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/tests/data/darkthemefinalwithnodevis.cx
--rw-r--r--   0 churas     (504) staff       (20)    10185 2021-03-31 01:22:47.000000 ndex2-3.5.0a3/tests/data/glypican2.cx
--rw-r--r--   0 churas     (504) staff       (20)    10436 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/data/glypican2.cx2
--rw-r--r--   0 churas     (504) staff       (20)    73563 2021-04-01 00:54:02.000000 ndex2-3.5.0a3/tests/data/wntsignaling.cx
--rw-r--r--   0 churas     (504) staff       (20)     1074 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test__init__.py
--rw-r--r--   0 churas     (504) staff       (20)    95333 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_client.py
--rw-r--r--   0 churas     (504) staff       (20)    12063 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_create_nice_cx_from_networkx.py
--rw-r--r--   0 churas     (504) staff       (20)     7496 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_create_nice_cx_from_pandas.py
--rw-r--r--   0 churas     (504) staff       (20)     2999 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_create_nice_cx_from_raw_cx.py
--rw-r--r--   0 churas     (504) staff       (20)    25010 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_defaultnetworkxfactory.py
--rw-r--r--   0 churas     (504) staff       (20)     2625 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_integration__init__.py
--rw-r--r--   0 churas     (504) staff       (20)    13161 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_integration_nice_cx_network.py
--rw-r--r--   0 churas     (504) staff       (20)    41784 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_integration_test_of_client.py
--rw-r--r--   0 churas     (504) staff       (20)     9488 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_legacynetworkxversiontwoplusfactory.py
--rw-r--r--   0 churas     (504) staff       (20)    13715 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_nice_cx_builder.py
--rw-r--r--   0 churas     (504) staff       (20)    41667 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_nice_cx_network.py
--rw-r--r--   0 churas     (504) staff       (20)     7828 2022-06-28 17:48:29.000000 ndex2-3.5.0a3/tests/test_pandasdataconverter.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/
+-rw-r--r--   0 churas     (504) staff       (20)     9490 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1526 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/LICENSE.txt
+-rw-r--r--   0 churas     (504) staff       (20)      237 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     2477 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/Makefile
+-rw-r--r--   0 churas     (504) staff       (20)    15318 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     2507 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      606 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2022-02-15 21:42:18.000000 ndex2-3.5.1a1/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 ndex2-3.5.1a1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 ndex2-3.5.1a1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)     9473 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)     1067 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/convertnicecx.rst
+-rw-r--r--   0 churas     (504) staff       (20)      520 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/createnicecx.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      241 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1062 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)       46 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/docs/license.rst
+-rw-r--r--   0 churas     (504) staff       (20)      581 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/miscref.rst
+-rw-r--r--   0 churas     (504) staff       (20)      545 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     2769 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/ndex2.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1949 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/ndex2client.rst
+-rw-r--r--   0 churas     (504) staff       (20)     7395 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/quicktutorial.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2/
+-rw-r--r--   0 churas     (504) staff       (20)    28035 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    88026 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/ndex2/client.py
+-rw-r--r--   0 churas     (504) staff       (20)     2635 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)      955 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/ndex2/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    20507 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/ndex2/niceCxInterface.py
+-rw-r--r--   0 churas     (504) staff       (20)   106528 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/nice_cx_network.py
+-rw-r--r--   0 churas     (504) staff       (20)     6120 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/util.py
+-rw-r--r--   0 churas     (504) staff       (20)       24 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/ndex2/version.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)    15318 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1425 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)      167 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       14 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2cx/
+-rw-r--r--   0 churas     (504) staff       (20)      697 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2cx/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    18128 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/ndex2cx/nice_cx_builder.py
+-rw-r--r--   0 churas     (504) staff       (20)      255 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/ndex2cx/parallelCX.py
+-rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     3578 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/tests/
+-rw-r--r--   0 churas     (504) staff       (20)     6148 2022-06-14 21:58:22.000000 ndex2-3.5.1a1/tests/.DS_Store
+-rw-r--r--   0 churas     (504) staff       (20)       60 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)   108653 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/data/darkthemefinal.cx
+-rw-r--r--   0 churas     (504) staff       (20)   218291 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/data/darkthemefinalwithnodevis.cx
+-rw-r--r--   0 churas     (504) staff       (20)    10185 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/data/glypican2.cx
+-rw-r--r--   0 churas     (504) staff       (20)    10436 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/data/glypican2.cx2
+-rw-r--r--   0 churas     (504) staff       (20)    73563 2021-04-01 00:54:02.000000 ndex2-3.5.1a1/tests/data/wntsignaling.cx
+-rw-r--r--   0 churas     (504) staff       (20)     1074 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    95333 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_client.py
+-rw-r--r--   0 churas     (504) staff       (20)    12063 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_create_nice_cx_from_networkx.py
+-rw-r--r--   0 churas     (504) staff       (20)     7496 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_create_nice_cx_from_pandas.py
+-rw-r--r--   0 churas     (504) staff       (20)     2999 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_create_nice_cx_from_raw_cx.py
+-rw-r--r--   0 churas     (504) staff       (20)    25010 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_defaultnetworkxfactory.py
+-rw-r--r--   0 churas     (504) staff       (20)     2625 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_integration__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    13161 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_integration_nice_cx_network.py
+-rw-r--r--   0 churas     (504) staff       (20)    41979 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_integration_test_of_client.py
+-rw-r--r--   0 churas     (504) staff       (20)     9488 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_legacynetworkxversiontwoplusfactory.py
+-rw-r--r--   0 churas     (504) staff       (20)    13715 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_nice_cx_builder.py
+-rw-r--r--   0 churas     (504) staff       (20)    41667 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_nice_cx_network.py
+-rw-r--r--   0 churas     (504) staff       (20)     7828 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_pandasdataconverter.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ndex2-3.5.0a3/HISTORY.rst` & `ndex2-3.5.1a1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =======
 History
 =======
 
+3.5.1 (2023-04-11)
+-------------------
+
+* Bug fixes
+
+    * Fixed bug where ``ndex2.create_nice_cx_from_networkx()`` fails with numpy version 1.24
+      `Issue #96 <https://github.com/ndexbio/ndex2-client/issues/96>`__
+
+    * Updated post and put calls in ``client.py`` to only pass credentials if they are
+      set. This change is to accommodate changes in upcoming version 3 of requests library
+
 3.5.0 (2022-06-28)
 -------------------
 
 * Enhancements
     * Added **skip_version_check** parameter to ``Ndex2()`` constructor to let caller
       optionally bypass NDEx server call to see if **v2** endpoint is supported
```

### Comparing `ndex2-3.5.0a3/LICENSE.txt` & `ndex2-3.5.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/Makefile` & `ndex2-3.5.1a1/Makefile`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/PKG-INFO` & `ndex2-3.5.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: ndex2
-Version: 3.5.0a3
+Version: 3.5.1a1
 Summary: Nice CX Python includes a client and a data model.
 Home-page: https://github.com/ndexbio/ndex2-client
 Author: The NDEx Project
 Author-email: contact@ndexbio.org
 License: BSD
 Description: **NDEx2 Python Client**
         =========================
         
         .. _NDEx: http://ndexbio.org
         .. _NDEx REST Server API: http://www.home.ndexbio.org/using-the-ndex-server-api
         
-        .. image:: https://img.shields.io/travis/ndexbio/ndex2-client.svg
-                :target: https://travis-ci.com/ndexbio/ndex2-client.svg?branch=master
+        .. image:: https://app.travis-ci.com/ndexbio/ndex2-client.svg?branch=master
+                :target: https://app.travis-ci.com/ndexbio/ndex2-client.svg?branch=master
         
         .. image:: https://img.shields.io/pypi/v/ndex2.svg
                 :target: https://pypi.python.org/pypi/ndex2
         
         .. image:: https://coveralls.io/repos/github/ndexbio/ndex2-client/badge.svg?branch=master
                 :target: https://coveralls.io/github/ndexbio/ndex2-client?branch=master
         
@@ -70,26 +70,44 @@
         can use this command instead:
         
         ::
         
             pip install --upgrade ndex2
         
         
+        **Resources**
+        --------------------------------------
+        
+        * The NDEx2 Python Client `documentation <https://ndex2.readthedocs.io/en/latest/>`_ is available on Read the Docs.
+        * Please refer to our `Jupyter Notebook Tutorials <https://github.com/ndexbio/ndex-jupyter-notebooks>`_ GitHub repository for code examples to work with networks using the NDEx2 Python Client and NiceCX object class. 
+        
+        
         **License**
         --------------------------------------
         
         See `LICENSE.txt <https://github.com/ndexbio/ndex2-client/blob/master/LICENSE.txt>`_
         
         
         
         
         =======
         History
         =======
         
+        3.5.1 (2023-04-11)
+        -------------------
+        
+        * Bug fixes
+        
+            * Fixed bug where ``ndex2.create_nice_cx_from_networkx()`` fails with numpy version 1.24
+              `Issue #96 <https://github.com/ndexbio/ndex2-client/issues/96>`__
+        
+            * Updated post and put calls in ``client.py`` to only pass credentials if they are
+              set. This change is to accommodate changes in upcoming version 3 of requests library
+        
         3.5.0 (2022-06-28)
         -------------------
         
         * Enhancements
             * Added **skip_version_check** parameter to ``Ndex2()`` constructor to let caller
               optionally bypass NDEx server call to see if **v2** endpoint is supported
```

### Comparing `ndex2-3.5.0a3/docs/Makefile` & `ndex2-3.5.1a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/conf.py` & `ndex2-3.5.1a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/convertnicecx.rst` & `ndex2-3.5.1a1/docs/convertnicecx.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/createnicecx.rst` & `ndex2-3.5.1a1/docs/createnicecx.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/installation.rst` & `ndex2-3.5.1a1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/miscref.rst` & `ndex2-3.5.1a1/docs/miscref.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/modules.rst` & `ndex2-3.5.1a1/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/ndex2.rst` & `ndex2-3.5.1a1/docs/ndex2.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/ndex2client.rst` & `ndex2-3.5.1a1/docs/ndex2client.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/docs/quicktutorial.rst` & `ndex2-3.5.1a1/docs/quicktutorial.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2/__init__.py` & `ndex2-3.5.1a1/ndex2/__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2/client.py` & `ndex2-3.5.1a1/ndex2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,27 @@
                         ': ' + str(error))
 
     def _get_version_endpoint(self, alt_version_endpoint=None):
         if alt_version_endpoint is None:
             return self.version_endpoint
         return alt_version_endpoint
 
+    def _get_auth_tuple(self):
+        """
+        Gets a tuple with username and password set via constructor
+        if they are both NOT ``None``
+
+        :return: (username, password) or ``None`` if values of both are
+                 ``None``
+        :rtype: tuple
+        """
+        if self.username is None and self.password is None:
+            return None
+        return self.username, self.password
+
     def put(self, route, put_json=None, alt_version_endpoint=None):
         url = self.host +\
               self._get_version_endpoint(alt_version_endpoint=
                                          alt_version_endpoint) + route
         self.logger.debug("PUT route: " + url)
         self.logger.debug("PUT json: " + str(put_json))
 
@@ -388,15 +401,15 @@
         self.logger.debug("PUT route: " + url)
 
         headers = {'Content-Type': multipart_data.content_type,
                    'Accept': 'application/json',
                    Ndex2.USER_AGENT_KEY: self._get_user_agent(),
                    'Connection': 'close'
                    }
-        response = requests.put(url, data=multipart_data, headers=headers, auth=(self.username, self.password))
+        response = requests.put(url, data=multipart_data, headers=headers, auth=self._get_auth_tuple())
         return self._return_response(response,
                                      returnjsonundertry=returnjsonundertry,
                                      returnfullresponse=returnfullresponse)
 
     # The Request is streamed, not the Response
     def post_multipart(self, route, fields, query_string=None, alt_version_endpoint=None,
                        returnjsonundertry=True, returnfullresponse=False):
@@ -408,15 +421,16 @@
 
         multipart_data = MultipartEncoder(fields=fields)
         self.logger.debug("POST route: " + url)
         headers = {'Content-Type': multipart_data.content_type,
                    Ndex2.USER_AGENT_KEY: self._get_user_agent(),
                    'Connection': 'close'
                    }
-        response = requests.post(url, data=multipart_data, headers=headers, auth=(self.username, self.password))
+
+        response = requests.post(url, data=multipart_data, headers=headers, auth=self._get_auth_tuple())
         return self._return_response(response,
                                      returnjsonundertry=returnjsonundertry,
                                      returnfullresponse=returnfullresponse)
 
 # Network methods
 
     def save_new_network(self, cx, visibility=None):
@@ -431,15 +445,15 @@
         :return: Response data
         :rtype: str or dict
         """
         if cx is None:
             raise NDExInvalidCXError('CX is None')
         if not isinstance(cx, list):
             raise NDExInvalidCXError('CX is not a list')
-        if len(cx) is 0:
+        if len(cx) == 0:
             raise NDExInvalidCXError('CX appears to be empty')
 
         indexed_fields = None
         #TODO add functionality for indexed_fields when it's supported by the server
         if cx[-1] is not None:
             if cx[-1].get('status') is None:
                 cx.append({"status": [{"error": "", "success": True}]})
@@ -520,15 +534,15 @@
                  (ie http://ndexbio.org/v3/networks/XXXX)
         :rtype: str
         """
         if cx is None:
             raise NDExInvalidCXError('CX is None')
         if not isinstance(cx, list):
             raise NDExInvalidCXError('CX is not a list')
-        if len(cx) is 0:
+        if len(cx) == 0:
             raise NDExInvalidCXError('CX appears to be empty')
 
         if sys.version_info.major == 3:
             stream = io.BytesIO(json.dumps(cx, cls=DecimalEncoder).encode('utf-8'))
         else:
             stream = io.BytesIO(json.dumps(cx, cls=DecimalEncoder))
```

### Comparing `ndex2-3.5.0a3/ndex2/constants.py` & `ndex2-3.5.1a1/ndex2/constants.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2/exceptions.py` & `ndex2-3.5.1a1/ndex2/exceptions.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2/niceCxInterface.py` & `ndex2-3.5.1a1/ndex2/niceCxInterface.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2/nice_cx_network.py` & `ndex2-3.5.1a1/ndex2/nice_cx_network.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2/util.py` & `ndex2-3.5.1a1/ndex2/util.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2.egg-info/PKG-INFO` & `ndex2-3.5.1a1/ndex2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: ndex2
-Version: 3.5.0a3
+Version: 3.5.1a1
 Summary: Nice CX Python includes a client and a data model.
 Home-page: https://github.com/ndexbio/ndex2-client
 Author: The NDEx Project
 Author-email: contact@ndexbio.org
 License: BSD
 Description: **NDEx2 Python Client**
         =========================
         
         .. _NDEx: http://ndexbio.org
         .. _NDEx REST Server API: http://www.home.ndexbio.org/using-the-ndex-server-api
         
-        .. image:: https://img.shields.io/travis/ndexbio/ndex2-client.svg
-                :target: https://travis-ci.com/ndexbio/ndex2-client.svg?branch=master
+        .. image:: https://app.travis-ci.com/ndexbio/ndex2-client.svg?branch=master
+                :target: https://app.travis-ci.com/ndexbio/ndex2-client.svg?branch=master
         
         .. image:: https://img.shields.io/pypi/v/ndex2.svg
                 :target: https://pypi.python.org/pypi/ndex2
         
         .. image:: https://coveralls.io/repos/github/ndexbio/ndex2-client/badge.svg?branch=master
                 :target: https://coveralls.io/github/ndexbio/ndex2-client?branch=master
         
@@ -70,26 +70,44 @@
         can use this command instead:
         
         ::
         
             pip install --upgrade ndex2
         
         
+        **Resources**
+        --------------------------------------
+        
+        * The NDEx2 Python Client `documentation <https://ndex2.readthedocs.io/en/latest/>`_ is available on Read the Docs.
+        * Please refer to our `Jupyter Notebook Tutorials <https://github.com/ndexbio/ndex-jupyter-notebooks>`_ GitHub repository for code examples to work with networks using the NDEx2 Python Client and NiceCX object class. 
+        
+        
         **License**
         --------------------------------------
         
         See `LICENSE.txt <https://github.com/ndexbio/ndex2-client/blob/master/LICENSE.txt>`_
         
         
         
         
         =======
         History
         =======
         
+        3.5.1 (2023-04-11)
+        -------------------
+        
+        * Bug fixes
+        
+            * Fixed bug where ``ndex2.create_nice_cx_from_networkx()`` fails with numpy version 1.24
+              `Issue #96 <https://github.com/ndexbio/ndex2-client/issues/96>`__
+        
+            * Updated post and put calls in ``client.py`` to only pass credentials if they are
+              set. This change is to accommodate changes in upcoming version 3 of requests library
+        
         3.5.0 (2022-06-28)
         -------------------
         
         * Enhancements
             * Added **skip_version_check** parameter to ``Ndex2()`` constructor to let caller
               optionally bypass NDEx server call to see if **v2** endpoint is supported
```

### Comparing `ndex2-3.5.0a3/ndex2.egg-info/SOURCES.txt` & `ndex2-3.5.1a1/ndex2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2cx/__init__.py` & `ndex2-3.5.1a1/ndex2cx/__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/ndex2cx/nice_cx_builder.py` & `ndex2-3.5.1a1/ndex2cx/nice_cx_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 __author__ = 'aarongary'
 
 import logging
 import base64
 import sys
 import math
-import numpy as np
 
 if sys.version_info.major == 3:
     from urllib.request import urlopen, Request, HTTPError, URLError
 else:
     from urllib2 import urlopen, Request, HTTPError, URLError
 
 
@@ -464,37 +463,37 @@
             if isinstance(val, str):
                 val = val.replace('"', '')
                 if ',' in val:
                     val = val.split(',')
                 elif ';' in val:
                     val = val.split(';')
 
-        if isinstance(val, float) or isinstance(val, np.float) or isinstance(val, np.double):
+        if isinstance(val, float):
             if math.isnan(val):
                 # do something (skip?)
                 val = None
             elif math.isinf(val):
                 val = 'INFINITY'
             return val, 'double'
         if isinstance(val, bool):
             # fix for https://github.com/ndexbio/ndex2-client/issues/83
             # a boolean is a sub type of int so bool must be tested first
             return val, 'boolean'
-        if isinstance(val, int) or isinstance(val, np.int):
+        if isinstance(val, int):
             return val, 'integer'
         if isinstance(val, list):
             # if the list is empty just set data type to list_of_string
             # fix for https://github.com/ndexbio/ndex2-client/issues/90
             attr_type = 'list_of_string'
             if len(val) > 0:
-                if isinstance(val[0], float) or isinstance(val[0], np.float) or isinstance(val[0], np.double):
+                if isinstance(val[0], float):
                     attr_type = 'list_of_double'
                 elif isinstance(val[0], bool):
                     # fix for https://github.com/ndexbio/ndex2-client/issues/83
                     # a boolean is a sub type of int so bool must be tested first
                     attr_type = 'list_of_boolean'
-                elif isinstance(val[0], int) or isinstance(val[0], np.int):
+                elif isinstance(val[0], int):
                     attr_type = 'list_of_integer'
 
         return val, attr_type
```

### Comparing `ndex2-3.5.0a3/setup.py` & `ndex2-3.5.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/.DS_Store` & `ndex2-3.5.1a1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/data/darkthemefinal.cx` & `ndex2-3.5.1a1/tests/data/darkthemefinal.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/data/darkthemefinalwithnodevis.cx` & `ndex2-3.5.1a1/tests/data/darkthemefinalwithnodevis.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/data/glypican2.cx` & `ndex2-3.5.1a1/tests/data/glypican2.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/data/glypican2.cx2` & `ndex2-3.5.1a1/tests/data/glypican2.cx2`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/data/wntsignaling.cx` & `ndex2-3.5.1a1/tests/data/wntsignaling.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test__init__.py` & `ndex2-3.5.1a1/tests/test__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_client.py` & `ndex2-3.5.1a1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_create_nice_cx_from_networkx.py` & `ndex2-3.5.1a1/tests/test_create_nice_cx_from_networkx.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_create_nice_cx_from_pandas.py` & `ndex2-3.5.1a1/tests/test_create_nice_cx_from_pandas.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_create_nice_cx_from_raw_cx.py` & `ndex2-3.5.1a1/tests/test_create_nice_cx_from_raw_cx.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_defaultnetworkxfactory.py` & `ndex2-3.5.1a1/tests/test_defaultnetworkxfactory.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_integration__init__.py` & `ndex2-3.5.1a1/tests/test_integration__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_integration_nice_cx_network.py` & `ndex2-3.5.1a1/tests/test_integration_nice_cx_network.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_integration_test_of_client.py` & `ndex2-3.5.1a1/tests/test_integration_test_of_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,23 +606,26 @@
     def test_get_network_ids_for_user(self):
         client = self.get_ndex2_client()
         creds = self.get_ndex_credentials_as_tuple()
         netid_one = None
         netid_two = None
         try:
             # query for networks for user in creds
-            network_ids = client.get_network_ids_for_user(creds['user'])
+            network_ids = client.get_network_ids_for_user(creds['user'], limit=100000)
             num_network_ids = len(network_ids)
             self.assertTrue(num_network_ids >= 0)
 
             # set offset to number of network ids and limit 1
             network_ids = client.get_network_ids_for_user(creds['user'],
                                                           offset=num_network_ids,
                                                           limit=1)
-            self.assertTrue(len(network_ids) == 0)
+            self.assertTrue(len(network_ids) == 0, 'this will fail if user has '
+                                                   'more then 100000 networks in'
+                                                   'there account')
+
 
             # add two networks just in case there are none and verify
             # they are returned
             net = ndex2.create_nice_cx_from_file(TestClientIntegration.GLYPICAN2_FILE)
             netname = 'ndex2-client integration test network1' + str(datetime.now())
             net.set_name(netname)
             res = client.save_new_network(net.to_cx(), visibility='PUBLIC')
```

### Comparing `ndex2-3.5.0a3/tests/test_legacynetworkxversiontwoplusfactory.py` & `ndex2-3.5.1a1/tests/test_legacynetworkxversiontwoplusfactory.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_nice_cx_builder.py` & `ndex2-3.5.1a1/tests/test_nice_cx_builder.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_nice_cx_network.py` & `ndex2-3.5.1a1/tests/test_nice_cx_network.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.0a3/tests/test_pandasdataconverter.py` & `ndex2-3.5.1a1/tests/test_pandasdataconverter.py`

 * *Files identical despite different names*

