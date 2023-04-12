# Comparing `tmp/wizata-dsapi-0.0.99.tar.gz` & `tmp/wizata-dsapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.0.99.tar", last modified: Wed Mar 15 21:02:15 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.1.tar", last modified: Wed Apr 12 17:56:22 2023, max compression
```

## Comparing `wizata-dsapi-0.0.99.tar` & `wizata-dsapi-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 21:02:15.261933 wizata-dsapi-0.0.99/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.0.99/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-03-15 21:02:15.259607 wizata-dsapi-0.0.99/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-03-03 13:11:49.000000 wizata-dsapi-0.0.99/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-15 21:02:15.261933 wizata-dsapi-0.0.99/setup.cfg
--rw-rw-rw-   0        0        0     1213 2023-03-15 21:02:11.000000 wizata-dsapi-0.0.99/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-15 21:02:15.210656 wizata-dsapi-0.0.99/wizata_dsapi/
--rw-rw-rw-   0        0        0      430 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0      702 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     3122 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0     4273 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     2644 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1313 2023-03-10 09:04:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0     1010 2023-03-15 21:02:11.000000 wizata-dsapi-0.0.99/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0     7229 2023-03-10 09:04:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     3166 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0      487 2023-03-06 18:04:49.000000 wizata-dsapi-0.0.99/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    13837 2023-03-15 13:29:01.000000 wizata-dsapi-0.0.99/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-03-15 21:02:15.256776 wizata-dsapi-0.0.99/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-03-15 21:02:15.000000 wizata-dsapi-0.0.99/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-03-15 21:02:15.000000 wizata-dsapi-0.0.99/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 21:02:15.000000 wizata-dsapi-0.0.99/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      538 2023-03-15 21:02:15.000000 wizata-dsapi-0.0.99/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-15 21:02:15.000000 wizata-dsapi-0.0.99/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 17:56:22.955187 wizata-dsapi-0.1.1/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-04-12 17:56:22.953980 wizata-dsapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:56:22.955187 wizata-dsapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:56:22.896469 wizata-dsapi-0.1.1/wizata_dsapi/
+-rw-rw-rw-   0        0        0      599 2023-04-05 20:20:01.000000 wizata-dsapi-0.1.1/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.1.1/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.1/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     1856 2023-04-03 19:42:17.000000 wizata-dsapi-0.1.1/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.1.1/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    13455 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.1/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3555 2023-04-05 21:53:34.000000 wizata-dsapi-0.1.1/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     5447 2023-04-05 21:53:34.000000 wizata-dsapi-0.1.1/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-04-05 19:26:47.000000 wizata-dsapi-0.1.1/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.1/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0     9756 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.1/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     6914 2023-04-03 19:42:17.000000 wizata-dsapi-0.1.1/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     2003 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.1/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2235 2023-04-12 17:51:36.000000 wizata-dsapi-0.1.1/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.1/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    33193 2023-04-08 18:17:48.000000 wizata-dsapi-0.1.1/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:56:22.949667 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 17:56:22.000000 wizata-dsapi-0.1.1/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.0.99/LICENSE.txt` & `wizata-dsapi-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.0.99/setup.py` & `wizata-dsapi-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.0.99',
+    version='0.1.1',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
         'numpy==1.23.5',
         'matplotlib==3.7.1',
         'protobuf==3.19.6',
         "tensorflow==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "tensorflow-macos==2.11; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        "tensorflow-macos==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
         "keras==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "keras==2.11; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        "keras==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
         'tensorflow_probability==0.15.0',
         'scikit-learn==1.2.2',
         'plotly==5.13.1',
         'adtk==0.6.2',
         'scipy==1.10.1',
         'xgboost==1.7.4',
         'joblib==1.2.0',
@@ -28,10 +28,11 @@
         'setuptools==67.6.0',
         'explainerdashboard==0.4.2.1',
         'ipywidgets==8.0.4',
         'kaleido==0.2.1',
         'pytest==7.2.2',
         'pytest-cov==4.0.0',
         'shapely==2.0.1',
-        'pyodbc==4.0.35'
+        'pyodbc==4.0.35',
+        'msal==1.21.0'
     ]
 )
```

### Comparing `wizata-dsapi-0.0.99/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.1/wizata_dsapi/dataframe_toolkit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,94 @@
 import pandas
 import io
 import datetime
 
 
-class DataFrameToolkit:
-
-    @classmethod
-    def convert_to_csv(cls, df: pandas.DataFrame) -> bytes:
-        """
-        Convert the DataFrame to a strongly formatted CSV.
-        :param df: pandas DataFrame compatible with Wizata standards.
-        :return: bytes containing the full CSV file.
-        """
-        b_buf = io.BytesIO()
-
-        df.to_csv(b_buf,
-                  date_format="%Y-%m-%d-%H-%M-%S-%f",
-                  sep=",",
-                  decimal=".",
-                  encoding="utf-8")
-
-        b_buf.seek(0)
-        return b_buf.read()
-
-    @classmethod
-    def read_from_csv(cls, b_data: bytes) -> pandas.DataFrame:
-        """
-        Convert the bytes to a pandas.DataFrame.
-        :param b_data: bytes representing a CSV file.
-        :return: pandas DataFrame formatted.
-        """
-        b_buf = io.BytesIO(b_data)
-
-        date_parser = lambda x: datetime.datetime.strptime(x, "%Y-%m-%d-%H-%M-%S-%f")
-        df = pandas.read_csv(b_buf,
-                             index_col='Timestamp',
-                             parse_dates=['Timestamp'],
-                             date_parser=date_parser,
-                             sep=",",
-                             decimal=".",
-                             encoding="utf-8")
-
-        return df
-
-    @classmethod
-    def convert_from_json(cls, json):
-        df = pandas.DataFrame.from_dict(json, orient='columns')
-        df = df.set_index('timestamp')
-        return df
-
-    @classmethod
-    def convert_to_json(cls, df: pandas.DataFrame):
-        df_json = {"timestamp": list(df.index)}
-        for col in list(df.columns):
-            if col != 'Timestamp':
-                df_json[col] = list(df[col].values.astype(float))
-            else:
-                df_json[col] = list(df[col].values)
-        return df_json
+def df_to_csv(df: pandas.DataFrame) -> bytes:
+    """
+    Convert the DataFrame to a strongly formatted CSV.
+    :param df: pandas DataFrame compatible with Wizata standards.
+    :return: bytes containing the full CSV file.
+    """
+    b_buf = io.BytesIO()
+
+    df.to_csv(b_buf,
+              date_format="%Y-%m-%d-%H-%M-%S-%f",
+              sep=",",
+              decimal=".",
+              encoding="utf-8")
+
+    b_buf.seek(0)
+    return b_buf.read()
+
+
+def df_from_csv(b_data: bytes) -> pandas.DataFrame:
+    """
+    Convert the bytes to a pandas.DataFrame.
+    :param b_data: bytes representing a CSV file.
+    :return: pandas DataFrame formatted.
+    """
+    b_buf = io.BytesIO(b_data)
+
+    df = pandas.read_csv(b_buf,
+                         sep=",",
+                         decimal=".",
+                         encoding="utf-8")
+
+    # detect timestamp column
+    if "timestamp" in df.columns:
+        df = df.rename(columns={'timestamp': 'Timestamp'})
+    if "Timestamp" not in df.columns:
+        raise ValueError('Cannot read dataframe as no Timestamp columns exists.')
+
+    # detect timestamp type
+    if df['Timestamp'].dtypes == 'int64':
+        df['Timestamp'] = pandas.to_datetime(df['Timestamp'], unit="ms")
+    elif df['Timestamp'].dtypes == 'object':
+        df['Timestamp'] = df['Timestamp'].apply(lambda _: datetime.datetime.strptime(_, "%Y-%m-%d-%H-%M-%S-%f"))
+
+    df = df.set_index('Timestamp')
+    df.rename_axis("sensorId", axis="columns", inplace=True)
+
+    return df
+
+
+def df_from_json(json):
+    """
+    Convert a dictionary dataframe using JSON convention into a panda Dataframe.
+
+    Dataframe must contain a timestamp column and be compatible to float data types.
+
+    :param json: JSON formatted dataframe.
+    :return: panda Dataframe
+    """
+    df = pandas.DataFrame.from_dict(json, orient='columns')
+    df = df.set_index('Timestamp')
+
+    if df.index.dtype == 'int64':
+        df.index = [datetime.datetime.fromtimestamp(i) for i in (df.index / 1000).astype(int)]
+        df.index.name = 'Timestamp'
+    if not isinstance(df.index, pandas.DatetimeIndex):
+        raise TypeError("Unexpected type {0}".format(df.index))
+
+    df.rename_axis("sensorId", axis="columns", inplace=True)
+    return df
+
+
+def df_to_json(df: pandas.DataFrame):
+    """
+    Convert a panda Dataframe to a JSON compatible dictionary.
+
+    Dataframe must be compatible to Wizata format using Timestamp index and float data types.
+
+    :param df: panda Dataframe to convert.
+    :return: dictionary representing JSON compatible dataframe.
+    """
+    df_json = {
+        "Timestamp": list(df.index)
+    }
+    for col in list(df.columns):
+        if col != 'Timestamp':
+            df_json[col] = list(df[col].values.astype(float))
+        else:
+            df_json[col] = list(df[col].values)
+    return df_json
```

### Comparing `wizata-dsapi-0.0.99/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.1/wizata_dsapi/dsapi_json_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json
+import uuid
 import pandas
 import time
 
 from .mlmodel import MLModel
 from .script import Script
 from .plot import Plot
 from .wizard_function import WizardStep, WizardFunction
 from .ds_dataframe import DSDataFrame
 
 
 class DSAPIEncoder(json.JSONEncoder):
 
     def default(self, obj):
+        if isinstance(obj, uuid.UUID):
+            return str(obj)
         if isinstance(obj, MLModel):
             json_obj = {
                 "id": str(obj.model_id),
                 "status": str(obj.status),
                 "generatedById": str(obj.generatedById),
                 "input_columns": list(obj.input_columns),
                 "output_columns": list(obj.output_columns),
@@ -45,24 +48,15 @@
             json_obj = {
                 "id": str(obj.df_id)
             }
             if obj.generatedById is not None:
                 json_obj["generatedById"] = str(obj.generatedById)
             return json_obj
         if isinstance(obj, Plot):
-            json_obj = {
-                "id": str(obj.plot_id)
-            }
-            if obj.name is not None:
-                json_obj["name"] = obj.name
-            if obj.figure is not None:
-                json_obj["figure"] = obj.figure
-            if obj.experiment_id is not None:
-                json_obj["experiment_id"] = obj.experiment_id
-            return json_obj
+            return obj.to_json()
         if isinstance(obj, pandas.Timestamp):
             return int(time.mktime(obj.timetuple()) * 1000)
         if isinstance(obj, WizardStep):
             json_obj = {
                 "id": obj.step_id,
                 "order": obj.order
             }
```

### Comparing `wizata-dsapi-0.0.99/wizata_dsapi/request.py` & `wizata-dsapi-0.1.1/wizata_dsapi/request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,58 @@
 import uuid
 from datetime import datetime, timedelta
 
 
 class Request:
+    """
+    A Request to fetch dataframes from Wizata App.
 
-    def __init__(self):
+    To execute the request please use a DS API client.
+
+    :ivar equipments: List of Equipments containing Digital Twin item and datapoints to fetch.
+    :ivar start: Datetime defining beginning of period.
+    :ivar end: Datetime defining end of period.
+    :ivar aggregation: Aggregation method to fetch, accept "mean" and "stddev".
+    :ivar interval: Interval in seconds between each aggregation.
+    :ivar filters: Filter to apply on the query (not yet fully implemented).
+    :ivar connections: Connections rules between equipment to align data in time (not yet fully implemented).
+    :ivar null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
+    """
+
+    def __init__(self,
+                 datapoints=None,
+                 start=None,
+                 end=None,
+                 agg_method='mean',
+                 interval=None,
+                 null='drop'):
         self.function = None
         self.equipments = []
-        self.start = None
-        self.end = None
-        self.aggregation = None
-        self.interval = None
+        if datapoints is not None:
+            self.add_datapoints(datapoints)
+
+        self.start = start
+        self.end = end
+
+        self.aggregation = agg_method
+        if interval is not None:
+            self.interval = int(interval) / 1000
+
         self.filters = None
         self.on_off_sensor = None
         self.restart_time = None
         self.sensitivity = None
         self.dataframe = None
         self.extra_data = None
         self.target_feat = None
         self.connections = None
         self.name = None
 
+        self.null = null
+
     def prepare(self):
         """
         prepare a dict JSON compatible only for the QUERY part of the request.
 
         :return: a dict JSON compatible
         """
         query = {}
@@ -42,70 +70,93 @@
         if self.aggregation is not None and self.interval:
             query["aggregations"] = {
                 "agg_method": self.aggregation,
                 "interval": self.interval * 1000
             }
         else:
             raise KeyError("Missing aggregations information inside the request")
+        if self.null is not None and self.null != 'drop':
+            query['null'] = self.null
         return query
 
     def __format_date(self, dt_to_format):
         if isinstance(dt_to_format, datetime):
             millisec = dt_to_format.timestamp() * 1000
             return int(millisec)
         else:
             raise TypeError("date is not a valid datetime")
 
     # add datapoints without any reference to an equipment
-    def add_datapoints(self, datapoints, shift=0):
+    def add_datapoints(self, datapoints, shift: int = 0):
+        """
+        Add datapoints to fetch without defining its equipments.
+        :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
+        :param shift: Shift to apply in seconds on timestamp, by default 0.
+        """
         self.equipments.append({
             "id": None,
             "datapoints": list(datapoints),
             "shift": str(shift) + "s"
         })
 
     def add_equipment(self, equipment_id: uuid.UUID, datapoints, shift=0):
+        """
+        Add datapoints to fetch with a Digital Twin ID identification.
+        :param equipment_id: UUID of the Digital Twin ID to which the datapoints are linked.
+        :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
+        :param shift: Shift to apply in seconds on timestamp, by default 0.
+        """
         if not isinstance(equipment_id, uuid.UUID):
             raise TypeError("equipment_id must be of type uuid.UUID")
         for equipment in self.equipments:
             if "id" in equipment.keys() and equipment["id"] == str(equipment_id):
                 raise ValueError("equipment_id is already in the request please remove it before adding datapoints.")
         self.equipments.append({
             "id": str(equipment_id),
             "datapoints": list(datapoints),
             "shift": str(shift) + "s"
         })
 
     # attempt to remove equipment from the query if exists
     def remove_equipment(self, equipment_id: uuid.UUID):
+        """
+        Remove an equipment from the list including all its listed datapoints.
+        :param equipment_id: UUID of the Digital Twin item.
+        """
         if equipment_id is not None and not isinstance(equipment_id, uuid.UUID):
             raise TypeError("equipment_id must be None or of type uuid.UUID")
         found = None
         for equipment in self.equipments:
             if "id" in equipment.keys() and equipment["id"] == str(equipment_id):
                 found = equipment
         if found is not None:
             self.equipments.remove(equipment)
 
     def set_aggregation(self, method, interval):
+        """
+        Specifies aggregation properties
+        :param method: 'mean' or 'stddev'
+        :param interval: interval in ms (will be stored in seconds)
+        """
         self.aggregation = method
-        self.interval = int(interval)
+        if interval is not None:
+            self.interval = int(interval) / 1000
 
     def to_json(self):
         """
         convert to a dict JSON compatible for all properties. For query only, use prepare().
 
         :return: a dict JSON compatible
         """
         obj = self.prepare()
         if self.target_feat is not None:
             obj["target_feat"] = {
                 "sensor": self.target_feat["sensor"],
                 "operator": self.target_feat["operator"],
-                "treshold": self.target_feat["treshold"]
+                "threshold": self.target_feat["threshold"]
             }
         if self.on_off_sensor is not None and self.restart_time is not None:
             obj["restart_filter"] = {
                 "on_off_sensor": self.on_off_sensor,
                 "stop_restart_time": self.restart_time
             }
 
@@ -114,14 +165,19 @@
 
         if self.extra_data is not None:
             obj["extra_data"] = self.extra_data
 
         return obj
 
     def from_json(self, json_data):
+        """
+        load a request based on dict from a JSON file.
+
+        :param json_data: JSON formatted dictionnary object representing a query.
+        """
         if "name" in json_data.keys():
             self.name = json_data["name"]
 
         if "equipments_list" not in json_data.keys():
             raise KeyError("No 'twin unit' nor 'data points' selected please select some and re-try.")
         self.equipments = json_data["equipments_list"]
 
@@ -149,14 +205,17 @@
 
         if "filters" in json_data.keys():
             self.filters = json_data["filters"]
 
         if "connections" in json_data.keys():
             self.connections = json_data["connections"]
 
+        if "null" in json_data.keys():
+            self.null = json_data["null"]
+
         if "target_feat" in json_data.keys():
             self.target_feat = json_data["target_feat"]
             if "sensor" not in self.target_feat.keys():
                 raise KeyError("No 'sensor' have been declared inside the target feature, this is a technical error.")
             if "operator" not in self.target_feat.keys():
                 raise KeyError("No 'operator' have been declared inside the target feature, this is a technical error.")
             if "threshold" not in self.target_feat.keys():
```

### Comparing `wizata-dsapi-0.0.99/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.1/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE.txt
 README.rst
 setup.py
 wizata_dsapi/__init__.py
+wizata_dsapi/api_dto.py
 wizata_dsapi/dataframe_toolkit.py
 wizata_dsapi/ds_dataframe.py
 wizata_dsapi/dsapi_json_encoder.py
 wizata_dsapi/execution.py
+wizata_dsapi/experiment.py
 wizata_dsapi/mlmodel.py
 wizata_dsapi/model_toolkit.py
 wizata_dsapi/plot.py
 wizata_dsapi/request.py
 wizata_dsapi/script.py
+wizata_dsapi/template.py
+wizata_dsapi/twinregistration.py
 wizata_dsapi/wizard_function.py
 wizata_dsapi/wizata_dsapi_client.py
 wizata_dsapi.egg-info/PKG-INFO
 wizata_dsapi.egg-info/SOURCES.txt
 wizata_dsapi.egg-info/dependency_links.txt
 wizata_dsapi.egg-info/requires.txt
 wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.0.99/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.1/wizata_dsapi.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 explainerdashboard==0.4.2.1
 ipywidgets==8.0.4
 kaleido==0.2.1
 pytest==7.2.2
 pytest-cov==4.0.0
 shapely==2.0.1
 pyodbc==4.0.35
+msal==1.21.0
 
 [:sys_platform != "darwin" or platform_machine != "arm64"]
 tensorflow==2.7
 keras==2.7
 
 [:sys_platform == "darwin" and platform_machine == "arm64"]
-tensorflow-macos==2.11
-keras==2.11
+tensorflow-macos==2.11.0
+keras==2.11.0
```

