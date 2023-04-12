# Comparing `tmp/replicate-0.7.0.tar.gz` & `tmp/replicate-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate-0.7.0.tar", last modified: Thu Apr  6 02:03:25 2023, max compression
+gzip compressed data, was "replicate-0.8.0.tar", last modified: Wed Apr 12 11:41:19 2023, max compression
```

## Comparing `replicate-0.7.0.tar` & `replicate-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 02:03:25.452797 replicate-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-04-06 02:03:15.000000 replicate-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-04-06 02:03:25.452797 replicate-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-04-06 02:03:15.000000 replicate-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 02:03:25.448797 replicate-0.7.0/replicate/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      980 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/training.py
--rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-04-06 02:03:15.000000 replicate-0.7.0/replicate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 02:03:25.448797 replicate-0.7.0/replicate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-04-06 02:03:25.000000 replicate-0.7.0/replicate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-06 02:03:25.000000 replicate-0.7.0/replicate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 02:03:25.000000 replicate-0.7.0/replicate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-06 02:03:25.000000 replicate-0.7.0/replicate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-06 02:03:25.000000 replicate-0.7.0/replicate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-06 02:03:25.452797 replicate-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-04-06 02:03:15.000000 replicate-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 02:03:25.452797 replicate-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-04-06 02:03:15.000000 replicate-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      916 2023-04-06 02:03:15.000000 replicate-0.7.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4944 2023-04-06 02:03:15.000000 replicate-0.7.0/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)     8617 2023-04-06 02:03:15.000000 replicate-0.7.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-04-12 11:41:10.000000 replicate-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18309 2023-04-12 11:41:19.023656 replicate-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-04-12 11:41:10.000000 replicate-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-04-12 11:41:10.000000 replicate-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/replicate/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1521 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2667 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-04-12 11:41:10.000000 replicate-0.8.0/replicate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/replicate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    18309 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 11:41:19.000000 replicate-0.8.0/replicate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 11:41:19.023656 replicate-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:41:19.023656 replicate-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      916 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8618 2023-04-12 11:41:10.000000 replicate-0.8.0/tests/test_version.py
```

### Comparing `replicate-0.7.0/LICENSE` & `replicate-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate-0.7.0/PKG-INFO` & `replicate-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: replicate
-Version: 0.7.0
-Summary: Python client for Replicate
-Home-page: https://github.com/replicate/replicate-python
-Author: Replicate, Inc.
-License: BSD
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Replicate Python client
 
 This is a Python client for [Replicate](https://replicate.com). It lets you run models from your Python code or Jupyter notebook, and do various other things on Replicate.
 
 ## Install
 
 ```sh
```

### Comparing `replicate-0.7.0/replicate/client.py` & `replicate-0.8.0/replicate/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import re
 from json import JSONDecodeError
-from typing import Any, Iterator, Union
+from typing import Any, Dict, Iterator, Optional, Union
 
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
 from replicate.__about__ import __version__
 from replicate.exceptions import ModelError, ReplicateError
 from replicate.model import ModelCollection
 from replicate.prediction import PredictionCollection
 from replicate.training import TrainingCollection
 
 
 class Client:
-    def __init__(self, api_token=None) -> None:
+    def __init__(self, api_token: Optional[str] = None) -> None:
         super().__init__()
         # Client is instantiated at import time, so do as little as possible.
         # This includes resolving environment variables -- they might be set programmatically.
         self.api_token = api_token
         self.base_url = os.environ.get(
             "REPLICATE_API_BASE_URL", "https://api.replicate.com"
         )
@@ -26,15 +26,15 @@
 
         # TODO: make thread safe
         self.read_session = requests.Session()
         read_retries = Retry(
             total=5,
             backoff_factor=2,
             # Only retry 500s on GET so we don't unintionally mutute data
-            method_whitelist=["GET"],
+            allowed_methods=["GET"],
             # https://support.cloudflare.com/hc/en-us/articles/115003011431-Troubleshooting-Cloudflare-5XX-errors
             status_forcelist=[
                 429,
                 500,
                 502,
                 503,
                 504,
@@ -50,22 +50,22 @@
         self.read_session.mount("http://", HTTPAdapter(max_retries=read_retries))
         self.read_session.mount("https://", HTTPAdapter(max_retries=read_retries))
 
         self.write_session = requests.Session()
         write_retries = Retry(
             total=5,
             backoff_factor=2,
-            method_whitelist=["POST", "PUT"],
+            allowed_methods=["POST", "PUT"],
             # Only retry POST/PUT requests on rate limits, so we don't unintionally mutute data
             status_forcelist=[429],
         )
         self.write_session.mount("http://", HTTPAdapter(max_retries=write_retries))
         self.write_session.mount("https://", HTTPAdapter(max_retries=write_retries))
 
-    def _request(self, method: str, path: str, **kwargs):
+    def _request(self, method: str, path: str, **kwargs) -> requests.Response:
         # from requests.Session
         if method in ["GET", "OPTIONS"]:
             kwargs.setdefault("allow_redirects", True)
         if method in ["HEAD"]:
             kwargs.setdefault("allow_redirects", False)
         kwargs.setdefault("headers", {})
         kwargs["headers"].update(self._headers())
@@ -77,21 +77,21 @@
             try:
                 raise ReplicateError(resp.json()["detail"])
             except (JSONDecodeError, KeyError):
                 pass
             raise ReplicateError(f"HTTP error: {resp.status_code, resp.reason}")
         return resp
 
-    def _headers(self):
+    def _headers(self) -> Dict[str, str]:
         return {
             "Authorization": f"Token {self._api_token()}",
             "User-Agent": f"replicate-python@{__version__}",
         }
 
-    def _api_token(self):
+    def _api_token(self) -> str:
         token = self.api_token
         # Evaluate lazily in case environment variable is set with dotenv, or something
         if token is None:
             token = os.environ.get("REPLICATE_API_TOKEN")
         if not token:
             raise ReplicateError(
                 """No API token provided. You need to set the REPLICATE_API_TOKEN environment variable or create a client with `replicate.Client(api_token=...)`.
@@ -108,15 +108,15 @@
     def predictions(self) -> PredictionCollection:
         return PredictionCollection(client=self)
 
     @property
     def trainings(self) -> TrainingCollection:
         return TrainingCollection(client=self)
 
-    def run(self, model_version, **kwargs) -> Union[Any, Iterator[Any]]:
+    def run(self, model_version: str, **kwargs) -> Union[Any, Iterator[Any]]:
         """
         Run a model in the format owner/name:version.
         """
         # Split model_version into owner, name, version in format owner/name:version
         m = re.match(r"^(?P<model>[^/]+/[^:]+):(?P<version>.+)$", model_version)
         if not m:
             raise ReplicateError(
```

### Comparing `replicate-0.7.0/replicate/files.py` & `replicate-0.8.0/replicate/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import base64
 import io
 import mimetypes
 import os
+from typing import Optional
 
 import requests
 
 
-def upload_file(fh: io.IOBase, output_file_prefix: str = None) -> str:
+def upload_file(fh: io.IOBase, output_file_prefix: Optional[str] = None) -> str:
     """
     Lifted straight from cog.files
     """
     fh.seek(0)
 
     if output_file_prefix is not None:
         name = getattr(fh, "name", "output")
         url = output_file_prefix + os.path.basename(name)
-        resp = requests.put(url, files={"file": fh})
+        resp = requests.put(url, files={"file": fh}, timeout=None)
         resp.raise_for_status()
         return url
 
     b = fh.read()
     # The file handle is strings, not bytes
     if isinstance(b, str):
         b = b.encode("utf-8")
```

### Comparing `replicate-0.7.0/replicate/json.py` & `replicate-0.8.0/replicate/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import io
 from pathlib import Path
 from types import GeneratorType
 from typing import Any, Callable
 
-
 try:
     import numpy as np  # type: ignore
 
     has_numpy = True
 except ImportError:
     has_numpy = False
 
 
-def encode_json(obj: Any, upload_file: Callable[[io.IOBase], str]) -> Any:
+def encode_json(
+    obj: Any, upload_file: Callable[[io.IOBase], str]  # noqa: ANN401
+) -> Any:  # noqa: ANN401
     """
     Returns a JSON-compatible version of the object. Effectively the same thing as cog.json.encode_json.
     """
     if isinstance(obj, dict):
         return {key: encode_json(value, upload_file) for key, value in obj.items()}
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         return [encode_json(value, upload_file) for value in obj]
```

### Comparing `replicate-0.7.0/replicate/prediction.py` & `replicate-0.8.0/replicate/prediction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 from typing import Any, Dict, Iterator, List, Optional
 
 from replicate.base_model import BaseModel
 from replicate.collection import Collection
-from replicate.exceptions import ModelError, ReplicateException
+from replicate.exceptions import ModelError
 from replicate.files import upload_file
 from replicate.json import encode_json
 from replicate.version import Version
 
 
 class Prediction(BaseModel):
     id: str
@@ -17,15 +17,15 @@
     output: Optional[Any]
     status: str
     version: Optional[Version]
     started_at: Optional[str]
     created_at: Optional[str]
     completed_at: Optional[str]
 
-    def wait(self):
+    def wait(self) -> None:
         """Wait for prediction to finish."""
         while self.status not in ["succeeded", "failed", "canceled"]:
             time.sleep(self._client.poll_interval)
             self.reload()
 
     def output_iterator(self) -> Iterator[Any]:
         # TODO: check output is list
@@ -43,29 +43,46 @@
             raise ModelError(self.error)
 
         output = self.output or []
         new_output = output[len(previous_output) :]
         for output in new_output:
             yield output
 
-    def cancel(self):
+    def cancel(self) -> None:
         """Cancel a currently running prediction"""
         self._client._request("POST", f"/v1/predictions/{self.id}/cancel")
 
 
 class PredictionCollection(Collection):
     model = Prediction
 
-    def create(
+    def list(self) -> List[Prediction]:
+        resp = self._client._request("GET", "/v1/predictions")
+        # TODO: paginate
+        predictions = resp.json()["results"]
+        for prediction in predictions:
+            # HACK: resolve this? make it lazy somehow?
+            del prediction["version"]
+        return [self.prepare_model(obj) for obj in predictions]
+
+    def get(self, id: str) -> Prediction:
+        resp = self._client._request("GET", f"/v1/predictions/{id}")
+        obj = resp.json()
+        # HACK: resolve this? make it lazy somehow?
+        del obj["version"]
+        return self.prepare_model(obj)
+
+    def create(  # type: ignore
         self,
         version: Version,
         input: Dict[str, Any],
         webhook: Optional[str] = None,
         webhook_completed: Optional[str] = None,
         webhook_events_filter: Optional[List[str]] = None,
+        **kwargs,
     ) -> Prediction:
         input = encode_json(input, upload_file=upload_file)
         body = {
             "version": version.id,
             "input": input,
         }
         if webhook is not None:
@@ -79,23 +96,7 @@
             "POST",
             "/v1/predictions",
             json=body,
         )
         obj = resp.json()
         obj["version"] = version
         return self.prepare_model(obj)
-
-    def get(self, id: str) -> Prediction:
-        resp = self._client._request("GET", f"/v1/predictions/{id}")
-        obj = resp.json()
-        # HACK: resolve this? make it lazy somehow?
-        del obj["version"]
-        return self.prepare_model(obj)
-
-    def list(self) -> List[Prediction]:
-        resp = self._client._request("GET", f"/v1/predictions")
-        # TODO: paginate
-        predictions = resp.json()["results"]
-        for prediction in predictions:
-            # HACK: resolve this? make it lazy somehow?
-            del prediction["version"]
-        return [self.prepare_model(obj) for obj in predictions]
```

### Comparing `replicate-0.7.0/replicate/schema.py` & `replicate-0.8.0/replicate/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from packaging import version
 
 # TODO: this code is shared with replicate's backend. Maybe we should put it in the Cog Python package as the source of truth?
 
 
-def version_has_no_array_type(cog_version):
+def version_has_no_array_type(cog_version: str) -> bool:
     """Iterators have x-cog-array-type=iterator in the schema from 0.3.9 onward"""
     return version.parse(cog_version) < version.parse("0.3.9")
 
 
-def make_schema_backwards_compatible(schema, version):
+def make_schema_backwards_compatible(
+    schema: dict,
+    version: str,
+) -> dict:
     """A place to add backwards compatibility logic for our openapi schema"""
     # If the top-level output is an array, assume it is an iterator in old versions which didn't have an array type
     if version_has_no_array_type(version):
         output = schema["components"]["schemas"]["Output"]
         if output.get("type") == "array":
             output["x-cog-array-type"] = "iterator"
     return schema
```

### Comparing `replicate-0.7.0/replicate/training.py` & `replicate-0.8.0/replicate/training.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import re
-import time
-from typing import Any, Dict, Iterator, List, Optional
+from typing import Any, Dict, List, Optional
 
 from replicate.base_model import BaseModel
 from replicate.collection import Collection
-from replicate.exceptions import ModelError, ReplicateException
+from replicate.exceptions import ReplicateException
 from replicate.files import upload_file
 from replicate.json import encode_json
-from replicate.version import Version
 
 
 class Training(BaseModel):
     completed_at: Optional[str]
     created_at: Optional[str]
     destination: Optional[str]
     error: Optional[str]
@@ -19,29 +17,47 @@
     input: Optional[Dict[str, Any]]
     logs: Optional[str]
     output: Optional[Any]
     started_at: Optional[str]
     status: str
     version: str
 
-    def cancel(self):
+    def cancel(self) -> None:
         """Cancel a running training"""
         self._client._request("POST", f"/v1/trainings/{self.id}/cancel")
 
 
 class TrainingCollection(Collection):
     model = Training
 
-    def create(
+    def list(self) -> List[Training]:
+        resp = self._client._request("GET", "/v1/trainings")
+        # TODO: paginate
+        trainings = resp.json()["results"]
+        for training in trainings:
+            # HACK: resolve this? make it lazy somehow?
+            del training["version"]
+        return [self.prepare_model(obj) for obj in trainings]
+
+    def get(self, id: str) -> Training:
+        resp = self._client._request(
+            "GET",
+            f"/v1/trainings/{id}",
+        )
+        obj = resp.json()
+        return self.prepare_model(obj)
+
+    def create(  # type: ignore
         self,
         version: str,
         input: Dict[str, Any],
         destination: str,
         webhook: Optional[str] = None,
         webhook_events_filter: Optional[List[str]] = None,
+        **kwargs,
     ) -> Training:
         input = encode_json(input, upload_file=upload_file)
         body = {
             "input": input,
             "destination": destination,
         }
         if webhook is not None:
@@ -51,28 +67,20 @@
 
         # Split version in format "username/model_name:version_id"
         match = re.match(
             r"^(?P<username>[^/]+)/(?P<model_name>[^:]+):(?P<version_id>.+)$", version
         )
         if not match:
             raise ReplicateException(
-                f"version must be in format username/model_name:version_id"
+                "version must be in format username/model_name:version_id"
             )
         username = match.group("username")
         model_name = match.group("model_name")
         version_id = match.group("version_id")
 
         resp = self._client._request(
             "POST",
             f"/v1/models/{username}/{model_name}/versions/{version_id}/trainings",
             json=body,
         )
         obj = resp.json()
         return self.prepare_model(obj)
-
-    def get(self, id: str) -> Training:
-        resp = self._client._request(
-            "GET",
-            f"/v1/trainings/{id}",
-        )
-        obj = resp.json()
-        return self.prepare_model(obj)
```

### Comparing `replicate-0.7.0/replicate/version.py` & `replicate-0.8.0/replicate/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import datetime
 import warnings
-from typing import Any, Iterator, List, Union
+from typing import TYPE_CHECKING, Any, Iterator, List, Union
+
+if TYPE_CHECKING:
+    from replicate.client import Client
+    from replicate.model import Model
+
 
 from replicate.base_model import BaseModel
 from replicate.collection import Collection
 from replicate.exceptions import ModelError
 from replicate.schema import make_schema_backwards_compatible
 
 
 class Version(BaseModel):
     id: str
     created_at: datetime.datetime
     cog_version: str
-    openapi_schema: Any
+    openapi_schema: dict
 
     def predict(self, **kwargs) -> Union[Any, Iterator[Any]]:
         warnings.warn(
             "version.predict() is deprecated. Use replicate.run() instead. It will be removed before version 1.0.",
             DeprecationWarning,
+            stacklevel=1,
         )
 
         prediction = self._client.predictions.create(version=self, input=kwargs)
         # Return an iterator of the output
         schema = self.get_transformed_schema()
         output = schema["components"]["schemas"]["Output"]
         if (
@@ -31,37 +37,40 @@
             return prediction.output_iterator()
 
         prediction.wait()
         if prediction.status == "failed":
             raise ModelError(prediction.error)
         return prediction.output
 
-    def get_transformed_schema(self):
+    def get_transformed_schema(self) -> dict:
         schema = self.openapi_schema
         schema = make_schema_backwards_compatible(schema, self.cog_version)
         return schema
 
 
 class VersionCollection(Collection):
     model = Version
 
-    def __init__(self, client, model):
+    def __init__(self, client: "Client", model: "Model") -> None:
         super().__init__(client=client)
         self._model = model
 
     # doesn't exist yet
     def get(self, id: str) -> Version:
         """
         Get a specific version.
         """
         resp = self._client._request(
             "GET", f"/v1/models/{self._model.username}/{self._model.name}/versions/{id}"
         )
         return self.prepare_model(resp.json())
 
+    def create(self, **kwargs) -> Version:
+        raise NotImplementedError()
+
     def list(self) -> List[Version]:
         """
         Return a list of all versions for a model.
         """
         resp = self._client._request(
             "GET", f"/v1/models/{self._model.username}/{self._model.name}/versions"
         )
```

### Comparing `replicate-0.7.0/replicate.egg-info/SOURCES.txt` & `replicate-0.8.0/replicate.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 replicate/__about__.py
 replicate/__init__.py
 replicate/base_model.py
 replicate/client.py
 replicate/collection.py
 replicate/exceptions.py
 replicate/files.py
@@ -18,8 +18,9 @@
 replicate.egg-info/SOURCES.txt
 replicate.egg-info/dependency_links.txt
 replicate.egg-info/requires.txt
 replicate.egg-info/top_level.txt
 tests/test_client.py
 tests/test_model.py
 tests/test_prediction.py
+tests/test_training.py
 tests/test_version.py
```

### Comparing `replicate-0.7.0/tests/test_client.py` & `replicate-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `replicate-0.7.0/tests/test_model.py` & `replicate-0.8.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.7.0/tests/test_prediction.py` & `replicate-0.8.0/tests/test_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import responses
 from responses import matchers
 
-import replicate
-
 from .factories import create_client, create_version
 
 
 @responses.activate
 def test_create_works_with_webhooks():
     client = create_client()
     version = create_version(client)
@@ -37,15 +35,15 @@
             "input": {"text": "world"},
             "output": None,
             "error": None,
             "logs": "",
         },
     )
 
-    prediction = client.predictions.create(
+    client.predictions.create(
         version=version,
         input={"text": "world"},
         webhook="https://example.com/webhook",
         webhook_events_filter=["completed"],
     )
 
     assert rsp.call_count == 1
@@ -152,13 +150,13 @@
     prediction = client.predictions.create(
         version=version,
         input={"text": "hello"},
         webhook_completed="https://example.com/webhook",
     )
 
     assert prediction.created_at == "2022-04-26T20:00:40.658234Z"
-    assert prediction.completed_at == None
-    assert prediction.output == None
+    assert prediction.completed_at is None
+    assert prediction.output is None
     prediction.wait()
     assert prediction.created_at == "2022-04-26T20:00:40.658234Z"
     assert prediction.completed_at == "2022-04-26T20:02:27.648305Z"
     assert prediction.output == "hello world"
```

### Comparing `replicate-0.7.0/tests/test_version.py` & `replicate-0.8.0/tests/test_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Iterable
 
 import pytest
 import responses
-from replicate.exceptions import ModelError
 from responses import matchers
 
+from replicate.exceptions import ModelError
+
 from .factories import (
     create_version,
     create_version_with_iterator_output,
     create_version_with_iterator_output_backwards_compatibility_0_3_8,
     create_version_with_list_output,
 )
```

