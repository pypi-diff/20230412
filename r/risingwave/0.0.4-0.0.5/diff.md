# Comparing `tmp/risingwave-0.0.4.tar.gz` & `tmp/risingwave-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risingwave-0.0.4.tar", last modified: Tue Apr  4 10:22:31 2023, max compression
+gzip compressed data, was "risingwave-0.0.5.tar", last modified: Wed Apr 12 11:25:21 2023, max compression
```

## Comparing `risingwave-0.0.4.tar` & `risingwave-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-04 10:22:31.498573 risingwave-0.0.4/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-04-04 10:22:31.498325 risingwave-0.0.4/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.4/README.md
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-04 10:22:31.481401 risingwave-0.0.4/risingwave/
--rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.4/risingwave/__init__.py
--rw-r--r--   0 wangrunji   (501) staff       (20)     9305 2023-04-04 04:46:10.000000 risingwave-0.0.4/risingwave/udf.py
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-04 10:22:31.497743 risingwave-0.0.4/risingwave.egg-info/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-04-04 10:22:31.000000 risingwave-0.0.4/risingwave.egg-info/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)      228 2023-04-04 10:22:31.000000 risingwave-0.0.4/risingwave.egg-info/SOURCES.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-04-04 10:22:31.000000 risingwave-0.0.4/risingwave.egg-info/dependency_links.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        8 2023-04-04 10:22:31.000000 risingwave-0.0.4/risingwave.egg-info/requires.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-04-04 10:22:31.000000 risingwave-0.0.4/risingwave.egg-info/top_level.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-04-04 10:22:31.498617 risingwave-0.0.4/setup.cfg
--rw-r--r--   0 wangrunji   (501) staff       (20)      605 2023-04-04 04:44:31.000000 risingwave-0.0.4/setup.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-12 11:25:21.415539 risingwave-0.0.5/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-04-12 11:25:21.415375 risingwave-0.0.5/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.5/README.md
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-12 11:25:21.412151 risingwave-0.0.5/risingwave/
+-rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.5/risingwave/__init__.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)    10275 2023-04-12 11:24:37.000000 risingwave-0.0.5/risingwave/udf.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-04-12 11:25:21.415120 risingwave-0.0.5/risingwave.egg-info/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)      228 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/SOURCES.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/dependency_links.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)        8 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/requires.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-04-12 11:25:21.000000 risingwave-0.0.5/risingwave.egg-info/top_level.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-04-12 11:25:21.415583 risingwave-0.0.5/setup.cfg
+-rw-r--r--   0 wangrunji   (501) staff       (20)      605 2023-04-12 11:25:01.000000 risingwave-0.0.5/setup.py
```

### Comparing `risingwave-0.0.4/PKG-INFO` & `risingwave-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.4
+Version: 0.0.5
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `risingwave-0.0.4/README.md` & `risingwave-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `risingwave-0.0.4/risingwave/udf.py` & `risingwave-0.0.5/risingwave/udf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import *
 import pyarrow as pa
 import pyarrow.flight
 import pyarrow.parquet
 import inspect
 import traceback
+import json
 
 
 class UserDefinedFunction:
     """
     Base interface for user-defined function.
     """
     _name: str
@@ -30,20 +31,43 @@
     def eval(self, *args) -> Any:
         """
         Method which defines the logic of the scalar function.
         """
         pass
 
     def eval_batch(self, batch: pa.RecordBatch) -> pa.RecordBatch:
-        column = [self.eval(*[col[i].as_py() for col in batch])
+        # parse value from json string for jsonb columns
+        inputs = [[v.as_py() for v in array] for array in batch]
+        inputs = [
+            _process_input_array(array, type)
+            for array, type in zip(inputs, self._input_schema.types)]
+
+        # evaluate the function for each row
+        column = [self.eval(*[col[i] for col in inputs])
                   for i in range(batch.num_rows)]
+
+        # convert value to json for jsonb columns
+        if self._result_schema.types[0] == pa.large_string():
+            column = [(json.dumps(v) if v is not None else None)
+                      for v in column]
         array = pa.array(column, type=self._result_schema.types[0])
         return pa.RecordBatch.from_arrays([array], schema=self._result_schema)
 
 
+def _process_input_array(array: list, type: pa.DataType) -> list:
+    if pa.types.is_list(type):
+        return [(_process_input_array(v, type.value_type)
+                if v is not None else None)
+                for v in array]
+    if pa.types.is_large_string(type):
+        return [(json.loads(v) if v is not None else None)
+                for v in array]
+    return array
+
+
 class TableFunction(UserDefinedFunction):
     """
     Base interface for user-defined table function. A user-defined table functions maps zero, one,
     or multiple table values to a new table value.
     """
 
     def eval(self, *args) -> Iterator:
@@ -258,14 +282,16 @@
         return pa.time32('ms')
     elif type_str in ('TIMESTAMP', 'TIMESTAMP WITHOUT TIME ZONE'):
         return pa.timestamp('ms')
     elif type_str.startswith('INTERVAL'):
         return pa.duration('us')
     elif type_str in ('VARCHAR'):
         return pa.string()
+    elif type_str in ('JSONB'):
+        return pa.large_string()
     elif type_str in ('BYTEA'):
         return pa.binary()
     elif type_str.endswith('[]'):
         return pa.list_(_string_to_data_type(type_str[:-2]))
     elif type_str.startswith('STRUCT'):
         # extract 'STRUCT<INT, VARCHAR, ...>'
         type_list = type_str[6:].strip('<>')
```

### Comparing `risingwave-0.0.4/risingwave.egg-info/PKG-INFO` & `risingwave-0.0.5/risingwave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.4
+Version: 0.0.5
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `risingwave-0.0.4/setup.py` & `risingwave-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="risingwave",
-    version="0.0.4",
+    version="0.0.5",
     author="RisingWave Labs",
     description="RisingWave Python API",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/risingwavelabs/risingwave",
     packages=find_packages(),
     classifiers=[
```

