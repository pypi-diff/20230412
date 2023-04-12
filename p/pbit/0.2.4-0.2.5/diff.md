# Comparing `tmp/pbit-0.2.4.tar.gz` & `tmp/pbit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.2.4.tar", last modified: Wed Apr 12 02:17:17 2023, max compression
+gzip compressed data, was "pbit-0.2.5.tar", last modified: Wed Apr 12 02:20:58 2023, max compression
```

## Comparing `pbit-0.2.4.tar` & `pbit-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:17:17.366071 pbit-0.2.4/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-12 02:17:17.364075 pbit-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.4/README.md
--rw-rw-rw-   0        0        0      518 2023-04-12 02:17:02.000000 pbit-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 02:17:17.366071 pbit-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 02:17:17.316202 pbit-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:17:17.324180 pbit-0.2.4/src/pbit/
--rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.4/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:17:17.363084 pbit-0.2.4/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.4/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.4/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.4/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.4/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.4/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.4/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.4/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     6700 2023-04-12 02:15:58.000000 pbit-0.2.4/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.4/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:17:17.347118 pbit-0.2.4/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-12 02:17:17.000000 pbit-0.2.4/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-12 02:17:17.000000 pbit-0.2.4/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:17:17.000000 pbit-0.2.4/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 02:17:17.000000 pbit-0.2.4/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-12 02:17:17.000000 pbit-0.2.4/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.626666 pbit-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-04-12 02:20:58.624672 pbit-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.5/README.md
+-rw-rw-rw-   0        0        0      518 2023-04-12 02:20:32.000000 pbit-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:20:58.626666 pbit-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.575802 pbit-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.583783 pbit-0.2.5/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.5/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.623685 pbit-0.2.5/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.5/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     6028 2023-04-12 02:16:53.000000 pbit-0.2.5/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.5/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.5/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.5/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.5/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.5/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     6731 2023-04-12 02:20:32.000000 pbit-0.2.5/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.5/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:20:58.607717 pbit-0.2.5/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-12 02:20:58.000000 pbit-0.2.5/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.2.4/LICENSE` & `pbit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/pyproject.toml` & `pbit-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.2.4/src/pbit/__init__.py` & `pbit-0.2.5/src/pbit/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/src/pbit/datamodelschema/__init__.py` & `pbit-0.2.5/src/pbit/datamodelschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/src/pbit/datamodelschema/column.py` & `pbit-0.2.5/src/pbit/datamodelschema/column.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/src/pbit/datamodelschema/measure.py` & `pbit-0.2.5/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/src/pbit/datamodelschema/partition.py` & `pbit-0.2.5/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/src/pbit/datamodelschema/powerquery.py` & `pbit-0.2.5/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/src/pbit/datamodelschema/relationship.py` & `pbit-0.2.5/src/pbit/datamodelschema/relationship.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.4/src/pbit/datamodelschema/table.py` & `pbit-0.2.5/src/pbit/datamodelschema/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,32 +138,32 @@
 
 	def new_column(
 		self,
 		name: str,
 		data_type: DaxType,
 		source_column: None | str = None
 	) -> Column:
-		if source_column == None and name != "":
+		if source_column != None and name != "":
 			source_column = name
 
 		assert self.get_if_column_exists(name) == False, f"column with name {name} in table {self.name} already exists!"
 
 		column = Column(name, data_type, source_column)
 		self.columns.append(column)
 		return column
 
 	def new_bin(self, target_column_name: str, increment: float, target_table_name: str | None = None,  bin_name: str | None = None, data_type: DaxType ="double") -> Column:
 		final_table_name = ""
-		if type(target_table_name) != None:
+		if type(target_table_name) == str:
 			final_table_name = target_table_name
 		else:
 			final_table_name = self.name
 
 		final_name = ""
-		if bin_name:
+		if type(bin_name) == str:
 			final_name = bin_name
 		else:
 			final_name = target_column_name + "_bin"
 
 		column = self.new_column(final_table_name, data_type)
 		column.set_as_bin(final_table_name, target_column_name, increment, final_name, data_type)
 		return column
@@ -179,24 +179,24 @@
 		denominator_column_name: str,
 		denominator_table_name: None | str = None,
 		name: None | str = None,
 		data_type: DaxType="double",
 		summarize_by: SummaryType="sum"
 	):
 		final_name: str = ""
-		if name:
+		if type(name) == str:
 			final_name = name
 		else:
 			final_name = numerator_column_name+"_per_"+denominator_column_name
 		
 		final_denominator_table_name: str = ""
-		if denominator_table_name == None:
-			final_denominator_table_name = self.name
+		if type(denominator_table_name) == str:
+			final_denominator_table_name = denominator_table_name	
 		else:
-			final_denominator_table_name = denominator_table_name
+			final_denominator_table_name = self.name
 
 		column = self.new_column(final_name, data_type)
 		column.set_as_normalized(self.name, numerator_column_name, final_denominator_table_name, denominator_column_name, final_name, data_type, summarize_by)
 		return column
 
 	def new_measure(self, name: str) -> Measure:
 		measure = Measure(name, "any")
```

### Comparing `pbit-0.2.4/src/pbit.egg-info/SOURCES.txt` & `pbit-0.2.5/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

