# Comparing `tmp/pbit-0.1.0.tar.gz` & `tmp/pbit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.1.0.tar", last modified: Tue Apr 11 22:31:06 2023, max compression
+gzip compressed data, was "pbit-0.1.1.tar", last modified: Tue Apr 11 22:48:05 2023, max compression
```

## Comparing `pbit-0.1.0.tar` & `pbit-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:31:06.190545 pbit-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-11 22:31:06.189543 pbit-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.1.0/README.md
--rw-rw-rw-   0        0        0      518 2023-04-11 22:30:04.000000 pbit-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 22:31:06.190545 pbit-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 22:31:06.129620 pbit-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 22:31:06.141063 pbit-0.1.0/src/pbit/
--rw-rw-rw-   0        0        0     2265 2023-04-11 22:24:01.000000 pbit-0.1.0/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:31:06.187594 pbit-0.1.0/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14209 2023-04-11 22:23:28.000000 pbit-0.1.0/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     4779 2023-04-11 22:03:31.000000 pbit-0.1.0/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.1.0/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2061 2023-04-11 22:01:58.000000 pbit-0.1.0/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2297 2023-04-11 22:02:23.000000 pbit-0.1.0/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8174 2023-04-11 22:05:03.000000 pbit-0.1.0/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.1.0/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     5268 2023-04-11 22:06:55.000000 pbit-0.1.0/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.1.0/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:31:06.168599 pbit-0.1.0/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-11 22:31:06.000000 pbit-0.1.0/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-11 22:31:06.000000 pbit-0.1.0/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:31:06.000000 pbit-0.1.0/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 22:31:06.000000 pbit-0.1.0/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 22:31:06.000000 pbit-0.1.0/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 22:48:05.327580 pbit-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-04-11 22:48:05.326583 pbit-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.1.1/README.md
+-rw-rw-rw-   0        0        0      518 2023-04-11 22:45:00.000000 pbit-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 22:48:05.327580 pbit-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 22:48:03.020670 pbit-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 22:48:03.866745 pbit-0.1.1/src/pbit/
+-rw-rw-rw-   0        0        0     2285 2023-04-11 22:41:25.000000 pbit-0.1.1/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:48:05.323591 pbit-0.1.1/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.1.1/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     4739 2023-04-11 22:44:53.000000 pbit-0.1.1/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.1.1/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.1.1/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.1.1/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.1.1/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.1.1/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     5148 2023-04-11 22:44:48.000000 pbit-0.1.1/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.1.1/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:48:05.231085 pbit-0.1.1/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.1.0/LICENSE` & `pbit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.1.0/pyproject.toml` & `pbit-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.1.0/src/pbit/__init__.py` & `pbit-0.1.1/src/pbit/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import zipfile
 from tempfile import TemporaryDirectory
 from .datamodelschema import read as read_pbit
 from .datamodelschema import write as write_pbit
 from .datamodelschema import DataModelSchema, DataModelSchemaData
 
-def pack_pbti_file(dir_path: str, out_path: str):
+def pack(dir_path: str, out_pbit_file_path: str):
 	zip_path = dir_path + ".zip"
 
 	# zip directory back up
 	if os.path.exists(zip_path):
 		os.remove(zip_path)
 	zip_out = zipfile.ZipFile(zip_path, 'w', zipfile.ZIP_DEFLATED)
 	for root, _, files in os.walk(dir_path):
@@ -20,45 +20,45 @@
 			# Construct the relative file path (relative to the directory being zipped)
 			relative_path = os.path.relpath(file_path, dir_path)
 			# Add the file to the ZIP file with the relative path as the archive name
 			zip_out.write(file_path, arcname=relative_path)
 	zip_out.close()
 
 	# convert to pbit file in final position
-	if os.path.exists(out_path):
-		os.remove(out_path)
-	shutil.move(zip_path, out_path)
+	if os.path.exists(out_pbit_file_path):
+		os.remove(out_pbit_file_path)
+	shutil.move(zip_path, out_pbit_file_path)
 
-def unpack_pbti_file(file_path: str, out_path: str):
-	base = os.path.split(out_path)[0]
+def unpack(pbit_file_path: str, out_dir_path: str):
+	base = os.path.split(out_dir_path)[0]
 	zip_path = base + ".zip"
 
 	# convert to zip file
 	if os.path.exists(zip_path):
 		os.remove(zip_path)
-	shutil.copy(file_path, zip_path)
+	shutil.copy(pbit_file_path, zip_path)
 
 	# unzip and extract data
-	if os.path.exists(out_path):
-		shutil.rmtree(out_path)
+	if os.path.exists(out_dir_path):
+		shutil.rmtree(out_dir_path)
 	zip_ref = zipfile.ZipFile(zip_path, 'r')
-	zip_ref.extractall(out_path)
+	zip_ref.extractall(out_dir_path)
 	zip_ref.close()
 		
 def write_model(pbit_file_path: str, source: DataModelSchemaData | DataModelSchema):
 	with TemporaryDirectory() as temp_dir_path:
 		pbti_dir = temp_dir_path + "/pbit"
-		unpack_pbti_file(pbit_file_path, pbti_dir)
+		unpack(pbit_file_path, pbti_dir)
 		if type(source) == DataModelSchema:
 			write_pbit(pbti_dir+"/DataModelSchema", source.dump())
 		elif type(source) == DataModelSchemaData:
 			write_pbit(pbti_dir+"/DataModelSchema", source)
-		pack_pbti_file(pbti_dir, pbit_file_path)	
+		pack(pbti_dir, pbit_file_path)	
 
 def read_model(pbit_file_path: str) -> DataModelSchemaData:
 	with TemporaryDirectory() as temp_dir_path:
 		pbti_dir = temp_dir_path + "/pbit"
-		unpack_pbti_file(pbit_file_path, pbti_dir)
+		unpack(pbit_file_path, pbti_dir)
 		return read_pbit(pbti_dir+"/DataModelSchema")
 
 def load_model(pbit_file_path: str) -> DataModelSchema:
 	return DataModelSchema(read_model(pbit_file_path))
```

### Comparing `pbit-0.1.0/src/pbit/datamodelschema/__init__.py` & `pbit-0.1.1/src/pbit/datamodelschema/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import inspect
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
-from pbit.datamodelschema.typeholder import AnnotationData
-from pbit.datamodelschema.relationship import RelationshipData, Relationship
-from pbit.datamodelschema.table import TableData, Table
+from .typeholder import AnnotationData
+from .relationship import RelationshipData, Relationship
+from .table import TableData, Table
 
 class AccessOptionsData(TypedDict):
 	legacyRedirects: bool
 	returnErrorValuesAsNull: bool
 
 class QueryGroupData(TypedDict):
 	folder: str
@@ -396,15 +396,15 @@
 	def clear_query_groups(self):
 		self.query_groups = []
 		if "model" in self.reference_data:
 			model_data = self.reference_data["model"]
 			if "queryGroups" in model_data:
 				model_data["queryGroups"] = []
 
-	def reset_model(self):
+	def clear(self):
 		self.clear_tables()
 		self.clear_relationships()
 		self.clear_query_groups()			
 
 	def get_table_by_name(self, name: str) -> Table:
 		final_table: Table | None
 		for table in self.tables:
```

### Comparing `pbit-0.1.0/src/pbit/datamodelschema/column.py` & `pbit-0.1.1/src/pbit/datamodelschema/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
-from pbit.datamodelschema.dax import DaxType
-from pbit.datamodelschema.typeholder import AnnotationData
+from .dax import DaxType
+from .typeholder import AnnotationData
 
 class ColumnAttributeHierarchyData(TypedDict):
 	state: str
 
 class ColumnData(TypedDict):
 	type: DaxType | None
 	lineageTag: str | None
```

### Comparing `pbit-0.1.0/src/pbit/datamodelschema/measure.py` & `pbit-0.1.1/src/pbit/datamodelschema/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
 from pandas import DataFrame
-from pbit.datamodelschema.column import DaxType
+from .column import DaxType
 
 class MeasureProperty(TypedDict):
 	property: str
 
 class MeasureData(TypedDict):
 	name: str
 	expression: str
```

### Comparing `pbit-0.1.0/src/pbit/datamodelschema/partition.py` & `pbit-0.1.1/src/pbit/datamodelschema/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
-from pbit.datamodelschema.column import DaxType
-from pbit.datamodelschema.powerquery import PowerQuery, MType, from_dax_type_to_m_type
+from .column import DaxType
+from .powerquery import PowerQuery, MType, from_dax_type_to_m_type
 
 class PartitionSourceData(TypedDict):
 	type: str
 	expression: list[str] | str
 
 class PartitionData(TypedDict):
 	name: str | None
```

### Comparing `pbit-0.1.0/src/pbit/datamodelschema/powerquery.py` & `pbit-0.1.1/src/pbit/datamodelschema/powerquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypedDict, Literal, Any, Callable
 from uuid import uuid4
-from pbit.datamodelschema.column import DaxType
+from .column import DaxType
 import os
 
 PRIOR_PREFIX: str = "~!PRIOR_TABLE_KEY!~"
 
 MType = Literal[
 	"Int64.Type",
 	"Currency.Type",
```

### Comparing `pbit-0.1.0/src/pbit/datamodelschema/relationship.py` & `pbit-0.1.1/src/pbit/datamodelschema/relationship.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.0/src/pbit/datamodelschema/table.py` & `pbit-0.1.1/src/pbit/datamodelschema/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import TypedDict, Literal, Any
 from uuid import uuid4
 from copy import deepcopy
 import pandas as pd
-from pbit.datamodelschema.dax import DaxType
-from pbit.datamodelschema.column import Column, ColumnData 
-from pbit.datamodelschema.partition import Partition, PartitionData
-from pbit.datamodelschema.measure import Measure, MeasureData
-from pbit.datamodelschema.typeholder import AnnotationData
-from pbit.datamodelschema.powerquery import MType
+from .dax import DaxType
+from .column import Column, ColumnData 
+from .partition import Partition, PartitionData
+from .measure import Measure, MeasureData
+from .typeholder import AnnotationData
+from .powerquery import MType
 
 class HierarchyLevelData(TypedDict):
 	name: str
 	ordinal: int
 	column: str
 	linageTag: str
```

### Comparing `pbit-0.1.0/src/pbit.egg-info/SOURCES.txt` & `pbit-0.1.1/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

