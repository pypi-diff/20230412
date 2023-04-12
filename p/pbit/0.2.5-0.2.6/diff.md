# Comparing `tmp/pbit-0.2.5.tar.gz` & `tmp/pbit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.2.5.tar", last modified: Wed Apr 12 02:20:58 2023, max compression
+gzip compressed data, was "pbit-0.2.6.tar", last modified: Wed Apr 12 02:25:18 2023, max compression
```

## Comparing `pbit-0.2.5.tar` & `pbit-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.626666 pbit-0.2.5/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-12 02:20:58.624672 pbit-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.5/README.md
--rw-rw-rw-   0        0        0      518 2023-04-12 02:20:32.000000 pbit-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 02:20:58.626666 pbit-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.575802 pbit-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.583783 pbit-0.2.5/src/pbit/
--rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.5/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.623685 pbit-0.2.5/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.5/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.5/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.5/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.5/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.5/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.5/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.5/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     6731 2023-04-12 02:20:32.000000 pbit-0.2.5/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.5/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.607717 pbit-0.2.5/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.586870 pbit-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-04-12 02:25:18.568714 pbit-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.6/README.md
+-rw-rw-rw-   0        0        0      518 2023-04-12 02:24:56.000000 pbit-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:25:18.587887 pbit-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.492756 pbit-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.504831 pbit-0.2.6/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.6/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.566720 pbit-0.2.6/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14167 2023-04-12 02:24:48.000000 pbit-0.2.6/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.6/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.6/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.6/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.6/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.6/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.6/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     6731 2023-04-12 02:20:32.000000 pbit-0.2.6/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.6/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:18.540415 pbit-0.2.6/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-12 02:25:18.000000 pbit-0.2.6/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.2.5/LICENSE` & `pbit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/pyproject.toml` & `pbit-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.2.5/src/pbit/__init__.py` & `pbit-0.2.6/src/pbit/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/src/pbit/datamodelschema/__init__.py` & `pbit-0.2.6/src/pbit/datamodelschema/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,31 +463,31 @@
 
 		self.relationships = []
 		self.tables = []
 		self.query_groups = []
 
 		if "relationships" in ref_model_data:
 			rel_list = ref_model_data["relationships"]
-			assert rel_list
+			assert rel_list != None
 			for relationship_data in rel_list:
 				relationship = self.new_relationship("", "", "")
 				relationship.load(relationship_data)
 			ref_model_data["relationships"] = []
 
 		if "tables" in ref_model_data:
 			tab_list = ref_model_data["tables"]
-			assert tab_list
+			assert tab_list != None
 			for i , table_data in enumerate(tab_list):
 				table = self.new_table("")
 				table.load(table_data)
 			# ref_model_data["tables"] = [get_default_table()]
 
 		if "queryGroups" in ref_model_data and ref_model_data["queryGroups"] != None:
 			ref_groups = ref_model_data["queryGroups"]
-			assert ref_groups
+			assert ref_groups != None
 			for query_group_data in ref_groups:
 				self.query_groups.append(query_group_data["folder"])
 			ref_model_data["queryGroups"] = None
 
 	def dump(self) -> DataModelSchemaData:
 		data_model_schema = deepcopy(self.reference_data)
```

### Comparing `pbit-0.2.5/src/pbit/datamodelschema/column.py` & `pbit-0.2.6/src/pbit/datamodelschema/column.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/src/pbit/datamodelschema/measure.py` & `pbit-0.2.6/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/src/pbit/datamodelschema/partition.py` & `pbit-0.2.6/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/src/pbit/datamodelschema/powerquery.py` & `pbit-0.2.6/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/src/pbit/datamodelschema/relationship.py` & `pbit-0.2.6/src/pbit/datamodelschema/relationship.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/src/pbit/datamodelschema/table.py` & `pbit-0.2.6/src/pbit/datamodelschema/table.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.5/src/pbit.egg-info/SOURCES.txt` & `pbit-0.2.6/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

