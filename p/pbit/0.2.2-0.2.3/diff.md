# Comparing `tmp/pbit-0.2.2.tar.gz` & `tmp/pbit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.2.2.tar", last modified: Wed Apr 12 02:04:01 2023, max compression
+gzip compressed data, was "pbit-0.2.3.tar", last modified: Wed Apr 12 02:07:10 2023, max compression
```

## Comparing `pbit-0.2.2.tar` & `pbit-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:04:01.106366 pbit-0.2.2/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-12 02:04:01.105369 pbit-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.2/README.md
--rw-rw-rw-   0        0        0      518 2023-04-12 02:03:26.000000 pbit-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 02:04:01.106366 pbit-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 02:04:01.054913 pbit-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 02:04:01.062371 pbit-0.2.2/src/pbit/
--rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.2/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:04:01.103375 pbit-0.2.2/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.2/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     6073 2023-04-12 02:03:08.000000 pbit-0.2.2/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.2/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.2/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.2/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.2/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.2/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     6557 2023-04-11 23:48:19.000000 pbit-0.2.2/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.2/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:04:01.085302 pbit-0.2.2/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-12 02:04:01.000000 pbit-0.2.2/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-12 02:04:01.000000 pbit-0.2.2/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:04:01.000000 pbit-0.2.2/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 02:04:01.000000 pbit-0.2.2/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-12 02:04:01.000000 pbit-0.2.2/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 02:07:10.240047 pbit-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-04-12 02:07:10.239051 pbit-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.2.3/README.md
+-rw-rw-rw-   0        0        0      518 2023-04-12 02:06:53.000000 pbit-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:07:10.240047 pbit-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 02:07:10.190182 pbit-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:07:10.196166 pbit-0.2.3/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 23:24:18.000000 pbit-0.2.3/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:07:10.237056 pbit-0.2.3/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.2.3/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     6073 2023-04-12 02:03:08.000000 pbit-0.2.3/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.2.3/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.2.3/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.2.3/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.2.3/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.2.3/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     6567 2023-04-12 02:06:43.000000 pbit-0.2.3/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.2.3/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:07:10.222095 pbit-0.2.3/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-04-12 02:07:10.000000 pbit-0.2.3/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-12 02:07:10.000000 pbit-0.2.3/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:07:10.000000 pbit-0.2.3/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 02:07:10.000000 pbit-0.2.3/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-12 02:07:10.000000 pbit-0.2.3/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.2.2/LICENSE` & `pbit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/pyproject.toml` & `pbit-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.2.2/src/pbit/__init__.py` & `pbit-0.2.3/src/pbit/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/src/pbit/datamodelschema/__init__.py` & `pbit-0.2.3/src/pbit/datamodelschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/src/pbit/datamodelschema/column.py` & `pbit-0.2.3/src/pbit/datamodelschema/column.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/src/pbit/datamodelschema/measure.py` & `pbit-0.2.3/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/src/pbit/datamodelschema/partition.py` & `pbit-0.2.3/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/src/pbit/datamodelschema/powerquery.py` & `pbit-0.2.3/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/src/pbit/datamodelschema/relationship.py` & `pbit-0.2.3/src/pbit/datamodelschema/relationship.py`

 * *Files identical despite different names*

### Comparing `pbit-0.2.2/src/pbit/datamodelschema/table.py` & `pbit-0.2.3/src/pbit/datamodelschema/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 			name = self.reference_data["name"]
 			assert name
 			self.name = name
 
 		self.id = self.reference_data["lineageTag"]
 
 		for column_data in self.reference_data["columns"]:
-			column = self.new_column("", "any")
+			column = self.new_column(str(uuid4()), "any")
 			column.load(column_data)
 		self.reference_data["columns"] = []
 
 		for partition_data in self.reference_data["partitions"]:
 			partition = self.new_partition("")
 			partition.load(partition_data)
```

### Comparing `pbit-0.2.2/src/pbit.egg-info/SOURCES.txt` & `pbit-0.2.3/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

