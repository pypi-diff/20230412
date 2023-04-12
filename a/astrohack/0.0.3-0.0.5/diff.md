# Comparing `tmp/astrohack-0.0.3.tar.gz` & `tmp/astrohack-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.0.3.tar", last modified: Wed Apr  5 22:28:31 2023, max compression
+gzip compressed data, was "astrohack-0.0.5.tar", last modified: Wed Apr 12 18:56:15 2023, max compression
```

## Comparing `astrohack-0.0.3.tar` & `astrohack-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.258189 astrohack-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-05 22:28:31.258189 astrohack-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-05 22:28:16.000000 astrohack-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:16.000000 astrohack-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-05 22:28:16.000000 astrohack-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 22:28:31.258189 astrohack-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.250189 astrohack-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.250189 astrohack-0.0.3/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.254189 astrohack-0.0.3/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.254189 astrohack-0.0.3/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.254189 astrohack-0.0.3/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    32035 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.254189 astrohack-0.0.3/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4899 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.254189 astrohack-0.0.3/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_system_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.254189 astrohack-0.0.3/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-05 22:28:16.000000 astrohack-0.0.3/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.250189 astrohack-0.0.3/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-05 22:28:31.000000 astrohack-0.0.3/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-05 22:28:31.000000 astrohack-0.0.3/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 22:28:31.000000 astrohack-0.0.3/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-05 22:28:31.000000 astrohack-0.0.3/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-05 22:28:31.000000 astrohack-0.0.3/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:28:31.258189 astrohack-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-05 22:28:16.000000 astrohack-0.0.3/tests/test_astrohack_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-05 22:28:16.000000 astrohack-0.0.3/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-05 22:28:16.000000 astrohack-0.0.3/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-05 22:28:16.000000 astrohack-0.0.3/tests/test_class_polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-05 22:28:16.000000 astrohack-0.0.3/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-05 22:28:16.000000 astrohack-0.0.3/tests/test_class_telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 18:56:15.661412 astrohack-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-12 18:55:57.000000 astrohack-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:55:57.000000 astrohack-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 18:55:58.000000 astrohack-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:56:15.661412 astrohack-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.653411 astrohack-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.657411 astrohack-0.0.5/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.657411 astrohack-0.0.5/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    25210 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dio_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33979 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.657411 astrohack-0.0.5/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-12 18:55:58.000000 astrohack-0.0.5/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-12 18:55:58.000000 astrohack-0.0.5/tests/test_class_ring_panel.py
```

### Comparing `astrohack-0.0.3/PKG-INFO` & `astrohack-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-Metadata-Version: 2.1
-Name: astrohack
-Version: 0.0.3
-Summary: Holography Antenna Commissioning Kit
-Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
-Requires-Python: <3.11,>=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-
 # astroHACK
 
-[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+[![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
 
 # Installing
```

### Comparing `astrohack-0.0.3/pyproject.toml` & `astrohack-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.0.3"
+version = "0.0.5"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
@@ -29,14 +29,15 @@
 'pytest==7.2.2',
 'scikit_image==0.19.3',
 'scipy==1.7.3',
 'setuptools==65.6.3',
 'Shapely==2.0.1',
 'xarray==2022.12.0',
 'zarr==2.13.3',
+'bokeh==2.4.3',
 'jupyterlab',
 'python_casacore==3.5.2; sys_platform != "darwin" '
 ]
 
 
 [project.optional-dependencies]
 docs = [
```

### Comparing `astrohack-0.0.3/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.0.5/src/astrohack/_classes/antenna_surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
             self.v_axis = inputxds.v_prime.values * self.wavelength
             computephase = False
 
         # Common elements
         self.unpix = self.u_axis.shape[0]
         self.vnpix = self.v_axis.shape[0]
         self.antenna_name = inputxds.attrs['ant_name']
+        
+        self.panel_meta = [inputxds.attrs['ant_name'],inputxds.attrs['ddi']]
 
         return computephase
 
     def _nullify(self):
         """
         Part of the initialization process, nullify the data objects to be used later
         """
@@ -254,14 +256,15 @@
                 panel = RingPanel(
                     self.panelkind,
                     angle,
                     ipanel,
                     self._panel_label(iring, ipanel),
                     self.telescope.inrad[iring],
                     self.telescope.ourad[iring],
+                    panel_meta=self.panel_meta,
                     margin=self.panel_margins,
                     screw_scheme=self.telescope.screw_description,
                     screw_offset=self.telescope.screw_offset
                 )
                 self.panels.append(panel)
         return
```

### Comparing `astrohack-0.0.3/src/astrohack/_classes/base_panel.py` & `astrohack-0.0.5/src/astrohack/_classes/base_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     markers = ['X', 'o', '*', 'P', 'D']
     colors = ['g', 'g', 'r', 'r', 'b']
     fontsize = 4
     linewidth = 0.5
     markersize = 2
     linecolor = 'black'
 
-    def __init__(self, kind, screws, label, center=None, zeta=None):
+    def __init__(self, kind, screws, label, panel_meta, center=None, zeta=None):
         """
         Initializes the base panel with the appropriated fitting methods and providing basic functionality
         Fitting method kinds are:
         AIPS fitting kinds:
             mean: The panel is corrected by the mean of its samples
             rigid: The panel samples are fitted to a rigid surface
         Corotated Paraboloids (the two bending axes are parallel and perpendicular to the radius of the antenna crossing
@@ -64,14 +64,15 @@
         self.kind = kind
         self.solved = False
         self.label = label
         self.screws = screws
         self.samples = []
         self.margins = []
         self.corr = None
+        self.panel_meta = panel_meta
 
         if center is None:
             self.center = [0, 0]
         else:
             self.center = center
         if zeta is None:
             self.zeta = 0
@@ -193,21 +194,21 @@
     def solve(self):
         """
         Wrapping method around fitting to allow for a fallback to mean fitting in the case of an impossible fit
         """
         logger = _get_astrohack_logger()
         # fallback behaviour for impossible fits
         if len(self.samples) < self.NPAR:
-            logger.warning("Impossible fit, falling back to mean")
+            logger.warning("Impossible fit, falling back to mean: " + str(self.panel_meta))
             self._fallback_solve()
         else:
             try:
                 self._solve_sub()
             except np.linalg.LinAlgError:
-                logger.warning("Fit diverged, falling back to mean")
+                logger.warning("Fit diverged, falling back to mean: " + str(self.panel_meta))
                 self._fallback_solve()
         return
 
     def _fallback_solve(self):
         """
         Changes the method association to mean surface fitting, and fits the panel with it
         """
@@ -266,15 +267,15 @@
         Builds the designer matrix for least squares fitting, and calls the _least_squares fitter for a corotated
         paraboloid centered at the center of the panel
         """
         # a*u**2 + b*v**2 + c
         data = np.array(self.samples)
         system = np.full((len(self.samples), self.NPAR), 1.0)
         xc, yc = self.center
-        system[:, 0] = ((data[:, 0] - xc) * np.cos(self.zeta) + (data[:, 1] - yc) * np.sin(self.zeta))**2  # U
+        system[:, 0] = ((data[:, 0] - xc) * np.cos(self.zeta) - (data[:, 1] - yc) * np.sin(self.zeta))**2  # U
         system[:, 1] = ((data[:, 0] - xc) * np.sin(self.zeta) + (data[:, 1] - yc) * np.cos(self.zeta))**2  # V
         vector = data[:, -1]
         self.par, _, _ = _least_squares_fit(system, vector)
         self.solved = True
 
     def _corr_point_corotated_lst_sq(self, xcoor, ycoor):
         """
@@ -283,15 +284,15 @@
             xcoor: Coordinate of point in X
             ycoor: Coordinate of point in Y
         Returns:
             The correction at point
         """
         # a*u**2 + b*v**2 + c
         xc, yc = self.center
-        usq = ((xcoor - xc) * np.cos(self.zeta) + (ycoor - yc) * np.sin(self.zeta))**2
+        usq = ((xcoor - xc) * np.cos(self.zeta) - (ycoor - yc) * np.sin(self.zeta))**2
         vsq = ((xcoor - xc) * np.sin(self.zeta) + (ycoor - yc) * np.cos(self.zeta))**2
         return self.par[0]*usq + self.par[1]*vsq + self.par[2]
 
     def _solve_scipy(self, verbose=False, x0=None):
         """
         Fit ponel surface by using arbitrary models through scipy fitting engine
         Args:
@@ -363,15 +364,15 @@
             theta: Angle between x,y and u,v coordinate systems
 
         Returns:
         Paraboloid value at X and Y
         """
         x, y = coords
         xc, yc = self.center
-        u = (x - xc) * np.cos(theta) + (y - yc) * np.sin(theta)
+        u = (x - xc) * np.cos(theta) - (y - yc) * np.sin(theta)
         v = (x - xc) * np.sin(theta) + (y - yc) * np.cos(theta)
         return ucurv * u**2 + vcurv * v**2 + zoff
 
     def _corotated_paraboloid(self, coords, ucurv, vcurv, zoff):
         """
         Surface model to be used in fitting with scipy
         Same as the rotated paraboloid above, but theta is the panel center angle
@@ -384,15 +385,15 @@
             zoff:  Z offset of the paraboloid
 
         Returns:
         Paraboloid value at X and Y
         """
         x, y = coords
         xc, yc = self.center
-        u = (x - xc) * np.cos(self.zeta) + (y - yc) * np.sin(self.zeta)
+        u = (x - xc) * np.cos(self.zeta) - (y - yc) * np.sin(self.zeta)
         v = (x - xc) * np.sin(self.zeta) + (y - yc) * np.cos(self.zeta)
         return ucurv * u**2 + vcurv * v**2 + zoff
 
     def _solve_rigid(self):
         """
         Fit panel surface using AIPS gaussian elimination model for rigid panels
         """
```

### Comparing `astrohack-0.0.3/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.0.5/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/_classes/ring_panel.py` & `astrohack-0.0.5/src/astrohack/_classes/ring_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from astrohack._classes.base_panel import BasePanel
 
 
 class RingPanel(BasePanel):
     # This class describes and treats panels that are arranged in
     # rings on the Antenna surface
 
-    def __init__(self, kind, angle, ipanel, label, inrad, ourad, margin=0.20, screw_scheme=None, screw_offset=None):
+    def __init__(self, kind, angle, ipanel, label, inrad, ourad, panel_meta, margin=0.20, screw_scheme=None, screw_offset=None):
         """
         Initializes a panel that is a section of a ring in a circular antenna
         Fitting method kinds are:
         AIPS fitting kinds:
             mean: The panel is corrected by the mean of its samples
             rigid: The panel samples are fitted to a rigid surface
         Corotated Paraboloids (the two bending axes are parallel and perpendicular to the radius of the antenna crossing
@@ -42,17 +42,18 @@
         self.margin_theta2 = self.theta2 - margin * angle
         self.margin_inrad = inrad + margin * dradius
         self.margin_ourad = ourad - margin * dradius
         self.first = ipanel == 0
         zeta = (ipanel + 0.5) * angle
         rt = (self.inrad + self.ourad) / 2
         self.center = [rt * np.cos(zeta), rt * np.sin(zeta)]
+        self.panel_meta = panel_meta
         screws = self._init_screws(screw_scheme, screw_offset)
         # Now we are ready to initialize the base object
-        super().__init__(kind, screws, label, center=self.center, zeta=zeta)
+        super().__init__(kind, screws, label, panel_meta, center=self.center, zeta=zeta)
 
     def _init_screws(self, scheme, offset):
         """
         Initialize screws according to the scheme
         Args:
             scheme: Tuple of strings containing the positioning of the screws
             offset: How far from the edge of the panel are corner screws (meters)
```

### Comparing `astrohack-0.0.3/src/astrohack/_classes/telescope.py` & `astrohack-0.0.5/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_algorithms.py` & `astrohack-0.0.5/src/astrohack/_utils/_algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import scipy
+import scipy.signal as scisig
 import numba
 
 import numpy as np
 
 def _apply_mask(data, scaling=0.5):
     """ Applies a cropping mask to the input data according to the scale factor
 
@@ -130,15 +131,15 @@
         float: peak maximum value
     """
     masked_data = _apply_mask(data, scaling=scaling)
 
     array = masked_data.flatten()
     cutoff = np.abs(array).max() * height
 
-    index, _ = scipy.signal.find_peaks(np.abs(array), height=cutoff)
+    index, _ = scisig.find_peaks(np.abs(array), height=cutoff)
     x, y = np.unravel_index(index, masked_data.shape)
 
     center = (masked_data.shape[0] // 2, masked_data.shape[1] // 2)
 
     distances = _calculate_euclidean_distance(x, y, center)
     index = distances.argmin()
```

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_constants.py` & `astrohack-0.0.5/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_conversion.py` & `astrohack-0.0.5/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             # Set the resource label to the ip of the node that the worker is on, so that tasks that require a specific node can be assigned to the correct worker.
             ip = worker[worker.rfind('/')+1:worker.rfind(':')]
             scheduler.add_resources(worker=worker,resources={ip:1})
 
     def update_graph(self, scheduler, dsk=None, keys=None, restrictions=None,
                      **kw):
         if self.autorestrictor:
-            print('Using autorestrictor')
+            #print('Using autorestrictor')
             """Processes dependencies to assign tasks to specific workers."""
             workers = list(scheduler.workers.keys())
             n_worker = len(workers)
 
             tasks = scheduler.tasks
             dependencies = kw["dependencies"]
```

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 
 from astrohack._utils._logger._astrohack_logger import _setup_astrohack_worker_logger
 
 class _astrohack_worker():
     def __init__(self,local_cache,log_parms):
-        print('init local cache')
+        #print('init local cache')
         self.local_cache = local_cache
         
         #print('log_parms',log_parms)
 
         self.log_to_term=log_parms['log_to_term']
         self.log_to_file=log_parms['log_to_file']
         self.log_file=log_parms['log_file']
```

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_holog.py` & `astrohack-0.0.5/src/astrohack/_utils/_holog.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,272 +39,277 @@
 
     Args:
         holog_chunk_params (dict): Dictionary containing holography parameters.
     """
     logger = _get_astrohack_logger()
     
     c = scipy.constants.speed_of_light
+    
 
     holog_file, ant_data_dict = _load_holog_file(
         holog_chunk_params["holog_file"],
-        dask_load=True,
+        dask_load=False,
         load_pnt_dict=False,
         ant_id=holog_chunk_params["ant_id"],
+        ddi_id=holog_chunk_params["ddi_id"]
     )
 
     meta_data = _read_meta_data(holog_chunk_params["holog_file"])
 
     # Calculate lm coordinates
     l, m = _calc_coords(holog_chunk_params["grid_size"], holog_chunk_params["cell_size"])
     grid_l, grid_m = list(map(np.transpose, np.meshgrid(l, m)))
     
     to_stokes = holog_chunk_params["to_stokes"]
 
-    for ddi in ant_data_dict.keys():
-    #for ddi in [1]: #### NB NB NB remove
-        n_scan = len(ant_data_dict[ddi].keys())
-        
-        # For a fixed ddi the frequency axis should not change over scans, consequently we only have to consider the first scan.
-        scan0 = list(ant_data_dict[ddi].keys())[0]  
-        
-        freq_chan = ant_data_dict[ddi][scan0].chan.values
-        n_chan = ant_data_dict[ddi][scan0].dims["chan"]
-        n_pol = ant_data_dict[ddi][scan0].dims["pol"]
+    ddi = holog_chunk_params["ddi_id"]
+    n_holog_map = len(ant_data_dict[ddi].keys())
+    
+    # For a fixed ddi the frequency axis should not change over holog_maps, consequently we only have to consider the first holog_map.
+    map0 = list(ant_data_dict[ddi].keys())[0]
+    
+    freq_chan = ant_data_dict[ddi][map0].chan.values
+    n_chan = ant_data_dict[ddi][map0].dims["chan"]
+    n_pol = ant_data_dict[ddi][map0].dims["pol"]
+    
+    if holog_chunk_params["chan_average"]:
+        reference_scaling_frequency = holog_chunk_params["reference_scaling_frequency"]
+
+        if reference_scaling_frequency is None:
+            reference_scaling_frequency = np.mean(freq_chan)
+
+        avg_chan_map, avg_freq = _create_average_chan_map(freq_chan, holog_chunk_params["chan_tolerance_factor"])
         
-        if holog_chunk_params["chan_average"]:
-            reference_scaling_frequency = holog_chunk_params["reference_scaling_frequency"]
+        # Only a single channel left after averaging.
+        beam_grid = np.zeros((n_holog_map,) + (1, n_pol) + grid_l.shape, dtype=np.complex)
+        
+        
+    else:
+        beam_grid = np.zeros((n_holog_map,) + (n_chan, n_pol) + grid_l.shape, dtype=np.complex)
 
-            if reference_scaling_frequency is None:
-                reference_scaling_frequency = np.mean(freq_chan)
+    time_centroid = []
 
-            avg_chan_map, avg_freq = _create_average_chan_map(freq_chan, holog_chunk_params["chan_tolerance_factor"])
-            
-            # Only a single channel left after averaging.
-            beam_grid = np.zeros((n_scan,) + (1, n_pol) + grid_l.shape, dtype=np.complex)  
-            
-            
-        else:
-            beam_grid = np.zeros((n_scan,) + (n_chan, n_pol) + grid_l.shape, dtype=np.complex)
+    for holog_map_index, holog_map in enumerate(ant_data_dict[ddi].keys()):
+        ant_xds = ant_data_dict[ddi][holog_map]
+        
+        ###To Do: Add flagging code
 
-        time_centroid = []
+        # Grid the data
+        vis = ant_xds.VIS.values
+        vis[vis==np.nan] = 0.0
+        lm = ant_xds.DIRECTIONAL_COSINES.values
+        weight = ant_xds.WEIGHT.values
 
-        for scan_index, scan in enumerate(ant_data_dict[ddi].keys()):
-            ant_xds = ant_data_dict[ddi][scan]
-            
-            ###To Do: Add flagging code
+        if holog_chunk_params["chan_average"]:
+            vis_avg, weight_sum = _chunked_average(vis, weight, avg_chan_map, avg_freq)
+            lm_freq_scaled = lm[:, :, None] * (avg_freq / reference_scaling_frequency)
 
-            # Grid the data
-            vis = ant_xds.VIS.values
-            vis[vis==np.nan] = 0.0
-            lm = ant_xds.DIRECTIONAL_COSINES.values
-            weight = ant_xds.WEIGHT.values
-
-            if holog_chunk_params["chan_average"]:
-                vis_avg, weight_sum = _chunked_average(vis, weight, avg_chan_map, avg_freq)
-                lm_freq_scaled = lm[:, :, None] * (avg_freq / reference_scaling_frequency)
+            n_chan = avg_freq.shape[0]
+            
+            # Unavoidable for loop because lm change over frequency.
+            for chan_index in range(n_chan):
 
-                n_chan = avg_freq.shape[0]
-                
-                # Unavoidable for loop because lm change over frequency.
-                for chan_index in range(n_chan):
-    
-                    # Average scaled beams.
-                    beam_grid[scan_index, 0, :, :, :] = (beam_grid[scan_index, 0, :, :, :] + np.moveaxis(griddata(lm_freq_scaled[:, :, chan_index], vis_avg[:, chan_index, :], (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0),(2),(0)))
+                # Average scaled beams.
+                beam_grid[holog_map_index, 0, :, :, :] = (beam_grid[holog_map_index, 0, :, :, :] + np.moveaxis(griddata(lm_freq_scaled[:, :, chan_index], vis_avg[:, chan_index, :], (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0),(2),(0)))
 
-                # Avergaing now complete
-                n_chan =  1 
-                
-                freq_chan = [np.mean(avg_freq)]
-            else:
-                beam_grid[scan_index, ...] = np.moveaxis(griddata(lm, vis, (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0), (0,1), (2,3))
+            # Avergaing now complete
+            n_chan =  1
+            
+            freq_chan = [np.mean(avg_freq)]
+        else:
+            beam_grid[holog_map_index, ...] = np.moveaxis(griddata(lm, vis, (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0), (0,1), (2,3))
 
 
-            time_centroid_index = ant_data_dict[ddi][scan].dims["time"] // 2
+        time_centroid_index = ant_data_dict[ddi][holog_map].dims["time"] // 2
 
-            time_centroid.append(ant_data_dict[ddi][scan].coords["time"][time_centroid_index].values)
-            
-            
-            ###########
+        time_centroid.append(ant_data_dict[ddi][holog_map].coords["time"][time_centroid_index].values)
+        
+        
+        ###########
 #            shape = np.array(beam_grid.shape[-2:])//2
 #            phase_diff = np.angle(beam_grid[:, :, 0, shape[0], shape[1]]) - np.angle(beam_grid[:, :, 3, shape[0], shape[1]])
 #            print('phase_diff',phase_diff)
 #            #beam_grid[:,:,0,:,:] = beam_grid[:,:,0,:,:]*(np.exp(-1j*phase_diff/2)[None,None,:,:])
 #            #beam_grid[:,:,3,:,:] = beam_grid[:,:,3,:,:]*(np.exp(1j*phase_diff/2)[None,None,:,:])
 #            #beam_grid[:,:,0,:,:] = beam_grid[:,:,0,:,:]*(np.exp(-1j*phase_diff/2)[None,None,:,:])
 #            beam_grid[:,:,3,:,:] = beam_grid[:,:,3,:,:]*(np.exp(1j*phase_diff)[None,None,:,:])
 #            #Not sure what to do with cross pol (RL, LR / XY, YX)
 #
 #            print(beam_grid[0, 0, 0, 15, 15],beam_grid[0, 0, 3, 15, 15])
 #            print(np.angle(beam_grid[0, 0, 0, 15, 15]-beam_grid[0, 0, 3, 15, 15]))
 #            print(np.angle(beam_grid[0, 0, 0, 15, 15]),np.angle(beam_grid[0, 0, 3, 15, 15]))
 #            #beam_grid[0, 0, 3, ...] = -1*beam_grid[0, 0, 3, ...]
 
-            for chan in range(n_chan): ### Todo: Vectorize scan and channel axis
-                xx_peak = _find_peak_beam_value(beam_grid[scan_index, chan, 0, ...], scaling=0.25)
-                
-                yy_peak = _find_peak_beam_value(beam_grid[scan_index, chan, 3, ...], scaling=0.25)
+        for chan in range(n_chan): ### Todo: Vectorize holog_map and channel axis
+            xx_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 0, ...], scaling=0.25)
+            
+            yy_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 3, ...], scaling=0.25)
 
-                #print(xx_peak,yy_peak,beam_grid[scan_index, chan, 0, ...][15,15],beam_grid[scan_index, chan, 3, ...][15,15])
-                #print(np.abs(xx_peak),np.abs(yy_peak),np.abs(beam_grid[scan_index, chan, 0, ...][15,15]),np.abs(beam_grid[scan_index, chan, 3, ...][15,15]))
-                #print(np.angle(xx_peak)*180/np.pi,np.angle(yy_peak)*180/np.pi)
-                
-                normalization = np.abs(0.5 * (xx_peak + yy_peak))
-                beam_grid[scan_index, chan, ...] /= normalization
-                #print('####normalization ', normalization)
+            #print(xx_peak,yy_peak,beam_grid[holog_map_index, chan, 0, ...][15,15],beam_grid[holog_map_index, chan, 3, ...][15,15])
+            #print(np.abs(xx_peak),np.abs(yy_peak),np.abs(beam_grid[holog_map_index, chan, 0, ...][15,15]),np.abs(beam_grid[holog_map_index, chan, 3, ...][15,15]))
+            #print(np.angle(xx_peak)*180/np.pi,np.angle(yy_peak)*180/np.pi)
+            
+            normalization = np.abs(0.5 * (xx_peak + yy_peak))
+            beam_grid[holog_map_index, chan, ...] /= normalization
+            #print('####normalization ', normalization)
 
-        beam_grid = _parallactic_derotation(data=beam_grid, parallactic_angle_dict=ant_data_dict[ddi])
-        
+    beam_grid = _parallactic_derotation(data=beam_grid, parallactic_angle_dict=ant_data_dict[ddi])
+    
 
-        ###############
-        if to_stokes:
-            beam_grid = _to_stokes(beam_grid,ant_data_dict[ddi][scan].pol.values)
-        ###############
-        
-        if holog_chunk_params["scan_average"]:          
-            beam_grid = np.mean(beam_grid,axis=0)[None,...]
-        
-        # Current bottleneck
-        aperture_grid, u, v, uv_cell_size = _calculate_aperture_pattern(
-            grid=beam_grid,
-            delta=holog_chunk_params["cell_size"],
-            padding_factor=holog_chunk_params["padding_factor"],
-        )
-        
-        # Get telescope info
-        ant_name = ant_data_dict[ddi][scan].attrs["antenna_name"]
+    ###############
+    pol = beam_grid,ant_data_dict[ddi][holog_map].pol.values
+    if to_stokes:
+        beam_grid = _to_stokes(beam_grid,ant_data_dict[ddi][holog_map].pol.values)
+        pol=['I','Q','U','V']
+    ###############
+    
+    if holog_chunk_params["scan_average"]:
+        beam_grid = np.mean(beam_grid,axis=0)[None,...]
+        time_centroid = np.mean(np.array(time_centroid))
+    
+    # Current bottleneck
+    aperture_grid, u, v, uv_cell_size = _calculate_aperture_pattern(
+        grid=beam_grid,
+        delta=holog_chunk_params["cell_size"],
+        padding_factor=holog_chunk_params["padding_factor"],
+    )
+    
+    # Get telescope info
+    ant_name = ant_data_dict[ddi][holog_map].attrs["antenna_name"]
+    
+    if  ant_name.upper().__contains__('DV'):
+        telescope_name = "_".join((meta_data['telescope_name'], 'DV'))
+
+    elif  ant_name.upper().__contains__('DA'):
+        telescope_name = "_".join((meta_data['telescope_name'], 'DA'))
         
-        if  ant_name.upper().__contains__('DV'):
-            telescope_name = "_".join((meta_data['telescope_name'], 'DV'))
+    elif  ant_name.upper().__contains__('EA'):
+        telescope_name = 'VLA'
 
-        elif  ant_name.upper().__contains__('DA'):
-            telescope_name = "_".join((meta_data['telescope_name'], 'DA'))
-            
-        elif  ant_name.upper().__contains__('EA'):
-            telescope_name = 'VLA'
+    else:
+        raise Exception("Antenna type not found: {}".format(meta_data['ant_name']))
 
-        else:
-            raise Exception("Antenna type not found: {}".format(meta_data['ant_name']))
+    telescope = Telescope(telescope_name)
+
+    min_wavelength = scipy.constants.speed_of_light/freq_chan[0]
+    max_aperture_radius = (0.5*telescope.diam)/min_wavelength
     
-        telescope = Telescope(telescope_name)
+    image_slice = aperture_grid[0, 0, 0, ...]
+    center_pixel = np.array(image_slice.shape[0:2])//2
+    radius_u = int(np.where(np.abs(u) < max_aperture_radius*1.1)[0].max() - center_pixel[0]) # Factor of 1.1: Let's not be too aggresive
+    radius_v = int(np.where(np.abs(v) < max_aperture_radius*1.1)[0].max() - center_pixel[1]) # Factor of 1.1: Let's not be too aggresive
+        
+    if radius_v > radius_u:
+        radius = radius_v
+    else:
+        radius = radius_u
+
+    if holog_chunk_params['apply_mask']:
+    # Masking Aperture image
+
+        mask = _mask_circular_disk(
+            center=None,
+            radius=radius,
+            array=aperture_grid,
+        )
 
-        min_wavelength = scipy.constants.speed_of_light/freq_chan[0]
-        max_aperture_radius = (0.5*telescope.diam)/min_wavelength
-        
-        image_slice = aperture_grid[0, 0, 0, ...]
-        center_pixel = np.array(image_slice.shape[0:2])//2
-        radius_u = int(np.where(np.abs(u) < max_aperture_radius*1.1)[0].max() - center_pixel[0]) # Factor of 1.1: Let's not be too aggresive
-        radius_v = int(np.where(np.abs(v) < max_aperture_radius*1.1)[0].max() - center_pixel[1]) # Factor of 1.1: Let's not be too aggresive
-            
-        if radius_v > radius_u:
-            radius = radius_v
-        else:
-            radius = radius_u
+        aperture_grid = mask*aperture_grid
 
-        if holog_chunk_params['apply_mask']:
-        # Masking Aperture image
+    start_cut = center_pixel - radius
+    end_cut = center_pixel + radius
 
-            mask = _mask_circular_disk(
-                center=None,
-                radius=radius,
-                array=aperture_grid,
-            )
-
-            aperture_grid = mask*aperture_grid
-
-        start_cut = center_pixel - radius
-        end_cut = center_pixel + radius
-
-        amplitude = np.absolute(aperture_grid[..., start_cut[0]:end_cut[0], start_cut[1]:end_cut[1]])
-        phase = np.angle(aperture_grid[..., start_cut[0]:end_cut[0], start_cut[1]:end_cut[1]])
-        phase_corrected_angle = np.zeros_like(phase)
-        u_prime = u[start_cut[0]:end_cut[0]]
-        v_prime = v[start_cut[1]:end_cut[1]]
-        
-
-        phase_fit_par = holog_chunk_params["phase_fit"]
-        if isinstance(phase_fit_par, bool):
-            do_phase_fit = phase_fit_par
-            do_pnt_off = True
-            do_xy_foc_off = True
-            do_z_foc_off = True
-            do_cass_off = True
-            if telescope.name == 'VLA' or telescope.name == 'VLBA':
-                do_sub_til = True
-            else:
-                do_sub_til = False
-        elif isinstance(phase_fit_par, (np.ndarray, list, tuple)):
-            if len(phase_fit_par) != 5:
-                logger.error("Phase fit parameter must have 5 elements")
-                raise Exception
-            else:
-                if np.sum(phase_fit_par) == 0:
-                    do_phase_fit = False
-                else:
-                    do_phase_fit = True
-                    do_pnt_off, do_xy_foc_off, do_z_foc_off, do_sub_til, do_cass_off = phase_fit_par
+    amplitude = np.absolute(aperture_grid[..., start_cut[0]:end_cut[0], start_cut[1]:end_cut[1]])
+    phase = np.angle(aperture_grid[..., start_cut[0]:end_cut[0], start_cut[1]:end_cut[1]])
+    phase_corrected_angle = np.zeros_like(phase)
+    u_prime = u[start_cut[0]:end_cut[0]]
+    v_prime = v[start_cut[1]:end_cut[1]]
+    
+
+    phase_fit_par = holog_chunk_params["phase_fit"]
+    if isinstance(phase_fit_par, bool):
+        do_phase_fit = phase_fit_par
+        do_pnt_off = True
+        do_xy_foc_off = True
+        do_z_foc_off = True
+        do_cass_off = True
+        if telescope.name == 'VLA' or telescope.name == 'VLBA':
+            do_sub_til = True
         else:
-            logger.error("Phase fit parameter is neither a boolean nor an array of booleans")
+            do_sub_til = False
+    elif isinstance(phase_fit_par, (np.ndarray, list, tuple)):
+        if len(phase_fit_par) != 5:
+            logger.error("Phase fit parameter must have 5 elements")
             raise Exception
-
-        if do_phase_fit:
-            logger.info("Applying phase correction ...")
-            
-            if to_stokes:
-                pols=(0,)
-            else:
-                pols=(0, 3)
-            
-            #? Wavelength
-            max_wavelength = scipy.constants.speed_of_light/freq_chan[-1]
-            
-            results, errors, phase_corrected_angle, _, in_rms, out_rms = _phase_fitting_block(
-                        pols=pols,
-                        wavelength=max_wavelength,
-                        telescope=telescope,
-                        cellxy=uv_cell_size[0]*max_wavelength, # THIS HAS TO BE CHANGES, (X, Y) CELL SIZE ARE NOT THE SAME.
-                        amplitude_image=amplitude,
-                        phase_image=phase,
-                        pointing_offset=do_pnt_off,
-                        focus_xy_offsets=do_xy_foc_off,
-                        focus_z_offset=do_z_foc_off,
-                        subreflector_tilt=do_sub_til,
-                        cassegrain_offset=do_cass_off)
         else:
-            logger.info("Skipping phase correction ...")
+            if np.sum(phase_fit_par) == 0:
+                do_phase_fit = False
+            else:
+                do_phase_fit = True
+                do_pnt_off, do_xy_foc_off, do_z_foc_off, do_sub_til, do_cass_off = phase_fit_par
+    else:
+        logger.error("Phase fit parameter is neither a boolean nor an array of booleans")
+        raise Exception
 
+    if do_phase_fit:
+        logger.info("Applying phase correction ...")
         
-        ###To Do: Add Paralactic angle as a non-dimension coordinate dependant on time.
-        xds = xr.Dataset()
-
-        xds["BEAM"] = xr.DataArray(beam_grid, dims=["time-centroid", "chan", "pol", "l", "m"])
-        xds["APERTURE"] = xr.DataArray(aperture_grid, dims=["time-centroid", "chan", "pol", "u", "v"])
+        if to_stokes:
+            pols=(0,)
+        else:
+            pols=(0, 3)
+        
+        #? Wavelength
+        max_wavelength = scipy.constants.speed_of_light/freq_chan[-1]
         
-        xds["AMPLITUDE"] = xr.DataArray(amplitude, dims=["time-centroid", "chan", "pol", "u_prime", "v_prime"])
-        xds["ANGLE"] = xr.DataArray(phase_corrected_angle, dims=["time-centroid", "chan", "pol", "u_prime", "v_prime"])
-
-        xds.attrs["ant_id"] = holog_chunk_params["ant_id"]
-        xds.attrs["ant_name"] = ant_name
-        xds.attrs["telescope_name"] = meta_data['telescope_name']
-        xds.attrs["time_centroid"] = np.array(time_centroid)
-
-        coords = {}
-        coords["time_centroid"] = np.array(time_centroid)
-        coords["ddi"] = list(ant_data_dict.keys())
-        coords["pol"] = [i for i in range(n_pol)]
-        coords["l"] = l
-        coords["m"] = m
-        coords["u"] = u
-        coords["v"] = v
-        coords["u_prime"] = u_prime
-        coords["v_prime"] = v_prime
-        coords["chan"] = freq_chan
+        results, errors, phase_corrected_angle, _, in_rms, out_rms = _phase_fitting_block(
+                    pols=pols,
+                    wavelength=max_wavelength,
+                    telescope=telescope,
+                    cellxy=uv_cell_size[0]*max_wavelength, # THIS HAS TO BE CHANGES, (X, Y) CELL SIZE ARE NOT THE SAME.
+                    amplitude_image=amplitude,
+                    phase_image=phase,
+                    pointing_offset=do_pnt_off,
+                    focus_xy_offsets=do_xy_foc_off,
+                    focus_z_offset=do_z_foc_off,
+                    subreflector_tilt=do_sub_til,
+                    cassegrain_offset=do_cass_off)
+    else:
+        logger.info("Skipping phase correction ...")
 
-        xds = xds.assign_coords(coords)
+    
+    ###To Do: Add Paralactic angle as a non-dimension coordinate dependant on time.
+    xds = xr.Dataset()
+
+    xds["BEAM"] = xr.DataArray(beam_grid, dims=["time", "chan", "pol", "l", "m"])
+    xds["APERTURE"] = xr.DataArray(aperture_grid, dims=["time", "chan", "pol", "u", "v"])
+    
+    xds["AMPLITUDE"] = xr.DataArray(amplitude, dims=["time", "chan", "pol", "u_prime", "v_prime"])
+    xds["ANGLE"] = xr.DataArray(phase_corrected_angle, dims=["time", "chan", "pol", "u_prime", "v_prime"])
+
+    xds.attrs["ant_id"] = holog_chunk_params["ant_id"]
+    xds.attrs["ant_name"] = ant_name
+    xds.attrs["telescope_name"] = meta_data['telescope_name']
+    xds.attrs["time_centroid"] = np.array(time_centroid)
+    xds.attrs["ddi"] = ddi
+
+    coords = {}
+    #coords["time"] = np.array(time_centroid)
+    coords["ddi"] = list(ant_data_dict.keys())
+    coords["pol"] = pol
+    coords["l"] = l
+    coords["m"] = m
+    coords["u"] = u
+    coords["v"] = v
+    coords["u_prime"] = u_prime
+    coords["v_prime"] = v_prime
+    coords["chan"] = freq_chan
+
+    xds = xds.assign_coords(coords)
 
-        xds.to_zarr("{name}/{ant}/{ddi}".format(name= holog_chunk_params["image_file"], ant=holog_chunk_params["ant_id"], ddi=ddi), mode="w", compute=True, consolidated=True)
+    xds.to_zarr("{name}/{ant}/{ddi}".format(name= holog_chunk_params["image_file"], ant=holog_chunk_params["ant_id"], ddi=ddi), mode="w", compute=True, consolidated=True)
 
 
 def _create_average_chan_map(freq_chan, chan_tolerance_factor):
     n_chan = len(freq_chan)
     cf_chan_map = np.zeros((n_chan,), dtype=int)
 
     orig_width = (np.max(freq_chan) - np.min(freq_chan)) / len(freq_chan)
@@ -332,43 +337,49 @@
     for i in range(n_chan):
         cf_chan_map[i], _ = _find_nearest(pb_freq, freq_chan[i])
 
     return cf_chan_map, pb_freq
 
 def _create_holog_meta_data(holog_file, holog_dict, holog_params):
     """Save holog file meta information to json file with the transformation
-        of the ordering (ddi, scan, ant) --> (ant, ddi, scan).
+        of the ordering (ddi, holog_map, ant) --> (ant, ddi, holog_map).
 
     Args:
         holog_name (str): holog file name.
         holog_dict (dict): Dictionary containing msdx data.
     """
     data_extent = []
     lm_extent = {"l": {"min": [], "max": []}, "m": {"min": [], "max": []}}
     ant_holog_dict = {}
-
-    for ddi, scan_dict in holog_dict.items():
+    
+    for ddi, map_dict in holog_dict.items():
         if "ddi_" in ddi:
-            for scan, ant_dict in scan_dict.items():
-                if "scan_" in scan:
+            for map, ant_dict in map_dict.items():
+                if "map_" in map:
                     for ant, xds in ant_dict.items():
                         if "ant_" in ant:
                             if ant not in ant_holog_dict:
-                                ant_holog_dict[ant] = {ddi:{scan:{}}}
+                                ant_holog_dict[ant] = {ddi:{map:{}}}
                             elif ddi not in ant_holog_dict[ant]:
-                                ant_holog_dict[ant][ddi] = {scan:{}}
+                                ant_holog_dict[ant][ddi] = {map:{}}
                     
-                            ant_holog_dict[ant][ddi][scan] = xds.to_dict(data=False)
+                            ant_holog_dict[ant][ddi][map] = xds.to_dict(data=False)
                 
                             #ant_sub_dict.setdefault(ddi, {})
-                            #ant_holog_dict.setdefault(ant, ant_sub_dict)[ddi][scan] = xds.to_dict(data=False)
+                            #ant_holog_dict.setdefault(ant, ant_sub_dict)[ddi][map] = xds.to_dict(data=False)
 
-                            # Find the average (l, m) extent for each antenna, over (ddi, scan) and write the meta data to file.
+                            # Find the average (l, m) extent for each antenna, over (ddi, map) and write the meta data to file.
                             dims = xds.dims
-                    
+                            
+                            lm_extent["l"]["min"].append(xds.attrs["l_min"])
+                            lm_extent["l"]["max"].append(xds.attrs["l_max"])
+                            lm_extent["m"]["min"].append(xds.attrs["m_min"])
+                            lm_extent["m"]["max"].append(xds.attrs["m_max"])
+                            
+                            '''
                             lm_extent["l"]["min"].append(
                                 np.min(xds.DIRECTIONAL_COSINES.values[:, 0])
                             )
 
                             lm_extent["l"]["max"].append(
                                 np.max(xds.DIRECTIONAL_COSINES.values[:, 0])
                             )
@@ -376,19 +387,19 @@
                             lm_extent["m"]["min"].append(
                                 np.min(xds.DIRECTIONAL_COSINES.values[:, 1])
                             )
 
                             lm_extent["m"]["max"].append(
                                 np.max(xds.DIRECTIONAL_COSINES.values[:, 1])
                             )
+                            '''
                     
                             data_extent.append(dims["time"])
 
 
-    
     max_value = int(np.array(data_extent).max())
 
     max_extent = {
         "n_time": max_value,
         "telescope_name": holog_params['telescope_name'],
         "ant_map": holog_params['holog_obs_dict'],
         "extent": {
```

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_imaging.py` & `astrohack-0.0.5/src/astrohack/_utils/_imaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
     padded_grid = np.pad(
         array=grid,
         pad_width=[(0, 0), (0, 0), (0, 0), (padding, padding), (padding, padding)],
         mode="constant",
     )
 
+    import scipy.fftpack
     shifted = scipy.fftpack.ifftshift(padded_grid)
 
     grid_fft = scipy.fftpack.fft2(shifted)
 
     aperture_grid = scipy.fftpack.fftshift(grid_fft)
 
     u_size = aperture_grid.shape[-2]
```

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_io.py` & `astrohack-0.0.5/src/astrohack/_utils/_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         raise FileExistsError
     elif  (os.path.exists(file) is True) and (overwrite is True):
         logger.warning(
             file + " will be overwritten."
         )
 
 
-def _load_panel_file(file=None, panel_dict=None):
+def _load_panel_file(file=None, panel_dict=None, dask_load=True):
     """ Open panel file.
 
     Args:
         file (str, optional): Path to panel file. Defaults to None.
 
     Returns:
         bool: Nested dictionary containing panel data xds.
@@ -59,29 +59,34 @@
     if panel_dict is not None:
             panel_data_dict = panel_dict
     
     ant_list =  [dir_name for dir_name in os.listdir(file) if os.path.isdir(file)]
     
     try:
         for ant in ant_list:
-            ddi_list =  [dir_name for dir_name in os.listdir(file + "/" + str(ant)) if os.path.isdir(file + "/" + str(ant))]
-            panel_data_dict[ant] = {}
-            
-            for ddi in ddi_list:
-                panel_data_dict[ant][ddi] = xr.open_zarr("{name}/{ant}/{ddi}/xds.zarr".format(name=file, ant=ant, ddi=ddi))                
+            if 'ant' in ant:
+                ddi_list =  [dir_name for dir_name in os.listdir(file + "/" + str(ant)) if os.path.isdir(file + "/" + str(ant))]
+                panel_data_dict[ant] = {}
+                
+                for ddi in ddi_list:
+                    if 'ddi' in ddi:
+                        if dask_load:
+                            panel_data_dict[ant][ddi] = xr.open_zarr("{name}/{ant}/{ddi}/xds.zarr".format(name=file, ant=ant, ddi=ddi))
+                        else:
+                            panel_data_dict[ant][ddi] = _open_no_dask_zarr("{name}/{ant}/{ddi}/xds.zarr".format(name=file, ant=ant, ddi=ddi))
     
     except Exception as e:
             logger.error(str(e))
             raise
 
     
     return panel_data_dict
 
 
-def _load_image_file(file=None, image_dict=None):
+def _load_image_file(file=None, image_dict=None,  dask_load=True):
         """ Open hologgraphy file.
 
         Args:s
             file (str, optional): Path to holography file. Defaults to None.
 
         Returns:
             bool: bool describing whether the file was opened properly
@@ -92,82 +97,87 @@
         if image_dict is not None:
             ant_data_dict = image_dict
 
         ant_list =  [dir_name for dir_name in os.listdir(file) if os.path.isdir(file)]
         
         try:
             for ant in ant_list:
-                ddi_list =  [dir_name for dir_name in os.listdir(file + "/" + str(ant)) if os.path.isdir(file + "/" + str(ant))]
-                ant_data_dict[ant] = {}
-                
-                for ddi in ddi_list:
-                    ant_data_dict[ant][ddi] = xr.open_zarr("{name}/{ant}/{ddi}".format(name=file, ant=ant, ddi=ddi) )
+                if 'ant' in ant:
+                    ddi_list =  [dir_name for dir_name in os.listdir(file + "/" + str(ant)) if os.path.isdir(file + "/" + str(ant))]
+                    ant_data_dict[ant] = {}
+                    
+                    for ddi in ddi_list:
+                        if 'ddi' in ddi:
+                            if dask_load:
+                                ant_data_dict[ant][ddi] = xr.open_zarr("{name}/{ant}/{ddi}".format(name=file, ant=ant, ddi=ddi))
+                            else:
+                                ant_data_dict[ant][ddi] = _open_no_dask_zarr("{name}/{ant}/{ddi}".format(name=file, ant=ant, ddi=ddi))
 
         except Exception as e:
             logger.error(str(e))
             raise
 
         return ant_data_dict
 
 
-def _load_holog_file(holog_file, dask_load=True, load_pnt_dict=True, ant_id=None, holog_dict=None):
+def _load_holog_file(holog_file, dask_load=True, load_pnt_dict=True, ant_id=None, ddi_id=None, holog_dict=None):
     """Loads holog file from disk
 
     Args:
         holog_name (str): holog file name
 
     Returns:
-        hologfile (nested-dict): {
-                            'point.dict':{}, 'ddi':
-                                                {'scan':
-                                                    {'antenna':
-                                                        {
-                                                            xarray.DataArray
-                                                        }
-                                                    }
-                                                }
-                        }
+
     """
+    
     logger = _get_astrohack_logger()
     
     if holog_dict is None:
         holog_dict = {}
 
     if load_pnt_dict == True:
         logger.info("Loading pointing dictionary to holog ...")
         holog_dict["pnt_dict"] = _load_pnt_dict(file=holog_file, ant_list=None, dask_load=dask_load)
 
     for ddi in os.listdir(holog_file):
         if "ddi_" in ddi:
-            if ddi not in holog_dict:
-                holog_dict[ddi] = {}
-            for scan in os.listdir(os.path.join(holog_file, ddi)):
-                if "scan_" in scan:
-                    if scan not in holog_dict[ddi]:
-                        holog_dict[ddi][scan] = {}
-                    for ant in os.listdir(os.path.join(holog_file, ddi + "/" + scan)):
+            
+            if ddi_id is None:
+                if ddi not in holog_dict:
+                    holog_dict[ddi] = {}
+            else:
+                if (ddi == ddi_id):
+                    holog_dict[ddi] = {}
+                else:
+                    continue
+                
+            for holog_map in os.listdir(os.path.join(holog_file, ddi)):
+                if "map_" in holog_map:
+                    if holog_map not in holog_dict[ddi]:
+                        holog_dict[ddi][holog_map] = {}
+                    for ant in os.listdir(os.path.join(holog_file, ddi + "/" + holog_map)):
                         if "ant_" in ant:
-                            mapping_ant_vis_holog_data_name = os.path.join(
-                                holog_file, ddi + "/" + scan + "/" + ant
-                            )
-                            
-
-                            if dask_load:
-                                holog_dict[ddi][scan][ant] = xr.open_zarr(
-                                    mapping_ant_vis_holog_data_name
+                            if (ant_id is None) or (ant_id in ant):
+                                mapping_ant_vis_holog_data_name = os.path.join(
+                                    holog_file, ddi + "/" + holog_map + "/" + ant
                                 )
-                            else:
-                                holog_dict[ddi][scan][ant] = _open_no_dask_zarr(mapping_ant_vis_holog_data_name)
+                                
+
+                                if dask_load:
+                                    holog_dict[ddi][holog_map][ant] = xr.open_zarr(
+                                        mapping_ant_vis_holog_data_name
+                                    )
+                                else:
+                                    holog_dict[ddi][holog_map][ant] = _open_no_dask_zarr(mapping_ant_vis_holog_data_name)
 
     
-    if ant_id == None:
+    if ant_id is None:
         return holog_dict
         
-
-    return holog_dict, _read_data_from_holog_json(holog_file=holog_file, holog_dict=holog_dict, ant_id=ant_id)
+    return holog_dict, _read_data_from_holog_json(holog_file=holog_file, holog_dict=holog_dict, ant_id=ant_id, ddi_id=ddi_id)
 
 
 def _read_fits(filename):
     """
     Reads a square FITS file and do sanity checks on its dimensionality
     Args:
         filename: a string containing the FITS file name/path
@@ -214,14 +224,16 @@
         devname: Name of the deviation FITS file
 
     Returns:
     Xarray dataset
     """
     amphead, ampdata = _read_fits(ampname)
     devhead, devdata = _read_fits(devname)
+    ampdata = np.flipud(ampdata)
+    devdata = np.flipud(devdata)
 
     if amphead["NAXIS1"] != devhead["NAXIS1"]:
         raise Exception(ampname+' and '+devname+' have different dimensions')
     if amphead["CRPIX1"] != devhead["CRPIX1"] or amphead["CRVAL1"] != devhead["CRVAL1"] \
             or amphead["CDELT1"] != devhead["CDELT1"]:
         raise Exception(ampname+' and '+devname+' have different axes descriptions')
 
@@ -262,15 +274,15 @@
         if wrds[1] == "Visibilities":
             npoint = np.sqrt(int(wrds[-1]))
         elif wrds[1] == "Observing":
             wavelength = float(wrds[-2])
     return npoint, wavelength
 
 
-def _load_image_xds(file_stem, ant, ddi):
+def _load_image_xds(file_stem, ant, ddi, dask_load=True):
     """ Load specific image xds
 
     Args:
         file_name (str): File directory
         ant (int): Antenna ID
         ddi (int): DDI 
 
@@ -280,15 +292,18 @@
     Returns:
         zarr: zarr image file
     """
 
     image_path = "{image}/{ant}/{ddi}".format(image=file_stem, ant=ant, ddi=ddi)
 
     if os.path.isdir(image_path):
-        return xr.open_zarr(image_path)
+        if dask_load:
+            return xr.open_zarr(image_path)
+        else:
+            return _open_no_dask_zarr(image_path)
     else:
         raise FileNotFoundError("Image file: {} not found".format(image_path))
 
 
 def _read_meta_data(holog_file):
     """Reads dimensional data from holog meta file.
 
@@ -306,27 +321,28 @@
     except Exception as error:
         logger.error(str(error))
         raise
 
     return json_dict
 
 
-def _read_data_from_holog_json(holog_file, holog_dict, ant_id):
-    """Read holog file meta data and extract antenna based xds information for each (ddi, scan)
+def _read_data_from_holog_json(holog_file, holog_dict, ant_id, ddi_id=None):
+    """Read holog file meta data and extract antenna based xds information for each (ddi, holog_map)
 
     Args:
         holog_file (str): holog file name.
         holog_dict (dict): holog file dictionary containing msxds data.
         ant_id (int): Antenna id
 
     Returns:
-        nested dict: nested dictionary (ddi, scan, xds) with xds data embedded in it.
+        nested dict: nested dictionary (ddi, holog_map, xds) with xds data embedded in it.
     """
     logger = _get_astrohack_logger()
     ant_id_str = str(ant_id)
+    
 
     holog_meta_data = "/".join((holog_file, ".holog_json"))
 
     try:
         with open(holog_meta_data, "r") as json_file:
             holog_json = json.load(json_file)
 
@@ -334,17 +350,21 @@
         logger.error(str(error))
         raise
 
     ant_data_dict = {}
 
     for ddi in holog_json[ant_id_str].keys():
         if "ddi_" in ddi:
-            for scan in holog_json[ant_id_str][ddi].keys():
-                if "scan_" in scan:
-                    ant_data_dict.setdefault(ddi, {})[scan] = holog_dict[ddi][scan][ant_id]
+            if (ddi_id is not None) and (ddi != ddi_id):
+                continue
+                
+            for holog_map in holog_json[ant_id_str][ddi].keys():
+                if "map_" in holog_map:
+                    ant_data_dict.setdefault(ddi, {})[holog_map] = holog_dict[ddi][holog_map][ant_id]
+
 
     return ant_data_dict
 
 
 def _open_no_dask_zarr(zarr_name, slice_dict={}):
     """
     Alternative to xarray open_zarr where the arrays are not Dask Arrays.
@@ -422,20 +442,22 @@
         ms_name (str): Measurement file name.
         ant_id (int): Antenna id
         pnt_name (str): Name of output poitning dictinary file name.
     """
     logger = _get_astrohack_logger()
     
     ant_id = pnt_parms['ant_id']
+    ant_name = pnt_parms['ant_name']
     pnt_name = pnt_parms['pnt_name']
     scan_time_dict = pnt_parms['scan_time_dict']
     
+    table_obj = ctables.table(os.path.join(ms_name, "POINTING"), readonly=True, lockoptions={'option': 'usernoread'}, ack=False)
     tb = ctables.taql(
-        "select DIRECTION, TIME, TARGET, ENCODER, ANTENNA_ID, POINTING_OFFSET from %s WHERE ANTENNA_ID == %s"
-        % (os.path.join(ms_name, "POINTING"), ant_id)
+        "select DIRECTION, TIME, TARGET, ENCODER, ANTENNA_ID, POINTING_OFFSET from $table_obj WHERE ANTENNA_ID == %s"
+        % (ant_id)
     )
 
     ### NB: Add check if directions refrence frame is Azemuth Elevation (AZELGEO)
     try:
         direction = tb.getcol("DIRECTION")[:, 0, :]
         target = tb.getcol("TARGET")[:, 0, :]
         encoder = tb.getcol("ENCODER")
@@ -443,14 +465,15 @@
         pointing_offset = tb.getcol("POINTING_OFFSET")[:, 0, :]
     except Exception as e:
         tb.close()
         logger.warning("Skipping antenna " + str(ant_id) + " no pointing info")
 
         return 0
     tb.close()
+    table_obj.close()
     
     pnt_xds = xr.Dataset()
     coords = {"time": direction_time}
     pnt_xds = pnt_xds.assign_coords(coords)
 
     # Measurement set v2 definition: https://drive.google.com/file/d/1IapBTsFYnUT1qPu_UK09DIFGM81EIZQr/view?usp=sharing
     # DIRECTION: Antenna pointing direction
@@ -503,19 +526,19 @@
     ###############
 
     pnt_xds.attrs['ant_name'] = pnt_parms['ant_name']
     
     
     logger.info(
         "Writing pointing xds to {file}".format(
-            file=os.path.join(pnt_name, "ant_" + str(ant_id))
+            file=os.path.join(pnt_name, "ant_" + str(ant_name))
         )
     )
     
-    pnt_xds.to_zarr(os.path.join(pnt_name, "ant_{}".format(str(ant_id)) ), mode="w", compute=True, consolidated=True)
+    pnt_xds.to_zarr(os.path.join(pnt_name, "ant_{}".format(str(ant_name)) ), mode="w", compute=True, consolidated=True)
 
 @convert_dict_from_numba
 @njit(cache=False, nogil=True)
 def _extract_scan_time_dict(time, scan_ids, ddi_ids):
     d1 = Dict.empty(
         key_type=types.int64,
         value_type=np.zeros(2, dtype=types.float64),
@@ -710,15 +733,15 @@
     vis_map_dict,
     weight_map_dict,
     pnt_map_dict,
     time_vis,
     chan,
     pol,
     flagged_mapping_antennas,
-    scan,
+    holog_map_key,
     ddi,
     ms_name,
     ant_names,
     overwrite,
 ):
     """Create holog-structured, formatted output file and save to zarr.
 
@@ -727,15 +750,15 @@
         vis_map_dict (dict): a nested dictionary/map of weighted visibilities indexed as [antenna][time, chan, pol]; mainains time ordering.
         weight_map_dict (dict): weights dictionary/map for visibilites in vis_map_dict
         pnt_map_dict (dict): pointing table map dictionary
         time_vis (numpy.ndarray): time_vis values
         chan (numpy.ndarray): channel values
         pol (numpy.ndarray): polarization values
         flagged_mapping_antennas (numpy.ndarray): list of mapping antennas that have been flagged.
-        scan (numpy.ndarray): scan number
+        holog_map_key(string): holog map id string
         ddi (numpy.ndarray): data description id; a combination of polarization and spectral window
     """
     logger = _get_astrohack_logger()
 
     ctb = ctables.table("/".join((ms_name, "ANTENNA")))
     observing_location = ctb.getcol("POSITION")
 
@@ -748,15 +771,15 @@
     astro_time_vis = astropy.time.Time(time_vis_days, format="mjd")
     time_samples, indicies = _get_time_samples(astro_time_vis)
 
     coords = {"time": time_vis, "chan": chan, "pol": pol}
 
     for map_ant_index in vis_map_dict.keys():
         if map_ant_index not in flagged_mapping_antennas:
-            map_ant_tag = 'ant_' + str(map_ant_index)
+            map_ant_tag = 'ant_' + ant_names[map_ant_index] #'ant_' + str(map_ant_index)
 
             direction = np.take(pnt_map_dict[map_ant_tag], indicies, axis=0)
 
             parallactic_samples = _calculate_parallactic_angle_chunk(
                 time_samples=time_samples,
                 observing_location=observing_location[map_ant_index],
                 direction=direction
@@ -772,35 +795,42 @@
                 weight_map_dict[map_ant_index], dims=["time", "chan", "pol"]
             )
 
             xds["DIRECTIONAL_COSINES"] = xr.DataArray(
                 pnt_map_dict[map_ant_tag], dims=["time", "lm"]
             )
 
-            xds.attrs["scan"] = scan
-            xds.attrs["ant_id"] = map_ant_tag
+            xds.attrs["holog_map_key"] = holog_map_key
+            #xds.attrs["ant_id"] = map_ant_tag
             xds.attrs["ddi"] = ddi
             xds.attrs["parallactic_samples"] = parallactic_samples
             xds.attrs["telescope_name"] = telescope_name
             xds.attrs["antenna_name"] = ant_names[map_ant_index]
+            
+            xds.attrs["l_max"] = np.max(xds["DIRECTIONAL_COSINES"][:,0].values)
+            xds.attrs["l_min"] = np.min(xds["DIRECTIONAL_COSINES"][:,0].values)
+            xds.attrs["m_max"] = np.max(xds["DIRECTIONAL_COSINES"][:,1].values)
+            xds.attrs["m_min"] = np.min(xds["DIRECTIONAL_COSINES"][:,1].values)
+            
+            #print(xds)
 
             holog_file = holog_name
 
             if overwrite is False:
                 if os.path.exists(holog_file):
                     logger.error(
                         "Holog file {file} exists. To overwite set the overwrite=True option in extract_holog or remove current file.".format(file=holog_file))
                     raise
 
             logger.info(
                 "Writing holog file to {file}".format(file=holog_file)
             )
             xds.to_zarr(
                 os.path.join(
-                    holog_file, 'ddi_' + str(ddi) + "/" + "scan_" + str(scan) + "/" + "ant_" + str(map_ant_index)
+                    holog_file, 'ddi_' + str(ddi) + "/" + str(holog_map_key) + "/" + "ant_" + str(ant_names[map_ant_index])
                 ),
                 mode="w",
                 compute=True,
                 consolidated=True,
             )
 
         else:
@@ -822,58 +852,66 @@
         map_ant_ids (numpy.narray): Array of antenna_id values corresponding to mapping data.
         ref_ant_ids (numpy.narray): Arry of antenna_id values corresponding to reference data.
         sel_state_ids (list): List pf state_ids corresponding to holography data/
     """
     logger = _get_astrohack_logger()
 
     ms_name = extract_holog_params["ms_name"]
-    pnt_name = extract_holog_params["pnt_name"]
+    pnt_name = extract_holog_params["point_name"]
     data_col = extract_holog_params["data_col"]
     ddi = extract_holog_params["ddi"]
     scans = extract_holog_params["scans"]
     ant_names = extract_holog_params["ant_names"]
     ref_ant_per_map_ant_tuple = extract_holog_params["ref_ant_per_map_ant_tuple"]
     map_ant_tuple = extract_holog_params["map_ant_tuple"]
-    holog_scan_id = extract_holog_params["holog_scan_id"]
+    ref_ant_per_map_ant_name_tuple = extract_holog_params["ref_ant_per_map_ant_name_tuple"]
+    map_ant_name_tuple = extract_holog_params["map_ant_name_tuple"]
+    
+    holog_map_key = extract_holog_params["holog_map_key"]
     telescope_name = extract_holog_params["telescope_name"]
     
     assert len(ref_ant_per_map_ant_tuple) == len(map_ant_tuple), "ref_ant_per_map_ant_tuple and map_ant_tuple should have same length."
     
     sel_state_ids = extract_holog_params["sel_state_ids"]
     holog_name = extract_holog_params["holog_name"]
     overwrite = extract_holog_params["overwrite"]
 
     chan_freq = extract_holog_params["chan_setup"]["chan_freq"]
     pol = extract_holog_params["pol_setup"]["pol"]
+    
+    table_obj = ctables.table(ms_name, readonly=True, lockoptions={'option': 'usernoread'}, ack=False)
 
     if sel_state_ids:    
         ctb = ctables.taql(
-            "select %s, ANTENNA1, ANTENNA2, TIME, TIME_CENTROID, WEIGHT, FLAG_ROW, FLAG from %s WHERE DATA_DESC_ID == %s AND SCAN_NUMBER in %s AND STATE_ID in %s"
-            % (data_col, ms_name, ddi, scans, sel_state_ids)
+            "select %s, ANTENNA1, ANTENNA2, TIME, TIME_CENTROID, WEIGHT, FLAG_ROW, FLAG from $table_obj WHERE DATA_DESC_ID == %s AND SCAN_NUMBER in %s AND STATE_ID in %s"
+            % (data_col, ddi, list(scans), list(sel_state_ids))
         )
     else:
         ctb = ctables.taql(
-            "select %s, ANTENNA1, ANTENNA2, TIME, TIME_CENTROID, WEIGHT, FLAG_ROW, FLAG from %s WHERE DATA_DESC_ID == %s AND SCAN_NUMBER in %s"
-            % (data_col, ms_name, ddi, scans)
+            "select %s, ANTENNA1, ANTENNA2, TIME, TIME_CENTROID, WEIGHT, FLAG_ROW, FLAG from $table_obj WHERE DATA_DESC_ID == %s AND SCAN_NUMBER in %s"
+            % (data_col, ddi, list(scans))
         )
         
     vis_data = ctb.getcol(data_col)
     weight = ctb.getcol("WEIGHT")
     ant1 = ctb.getcol("ANTENNA1")
     ant2 = ctb.getcol("ANTENNA2")
     time_vis_row = ctb.getcol("TIME")
     time_vis_row_centroid = ctb.getcol("TIME_CENTROID")
     flag = ctb.getcol("FLAG")
     flag_row = ctb.getcol("FLAG_ROW")
     ctb.close()
+    table_obj.close()
     
     time_vis, unique_index = np.unique(
         time_vis_row, return_index=True
     )  # Note that values are sorted.
     
+    #print(vis_data.shape,weight.shape,ant1.shape,ant2.shape,time_vis_row.shape,time_vis.shape,flag.shape,flag_row.shape,ref_ant_per_map_ant_tuple,map_ant_tuple,)
+    
     vis_map_dict, weight_map_dict, flagged_mapping_antennas = _extract_holog_chunk_jit(
         vis_data,
         weight,
         ant1,
         ant2,
         time_vis_row,
         time_vis,
@@ -881,21 +919,21 @@
         flag_row,
         ref_ant_per_map_ant_tuple,
         map_ant_tuple,
     )
 
     del vis_data, weight, ant1, ant2, time_vis_row, flag, flag_row
 
-    map_ant_list = list(map(str, map_ant_tuple))
+    map_ant_name_list = list(map(str, map_ant_name_tuple))
 
-    map_ant_list = ['ant_' + i for i in map_ant_list]
+    map_ant_name_list = ['ant_' + i for i in map_ant_name_list]
 
-    pnt_ant_dict = _load_pnt_dict(pnt_name, map_ant_list, dask_load=False)
+    pnt_ant_dict = _load_pnt_dict(pnt_name, map_ant_name_list, dask_load=False)
 
-    pnt_map_dict = _extract_pointing_chunk(map_ant_list, time_vis, pnt_ant_dict)
+    pnt_map_dict = _extract_pointing_chunk(map_ant_name_list, time_vis, pnt_ant_dict)
     
     ''' Removing for now. Code struggles with VLA pointing errors
     ################### Average multiple repeated samples
     if telescope_name != "ALMA":
         over_flow_protector_constant = float("%.5g" % time_vis[0])  # For example 5076846059.4 -> 5076800000.0
         time_vis = time_vis - over_flow_protector_constant
 
@@ -911,24 +949,24 @@
         vis_map_dict,
         weight_map_dict,
         pnt_map_dict,
         time_vis,
         chan_freq,
         pol,
         flagged_mapping_antennas,
-        holog_scan_id,
+        holog_map_key,
         ddi,
         ms_name,
         ant_names,
         overwrite=overwrite,
     )
 
     logger.info(
-        "Finished extracting holography chunk for ddi: {ddi} holog_scan_id: {holog_scan_id}".format(
-            ddi=ddi, holog_scan_id=holog_scan_id
+        "Finished extracting holography chunk for ddi: {ddi} holog_map_key: {holog_map_key}".format(
+            ddi=ddi, holog_map_key=holog_map_key
         )
     )
 
 def _get_attrs(zarr_obj):
     """Get attributes of zarr obj (groups or arrays)
 
     Args:
```

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.0.5/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         return logging.getLogger()
 
 def _setup_astrohack_logger(log_to_term=False,log_to_file=True,log_file='astrohack_', log_level='INFO', name=hack_logger_name):
     """To setup as many loggers as you want"""
     logger = logging.getLogger(name)
     logger.setLevel(logging.getLevelName(log_level))
     
+    logger.handlers.clear()
+    
     if log_to_term:
         handler = logging.StreamHandler(sys.stdout)
         handler.setFormatter(astrohack_formatter())
         logger.addHandler(handler)
     
     if log_to_file:
         log_file = log_file+datetime.today().strftime('%Y%m%d_%H%M%S')+'.log'
```

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_panel.py` & `astrohack-0.0.5/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.0.5/src/astrohack/_utils/gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/astrohack_client.py` & `astrohack-0.0.5/src/astrohack/astrohack_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     '''
     # setup dask.distributed based multiprocessing environment
     if cores is None: cores = multiprocessing.cpu_count()
     if memory_limit is None: memory_limit = str(round(((psutil.virtual_memory().available / (1024 ** 2))) / cores)) + 'MB'
     
     #print('cores',cores,memory_limit)
     
-    cluster = dask.distributed.LocalCluster(n_workers=cores, threads_per_worker=1, processes=True, memory_limit=memory_limit) #, silence_logs=logging.ERROR #,resources={'GPU': 2}
+    cluster = dask.distributed.LocalCluster(n_workers=cores, threads_per_worker=1, processes=True, memory_limit=memory_limit,silence_logs=logging.ERROR) #, silence_logs=logging.ERROR #,resources={'GPU': 2}
     client = dask.distributed.Client(cluster)
     client.get_versions(check=True)
     
     #print(client)
 
     '''
     When constructing a graph that has local cache enabled all workers need to be up and running.
```

### Comparing `astrohack-0.0.3/src/astrohack/dio.py` & `astrohack-0.0.5/src/astrohack/_utils/_dio_classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import xarray as xr
 import numpy as np
 
 from casacore import tables as ctables
 
 from prettytable import PrettyTable
 
-from astrohack._utils import _system_message as console
+from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 from astrohack._utils._holog import _create_holog_meta_data 
 
 from astrohack._utils._io import _load_pnt_dict 
 from astrohack._utils._io import _extract_holog_chunk
 from astrohack._utils._io import _open_no_dask_zarr
 from astrohack._utils._io import _read_data_from_holog_json
@@ -33,35 +33,36 @@
         self.holog = None
         self.image = None
             
         self._verify_holog_files(file_stem, path)
             
 
     def _verify_holog_files(self, file_stem, path):
-        console.info("Verifying {stem}.* files in path={path} ...".format(stem=file_stem, path=path))
+        logger = _get_astrohack_logger()
+        logger.info("Verifying {stem}.* files in path={path} ...".format(stem=file_stem, path=path))
 
         file_path = "{path}/{stem}.holog.zarr".format(path=path, stem=file_stem)
             
         if os.path.isdir(file_path):
-            console.info("Found {stem}.holog.zarr directory ...".format(stem=file_stem))
+            logger.info("Found {stem}.holog.zarr directory ...".format(stem=file_stem))
             self._holog_path = file_path
             self.holog = AstrohackHologFile(file_path)
                 
 
         file_path = "{path}/{stem}.image.zarr".format(path=path, stem=file_stem)
 
         if os.path.isdir(file_path):
-            console.info("Found {stem}.image.zarr directory ...".format(stem=file_stem))
+            logger.info("Found {stem}.image.zarr directory ...".format(stem=file_stem))
             self._image_path = file_path
             self.image = AstrohackImageFile(file_path)
 
         file_path = "{path}/{stem}.panel.zarr".format(path=path, stem=file_stem)
 
         if os.path.isdir(file_path):
-            console.info("Found {stem}.panel.zarr directory ...".format(stem=file_stem))
+            logger.info("Found {stem}.panel.zarr directory ...".format(stem=file_stem))
             self._image_path = file_path
             self.panel = AstrohackPanelFile(file_path)
 
 class AstrohackImageFile(dict):
     """
         Data class for holography image data.
     """
@@ -85,56 +86,58 @@
 
         Args:self =_
             file (str, optional): Path to holography file. Defaults to None.
 
         Returns:
             bool: bool describing whether the file was opened properly
         """
-
+        logger = _get_astrohack_logger()
         if file is None:
             file = self.file
         
         try:
             _load_image_file(file, image_dict=self)
 
             self._open = True
 
         except Exception as e:
-            console.error("[AstroHackImageFile.open()]: {}".format(e))
+            logger.error("[AstroHackImageFile.open()]: {}".format(e))
             self._open = False
 
         return self._open
 
     def summary(self):
         """
            Prints summary table of holog image file. 
         """
 
         table = PrettyTable()
         table.field_names = ["antenna", "ddi"]
         table.align = "l"
         
         for ant in self.keys():
-            table.add_row([ant, list(self[int(ant)].keys())])
+            table.add_row([ant, list(self[ant].keys())])
         
         print(table)
 
 
     def select(self, ant=None, ddi=None, polar=False):
         """Select data on the basis of ddi, scan, ant. This is a convenience function.
 
         Args:
             ddi (int, optional): Data description ID. Defaults to None.
             ant (int, optional): Antenna ID. Defaults to None.
 
         Returns:
             xarray.Dataset: xarray dataset of corresponding ddi, scan, antenna ID.
         """
+        logger = _get_astrohack_logger()
+        
         if ant is None and ddi is None:
-            console.info("No selections made ...")
+            logger.info("No selections made ...")
             return self
         else:
             if polar:
                 return self[ant][ddi].apply(np.absolute), self[ant][ddi].apply(np.angle, deg=True)
 
             return self[ant][ddi]
 
@@ -165,26 +168,27 @@
         Args:self =_
             file (str, optional): Path to holography file. Defaults to None.
             dask_load (bool, optional): If True the file is loaded with Dask. Defaults to False.
 
         Returns:
             bool: bool describing whether the file was opened properly
         """
+        logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
 
         self._meta_data = _read_meta_data(holog_file=file)
 
         try:
             _load_holog_file(holog_file=file, dask_load=dask_load, load_pnt_dict=False, holog_dict=self)
             self._open = True
 
         except Exception as e:
-            console.error("[AstrohackHologFile]: {}".format(e))
+            logger.error("[AstrohackHologFile]: {}".format(e))
             self._open = False
         
         return self._open
 
     def summary(self):
         """
             Prints summary table of holog file.
@@ -207,16 +211,18 @@
             ddi (int, optional): Data description ID. Defaults to None.
             scan (int, optional): Scan number. Defaults to None.
             ant (int, optional): Antenna ID. Defaults to None.
 
         Returns:
             xarray.Dataset: xarray dataset of corresponding ddi, scan, antenna ID.
         """
+        logger = _get_astrohack_logger()
+        
         if ant is None or ddi is None or scan is None:
-            console.info("No selections made ...")
+            logger.info("No selections made ...")
             return self
         else:
             return self[ddi][scan][ant]
 
     @property
     def meta_data(self):
         """ Holog file meta data.
@@ -251,35 +257,36 @@
 
         Args:self =_
             file (str, optional): Path to holography file. Defaults to None.
 
         Returns:
             bool: bool describing whether the file was opened properly
         """
+        logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
         
         try:
             _load_panel_file(file, panel_dict=self)
 
             self._open = True
 
         except Exception as e:
-            console.error("[AstroHackPanelFile.open()]: {}".format(e))
+            logger.error("[AstroHackPanelFile.open()]: {}".format(e))
             self._open = False
 
         return self._open
 
-#    def summary(self):
-#        """
-#           Prints summary table of panel image file. 
-#        """
-
-#        table = PrettyTable()
-#        table.field_names = ["antenna", "ddi"]
-#        table.align = "l"
+    def summary(self):
+        """
+           Prints summary table of panel image file.
+        """
+
+        table = PrettyTable()
+        table.field_names = ["antenna", "ddi"]
+        table.align = "l"
         
-#        for ant in self.keys():
-#            table.add_row([ant, list(self[int(ant)].keys())])
+        for ant in self.keys():
+            table.add_row([ant, list(self[ant].keys())])
         
-#        print(table)
+        print(table)
```

### Comparing `astrohack-0.0.3/src/astrohack/extract_holog.py` & `astrohack-0.0.5/src/astrohack/extract_holog.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,63 +17,98 @@
 from astrohack._utils._io import _load_pnt_dict 
 from astrohack._utils._io import _extract_holog_chunk 
 from astrohack._utils._io import _open_no_dask_zarr
 from astrohack._utils._io import _read_data_from_holog_json
 from astrohack._utils._io import _read_meta_data
 from astrohack._utils._io import _load_holog_file
 from astrohack._utils._io import  check_if_file_will_be_overwritten,check_if_file_exists
-#from memory_profiler import profile
-
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from  astrohack._utils._parm_utils._check_parms import _check_parm
+from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
+from astrohack._utils._io import _load_holog_file
 
 
-#@profile(stream=fp)
+from astrohack._utils._dio_classes import AstrohackHologFile
 def extract_holog(
     ms_name,
     holog_obs_dict,
     holog_name=None,
     point_name=None,
     data_col="DATA",
     parallel=False,
     overwrite=False,
 ):
     """
-    From a measurement set with holography data extract the pointing information (saved into a folder with a .point.zarr extension) and holography data (saved into a folder with an extension .holog.zarr).
+    Extract holography and optionally pointing data, from measurement set. Creates holography output file.
+
+    :param ms_name: Name of input measurement file name.
+    :type ms_name: str
+
+    :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set.
+    :type holog_obs_dict: dict        
+
+    :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
+    :type holog_name: str, optional
+
+    :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
+    :type point_name: str, optional
+
+    :param data_col: Determines the data column to pull from the measurement set. Defaults to "DATA"
+    :type data_col: str, optional
+
+    :param parallel: Boolean for whether to process in parallel. Defaults to False
+    :type parallel: bool, optional
+
+    :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files., defaults to False
+    :type overwrite: bool, optional
+
+    .. _Description:
+
+    **Additional Information**
+
+        This function extracts the holography related information from the given measurement file. The data is restructured into an astrohack file format and saved into a file in the form of *<holog_name>.holog.zarr*. The extension *.holog.zarr* is used for all holography files. In addition, the pointing information is recorded into a holography file of format *<pointing_name>.point.zarr*. The extension *.point.zarr* is used for all holography pointing files. 
+
+        **holog_obs_dict[holog_mapping_id] (dict):**
+        *holog_mapping_id* is a unique, arbitrary, user-defined integer assigned to the data that describes a single complete mapping of the beam.
+        
+        .. rubric:: This is needed for two reasons:
+        * A complete mapping of the beam can be done over more than one scan (for example the VLA data). 
+        * A measurement set can contain more than one mapping of the beam (for example the ALMA data).
+    
+        **holog_obs_dict[holog_mapping_id][scans] (int | numpy.ndarray | list):**
+        All the scans in the measurement set the *holog_mapping_id*.
+    
+        **holog_obs_dict[holog_mapping_id][ant] (dict):**
+        The dictionary keys are the mapping antenna names and the values a list of the reference antennas. See example below.
+    
+        **holog_obs_dict[ddi] (int | numpy.ndarray | list):**
+        Value(s) of DDI that should be extracted from the measurement set.
+
+        The below example shows how the *holog_obs_description* dictionary should be laid out. For each *holog_mapping_id* the relevant scans 
+        and antennas must be provided. For the `ant` key, an entry is required for each mapping antenna and the accompanying reference antenna(s).
+    
+        .. parsed-literal::
+            holog_obs_description = {
+                'map_0' :{
+                    'scans':[2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22],
+                    'ant':{
+                        'DA44':[
+                            'DV02', 'DV03', 'DV04', 
+                            'DV11', 'DV12', 'DV13', 
+                            'DV14', 'DV15', 'DV16', 
+                            'DV17', 'DV18', 'DV19', 
+                            'DV20', 'DV21', 'DV22', 
+                            'DV23', 'DV24', 'DV25'
+                        ]
+                    }
+                }
+            }
+            holog_obs_description['ddi'] = [0]
 
-    Parameters
-    ----------
-    ms_name (string):
-        Measurement file name.
-    holog_obs_dict (dict):
-        The holog_obs_dict describes which scans and antennas's data to exstract from the ms.
-        For example:
-        scans=[8,9,10,12,13,14,16,17,18,23,24,25,27,28,29,31,32,33,38,39,40,42,43,44,46,47,48,53,54,55,57]
-        holog_obs_description = {0 :{'scans':scans,'ant':{'ea25':['ea04']}}}
-        holog_obs_description['ddi'] = [0]
-    holog_obs_dict[holog_mapping_id] (dict):
-        A dictionary where each key is a holog_mapping_id. The holog_mapping_ids can be any numbers chosen arbiterily and represent one complete mapping of the beam. The holog_mapping_id is needed since the mapping of a beam can take more than one scan and an ms can have more than one mapping of the beam.
-    holog_obs_dict[holog_mapping_id]['scans'] (int np.ndarray/list):
-        All the scans in the ms that form part of the holog_mapping_id.
-    holog_obs_dict[holog_mapping_id]['ant'] (dict):
-        The keys are the mapping antenna names and the values lists of the reference antennas.
-    holog_obs_dict[ddi] (int np.ndarray/list):
-        All the ddi's in the ms from which data should be exstracted.
-    holog_name (string, default= ms name with holog.zarr extension):
-        Name of holog.zarr file to create.
-    point_name (string, default= ms name with point.zarr extension):
-        Name of point.zarr file to create.
-    data_col (str, default='DATA'):
-        Data column from measurement set to acquire.
-    parallel (bool, default=False):
-        Boolean for whether to process in parallel. If parallel processing is
-    overwrite (bool, optional):
-        Boolean for whether to overwrite current holog.zarr and point.zarr files.
     """
     logger = _get_astrohack_logger()
     
     
     extract_holog_parms = _check_extract_holog_parms(ms_name,
                                 holog_obs_dict,
                                 holog_name,
@@ -83,17 +118,17 @@
                                 overwrite)
     
     check_if_file_exists(extract_holog_parms['ms_name'])
     check_if_file_will_be_overwritten(extract_holog_parms['holog_name'],extract_holog_parms['overwrite'])
     check_if_file_will_be_overwritten(extract_holog_parms['point_name'],extract_holog_parms['overwrite'])
 
 #    try:
-#        pnt_dict = _load_pnt_dict(point_name)
+#        pnt_dict = _load_pnt_dict(extract_holog_parms['point_name'])
 #    except:
-#        pnt_dict = _make_ant_pnt_dict(ms_name, point_name, parallel=parallel)
+#        pnt_dict = _make_ant_pnt_dict(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
     
     pnt_dict = _make_ant_pnt_dict(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
 
     ''' VLA datasets causeing issues.
     if holog_obs_dict is None:
         ant_names_list = []
         #Create mapping antennas
@@ -193,129 +228,147 @@
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
     
     telescope_name = obs_ctb.getcol("TELESCOPE_NAME")[0]
 
-    extract_holog_params = {}
-
     ## DDI selection
     if holog_obs_dict['ddi'] is None:
         logger.error("No DDIs in holog_obs_dict.")
         raise Exception()
 
     delayed_list = []
     
     for ddi in holog_obs_dict['ddi']:
         spw_setup_id = ddi_spw[ddi]
         pol_setup_id = ddpol_indexol[ddi]
         
-        extract_holog_params["ddi"] = ddi
-        extract_holog_params["chan_setup"] = {}
-        extract_holog_params["pol_setup"] = {}
+        extract_holog_parms["ddi"] = ddi
+        extract_holog_parms["chan_setup"] = {}
+        extract_holog_parms["pol_setup"] = {}
         
-        extract_holog_params["chan_setup"]["chan_freq"] = spw_ctb.getcol("CHAN_FREQ", startrow=spw_setup_id, nrow=1)[0, :]
-        extract_holog_params["chan_setup"]["chan_width"] = spw_ctb.getcol("CHAN_WIDTH", startrow=spw_setup_id, nrow=1)[0, :]
-        extract_holog_params["chan_setup"]["eff_bw"] = spw_ctb.getcol("EFFECTIVE_BW", startrow=spw_setup_id, nrow=1)[0, :]
-        extract_holog_params["chan_setup"]["ref_freq"] = spw_ctb.getcol("REF_FREQUENCY", startrow=spw_setup_id, nrow=1)[0]
-        extract_holog_params["chan_setup"]["total_bw"] = spw_ctb.getcol("TOTAL_BANDWIDTH", startrow=spw_setup_id, nrow=1)[0]
+        extract_holog_parms["chan_setup"]["chan_freq"] = spw_ctb.getcol("CHAN_FREQ", startrow=spw_setup_id, nrow=1)[0, :]
+        extract_holog_parms["chan_setup"]["chan_width"] = spw_ctb.getcol("CHAN_WIDTH", startrow=spw_setup_id, nrow=1)[0, :]
+        extract_holog_parms["chan_setup"]["eff_bw"] = spw_ctb.getcol("EFFECTIVE_BW", startrow=spw_setup_id, nrow=1)[0, :]
+        extract_holog_parms["chan_setup"]["ref_freq"] = spw_ctb.getcol("REF_FREQUENCY", startrow=spw_setup_id, nrow=1)[0]
+        extract_holog_parms["chan_setup"]["total_bw"] = spw_ctb.getcol("TOTAL_BANDWIDTH", startrow=spw_setup_id, nrow=1)[0]
 
-        extract_holog_params["pol_setup"]["pol"] = pol_str[pol_ctb.getcol("CORR_TYPE", startrow=pol_setup_id, nrow=1)[0, :]]
+        extract_holog_parms["pol_setup"]["pol"] = pol_str[pol_ctb.getcol("CORR_TYPE", startrow=pol_setup_id, nrow=1)[0, :]]
                 
         
-        extract_holog_params["telescope_name"] = obs_ctb.getcol("TELESCOPE_NAME")[0]
+        extract_holog_parms["telescope_name"] = obs_ctb.getcol("TELESCOPE_NAME")[0]
         
 
-        for holog_scan_id in holog_obs_dict.keys(): #loop over all beam_scan_ids, a beam_scan_id can conist out of more than one scan in an ms (this is the case for the VLA pointed mosiacs).
-            if isinstance(holog_scan_id,int):
-                scans = holog_obs_dict[holog_scan_id]["scans"]
+        for holog_map_key in holog_obs_dict.keys(): #loop over all beam_scan_ids, a beam_scan_id can conist out of more than one scan in an ms (this is the case for the VLA pointed mosiacs).
+            #if isinstance(holog_map_key,int):
+            if 'map' in holog_map_key:
+                scans = holog_obs_dict[holog_map_key]["scans"]
                 logger.info("Processing ddi: {ddi}, scans: {scans}".format(ddi=ddi, scans=scans))
             
                 map_ant_list = []
                 ref_ant_per_map_ant_list = [] #
-                for map_ant_str in holog_obs_dict[holog_scan_id]['ant'].keys():
-                    ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names,list(holog_obs_dict[holog_scan_id]['ant'][map_ant_str])))
+                
+                map_ant_name_list = []
+                ref_ant_per_map_ant_name_list = [] #
+                for map_ant_str in holog_obs_dict[holog_map_key]['ant'].keys():
+                    ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names,list(holog_obs_dict[holog_map_key]['ant'][map_ant_str])))
                     map_ant_id = _convert_ant_name_to_id(ant_names,map_ant_str)[0]
 
                     ref_ant_per_map_ant_list.append(ref_ant_ids)
                     map_ant_list.append(map_ant_id)
                     
-                extract_holog_params["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
-                extract_holog_params["map_ant_tuple"] = tuple(map_ant_list)
-                extract_holog_params["scans"] = scans
-                extract_holog_params["sel_state_ids"] = state_ids
-                extract_holog_params["holog_scan_id"] = holog_scan_id
-                extract_holog_params["ant_names"] = ant_names
+                    ref_ant_per_map_ant_name_list.append(list(holog_obs_dict[holog_map_key]['ant'][map_ant_str]))
+                    map_ant_name_list.append(map_ant_str) #
+                    
+                    
+                    
+                extract_holog_parms["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
+                extract_holog_parms["map_ant_tuple"] = tuple(map_ant_list)
+                
+                extract_holog_parms["ref_ant_per_map_ant_name_tuple"] = tuple(ref_ant_per_map_ant_name_list)
+                extract_holog_parms["map_ant_name_tuple"] = tuple(map_ant_name_list)
+                
+                extract_holog_parms["scans"] = scans
+                extract_holog_parms["sel_state_ids"] = state_ids
+                extract_holog_parms["holog_map_key"] = holog_map_key
+                extract_holog_parms["ant_names"] = ant_names
                 
                 if parallel:
                     delayed_list.append(
                         dask.delayed(_extract_holog_chunk)(
-                            dask.delayed(extract_holog_params)
+                            dask.delayed(extract_holog_parms)
                         )
                     )
                 else:
-                    _extract_holog_chunk(extract_holog_params)
+                    _extract_holog_chunk(extract_holog_parms)
 
     spw_ctb.close()
     pol_ctb.close()
 
     if parallel:
         dask.compute(delayed_list)    
 
-    extract_holog_params["holog_obs_dict"] = {}
+    extract_holog_parms["holog_obs_dict"] = {}
 
     for id in ant_id:
-        extract_holog_params["holog_obs_dict"][str(id)] = ant_names[id]
+        extract_holog_parms["holog_obs_dict"][str(id)] = ant_names[id]
 
-    holog_dict = _load_holog_file(holog_file=holog_name, dask_load=True, load_pnt_dict=False)
+    holog_dict = _load_holog_file(holog_file=extract_holog_parms["holog_name"], dask_load=True, load_pnt_dict=False)
 
-    _create_holog_meta_data(holog_file=holog_name, holog_dict=holog_dict, holog_params=extract_holog_params)
+    _create_holog_meta_data(holog_file=extract_holog_parms['holog_name'], holog_dict=holog_dict, holog_params=extract_holog_parms)
+    
+    holog_mds = AstrohackHologFile(extract_holog_parms['holog_name'])
+    holog_mds.open()
+    
+    return holog_mds
+    
 
 
 def _check_extract_holog_parms(    ms_name,
     holog_obs_dict,
     holog_name,
     point_name,
     data_col,
     parallel,
     overwrite):
     
-    extract_holog_params = {}
-    extract_holog_params["ms_name"] = ms_name
-    extract_holog_params["holog_name"] = holog_name
-    extract_holog_params["point_name"] = point_name
-    extract_holog_params["parallel"] = parallel
-    extract_holog_params["overwrite"] = overwrite
+    extract_holog_parms = {}
+    extract_holog_parms["ms_name"] = ms_name
+    extract_holog_parms["holog_name"] = holog_name
+    extract_holog_parms["point_name"] = point_name
+    extract_holog_parms["data_col"] = data_col
+    extract_holog_parms["parallel"] = parallel
+    extract_holog_parms["overwrite"] = overwrite
 
     
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
-    parms_passed = parms_passed and _check_parms(extract_holog_params, 'ms_name', [str],default=None)
+    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'ms_name', [str],default=None)
 
     base_name = _remove_suffix(ms_name,'.ms')
-    parms_passed = parms_passed and _check_parms(extract_holog_params,'holog_name', [str],default=base_name+'.holog.zarr')
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'holog_name', [str],default=base_name+'.holog.zarr')
   
     
-    point_base_name = _remove_suffix(holog_name,'.holog.zarr')
-    parms_passed = parms_passed and _check_parms(extract_holog_params,'point_name', [str],default=point_base_name+'.point.zarr')
+    point_base_name = _remove_suffix(extract_holog_parms['holog_name'],'.holog.zarr')
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'point_name', [str],default=point_base_name+'.point.zarr')
   
     #To Do: special function needed to check holog_obs_dict.
     parm_check = isinstance(holog_obs_dict,dict)
     parms_passed = parms_passed and parm_check
     if not parm_check:
         logger.error('Parameter holog_obs_dict must be of type '+ str(dict))
         
-    parms_passed = parms_passed and _check_parms(extract_holog_params,'data_col', [str],default='DATA')
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'data_col', [str],default='DATA')
 
-    parms_passed = parms_passed and _check_parms(extract_holog_params, 'parallel', [bool],default=False)
+    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'parallel', [bool],default=False)
 
-    parms_passed = parms_passed and _check_parms(extract_holog_params, 'overwrite', [bool],default=False)
+    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'overwrite', [bool],default=False)
 
     if not parms_passed:
         logger.error("extract_holog parameter checking failed.")
         raise Exception("extract_holog parameter checking failed.")
     
     
-    return extract_holog_params
+    return extract_holog_parms
```

### Comparing `astrohack-0.0.3/src/astrohack/holog.py` & `astrohack-0.0.5/src/astrohack/holog.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,75 +4,134 @@
 import dask
 import dask.distributed
 import numpy as np
 import numbers
 
 from astrohack._utils._holog import _holog_chunk
 
-from memory_profiler import profile
-
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from  astrohack._utils._parm_utils._check_parms import _check_parms
+from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
    
-from astrohack._utils._io import  check_if_file_will_be_overwritten,check_if_file_exists
+from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists
+from astrohack._utils._dio_classes import AstrohackImageFile
 
 #fp=open('holog.log','w+')
 #@profile(stream=fp)
 def holog(
     holog_name,
     grid_size,
     cell_size,
     image_name=None,
     padding_factor=50,
-    parallel=True,
     grid_interpolation_mode="nearest",
     chan_average=True,
     chan_tolerance_factor=0.005,
     reference_scaling_frequency=None,
-    scan_average = True,
-    ant_list = None,
-    to_stokes = True,
+    scan_average=True,
+    ant_list=None,
+    to_stokes=True,
     apply_mask=True,
     phase_fit=True,
-    overwrite=False):
-    """
-    Process holography data
+    overwrite=False,
+    parallel=True):
+    """ Process holography data and derive aperture illumination pattern.
+
+    :param holog_name: Name of holography .holog.zarr file to process.
+    :type holog_name: str
+
+    :param grid_size: Numpy array specifying the dimensions of the grid used in data gridding.
+    :type grid_size: numpy.ndarray, dtype int
+
+    :param cell_size: Numpy array defining the cell size of each grid bin.
+    :type cell_size: numpy.ndarray, dtype float
+
+    :param image_name: Defines the name of the output image name. If value is None, the name will be set to <base_name>.image.zarr, defaults to None
+    :type image_name: str, optional
+
+    :param padding_factor: Padding factor applied to beam grid before computing the fast-fourier transform. The default has been set for operation on most systems. The user should be aware of memory constraints before increasing this parameter significatly., defaults to 50
+    :type padding_factor: int, optional
+
+    :param parallel: Run in parallel with Dask or in serial., defaults to True
+    :type parallel: bool, optional
+
+    :param grid_interpolation_mode: Method of interpolation used when gridding data. This is done using the `scipy.interpolate.griddata` method. For more information on the interpolation see `scipy.interploate <https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.griddata.html#scipy.interpolate.griddata>`_, defaults to "nearest"
+    :type grid_interpolation_mode: str, optional
+
+    :param chan_average: Boolean dictating whether the channel average is computed and written to the output holog file., defaults to True
+    :type chan_average: bool, optional
+
+    :param chan_tolerance_factor: Tolerance used in channel averaging to determine the number of primary beam channels., defaults to 0.005
+    :type chan_tolerance_factor: float, optional
+
+    :param reference_scaling_frequency: When computing the channel average the lm frequency values are scaled by frequency. If the default None is used, the scaling is simply unity, however if `reference_scaling_frequency` is set then the scaling is done according to (average_frequency/reference_scaling_frequency)., defaults to None
+    :type reference_scaling_frequency: _type_, optional
+
+    :param scan_average: Boolean dicating whether averagin is done over scan., defaults to True
+    :type scan_average: bool, optional
+
+    :param ant_list: Optional list of sub-antennas to use when the user doesn't to do holography for all antennas, defaults to None
+    :type ant_list: list, optional
+
+    :param to_stokes: Dictates whether polarization is computed according to stokes values., defaults to True
+    :type to_stokes: bool, optional
+
+    :param apply_mask: If True applies a mask to the aperture setting values outside of the aperture to zero., defaults to True
+    :type apply_mask: bool, optional
 
-    Args:
-        holog_name (str): holog file name
-        parallel (bool, optional): Run in parallel with Dask or in serial. Defaults to True.
+    :param phase_fit: If a boolean array is given each element controls one aspect of phase fitting. defaults to True.
         
-        phase_fit (bool or bool np.ndarray 5x1): if a boolean array is given each element controls one aspect of
-        phase fitting: 0 -> pointing offset; 
-                       1 -> focus xy offsets; 
-                       2 -> focus z offset; 
-                       3 -> subreflector tilt; (This one is off by default except for VLA and VLBA)
-                       4 -> cassegrain offset
-         
-        cell_size: float np.ndarray 2x1
-        grid_size: int np.ndarray 2X1
+        Phase fitting:
+        
+        - [0]: pointing offset; 
+        - [1]: focus xy offsets; 
+        - [2]: focus z offset; 
+        - [3]: subreflector tilt (off by default except for VLA and VLBA)
+        - [4]: cassegrain offset
+
+    :type phase_fit: bool, optional
+
+    :param overwrite: Overwrite existing files on disk, defaults to False
+    :type overwrite: bool, optional
+
     """
     
     logger = _get_astrohack_logger()
     
-    holog_params = _check_holog_parms(holog_name,grid_size,cell_size,image_name,padding_factor,parallel,grid_interpolation_mode,chan_average,chan_tolerance_factor,reference_scaling_frequency,scan_average,ant_list,to_stokes,apply_mask,phase_fit,overwrite)
+    holog_params = _check_holog_parms(
+        holog_name, 
+        grid_size,
+        cell_size, 
+        image_name, 
+        padding_factor, 
+        parallel, 
+        grid_interpolation_mode, 
+        chan_average, 
+        chan_tolerance_factor, 
+        reference_scaling_frequency, 
+        scan_average,
+        ant_list, 
+        to_stokes, 
+        apply_mask, 
+        phase_fit,
+        overwrite
+    )
     
     check_if_file_exists(holog_params['holog_file'])
     check_if_file_will_be_overwritten(holog_params['image_file'],holog_params['overwrite'])
 
     json_data = "/".join((holog_params['holog_file'], ".holog_json"))
     meta_data = "/".join((holog_params['holog_file'], ".holog_attr"))
     
     with open(json_data, "r") as json_file:
         holog_json = json.load(json_file)
     
     with open(meta_data, "r") as meta_file:
         meta_data = json.load(meta_file)
-        
+        image_name=None,
 
     if  holog_params['ant_list'] == 'all':
         holog_params['ant_list'] = list(holog_json.keys())
         
     logger.info('Mapping antennas ' + str(holog_params['ant_list']))
 
     ''' VLA data sampling can be uneven so averging step in extracty_holog does not work consequntly int(np.sqrt(meta_data["n_time"])) is not correct.
@@ -99,31 +158,43 @@
         holog_chunk_params["grid_size"] = grid_size
 
         logger.info("Cell size: " + str(cell_size) + " Grid size " + str(grid_size))
     else:
         holog_chunk_params["cell_size"] = cell_size
         holog_chunk_params["grid_size"] = grid_size
     '''
+
+    
     holog_chunk_params =  holog_params
     delayed_list = []
-
+    
+    
     for ant_id in holog_chunk_params['ant_list']:
-        logger.info("Processing ant_id: " + str(ant_id))
-        holog_chunk_params["ant_id"] = ant_id
-
-        if parallel:
-            delayed_list.append(
-                dask.delayed(_holog_chunk)(dask.delayed(holog_chunk_params))
-            )
-
-        else:
-            _holog_chunk(holog_chunk_params)
+        for ddi in list(holog_json[ant_id].keys()):
+            logger.info("Processing ant_id: " + str(ant_id)  + " and " + ddi)
+            holog_chunk_params["ant_id"] = ant_id
+            holog_chunk_params["ddi_id"] = ddi
+            
+            if parallel:
+                delayed_list.append(
+                    dask.delayed(_holog_chunk)(dask.delayed(holog_chunk_params))
+                )
+
+            else:
+                _holog_chunk(holog_chunk_params)
+            
 
     if holog_chunk_params['parallel']:
         dask.compute(delayed_list)
+        
+    image_mds = AstrohackImageFile(holog_chunk_params['image_file'])
+    image_mds.open()
+    
+    return image_mds
+
 
 
 def _check_holog_parms(holog_name,grid_size,cell_size,image_name,
                       padding_factor,parallel,grid_interpolation_mode,
                       chan_average,chan_tolerance_factor,
                       reference_scaling_frequency,scan_average,
                       ant_list,to_stokes,apply_mask,phase_fit,overwrite):
```

### Comparing `astrohack-0.0.3/src/astrohack/profiling.py` & `astrohack-0.0.5/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack/visualization/viewer.py` & `astrohack-0.0.5/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.3/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.3
+Version: 0.0.5
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 # astroHACK
 
-[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+[![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
 
 # Installing
```

### Comparing `astrohack-0.0.3/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.0.5/src/astrohack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 README.rst
 pyproject.toml
 src/astrohack/__init__.py
 src/astrohack/astrohack_client.py
 src/astrohack/dio.py
 src/astrohack/extract_holog.py
+src/astrohack/gdown_utils.py
 src/astrohack/holog.py
 src/astrohack/locit.py
 src/astrohack/panel.py
 src/astrohack/profiling.py
 src/astrohack.egg-info/PKG-INFO
 src/astrohack.egg-info/SOURCES.txt
 src/astrohack.egg-info/dependency_links.txt
@@ -19,30 +20,26 @@
 src/astrohack/_classes/polygon_panel.py
 src/astrohack/_classes/ring_panel.py
 src/astrohack/_classes/telescope.py
 src/astrohack/_utils/__init__.py
 src/astrohack/_utils/_algorithms.py
 src/astrohack/_utils/_constants.py
 src/astrohack/_utils/_conversion.py
+src/astrohack/_utils/_dio_classes.py
 src/astrohack/_utils/_holog.py
 src/astrohack/_utils/_imaging.py
 src/astrohack/_utils/_io.py
 src/astrohack/_utils/_panel.py
-src/astrohack/_utils/_system_message.py
 src/astrohack/_utils/_utils.py
 src/astrohack/_utils/gaussfitter.py
 src/astrohack/_utils/_dask_plugins/__init__.py
 src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
 src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
 src/astrohack/_utils/_logger/__init__.py
 src/astrohack/_utils/_logger/_astrohack_logger.py
 src/astrohack/_utils/_parm_utils/__init__.py
 src/astrohack/_utils/_parm_utils/_check_logger_parms.py
 src/astrohack/_utils/_parm_utils/_check_parms.py
 src/astrohack/visualization/__init__.py
 src/astrohack/visualization/viewer.py
-tests/test_astrohack_dio.py
-tests/test_class_antenna_surface.py
 tests/test_class_base_panel.py
-tests/test_class_polygon_panel.py
-tests/test_class_ring_panel.py
-tests/test_class_telescope.py
+tests/test_class_ring_panel.py
```

### Comparing `astrohack-0.0.3/src/astrohack.egg-info/requires.txt` & `astrohack-0.0.5/src/astrohack.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pytest==7.2.2
 scikit_image==0.19.3
 scipy==1.7.3
 setuptools==65.6.3
 Shapely==2.0.1
 xarray==2022.12.0
 zarr==2.13.3
+bokeh==2.4.3
 jupyterlab
 
 [:sys_platform != "darwin"]
 python_casacore==3.5.2
 
 [docs]
 ipykernel
```

