# Comparing `tmp/kaskada-0.1.2.tar.gz` & `tmp/kaskada-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.1.2.tar", max compression
+gzip compressed data, was "kaskada-0.1.3.tar", max compression
```

## Comparing `kaskada-0.1.2.tar` & `kaskada-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,25 @@
--rw-r--r--   0        0        0     1097 2023-03-14 21:18:57.392670 kaskada-0.1.2/README.md
--rw-r--r--   0        0        0     3387 2023-03-28 19:56:58.816253 kaskada-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7078 2023-03-14 21:18:57.392951 kaskada-0.1.2/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-03-14 21:18:57.393077 kaskada-0.1.2/src/fenlmagic/utils.py
--rw-r--r--   0        0        0     1179 2023-03-20 22:45:18.890752 kaskada-0.1.2/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0     6381 2023-03-14 21:18:57.393970 kaskada-0.1.2/src/kaskada/api/release.py
--rw-r--r--   0        0        0     8961 2023-03-20 22:45:18.891097 kaskada-0.1.2/src/kaskada/api/session.py
--rw-r--r--   0        0        0     5688 2023-03-13 21:07:55.911920 kaskada-0.1.2/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-02-16 15:04:32.259854 kaskada-0.1.2/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-02-16 15:04:32.259950 kaskada-0.1.2/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-03-14 21:18:57.394533 kaskada-0.1.2/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7318 2023-02-22 15:54:38.099392 kaskada-0.1.2/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0     9380 2023-03-20 22:45:18.891455 kaskada-0.1.2/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0    13473 2023-03-28 16:38:34.337662 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.337864 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    16889 2023-03-28 16:38:34.337967 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0     6628 2023-03-28 16:38:34.337668 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     5994 2023-03-28 16:38:34.336654 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-03-28 16:38:34.337527 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     6210 2023-03-28 16:38:34.337662 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.337893 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     3526 2023-03-28 16:38:34.337913 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.338429 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     6288 2023-03-28 16:38:34.338101 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-03-28 16:38:34.338253 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0    16522 2023-03-28 16:38:34.338354 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-03-28 16:38:34.338379 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1846 2023-03-28 16:38:34.338767 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.338775 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    21703 2023-03-28 16:38:34.338563 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.338652 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     4975 2023-03-28 16:38:34.338898 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-03-28 16:38:34.338783 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0    16745 2023-03-28 16:38:34.339392 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-03-28 16:38:34.339150 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4886 2023-03-28 16:38:34.339283 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.339286 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2882 2023-03-28 16:38:34.339627 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.339397 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    17092 2023-03-28 16:38:34.339527 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-03-28 16:38:34.339473 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     6835 2023-03-28 16:38:34.339762 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-03-28 16:38:34.339983 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0    11387 2023-03-28 16:38:34.339855 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-03-28 16:38:34.339858 kaskada-0.1.2/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    26181 2023-03-28 16:38:34.340086 kaskada-0.1.2/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-03-28 16:38:34.340073 kaskada-0.1.2/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     7814 2023-03-14 21:18:57.394688 kaskada-0.1.2/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9224 2023-03-14 21:18:57.394827 kaskada-0.1.2/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-02-16 15:04:32.260683 kaskada-0.1.2/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0     9463 2023-03-20 22:45:22.074597 kaskada-0.1.2/src/kaskada/table.py
--rw-r--r--   0        0        0     6690 2023-03-20 22:45:22.074740 kaskada-0.1.2/src/kaskada/utils.py
--rw-r--r--   0        0        0     4515 2023-02-16 21:15:36.589584 kaskada-0.1.2/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-02-16 15:04:32.261759 kaskada-0.1.2/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-02-16 15:04:32.261899 kaskada-0.1.2/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-02-16 15:04:32.262038 kaskada-0.1.2/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-02-16 15:04:32.262128 kaskada-0.1.2/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     2323 1970-01-01 00:00:00.000000 kaskada-0.1.2/setup.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 kaskada-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-04-11 22:38:35.487057 kaskada-0.1.3/README.md
+-rw-r--r--   0        0        0     3387 2023-04-11 22:38:35.487057 kaskada-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7084 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0     1179 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0     6381 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     8961 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/api/session.py
+-rw-r--r--   0        0        0     5688 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7318 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0     9805 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0     8594 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9232 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10098 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/table.py
+-rw-r--r--   0        0        0     6690 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4515 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     2266 1970-01-01 00:00:00.000000 kaskada-0.1.3/setup.py
+-rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 kaskada-0.1.3/PKG-INFO
```

### Comparing `kaskada-0.1.2/README.md` & `kaskada-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 #### Build the Client
 To build the client: `$ poetry build`
 
 #### Install the Client
 To install the client: `$ pip install dist/*.whl`
 
 #### Open a Jupyter Notebook
-To open a notebook: `$ jupyter notebook`
+To open a notebook: `$ jupyter notebook`
```

### Comparing `kaskada-0.1.2/pyproject.toml` & `kaskada-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.1.2"
+version = "0.1.3"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
```

### Comparing `kaskada-0.1.2/src/fenlmagic/__init__.py` & `kaskada-0.1.3/src/fenlmagic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,29 +135,29 @@
             )
             query_result = QueryResult(expression, resp)
 
             if not dry_run and render_dataframe:
                 # TODO: figure out how to support reading from multiple parquet paths
                 if (
                     len(
-                        query_result.query_response.output_to.object_store.output_paths.paths
+                        query_result.query_response.destination.object_store.output_paths.paths
                     )
                     > 0
                 ):
                     if response_as == query.ResponseType.FILE_TYPE_PARQUET:
                         df = pandas.read_parquet(
-                            query_result.query_response.output_to.object_store.output_paths.paths[
+                            query_result.query_response.destination.object_store.output_paths.paths[
                                 0
                             ],
                             engine="pyarrow",
                         )
                         query_result.set_dataframe(df)
                     elif response_as == query.ResponseType.FILE_TYPE_CSV:
                         df = pandas.read_csv(
-                            query_result.query_response.output_to.object_store.output_paths.paths[
+                            query_result.query_response.destination.object_store.output_paths.paths[
                                 0
                             ],
                         )
                         query_result.set_dataframe(df)
 
             if var is not None:
                 IPython.get_ipython().push({var: query_result})
```

### Comparing `kaskada-0.1.2/src/kaskada/api/api_utils.py` & `kaskada-0.1.3/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/api/release.py` & `kaskada-0.1.3/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/api/session.py` & `kaskada-0.1.3/src/kaskada/api/session.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/client.py` & `kaskada-0.1.3/src/kaskada/client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/formatters.css` & `kaskada-0.1.3/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/formatters.js` & `kaskada-0.1.3/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/formatters.py` & `kaskada-0.1.3/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/formatters_helpers.py` & `kaskada-0.1.3/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/formatters_shared.py` & `kaskada-0.1.3/src/kaskada/formatters_shared.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pprint
 from typing import Optional
 
 import pandas as pd
 from domonic.html import pre, table, td, th, tr
 from domonic.utils import Utils
 
+import kaskada.kaskada.v1alpha.pulsar_pb2 as pulsar_pb
 import kaskada.kaskada.v1alpha.table_service_pb2 as table_pb
 import kaskada.kaskada.v1alpha.view_service_pb2 as view_pb
 
 from .formatters_helpers import (
     appendChildren,
     appendHtmlObjTableRowIfAttrExists,
     convert_fenl_datatype,
@@ -179,18 +180,22 @@
     if obj is not None and obj.HasField("percent"):
         details.appendChild(html_obj_table_row("percent", obj.percent.percent))
     else:
         details.appendChild(html_obj_table_row("None", "(full dataset used for query)"))
     return details
 
 
-def get_table_source_pulsar(obj: table_pb.Table.PulsarSource) -> table:
+def get_table_pulsar_config(obj: pulsar_pb.PulsarConfig) -> table:
     pulsar = table(_class="kda_table")
-    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "protocol_url")
-    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "topic")
+    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "broker_service_url")
+    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "auth_plugin")
+    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "tenant")
+    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "namespace")
+    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "topic_name")
+    appendHtmlObjTableRowIfAttrExists(pulsar, obj, "topic_url")
     return pulsar
 
 
 def get_table_html_and_schema_df(obj: table_pb.Table):
     schema_df = get_schema_dataframe(obj)
     details = table(_class="kda_table")
     appendHtmlObjTableRowIfAttrExists(details, obj, "table_name")
@@ -198,18 +203,21 @@
     appendHtmlObjTableRowIfAttrExists(details, obj, "time_column_name")
     appendHtmlObjTableRowIfAttrExists(details, obj, "grouping_id")
     if obj.HasField("subsort_column_name"):
         details.appendChild(
             html_obj_table_row("subsort_column_name", obj.subsort_column_name.value)
         )
 
-    if hasattr(obj, "table_source") and obj.HasField("table_source"):
-        if hasattr(obj.table_source, "pulsar") and obj.table_source.HasField("pulsar"):
-            pulsar = get_table_source_pulsar(obj.table_source.pulsar)
-            details.appendChild(html_table_row("pulsar", pulsar))
+    if hasattr(obj, "source") and obj.HasField("source"):
+        if hasattr(obj.source, "pulsar") and obj.source.HasField("pulsar"):
+            if hasattr(obj.source.pulsar, "config") and obj.source.pulsar.HasField(
+                "config"
+            ):
+                pulsar = get_table_pulsar_config(obj.source.pulsar.config)
+                details.appendChild(html_table_row("pulsar", pulsar))
 
     appendHtmlObjTableRowIfAttrExists(details, obj, "version")
     if schema_df is not None:
         details.appendChild(html_obj_table_row("schema", "(see Schema tab)"))
     appendTimes(details, obj)
     return details, schema_df
```

### Comparing `kaskada-0.1.2/src/kaskada/materialization.py` & `kaskada-0.1.3/src/kaskada/materialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,39 +81,51 @@
 class PulsarDestination(Destination):
     def __init__(
         self,
         tenant: str = "public",
         namespace: str = "default",
         topic_name: Optional[str] = None,
         broker_service_url: str = "pulsar://127.0.0.1:6650",
+        admin_service_url: str = "http://127.0.0.1:8080",
+        auth_plugin: Optional[str] = None,
+        auth_params: Optional[str] = None,
     ):
         """
         Pulsar Materialization Destination
 
         Args:
             tenant (str): pulsar tenant. defaults to "public".
             namespace (str): pulsar namespace. defaults to "default".
             topic_name (str): final part of topic url. defaults to a randomly generated uuid
             broker_service_url (str): url to connect to pulsar broker. defaults to "pulsar://127.0.0.1:6650"
+            admin_service_url (str): the pulsar admin REST URL for the cluster. defaults to http://127.0.0.1:8080
+            auth_plugin (str): authentication plugin to use. e.g. "org.apache.pulsar.client.impl.auth.AuthenticationToken"
+            auth_params (str): authentication parameters. e.g. "token:xxx"
         """
         self._tenant = tenant
         self._namespace = namespace
         self._topic_name = (
             topic_name
             if topic_name and len(topic_name.strip()) > 0
             else str(uuid.uuid4())
         )
         self._broker_service_url = broker_service_url
+        self._admin_service_url = admin_service_url
+        self._auth_plugin = auth_plugin
+        self._auth_params = auth_params
 
     def to_request(self) -> Dict[str, Any]:
         return {
             "tenant": self._tenant,
             "namespace": self._namespace,
             "topic_name": self._topic_name,
             "broker_service_url": self._broker_service_url,
+            "admin_service_url": self._admin_service_url,
+            "auth_plugin": self._auth_plugin,
+            "auth_params": self._auth_params,
         }
 
 
 class MaterializationView(object):
     def __init__(self, name: str, expression: str):
         """
         Kaskada Materialization View
@@ -146,15 +158,17 @@
             "slice": slice_request,
         }
         if isinstance(destination, ObjectStoreDestination):
             materialization["destination"] = {"object_store": destination.to_request()}
         elif isinstance(destination, RedisDestination):
             materialization["destination"] = {"redis": destination.to_request()}
         elif isinstance(destination, PulsarDestination):
-            materialization["destination"] = {"pulsar": destination.to_request()}
+            materialization["destination"] = {
+                "pulsar": {"config": destination.to_request()}
+            }
         else:
             raise ValueError("invalid destination supplied")
 
         req = material_pb.CreateMaterializationRequest(
             **{"materialization": materialization}
         )
         logger.debug(f"Create Materialization Request: {req}")
```

### Comparing `kaskada-0.1.2/src/kaskada/query.py` & `kaskada-0.1.3/src/kaskada/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
             "data_token_id": self.query.data_token_id,
             "changed_since_time": self.query.changed_since_time,
             "final_result_time": self.query.final_result_time,
             "limits": self.query.limits,
             "result_behavior": self.query.result_behavior,
         }
         if isinstance(self.query, Message):
-            if self.query.HasField("output_to"):
-                result["output_to"] = self.query.output_to
+            if self.query.HasField("destination"):
+                result["destination"] = self.query.destination
 
         return result
 
     def run(
         self,
         data_token=None,
         dry_run=False,
@@ -161,15 +161,15 @@
                     "result_behavior"
                 ] = "RESULT_BEHAVIOR_FINAL_RESULTS_AT_TIME"
         else:
             query_request["result_behavior"] = "RESULT_BEHAVIOR_ALL_RESULTS"
 
         destination_args = {"file_type": response_as.name}
         destination = destinations_pb.ObjectStoreDestination(**destination_args)
-        query_request["output_to"] = {"object_store": destination}
+        query_request["destination"] = {"object_store": destination}
 
         if slice_filter is not None:
             query_request["slice"] = slice_filter.to_request()
 
         in_ipython = kaskada.formatters.in_ipython()
         if in_ipython:
             query_options["stream_metrics"] = True
```

### Comparing `kaskada-0.1.2/src/kaskada/slice_filters.py` & `kaskada-0.1.3/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/table.py` & `kaskada-0.1.3/src/kaskada/table.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,29 @@
 
 
 class TableSource(object):
     pass
 
 
 class PulsarTableSource(TableSource):
-    def __init__(self, protocol_url: str, topic: str):
-        self._protocol_url = protocol_url
-        self._topic = topic
+    def __init__(
+        self,
+        broker_service_url: str,
+        auth_plugin: str,
+        auth_params: str,
+        tenant: str,
+        namespace: str,
+        topic_name: str,
+    ):
+        self._broker_service_url = broker_service_url
+        self._auth_plugin = auth_plugin
+        self._auth_params = auth_params
+        self._tenant = tenant
+        self._namespace = namespace
+        self._topic_name = topic_name
 
 
 def get_table_name(
     table: Union[
         table_pb.Table, table_pb.CreateTableResponse, table_pb.GetTableResponse, str
     ]
 ) -> str:
@@ -156,18 +168,24 @@
             table_args["grouping_id"] = grouping_id
         if subsort_column_name is not None:
             table_args["subsort_column_name"] = wrappers.StringValue(
                 value=subsort_column_name
             )
         if source is not None:
             if isinstance(source, PulsarTableSource):
-                table_args["table_source"] = {
+                table_args["source"] = {
                     "pulsar": {
-                        "protocol_url": source._protocol_url,
-                        "topic": source._topic,
+                        "config": {
+                            "broker_service_url": source._broker_service_url,
+                            "auth_plugin": source._auth_plugin,
+                            "auth_params": source._auth_params,
+                            "tenant": source._tenant,
+                            "namespace": source._namespace,
+                            "topic_name": source._topic_name,
+                        }
                     }
                 }
             else:
                 raise ValueError("invalid table source provided")
 
         req = table_pb.CreateTableRequest(table=table_pb.Table(**table_args))
         logger.debug(f"Create Tables Request: {req}")
```

### Comparing `kaskada-0.1.2/src/kaskada/utils.py` & `kaskada-0.1.3/src/kaskada/utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/src/kaskada/view.py` & `kaskada-0.1.3/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/vendor/validate/validate.proto` & `kaskada-0.1.3/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/vendor/validate/validate_pb2.py` & `kaskada-0.1.3/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/vendor/validate/validate_pb2.pyi` & `kaskada-0.1.3/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.2/setup.py` & `kaskada-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src', 'fenlmagic': 'src/fenlmagic', 'validate': 'vendor/validate'}
 
 packages = \
-['fenlmagic',
- 'kaskada',
- 'kaskada.api',
- 'kaskada.kaskada.v1alpha',
- 'kaskada.kaskada.v2alpha',
- 'validate']
+['fenlmagic', 'kaskada', 'kaskada.api', 'validate']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['certifi>=2022.12.7,<2023.0.0',
  'domonic>=0.9.11,<0.10.0',
@@ -27,17 +22,17 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A client library for the Kaskada time travel machine learning service',
-    'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`',
+    'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `kaskada-0.1.2/PKG-INFO` & `kaskada-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.1.2
+Version: 0.1.3
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -63,7 +63,8 @@
 To build the client: `$ poetry build`
 
 #### Install the Client
 To install the client: `$ pip install dist/*.whl`
 
 #### Open a Jupyter Notebook
 To open a notebook: `$ jupyter notebook`
+
```

