# Comparing `tmp/percy-appium-app-1.1.0.tar.gz` & `tmp/percy-appium-app-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-appium-app-1.1.0.tar", last modified: Mon Apr 10 08:10:06 2023, max compression
+gzip compressed data, was "percy-appium-app-1.2.0.tar", last modified: Wed Apr 12 12:27:28 2023, max compression
```

## Comparing `percy-appium-app-1.1.0.tar` & `percy-appium-app-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/configs/devices.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/tile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/metadata_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/provider_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy_appium_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_metadata_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.524994 percy-appium-app-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-12 12:27:28.524994 percy-appium-app-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/configs/devices.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/metadata_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/provider_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy_appium_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:27:28.524994 percy-appium-app-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_metadata_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_tile.py
```

### Comparing `percy-appium-app-1.1.0/LICENSE` & `percy-appium-app-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/PKG-INFO` & `percy-appium-app-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: percy-appium-app
-Version: 1.1.0
-Summary: Python client for visual testing with Percy for mobile apps
-Home-page: https://github.com/percy/percy-appium-python
-Author: Perceptual Inc.
-Author-email: team@percy.io
-License: MIT
-Keywords: appium percy visual testing
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # percy-appium-python
 [![PyPI version](https://badge.fury.io/py/percy-appium-app.svg)](https://pypi.org/project/percy-appium-app/)
 ![Test](https://github.com/percy/percy-appium-python/workflows/Test/badge.svg)
 
 [Percy](https://percy.io) visual testing for Python Appium.
 
 ## Installation
@@ -84,14 +63,39 @@
 - `device_name` (**optional**) - The device name used for capturing screenshot
 - `orientation` (**optional**) - Orientation of device while capturing screeenshot; Allowed values [`portrait` | `landscape`]
 - `status_bar_height` (**optional**) - Height of status bar; int
 - `nav_bar_height` (**optional**) - Height of navigation bar; int
 - `full_screen` (**optional**) - Indicate whether app is full screen; boolean
 - `fullpage` (**optional**) - [Experimental] only supported on App Automate driver sessions [ needs @percy/cli 1.20.2+ ]; boolean
 - `screen_lengths` (**optional**) - [Experimental] max screen lengths for fullPage [ needs @percy/cli 1.20.2+ ]; boolean
+- `scrollable_xpath` (**optional**) - [Experimental] scrollable element xpath for fullpage [ needs @percy/cli 1.20.2+ ]; string
+- `scrollable_id` (**optional**) - [Experimental] scrollable element accessibility id for fullpage [ needs @percy/cli 1.20.2+ ]; string
+- `ignore_regions_xpaths` (**optional**) - elements xpaths that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of string
+- `ignore_region_accessibility_ids` (**optional**) - elements accessibility_ids that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of string
+- `ignore_region_appium_elements` (**optional**) - appium elements that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of appium element object
+- `custom_ignore_regions` (**optional**) - custom locations that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of ignore_region object
+  - IgnoreRegion:-
+    - Description: This class represents a rectangular area on a screen that needs to be ignored for visual diff.
+
+    - Constructor:
+      ```
+      init(self, top, bottom, left, right)
+      ```
+
+    - Parameters:
+
+      `top` (int): Top coordinate of the ignore region.
+
+      `bottom` (int): Bottom coordinate of the ignore region.
+
+      `left` (int): Left coordinate of the ignore region.
+
+      `right` (int): Right coordinate of the ignore region.
+    - Raises:ValueError: If top, bottom, left, or right is less than 0 or top is greater than or equal to bottom or left is greater than or equal to right.
+    - valid: Ignore region should be within the boundaries of the screen.
 ### Migrating Config
 
 If you have a previous Percy configuration file, migrate it to the newest version with the
 [`config:migrate`](https://github.com/percy/cli/tree/master/packages/cli-config#percy-configmigrate-filepath-output) command:
 
 ```sh-session
 $ percy config:migrate
```

### Comparing `percy-appium-app-1.1.0/percy/__init__.py` & `percy-appium-app-1.2.0/percy/__init__.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/configs/devices.json` & `percy-appium-app-1.2.0/percy/configs/devices.json`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/lib/app_percy.py` & `percy-appium-app-1.2.0/percy/lib/app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/lib/cache.py` & `percy-appium-app-1.2.0/percy/lib/cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/lib/cli_wrapper.py` & `percy-appium-app-1.2.0/percy/lib/cli_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,26 +40,26 @@
 
             return True
         except Exception as e:
             log('Percy is not running, disabling screenshots')
             log(e, on_debug=True)
             return False
 
-    def post_screenshots(self, name, tag, tiles, external_debug_url=None):
-        body = self._request_body(name, tag, tiles, external_debug_url)
+    def post_screenshots(self, name, tag, tiles, external_debug_url=None, ignored_elements_data=None):
+        body = self._request_body(name, tag, tiles, external_debug_url, ignored_elements_data)
 
         body['client_info'] = CLIENT_INFO
         body['environment_info'] = ENV_INFO
 
         response = requests.post(f'{PERCY_CLI_API}/percy/comparison', json=body, timeout=30)
         # Handle errors
         response.raise_for_status()
         data = response.json()
 
         if response.status_code != 200:
             raise CLIException(data.get('error', 'UnknownException'))
         return data
 
     @staticmethod
-    def _request_body(name, tag, tiles, external_debug_url):
+    def _request_body(name, tag, tiles, external_debug_url, ignored_elements_data):
         tiles = list(map(dict, tiles))
-        return {"name": name, "tag": tag, "tiles": tiles, "external_debug_url": external_debug_url}
+        return {"name": name, "tag": tag, "tiles": tiles, "ignored_elements_data": ignored_elements_data, "external_debug_url": external_debug_url}
```

### Comparing `percy-appium-app-1.1.0/percy/lib/percy_options.py` & `percy-appium-app-1.2.0/percy/lib/percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/lib/tile.py` & `percy-appium-app-1.2.0/percy/lib/tile.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/metadata/android_metadata.py` & `percy-appium-app-1.2.0/percy/metadata/android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/metadata/ios_metadata.py` & `percy-appium-app-1.2.0/percy/metadata/ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/metadata/metadata.py` & `percy-appium-app-1.2.0/percy/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/providers/app_automate.py` & `percy-appium-app-1.2.0/percy/providers/app_automate.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,17 +34,21 @@
         self.debug_url = "https://app-automate.browserstack.com/dashboard/v2/builds/" + build_hash + "/sessions/" + session_hash
 
     def _get_tiles(self, **kwargs):
         fullpage_ss = kwargs.get('fullpage', False)
         if not fullpage_ss:
             return super()._get_tiles(**kwargs)
         screen_lengths = kwargs.get('screen_lengths', 4)
+        scrollable_xpath = kwargs.get('scollable_xpath')
+        scrollable_id = kwargs.get('scrollable_id')
         data = self.execute_percy_screenshot(
             self.metadata.device_screen_size.get('height', 1),
             screen_lengths,
+            scrollable_xpath,
+            scrollable_id,
             self.metadata.scale_factor,
         )
         tiles = []
         status_bar_height = self.metadata.status_bar_height
         nav_bar_height = self.metadata.navigation_bar_height
         for tile_data in json.loads(data.get('result')):
             tiles.append(Tile(
@@ -90,24 +94,29 @@
             if status_message: request_body['arguments']['statusMessage'] = status_message
             command = f'browserstack_executor: {json.dumps(request_body)}'
             self.metadata.execute_script(command)
         except Exception as e:
             log('Error occurred during end call', on_debug=True)
             log(e, on_debug=True)
 
-    def execute_percy_screenshot(self, device_height, screen_lengths, scale_factor=1):
+    def execute_percy_screenshot(self, device_height, screen_lengths, scrollable_xpath=None, scrollable_id=None, scale_factor=1):
         try:
             request_body = {
                 'action': 'percyScreenshot',
                 'arguments': {
                     'state': 'screenshot',
                     'percyBuildId':  os.getenv('PERCY_BUILD_ID', ''),
                     'screenshotType': 'fullpage',
                     'scaleFactor': scale_factor,
-                    'options': { "numOfTiles": screen_lengths, "deviceHeight": device_height },
+                    'options': { 
+                        "numOfTiles": screen_lengths,
+                        "deviceHeight": device_height,
+                        "scrollableXpath":  scrollable_xpath,
+                        "scrollableId": scrollable_id
+                    },
                 }
             }
             command = f'browserstack_executor: {json.dumps(request_body)}'
             response = self.metadata.execute_script(command)
             response = json.loads(response)
             return response
         except Exception as e:
```

### Comparing `percy-appium-app-1.1.0/percy/providers/provider_resolver.py` & `percy-appium-app-1.2.0/percy/providers/provider_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy/screenshot.py` & `percy-appium-app-1.2.0/percy/screenshot.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/percy_appium_app.egg-info/PKG-INFO` & `percy-appium-app-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -84,14 +84,39 @@
 - `device_name` (**optional**) - The device name used for capturing screenshot
 - `orientation` (**optional**) - Orientation of device while capturing screeenshot; Allowed values [`portrait` | `landscape`]
 - `status_bar_height` (**optional**) - Height of status bar; int
 - `nav_bar_height` (**optional**) - Height of navigation bar; int
 - `full_screen` (**optional**) - Indicate whether app is full screen; boolean
 - `fullpage` (**optional**) - [Experimental] only supported on App Automate driver sessions [ needs @percy/cli 1.20.2+ ]; boolean
 - `screen_lengths` (**optional**) - [Experimental] max screen lengths for fullPage [ needs @percy/cli 1.20.2+ ]; boolean
+- `scrollable_xpath` (**optional**) - [Experimental] scrollable element xpath for fullpage [ needs @percy/cli 1.20.2+ ]; string
+- `scrollable_id` (**optional**) - [Experimental] scrollable element accessibility id for fullpage [ needs @percy/cli 1.20.2+ ]; string
+- `ignore_regions_xpaths` (**optional**) - elements xpaths that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of string
+- `ignore_region_accessibility_ids` (**optional**) - elements accessibility_ids that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of string
+- `ignore_region_appium_elements` (**optional**) - appium elements that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of appium element object
+- `custom_ignore_regions` (**optional**) - custom locations that user want to ignore in visual diff [ needs @percy/cli 1.23.0+ ]; list of ignore_region object
+  - IgnoreRegion:-
+    - Description: This class represents a rectangular area on a screen that needs to be ignored for visual diff.
+
+    - Constructor:
+      ```
+      init(self, top, bottom, left, right)
+      ```
+
+    - Parameters:
+
+      `top` (int): Top coordinate of the ignore region.
+
+      `bottom` (int): Bottom coordinate of the ignore region.
+
+      `left` (int): Left coordinate of the ignore region.
+
+      `right` (int): Right coordinate of the ignore region.
+    - Raises:ValueError: If top, bottom, left, or right is less than 0 or top is greater than or equal to bottom or left is greater than or equal to right.
+    - valid: Ignore region should be within the boundaries of the screen.
 ### Migrating Config
 
 If you have a previous Percy configuration file, migrate it to the newest version with the
 [`config:migrate`](https://github.com/percy/cli/tree/master/packages/cli-config#percy-configmigrate-filepath-output) command:
 
 ```sh-session
 $ percy config:migrate
```

### Comparing `percy-appium-app-1.1.0/percy_appium_app.egg-info/SOURCES.txt` & `percy-appium-app-1.2.0/percy_appium_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 percy/common/__init__.py
 percy/configs/devices.json
 percy/errors/__init__.py
 percy/lib/__init__.py
 percy/lib/app_percy.py
 percy/lib/cache.py
 percy/lib/cli_wrapper.py
+percy/lib/ignore_region.py
 percy/lib/percy_options.py
 percy/lib/tile.py
 percy/metadata/__init__.py
 percy/metadata/android_metadata.py
 percy/metadata/ios_metadata.py
 percy/metadata/metadata.py
 percy/metadata/metadata_resolver.py
@@ -30,13 +31,14 @@
 percy_appium_app.egg-info/top_level.txt
 tests/test_android_metadata.py
 tests/test_app_automate.py
 tests/test_app_percy.py
 tests/test_cache.py
 tests/test_cli_wrapper.py
 tests/test_generic_provider.py
+tests/test_ignore_region.py
 tests/test_ios_metadata.py
 tests/test_metadata.py
 tests/test_metadata_resolver.py
 tests/test_percy_options.py
 tests/test_screenshot.py
 tests/test_tile.py
```

### Comparing `percy-appium-app-1.1.0/setup.py` & `percy-appium-app-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_android_metadata.py` & `percy-appium-app-1.2.0/tests/test_android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_app_automate.py` & `percy-appium-app-1.2.0/tests/test_app_automate.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_app_percy.py` & `percy-appium-app-1.2.0/tests/test_app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_cache.py` & `percy-appium-app-1.2.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_ios_metadata.py` & `percy-appium-app-1.2.0/tests/test_ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_metadata.py` & `percy-appium-app-1.2.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_metadata_resolver.py` & `percy-appium-app-1.2.0/tests/test_metadata_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_percy_options.py` & `percy-appium-app-1.2.0/tests/test_percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.1.0/tests/test_screenshot.py` & `percy-appium-app-1.2.0/tests/test_screenshot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pylint: disable=[arguments-differ]
 import unittest
 from unittest.mock import patch, MagicMock, PropertyMock
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from threading import Thread
 from appium.webdriver.webdriver import WebDriver
+from appium.webdriver.common.appiumby import AppiumBy
+
 
 import httpretty
 
 from percy import percy_screenshot
 from percy.common import LABEL
 from percy.lib.cli_wrapper import CLIWrapper
 from percy.metadata import Metadata
@@ -16,132 +18,211 @@
 from tests.mocks.mock_methods import android_capabilities
 
 
 # mock a simple webpage to screenshot
 class MockServerRequestHandler(BaseHTTPRequestHandler):
     def do_GET(self):
         self.send_response(200)
-        self.send_header('Content-Type', 'application/json')
+        self.send_header("Content-Type", "application/json")
         self.end_headers()
-        self.wfile.write('Screenshot Me'.encode('utf-8'))
+        self.wfile.write("Screenshot Me".encode("utf-8"))
 
 
 # daemon threads automatically shut down when the main process exits
-mock_server = HTTPServer(('localhost', 8000), MockServerRequestHandler)
+mock_server = HTTPServer(("localhost", 8000), MockServerRequestHandler)
 mock_server_thread = Thread(target=mock_server.serve_forever)
 mock_server_thread.daemon = True
 mock_server_thread.start()
 
 
 # mock helpers
-def mock_healthcheck(fail=False, fail_how='error'):
+def mock_healthcheck(fail=False, fail_how="error"):
     health_body = '{ "success": true }'
-    health_headers = {'X-Percy-Core-Version': '1.0.0'}
+    health_headers = {"X-Percy-Core-Version": "1.0.0"}
     health_status = 200
 
-    if fail and fail_how == 'error':
+    if fail and fail_how == "error":
         health_body = '{ "success": false, "error": "test" }'
         health_status = 500
-    elif fail and fail_how == 'wrong-version':
-        health_headers = {'X-Percy-Core-Version': '2.0.0'}
-    elif fail and fail_how == 'no-version':
+    elif fail and fail_how == "wrong-version":
+        health_headers = {"X-Percy-Core-Version": "2.0.0"}
+    elif fail and fail_how == "no-version":
         health_headers = {}
 
     httpretty.register_uri(
-        httpretty.GET, 'http://localhost:5338/percy/healthcheck',
+        httpretty.GET,
+        "http://localhost:5338/percy/healthcheck",
         body=health_body,
         adding_headers=health_headers,
-        status=health_status)
+        status=health_status,
+    )
 
 
 def mock_screenshot(fail=False):
     httpretty.register_uri(
-        httpretty.POST, 'http://localhost:5338/percy/comparison',
-        body=('{ "success": ' + ('true' if not fail else 'false, "error": "test"') + '}'),
-        status=(500 if fail else 200))
+        httpretty.POST,
+        "http://localhost:5338/percy/comparison",
+        body=(
+            '{ "success": ' + ("true" if not fail else 'false, "error": "test"') + "}"
+        ),
+        status=(500 if fail else 200),
+    )
 
 
 class TestPercyScreenshot(unittest.TestCase):
-    @patch('appium.webdriver.webdriver.WebDriver')
+    @patch("appium.webdriver.webdriver.WebDriver")
     def setUp(self, mock_webdriver) -> None:
         mock_webdriver.__class__ = WebDriver
         CLIWrapper.is_percy_enabled.cache_clear()
         httpretty.enable()
-
+        self.maxDiff = None
         self.mock_webdriver = mock_webdriver
         self.mock_webdriver.capabilities = android_capabilities
-        self.mock_webdriver.orientation = 'PORTRAIT'
-        self.mock_webdriver.get_system_bars.return_value = \
-            {'statusBar': {'height': 10, 'width': 20}, 'navigationBar': {'height': 10, 'width': 20}}
+        self.mock_webdriver.orientation = "PORTRAIT"
+        self.mock_webdriver.get_system_bars.return_value = {
+            "statusBar": {"height": 10, "width": 20},
+            "navigationBar": {"height": 10, "width": 20},
+        }
 
     def tearDown(self):
         httpretty.disable()
         httpretty.reset()
 
-    @patch.object(GenericProvider, '_write_screenshot', MagicMock(return_value='path-to-png-file'))
-    @patch('appium.webdriver.webdriver.WebDriver')
+    @patch.object(
+        GenericProvider, "_write_screenshot", MagicMock(return_value="path-to-png-file")
+    )
+    @patch("appium.webdriver.webdriver.WebDriver")
     def test_throws_error_when_app_percy_arg_type_mismatch(self, mock_webdriver):
         mock_ios_webdriver = mock_webdriver
         mock_ios_webdriver.capabilities = android_capabilities
-        with patch('percy.metadata.IOSMetadata.remote_url', new_callable=PropertyMock) \
-                as mock_remote_url:
-            mock_remote_url.return_value = ''
+        with patch(
+            "percy.metadata.IOSMetadata.remote_url", new_callable=PropertyMock
+        ) as mock_remote_url:
+            mock_remote_url.return_value = ""
             app_percy = AppPercy(self.mock_webdriver)
             self.assertRaises(TypeError, app_percy.screenshot, 123)
-            self.assertRaises(TypeError, app_percy.screenshot, 'screenshot 1', device_name = 123)
-            self.assertRaises(TypeError, app_percy.screenshot, 'screenshot 1', full_screen = 123)
-            self.assertRaises(TypeError, app_percy.screenshot, 'screenshot 1', orientation = 123)
-            self.assertRaises(TypeError, app_percy.screenshot, 'screenshot 1', status_bar_height = 'height')
-            self.assertRaises(TypeError, app_percy.screenshot, 'screenshot 1', nav_bar_height = 'height')
-
+            self.assertRaises(
+                TypeError, app_percy.screenshot, "screenshot 1", device_name=123
+            )
+            self.assertRaises(
+                TypeError, app_percy.screenshot, "screenshot 1", full_screen=123
+            )
+            self.assertRaises(
+                TypeError, app_percy.screenshot, "screenshot 1", orientation=123
+            )
+            self.assertRaises(
+                TypeError,
+                app_percy.screenshot,
+                "screenshot 1",
+                status_bar_height="height",
+            )
+            self.assertRaises(
+                TypeError, app_percy.screenshot, "screenshot 1", nav_bar_height="height"
+            )
 
     def test_throws_error_when_a_driver_is_not_provided(self):
         with self.assertRaises(Exception):
             percy_screenshot()
+
     #
     def test_throws_error_when_a_name_is_not_provided(self):
         with self.assertRaises(Exception):
             percy_screenshot(self.mock_webdriver)
-    #
+
     def test_disables_screenshots_when_the_healthcheck_fails(self):
         mock_healthcheck(fail=True)
 
-        with patch('builtins.print') as mock_print:
-            percy_screenshot(self.mock_webdriver, 'screenshot 1')
-            percy_screenshot(self.mock_webdriver, 'screenshot 2')
-
-            mock_print.assert_called_with(f'{LABEL} Percy is not running, disabling screenshots')
+        with patch("builtins.print") as mock_print:
+            percy_screenshot(self.mock_webdriver, "screenshot 1")
+            percy_screenshot(self.mock_webdriver, "screenshot 2")
+
+            mock_print.assert_called_with(
+                f"{LABEL} Percy is not running, disabling screenshots"
+            )
 
-        self.assertEqual(httpretty.last_request().path, '/percy/healthcheck')
+        self.assertEqual(httpretty.last_request().path, "/percy/healthcheck")
 
     def test_disables_screenshots_when_the_healthcheck_version_is_wrong(self):
-        mock_healthcheck(fail=True, fail_how='wrong-version')
+        mock_healthcheck(fail=True, fail_how="wrong-version")
 
-        with patch('builtins.print') as mock_print:
-            percy_screenshot(self.mock_webdriver, 'screenshot 1')
-            percy_screenshot(self.mock_webdriver, 'screenshot 2')
+        with patch("builtins.print") as mock_print:
+            percy_screenshot(self.mock_webdriver, "screenshot 1")
+            percy_screenshot(self.mock_webdriver, "screenshot 2")
+
+            mock_print.assert_called_with(
+                f"{LABEL} Unsupported Percy CLI version, 2.0.0"
+            )
+
+        self.assertEqual(httpretty.last_request().path, "/percy/healthcheck")
+
+    @patch.object(
+        Metadata, "session_id", PropertyMock(return_value="unique_session_id")
+    )
+    @patch.object(
+        GenericProvider, "_write_screenshot", MagicMock(return_value="path-to-png-file")
+    )
+    def test_posts_multiple_screenshots_to_the_local_percy_server(self):
+        mock_healthcheck()
+        mock_screenshot()
 
-            mock_print.assert_called_with(f'{LABEL} Unsupported Percy CLI version, 2.0.0')
+        percy_screenshot(self.mock_webdriver, "screenshot 1")
+        percy_screenshot(self.mock_webdriver, "screenshot 2", full_screen=False)
 
-        self.assertEqual(httpretty.last_request().path, '/percy/healthcheck')
+        self.assertEqual(httpretty.last_request().path, "/percy/comparison")
 
-    @patch.object(Metadata, 'session_id', PropertyMock(return_value='unique_session_id'))
-    @patch.object(GenericProvider, '_write_screenshot', MagicMock(return_value='path-to-png-file'))
-    def test_posts_multiple_screenshots_to_the_local_percy_server(self):
+        body = httpretty.latest_requests()[2].parsed_body
+
+        # self.assertEqual(s1['name'], 'screenshot 1')
+        self.assertRegex(body["client_info"], r"percy-appium-app/\d+")
+        self.assertRegex(body["environment_info"][0], r"appium/\d+")
+        self.assertRegex(body["environment_info"][1], r"python/\d+")
+
+    @patch.object(
+        Metadata, "session_id", PropertyMock(return_value="unique_session_id")
+    )
+    @patch.object(
+        GenericProvider, "_write_screenshot", MagicMock(return_value="path-to-png-file")
+    )
+    def test_ignore_region_screenshots_to_the_local_percy_server(self):
         mock_healthcheck()
         mock_screenshot()
 
-        percy_screenshot(self.mock_webdriver, 'screenshot 1')
-        percy_screenshot(self.mock_webdriver, 'screenshot 2', full_screen=False)
+        # mock element
+        mock_element = MagicMock()
+        mock_element.location = {"x": 10, "y": 20}
+        mock_element.size = {"width": 200, "height": 400}
+
+        xpaths = ["//path/to/element"]
+
+        # mock call
+        self.mock_webdriver.find_element.return_value = mock_element
+
+        # exepected value
+        ignored_elements_data = {
+            "ignoreElementsData": [
+                {
+                    "selector": "xpath: //path/to/element",
+                    "coOrdinates": {"top": 20, "bottom": 420, "left": 10, "right": 210},
+                },
+            ]
+        }
+
+        percy_screenshot(
+            self.mock_webdriver, "screenshot 1", ignore_regions_xpaths=xpaths
+        )
 
-        self.assertEqual(httpretty.last_request().path, '/percy/comparison')
+        self.assertEqual(httpretty.last_request().path, "/percy/comparison")
 
-        s1 = httpretty.latest_requests()[2].parsed_body
+        body = httpretty.latest_requests()[1].parsed_body
 
         # self.assertEqual(s1['name'], 'screenshot 1')
-        self.assertRegex(s1['client_info'], r'percy-appium-app/\d+')
-        self.assertRegex(s1['environment_info'][0], r'appium/\d+')
-        self.assertRegex(s1['environment_info'][1], r'python/\d+')
+        self.assertRegex(body["client_info"], r"percy-appium-app/\d+")
+        self.assertRegex(body["environment_info"][0], r"appium/\d+")
+        self.assertDictEqual(body["ignored_elements_data"], ignored_elements_data)
+        self.mock_webdriver.find_element.assert_called_with(
+            by=AppiumBy.XPATH, value="//path/to/element"
+        )
+        self.assertEqual(self.mock_webdriver.find_element.call_count, 1)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `percy-appium-app-1.1.0/tests/test_tile.py` & `percy-appium-app-1.2.0/tests/test_tile.py`

 * *Files identical despite different names*

