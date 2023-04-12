# Comparing `tmp/nowcasting_datamodel-1.2.7.tar.gz` & `tmp/nowcasting_datamodel-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.2.7.tar", last modified: Tue Apr 11 17:12:04 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.2.8.tar", last modified: Wed Apr 12 10:30:06 2023, max compression
```

## Comparing `nowcasting_datamodel-1.2.7.tar` & `nowcasting_datamodel-1.2.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.256847 nowcasting_datamodel-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 17:12:04.252848 nowcasting_datamodel-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.248847 nowcasting_datamodel-1.2.7/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.248847 nowcasting_datamodel-1.2.7/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.252848 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.252848 nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.252848 nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.248847 nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 17:12:04.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 17:12:04.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:12:04.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 17:12:04.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 17:12:04.000000 nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:12:04.256847 nowcasting_datamodel-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:12:04.252848 nowcasting_datamodel-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-11 17:11:50.000000 nowcasting_datamodel-1.2.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.668275 nowcasting_datamodel-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-12 10:30:06.668275 nowcasting_datamodel-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.660275 nowcasting_datamodel-1.2.8/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.664275 nowcasting_datamodel-1.2.8/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.664275 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.668275 nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.668275 nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.664275 nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-12 10:30:06.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-12 10:30:06.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:30:06.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 10:30:06.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 10:30:06.000000 nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:30:06.668275 nowcasting_datamodel-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:30:06.668275 nowcasting_datamodel-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 10:29:55.000000 nowcasting_datamodel-1.2.8/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.2.7/PKG-INFO` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nowcasting_datamodel
-Version: 1.2.7
+Name: nowcasting-datamodel
+Version: 1.2.8
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.2.7/README.md` & `nowcasting_datamodel-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/diagram.png` & `nowcasting_datamodel-1.2.8/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/diagram_pv.png` & `nowcasting_datamodel-1.2.8/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,14 @@
             )
 
         return self
 
     def adjust(self, limit: float = 0.0):
         """Adjust forecasts"""
         if isinstance(self._adjust_mw, float):
-
             adjust_mw = self._adjust_mw
             if adjust_mw > limit:
                 adjust_mw = limit
             elif adjust_mw < -limit:
                 adjust_mw = -limit
 
             self.expected_power_generation_megawatts = (
```

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/blend.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/blend.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
     # if all forecasts are later than 2 hours, then we use the blend,
     # otherwise we only use forecast less than 2 hours
     if one_forecast_created_within_timedelta:
         # remove all forecasts that are older than 2 hours
         forecast_values_all_model_valid = []
         for model_name, forecast_values_one_model in forecast_values_all_model:
-
             one_forecast_created_within_timedelta = forecast_values_one_model[
                 0
             ].created_utc < datetime.now(timezone.utc) - timedelta(hours=2)
 
             if one_forecast_created_within_timedelta:
                 logger.debug(f"Will be using forecast {model_name} as it is newer than 2 hours")
                 forecast_values_all_model_valid.append([model_name, forecast_values_one_model])
@@ -92,15 +91,14 @@
     # - "expected_power_generation_megawatts",
     # - "adjust_mw",
     # - "created_utc",
     # - "model_name",
     logger.debug(f"Getting values from {len(forecast_values_all_model_valid)} models")
     forecast_values_all_model_df = []
     for model_name, forecast_values_one_model in forecast_values_all_model_valid:
-
         logger.debug(f"Making dataframe for {model_name}")
 
         values_list = [
             [
                 value.target_time,
                 value.expected_power_generation_megawatts,
                 value.adjust_mw,
@@ -157,15 +155,14 @@
 
     # now lets deal with the weights
     duplicated = forecast_values_all_model.loc[duplicated_target_times_idx]
     duplicated = duplicated.drop_duplicates()
 
     # only do this if there are duplicated
     if len(duplicated) > 0:
-
         logger.debug(f"Now blending the duplicated target times using {weights_df}")
 
         pd.DataFrame()
         # unstack the weights
         weights_one_df = weights_df.stack()
         weights_one_df.name = "weight"
         weights_one_df = weights_one_df.reset_index()
```

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nowcasting-datamodel
-Version: 1.2.7
+Name: nowcasting_datamodel
+Version: 1.2.8
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.2.7/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.2.8/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/setup.py` & `nowcasting_datamodel-1.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.2.8/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/tests/test_fake.py` & `nowcasting_datamodel-1.2.8/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/tests/test_fake_pv.py` & `nowcasting_datamodel-1.2.8/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.7/tests/test_national.py` & `nowcasting_datamodel-1.2.8/tests/test_national.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from nowcasting_datamodel import N_GSP
 from nowcasting_datamodel.models import LocationSQL
 from nowcasting_datamodel.models.forecast import Forecast, ForecastSQL
 from nowcasting_datamodel.national import make_national_forecast
 
 
 def test_make_national_forecast(forecasts_all, db_session):
-
     locations = db_session.query(LocationSQL).all()
     assert len(locations) == N_GSP
 
     national_forecast = make_national_forecast(forecasts=forecasts_all, session=db_session)
     db_session.add(national_forecast)
     db_session.commit()
```

### Comparing `nowcasting_datamodel-1.2.7/tests/test_utils.py` & `nowcasting_datamodel-1.2.8/tests/test_utils.py`

 * *Files identical despite different names*

