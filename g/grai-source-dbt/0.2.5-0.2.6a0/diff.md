# Comparing `tmp/grai_source_dbt-0.2.5.tar.gz` & `tmp/grai_source_dbt-0.2.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.2.5.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.2.6a0.tar", max compression
```

## Comparing `grai_source_dbt-0.2.5.tar` & `grai_source_dbt-0.2.6a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      735 2023-03-24 13:32:53.677840 grai_source_dbt-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.5/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.5/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     5964 2023-02-28 23:36:16.177785 grai_source_dbt-0.2.5/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      531 2023-02-23 22:53:26.661353 grai_source_dbt-0.2.5/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.5/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.5/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.5/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.5/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     5368 2023-03-23 15:27:47.244520 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.5/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.5/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.5/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.5/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.5/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.5/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.5/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.5/setup.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      741 2023-04-12 16:58:27.208366 grai_source_dbt-0.2.6a0/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.6a0/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     5964 2023-04-10 15:35:17.408407 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      531 2023-04-10 15:35:17.409417 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.6a0/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     5499 2023-04-12 16:56:50.880225 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.6a0/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.6a0/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.6a0/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.6a0/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6a0/setup.py
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6a0/PKG-INFO
```

### Comparing `grai_source_dbt-0.2.5/pyproject.toml` & `grai_source_dbt-0.2.6a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt"
-version = "0.2.5"
+version = "0.2.6-alpha"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt", from = "src" },
 ]
```

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/adapters/adapters.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/base.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/data_tools.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v1.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,20 @@
                 column = self.columns[(table.unique_id, column.name)]
                 edge = self.make_edge(table, column, Constraint("bt"), EdgeTypeLabels.table_to_column)
                 result.append(edge)
 
             # Seeds don't have depends_on and will error without this check.
             if hasattr(table.depends_on, "nodes"):
                 for parent_str in table.depends_on.nodes:
-                    source_node = (
-                        self.node_map[parent_str] if parent_str in self.node_map else self.manifest.sources[parent_str]
-                    )
+                    if parent_str in self.node_map:
+                        source_node = self.node_map[parent_str]
+                    elif parent_str in self.manifest.sources:
+                        source_node = self.manifest.sources[parent_str]
+                    else:
+                        continue
                     edge = self.make_edge(source_node, table, Constraint("dbtm"), EdgeTypeLabels.table_to_table, True)
                     result.append(edge)
 
         for table in self.manifest.sources.values():
             for column in table.columns.values():
                 column = self.columns[(table.unique_id, column.name)]
                 edge = self.make_edge(table, column, Constraint("bt"), EdgeTypeLabels.table_to_column)
```

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v7.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/loaders/v8.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v8.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/grai.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/shared.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/processor.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/processor.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.5/setup.py` & `grai_source_dbt-0.2.6a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ['dbt-artifacts-parser>=0.2.4,<0.3.0',
  'grai-client>=0.2.0,<0.3.0',
  'grai-schemas>=0.1.10,<0.2.0',
  'pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-dbt',
-    'version': '0.2.5',
+    'version': '0.2.6a0',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_dbt-0.2.5/PKG-INFO` & `grai_source_dbt-0.2.6a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt
-Version: 0.2.5
+Version: 0.2.6a0
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

