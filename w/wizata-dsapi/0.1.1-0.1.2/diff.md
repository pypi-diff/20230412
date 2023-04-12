# Comparing `tmp/wizata-dsapi-0.1.1.tar.gz` & `tmp/wizata-dsapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.1.tar", last modified: Wed Apr 12 17:56:22 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.2.tar", last modified: Wed Apr 12 18:24:50 2023, max compression
```

## Comparing `wizata-dsapi-0.1.1.tar` & `wizata-dsapi-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 17:56:22.955187 wizata-dsapi-0.1.1/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-04-12 17:56:22.953980 wizata-dsapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-12 17:56:22.955187 wizata-dsapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:56:22.896469 wizata-dsapi-0.1.1/wizata_dsapi/
--rw-rw-rw-   0        0        0      599 2023-04-05 20:20:01.000000 wizata-dsapi-0.1.1/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.1.1/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.1/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     1856 2023-04-03 19:42:17.000000 wizata-dsapi-0.1.1/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.1.1/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    13455 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.1/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3555 2023-04-05 21:53:34.000000 wizata-dsapi-0.1.1/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     5447 2023-04-05 21:53:34.000000 wizata-dsapi-0.1.1/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-04-05 19:26:47.000000 wizata-dsapi-0.1.1/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.1/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0     9756 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.1/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     6914 2023-04-03 19:42:17.000000 wizata-dsapi-0.1.1/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     2003 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.1/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2235 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.1/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.1/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    33193 2023-04-08 18:17:48.000000 wizata-dsapi-0.1.1/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:56:22.949667 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 18:24:50.611252 wizata-dsapi-0.1.2/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-04-12 18:24:50.603362 wizata-dsapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-12 18:24:50.611252 wizata-dsapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-04-12 18:24:46.000000 wizata-dsapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:24:50.579023 wizata-dsapi-0.1.2/wizata_dsapi/
+-rw-rw-rw-   0        0        0      679 2023-04-12 18:24:46.000000 wizata-dsapi-0.1.2/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.1.2/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.2/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     1856 2023-04-03 19:42:17.000000 wizata-dsapi-0.1.2/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.1.2/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    13455 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.2/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3555 2023-04-05 21:53:34.000000 wizata-dsapi-0.1.2/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     5447 2023-04-05 21:53:34.000000 wizata-dsapi-0.1.2/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-04-05 19:26:47.000000 wizata-dsapi-0.1.2/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.2/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0     9756 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.2/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     6914 2023-04-03 19:42:17.000000 wizata-dsapi-0.1.2/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     2003 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.2/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2235 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.2/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.2/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    33193 2023-04-08 18:17:48.000000 wizata-dsapi-0.1.2/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:24:50.603362 wizata-dsapi-0.1.2/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-04-12 18:24:50.000000 wizata-dsapi-0.1.2/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-04-12 18:24:50.000000 wizata-dsapi-0.1.2/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 18:24:50.000000 wizata-dsapi-0.1.2/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-04-12 18:24:50.000000 wizata-dsapi-0.1.2/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 18:24:50.000000 wizata-dsapi-0.1.2/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.1/LICENSE.txt` & `wizata-dsapi-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/setup.py` & `wizata-dsapi-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.1',
+    version='0.1.2',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.2/wizata_dsapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .plot import Plot
 from .mlmodel import MLModel
 from .request import Request
 from .execution import Execution
 from .experiment import Experiment
 from .ds_dataframe import DSDataFrame
 from .script import Script
+from .template import Template
+from .twinregistration import TwinRegistration
 
 # Api
 from .wizata_dsapi_client import api
 from .wizata_dsapi_client import WizataDSAPIClient
 from .dataframe_toolkit import df_to_json, df_to_csv, df_from_json, df_from_csv
 from .model_toolkit import predict
```

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.2/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.2/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.2/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.2/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.2/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.2/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.2/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.2/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.2/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/request.py` & `wizata-dsapi-0.1.2/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/script.py` & `wizata-dsapi-0.1.2/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/template.py` & `wizata-dsapi-0.1.2/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.2/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.2/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.2/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.1/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.2/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

