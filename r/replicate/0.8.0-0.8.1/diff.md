# Comparing `tmp/replicate-0.8.0.tar.gz` & `tmp/replicate-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate-0.8.0.tar", last modified: Wed Apr 12 11:41:19 2023, max compression
+gzip compressed data, was "replicate-0.8.1.tar", last modified: Wed Apr 12 14:16:04 2023, max compression
```

## Comparing `replicate-0.8.0.tar` & `replicate-0.8.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-04-12 11:41:10.000000 replicate-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    18309 2023-04-12 11:41:19.023656 replicate-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-04-12 11:41:10.000000 replicate-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-04-12 11:41:10.000000 replicate-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/replicate/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1521 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2667 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/training.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/replicate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18309 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      587 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 11:41:19.023656 replicate-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      916 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (122)     8618 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.991200 replicate-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-04-12 14:15:53.000000 replicate-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-04-12 14:16:04.987200 replicate-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-12 14:15:53.000000 replicate-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 14:15:53.000000 replicate-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.987200 replicate-0.8.1/replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.987200 replicate-0.8.1/replicate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:16:04.991200 replicate-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.987200 replicate-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_version.py
```

### Comparing `replicate-0.8.0/LICENSE` & `replicate-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/PKG-INFO` & `replicate-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python client for Replicate
 Author: Replicate, Inc.
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `replicate-0.8.0/README.md` & `replicate-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/pyproject.toml` & `replicate-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "replicate"
-version = "0.8.0"
+version = "0.8.1"
 description = "Python client for Replicate"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Replicate, Inc." }]
 requires-python = ">=3.8"
 dependencies = ["packaging", "pydantic>1", "requests>2"]
 optional-dependencies = { dev = [
```

### Comparing `replicate-0.8.0/replicate/base_model.py` & `replicate-0.8.1/replicate/base_model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/client.py` & `replicate-0.8.1/replicate/client.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/collection.py` & `replicate-0.8.1/replicate/collection.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/files.py` & `replicate-0.8.1/replicate/files.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/json.py` & `replicate-0.8.1/replicate/json.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/model.py` & `replicate-0.8.1/replicate/model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/prediction.py` & `replicate-0.8.1/replicate/prediction.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/schema.py` & `replicate-0.8.1/replicate/schema.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate/training.py` & `replicate-0.8.1/replicate/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 from typing import Any, Dict, List, Optional
 
 from replicate.base_model import BaseModel
 from replicate.collection import Collection
 from replicate.exceptions import ReplicateException
 from replicate.files import upload_file
 from replicate.json import encode_json
+from replicate.version import Version
 
 
 class Training(BaseModel):
     completed_at: Optional[str]
     created_at: Optional[str]
     destination: Optional[str]
     error: Optional[str]
     id: str
     input: Optional[Dict[str, Any]]
     logs: Optional[str]
     output: Optional[Any]
     started_at: Optional[str]
     status: str
-    version: str
+    version: Optional[Version]
 
     def cancel(self) -> None:
         """Cancel a running training"""
         self._client._request("POST", f"/v1/trainings/{self.id}/cancel")
 
 
 class TrainingCollection(Collection):
@@ -40,14 +41,16 @@
 
     def get(self, id: str) -> Training:
         resp = self._client._request(
             "GET",
             f"/v1/trainings/{id}",
         )
         obj = resp.json()
+        # HACK: resolve this? make it lazy somehow?
+        del obj["version"]
         return self.prepare_model(obj)
 
     def create(  # type: ignore
         self,
         version: str,
         input: Dict[str, Any],
         destination: str,
@@ -79,8 +82,9 @@
 
         resp = self._client._request(
             "POST",
             f"/v1/models/{username}/{model_name}/versions/{version_id}/trainings",
             json=body,
         )
         obj = resp.json()
+        del obj["version"]
         return self.prepare_model(obj)
```

### Comparing `replicate-0.8.0/replicate/version.py` & `replicate-0.8.1/replicate/version.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/replicate.egg-info/PKG-INFO` & `replicate-0.8.1/replicate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python client for Replicate
 Author: Replicate, Inc.
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `replicate-0.8.0/replicate.egg-info/SOURCES.txt` & `replicate-0.8.1/replicate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/tests/test_client.py` & `replicate-0.8.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/tests/test_model.py` & `replicate-0.8.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/tests/test_prediction.py` & `replicate-0.8.1/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/tests/test_training.py` & `replicate-0.8.1/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.0/tests/test_version.py` & `replicate-0.8.1/tests/test_version.py`

 * *Files identical despite different names*

