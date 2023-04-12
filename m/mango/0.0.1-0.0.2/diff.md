# Comparing `tmp/mango-0.0.1.tar.gz` & `tmp/mango-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-0.0.1.tar", last modified: Thu Mar  9 16:24:23 2023, max compression
+gzip compressed data, was "mango-0.0.2.tar", last modified: Wed Apr 12 13:41:11 2023, max compression
```

## Comparing `mango-0.0.1.tar` & `mango-0.0.2.tar`

### file list

```diff
@@ -1,75 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.334149 mango-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-03-09 16:24:17.000000 mango-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-09 16:24:17.000000 mango-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-09 16:24:23.334149 mango-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-09 16:24:17.000000 mango-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.322149 mango-0.0.1/mango/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 16:24:17.000000 mango-0.0.1/mango/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.326149 mango-0.0.1/mango/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:17.000000 mango-0.0.1/mango/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-03-09 16:24:17.000000 mango-0.0.1/mango/clients/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-09 16:24:17.000000 mango-0.0.1/mango/clients/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-03-09 16:24:17.000000 mango-0.0.1/mango/clients/email_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-09 16:24:17.000000 mango-0.0.1/mango/clients/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-03-09 16:24:17.000000 mango-0.0.1/mango/clients/google_cloud_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.326149 mango-0.0.1/mango/config/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-09 16:24:17.000000 mango-0.0.1/mango/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-03-09 16:24:17.000000 mango-0.0.1/mango/config/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.326149 mango-0.0.1/mango/data/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-09 16:24:17.000000 mango-0.0.1/mango/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-03-09 16:24:17.000000 mango-0.0.1/mango/data/ts_dataset.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.326149 mango-0.0.1/mango/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:17.000000 mango-0.0.1/mango/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-03-09 16:24:17.000000 mango-0.0.1/mango/images/images_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.326149 mango-0.0.1/mango/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-09 16:24:17.000000 mango-0.0.1/mango/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-09 16:24:17.000000 mango-0.0.1/mango/logging/chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-09 16:24:17.000000 mango-0.0.1/mango/logging/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.330149 mango-0.0.1/mango/models/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-09 16:24:17.000000 mango-0.0.1/mango/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-09 16:24:17.000000 mango-0.0.1/mango/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-09 16:24:17.000000 mango-0.0.1/mango/models/neural_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.330149 mango-0.0.1/mango/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:17.000000 mango-0.0.1/mango/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-03-09 16:24:17.000000 mango-0.0.1/mango/plots/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.330149 mango-0.0.1/mango/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-09 16:24:17.000000 mango-0.0.1/mango/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-09 16:24:17.000000 mango-0.0.1/mango/processing/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-03-09 16:24:17.000000 mango-0.0.1/mango/processing/file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-03-09 16:24:17.000000 mango-0.0.1/mango/processing/object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-03-09 16:24:17.000000 mango-0.0.1/mango/processing/processing_time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.330149 mango-0.0.1/mango/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-09 16:24:17.000000 mango-0.0.1/mango/schemas/location.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.330149 mango-0.0.1/mango/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-09 16:24:17.000000 mango-0.0.1/mango/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-09 16:24:17.000000 mango-0.0.1/mango/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-09 16:24:17.000000 mango-0.0.1/mango/shared/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-09 16:24:17.000000 mango-0.0.1/mango/shared/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.334149 mango-0.0.1/mango/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.334149 mango-0.0.1/mango/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/data/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/data/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/data/test.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/data/test_bad_type.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/data/test_bad_value.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/data/test_good.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_arcgis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_processing_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-09 16:24:17.000000 mango-0.0.1/mango/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:24:23.322149 mango-0.0.1/mango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-09 16:24:22.000000 mango-0.0.1/mango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-09 16:24:23.000000 mango-0.0.1/mango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:24:22.000000 mango-0.0.1/mango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-09 16:24:22.000000 mango-0.0.1/mango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-09 16:24:22.000000 mango-0.0.1/mango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 16:24:23.338149 mango-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-09 16:24:17.000000 mango-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.225054 mango-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-12 13:41:07.000000 mango-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 13:41:07.000000 mango-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 13:41:11.225054 mango-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 13:41:07.000000 mango-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.205054 mango-0.0.2/mango/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 13:41:07.000000 mango-0.0.2/mango/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/email_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-12 13:41:07.000000 mango-0.0.2/mango/clients/google_cloud_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 13:41:07.000000 mango-0.0.2/mango/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-12 13:41:07.000000 mango-0.0.2/mango/config/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 13:41:07.000000 mango-0.0.2/mango/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-12 13:41:07.000000 mango-0.0.2/mango/data/ts_dataset.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.209054 mango-0.0.2/mango/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-12 13:41:07.000000 mango-0.0.2/mango/images/images_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.213054 mango-0.0.2/mango/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-12 13:41:07.000000 mango-0.0.2/mango/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.213054 mango-0.0.2/mango/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 13:41:07.000000 mango-0.0.2/mango/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 13:41:07.000000 mango-0.0.2/mango/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-12 13:41:07.000000 mango-0.0.2/mango/models/neural_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.213054 mango-0.0.2/mango/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 13:41:07.000000 mango-0.0.2/mango/plots/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-12 13:41:07.000000 mango-0.0.2/mango/processing/processing_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 13:41:07.000000 mango-0.0.2/mango/schemas/location.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 13:41:07.000000 mango-0.0.2/mango/shared/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.217054 mango-0.0.2/mango/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21180 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/pytups_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/pytups_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-12 13:41:07.000000 mango-0.0.2/mango/table/table_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.225054 mango-0.0.2/mango/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.225054 mango-0.0.2/mango/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/json_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test_bad_type.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test_bad_value.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/data/test_good.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_arcgis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_processing_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41638 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 13:41:07.000000 mango-0.0.2/mango/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:41:11.205054 mango-0.0.2/mango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 13:41:11.000000 mango-0.0.2/mango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:41:11.225054 mango-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-12 13:41:07.000000 mango-0.0.2/setup.py
```

### Comparing `mango-0.0.1/LICENSE` & `mango-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/PKG-INFO` & `mango-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
@@ -25,7 +25,8 @@
 Provides-Extra: data
 Provides-Extra: images
 Provides-Extra: logging
 Provides-Extra: model
 Provides-Extra: plot
 Provides-Extra: processing
 Provides-Extra: shared
+Provides-Extra: table
```

### Comparing `mango-0.0.1/mango/clients/email_downloader.py` & `mango-0.0.2/mango/clients/email_downloader.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/clients/email_sender.py` & `mango-0.0.2/mango/clients/email_sender.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/clients/google_cloud_storage.py` & `mango-0.0.2/mango/clients/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/config/base_config.py` & `mango-0.0.2/mango/config/base_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/data/ts_dataset.pkl` & `mango-0.0.2/mango/data/ts_dataset.pkl`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/images/images_functions.py` & `mango-0.0.2/mango/images/images_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/logging/chrono.py` & `mango-0.0.2/mango/logging/chrono.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 import time
-import logging
-
-logger = logging.getLogger("root")
+from .logger import get_basic_logger
 
 
 class Chrono:
     """
     Class to measure time
     """
 
-    def __init__(self, name: str, silent: bool = False, precision: int = 2):
+    basic_logger = get_basic_logger()
+
+    def __init__(
+        self, name: str, silent: bool = False, precision: int = 2, logger=basic_logger
+    ):
         """
         Constructor of the class
 
         :param name: name of the chrono
         :param silent: if the chrono should be silent
         :param precision: number of decimals to round the time to
+        :param logger: logging logger object
         """
         self.silent = silent
         self.precision = precision
         self.start_time = {name: time.time()}
         self.end = {name: None}
+        self.logger = logger
 
     def new(self, name: str):
         """
         Method to create a new chrono
 
         :param name: name of the chrono
         """
         self.start_time[name] = None
         self.end[name] = None
 
-    def start(self, name):
+    def start(self, name, silent=True):
         """
         Method to start a chrono
 
         :param name: name of the chrono
         """
         self.new(name)
         self.start_time[name] = time.time()
+        if not silent:
+            self.logger.info(f"Operation {name} starts")
 
     def stop(self, name: str):
         """
         Method to stop a chrono and get back its duration
 
         :param name: name of the chrono
         :return: the time elapsed for the specific chrono
         :rtype: float
         """
         self.end[name] = time.time()
         duration = self.end[name] - self.start_time[name]
         if not self.silent:
-            logger.info(
+            self.logger.info(
                 f"Operation {name} took: {round(duration, self.precision)} seconds"
             )
         return duration
 
     def stop_all(self):
         """
         Method to stop all chronos and get back a dict with their durations
@@ -75,27 +81,27 @@
         """
 
         if self.end[name] is not None:
             msg = f"Operation {name} took: {round(self.end[name] - self.start_time[name], self.precision)} seconds"
             if message is not None:
                 msg = f"{msg}. {message}"
 
-            logger.info(msg)
+            self.logger.info(msg)
 
             return self.end[name] - self.start_time[name]
         else:
             duration = time.time() - self.start_time[name]
             msg = (
                 f"Operation {name} is still running. "
                 f"Time elapsed: {round(duration, self.precision)} seconds"
             )
             if message is not None:
                 msg = f"{msg}. {message}"
 
-            logger.info(msg)
+            self.logger.info(msg)
 
             return duration
 
     def report_all(self):
         """
         Method to report the time of all chronos and get back a dict with all the durations
         """
```

### Comparing `mango-0.0.1/mango/logging/decorators.py` & `mango-0.0.2/mango/logging/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/models/neural_networks.py` & `mango-0.0.2/mango/models/neural_networks.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/plots/plots.py` & `mango-0.0.2/mango/plots/plots.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/processing/__init__.py` & `mango-0.0.2/mango/processing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,13 +22,14 @@
     cumsum,
     lag_list,
     lead_list,
     row_number,
     flatten,
     df_to_list,
     df_to_dict,
+    as_list
 )
 from .processing_time_series import (
     create_dense_data,
     create_lags_col,
     create_recurrent_dataset,
 )
```

### Comparing `mango-0.0.1/mango/processing/date_functions.py` & `mango-0.0.2/mango/processing/date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/processing/file_functions.py` & `mango-0.0.2/mango/processing/file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/processing/object_functions.py` & `mango-0.0.2/mango/processing/object_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     """
     The flatten function takes a list of lists and returns a flattened list.
 
     :param lst: the list of lists to be flattened
     :return: a flattened list
     :doc-author: baobab soluciones
     """
-    return [item for sublist in lst for item in sublist]
+    return [item for sublist in lst for item in as_list(sublist)]
 
 
 def df_to_list(df: pandas.DataFrame) -> list:
     """
     The data_frame_to_list function takes a DataFrame and returns a list of dictionaries with the
     column names as keys and the values as values.
```

### Comparing `mango-0.0.1/mango/processing/processing_time_series.py` & `mango-0.0.2/mango/processing/processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/shared/const.py` & `mango-0.0.2/mango/shared/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/shared/decorators.py` & `mango-0.0.2/mango/shared/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/const.py` & `mango-0.0.2/mango/tests/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/data/test.xlsx` & `mango-0.0.2/mango/tests/data/test.xlsx`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_arcgis_client.py` & `mango-0.0.2/mango/tests/test_arcgis_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,45 +39,49 @@
         mock_requests.post.assert_called_once()
 
     @mock.patch("mango.clients.arcgis.requests")
     def test_get_geo_location(self, mock_requests):
         mock_requests.get.return_value.json.return_value = {
             "candidates": [{"location": {"x": 1, "y": 2}}]
         }
+        mock_requests.get.return_value.status_code = 200
         client = self.test_connect()
         result = client.get_geolocation("Some address somewhere")
         self.assertEqual(result, (1, 2))
         mock_requests.get.assert_called_once()
 
     @mock.patch("mango.clients.arcgis.requests")
     def test_geo_location_no_candidates(self, mock_requests):
         mock_requests.get.return_value.json.return_value = {"candidates": []}
+        mock_requests.get.return_value.status_code = 200
         client = self.test_connect()
         result = client.get_geolocation("Some address somewhere")
         self.assertEqual(result, (None, None))
         mock_requests.get.assert_called_once()
 
     @mock.patch("mango.clients.arcgis.requests")
     def test_geo_location_no_candidates_key(self, mock_requests):
         mock_requests.get.return_value.json.return_value = {}
+        mock_requests.get.return_value.status_code = 200
         client = self.test_connect()
         self.assertRaises(JobError, client.get_geolocation, "Some address somewhere")
         mock_requests.get.assert_called_once()
 
     @mock.patch("mango.clients.arcgis.requests")
     def test_geo_location_no_location_key(self, mock_requests):
         mock_requests.get.return_value.json.return_value = {
             "candidates": [{"other": 0}]
         }
+        mock_requests.get.return_value.status_code = 200
         client = self.test_connect()
         self.assertRaises(JobError, client.get_geolocation, "Some address somewhere")
         mock_requests.get.assert_called_once()
 
     @mock.patch("mango.clients.arcgis.requests")
-    def test_get_distances(self, mock_requests):
+    def test_get_distances_async(self, mock_requests):
         origins = [{"x": 1, "y": 1, "name": "First location"}]
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
 
         mock_requests.get.return_value.json.side_effect = [
             {"jobId": 100},
             {"jobStatus": "esriJobSucceeded"},
@@ -92,17 +96,18 @@
                                 "DestinationName": "Second location",
                             }
                         }
                     ]
                 }
             },
         ]
+        mock_requests.get.return_value.status_code = 200
 
         response = client.get_origin_destination_matrix(
-            origins=origins, destinations=destinations
+            mode="async", origins=origins, destinations=destinations
         )
 
         self.assertEqual(
             response,
             [
                 {
                     "origin": "First location",
@@ -111,111 +116,119 @@
                     "time": 100,
                 }
             ],
         )
 
         mock_requests.get.assert_called()
 
-    def test_too_many_origins(self):
+    def test_too_many_origins_async(self):
         origins = [{"x": 1, "y": 1, "name": "First location"}] * 1001
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
         self.assertRaises(
             NotImplementedError,
             client.get_origin_destination_matrix,
             origins=origins,
             destinations=destinations,
         )
 
     @mock.patch("mango.clients.arcgis.requests")
-    def test_job_failed(self, mock_requests):
+    def test_job_failed_async(self, mock_requests):
         origins = [{"x": 1, "y": 1, "name": "First location"}]
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
 
         mock_requests.get.return_value.json.side_effect = [
             {"jobId": 100},
             {"jobStatus": "esriJobFailed"},
             {"jobStatus": "esriJobFailed"},
         ]
+        mock_requests.get.return_value.status_code = 200
 
         self.assertRaises(
             JobError,
             client.get_origin_destination_matrix,
             origins=origins,
             destinations=destinations,
+            mode="async",
         )
 
         mock_requests.get.assert_called()
 
     @mock.patch("mango.clients.arcgis.requests")
-    def test_job_cancelled(self, mock_requests):
+    def test_job_cancelled_async(self, mock_requests):
         origins = [{"x": 1, "y": 1, "name": "First location"}]
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
 
         mock_requests.get.return_value.json.side_effect = [
             {"jobId": 100},
             {"jobStatus": "esriJobCancelled"},
             {"jobStatus": "esriJobCancelled"},
         ]
+        mock_requests.get.return_value.status_code = 200
 
         self.assertRaises(
             JobError,
             client.get_origin_destination_matrix,
             origins=origins,
             destinations=destinations,
+            mode="async",
         )
 
         mock_requests.get.assert_called()
 
     @mock.patch("mango.clients.arcgis.requests")
-    def test_job_timed_out(self, mock_requests):
+    def test_job_timed_out_async(self, mock_requests):
         origins = [{"x": 1, "y": 1, "name": "First location"}]
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
 
         mock_requests.get.return_value.json.side_effect = [
             {"jobId": 100},
             {"jobStatus": "esriJobTimedOut"},
             {"jobStatus": "esriJobTimedOut"},
         ]
+        mock_requests.get.return_value.status_code = 200
 
         self.assertRaises(
             JobError,
             client.get_origin_destination_matrix,
             origins=origins,
             destinations=destinations,
+            mode="async",
         )
 
         mock_requests.get.assert_called()
 
     @mock.patch("mango.clients.arcgis.requests")
-    def test_job_cancelling(self, mock_requests):
+    def test_job_cancelling_async(self, mock_requests):
         origins = [{"x": 1, "y": 1, "name": "First location"}]
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
 
         mock_requests.get.return_value.json.side_effect = [
             {"jobId": 100},
             {"jobStatus": "esriJobCancelling"},
             {"jobStatus": "esriJobCancelling"},
         ]
+        mock_requests.get.return_value.status_code = 200
 
         self.assertRaises(
             JobError,
             client.get_origin_destination_matrix,
             origins=origins,
             destinations=destinations,
+            mode="async",
         )
 
         mock_requests.get.assert_called()
 
     @mock.patch("mango.clients.arcgis.requests")
-    def test_iterations_correct(self, mock_requests):
+    def test_iterations_correct_async(self, mock_requests):
         origins = [{"x": 1, "y": 1, "name": "First location"}]
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
 
         mock_requests.get.return_value.json.side_effect = [
             {"jobId": 100},
             {"jobStatus": "some_other_status"},
@@ -231,17 +244,20 @@
                                 "DestinationName": "Second location",
                             }
                         }
                     ]
                 }
             },
         ]
+        mock_requests.get.return_value.status_code = 200
 
         response = client.get_origin_destination_matrix(
-            origins=origins, destinations=destinations
+            origins=origins,
+            destinations=destinations,
+            mode="async",
         )
 
         self.assertEqual(
             response,
             [
                 {
                     "origin": "First location",
@@ -251,24 +267,100 @@
                 }
             ],
         )
 
         mock_requests.get.assert_called()
 
     @mock.patch("mango.clients.arcgis.requests")
-    def test_job_id_missing(self, mock_requests):
+    def test_job_id_missing_async(self, mock_requests):
         origins = [{"x": 1, "y": 1, "name": "First location"}]
         destinations = [{"x": 2, "y": 2, "name": "Second location"}]
         client = self.test_connect()
 
         mock_requests.get.return_value.json.side_effect = [
             {"no_job_id": 100},
             {"no_job_id": 100},
         ]
+        mock_requests.get.return_value.status_code = 200
 
         self.assertRaises(
             JobError,
             client.get_origin_destination_matrix,
             origins=origins,
             destinations=destinations,
+            mode="async",
         )
         mock_requests.get.assert_called_once()
+
+    @mock.patch("mango.clients.arcgis.requests")
+    def test_get_distances_sync(self, mock_requests):
+        origins = [{"x": 1, "y": 1, "name": "First location"}]
+        destinations = [{"x": 2, "y": 2, "name": "Second location"}]
+        client = self.test_connect()
+
+        mock_requests.get.return_value.status_code = 200
+        mock_requests.get.return_value.json.side_effect = [
+            {"keys": ["odCostMatrix"]},
+            {
+                "requestID": "45677c50-593e-4591-8dcf-4902f1dd6cdd",
+                "odCostMatrix": {
+                    "costAttributeNames": ["TravelTime", "Miles", "Kilometers"],
+                    "1001": {
+                        "10001": [
+                            1,
+                            1,
+                            1,
+                        ]
+                    },
+                },
+                "messages": [],
+            },
+        ]
+
+        response = client.get_origin_destination_matrix(
+            mode="sync", origins=origins, destinations=destinations
+        )
+
+        self.assertEqual(
+            response,
+            [
+                {
+                    "origin": "First location",
+                    "destination": "Second location",
+                    "distance": 1000,
+                    "time": 60,
+                }
+            ],
+        )
+
+    @mock.patch("mango.clients.arcgis.requests")
+    def test_get_distances_sync_error(self, mock_requests):
+        origins = [{"x": 1, "y": 1, "name": "First location"}]
+        destinations = [{"x": 2, "y": 2, "name": "Second location"}]
+        client = self.test_connect()
+
+        mock_requests.get.return_value.status_code = 400
+        self.assertRaises(
+            Exception,
+            client.get_origin_destination_matrix,
+            origins=origins,
+            destinations=destinations,
+            mode="sync",
+        )
+
+    @mock.patch("mango.clients.arcgis.requests")
+    def test_get_distances_sync_error_message(self, mock_requests):
+        origins = [{"x": 1, "y": 1, "name": "First location"}]
+        destinations = [{"x": 2, "y": 2, "name": "Second location"}]
+        client = self.test_connect()
+
+        mock_requests.get.return_value.status_code = 200
+        mock_requests.get.return_value.json.side_effect = [
+            {"keys": ["odCostMatrix"]},
+        ]
+        self.assertRaises(
+            Exception,
+            client.get_origin_destination_matrix,
+            origins=origins,
+            destinations=destinations,
+            mode="sync",
+        )
```

### Comparing `mango-0.0.1/mango/tests/test_config.py` & `mango-0.0.2/mango/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_date_functions.py` & `mango-0.0.2/mango/tests/test_date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_file_functions.py` & `mango-0.0.2/mango/tests/test_file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_images.py` & `mango-0.0.2/mango/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_logging.py` & `mango-0.0.2/mango/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_models.py` & `mango-0.0.2/mango/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_object_functions.py` & `mango-0.0.2/mango/tests/test_object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_processing_time_series.py` & `mango-0.0.2/mango/tests/test_processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango/tests/test_validation.py` & `mango-0.0.2/mango/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.1/mango.egg-info/PKG-INFO` & `mango-0.0.2/mango.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
@@ -25,7 +25,8 @@
 Provides-Extra: data
 Provides-Extra: images
 Provides-Extra: logging
 Provides-Extra: model
 Provides-Extra: plot
 Provides-Extra: processing
 Provides-Extra: shared
+Provides-Extra: table
```

### Comparing `mango-0.0.1/mango.egg-info/SOURCES.txt` & `mango-0.0.2/mango.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 mango/data/__init__.py
 mango/data/ts_dataset.pkl
 mango/images/__init__.py
 mango/images/images_functions.py
 mango/logging/__init__.py
 mango/logging/chrono.py
 mango/logging/decorators.py
+mango/logging/logger.py
 mango/models/__init__.py
 mango/models/activations.py
 mango/models/neural_networks.py
 mango/plots/__init__.py
 mango/plots/plots.py
 mango/processing/__init__.py
 mango/processing/date_functions.py
@@ -34,25 +35,32 @@
 mango/processing/object_functions.py
 mango/processing/processing_time_series.py
 mango/schemas/location.json
 mango/shared/__init__.py
 mango/shared/const.py
 mango/shared/decorators.py
 mango/shared/exceptions.py
+mango/table/__init__.py
+mango/table/pytups_table.py
+mango/table/pytups_tools.py
+mango/table/table_tools.py
 mango/tests/__init__.py
 mango/tests/const.py
 mango/tests/test_arcgis_client.py
 mango/tests/test_config.py
 mango/tests/test_date_functions.py
 mango/tests/test_file_functions.py
 mango/tests/test_images.py
 mango/tests/test_logging.py
 mango/tests/test_models.py
 mango/tests/test_object_functions.py
 mango/tests/test_processing_time_series.py
+mango/tests/test_table.py
+mango/tests/test_tools.py
 mango/tests/test_validation.py
+mango/tests/data/json_dataset.json
 mango/tests/data/test.csv
 mango/tests/data/test.json
 mango/tests/data/test.xlsx
 mango/tests/data/test_bad_type.cfg
 mango/tests/data/test_bad_value.cfg
 mango/tests/data/test_good.cfg
```

### Comparing `mango-0.0.1/setup.py` & `mango-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,20 +29,26 @@
     ],
     "processing": [
         "numpy",
         "pandas",
         "xlsxwriter",
     ],
     "shared": ["fastjsonschema"],
+    "table": [
+        "pytups",
+        "numpy",
+        "pandas",
+        "xlsxwriter",
+    ],
 }
 
 
 setuptools.setup(
     name="mango",
-    version="0.0.1",
+    version="0.0.2",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Library with a collection of useful classes and methods to DRY",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/mango",
     packages=setuptools.find_packages(),
     classifiers=[
```

