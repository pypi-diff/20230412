# Comparing `tmp/pybicyclewheel-0.0.9.tar.gz` & `tmp/pybicyclewheel-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybicyclewheel-0.0.9.tar", last modified: Wed Apr 12 15:04:24 2023, max compression
+gzip compressed data, was "pybicyclewheel-0.0.9a0.tar", last modified: Wed Apr 12 15:04:04 2023, max compression
```

## Comparing `pybicyclewheel-0.0.9.tar` & `pybicyclewheel-0.0.9a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:24.286132 pybicyclewheel-0.0.9/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    34078 2022-06-08 15:42:59.000000 pybicyclewheel-0.0.9/LICENSE.md
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3537 2023-04-12 15:04:24.286132 pybicyclewheel-0.0.9/PKG-INFO
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:24.286132 pybicyclewheel-0.0.9/pybicyclewheel/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       19 2023-04-12 15:04:19.000000 pybicyclewheel-0.0.9/pybicyclewheel/__init__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1871 2022-05-15 08:04:04.000000 pybicyclewheel-0.0.9/pybicyclewheel/dataloader.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1956 2021-08-25 01:20:47.000000 pybicyclewheel-0.0.9/pybicyclewheel/hub.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      472 2021-06-15 07:13:11.000000 pybicyclewheel-0.0.9/pybicyclewheel/rim.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2019 2021-06-15 07:13:11.000000 pybicyclewheel-0.0.9/pybicyclewheel/wheel.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1225 2023-04-12 15:00:52.000000 pybicyclewheel-0.0.9/pybicyclewheel/xls_calc.py
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:24.286132 pybicyclewheel-0.0.9/pybicyclewheel.egg-info/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3537 2023-04-12 15:04:24.000000 pybicyclewheel-0.0.9/pybicyclewheel.egg-info/PKG-INFO
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      489 2023-04-12 15:04:24.000000 pybicyclewheel-0.0.9/pybicyclewheel.egg-info/SOURCES.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        1 2023-04-12 15:04:24.000000 pybicyclewheel-0.0.9/pybicyclewheel.egg-info/dependency_links.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       21 2023-04-12 15:04:24.000000 pybicyclewheel-0.0.9/pybicyclewheel.egg-info/requires.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       34 2023-04-12 15:04:24.000000 pybicyclewheel-0.0.9/pybicyclewheel.egg-info/top_level.txt
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:24.286132 pybicyclewheel-0.0.9/pybicyclewheel_gui/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        0 2021-07-30 04:27:58.000000 pybicyclewheel-0.0.9/pybicyclewheel_gui/__init__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     7030 2023-04-12 15:00:53.000000 pybicyclewheel-0.0.9/pybicyclewheel_gui/__main__.py
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:24.286132 pybicyclewheel-0.0.9/pybicyclewheel_gui/tile/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      279 2021-09-23 08:33:01.000000 pybicyclewheel-0.0.9/pybicyclewheel_gui/tile/__init__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    12710 2023-04-12 15:00:53.000000 pybicyclewheel-0.0.9/pybicyclewheel_gui/tile/core.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       38 2023-04-12 15:04:24.286132 pybicyclewheel-0.0.9/setup.cfg
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1666 2022-06-08 15:55:12.000000 pybicyclewheel-0.0.9/setup.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:04.713987 pybicyclewheel-0.0.9a0/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    34078 2022-06-08 15:42:59.000000 pybicyclewheel-0.0.9a0/LICENSE.md
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3539 2023-04-12 15:04:04.709987 pybicyclewheel-0.0.9a0/PKG-INFO
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:04.709987 pybicyclewheel-0.0.9a0/pybicyclewheel/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       20 2022-05-15 07:28:57.000000 pybicyclewheel-0.0.9a0/pybicyclewheel/__init__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1871 2022-05-15 08:04:04.000000 pybicyclewheel-0.0.9a0/pybicyclewheel/dataloader.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1956 2021-08-25 01:20:47.000000 pybicyclewheel-0.0.9a0/pybicyclewheel/hub.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      472 2021-06-15 07:13:11.000000 pybicyclewheel-0.0.9a0/pybicyclewheel/rim.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2019 2021-06-15 07:13:11.000000 pybicyclewheel-0.0.9a0/pybicyclewheel/wheel.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1225 2023-04-12 15:00:52.000000 pybicyclewheel-0.0.9a0/pybicyclewheel/xls_calc.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:04.709987 pybicyclewheel-0.0.9a0/pybicyclewheel.egg-info/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3539 2023-04-12 15:04:04.000000 pybicyclewheel-0.0.9a0/pybicyclewheel.egg-info/PKG-INFO
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      489 2023-04-12 15:04:04.000000 pybicyclewheel-0.0.9a0/pybicyclewheel.egg-info/SOURCES.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        1 2023-04-12 15:04:04.000000 pybicyclewheel-0.0.9a0/pybicyclewheel.egg-info/dependency_links.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       21 2023-04-12 15:04:04.000000 pybicyclewheel-0.0.9a0/pybicyclewheel.egg-info/requires.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       34 2023-04-12 15:04:04.000000 pybicyclewheel-0.0.9a0/pybicyclewheel.egg-info/top_level.txt
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:04.709987 pybicyclewheel-0.0.9a0/pybicyclewheel_gui/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        0 2021-07-30 04:27:58.000000 pybicyclewheel-0.0.9a0/pybicyclewheel_gui/__init__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     7030 2023-04-12 15:00:53.000000 pybicyclewheel-0.0.9a0/pybicyclewheel_gui/__main__.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-04-12 15:04:04.709987 pybicyclewheel-0.0.9a0/pybicyclewheel_gui/tile/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      279 2021-09-23 08:33:01.000000 pybicyclewheel-0.0.9a0/pybicyclewheel_gui/tile/__init__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    12710 2023-04-12 15:00:53.000000 pybicyclewheel-0.0.9a0/pybicyclewheel_gui/tile/core.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       38 2023-04-12 15:04:04.713987 pybicyclewheel-0.0.9a0/setup.cfg
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1666 2022-06-08 15:55:12.000000 pybicyclewheel-0.0.9a0/setup.py
```

### Comparing `pybicyclewheel-0.0.9/LICENSE.md` & `pybicyclewheel-0.0.9a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybicyclewheel-0.0.9/PKG-INFO` & `pybicyclewheel-0.0.9a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybicyclewheel
-Version: 0.0.9
+Version: 0.0.9a0
 Summary: pybicyclewheel - bicycle spoke length calculator
 Home-page: https://github.com/kr-g/pybicyclewheel
 Author: k. goger
 Author-email: k.r.goger+pybicyclewheel@gmail.com
 License: UNKNOWN
 Keywords: bicycle spoke length calculator
 Platform: UNKNOWN
```

### Comparing `pybicyclewheel-0.0.9/pybicyclewheel/dataloader.py` & `pybicyclewheel-0.0.9a0/pybicyclewheel/dataloader.py`

 * *Files identical despite different names*

### Comparing `pybicyclewheel-0.0.9/pybicyclewheel/hub.py` & `pybicyclewheel-0.0.9a0/pybicyclewheel/hub.py`

 * *Files identical despite different names*

### Comparing `pybicyclewheel-0.0.9/pybicyclewheel/wheel.py` & `pybicyclewheel-0.0.9a0/pybicyclewheel/wheel.py`

 * *Files identical despite different names*

### Comparing `pybicyclewheel-0.0.9/pybicyclewheel/xls_calc.py` & `pybicyclewheel-0.0.9a0/pybicyclewheel/xls_calc.py`

 * *Files identical despite different names*

### Comparing `pybicyclewheel-0.0.9/pybicyclewheel.egg-info/PKG-INFO` & `pybicyclewheel-0.0.9a0/pybicyclewheel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybicyclewheel
-Version: 0.0.9
+Version: 0.0.9a0
 Summary: pybicyclewheel - bicycle spoke length calculator
 Home-page: https://github.com/kr-g/pybicyclewheel
 Author: k. goger
 Author-email: k.r.goger+pybicyclewheel@gmail.com
 License: UNKNOWN
 Keywords: bicycle spoke length calculator
 Platform: UNKNOWN
```

### Comparing `pybicyclewheel-0.0.9/pybicyclewheel_gui/__main__.py` & `pybicyclewheel-0.0.9a0/pybicyclewheel_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `pybicyclewheel-0.0.9/pybicyclewheel_gui/tile/core.py` & `pybicyclewheel-0.0.9a0/pybicyclewheel_gui/tile/core.py`

 * *Files identical despite different names*

### Comparing `pybicyclewheel-0.0.9/setup.py` & `pybicyclewheel-0.0.9a0/setup.py`

 * *Files identical despite different names*

