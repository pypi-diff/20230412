# Comparing `tmp/flow360-0.1.8.tar.gz` & `tmp/flow360-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.1.8.tar", max compression
+gzip compressed data, was "flow360-0.2.0b1.tar", max compression
```

## Comparing `flow360-0.1.8.tar` & `flow360-0.2.0b1.tar`

### file list

```diff
@@ -1,21 +1,57 @@
--rw-r--r--   0        0        0    26526 2023-03-21 19:02:37.356707 flow360-0.1.8/LICENSE
--rw-r--r--   0        0        0      345 2023-03-21 19:02:37.356707 flow360-0.1.8/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-03-21 19:02:37.356707 flow360-0.1.8/flow360/cli/__init__.py
--rw-r--r--   0        0        0     1126 2023-03-21 19:02:37.356707 flow360-0.1.8/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-03-21 19:02:37.356707 flow360-0.1.8/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     2469 2023-03-21 19:02:37.356707 flow360-0.1.8/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1492 2023-03-21 19:02:37.356707 flow360-0.1.8/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     8981 2023-03-21 19:02:37.356707 flow360-0.1.8/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      672 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/component/__init__.py
--rw-r--r--   0        0        0    21896 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/component/case.py
--rw-r--r--   0        0        0     4483 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/component/flow360_base_model.py
--rw-r--r--   0        0        0     6911 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/component/flow360_solver_params.py
--rw-r--r--   0        0        0     4440 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0      338 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/component/utils.py
--rw-r--r--   0        0        0    18766 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2075 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/environment.py
--rw-r--r--   0        0        0     1146 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/solver_version.py
--rw-r--r--   0        0        0       38 2023-03-21 19:02:37.360707 flow360-0.1.8/flow360/version.py
--rw-r--r--   0        0        0     1439 2023-03-21 19:02:53.468925 flow360-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 flow360-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-04-12 14:58:52.250627 flow360-0.2.0b1/LICENSE
+-rw-r--r--   0        0        0     1473 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     1126 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     2869 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1466 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     8842 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      687 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/__init__.py
+-rw-r--r--   0        0        0    22372 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/constants.py
+-rw-r--r--   0        0        0    32080 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/flow360_params.py
+-rw-r--r--   0        0        0      220 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     6145 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0    18009 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/params_base.py
+-rw-r--r--   0        0        0     7550 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    10105 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2326 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/types.py
+-rw-r--r--   0        0        0     1019 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/utils.py
+-rw-r--r--   0        0        0     2940 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/validator.py
+-rw-r--r--   0        0        0    21661 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2137 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/environment.py
+-rw-r--r--   0        0        0      237 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5515 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-04-12 14:58:52.258627 flow360-0.2.0b1/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-04-12 14:58:52.262627 flow360-0.2.0b1/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0     2305 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1354 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/exceptions.py
+-rw-r--r--   0        0        0     5810 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/solver_version.py
+-rw-r--r--   0        0        0       38 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/version.py
+-rw-r--r--   0        0        0     1480 2023-04-12 14:59:09.794860 flow360-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 flow360-0.2.0b1/PKG-INFO
```

### Comparing `flow360-0.1.8/LICENSE` & `flow360-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.1.8/flow360/cli/app.py` & `flow360-0.2.0b1/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.1.8/flow360/cloud/http_util.py` & `flow360-0.2.0b1/flow360/cloud/http_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 """
 from functools import wraps
 
 import requests
 
 from ..environment import Env
 from ..version import __version__
+from ..exceptions import AuthorisationError, WebNotFoundError, WebError
+from ..log import log
 
 from .security import api_key
 
 
 def api_key_auth(request):
     """
     Set the authentication.
     :param request:
     :return:
     """
-    key = api_key()
+    key = api_key(Env.current.apikey_profile)
     if not key:
         raise ValueError("API key not found, please set it by commandline: flow360 configure.")
     request.headers["simcloud-api-key"] = key
     request.headers["flow360-python-version"] = __version__
     return request
 
 
@@ -34,26 +36,32 @@
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         """A wrapper function"""
 
         # Extend some capabilities of func
+        log.debug(f"call: {func.__name__}({args}, {kwargs})")
+
         resp = func(*args, **kwargs)
+
+        if resp.status_code == 400:
+            raise WebError(f"Web {args[1]}: Bad request error: {resp.json()['error']}")
+
         if resp.status_code == 401:
-            raise Exception("Unauthorized.")
+            raise AuthorisationError("Unauthorized.")
 
         if resp.status_code == 404:
-            return None
+            raise WebNotFoundError(f"Web {args[1]}: Not found error: {resp.json()}")
 
         if resp.status_code == 200:
             result = resp.json()
             return result.get("data")
 
-        raise Exception(f"Unexpected response: {resp.status_code}")
+        raise Exception(f"Web {args[1]}: Unexpected response error: {resp.status_code}")
 
     return wrapper
 
 
 class Http:
     """
     Http util class.
@@ -67,15 +75,15 @@
         """
         Get the resource.
         :param path:
         :param json:
         :return:
         """
         return self.session.get(
-            url=Env.current.get_real_url(path), auth=api_key_auth, json=json, params=params
+            url=Env.current.get_real_url(path), json=json, params=params, auth=api_key_auth
         )
 
     @http_interceptor
     def post(self, path: str, json=None):
         """
         Create the resource.
         :param path:
```

### Comparing `flow360-0.1.8/flow360/cloud/rest_api.py` & `flow360-0.2.0b1/flow360/cloud/rest_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     """
 
     # pylint: disable=redefined-builtin
     def __init__(self, endpoint, id=None):
         is_valid_uuid(id, ignore_none=True)
         self._id = id
         self._endpoint = endpoint
-        self._info = None
 
     def _url(self, method):
         url = f"{self._endpoint}"
         if self._id is not None:
             url += f"/{self._id}"
         if method is not None:
             url += f"/{method}"
```

### Comparing `flow360-0.1.8/flow360/cloud/s3_utils.py` & `flow360-0.2.0b1/flow360/cloud/s3_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,31 +155,28 @@
     """
     Enum for s3 transfer type
     """
 
     VOLUME_MESH = "VolumeMesh"
     SURFACE_MESH = "SurfaceMesh"
     CASE = "Case"
-    STUDIO = "Studio"
 
     def _get_grant_url(self, resource_id, file_name: str) -> str:
         """
         Get the grant url for a file.
         :param resource_id:
         :param file_name:
         :return:
         """
         if self is S3TransferType.VOLUME_MESH:
             return f"volumemeshes/{resource_id}/file?filename={file_name}"
         if self is S3TransferType.SURFACE_MESH:
             return f"surfacemeshes/{resource_id}/file?filename={file_name}"
         if self is S3TransferType.CASE:
             return f"cases/{resource_id}/file?filename={file_name}"
-        if self is S3TransferType.STUDIO:
-            return f"volumemeshes/{resource_id}/file?filename={file_name}"
 
         return None
 
     def upload_file(
         self, resource_id: str, remote_file_name: str, file_name: str, progress_callback=None
     ):
         """
```

### Comparing `flow360-0.1.8/flow360/component/case.py` & `flow360-0.2.0b1/flow360/component/case.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,285 +1,376 @@
 """
 Case component
 """
 from __future__ import annotations
 import json
 from enum import Enum
-from pydantic import Extra, Field
+from typing import Iterator, List
+from pydantic import Field
 from pylab import show, subplots
 
 from ..cloud.s3_utils import S3TransferType, CloudFileNotFoundError
 from ..cloud.rest_api import RestApi
-from .flow360_base_model import (
-    Flow360BaseModel,
+from .resource_base import (
+    Flow360ResourceBaseModel,
     Flow360Resource,
+    Flow360ResourceListBase,
+    ResourceDraft,
     before_submit_only,
-    on_cloud_resource_only,
     is_object_cloud_resource,
 )
-from .flow360_solver_params import Flow360Params
+from .flow360_params import Flow360Params
 from .utils import is_valid_uuid
+from .validator import Validator
 
 
-class CaseMeta(Flow360BaseModel, extra=Extra.allow):
+class CaseBase:
     """
-    Case component
+    Case Base component
+    """
+
+    _endpoint = "cases"
+
+    def copy(
+        self, name: str = None, params: Flow360Params = None, tags: List[str] = None
+    ) -> CaseDraft:
+        """
+        Alias for retry case
+        :param name:
+        :param params:
+        :param tags:
+        :return:
+        """
+
+        return self.retry(name, params, tags)
+
+    # pylint: disable=no-member
+    def retry(
+        self, name: str = None, params: Flow360Params = None, tags: List[str] = None
+    ) -> CaseDraft:
+        """
+        Retry case
+        :param name:
+        :param params:
+        :param tags:
+        :return:
+        """
+
+        name = name or self.name or self.info.name
+        params = params or self.params.copy(deep=True)
+        new_case = Case.new(name, params, other_case=self, tags=tags)
+        return new_case
+
+    def continuation(
+        self, name: str = None, params: Flow360Params = None, tags: List[str] = None
+    ) -> Case:
+        """
+        Alias for fork a case to continue simulation
+        :param name:
+        :param params:
+        :param tags:
+        :return:
+        """
+
+        return self.fork(name, params, tags)
+
+    # pylint: disable=no-member
+    def fork(
+        self, name: str = None, params: Flow360Params = None, tags: List[str] = None
+    ) -> CaseDraft:
+        """
+        Fork a case to continue simulation
+        :param name:
+        :param params:
+        :param tags:
+        :return:
+        """
+
+        name = name or self.name or self.info.name
+        params = params or self.params.copy(deep=True)
+        return Case.new(name, params, parent_case=self, tags=tags)
+
+
+class CaseMeta(Flow360ResourceBaseModel):
+    """
+    CaseMeta data component
     """
 
     id: str = Field(alias="caseId")
     case_mesh_id: str = Field(alias="caseMeshId")
-    status: str = Field(alias="caseStatus")
     parent_id: str = Field(alias="parentId")
 
     def to_case(self) -> Case:
         """
         returns Case object from case meta info
         """
         return Case(self.id)
 
 
 # pylint: disable=too-many-instance-attributes
-class Case(Flow360Resource):
+class CaseDraft(CaseBase, ResourceDraft):
     """
-    Case component
+    Case Draft component (before submission)
     """
 
-    def __init__(self, case_id: str = None):
-        super().__init__(
-            resource_type="Case",
-            info_type_class=CaseMeta,
-            s3_transfer_method=S3TransferType.CASE,
-            endpoint="case",
-            id=case_id,
-        )
-        if case_id is not None:
-            self.get_info()
-            self._params = Flow360Params(**json.loads(self.get(method="runtimeParams")["content"]))
-
+    def __init__(self):
         self.other_case = None
         self.parent_case = None
         self.parent_id = None
         self.tags = None
-        self._results = CaseResults(self)
+        self._id = None
+        self._submitted_case = None
 
     def __str__(self):
-        if self._info is not None:
-            return self.info.__str__()
-        return "Case is not yet submitted"
+        return self.params.__str__()
 
     @property
-    def params(self):
+    def params(self) -> Flow360Params:
         """
         returns case params
         """
         return self._params
 
     @params.setter
-    @before_submit_only
-    def params(self, value):
+    def params(self, value: Flow360Params):
         """
         sets case params (before submit only)
         """
         if not isinstance(value, Flow360Params):
             raise ValueError("params are not of type Flow360Params.")
         self._params = value
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         returns case name
         """
-        if self.is_cloud_resource():
-            return self.info.name
         return self._name
 
     @name.setter
-    @before_submit_only
-    def name(self, value):
+    def name(self, value) -> str:
         """
-        sets case name (before submit only)
+        sets case name
         """
         self._name = value
 
     @property
     def volume_mesh_id(self):
         """
-        returns volume mesh id (before submit only)
+        returns volume mesh id
         """
-        if self.is_cloud_resource():
-            return self.info.case_mesh_id
         return self._volume_mesh_id
 
     @volume_mesh_id.setter
-    @before_submit_only
     def volume_mesh_id(self, value):
         """
-        sets volume mesh id (before submit only)
+        sets volume mesh id
         """
         self._volume_mesh_id = value
 
-    @property
-    @on_cloud_resource_only
-    def results(self) -> CaseResults:
-        """
-        returns results object to managing case results
-        """
-        return self._results
-
     @before_submit_only
-    def submit(self):
+    def submit(self) -> Case:
         """
         submits case to cloud for running
         """
         assert self.name
         assert self.volume_mesh_id or self.other_case or self.parent_id or self.parent_case
         assert self.params
 
         self.validate_case_inputs(pre_submit_checks=True)
 
         volume_mesh_id = self.volume_mesh_id
         parent_id = self.parent_id
         if parent_id is not None:
             self.parent_case = Case(self.parent_id)
 
+        if isinstance(self.parent_case, CaseDraft):
+            self.parent_case = Case(self.parent_case.id)
+
+        if isinstance(self.other_case, CaseDraft):
+            self.other_case = Case(self.other_case.id)
+
         if self.parent_case is not None:
             parent_id = self.parent_case.id
             volume_mesh_id = self.parent_case.volume_mesh_id
 
         volume_mesh_id = volume_mesh_id or self.other_case.volume_mesh_id
 
         is_valid_uuid(volume_mesh_id)
         is_valid_uuid(parent_id, ignore_none=True)
+        self.validator_api(self.params, volume_mesh_id=volume_mesh_id)
 
-        resp = self.post(
+        resp = RestApi(self._endpoint).post(
             json={
                 "name": self.name,
                 "meshId": volume_mesh_id,
-                "runtimeParams": self.params.json(),
+                "runtimeParams": self.params.to_flow360_json(),
                 "tags": self.tags,
                 "parentId": parent_id,
             },
             path=f"volumemeshes/{volume_mesh_id}/case",
         )
-        self._info = CaseMeta(**resp)
-        self.init_id(self._info.id)
+        info = CaseMeta(**resp)
+        self._id = info.id
+
+        self._submitted_case = Case(self.id)
+        return self._submitted_case
+
+    def validate_case_inputs(self, pre_submit_checks=False):
+        """
+        validates case inputs (before submit only)
+        """
+        if self.volume_mesh_id is not None and self.other_case is not None:
+            raise ValueError("You cannot specify both volume_mesh_id AND other_case.")
+
+        if self.parent_id is not None and self.parent_case is not None:
+            raise ValueError("You cannot specify both parent_id AND parent_case.")
+
+        if self.parent_id is not None or self.parent_case is not None:
+            if self.volume_mesh_id is not None or self.other_case is not None:
+                raise ValueError(
+                    "You cannot specify volume_mesh_id OR other_case when parent case provided."
+                )
+
+        is_valid_uuid(self.volume_mesh_id, ignore_none=True)
+
+        if pre_submit_checks:
+            is_object_cloud_resource(self.other_case)
+            is_object_cloud_resource(self.parent_case)
+
+    @classmethod
+    def validator_api(cls, params: Flow360Params, volume_mesh_id):
+        """
+        validation api: validates case parameters before submitting
+        """
+        return Validator.CASE.validate(params, mesh_id=volume_mesh_id)
+
+
+# pylint: disable=too-many-instance-attributes
+class Case(CaseBase, Flow360Resource):
+    """
+    Case component
+    """
+
+    def __init__(self, case_id: str = None, meta_info: CaseMeta = None):
+        if (case_id is None and meta_info is None) or (
+            case_id is not None and meta_info is not None
+        ):
+            raise ValueError("You must provide case_id OR meta_info to constructor.")
+
+        if meta_info is not None:
+            case_id = meta_info.id
+
+        assert case_id is not None
+
+        super().__init__(
+            resource_type="Case",
+            info_type_class=CaseMeta,
+            s3_transfer_method=S3TransferType.CASE,
+            endpoint=self._endpoint,
+            id=case_id,
+        )
+
+        if meta_info is not None:
+            self._info = meta_info
+        self._params = None
+        self._results = CaseResults(self)
+
+    @property
+    def params(self) -> Flow360Params:
+        """
+        returns case params
+        """
+        if self._params is None:
+            self._params = Flow360Params(**json.loads(self.get(method="runtimeParams")["content"]))
+        return self._params
+
+    @property
+    def name(self) -> str:
+        """
+        returns case name
+        """
+        return self.info.name
+
+    @property
+    def info(self) -> CaseMeta:
+        """
+        returns metadata info for case
+        """
+        return super().info
+
+    @property
+    def volume_mesh_id(self):
+        """
+        returns volume mesh id
+        """
+        return self.info.case_mesh_id
+
+    @property
+    def results(self) -> CaseResults:
+        """
+        returns results object to managing case results
+        """
+        return self._results
 
-    @on_cloud_resource_only
     def download_log(self, log, to_file=".", keep_folder: bool = True):
         """
         Download log
         :param log:
         :param to_file: file name on local disk, could be either folder or file name.
         :param keep_folder: If true, the downloaded file will be put in the same folder as the file on cloud. Only work
         when file_name is a folder name.
         :return:
         """
 
         self.download_file(f"logs/{log.value}", to_file, keep_folder)
 
-    @on_cloud_resource_only
-    def is_case_steady(self):
+    def is_steady(self):
         """
         returns True when case is steady state
         """
         return self.params.time_stepping.time_step_size == "inf"
 
-    @on_cloud_resource_only
     def has_actuator_disks(self):
         """
         returns True when case has actuator disk
         """
         if self.params.actuator_disks is not None:
             if len(self.params.actuator_disks) > 0:
                 return True
         return False
 
-    @on_cloud_resource_only
     def has_bet_disks(self):
         """
         returns True when case has BET disk
         """
         if self.params.bet_disks is not None:
             if len(self.params.bet_disks) > 0:
                 return True
         return False
 
-    def copy(self, name: str = None, params: Flow360Params = None, tags: [str] = None) -> Case:
-        """
-        Alias for retry case
-        :param name:
-        :param params:
-        :param tags:
-        :return:
-        """
-
-        return self.retry(name, params, tags)
-
-    def retry(self, name: str = None, params: Flow360Params = None, tags: [str] = None) -> Case:
-        """
-        Retry case
-        :param name:
-        :param params:
-        :param tags:
-        :return:
-        """
-
-        name = name or self.name or self.info.name
-        params = params or self.params.copy(deep=True)
-        new_case = Case.new(name, params, other_case=self, tags=tags)
-        return new_case
-
-    def continuation(
-        self, name: str = None, params: Flow360Params = None, tags: [str] = None
-    ) -> Case:
+    def is_finished(self):
         """
-        Alias for fork a case to continue simulation
-        :param name:
-        :param params:
-        :param tags:
-        :return:
+        returns False when case is in running or preprocessing state
         """
+        return self.status.is_final()
 
-        return self.fork(name, params, tags)
-
-    def fork(self, name: str = None, params: Flow360Params = None, tags: [str] = None) -> Case:
+    @classmethod
+    def _meta_class(cls):
         """
-        Fork a case to continue simulation
-        :param name:
-        :param params:
-        :param tags:
-        :return:
+        returns case meta info class: CaseMeta
         """
+        return CaseMeta
 
-        name = name or self.name or self.info.name
-        params = params or self.params.copy(deep=True)
-        return Case.new(name, params, parent_case=self, tags=tags)
-
-    @before_submit_only
-    def validate_case_inputs(self, pre_submit_checks=False):
+    @classmethod
+    def _params_ancestor_id_name(cls):
         """
-        validates case inputs (before submit only)
+        returns volumeMeshId name
         """
-        if self.volume_mesh_id is not None and self.other_case is not None:
-            raise ValueError("You cannot specify both volume_mesh_id AND other_case.")
-
-        if self.parent_id is not None and self.parent_case is not None:
-            raise ValueError("You cannot specify both parent_id AND parent_case.")
-
-        if self.parent_id is not None or self.parent_case is not None:
-            if self.volume_mesh_id is not None or self.other_case is not None:
-                raise ValueError(
-                    "You cannot specify volume_mesh_id OR other_case when parent case provided."
-                )
-
-        is_valid_uuid(self.volume_mesh_id, ignore_none=True)
-
-        if pre_submit_checks:
-            is_object_cloud_resource(self.other_case)
-            is_object_cloud_resource(self.parent_case)
+        return "meshId"
 
     @classmethod
     def from_cloud(cls, case_id: str):
         """
         get case from cloud
         """
         return cls(case_id)
@@ -287,19 +378,19 @@
     # pylint: disable=too-many-arguments
     @classmethod
     def new(
         cls,
         name: str,
         params: Flow360Params,
         volume_mesh_id: str = None,
-        tags: [str] = None,
+        tags: List[str] = None,
         parent_id=None,
         other_case: Case = None,
         parent_case: Case = None,
-    ) -> Case:
+    ) -> CaseDraft:
         """
         Create new case
         :param name:
         :param params:
         :param volume_mesh_id:
         :param other_case:
         :param tags:
@@ -311,79 +402,27 @@
         assert name
         assert volume_mesh_id or other_case or parent_id or parent_case
         assert params
 
         if not isinstance(params, Flow360Params):
             raise ValueError("params are not of type Flow360Params.")
 
-        new_case = cls()
+        new_case = CaseDraft()
         new_case.name = name
         new_case.volume_mesh_id = volume_mesh_id
         new_case.other_case = other_case
         new_case.params = params.copy(deep=True)
         new_case.tags = tags
         new_case.parent_id = parent_id
         new_case.parent_case = parent_case
 
         new_case.validate_case_inputs()
 
         return new_case
 
-    # pylint: disable=too-many-arguments
-    # @classmethod
-    # def submit_multiple_phases(
-    #     cls,
-    #     name: str,
-    #     volume_mesh_id: str,
-    #     params: Flow360Params,
-    #     tags: [str] = None,
-    #     phase_steps=1,
-    # ):
-    #     """
-    #     Create multiple cases from volume mesh
-    #     :param name:
-    #     :param volume_mesh_id:
-    #     :param params:
-    #     :param tags:
-    #     :param parent_id:
-    #     :param phase_steps:
-    #     :return:
-    #     """
-
-    #     assert name
-    #     assert volume_mesh_id
-    #     assert params
-    #     assert phase_steps >= 1
-
-    #     result = []
-
-    #     total_steps = (
-    #         params.time_stepping.max_physical_steps
-    #         if params.time_stepping and params.time_stepping.max_physical_steps
-    #         else 1
-    #     )
-
-    #     num_cases = math.ceil(total_steps / phase_steps)
-    #     for i in range(1, num_cases + 1):
-    #         parent_id = result[-1].case_id if result else None
-    #         case = http.post(
-    #             f"volumemeshes/{volume_mesh_id}/case",
-    #             json={
-    #                 "name": f"{name}_{i}",
-    #                 "meshId": volume_mesh_id,
-    #                 "runtimeParams": params.json(),
-    #                 "tags": tags,
-    #                 "parentId": parent_id,
-    #             },
-    #         )
-
-    #         result.append(cls(**case))
-
-    #     return result
-
 
 class CaseResultType(Enum):
     """
     Case results types
     """
 
     NONLINEAR_RESIDUALS = "nonlinear_residual_v2"
@@ -430,15 +469,15 @@
 
         Returns
         -------
         CacheableData
             self
         """
         if self.data is None or force:
-            self.data = self.get_method(method=self.path)
+            self.data = self.get_method(method=self.path)["csvOutput"]
         return self
 
     @property
     def raw(self):
         """
         returns data in raw format: dictionary of lists
         """
@@ -464,15 +503,15 @@
 
     def __init__(self, results: CaseResults):
         self.results = results
 
     # pylint: disable=protected-access
     def total_forces(self):
         """plot total forces"""
-        steady = self.results._case.is_case_steady()
+        steady = self.results._case.is_steady()
         forces = self.results.total_forces.raw
         if steady:
             _, ax1 = subplots()
 
             ax2 = ax1.twinx()
             ax1.plot(forces["pseudo_step"], forces["CL"], "-g")
             ax2.plot(forces["pseudo_step"], forces["CD"], "-b")
@@ -507,15 +546,15 @@
         self._minmax_state = CacheableData(
             self._case.get, self._get_result_path(CaseResultType.MINMAX_STATE)
         )
         self._cfl = CacheableData(self._case.get, self._get_result_path(CaseResultType.CFL))
         self._plotter = ResultsPloter(self)
 
     def _get_result_path(self, result_type: CaseResultType):
-        return f"result/{result_type.value}"
+        return f"results/v2/{result_type.value}.csv"
 
     def get_residuals(self, force: bool = False):
         """
         Returns residuals
         :param force: when True, fetches data from server, otherwise uses cached data if exist
         """
         return self._residuals.get(force=force)
@@ -608,15 +647,15 @@
 
     def download_surface(self):
         """
         download surface results data
         """
         self.download_file(CaseDownloadable.SURFACE)
 
-    # pylint: disable=redefined-builtin,too-many-locals
+    # pylint: disable=redefined-builtin,too-many-locals,too-many-arguments
     def download_manager(
         self,
         surface: bool = False,
         volume: bool = False,
         nonlinear_residuals: bool = False,
         linear_residuals: bool = False,
         cfl: bool = False,
@@ -699,41 +738,39 @@
                     if actuator_disk_output:
                         print("Case does not have any actuator disks.")
                 else:
                     print("A problem occured when trying to download actuator disk results")
                     raise err
 
 
-class CaseList(list, RestApi):
+class CaseList(Flow360ResourceListBase):
     """
     Case List component
     """
 
-    def __init__(self, mesh_id: str = None, from_cloud: bool = True, include_deleted: bool = False):
-        if mesh_id is not None:
-            RestApi.__init__(self, endpoint=f"volumemeshes/{mesh_id}/cases")
-        else:
-            RestApi.__init__(self, endpoint="cases")
-
-        if from_cloud:
-            resp = self.get(params={"includeDeleted": include_deleted})
-            list.__init__(self, [CaseMeta(**item) for item in resp])
+    def __init__(
+        self, mesh_id: str = None, from_cloud: bool = True, include_deleted: bool = False, limit=100
+    ):
+        super().__init__(
+            ancestor_id=mesh_id,
+            from_cloud=from_cloud,
+            include_deleted=include_deleted,
+            limit=limit,
+            resourceClass=Case,
+        )
 
     def filter(self):
         """
         flitering list, not implemented yet
         """
         raise NotImplementedError("Filters are not implemented yet")
         # resp = list(filter(lambda i: i['caseStatus'] != 'deleted', resp))
 
-    def __getitem__(self, index) -> CaseMeta:
+    # pylint: disable=useless-parent-delegation
+    def __getitem__(self, index) -> Case:
         """
         returns CaseMeta info item of the list
         """
         return super().__getitem__(index)
 
-    @classmethod
-    def from_cloud(cls, mesh_id: str = None):
-        """
-        get Case List from cloud
-        """
-        return cls(mesh_id=mesh_id, from_cloud=True)
+    def __iter__(self) -> Iterator[Case]:
+        return super().__iter__()
```

### Comparing `flow360-0.1.8/flow360/component/volume_mesh.py` & `flow360-0.2.0b1/flow360/component/volume_mesh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 """
 Volume mesh component
 """
 from __future__ import annotations
 import os.path
-import json
 from enum import Enum
-from typing import Optional, Union, List
-
+from typing import Optional, Union, List, Iterator
 import numpy as np
-from pydantic import Extra, Field, validator, ValidationError
+from pydantic import Extra, Field, validator
 
 from ..cloud.s3_utils import S3TransferType
 from ..cloud.rest_api import RestApi
 from ..solver_version import Flow360Version
-from .flow360_base_model import (
-    Flow360BaseModel,
+from .resource_base import (
+    Flow360ResourceBaseModel,
     Flow360Resource,
-    on_cloud_resource_only,
+    Flow360ResourceListBase,
+    ResourceDraft,
 )
-from .flow360_solver_params import (
+from .flow360_params import (
     Flow360MeshParams,
     Flow360Params,
-    MeshBoundary,
     NoSlipWall,
+    _GenericBoundaryWrapper,
 )
+from .meshing.params import VolumeMeshingParams
+from .case import Case, CaseDraft
+from .params_base import params_generic_validator
+from .validator import Validator
+
+from ..log import log
+from ..exceptions import ValueError as FlValueError
+from ..exceptions import FileError as FlFileError
+from ..exceptions import Flow360NotImplementedError
 
 try:
     import h5py
 
     _H5PY_AVAILABLE = True
 except ImportError:
     _H5PY_AVAILABLE = False
@@ -49,26 +57,27 @@
     """
     Get wall boundary names
     :param params:
     :param solver_version:
     :return:
     """
     assert params
+
     if (
         isinstance(params, Flow360MeshParams)
         and params.boundaries
         and params.boundaries.no_slip_walls
     ):
         return params.boundaries.no_slip_walls
 
     if isinstance(params, Flow360Params) and params.boundaries:
         return [
             wall_name
-            for wall_name, wall in params.boundaries.items()
-            if isinstance(wall, NoSlipWall)
+            for wall_name, wall in params.boundaries.dict().items()
+            if _GenericBoundaryWrapper(v=wall).v.type == NoSlipWall().type
         ]
 
     return []
 
 
 def get_boundries_from_sliding_interfaces(params: Union[Flow360Params, Flow360MeshParams]):
     """
@@ -125,15 +134,14 @@
                         ]
                         if first_element_type_tag in [5, 7]:
                             names.append(f"{zone_name}/{section_name}")
                 else:
                     if section.attrs["label"].decode() != "ZoneBC_t":
                         continue
                     for bc_name, bc_zone in section.items():
-
                         if bc_zone.attrs["label"].decode() == "BC_t":
                             names.append(f"{zone_name}/{bc_name}")
 
         return names
 
 
 def validate_cgns(
@@ -147,24 +155,29 @@
     :return:
     """
     assert cgns_file
     assert params
     boundaries_in_file = get_boundaries_from_file(cgns_file, solver_version)
 
     boundaries_in_params = get_no_slip_walls(params) + get_boundries_from_sliding_interfaces(params)
+    print(get_no_slip_walls(params), boundaries_in_params)
+
     boundaries_in_file = set(boundaries_in_file)
     boundaries_in_params = set(boundaries_in_params)
+
+    print(boundaries_in_file, boundaries_in_params)
+
     if not boundaries_in_file.issuperset(boundaries_in_params):
-        raise ValueError(
+        raise FlValueError(
             "The following input boundary names from mesh json are not found in mesh:"
             + f" {' '.join(boundaries_in_params - boundaries_in_file)}."
             + f" Boundary names in cgns: {' '.join(boundaries_in_file)}"
             + f" Boundary names in params: {' '.join(boundaries_in_file)}"
         )
-    print(
+    log.info(
         f'Notice: {" ".join(boundaries_in_file - boundaries_in_params)} is '
         + "tagged as wall in cgns file, but not in input params"
     )
 
 
 class VolumeMeshLog(Enum):
     """
@@ -281,49 +294,35 @@
             return CompressionFormat.GZ, file_name
         if ext == CompressionFormat.BZ2.ext():
             return CompressionFormat.BZ2, file_name
         return CompressionFormat.NONE, file
 
 
 # pylint: disable=E0213
-class VolumeMeshMeta(Flow360BaseModel, extra=Extra.allow):
+class VolumeMeshMeta(Flow360ResourceBaseModel, extra=Extra.allow):
     """
     VolumeMeshMeta component
     """
 
     id: str = Field(alias="meshId")
     name: str = Field(alias="meshName")
-    status: str = Field(alias="meshStatus")
     created_at: str = Field(alias="meshAddTime")
     surface_mesh_id: Optional[str] = Field(alias="surfaceMeshId")
     mesh_params: Union[Flow360MeshParams, None, dict] = Field(alias="meshParams")
     mesh_format: VolumeMeshFileFormat = Field(alias="meshFormat")
     endianness: UGRIDEndianness = Field(alias="meshEndianness")
     compression: CompressionFormat = Field(alias="meshCompression")
     boundaries: Union[List, None]
 
     @validator("mesh_params", pre=True)
     def init_mesh_params(cls, value):
         """
         validator for mesh_params
         """
-        params = value
-        if isinstance(value, str):
-            try:
-                params = json.loads(value)
-            except json.decoder.JSONDecodeError:
-                return None
-        try:
-            Flow360MeshParams(**params)
-        except ValidationError:
-            return None
-        except TypeError:
-            return None
-
-        return params
+        return params_generic_validator(value, Flow360MeshParams)
 
     @validator("endianness", pre=True)
     def init_endianness(cls, value):
         """
         validator for endianess
         """
         return UGRIDEndianness(value) or UGRIDEndianness.NONE
@@ -341,64 +340,216 @@
     def to_volume_mesh(self) -> VolumeMesh:
         """
         returns VolumeMesh object from volume mesh meta info
         """
         return VolumeMesh(self.id)
 
 
-class VolumeMesh(Flow360Resource):
+# pylint: disable=too-few-public-methods
+class VolumeMeshBase:
+    """VolumeMeshBase base class"""
+
+    _endpoint = "volumemeshes"
+
+
+class VolumeMeshDraft(VolumeMeshBase, ResourceDraft):
+    """
+    Volume mesh draft component (before submit)
+    """
+
+    # pylint: disable=too-many-arguments
+    def __init__(
+        self,
+        file_name: str = None,
+        params: Union[Flow360MeshParams, VolumeMeshingParams] = None,
+        name: str = None,
+        surface_mesh_id=None,
+        tags: List[str] = None,
+        solver_version=None,
+        endianess: UGRIDEndianness = None,
+        isascii: bool = False,
+    ):
+        if file_name is not None and not os.path.exists(file_name):
+            raise FlFileError(f"{file_name} not found.")
+
+        if endianess is not None:
+            raise Flow360NotImplementedError(
+                "endianess selections not supported, it is inferred from filename"
+            )
+
+        if isascii is True:
+            raise Flow360NotImplementedError("isascii not supported")
+
+        self.params = None
+        if params is not None:
+            self.params = params.copy(deep=True)
+
+        # if not params or not isinstance(params, Flow360MeshParams):
+        #     raise ValueError(f'params={params} are not of type Flow360MeshParams')
+
+        if name is None and file_name is not None:
+            name = os.path.splitext(os.path.basename(file_name))[0]
+
+        self.file_name = file_name
+        self.name = name
+        self.surface_mesh_id = surface_mesh_id
+        self.tags = tags
+        self.solver_version = solver_version
+        self._id = None
+
+    def _submit_from_surface(self):
+        self.validator_api(self.params, solver_version=self.solver_version)
+        body = {
+            "name": self.name,
+            "tags": self.tags,
+            "surfaceMeshId": self.surface_mesh_id,
+            "config": self.params.to_flow360_json(),
+            "format": "cgns",
+        }
+
+        if self.solver_version:
+            body["solverVersion"] = self.solver_version
+
+        resp = RestApi(self._endpoint).post(body)
+        if not resp:
+            return None
+
+        info = VolumeMeshMeta(**resp)
+        self._id = info.id
+        mesh = VolumeMesh(self.id)
+        return mesh
+
+    # pylint: disable=protected-access
+    def _submit_upload_mesh(self, progress_callback=None):
+        assert os.path.exists(self.file_name)
+
+        compression, file_name_no_compression = CompressionFormat.detect(self.file_name)
+        mesh_format = VolumeMeshFileFormat.detect(file_name_no_compression)
+        endianness = UGRIDEndianness.detect(file_name_no_compression)
+
+        name = self.name
+        if name is None:
+            name = os.path.splitext(os.path.basename(self.file_name))[0]
+
+        body = {
+            "meshName": name,
+            "meshTags": self.tags,
+            "meshFormat": mesh_format.value,
+            "meshEndianness": endianness.value,
+        }
+        if self.params:
+            body["meshParams"] = self.params.to_flow360_json()
+
+        if self.solver_version:
+            body["solverVersion"] = self.solver_version
+
+        resp = RestApi(self._endpoint).post(body)
+        if not resp:
+            return None
+
+        info = VolumeMeshMeta(**resp)
+        self._id = info.id
+        mesh = VolumeMesh(self.id)
+        remote_file_name = mesh._remote_file_name(mesh_format, compression, endianness)
+        mesh.upload_file(remote_file_name, self.file_name, progress_callback=progress_callback)
+        mesh._complete_upload(remote_file_name)
+        return mesh
+
+    def submit(self, progress_callback=None) -> VolumeMesh:
+        """submit mesh to cloud
+
+        Parameters
+        ----------
+        progress_callback : callback, optional
+            Use for custom progress bar, by default None
+
+        Returns
+        -------
+        VolumeMesh
+            VolumeMesh object with id
+        """
+        print(self.surface_mesh_id, self.name, self.params, self.file_name)
+
+        if self.file_name is not None:
+            return self._submit_upload_mesh(progress_callback)
+
+        if self.surface_mesh_id is not None and self.name is not None and self.params is not None:
+            return self._submit_from_surface()
+
+        raise FlValueError(
+            "You must provide volume mesh file for upload or surface mesh Id with meshing parameters."
+        )
+
+    @classmethod
+    def validator_api(cls, params: VolumeMeshingParams, solver_version=None):
+        """
+        validation api: validates surface meshing parameters before submitting
+        """
+        return Validator.VOLUME_MESH.validate(params, solver_version=solver_version)
+
+
+class VolumeMesh(VolumeMeshBase, Flow360Resource):
     """
     Volume mesh component
     """
 
-    def __init__(self, mesh_id: str = None):
+    def __init__(self, mesh_id: str = None, meta_info: VolumeMeshMeta = None):
+        if (mesh_id is None and meta_info is None) or (
+            mesh_id is not None and meta_info is not None
+        ):
+            raise ValueError("You must provide mesh_id OR meta_info to constructor.")
+
+        if meta_info is not None:
+            mesh_id = meta_info.id
+
+        assert mesh_id is not None
+
         super().__init__(
             resource_type="Volume Mesh",
             info_type_class=VolumeMeshMeta,
             s3_transfer_method=S3TransferType.VOLUME_MESH,
-            endpoint="volumemeshes",
+            endpoint=self._endpoint,
             id=mesh_id,
         )
-        if mesh_id is not None:
-            self.get_info()
-            try:
-                self._params = Flow360MeshParams(**self.info.mesh_params.dict())
-            except AttributeError:
-                self._params = Flow360MeshParams(boundaries=MeshBoundary(no_slip_walls=[]))
+
+        if meta_info is not None:
+            self._info = meta_info
+
+        self.__mesh_params = None
 
     @property
     def info(self) -> VolumeMeshMeta:
         return super().info
 
     @property
-    @on_cloud_resource_only
-    def params(self) -> Flow360MeshParams:
+    def _mesh_params(self) -> Flow360MeshParams:
         """
         returns mesh params
         """
-        return self._params
+        if self.__mesh_params is None:
+            self.__mesh_params = self.info.mesh_params
+        return self.__mesh_params
 
     @property
-    @on_cloud_resource_only
     def no_slip_walls(self):
         """
         returns mesh no_slip_walls
         """
-        return self._params.boundaries.no_slip_walls
+        if self._mesh_params is None:
+            return None
+        return self._mesh_params.boundaries.no_slip_walls
 
     @property
-    @on_cloud_resource_only
     def all_boundaries(self):
         """
         returns mesh no_slip_walls
         """
         return self.info.boundaries
 
     # pylint: disable=too-many-arguments
-    @on_cloud_resource_only
     def download_file(
         self,
         file_name: Union[str, VolumeMeshDownloadable],
         to_file=".",
         keep_folder: bool = True,
         overwrite: bool = True,
         progress_callback=None,
@@ -416,96 +567,66 @@
             file_name,
             to_file,
             keep_folder=keep_folder,
             overwrite=overwrite,
             progress_callback=progress_callback,
         )
 
-    @on_cloud_resource_only
     def download(self, to_file=".", keep_folder: bool = True):
         """
         Download volume mesh file
         :param to_file:
         :param keep_folder:
         :return:
         """
         super().download_file(self._remote_file_name(), to_file, keep_folder)
 
-    @on_cloud_resource_only
-    def download_log(self, log: VolumeMeshLog, to_file=".", keep_folder: bool = True):
+    def download_log(self, log_file: VolumeMeshLog, to_file=".", keep_folder: bool = True):
         """
-        Download log
-        :param log:
+        Download logs
+        :param log_file:
         :param to_file: file name on local disk, could be either folder or file name.
         :param keep_folder: If true, the downloaded file will be put in the same folder as the file on cloud. Only work
         when file_name is a folder name.
         :return:
         """
 
-        self.download_file(f"logs/{log.value}", to_file, keep_folder)
+        self.download_file(f"logs/{log_file.value}", to_file, keep_folder)
 
-    @on_cloud_resource_only
     def _complete_upload(self, remote_file_name):
         """
         Complete volume mesh upload
         :return:
         """
         resp = self.post({}, method=f"completeUpload?fileName={remote_file_name}")
         self._info = VolumeMeshMeta(**resp)
 
     @classmethod
+    def _meta_class(cls):
+        """
+        returns volume mesh meta info class: VolumeMeshMeta
+        """
+        return VolumeMeshMeta
+
+    @classmethod
+    def _params_ancestor_id_name(cls):
+        """
+        returns surfaceMeshId name
+        """
+        return "surfaceMeshId"
+
+    @classmethod
     def from_cloud(cls, mesh_id: str):
         """
         Get volume mesh info from cloud
         :param mesh_id:
         :return:
         """
         return cls(mesh_id)
 
-    # pylint: disable=too-many-arguments
-    # @classmethod
-    # def from_surface_mesh(
-    #     cls,
-    #     volume_mesh_name: str,
-    #     surface_mesh_id: str,
-    #     config_file: str,
-    #     tags: [str] = None,
-    #     solver_version=None,
-    # ):
-    #     """
-    #     Create volume mesh from surface mesh
-    #     :param volume_mesh_name:
-    #     :param surface_mesh_id:
-    #     :param config_file:
-    #     :param tags:
-    #     :param solver_version:
-    #     :return:
-    #     """
-    #     assert volume_mesh_name
-    #     assert os.path.exists(config_file)
-    #     assert surface_mesh_id
-    #     with open(config_file, "r", encoding="utf-8") as config_f:
-    #         json_content = json.load(config_f)
-    #     body = {
-    #         "name": volume_mesh_name,
-    #         "tags": tags,
-    #         "surfaceMeshId": surface_mesh_id,
-    #         "config": json.dumps(json_content),
-    #         "format": "cgns",
-    #     }
-
-    #     if solver_version:
-    #         body["solverVersion"] = solver_version
-
-    #     resp = http.post("volumemeshes", body)
-    #     if resp:
-    #         return cls(**resp)
-    #     return None
-
-    @on_cloud_resource_only
     def _remote_file_name(self, mesh_format=None, compression=None, endianness=None):
         """
         mesh filename on cloud
         """
         compression = compression or self.info.compression
         mesh_format = mesh_format or self.info.mesh_format
         endianness = endianness or self.info.endianness
@@ -516,135 +637,110 @@
 
         return f"{remote_file_name}{endianness.ext()}{mesh_format.ext()}{compression.ext()}"
 
     @classmethod
     def from_file(
         cls,
         file_name: str,
-        params: Flow360MeshParams,
+        params: Union[Flow360MeshParams, None] = None,
         name: str = None,
-        tags: [str] = None,
+        tags: List[str] = None,
         solver_version=None,
-        progress_callback=None,
-    ):
+        endianess: UGRIDEndianness = None,
+        isascii: bool = False,
+    ) -> VolumeMeshDraft:
         """
-        Create volume mesh from ugrid file
+        Upload volume mesh from file
         :param volume_mesh_name:
         :param file_name:
         :param params:
         :param tags:
         :param solver_version:
         :return:
         """
-        assert os.path.exists(file_name)
-        assert params
-
-        if name is None:
-            name = os.path.splitext(os.path.basename(file_name))[0]
-
-        mesh = cls()
-        compression, file_name_no_compression = CompressionFormat.detect(file_name)
-        mesh_format = VolumeMeshFileFormat.detect(file_name_no_compression)
-        endianness = UGRIDEndianness.detect(file_name_no_compression)
-
-        body = {
-            "meshName": name,
-            "meshTags": tags,
-            "meshFormat": mesh_format.value,
-            "meshEndianness": endianness.value,
-            "meshParams": params.json(),
-        }
 
-        if solver_version:
-            body["solverVersion"] = solver_version
-
-        resp = mesh.post(body)
+        return VolumeMeshDraft(
+            file_name=file_name,
+            name=name,
+            tags=tags,
+            solver_version=solver_version,
+            params=params,
+            endianess=endianess,
+            isascii=isascii,
+        )
 
-        if not resp:
-            return None
+    @classmethod
+    def new(
+        cls,
+        name: str,
+        params: VolumeMeshingParams,
+        surface_mesh_id,
+        tags: List[str] = None,
+        solver_version=None,
+    ) -> VolumeMeshDraft:
+        """
+        Create volume mesh from surface mesh
+        """
 
-        mesh._info = VolumeMeshMeta(**resp)
-        mesh._params = Flow360MeshParams(**mesh._info.mesh_params.dict())
-        mesh.init_id(mesh._info.id)
-        remote_file_name = mesh._remote_file_name(mesh_format, compression, endianness)
-        mesh.upload_file(remote_file_name, file_name, progress_callback=progress_callback)
-        mesh._complete_upload(remote_file_name)
-        return mesh
+        return VolumeMeshDraft(
+            name=name,
+            surface_mesh_id=surface_mesh_id,
+            solver_version=solver_version,
+            params=params,
+            tags=tags,
+        )
 
-    #     # pylint: disable=too-many-arguments
+    def new_case(
+        self,
+        name: str,
+        params: Flow360Params,
+        tags: List[str] = None,
+    ) -> CaseDraft:
+        """
+        Create new case
+        :param name:
+        :param params:
+        :param tags:
+        :return:
+        """
 
-    # @classmethod
-    # def from_cgns_file(
-    #     cls,
-    #     volume_mesh_name: str,
-    #     file_name: str,
-    #     params: Union[Flow360Params, Flow360MeshParams],
-    #     tags: [str] = None,
-    #     solver_version=None,
-    # ):
-    #     """
-    #     Create volume mesh from ugrid file
-    #     :param volume_mesh_name:
-    #     :param file_name:
-    #     :param params:
-    #     :param tags:
-    #     :param solver_version:
-    #     :return:
-    #     """
-    #     assert volume_mesh_name
-    #     assert os.path.exists(file_name)
-    #     assert params
-
-    #     if _H5PY_AVAILABLE:
-    #         validate_cgns(file_name, params, solver_version=solver_version)
-    #     else:
-    #         warnings.warn(
-    #             "Could not check consistency between mesh file and"
-    #             " Flow360.json file. h5py module not found. This is optional functionality"
-    #         )
-
-    #     body = {
-    #         "meshName": volume_mesh_name,
-    #         "meshTags": tags,
-    #         "meshFormat": "cgns",
-    #         "meshParams": params.json(),
-    #     }
-
-    #     if solver_version:
-    #         body["solverVersion"] = solver_version
-
-    #     resp = http.post("volumemeshes", body)
-    #     if resp:
-    #         return cls(**resp)
-    #     return None
+        return Case.new(name, params, volume_mesh_id=self.id, tags=tags)
 
 
-class VolumeMeshList(list, RestApi):
+class VolumeMeshList(Flow360ResourceListBase):
     """
     VolumeMesh List component
     """
 
-    def __init__(self, from_cloud: bool = True, include_deleted: bool = False):
-        RestApi.__init__(self, endpoint="volumemeshes")
-
-        if from_cloud:
-            resp = self.get(params={"includeDeleted": include_deleted})
-            list.__init__(self, [VolumeMeshMeta(**item) for item in resp])
+    def __init__(
+        self,
+        surface_mesh_id: str = None,
+        from_cloud: bool = True,
+        include_deleted: bool = False,
+        limit=100,
+    ):
+        super().__init__(
+            ancestor_id=surface_mesh_id,
+            from_cloud=from_cloud,
+            include_deleted=include_deleted,
+            limit=limit,
+            resourceClass=VolumeMesh,
+        )
 
     def filter(self):
         """
         flitering list, not implemented yet
         """
+        raise NotImplementedError("Filters are not implemented yet")
+
         # resp = list(filter(lambda i: i['caseStatus'] != 'deleted', resp))
 
-    def __getitem__(self, index) -> VolumeMeshMeta:
+    # pylint: disable=useless-parent-delegation
+    def __getitem__(self, index) -> VolumeMesh:
         """
         returns VolumeMeshMeta item of the list
         """
         return super().__getitem__(index)
 
-    @classmethod
-    def from_cloud(cls):
-        """
-        get VolumeMeshList from cloud
-        """
-        return cls(from_cloud=True)
+    # pylint: disable=useless-parent-delegation
+    def __iter__(self) -> Iterator[VolumeMesh]:
+        return super().__iter__()
```

### Comparing `flow360-0.1.8/flow360/solver_version.py` & `flow360-0.2.0b1/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.1.8/pyproject.toml` & `flow360-0.2.0b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "flow360"
-version = "0.1.8"
+version = "v0.2.0b1"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
 click = "^8.1.3"
 toml = "^0.10.2"
 requests = "^2.28.1"
 boto3 = "^1.24.63"
 numpy = [{ python = "^3.7", version = "^1.19.0" },
@@ -17,26 +17,28 @@
     { python = "^3.9", version = "^1.23.0" },
     { python = "^3.10", version = "^1.23.0" }]
 h5py = "^3.7.0"
 matplotlib =  [{ python = "^3.7", version = "^3.5.3" },
     { python = "^3.8", version = "^3.6.2" },
     { python = "^3.9", version = "^3.6.2" },
     { python = "^3.10", version = "^3.6.2" }]
+pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 autohooks = "^22.8.1"
 autohooks-plugin-black = "^22.8.1"
 autohooks-plugin-pylint = "^22.8.1"
 autohooks-plugin-isort = "^22.8.0"
 pylint = "^2.15.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.20.3"
+pytest-cov = "^4.0.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 100
 target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `flow360-0.1.8/PKG-INFO` & `flow360-0.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.1.8
+Version: 0.2.0b1
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.24.63,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
@@ -19,9 +19,10 @@
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0) ; python_version >= "3.9" and python_version < "4.0"
 Requires-Dist: numpy (>=1.19.0,<2.0.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: numpy (>=1.20.0,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: numpy (>=1.23.0,<2.0.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: numpy (>=1.23.0,<2.0.0) ; python_version >= "3.9" and python_version < "4.0"
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

