# Comparing `tmp/adt_clients-2.1.0-py3-none-any.whl.zip` & `tmp/adt_clients-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11624 bytes, number of entries: 9
--rw-r--r--  2.0 unx      791 b- defN 23-Mar-13 15:42 adt_clients/__init__.py
--rw-r--r--  2.0 unx     9384 b- defN 23-Mar-13 15:42 adt_clients/analytic_dataset_client.py
--rw-r--r--  2.0 unx     3153 b- defN 23-Mar-13 15:42 adt_clients/analytic_dataset_definition_client.py
--rw-r--r--  2.0 unx    27896 b- defN 23-Mar-13 15:42 adt_clients/models.py
--rw-rw-rw-  2.0 unx      575 b- defN 23-Mar-13 16:16 adt_clients-2.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      895 b- defN 23-Mar-13 16:16 adt_clients-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-13 16:16 adt_clients-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Mar-13 16:16 adt_clients-2.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      767 b- defN 23-Mar-13 16:16 adt_clients-2.1.0.dist-info/RECORD
-9 files, 43565 bytes uncompressed, 10290 bytes compressed:  76.4%
+Zip file size: 11962 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      791 b- defN 23-Apr-04 15:31 adt_clients/__init__.py
+-rw-r--r--  2.0 unx    11293 b- defN 23-Apr-05 09:59 adt_clients/analytic_dataset_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 22-Oct-18 08:26 adt_clients/analytic_dataset_definition_client.py
+-rw-r--r--  2.0 unx    28111 b- defN 23-Apr-05 11:30 adt_clients/models.py
+-rw-rw-rw-  2.0 unx      575 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      845 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      768 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/RECORD
+9 files, 45640 bytes uncompressed, 10628 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: adt_clients/analytic_dataset_definition_client.py
 Comment: 
 
 Filename: adt_clients/models.py
 Comment: 
 
-Filename: adt_clients-2.1.0.dist-info/LICENSE.txt
+Filename: adt_clients-2.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: adt_clients-2.1.0.dist-info/METADATA
+Filename: adt_clients-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: adt_clients-2.1.0.dist-info/WHEEL
+Filename: adt_clients-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: adt_clients-2.1.0.dist-info/top_level.txt
+Filename: adt_clients-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: adt_clients-2.1.0.dist-info/RECORD
+Filename: adt_clients-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adt_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 __all__ = [
     "AnalyticDatasetClient",
     "AnalyticDatasetModel",
     "AnalyticDatasetDefinitionClient",
     "AnalyticDatasetDefinitionModel",
     "AnalyticDatasetMergeRequestModel",
```

## adt_clients/analytic_dataset_client.py

```diff
@@ -1,13 +1,14 @@
 import math
 import time
 import uuid
 import pathlib
 import requests
-from typing import Dict, Any, Callable, Union  # noqa: F401
+import warnings
+from typing import Dict, Any, Callable, Union, Optional  # noqa: F401
 from typing.io import BinaryIO
 from dataclasses import dataclass
 from clients_core.service_clients import E360ServiceClient
 from .models import (
     AnalyticDatasetModel,
     AnalyticDatasetStatus,
     AnalyticDatasetColumnsModel,
@@ -28,14 +29,15 @@
 
     """
 
     correlation_id: str = str(uuid.uuid4())
 
     service_endpoint = ""
     extra_headers = {}  # type: Dict[str, str]
+    FILE_WRITER_CHUNK_SIZE = 512
 
     def __post_init__(self) -> None:
         self.extra_headers.update(
             {"x-correlation-id": self.correlation_id, **self.get_ims_claims()}
         )
 
     def create(
@@ -68,21 +70,68 @@
         Returns the information about report columns
         """
         response = self.client.get(
             f"{dataset_id}/columns", headers=self.extra_headers, raises=True, **kwargs
         )
         return AnalyticDatasetColumnsModel.parse_obj(response.json())
 
-    @staticmethod
-    def _file_writer(response: requests.Response, output_path: pathlib.Path) -> None:
+    @classmethod
+    def _file_writer(
+        cls, response: requests.Response, output_path: pathlib.Path
+    ) -> None:
         with output_path.open(mode="wb") as file_writer:
-            for chunk in response.iter_content(chunk_size=512):
+            for chunk in response.iter_content(chunk_size=cls.FILE_WRITER_CHUNK_SIZE):
                 if chunk:
                     file_writer.write(chunk)
 
+    def download(
+        self,
+        dataset: AnalyticDatasetModel,
+        output_path: pathlib.Path,
+        overwrite_output: bool = False,
+        impersonate_id: Optional[str] = None,
+        **kwargs: Any,
+    ) -> bool:
+        """
+        Downloads a dataset to provided output path.
+
+        Args:
+            dataset: instance of the dataset to download.
+            output_path: Path object where to save the file to.
+            overwrite_output: if set to True, will overwrite existing output.
+            impersonate_id: the user Id to perform the operation on behalf of
+            **kwargs: passed onto the self.client
+
+        Resturns:
+            bool: that an output file has been created successfully.
+
+        Raises:
+            clients_core.exceptions.HttpResponseError: on server response errors.
+            FileExistsError: if the ``output_path`` already exists.
+
+        """
+        if all([output_path.exists(), overwrite_output is False]):
+            raise FileExistsError(
+                "Specified `output_path` already exists. Set `overwrite_output=True` to overwrite it."
+            )
+
+        if impersonate_id:
+            if not hasattr(kwargs, "params"):
+                kwargs["params"] = {}
+            kwargs["params"] = {"workspaceImpersonationId": impersonate_id}
+        response = self.client.get(
+            f"{dataset.id}/download",
+            stream=True,
+            headers={**dataset.outputType.get_accept_header(), **self.extra_headers},
+            raises=True,
+            **kwargs,
+        )
+        self._file_writer(response, output_path)
+        return all([output_path.exists(), output_path.is_file()])
+
     def download_report(
         self,
         dataset_id: str,
         output_path: pathlib.Path,
         accept: str,
         overwrite_output: bool = False,
         impersonate_id: str = "",
@@ -103,14 +152,19 @@
             bool: that an output file has been created successfully.
 
         Raises:
             clients_core.exceptions.HttpResponseError: on server response errors.
             FileExistsError: if the ``output_path`` already exists.
 
         """
+        warnings.warn(
+            "This method is being deprecated, use `.download` instead",
+            DeprecationWarning,
+        )
+
         if all([output_path.exists(), overwrite_output is False]):
             raise FileExistsError(
                 "Specified `output_path` already exists. Set `overwrite_output=True` to overwrite it."
             )
 
         endpoint_path = f"{dataset_id}/download"
         if impersonate_id != "":
```

## adt_clients/models.py

```diff
@@ -1,26 +1,23 @@
 from __future__ import annotations
 
 import json
 from datetime import datetime
 from enum import Enum
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Dict
 from uuid import UUID
 
 from pydantic import BaseModel, Field
 
 
 class BaseADTModel(BaseModel):
     def dump(self) -> dict:
-        return json.loads(
-            self.json(by_alias=True, exclude_none=True, exclude_unset=True)
-        )
+        return json.loads(self.json(by_alias=True, exclude_none=True))
 
     class Config:
-        use_enum_values = True
         anystr_strip_whitespace = True
 
 
 class Granularity(str, Enum):
     # https://rwes-gitlab01.internal.imsglobal.com/e360/analytic-dataset-tools-api/-/blob/master/src/Models/Enums/Granularity.cs
     EVENT = "event"  # -1
     PATIENT = "patient"  # 0
@@ -154,17 +151,24 @@
     STANDARD = "standard"  # 1
     UPLOAD = "upload"  # 2
 
 
 class OutputType(str, Enum):
     # https://rwes-gitlab01.internal.imsglobal.com/e360/analytic-dataset-tools-api/-/blob/master/src/Models/Enums/OutputType.cs
     CSV = "csv"  # 1
-    ZIP = "zip"  # 2
-    PARQUET = "parquet"  # 3
-    MULTIPARTPARQUETZIP = "multipartparquetzip"  # 4
+    CSVZIP = "csvZip"  # 2
+    # PARQUET = "parquet"  # 3  # DEPRECATED
+    MULTIPARTPARQUETZIP = "multiPartParquetZip"  # 4
+
+    def get_accept_header(self) -> Dict[str, str]:
+        """Returns an accept header value for http request (used when downloading)"""
+        accept = {
+            OutputType.CSV: "text/csv",
+        }.get(self, "application/zip")
+        return {"accept": accept}
 
 
 class AnalyticDatasetResultModel(BaseADTModel):
     completedDate: Optional[datetime] = None
     downloadUrl: Optional[str] = None
     fileSize: Optional[int] = None
     rowCount: Optional[int] = None
@@ -184,15 +188,15 @@
     cohortOfInterestId: Optional[int] = None
     cohortOfInterestAssetId: Optional[UUID] = None
     combineEventsOnSameDay: Optional[bool] = None
     columns: Optional[List[CharacteristicReportColumnModel]] = None
     randomPatientCount: Optional[int] = None
     status: Optional[AnalyticDatasetStatus] = None
     source: Optional[AnalyticDatasetSource] = None
-    outputType: Optional[OutputType] = OutputType.ZIP
+    outputType: OutputType = OutputType.CSV
     result: Optional[AnalyticDatasetResultModel] = None
     emailAddresses: Optional[List[EmailAddressModel]] = None
     generateAsset: Optional[bool] = None
     datasetReleaseIdentifier: Optional[str] = None
     hashSecret: Optional[str] = None
     id: Optional[UUID] = None
     created: Optional[datetime] = None
```

## Comparing `adt_clients-2.1.0.dist-info/LICENSE.txt` & `adt_clients-2.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `adt_clients-2.1.0.dist-info/METADATA` & `adt_clients-2.2.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adt-clients
-Version: 2.1.0
+Version: 2.2.0
 Summary: E360 Analytic Dataset Tools Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: clients-core (<3,>=1.1.0)
 Requires-Dist: pydantic
```

## Comparing `adt_clients-2.1.0.dist-info/RECORD` & `adt_clients-2.2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-adt_clients/__init__.py,sha256=IHS4adefMf9958M2sn06dM-Kk2sxqe40xq37JOY_NNY,791
-adt_clients/analytic_dataset_client.py,sha256=BrWsb9wnL6xCH9nK463Jf-SIWD9qSsBWhUYuTIvmBjs,9384
+adt_clients/__init__.py,sha256=i4k0nCX_7fBkTBXzadEteRZmX22OLBGgU8-x4qfWn68,791
+adt_clients/analytic_dataset_client.py,sha256=YLlu9snUgHMrQoIFxtb_hcrIRcHQ4UvzAvZw5kqvJcQ,11293
 adt_clients/analytic_dataset_definition_client.py,sha256=_XrRejeGvfyCNAE2I3Ugv-7FYLNCm5wspaajU9mR7E4,3153
-adt_clients/models.py,sha256=j7HMOZATZxpQttLHLwpmypuuSzGkf_K7EvledQl2CCo,27896
-adt_clients-2.1.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
-adt_clients-2.1.0.dist-info/METADATA,sha256=XaFLkIFk_APOkkCtu8-ZLcDxwBLxFwgp0roLokQJcQ0,895
-adt_clients-2.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-adt_clients-2.1.0.dist-info/top_level.txt,sha256=rW_Jf5iTyds74mmCEkdUO2G_ryraJ6g5LQXDdeBOsfs,12
-adt_clients-2.1.0.dist-info/RECORD,,
+adt_clients/models.py,sha256=bADidocTYapS3YnErjgkgu3UNUxOvM7F2-xPF5-Da4Y,28111
+adt_clients-2.2.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
+adt_clients-2.2.0.dist-info/METADATA,sha256=Grueexm5A1Uy6WU59CAkEizvXwkpIRCwYlVoK0D3B8U,845
+adt_clients-2.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+adt_clients-2.2.0.dist-info/top_level.txt,sha256=rW_Jf5iTyds74mmCEkdUO2G_ryraJ6g5LQXDdeBOsfs,12
+adt_clients-2.2.0.dist-info/RECORD,,
```

