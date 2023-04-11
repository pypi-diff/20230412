# Comparing `tmp/pbit-0.1.2.tar.gz` & `tmp/pbit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.1.2.tar", last modified: Tue Apr 11 22:54:56 2023, max compression
+gzip compressed data, was "pbit-0.2.0.tar", last modified: Tue Apr 11 23:26:24 2023, max compression
```

## Comparing `pbit-0.1.2.tar` & `pbit-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:54:56.005170 pbit-0.1.2/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-11 22:54:56.003193 pbit-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.1.2/README.md
--rw-rw-rw-   0        0        0      518 2023-04-11 22:54:22.000000 pbit-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 22:54:56.005170 pbit-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.950560 pbit-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.960586 pbit-0.1.2/src/pbit/
--rw-rw-rw-   0        0        0     2330 2023-04-11 22:54:16.000000 pbit-0.1.2/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.998976 pbit-0.1.2/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.1.2/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     4739 2023-04-11 22:44:53.000000 pbit-0.1.2/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.1.2/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.1.2/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.1.2/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.1.2/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.1.2/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     5148 2023-04-11 22:44:48.000000 pbit-0.1.2/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.1.2/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.982555 pbit-0.1.2/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.206083 pbit-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-04-11 23:26:24.205086 pbit-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.0/README.md
+-rw-rw-rw-   0        0        0      518 2023-04-11 23:25:27.000000 pbit-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 23:26:24.206083 pbit-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.150488 pbit-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.161464 pbit-0.2.0/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.0/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.203098 pbit-0.2.0/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.0/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     6322 2023-04-11 23:21:11.000000 pbit-0.2.0/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.0/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.0/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.0/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.0/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.0/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     5148 2023-04-11 22:44:48.000000 pbit-0.2.0/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.0/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:26:24.186401 pbit-0.2.0/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 23:26:24.000000 pbit-0.2.0/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.1.2/LICENSE` & `pbit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.1.2/pyproject.toml` & `pbit-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.1.2/src/pbit/__init__.py` & `pbit-0.2.0/src/pbit/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.2/src/pbit/datamodelschema/__init__.py` & `pbit-0.2.0/src/pbit/datamodelschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.2/src/pbit/datamodelschema/column.py` & `pbit-0.2.0/src/pbit/datamodelschema/table.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,175 +1,194 @@
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
+import pandas as pd
 from .dax import DaxType
+from .column import Column, ColumnData 
+from .partition import Partition, PartitionData
+from .measure import Measure, MeasureData
 from .typeholder import AnnotationData
+from .powerquery import MType
 
-class ColumnAttributeHierarchyData(TypedDict):
-	state: str
+class HierarchyLevelData(TypedDict):
+	name: str
+	ordinal: int
+	column: str
+	linageTag: str
 
-class ColumnData(TypedDict):
-	type: DaxType | None
-	lineageTag: str | None
-	summarizeBy: str | None
-	sourceColumn: str | None
+class HierarchyData(TypedDict):
 	name: str
-	dataType: str
-	formatString: str | None
-	dataCategory: str | None
-	isNameInferred: bool | None
-	expression: str | list[str] | None
-	isDataTypeInferred: bool | None
+	lineageTag: str
+	state: str
+	levels: list[HierarchyLevelData]
+
+class TableData(TypedDict):
+	name: str | None
 	isHidden: bool | None
-	isUnique: bool | None
-	sortByColumn: str | None
-	isKey: bool | None
-	isNullable: bool | None
-	attributeHierarchy: ColumnAttributeHierarchyData
-	annotations: list[AnnotationData] | None
+	isPrivate: bool | None
+	showAsVariationsOnly: bool | None
+	lineageTag: str
+	columns: list[ColumnData]
+	partitions: list[PartitionData]
+	hierarchies: list[HierarchyData] | None
+	annotations: list[AnnotationData]
+	measures: list[MeasureData] | None
 
-class Column():
+class Table():
 	name: str
 	id: str
-	data_type: str
-	source_column: str | None
-	reference_data: ColumnData
+	columns: list[Column]
+	partitions: list[Partition]
+	measures: list[Measure]
+	reference_data: TableData
 
 	def __init__(
 		self,
-		name: str,
-		dataType: str,
-		source_column: str | None = None
+		name: str
 	):
 		self.name = name
 		self.id = str(uuid4())
-		self.data_type = dataType
-		self.source_column = source_column
-		self.reference_data: ColumnData = {
-			"formatString": None,
-			"dataCategory": None,
-			"isNameInferred": None,
-			"expression": None,
-			"isDataTypeInferred": None,
-			"sortByColumn": None,
-			"type": None,
-			"isHidden": None,
-			"isUnique": None,
-			"isKey": None,
-			"isNullable": None,
+		self.columns: list[Column] = []
+		self.partitions: list[Partition] = []
+		self.measures: list[Measure] = []
+		ref_data: Any = {
 			"name": self.name,
-			"dataType": self.data_type,
-			"sourceColumn": self.source_column,
 			"lineageTag": self.id,
-			"summarizeBy": "none",
-			"attributeHierarchy": {
-				"state": "ready"
-			},
-			"annotations": [
-				{
-					"name": "SummarizationSetBy",
-					"value": "Automatic"
-				}
-			]
-		}
-
-	def set_as_bin(self, target_table_name: str, target_column_name: str, increment: float, bin_name: str | None = None, data_type: DaxType="double"):
-		final_name: str = ""
-		if bin_name:
-			final_name = bin_name
-		else:
-			final_name = target_column_name + "_bin"
-		
-		reference_data: Any = {
-			"type": "calculated",
-			"name": final_name,
-			"dataType": data_type,
-			"isDataTypeInferred": True,
-			"expression": [
-				"IF(",
-				f"\tISBLANK('{target_table_name}'[{target_column_name}]),",
-				"\tBLANK(),",
-				"\tIF(",
-				f"\t\t'{target_table_name}'[{target_column_name}] >= 0,",
-				f"\t\tROUNDDOWN('{target_table_name}'[{target_column_name}] / {increment}, 0) * {increment},",
-				f"\t\tROUNDUP('{target_table_name}'[{target_column_name}] / {increment}, 0) * {increment}",
-				"\t)",
-				")"
-			],
-			"lineageTag": self.id,
-			"summarizeBy": "none",
-			"attributeHierarchy": {
-				"state": "ready"
-			},
-			"extendedProperties": [
+			"isHidden": None,
+			"isPrivate": None,
+			"showAsVariationsOnly": None,
+			"hierarchies": None,
+			"columns": [
 				{
-					"type": "json",
-					"name": "GroupingMetadata",
-					"value": {
-						"version": 0,
-						"groupedColumns": [
-							{
-								"Column": {
-									"Expression": {
-										"SourceRef": {
-											"Entity": target_table_name
-										}
-									},
-									"Property": target_column_name
-								}
-							}
-						],
-						"binningMetadata": {
-							"binSize": {
-								"value": 5.0,
-								"unit": 0
-							}
+					"formatString": None,
+					"dataCategory": None,
+					"isNameInferred": None,
+					"expression": None,
+					"isDataTypeInferred": None,
+					"sortByColumn": None,
+					"type": "rowNumber",
+					"name": "RowNumber-2662979B-1795-4F74-8F37-6A1BA8059B61",
+					"dataType": "int64",
+					"isHidden": True,
+					"isUnique": True,
+					"isKey": True,
+					"isNullable": False,
+					"lineageTag": None,
+					"summarizeBy": None,
+					"sourceColumn": None,
+					"annotations": [
+						{
+							"name": "PBI_ResultType",
+							"value": "Table"
 						}
-					}
-				}
+					],
+					"attributeHierarchy": {
+						"state": "ready"
+					},
+				},
 			],
+			"partitions": [],
+			"measures": None,
 			"annotations": [
 				{
-					"name": "GroupingDesignState",
-					"value": "{\"Version\":0,\"Sources\":[{\"Name\":\"p\",\"Entity\":\""
-						+target_table_name+"\"}],\"GroupedColumns\":[{\"Column\":{\"Expression\":{\"SourceRef\":{\"Source\":\"p\"}},\"Property\":\""
-						+target_column_name+"\"}}],\"BinItem\":{\"Expression\":{\"Floor\":{\"Expression\":{\"Column\":{\"Expression\":{\"SourceRef\":{\"Source\":\"p\"}},\"Property\":\""
-						+target_column_name+"\"}},\"Size\":"
-						+str(increment)+"}}}}"
-				},
-				{
-					"name": "SummarizationSetBy",
-					"value": "Automatic"
-				},
-				{
-					"name": "PBI_FormatHint",
-					"value": "{\"isGeneralNumber\":true}"
+					"name": "PBI_ResultType",
+					"value": "Table"
 				}
 			]
 		}
-		self.load(reference_data)
+		self.reference_data: TableData = ref_data
 
-	def load(self, data: ColumnData):
-		self.reference_data = deepcopy(data)
-		self.name = self.reference_data["name"]
-		self.data_type = self.reference_data["dataType"]
-		if "sourceColumn" in self.reference_data:
-			source_column_ref = self.reference_data["sourceColumn"]
-			assert source_column_ref
-			self.source_column = source_column_ref
+	def bind_to_json(
+		self, 
+		relative_json_path: str, 
+		type_dictionary: dict[str, DaxType], 
+		group_name: str | None = None
+	):
+		self.new_partition(group_name).set_to_json_reader(relative_json_path, type_dictionary)
 		
-		if "lineageTag" in self.reference_data:
-			lin_tag = self.reference_data["lineageTag"]
-			assert lin_tag
-			self.id = lin_tag
-
-	def dump(self) -> ColumnData:
-		column_data: ColumnData = deepcopy(self.reference_data)
-		column_data["name"] = self.name
-		column_data["dataType"] = self.data_type
-		if column_data["dataType"] == "any":
-			column_data["dataType"] = "string"
+		# add columns
+		for name, col_type in type_dictionary.items():
+			self.new_column(name, col_type, name)
+
+	def new_partition(self, name="", language="m", query_group: str | None = None) -> Partition:
+		if name == "":
+			name = self.name
+
+		partition = Partition(name, language, query_group)
+		self.partitions.append(partition)
+		return partition
+
+	def get_column_by_name(self, name: str) -> Column:
+		final_column: Column | None = None
+		# print("column count: ", len(self.columns))
+		for column in self.columns:
+			# print(name, " =? ", column.name)
+			if column.name == name:
+				final_column = column
+				break
+
+		assert final_column, f"column {name} does not exist in table {self.name}"
+		return final_column
+
+	def new_column(
+		self,
+		name: str,
+		data_type: DaxType,
+		source_column: None | str = None
+	) -> Column:
+		if source_column == None and name != "":
+			source_column = name
+		column = Column(name, data_type, source_column)
+		self.columns.append(column)
+		return column
+
+	def new_bin(self, target_column_name: str, increment: float, target_table_name: str | None = None,  bin_name: str | None = None, data_type: DaxType ="double"):
+		final_table_name = ""
+		if target_table_name:
+			final_table_name = target_table_name
+		else:
+			final_table_name = self.name
+
+		column = self.new_column("", data_type)
+		column.set_as_bin(final_table_name, target_column_name, increment, bin_name, data_type)
+
+	def new_measure(self, name: str) -> Measure:
+		measure = Measure(name, "any")
+		self.measures.append(measure)
+		return measure
+
+	def load(self, data: TableData):
+		self.reference_data = deepcopy(data)
+		if "name" in self.reference_data:
+			name = self.reference_data["name"]
+			assert name
+			self.name = name
+
+		self.id = self.reference_data["lineageTag"]
+
+		for column_data in self.reference_data["columns"]:
+			column = self.new_column("", "any")
+			column.load(column_data)
+		self.reference_data["columns"] = []
+
+		for partition_data in self.reference_data["partitions"]:
+			partition = self.new_partition("")
+			partition.load(partition_data)
+
+		self.reference_data["partitions"] = []
+
+	def dump(self) -> TableData:
+		table_data: TableData = deepcopy(self.reference_data)
+
+		for column in self.columns:
+			table_data["columns"].append(column.dump())
+
+		for partition in self.partitions:
+			table_data["partitions"].append(partition.dump())
 
-		column_data["sourceColumn"] = self.source_column
-		column_data["lineageTag"] = self.id
+		if len(self.measures) > 0:
+			measure_list = []
+			for measure in self.measures:
+				measure_list.append(measure.dump())
+			table_data["measures"] = measure_list
 
-		return column_data
+		return table_data
```

### Comparing `pbit-0.1.2/src/pbit/datamodelschema/measure.py` & `pbit-0.2.0/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.2/src/pbit/datamodelschema/partition.py` & `pbit-0.2.0/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.2/src/pbit/datamodelschema/powerquery.py` & `pbit-0.2.0/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.2/src/pbit/datamodelschema/relationship.py` & `pbit-0.2.0/src/pbit/datamodelschema/relationship.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.2/src/pbit/datamodelschema/table.py` & `pbit-0.2.0/src/pbit/datamodelschema/column.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,223 @@
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
-import pandas as pd
 from .dax import DaxType
-from .column import Column, ColumnData 
-from .partition import Partition, PartitionData
-from .measure import Measure, MeasureData
 from .typeholder import AnnotationData
-from .powerquery import MType
 
-class HierarchyLevelData(TypedDict):
-	name: str
-	ordinal: int
-	column: str
-	linageTag: str
+SummaryType = Literal["sum"]
 
-class HierarchyData(TypedDict):
-	name: str
-	lineageTag: str
+class ColumnAttributeHierarchyData(TypedDict):
 	state: str
-	levels: list[HierarchyLevelData]
 
-class TableData(TypedDict):
-	name: str | None
+class ColumnData(TypedDict):
+	type: DaxType | None
+	lineageTag: str | None
+	summarizeBy: str | None
+	sourceColumn: str | None
+	name: str
+	dataType: str
+	formatString: str | None
+	dataCategory: str | None
+	isNameInferred: bool | None
+	expression: str | list[str] | None
+	isDataTypeInferred: bool | None
 	isHidden: bool | None
-	isPrivate: bool | None
-	showAsVariationsOnly: bool | None
-	lineageTag: str
-	columns: list[ColumnData]
-	partitions: list[PartitionData]
-	hierarchies: list[HierarchyData] | None
-	annotations: list[AnnotationData]
-	measures: list[MeasureData] | None
+	isUnique: bool | None
+	sortByColumn: str | None
+	isKey: bool | None
+	isNullable: bool | None
+	attributeHierarchy: ColumnAttributeHierarchyData
+	annotations: list[AnnotationData] | None
 
-class Table():
+class Column():
 	name: str
 	id: str
-	columns: list[Column]
-	partitions: list[Partition]
-	measures: list[Measure]
-	reference_data: TableData
+	data_type: str
+	source_column: str | None
+	reference_data: ColumnData
 
 	def __init__(
 		self,
-		name: str
+		name: str,
+		dataType: str,
+		source_column: str | None = None
 	):
 		self.name = name
 		self.id = str(uuid4())
-		self.columns: list[Column] = []
-		self.partitions: list[Partition] = []
-		self.measures: list[Measure] = []
-		ref_data: Any = {
+		self.data_type = dataType
+		self.source_column = source_column
+		self.reference_data: ColumnData = {
+			"formatString": None,
+			"dataCategory": None,
+			"isNameInferred": None,
+			"expression": None,
+			"isDataTypeInferred": None,
+			"sortByColumn": None,
+			"type": None,
+			"isHidden": None,
+			"isUnique": None,
+			"isKey": None,
+			"isNullable": None,
 			"name": self.name,
+			"dataType": self.data_type,
+			"sourceColumn": self.source_column,
 			"lineageTag": self.id,
-			"isHidden": None,
-			"isPrivate": None,
-			"showAsVariationsOnly": None,
-			"hierarchies": None,
-			"columns": [
+			"summarizeBy": "none",
+			"attributeHierarchy": {
+				"state": "ready"
+			},
+			"annotations": [
 				{
-					"formatString": None,
-					"dataCategory": None,
-					"isNameInferred": None,
-					"expression": None,
-					"isDataTypeInferred": None,
-					"sortByColumn": None,
-					"type": "rowNumber",
-					"name": "RowNumber-2662979B-1795-4F74-8F37-6A1BA8059B61",
-					"dataType": "int64",
-					"isHidden": True,
-					"isUnique": True,
-					"isKey": True,
-					"isNullable": False,
-					"lineageTag": None,
-					"summarizeBy": None,
-					"sourceColumn": None,
-					"annotations": [
-						{
-							"name": "PBI_ResultType",
-							"value": "Table"
+					"name": "SummarizationSetBy",
+					"value": "Automatic"
+				}
+			]
+		}
+
+	def set_as_bin(self, target_table_name: str, target_column_name: str, increment: float, bin_name: str | None = None, data_type: DaxType="double"):
+		final_name: str = ""
+		if bin_name:
+			final_name = bin_name
+		else:
+			final_name = target_column_name + "_bin"
+		
+		reference_data: Any = {
+			"type": "calculated",
+			"name": final_name,
+			"dataType": data_type,
+			"isDataTypeInferred": True,
+			"expression": [
+				"IF(",
+				f"\tISBLANK('{target_table_name}'[{target_column_name}]),",
+				"\tBLANK(),",
+				"\tIF(",
+				f"\t\t'{target_table_name}'[{target_column_name}] >= 0,",
+				f"\t\tROUNDDOWN('{target_table_name}'[{target_column_name}] / {increment}, 0) * {increment},",
+				f"\t\tROUNDUP('{target_table_name}'[{target_column_name}] / {increment}, 0) * {increment}",
+				"\t)",
+				")"
+			],
+			"lineageTag": self.id,
+			"summarizeBy": "none",
+			"attributeHierarchy": {
+				"state": "ready"
+			},
+			"extendedProperties": [
+				{
+					"type": "json",
+					"name": "GroupingMetadata",
+					"value": {
+						"version": 0,
+						"groupedColumns": [
+							{
+								"Column": {
+									"Expression": {
+										"SourceRef": {
+											"Entity": target_table_name
+										}
+									},
+									"Property": target_column_name
+								}
+							}
+						],
+						"binningMetadata": {
+							"binSize": {
+								"value": 5.0,
+								"unit": 0
+							}
 						}
-					],
-					"attributeHierarchy": {
-						"state": "ready"
-					},
-				},
+					}
+				}
 			],
-			"partitions": [],
-			"measures": None,
 			"annotations": [
 				{
-					"name": "PBI_ResultType",
-					"value": "Table"
+					"name": "GroupingDesignState",
+					"value": "{\"Version\":0,\"Sources\":[{\"Name\":\"p\",\"Entity\":\""
+						+target_table_name+"\"}],\"GroupedColumns\":[{\"Column\":{\"Expression\":{\"SourceRef\":{\"Source\":\"p\"}},\"Property\":\""
+						+target_column_name+"\"}}],\"BinItem\":{\"Expression\":{\"Floor\":{\"Expression\":{\"Column\":{\"Expression\":{\"SourceRef\":{\"Source\":\"p\"}},\"Property\":\""
+						+target_column_name+"\"}},\"Size\":"
+						+str(increment)+"}}}}"
+				},
+				{
+					"name": "SummarizationSetBy",
+					"value": "Automatic"
+				},
+				{
+					"name": "PBI_FormatHint",
+					"value": "{\"isGeneralNumber\":true}"
 				}
 			]
 		}
-		self.reference_data: TableData = ref_data
+		self.load(reference_data)
 
-	def bind_to_json(
-		self, 
-		relative_json_path: str, 
-		type_dictionary: dict[str, DaxType], 
-		group_name: str | None = None
-	):
-		self.new_partition(group_name).set_to_json_reader(relative_json_path, type_dictionary)
-		
-		# add columns
-		for name, col_type in type_dictionary.items():
-			self.new_column(name, col_type, name)
-
-	def new_partition(self, name="", language="m", query_group: str | None = None) -> Partition:
-		if name == "":
-			name = self.name
-
-		partition = Partition(name, language, query_group)
-		self.partitions.append(partition)
-		return partition
-
-	def get_column_by_name(self, name: str) -> Column:
-		final_column: Column | None = None
-		# print("column count: ", len(self.columns))
-		for column in self.columns:
-			# print(name, " =? ", column.name)
-			if column.name == name:
-				final_column = column
-				break
-
-		assert final_column, f"column {name} does not exist in table {self.name}"
-		return final_column
-
-	def new_column(
+	def set_as_normalized(
 		self,
-		name: str,
-		data_type: DaxType,
-		source_column: None | str = None
-	) -> Column:
-		if source_column == None and name != "":
-			source_column = name
-		column = Column(name, data_type, source_column)
-		self.columns.append(column)
-		return column
-
-	def new_bin(self, target_column_name: str, increment: float, target_table_name: str | None = None,  bin_name: str | None = None, data_type: DaxType ="double"):
-		final_table_name = ""
-		if target_table_name:
-			final_table_name = target_table_name
+		numerator_table_name: str, 
+		numerator_column_name: str, 
+		denominator_table_name: str, 
+		denominator_column_name: str,
+		name: None | str = None,
+		data_type: DaxType="double",
+		summarize_by: SummaryType="sum"
+	): 
+		final_name: str = ""
+		if name:
+			final_name = name
 		else:
-			final_table_name = self.name
+			final_name = numerator_column_name+"_per_"+denominator_column_name
+		dax = f"{numerator_table_name}[{numerator_column_name}] / {denominator_table_name}[{denominator_column_name}]"
+		if denominator_table_name != numerator_table_name:
+			dax = f"{numerator_table_name}[{numerator_column_name}] / RELATED({denominator_table_name}[{denominator_column_name}])"
 
-		column = self.new_column("", data_type)
-		column.set_as_bin(final_table_name, target_column_name, increment, bin_name, data_type)
+		self.set_dax(dax, final_name, data_type,  summarize_by)
 
-	def new_measure(self, name: str) -> Measure:
-		measure = Measure(name, "any")
-		self.measures.append(measure)
-		return measure
+	def set_dax(self, dax: str, name: str, data_type: DaxType="double", summarize_by: SummaryType="sum"):
+		ref_data: Any = {
+            "type": "calculated",
+            "name": name,
+            "dataType": data_type,
+            "isDataTypeInferred": True,
+            "expression": dax,
+            "lineageTag": self.id,
+            "summarizeBy": summarize_by,
+            "attributeHierarchy": {
+              "state": "ready"
+            },
+            "annotations": [
+              {
+                "name": "SummarizationSetBy",
+                "value": "Automatic"
+              },
+              {
+                "name": "PBI_FormatHint",
+                "value": "{\"isGeneralNumber\":true}"
+              }
+            ]
+          }
+		self.load(ref_data)
 
-	def load(self, data: TableData):
+	def load(self, data: ColumnData):
 		self.reference_data = deepcopy(data)
-		if "name" in self.reference_data:
-			name = self.reference_data["name"]
-			assert name
-			self.name = name
-
-		self.id = self.reference_data["lineageTag"]
-
-		for column_data in self.reference_data["columns"]:
-			column = self.new_column("", "any")
-			column.load(column_data)
-		self.reference_data["columns"] = []
-
-		for partition_data in self.reference_data["partitions"]:
-			partition = self.new_partition("")
-			partition.load(partition_data)
-
-		self.reference_data["partitions"] = []
-
-	def dump(self) -> TableData:
-		table_data: TableData = deepcopy(self.reference_data)
-
-		for column in self.columns:
-			table_data["columns"].append(column.dump())
-
-		for partition in self.partitions:
-			table_data["partitions"].append(partition.dump())
+		self.name = self.reference_data["name"]
+		self.data_type = self.reference_data["dataType"]
+		if "sourceColumn" in self.reference_data:
+			source_column_ref = self.reference_data["sourceColumn"]
+			assert source_column_ref
+			self.source_column = source_column_ref
+		
+		if "lineageTag" in self.reference_data:
+			lin_tag = self.reference_data["lineageTag"]
+			assert lin_tag
+			self.id = lin_tag
+
+	def dump(self) -> ColumnData:
+		column_data: ColumnData = deepcopy(self.reference_data)
+		column_data["name"] = self.name
+		column_data["dataType"] = self.data_type
+		if column_data["dataType"] == "any":
+			column_data["dataType"] = "string"
 
-		if len(self.measures) > 0:
-			measure_list = []
-			for measure in self.measures:
-				measure_list.append(measure.dump())
-			table_data["measures"] = measure_list
+		column_data["sourceColumn"] = self.source_column
+		column_data["lineageTag"] = self.id
 
-		return table_data
+		return column_data
```

### Comparing `pbit-0.1.2/src/pbit.egg-info/SOURCES.txt` & `pbit-0.2.0/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

