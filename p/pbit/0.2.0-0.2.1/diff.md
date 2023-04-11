# Comparing `tmp/pbit-0.2.0.tar.gz` & `tmp/pbit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.2.0.tar", last modified: Tue Apr 11 23:26:24 2023, max compression
+gzip compressed data, was "pbit-0.2.1.tar", last modified: Tue Apr 11 23:49:47 2023, max compression
```

## Comparing `pbit-0.2.0.tar` & `pbit-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.206083 pbit-0.2.0/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-11 23:26:24.205086 pbit-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.0/README.md
--rw-rw-rw-   0        0        0      518 2023-04-11 23:25:27.000000 pbit-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 23:26:24.206083 pbit-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.150488 pbit-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.161464 pbit-0.2.0/src/pbit/
--rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.0/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.203098 pbit-0.2.0/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.0/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     6322 2023-04-11 23:21:11.000000 pbit-0.2.0/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.0/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.0/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.0/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.0/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.0/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     5148 2023-04-11 22:44:48.000000 pbit-0.2.0/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.0/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.186401 pbit-0.2.0/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 23:49:47.648467 pbit-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-04-11 23:49:47.647456 pbit-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.1/README.md
+-rw-rw-rw-   0        0        0      518 2023-04-11 23:49:21.000000 pbit-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 23:49:47.648467 pbit-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 23:49:47.574497 pbit-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 23:49:47.597442 pbit-0.2.1/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.1/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:49:47.644465 pbit-0.2.1/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.1/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     6028 2023-04-11 23:48:19.000000 pbit-0.2.1/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.1/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.1/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.1/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.1/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.1/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     6557 2023-04-11 23:48:19.000000 pbit-0.2.1/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.1/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:49:47.624528 pbit-0.2.1/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-04-11 23:49:47.000000 pbit-0.2.1/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-11 23:49:47.000000 pbit-0.2.1/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 23:49:47.000000 pbit-0.2.1/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 23:49:47.000000 pbit-0.2.1/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 23:49:47.000000 pbit-0.2.1/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.2.0/LICENSE` & `pbit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.2.0/pyproject.toml` & `pbit-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.2.0/src/pbit/__init__.py` & `pbit-0.2.1/src/pbit/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.0/src/pbit/datamodelschema/__init__.py` & `pbit-0.2.1/src/pbit/datamodelschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.0/src/pbit/datamodelschema/column.py` & `pbit-0.2.1/src/pbit/datamodelschema/column.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,24 +70,19 @@
 				{
 					"name": "SummarizationSetBy",
 					"value": "Automatic"
 				}
 			]
 		}
 
-	def set_as_bin(self, target_table_name: str, target_column_name: str, increment: float, bin_name: str | None = None, data_type: DaxType="double"):
-		final_name: str = ""
-		if bin_name:
-			final_name = bin_name
-		else:
-			final_name = target_column_name + "_bin"
-		
+	def set_as_bin(self, target_table_name: str, target_column_name: str, increment: float, bin_name: str, data_type: DaxType="double"):
+
 		reference_data: Any = {
 			"type": "calculated",
-			"name": final_name,
+			"name": bin_name,
 			"dataType": data_type,
 			"isDataTypeInferred": True,
 			"expression": [
 				"IF(",
 				f"\tISBLANK('{target_table_name}'[{target_column_name}]),",
 				"\tBLANK(),",
 				"\tIF(",
@@ -152,28 +147,24 @@
 
 	def set_as_normalized(
 		self,
 		numerator_table_name: str, 
 		numerator_column_name: str, 
 		denominator_table_name: str, 
 		denominator_column_name: str,
-		name: None | str = None,
+		name: str,
 		data_type: DaxType="double",
 		summarize_by: SummaryType="sum"
 	): 
-		final_name: str = ""
-		if name:
-			final_name = name
-		else:
-			final_name = numerator_column_name+"_per_"+denominator_column_name
+
 		dax = f"{numerator_table_name}[{numerator_column_name}] / {denominator_table_name}[{denominator_column_name}]"
 		if denominator_table_name != numerator_table_name:
 			dax = f"{numerator_table_name}[{numerator_column_name}] / RELATED({denominator_table_name}[{denominator_column_name}])"
 
-		self.set_dax(dax, final_name, data_type,  summarize_by)
+		self.set_dax(dax, name, data_type,  summarize_by)
 
 	def set_dax(self, dax: str, name: str, data_type: DaxType="double", summarize_by: SummaryType="sum"):
 		ref_data: Any = {
             "type": "calculated",
             "name": name,
             "dataType": data_type,
             "isDataTypeInferred": True,
```

### Comparing `pbit-0.2.0/src/pbit/datamodelschema/measure.py` & `pbit-0.2.1/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.0/src/pbit/datamodelschema/partition.py` & `pbit-0.2.1/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.0/src/pbit/datamodelschema/powerquery.py` & `pbit-0.2.1/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.0/src/pbit/datamodelschema/relationship.py` & `pbit-0.2.1/src/pbit/datamodelschema/relationship.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.0/src/pbit/datamodelschema/table.py` & `pbit-0.2.1/src/pbit/datamodelschema/table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
 import pandas as pd
 from .dax import DaxType
-from .column import Column, ColumnData 
+from .column import Column, ColumnData, SummaryType
 from .partition import Partition, PartitionData
 from .measure import Measure, MeasureData
 from .typeholder import AnnotationData
 from .powerquery import MType
 
 class HierarchyLevelData(TypedDict):
 	name: str
@@ -113,14 +113,21 @@
 		if name == "":
 			name = self.name
 
 		partition = Partition(name, language, query_group)
 		self.partitions.append(partition)
 		return partition
 
+	def get_if_column_exists(self, name: str) -> bool:
+		for column in self.columns:
+			# print(name, " =? ", column.name)
+			if column.name == name:
+				return True
+		return False
+
 	def get_column_by_name(self, name: str) -> Column:
 		final_column: Column | None = None
 		# print("column count: ", len(self.columns))
 		for column in self.columns:
 			# print(name, " =? ", column.name)
 			if column.name == name:
 				final_column = column
@@ -133,27 +140,61 @@
 		self,
 		name: str,
 		data_type: DaxType,
 		source_column: None | str = None
 	) -> Column:
 		if source_column == None and name != "":
 			source_column = name
+
+		assert self.get_if_column_exists(name) == False, f"column with name {name} in table {self.name} already exists!"
+
 		column = Column(name, data_type, source_column)
 		self.columns.append(column)
 		return column
 
-	def new_bin(self, target_column_name: str, increment: float, target_table_name: str | None = None,  bin_name: str | None = None, data_type: DaxType ="double"):
+	def new_bin(self, target_column_name: str, increment: float, target_table_name: str | None = None,  bin_name: str | None = None, data_type: DaxType ="double") -> Column:
 		final_table_name = ""
 		if target_table_name:
 			final_table_name = target_table_name
 		else:
 			final_table_name = self.name
 
-		column = self.new_column("", data_type)
+		column = self.new_column(final_table_name, data_type)
 		column.set_as_bin(final_table_name, target_column_name, increment, bin_name, data_type)
+		return column
+
+	def new_dax_column(self, dax: str, name: str, data_type: DaxType="double", summarize_by: SummaryType="sum") -> Column:
+		column = self.new_column(name, data_type)
+		column.set_dax(dax, name, data_type, summarize_by)
+		return column
+	
+	def new_normalized_column(
+		self,
+		numerator_column_name: str,  
+		denominator_column_name: str,
+		denominator_table_name: None | str = None,
+		name: None | str = None,
+		data_type: DaxType="double",
+		summarize_by: SummaryType="sum"
+	):
+		final_name: str = ""
+		if name:
+			final_name = name
+		else:
+			final_name = numerator_column_name+"_per_"+denominator_column_name
+		
+		final_denominator_table_name: str = ""
+		if denominator_table_name == None:
+			final_denominator_table_name = self.name
+		else:
+			final_denominator_table_name = denominator_table_name
+
+		column = self.new_column(final_name, data_type)
+		column.set_as_normalized(self.name, numerator_column_name, final_denominator_table_name, denominator_column_name, final_name, data_type, summarize_by)
+		return column
 
 	def new_measure(self, name: str) -> Measure:
 		measure = Measure(name, "any")
 		self.measures.append(measure)
 		return measure
 
 	def load(self, data: TableData):
```

### Comparing `pbit-0.2.0/src/pbit.egg-info/SOURCES.txt` & `pbit-0.2.1/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

