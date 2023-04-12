# Comparing `tmp/py_silhouette-0.4.2.tar.gz` & `tmp/py_silhouette-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_silhouette-0.4.2.tar", last modified: Fri Aug 26 13:24:01 2022, max compression
+gzip compressed data, was "py_silhouette-0.4.3.tar", last modified: Wed Apr 12 06:33:24 2023, max compression
```

## Comparing `py_silhouette-0.4.2.tar` & `py_silhouette-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-08-26 13:24:01.101030 py_silhouette-0.4.2/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      818 2022-08-26 13:24:01.101030 py_silhouette-0.4.2/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2670 2019-01-20 19:51:33.000000 py_silhouette-0.4.2/README.md
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-08-26 13:24:01.097699 py_silhouette-0.4.2/py_silhouette/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      202 2019-01-20 19:37:22.000000 py_silhouette-0.4.2/py_silhouette/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    24367 2022-01-28 21:46:08.000000 py_silhouette-0.4.2/py_silhouette/device.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       23 2022-08-26 13:23:49.000000 py_silhouette-0.4.2/py_silhouette/version.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-08-26 13:24:01.101030 py_silhouette-0.4.2/py_silhouette.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      818 2022-08-26 13:24:00.000000 py_silhouette-0.4.2/py_silhouette.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      296 2022-08-26 13:24:01.000000 py_silhouette-0.4.2/py_silhouette.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2022-08-26 13:24:00.000000 py_silhouette-0.4.2/py_silhouette.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2022-08-26 13:24:00.000000 py_silhouette-0.4.2/py_silhouette.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       14 2022-08-26 13:24:01.000000 py_silhouette-0.4.2/py_silhouette.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2022-08-26 13:24:01.101030 py_silhouette-0.4.2/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1086 2022-08-26 13:23:43.000000 py_silhouette-0.4.2/setup.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-08-26 13:24:01.101030 py_silhouette-0.4.2/test/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4367 2020-09-01 13:44:40.000000 py_silhouette-0.4.2/test/test_sheet.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.752268 py_silhouette-0.4.3/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2670 2019-01-20 19:51:33.000000 py_silhouette-0.4.3/README.md
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/py_silhouette/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      202 2019-01-20 19:37:22.000000 py_silhouette-0.4.3/py_silhouette/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    24444 2023-04-12 06:27:29.000000 py_silhouette-0.4.3/py_silhouette/device.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       23 2023-04-12 06:31:20.000000 py_silhouette-0.4.3/py_silhouette/version.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/py_silhouette.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      296 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       14 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2023-04-12 06:33:24.752268 py_silhouette-0.4.3/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1086 2022-08-26 13:23:43.000000 py_silhouette-0.4.3/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/test/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4367 2020-09-01 13:44:40.000000 py_silhouette-0.4.3/test/test_sheet.py
```

### Comparing `py_silhouette-0.4.2/PKG-INFO` & `py_silhouette-0.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: py_silhouette
-Version: 0.4.2
+Version: 0.4.3
 Summary: A USB driver and Python API to control the Silhouette Portrait plotter.
 Home-page: https://github.com/mossblaser/py_silhouette
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: plotter cutter driver usb silhouette
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
-
-UNKNOWN
-
```

### Comparing `py_silhouette-0.4.2/README.md` & `py_silhouette-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `py_silhouette-0.4.2/py_silhouette/device.py` & `py_silhouette-0.4.3/py_silhouette/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,24 +222,26 @@
         area_width_max=inch2mm(12.0),
         area_height_min=inch2mm(3.0),
         area_height_max=inch2mm(40.0),
         tool_depth_min=0,
         tool_depth_max=10,
     ),
     # Contributed by Yohalmo Garcia (@yohalmogarcia on GitHub, see issue #3)
+    # and @LoveisAFK on GitHub (see issue #6)
     DeviceParameters(
         product_name='Silhouette Cameo4',
         usb_vendor_id=0x0B4D,
         usb_product_id=0x1137,
         area_width_min=inch2mm(3.0),
         area_width_max=inch2mm(12.0),
         area_height_min=inch2mm(3.0),
         area_height_max=inch2mm(40.0),
         tool_depth_min=0,
         tool_depth_max=10,
+        tool_speed_max=3000.0,
     ),
 ]
 
 
 def enumerate_devices(supported_device_parameters=SUPPORTED_DEVICE_PARAMETERS):
     """
     Generator which produces a series of ``(device, device_params)`` pairs for
```

### Comparing `py_silhouette-0.4.2/py_silhouette.egg-info/PKG-INFO` & `py_silhouette-0.4.3/py_silhouette.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: py-silhouette
-Version: 0.4.2
+Version: 0.4.3
 Summary: A USB driver and Python API to control the Silhouette Portrait plotter.
 Home-page: https://github.com/mossblaser/py_silhouette
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: plotter cutter driver usb silhouette
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
-
-UNKNOWN
-
```

### Comparing `py_silhouette-0.4.2/setup.py` & `py_silhouette-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `py_silhouette-0.4.2/test/test_sheet.py` & `py_silhouette-0.4.3/test/test_sheet.py`

 * *Files identical despite different names*

