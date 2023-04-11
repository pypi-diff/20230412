# Comparing `tmp/pbit-0.1.1.tar.gz` & `tmp/pbit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbit-0.1.1.tar", last modified: Tue Apr 11 22:48:05 2023, max compression
+gzip compressed data, was "pbit-0.1.2.tar", last modified: Tue Apr 11 22:54:56 2023, max compression
```

## Comparing `pbit-0.1.1.tar` & `pbit-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:48:05.327580 pbit-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      472 2023-04-11 22:48:05.326583 pbit-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.1.1/README.md
--rw-rw-rw-   0        0        0      518 2023-04-11 22:45:00.000000 pbit-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 22:48:05.327580 pbit-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 22:48:03.020670 pbit-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 22:48:03.866745 pbit-0.1.1/src/pbit/
--rw-rw-rw-   0        0        0     2285 2023-04-11 22:41:25.000000 pbit-0.1.1/src/pbit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:48:05.323591 pbit-0.1.1/src/pbit/datamodelschema/
--rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.1.1/src/pbit/datamodelschema/__init__.py
--rw-rw-rw-   0        0        0     4739 2023-04-11 22:44:53.000000 pbit-0.1.1/src/pbit/datamodelschema/column.py
--rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.1.1/src/pbit/datamodelschema/dax.py
--rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.1.1/src/pbit/datamodelschema/measure.py
--rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.1.1/src/pbit/datamodelschema/partition.py
--rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.1.1/src/pbit/datamodelschema/powerquery.py
--rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.1.1/src/pbit/datamodelschema/relationship.py
--rw-rw-rw-   0        0        0     5148 2023-04-11 22:44:48.000000 pbit-0.1.1/src/pbit/datamodelschema/table.py
--rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.1.1/src/pbit/datamodelschema/typeholder.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:48:05.231085 pbit-0.1.1/src/pbit.egg-info/
--rw-rw-rw-   0        0        0      472 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 22:48:02.000000 pbit-0.1.1/src/pbit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 22:54:56.005170 pbit-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 21:57:47.000000 pbit-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      472 2023-04-11 22:54:56.003193 pbit-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-11 21:57:47.000000 pbit-0.1.2/README.md
+-rw-rw-rw-   0        0        0      518 2023-04-11 22:54:22.000000 pbit-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 22:54:56.005170 pbit-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.950560 pbit-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.960586 pbit-0.1.2/src/pbit/
+-rw-rw-rw-   0        0        0     2330 2023-04-11 22:54:16.000000 pbit-0.1.2/src/pbit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.998976 pbit-0.1.2/src/pbit/datamodelschema/
+-rw-rw-rw-   0        0        0    14143 2023-04-11 22:44:53.000000 pbit-0.1.2/src/pbit/datamodelschema/__init__.py
+-rw-rw-rw-   0        0        0     4739 2023-04-11 22:44:53.000000 pbit-0.1.2/src/pbit/datamodelschema/column.py
+-rw-rw-rw-   0        0        0      120 2023-04-11 22:03:31.000000 pbit-0.1.2/src/pbit/datamodelschema/dax.py
+-rw-rw-rw-   0        0        0     2041 2023-04-11 22:44:53.000000 pbit-0.1.2/src/pbit/datamodelschema/measure.py
+-rw-rw-rw-   0        0        0     2257 2023-04-11 22:44:48.000000 pbit-0.1.2/src/pbit/datamodelschema/partition.py
+-rw-rw-rw-   0        0        0     8154 2023-04-11 22:44:48.000000 pbit-0.1.2/src/pbit/datamodelschema/powerquery.py
+-rw-rw-rw-   0        0        0     2452 2023-04-11 01:22:47.000000 pbit-0.1.2/src/pbit/datamodelschema/relationship.py
+-rw-rw-rw-   0        0        0     5148 2023-04-11 22:44:48.000000 pbit-0.1.2/src/pbit/datamodelschema/table.py
+-rw-rw-rw-   0        0        0      156 2023-04-10 16:51:37.000000 pbit-0.1.2/src/pbit/datamodelschema/typeholder.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:54:55.982555 pbit-0.1.2/src/pbit.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 22:54:55.000000 pbit-0.1.2/src/pbit.egg-info/top_level.txt
```

### Comparing `pbit-0.1.1/LICENSE` & `pbit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/pyproject.toml` & `pbit-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pbit"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"pandas~=2.0.0",
 ]
 description = "a package with useful functions for downloading and working with midas generated analytics data"
```

### Comparing `pbit-0.1.1/src/pbit/__init__.py` & `pbit-0.1.2/src/pbit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,8 +57,11 @@
 def read_model(pbit_file_path: str) -> DataModelSchemaData:
 	with TemporaryDirectory() as temp_dir_path:
 		pbti_dir = temp_dir_path + "/pbit"
 		unpack(pbit_file_path, pbti_dir)
 		return read_pbit(pbti_dir+"/DataModelSchema")
 
 def load_model(pbit_file_path: str) -> DataModelSchema:
-	return DataModelSchema(read_model(pbit_file_path))
+	data = read_model(pbit_file_path)
+	model = DataModelSchema()
+	model.load(data)
+	return model
```

### Comparing `pbit-0.1.1/src/pbit/datamodelschema/__init__.py` & `pbit-0.1.2/src/pbit/datamodelschema/__init__.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/src/pbit/datamodelschema/column.py` & `pbit-0.1.2/src/pbit/datamodelschema/column.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/src/pbit/datamodelschema/measure.py` & `pbit-0.1.2/src/pbit/datamodelschema/measure.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/src/pbit/datamodelschema/partition.py` & `pbit-0.1.2/src/pbit/datamodelschema/partition.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/src/pbit/datamodelschema/powerquery.py` & `pbit-0.1.2/src/pbit/datamodelschema/powerquery.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/src/pbit/datamodelschema/relationship.py` & `pbit-0.1.2/src/pbit/datamodelschema/relationship.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/src/pbit/datamodelschema/table.py` & `pbit-0.1.2/src/pbit/datamodelschema/table.py`

 * *Files identical despite different names*

### Comparing `pbit-0.1.1/src/pbit.egg-info/SOURCES.txt` & `pbit-0.1.2/src/pbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

