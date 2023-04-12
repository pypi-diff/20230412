# Comparing `tmp/qdrant_txtai-1.0.0.tar.gz` & `tmp/qdrant_txtai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_txtai-1.0.0.tar", max compression
+gzip compressed data, was "qdrant_txtai-1.0.1.tar", max compression
```

## Comparing `qdrant_txtai-1.0.0.tar` & `qdrant_txtai-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-02-10 12:46:21.970170 qdrant_txtai-1.0.0/LICENSE
--rw-r--r--   0        0        0     2802 2023-02-10 12:46:21.970170 qdrant_txtai-1.0.0/README.md
--rw-r--r--   0        0        0      675 2023-02-10 12:46:21.970170 qdrant_txtai-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 12:46:21.974170 qdrant_txtai-1.0.0/src/qdrant_txtai/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 12:46:21.974170 qdrant_txtai-1.0.0/src/qdrant_txtai/ann/__init__.py
--rw-r--r--   0        0        0     4489 2023-02-10 12:46:21.974170 qdrant_txtai-1.0.0/src/qdrant_txtai/ann/qdrant.py
--rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 qdrant_txtai-1.0.0/setup.py
--rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 qdrant_txtai-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-12 11:25:58.610895 qdrant_txtai-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4044 2023-04-12 11:25:58.610895 qdrant_txtai-1.0.1/README.md
+-rw-r--r--   0        0        0      676 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/src/qdrant_txtai/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/src/qdrant_txtai/ann/__init__.py
+-rw-r--r--   0        0        0     4721 2023-04-12 11:25:58.614895 qdrant_txtai-1.0.1/src/qdrant_txtai/ann/qdrant.py
+-rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 qdrant_txtai-1.0.1/PKG-INFO
```

### Comparing `qdrant_txtai-1.0.0/LICENSE` & `qdrant_txtai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_txtai-1.0.0/README.md` & `qdrant_txtai-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -66,28 +66,67 @@
 ## Configuration properties
 
 *qdrant-txtai* allows you to configure both the connection details, and some 
 internal properties of the vector collection which may impact both speed and
 accuracy. Please refer to [Qdrant docs](https://qdrant.github.io/qdrant/redoc/index.html#tag/collections/operation/create_collection)
 if you are interested in the meaning of each property.
 
-The example below presents all the available options:
+The example below presents all the available options, if we connect to Qdrant server:
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
   metric: l2 # allowed values: l2 / cosine / ip
   qdrant:
-    host: qdrant.host
+    url: qdrant.host
     port: 6333
     grpc_port: 6334
     prefer_grpc: true
     collection: CustomCollectionName
     https: true # for Qdrant Cloud
     api_key: XYZ # for Qdrant Cloud
     hnsw:
       m: 8
       ef_construct: 256
       full_scan_threshold:
       ef_search: 512
 ```
+
+### Local in-memory/disk-persisted mode
+
+Qdrant Python client, from version 1.1.1, supports local in-memory/disk-persisted mode. 
+That's a good choice for any test scenarios and quick experiments in which you do not 
+plan to store lots of vectors. In such a case spinning a Docker container might be even 
+not required.
+
+#### In-memory storage
+
+In case you want to have a transient storage, for example in case of automated tests 
+launched during your CI/CD pipeline, using Qdrant Local mode with in-memory storage 
+might be a preferred option.
+
+```yaml
+embeddings:
+  path: sentence-transformers/all-MiniLM-L6-v2
+  backend: qdrant_txtai.ann.qdrant.Qdrant
+  metric: l2 # allowed values: l2 / cosine / ip
+  qdrant:
+    location: ':memory:'
+    prefer_grpc: true
+```
+
+#### On disk storage
+
+However, if you prefer to keep the vectors between different runs of your application, 
+it might be better to use on disk storage and pass the path that should be used to 
+persist the data.
+
+```yaml
+embeddings:
+  path: sentence-transformers/all-MiniLM-L6-v2
+  backend: qdrant_txtai.ann.qdrant.Qdrant
+  metric: l2 # allowed values: l2 / cosine / ip
+  qdrant:
+    path: '/home/qdrant/storage_local'
+    prefer_grpc: true
+```
```

### Comparing `qdrant_txtai-1.0.0/pyproject.toml` & `qdrant_txtai-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "qdrant-txtai"
-version = "1.0.0"
+version = "1.0.1"
 description = "An integration of Qdrant ANN vector database backend with txtai"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_txtai", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<=3.11"
 txtai = "^5.0.0"
-qdrant-client = "1.0.0"
+qdrant-client = "^1.1.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pre-commit = "^2.20.0"
 black = "^23.1.0"
 
 [build-system]
```

### Comparing `qdrant_txtai-1.0.0/src/qdrant_txtai/ann/qdrant.py` & `qdrant_txtai-1.0.1/src/qdrant_txtai/ann/qdrant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 
-import qdrant_client
+from grpc import RpcError
 from qdrant_client import QdrantClient
+from qdrant_client.http.exceptions import UnexpectedResponse
 from qdrant_client.http.models import (
     PointIdsList,
     VectorParams,
     Distance,
     HnswConfigDiff,
     SearchRequest,
     SearchParams,
@@ -25,40 +26,44 @@
     }
 
     def __init__(self, config):
         super().__init__(config)
 
         # Load Qdrant specific configuration from the nested configuration dict
         self.qdrant_config = self.config.get("qdrant", {})
+        location = self.qdrant_config.get("location")
         url = self.qdrant_config.get("url")
         port = self.qdrant_config.get("port", 6333)
         grpc_port = self.qdrant_config.get("grpc_port", 6334)
         prefer_grpc = self.qdrant_config.get("prefer_grpc", False)
         https = self.qdrant_config.get("https")
         api_key = self.qdrant_config.get("api_key")
         prefix = self.qdrant_config.get("prefix")
         timeout = self.qdrant_config.get("timeout")
         host = self.qdrant_config.get("host")
+        path = self.qdrant_config.get("path")
         self.qdrant_client = QdrantClient(
+            location=location,
             url=url,
             port=port,
             grpc_port=grpc_port,
             prefer_grpc=prefer_grpc,
             https=https,
             api_key=api_key,
             prefix=prefix,
             timeout=timeout,
             host=host,
+            path=path,
         )
         self.collection_name = self.qdrant_config.get("collection", "embeddings")
 
         # Initial offset is set to the number of existing rows
         try:
             self.config["offset"] = self.count()
-        except qdrant_client.http.exceptions.UnexpectedResponse:
+        except (UnexpectedResponse, RpcError, ValueError):
             self.config["offset"] = 0
 
     def load(self, path):
         # Since Qdrant does not rely on files, there is no need to load anything
         # from given path. Instead, the file path is used as a collection name,
         # effectively allowing to use different embeddings.
         warnings.warn(
@@ -86,22 +91,22 @@
         )
 
         self.config["offset"] = 0
         self.append(embeddings)
 
     def append(self, embeddings):
         offset = self.config.get("offset", 0)
-        new = embeddings.shape[0]
-        ids = list(range(offset, offset + new))
+        new_count = embeddings.shape[0]
+        ids = list(range(offset, offset + new_count))
         self.qdrant_client.upload_collection(
             collection_name=self.collection_name,
             vectors=embeddings,
             ids=ids,
         )
-        self.config["offset"] += new
+        self.config["offset"] += new_count
 
     def delete(self, ids):
         self.qdrant_client.delete(
             collection_name=self.collection_name,
             points_selector=PointIdsList(points=ids),
         )
```

### Comparing `qdrant_txtai-1.0.0/PKG-INFO` & `qdrant_txtai-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qdrant-txtai
-Version: 1.0.0
+Version: 1.0.1
 Summary: An integration of Qdrant ANN vector database backend with txtai
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
 Requires-Python: >=3.7,<=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: qdrant-client (==1.0.0)
+Requires-Dist: qdrant-client (>=1.1.4,<2.0.0)
 Requires-Dist: txtai (>=5.0.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # qdrant-txtai
 
 [txtai](https://github.com/neuml/txtai) simplifies building AI-powered semantic 
 search applications using Transformers. It leverages the neural embeddings and
@@ -85,29 +85,68 @@
 ## Configuration properties
 
 *qdrant-txtai* allows you to configure both the connection details, and some 
 internal properties of the vector collection which may impact both speed and
 accuracy. Please refer to [Qdrant docs](https://qdrant.github.io/qdrant/redoc/index.html#tag/collections/operation/create_collection)
 if you are interested in the meaning of each property.
 
-The example below presents all the available options:
+The example below presents all the available options, if we connect to Qdrant server:
 
 ```yaml
 embeddings:
   path: sentence-transformers/all-MiniLM-L6-v2
   backend: qdrant_txtai.ann.qdrant.Qdrant
   metric: l2 # allowed values: l2 / cosine / ip
   qdrant:
-    host: qdrant.host
+    url: qdrant.host
     port: 6333
     grpc_port: 6334
     prefer_grpc: true
     collection: CustomCollectionName
     https: true # for Qdrant Cloud
     api_key: XYZ # for Qdrant Cloud
     hnsw:
       m: 8
       ef_construct: 256
       full_scan_threshold:
       ef_search: 512
 ```
 
+### Local in-memory/disk-persisted mode
+
+Qdrant Python client, from version 1.1.1, supports local in-memory/disk-persisted mode. 
+That's a good choice for any test scenarios and quick experiments in which you do not 
+plan to store lots of vectors. In such a case spinning a Docker container might be even 
+not required.
+
+#### In-memory storage
+
+In case you want to have a transient storage, for example in case of automated tests 
+launched during your CI/CD pipeline, using Qdrant Local mode with in-memory storage 
+might be a preferred option.
+
+```yaml
+embeddings:
+  path: sentence-transformers/all-MiniLM-L6-v2
+  backend: qdrant_txtai.ann.qdrant.Qdrant
+  metric: l2 # allowed values: l2 / cosine / ip
+  qdrant:
+    location: ':memory:'
+    prefer_grpc: true
+```
+
+#### On disk storage
+
+However, if you prefer to keep the vectors between different runs of your application, 
+it might be better to use on disk storage and pass the path that should be used to 
+persist the data.
+
+```yaml
+embeddings:
+  path: sentence-transformers/all-MiniLM-L6-v2
+  backend: qdrant_txtai.ann.qdrant.Qdrant
+  metric: l2 # allowed values: l2 / cosine / ip
+  qdrant:
+    path: '/home/qdrant/storage_local'
+    prefer_grpc: true
+```
+
```

