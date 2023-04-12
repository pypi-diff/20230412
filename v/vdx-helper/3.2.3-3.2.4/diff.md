# Comparing `tmp/vdx-helper-3.2.3.tar.gz` & `tmp/vdx_helper-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdx-helper-3.2.3.tar", max compression
+gzip compressed data, was "vdx_helper-3.2.4.tar", max compression
```

## Comparing `vdx-helper-3.2.3.tar` & `vdx_helper-3.2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1081 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/LICENSE
--rw-r--r--   0        0        0     2615 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/README.md
--rw-r--r--   0        0        0      980 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/vdx_helper/__init__.py
--rw-r--r--   0        0        0      729 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/vdx_helper/domain.py
--rw-r--r--   0        0        0     1259 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/vdx_helper/errors.py
--rw-r--r--   0        0        0     6907 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/vdx_helper/mappers.py
--rw-r--r--   0        0        0     9836 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/vdx_helper/models.py
--rw-r--r--   0        0        0     2207 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/vdx_helper/util.py
--rw-r--r--   0        0        0    37823 2022-07-26 17:02:06.000000 vdx-helper-3.2.3/vdx_helper/vdx_helper.py
--rw-r--r--   0        0        0     3380 2022-07-26 17:03:54.300812 vdx-helper-3.2.3/setup.py
--rw-r--r--   0        0        0     3481 2022-07-26 17:03:54.301341 vdx-helper-3.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/LICENSE
+-rw-r--r--   0        0        0     2839 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/README.md
+-rw-r--r--   0        0        0     1032 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/__init__.py
+-rw-r--r--   0        0        0      729 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/domain.py
+-rw-r--r--   0        0        0     1211 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/errors.py
+-rw-r--r--   0        0        0     7181 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/mappers.py
+-rw-r--r--   0        0        0     9779 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/models.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/py.typed
+-rw-r--r--   0        0        0     2207 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/util.py
+-rw-r--r--   0        0        0    38753 2023-04-12 10:32:53.000000 vdx_helper-3.2.4/vdx_helper/vdx_helper.py
+-rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 vdx_helper-3.2.4/PKG-INFO
```

### Comparing `vdx-helper-3.2.3/LICENSE` & `vdx_helper-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vdx-helper-3.2.3/README.md` & `vdx_helper-3.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,14 +49,30 @@
 
 You can run the tests with poetry if you like. You can also obtain the code coverage.
 
 ```
 poetry run pytest --cov=vdx_helper
 ```
 
+* **Mypy:**
+```shell
+poetry run mypy --config-file conf/mypy.ini vdx_helper
+```
+
+* **Coverage:**
+```shell
+poetry run coverage run --source=vdx_helper -m pytest
+poetry run coverage report
+```
+
+* **Tox:**
+```shell
+tox -p
+```
+
 ### Run the test locally with docker-compose step-by-step
 1. Spin up the docker-containers
 ```
 docker-compose up -d
 ```
 
 2. Run the tests via the vdx-helper docker container
```

### Comparing `vdx-helper-3.2.3/pyproject.toml` & `vdx_helper-3.2.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vdx-helper"
-version = "3.2.3"
+version = "3.2.4"
 description = "Python client library to connect to the VDX Core API"
 authors = ["Joana Teixeira <joana.teixeira@vizidox.com>", "Tiago Santos <tiago.santos@vizidox.com>",
            "Rita Mariquitos <rita.mariquitos@morphotech.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://vizidox.com"
 repository = "https://github.com/Morphotech/vdx-helper-python"
@@ -13,21 +13,24 @@
                "Programming Language :: Python :: 3",
                "Topic :: Software Development :: Libraries :: Python Modules"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests="^2.27"
-nndict="1.0.0"
+nndict="^2.0.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "5.4.3"
-coverage = "^5.0"
-pytest-cov = "^2.10.1"
+pytest = "^7.3.0"
+coverage = "^7.2.3"
+pytest-cov = "^4.0.0"
 testcontainers = "^3.5"
-mypy="0.910"
-sphinx="4.3.0"
-sphinx-rtd-theme="1.0.0"
+mypy="^1.2"
+sphinx="^5.3.0"
+sphinx-rtd-theme="^1.2.0"
+tox = "^4.4.11"
+
+types-requests = "^2.28.11.17"
 
 [build-system]
-requires = ["poetry>=1.0"]
+requires = ["poetry>=1.3"]
 build-backend = "poetry.masonry.api"
```

### Comparing `vdx-helper-3.2.3/vdx_helper/domain.py` & `vdx_helper-3.2.4/vdx_helper/domain.py`

 * *Files identical despite different names*

### Comparing `vdx-helper-3.2.3/vdx_helper/errors.py` & `vdx_helper-3.2.4/vdx_helper/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,27 @@
     """
 
     def __init__(self, code: HTTPStatus, message: str):
         self.code = code
         self.message = message
 
 
-def error_from_response(status: HTTPStatus, response: Response):
+def error_from_response(status: HTTPStatus, response: Response) -> VDXError:
     """
     Maps a given error from an endpoint response to an exception with the correct status code and description of the
     error
 
     :param status: The status code of the endpoint response
     :type status: HTTPStatus
 
     :param response: The endpoint response
     :type response: :class:`requests.Response`
 
     :return: A VDXError to be raised
     :rtype: :class:`VDXError`
     """
-    if status is not HTTPStatus.OK:
-        try:
-            json_response = response.json()
-            description = json_response.get("description")
-        except (ValueError, AttributeError):
-            description = ""
-        return VDXError(code=status, message=description)
+    try:
+        json_response = response.json()
+        description = json_response.get("description")
+    except (ValueError, AttributeError):
+        description = ""
+    return VDXError(code=status, message=description)
```

### Comparing `vdx-helper-3.2.3/vdx_helper/mappers.py` & `vdx_helper-3.2.4/vdx_helper/mappers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from datetime import datetime
-from typing import TypeVar, Callable
+from typing import TypeVar, Callable, Dict, Any
 from uuid import UUID
 
 from vdx_helper.domain import VerificationStatus, StepStatus, JobStatus
 from vdx_helper.models import File, PaginatedResponse, Credential, Job, VerificationResponse, \
     VerificationStepResult, Certificate, Claim, Partner, \
     VerificationReport
-from vdx_helper.util import optional_datetime_from_string
+from vdx_helper.util import optional_datetime_from_string, datetime_from_string
 
 T = TypeVar('T')
 
 
-def json_mapper(json_: dict) -> dict:
+def json_mapper(json_: Dict[str, Any]) -> Dict[str, Any]:
     """
     Directly map any json response to a json response.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: The response in json format
-    :rtype: dict
+    :rtype: Dict[str, Any]
     """
     return json_
 
 
-def get_paginated_mapper(mapper: Callable[[dict], T]) -> Callable[[dict], 'PaginatedResponse[T]']:
+def get_paginated_mapper(mapper: Callable[[Dict[str, Any]], T]) -> Callable[[Dict[str, Any]], 'PaginatedResponse']:
     """
     Obtain a mapper method that maps a json response from the Core API into a PaginatedResponse object containing
     a specific object as its items.
 
     :param mapper: The mapper to use to map the Paginated result's items
     :type mapper: Callable
 
     :return: A mapping function
     :rtype: Callable
     """
-    def paginated_mapper(json_: dict) -> 'PaginatedResponse[T]':
+    def paginated_mapper(json_: Dict[str, Any]) -> 'PaginatedResponse':
         """
         Maps the json response into a Paginated Response object.
 
         :param json_: The json obtained from the endpoint call
-        :type json_: dict
+        :type json_: Dict[str, Any]
 
         :return: A Paginated Response instance
         :rtype: class:`vdx_helper.models.PaginatedResponse`
         """
         return PaginatedResponse(
             page=int(json_["page"]),
             total_pages=int(json_["total_pages"]),
@@ -52,36 +52,36 @@
             total_items=int(json_["total_items"]),
             items=[mapper(json_item) for json_item in json_["items"]]
         )
 
     return paginated_mapper
 
 
-def file_mapper(json_: dict) -> File:
+def file_mapper(json_: Dict[str, Any]) -> File:
     """
     Maps the json file response into a File object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: A File instance
     :rtype: :class:`vdx_helper.models.File`
     """
     return File(
         file_hash=json_["file_hash"],
         file_type=json_["file_type"]
     )
 
 
-def credential_mapper(json_: dict) -> Credential:
+def credential_mapper(json_: Dict[str, Any]) -> Credential:
     """
     Maps the json credential response into a Credential object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: A Credential instance
     :rtype: :class:`vdx_helper.models.Credential`
     """
     return Credential(
         uid=UUID(json_["uid"]),
         title=json_["title"],
@@ -90,130 +90,130 @@
         credentials=[credential_mapper(credential) for credential in json_["credentials"]],
         upload_date=datetime.fromisoformat(json_["upload_date"]),
         tags=json_["tags"],
         expiry_date=optional_datetime_from_string(json_["expiry_date"])
     )
 
 
-def job_mapper(json_: dict) -> Job:
+def job_mapper(json_: Dict[str, Any]) -> Job:
     """
     Maps the json job response into a Job object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: A Job instance
     :rtype: :class:`vdx_helper.models.Job`
     """
     return Job(
         uid=UUID(json_["uid"]),
         partner=partner_mapper(json_["partner"]),
         chain=json_["chain"],
         tags=json_["tags"],
         status=JobStatus(json_["status"]),
-        created_date=optional_datetime_from_string(json_.get("created_date")),
+        created_date=datetime_from_string(json_["created_date"]),
         start_date=optional_datetime_from_string(json_.get("start_date")),
         issued_date=optional_datetime_from_string(json_.get("issued_date")),
         finished_date=optional_datetime_from_string(json_.get("finished_date")),
         failed_date=optional_datetime_from_string(json_.get("failed_date")),
         scheduled_date=optional_datetime_from_string(json_.get("scheduled_date"))
     )
 
 
-def verification_mapper(json_: dict) -> VerificationResponse:
+def verification_mapper(json_: Dict[str, Any]) -> VerificationResponse:
     """
     Maps the json verification response into a VerificationResponse object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: A VerificationResponse instance
     :rtype: :class:`vdx_helper.models.VerificationResponse`
     """
     return VerificationResponse(
         verification={key: verification_step_mapper(step) for key, step in json_["verification"].items()},
         result=verification_report_mapper(json_["result"])
     )
 
 
-def verification_step_mapper(json_: dict) -> VerificationStepResult:
+def verification_step_mapper(json_: Dict[str, Any]) -> VerificationStepResult:
     """
     Maps the json verification step result response into a Verification Step Result object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, str]
 
     :return: A VerificationStepResult instance
     :rtype: :class:`vdx_helper.models.VerificationStepResult`
     """
     return VerificationStepResult(
         name=json_["name"],
         description=json_["description"],
         status=StepStatus(json_["status"])
     )
 
 
-def partner_mapper(json_: dict) -> Partner:
+def partner_mapper(json_: Dict[str, Any]) -> Partner:
     """
     Maps the json partner response into a Partner object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: A Partner instance
     :rtype: :class:`vdx_helper.models.Partner`
     """
     return Partner(
         **json_
     )
 
 
-def claim_mapper(json_: dict) -> Claim:
+def claim_mapper(json_: Dict[str, Any]) -> Claim:
     """
     Maps the json claim response into a Claim object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: A Claim instance
     :rtype: :class:`vdx_helper.models.Claim`
     """
     return Claim(
         uid=UUID(json_["uid"]),
         partner=partner_mapper(json_["partner"]),
         credential=credential_mapper(json_["credential"]),
         issued_date=datetime.fromisoformat(json_["issued_date"]),
         signature=json_["signature"]
     )
 
 
-def certificate_mapper(json_: dict) -> Certificate:
+def certificate_mapper(json_: Dict[str, Any]) -> Certificate:
     """
     Maps the json certificate response into a Certificate object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, Any]
 
     :return: A Certificate instance
     :rtype: :class:`vdx_helper.models.Certificate`
     """
     json_verification = json_.get("last_verification")
     return Certificate(
         certificate=claim_mapper(json_["certificate"]),
         revoked_date=optional_datetime_from_string(json_.get("revoked_date")),
         last_verification=verification_report_mapper(json_verification) if json_verification is not None else None
     )
 
 
-def verification_report_mapper(json_: dict) -> VerificationReport:
+def verification_report_mapper(json_: Dict[str, str]) -> VerificationReport:
     """
     Maps the json verification report response into a Verification Report object.
 
     :param json_: The json obtained from the endpoint call
-    :type json_: dict
+    :type json_: Dict[str, str]
 
     :return: A VerificationReport instance
     :rtype: :class:`vdx_helper.models.VerificationReport`
     """
     return VerificationReport(
         status=VerificationStatus(json_["status"]),
         timestamp=datetime.fromisoformat(json_["timestamp"])
```

### Comparing `vdx-helper-3.2.3/vdx_helper/models.py` & `vdx_helper-3.2.4/vdx_helper/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import NamedTuple, Optional, List, Mapping, Generic, TypeVar, Dict
+from typing import NamedTuple, Optional, List, Mapping, TypeVar, Dict, Any
 from uuid import UUID
 
 from vdx_helper.domain import VerificationStatus, StepStatus, JobStatus
 
 T = TypeVar('T')
 
 
@@ -16,20 +16,20 @@
 
     :param name: The name of the partner
     :type name: str
     """
     id: str
     name: str
 
-    def __eq__(self, obj: 'Partner'):
+    def __eq__(self, obj: object) -> bool:
         """
-        Overriding of the equals method for simplified comparison between Paginated objects.
+        Overriding of the equals method for simplified comparison between Partner objects.
 
-        :param obj: The other instance of a paginated object
-        :type obj: :class:`PaginatedResponse`
+        :param obj: The other instance of a Partner object
+        :type obj: object
 
         :return: True if the two objects are equal
         :rtype: bool
         """
         return isinstance(obj, Partner) and obj.id == self.id and obj.name == self.name
 
 
@@ -42,20 +42,20 @@
 
     :param file_type: The file `MIME type <https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types>`
     :type file_type: str, optional
     """
     file_hash: str
     file_type: Optional[str]
 
-    def __eq__(self, obj: 'File'):
+    def __eq__(self, obj: object) -> bool:
         """
         Overriding of the equals method for simplified comparison between File objects.
 
         :param obj: The other instance of a File object
-        :type obj: :class:`File`
+        :type obj: object
 
         :return: True if the two objects are equal
         :rtype: bool
         """
         return isinstance(obj, File) \
                and obj.file_hash == self.file_hash \
                and obj.file_type == self.file_type
@@ -68,15 +68,15 @@
     :param uid: The uid of the credential
     :type uid: :class:`uuid.UUID`
 
     :param title: The credential title
     :type title: str
 
     :param metadata: Any additional data in the credential
-    :type metadata: dict
+    :type metadata: Dict
 
     :param files: List of files issued on the credential
     :type files: List[:class:`File`]
 
     :param credentials: List of credentials associated to the credential
     :type credentials: List[:class:`Credential`]
 
@@ -87,27 +87,27 @@
     :type tags: List[str]
 
     :param expiry_date: The date the credential expires, if set
     :type expiry_date: :class:`datetime.datetime`, optional
     """
     uid: UUID
     title: str
-    metadata: dict
+    metadata: Dict[str, Any]
     files: List[File]
     credentials: List['Credential']
     upload_date: datetime
     tags: List[str]
     expiry_date: Optional[datetime]
 
-    def __eq__(self, obj: 'Credential'):
+    def __eq__(self, obj: object) -> bool:
         """
         Overriding of the equals method for simplified comparison between Credential objects.
 
         :param obj: The other instance of a credential object
-        :type obj: :class:`Credential`
+        :type obj: object
 
         :return: True if the two objects are equal
         :rtype: bool
         """
         return (
             isinstance(obj, Credential)
             and obj.uid == self.uid
@@ -245,20 +245,20 @@
     """
     uid: UUID
     partner: Partner
     credential: Credential
     issued_date: datetime
     signature: str
 
-    def __eq__(self, obj: 'Claim'):
+    def __eq__(self, obj: object) -> bool:
         """
         Overriding of the equals method for simplified comparison between Claim objects.
 
         :param obj: The other instance of a claim object
-        :type obj: :class:`Claim`
+        :type obj: object
 
         :return: True if the two objects are equal
         :rtype: bool
         """
         return isinstance(obj, Claim) and obj.uid == self.uid
 
 
@@ -276,15 +276,15 @@
     :type last_verification: :class:`VerificationReport`
     """
     certificate: Claim
     revoked_date: Optional[datetime]
     last_verification: Optional[VerificationReport]
 
 
-class PaginatedResponse(NamedTuple, Generic[T]):
+class PaginatedResponse(NamedTuple):
     """
     Object representing a paginated response from the API.
     from the API
 
     :param page: The page the items are from
     :type page: int
 
@@ -294,28 +294,28 @@
     :param per_page: The number of items returned per page
     :type per_page: int
 
     :param total_items: The total number of items
     :type total_items: int
 
     :param items: The list of objects returned by the API
-    :type items: List[T]
+    :type items: List[Any]
     """
     page: int
     total_pages: int
     per_page: int
     total_items: int
-    items: List[T]
+    items: List[Any]
 
-    def __eq__(self, obj: 'PaginatedResponse'):
+    def __eq__(self, obj: object) -> bool:
         """
         Overriding of the equals method for simplified comparison between Paginated objects.
 
         :param obj: The other instance of a paginated object
-        :type obj: :class:`PaginatedResponse`
+        :type obj: object
 
         :return: True if the two objects are equal
         :rtype: bool
         """
         return (
                 isinstance(obj, PaginatedResponse)
                 and obj.page == self.page
```

### Comparing `vdx-helper-3.2.3/vdx_helper/util.py` & `vdx_helper-3.2.4/vdx_helper/util.py`

 * *Files identical despite different names*

### Comparing `vdx-helper-3.2.3/vdx_helper/vdx_helper.py` & `vdx_helper-3.2.4/vdx_helper/vdx_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import io
 import time
 from datetime import datetime
 from http import HTTPStatus
-from typing import Optional, Callable, Dict, TypeVar, Tuple, List, Iterable, BinaryIO
+from typing import Optional, Callable, Dict, Tuple, List, Iterable, BinaryIO, Any
 from uuid import UUID
 
 import requests
 from nndict import nndict
 from vdx_helper.errors import error_from_response, VDXError
 from vdx_helper.mappers import file_mapper, get_paginated_mapper, credential_mapper, job_mapper, \
     certificate_mapper, verification_mapper
 from vdx_helper.util import optional_uuid_to_string, optional_uuids_to_string, datetime_from_string, uuids_to_string
 
-T = TypeVar('T')
-
 
 class VDXHelper:
     """
     Helper class that allows its users to connect to the VDX Core API with little fuss. Each method corresponds to
     an endpoint on the Core API, including all of its parameters. By default, the results are mapped into specific
     objects, but a JSON mapper can also be used (directly returns the results in JSON), as well as custom mappers.
     More information on mappers on the :mod:`vdx_helper.mappers` module.
@@ -92,27 +90,27 @@
         if self.auth_token is None or time.time() > self.token_expiration_date:
             self.auth_token, token_expiration_date = self._fetch_token()
             self.token_expiration_date = token_expiration_date
 
         return self.auth_token
 
     @property
-    def header(self) -> dict:
+    def header(self) -> Dict[str, Any]:
         """
         Creates a header structure to be used by all requests for authentication.
 
         :return: The request header
-        :rtype: dict
+        :rtype: Dict[str, Any]
         """
         return {"Authorization": f"Bearer {self._token}", "Accept": "application/json"}
 
     def upload_file(self,
                     file_stream: BinaryIO,
                     ignore_duplicated: bool = False,
-                    mapper: Callable[[dict], T] = file_mapper) -> T:
+                    mapper: Callable[[Dict[str, Any]], Any] = file_mapper) -> Any:
         """
         Upload a file to the Core API servers.
 
         :param file_stream: File to be uploaded
         :type file_stream: BinaryIO
 
         :param ignore_duplicated: Flag indicating if duplicate files should be ignored. If true, and the file has
@@ -133,62 +131,66 @@
 
         status = HTTPStatus(response.status_code)
         if status not in [HTTPStatus.OK, HTTPStatus.CREATED]:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def get_file(self, file_hash: str, mapper: Callable[[dict], T] = file_mapper) -> T:
+    def get_file(self, file_hash: str, mapper: Callable[[Dict[str, Any]], Any] = file_mapper) -> Any:
         """
         Retrieve file details by its hash.
 
         :param file_hash: File hash to retrieve
         :type file_hash: str
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         response = requests.get(f"{self.api_url}/files/{file_hash}", headers=self.header)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def get_files(self, mapper: Callable[[dict], T] = get_paginated_mapper(file_mapper),
-                  file_hash: Optional[str] = None, **pagination) -> T:
+    def get_files(self, mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(file_mapper),
+                  file_hash: Optional[str] = None, **pagination: Dict[str, Any]) -> Any:
         """
         Retrieve all files uploaded by the Partner, or filter them via their hash.
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :param file_hash: File hash to filter by
         :type file_hash: str, optional
 
+        :param pagination: Keyword arguments for pagination
+        :type pagination: Dict[str, Any]
+
         :return: The result of the endpoint call
         :rtype: :class:`T`
         """
 
         params = nndict(file_hash=file_hash, **pagination)
         response = requests.get(f"{self.api_url}/files", headers=self.header, params=params)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
         return mapper(response.json()["result"])
 
-    def get_credentials(self, mapper: Callable[[dict], T] = get_paginated_mapper(credential_mapper), *,
-                        metadata: Optional[dict] = None, uid: Optional[UUID] = None,
+    def get_credentials(self, mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(credential_mapper), *,
+                        metadata: Optional[Dict[str, Any]] = None, uid: Optional[UUID] = None,
                         start_date: Optional[datetime] = None, end_date: Optional[datetime] = None,
-                        and_tags: Optional[str] = None, or_tags: Optional[str] = None, **pagination) -> T:
+                        and_tags: Optional[str] = None, or_tags: Optional[str] = None,
+                        **pagination: Dict[str, Any]) -> Any:
         """
         Retrieve all partner credentials, or filter by metadata values, uid,
         upload_date (start_date < upload_date < end_date), and tags.
 
         More information on tags on the `VDX Core API <https://docs.vizidox.com/#tags>`__ official documentation.
         Results are paginated, and the pagination parameters should be provided as keyword arguments.
 
@@ -214,18 +216,18 @@
         :param and_tags: Filter Credentials that contain all the given tags
         :type and_tags: List[str], optional
 
         :param or_tags: Filter Credentials that contain at least one of the given tags
         :type or_tags: List[str], optional
 
         :param pagination: Keyword arguments for pagination
-        :type pagination: dict
+        :type pagination: Dict[str, Any]
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         params = nndict(
             uid=optional_uuid_to_string(uid),
             upload_date_from=start_date,
             upload_date_until=end_date,
             and_tags=and_tags,
             or_tags=or_tags
@@ -239,48 +241,49 @@
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def get_credential(self, cred_uid: UUID, mapper: Callable[[dict], T] = credential_mapper) -> T:
+    def get_credential(self, cred_uid: UUID, mapper: Callable[[Dict[str, Any]], Any] = credential_mapper) -> Any:
         """
         Retrieve a specific credential from the Core API, via its UUID.
 
         :param cred_uid: Credential UID to obtain
         :type cred_uid: :class:`uuid.UUID`
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         response = requests.get(f"{self.api_url}/credentials/{cred_uid}", headers=self.header)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def create_credential(self, title: str, metadata: dict, tags: Optional[Iterable[str]] = None,
+    def create_credential(self, title: str, metadata: Dict[str, Any], tags: Optional[Iterable[str]] = None,
                           file_hashes: Optional[List[str]] = None, cred_ids: List[UUID] = None,
-                          expiry_date: Optional[str] = None, mapper: Callable[[dict], T] = credential_mapper) -> T:
+                          expiry_date: Optional[str] = None,
+                          mapper: Callable[[Dict[str, Any]], Any] = credential_mapper) -> Any:
         """
         Create a new credential from a previously uploaded file, or provided metadata.
 
         :param title: The title of the credential
         :type title: str
 
         :param metadata: Metadata values to filter by. A dictionary is expected with the key corresponding to the
                          field name found in the metadata, and the value corresponding to that field's value. Can be
                          an empty dictionary as long as at least one file hash is provided.
-        :type metadata: dict
+        :type metadata: Dict[str, Any]
 
         :param tags: Optional text tags that can be used to identify and filter the credential. Must have at least
                     3 characters, and can only contain alphanumeric characters, '-' or '_'
         :type tags: Iterable[str], optional
 
         :param file_hashes: List of hashes of files to associate to the credential. Must be hashes of files previously
                             uploaded to the core API. Can be None as long as provided metadata is not empty.
@@ -292,15 +295,15 @@
         :param expiry_date: Date the credential should expire, if applicable
         :type expiry_date: :class:`datetime.datetime`, optional
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         payload = nndict(
             title=title,
             files=file_hashes,
             credentials=optional_uuids_to_string(cred_ids),
             tags=list(set(tags)) if tags is not None else None,
             expiry_date=expiry_date
@@ -330,15 +333,15 @@
                 {
                     "credential_uid": "7f026924-b3f8-4670-bc65-37fd7da8867c",
                     "tags": ["tagD"]
                 }
             ]
 
         :param updated_credential_tags: Dictionary containing the credential UUIDs to update and the new tags to add
-        :type updated_credential_tags: dict
+        :type updated_credential_tags: Dict[str, List[str]]
         """
         payload = {"credentials": updated_credential_tags}
         response = requests.patch(f"{self.api_url}/credentials", headers=self.header, json=payload)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
@@ -392,69 +395,70 @@
                                   headers=self.header,
                                   params=params)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
-    def schedule_credentials(self, engine: str, credentials: List[UUID], mapper: Callable[[dict], T] = job_mapper) -> T:
+    def schedule_credentials(self, engine: str, credentials: List[UUID],
+                             mapper: Callable[[Dict[str, Any]], Any] = job_mapper) -> Any:
         """
         Schedule the given list of credentials to be issued on the Blockchain engine.
 
         :param engine: Blockchain Engine to schedule the credentials
         :type engine: str
 
         :param credentials: List of UUIDs of the credentials to schedule
         :type credentials: List[:class:`uuid.UUID`]
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         payload = {
             "engine": engine,
             "credentials": uuids_to_string(credentials)
         }
         response = requests.post(f"{self.api_url}/credentials/schedule", headers=self.header, json=payload)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.CREATED:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def issue_job(self, engine: str, mapper: Callable[[dict], T] = job_mapper) -> T:
+    def issue_job(self, engine: str, mapper: Callable[[Dict[str, Any]], Any] = job_mapper) -> Any:
         """
         Immediately issues the next scheduled job for the given blockchain engine, if there are scheduled credentials.
 
         :param engine: Blockchain engine to issue
         :type engine: str
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         payload = {"engine": engine}
 
         response = requests.post(f"{self.api_url}/jobs/immediate", headers=self.header, json=payload)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.CREATED:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def get_jobs(self, mapper: Callable[[dict], T] = get_paginated_mapper(job_mapper), *,
+    def get_jobs(self, mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(job_mapper), *,
                  job_status: Optional[str] = None, uid: Optional[UUID] = None,
                  start_date: Optional[datetime] = None, end_date: Optional[datetime] = None,
-                 and_tags: Optional[str] = None, or_tags: Optional[str] = None, **pagination) -> T:
+                 and_tags: Optional[str] = None, or_tags: Optional[str] = None, **pagination: Dict[str, Any]) -> Any:
         """
         Retrieve all partner jobs, or filter by a specific status, uid,
         issued date (start_date < issued_date < end_date), and tags.
 
         More information on tags on the `VDX Core API <https://docs.vizidox.com/#tags>`__ official documentation.
         Results are paginated, and the pagination parameters should be provided as keyword arguments.
         For more information on the possible parameters, check the
@@ -478,18 +482,18 @@
         :param and_tags: Filter Jobs that contain all the given tags
         :type and_tags: List[str], optional
 
         :param or_tags: Filter Jobs that contain at least one of the given tags
         :type or_tags: List[str], optional
 
         :param pagination: Keyword arguments for pagination
-        :type pagination: dict
+        :type pagination: Dict[str, Any]
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         params = nndict(
             uid=optional_uuid_to_string(uid),
             status=job_status,
             issued_date_from=start_date,
             issued_date_until=end_date,
             and_tags=and_tags,
@@ -501,36 +505,36 @@
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def get_job(self, job_uid: UUID, mapper: Callable[[dict], T] = job_mapper) -> T:
+    def get_job(self, job_uid: UUID, mapper: Callable[[Dict[str, Any]], Any] = job_mapper) -> Any:
         """
         Retrieve a specific job from the Core API, via its UUID.
 
         :param job_uid: Job UID to obtain
         :type job_uid: :class:`uuid.UUID`
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         response = requests.get(f"{self.api_url}/jobs/{job_uid}", headers=self.header)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def update_job_tags(self, updated_job_tags: List[dict]) -> None:
+    def update_job_tags(self, updated_job_tags: List[Dict[str, Any]]) -> None:
         """
         Add new tags to one or more jobs. Previous job tags are not changed.
 
         Example format of the parameter:
 
         .. code-block:: json
 
@@ -542,26 +546,26 @@
                 {
                     "job_uid": "7f026924-b3f8-4670-bc65-37fd7da8867c",
                     "tags": ["tagD"]
                 }
             ]
 
         :param updated_job_tags: Dictionary containing the job UUIDs to update and the new tags to add
-        :type updated_job_tags: dict
+        :type updated_job_tags: Dict[str, Any]
         """
         payload = {"jobs": updated_job_tags}
         response = requests.patch(f"{self.api_url}/jobs", headers=self.header, json=payload)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return None
 
-    def replace_job_tags(self, replace_job_tags: List[dict]) -> None:
+    def replace_job_tags(self, replace_job_tags: List[Dict[str, Any]]) -> None:
         """
         Replaces all the given job tags with the new ones.
 
         Example format of the parameter:
 
         .. code-block:: json
 
@@ -572,28 +576,30 @@
                 },
                 {
                     "job_uid": "7f026924-b3f8-4670-bc65-37fd7da8867c",
                     "tags": ["tagD"]
                 }
             ]
 
-        :param replace_job_tags: Dictionary containing the job UUIDs to update and the new tags to replace the old ones with
-        :type replace_job_tags: dict
+        :param replace_job_tags: Dictionary containing the job UUIDs to update and the new tags to replace
+                                 the old ones with
+        :type replace_job_tags: Dict[str, Any]
         """
         payload = {"jobs": replace_job_tags}
         response = requests.put(f"{self.api_url}/jobs", headers=self.header, json=payload)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return None
 
     def get_job_certificates(self, job_uid: UUID, and_tags: Optional[str] = None, or_tags: Optional[str] = None,
-                             mapper: Callable[[dict], T] = get_paginated_mapper(certificate_mapper), **pagination) -> T:
+                             mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(certificate_mapper),
+                             **pagination: Dict[str, Any]) -> Any:
         """
         Retrieve all certificates issued in a specific Job, or filter by tags.
 
         More information on tags on the `VDX Core API <https://docs.vizidox.com/#tags>`__ official documentation.
 
         Results are paginated, and the pagination parameters should be provided as keyword arguments.
 
@@ -609,32 +615,32 @@
         :param or_tags: Filter Certificates issued from credentials that contain at least one of the given tags
         :type or_tags: List[str], optional
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :param pagination: Keyword arguments for pagination
-        :type pagination: dict
+        :type pagination: Dict[str, Any]
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         params = nndict(and_tags=and_tags, or_tags=or_tags)
         params = {**params, **nndict(pagination)}
         response = requests.get(f"{self.api_url}/jobs/{job_uid}/certificates", headers=self.header, params=params)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
     def get_job_credentials(self, job_uid: UUID, and_tags: Optional[str] = None, or_tags: Optional[str] = None,
-                            mapper: Callable[[dict], T] = get_paginated_mapper(credential_mapper),
-                            **pagination) -> Optional[T]:
+                            mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(credential_mapper),
+                            **pagination: Dict[str, Any]) -> Optional[Any]:
         """
         Retrieve all credentials issued in a specific Job, or filter by tags.
 
         More information on tags on the `VDX Core API <https://docs.vizidox.com/#tags>`__ official documentation.
 
         Results are paginated, and the pagination parameters should be provided as keyword arguments.
 
@@ -650,35 +656,35 @@
         :param or_tags: Filter Credentials that contain at least one of the given tags
         :type or_tags: List[str], optional
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :param pagination: Keyword arguments for pagination
-        :type pagination: dict
+        :type pagination: Dict[str, Any]
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         params = nndict(and_tags=and_tags, or_tags=or_tags)
         params = {**params, **nndict(pagination)}
         response = requests.get(f"{self.api_url}/jobs/{job_uid}/credentials", headers=self.header, params=params)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
-    def get_certificates(self, mapper: Callable[[dict], T] = get_paginated_mapper(certificate_mapper), *,
+    def get_certificates(self, mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(certificate_mapper), *,
                          job_uid: Optional[UUID] = None, cred_uid: Optional[UUID] = None, uid: Optional[UUID] = None,
                          start_date: Optional[datetime] = None, end_date: Optional[datetime] = None,
                          and_credential_tags: Optional[str] = None, or_credential_tags: Optional[str] = None,
                          and_job_tags: Optional[str] = None, or_job_tags: Optional[str] = None,
-                         verification_status: Optional[str] = None, **pagination) -> T:
+                         verification_status: Optional[str] = None, **pagination: Dict[str, Any]) -> Any:
         """
         Retrieve all partner certificates, or filter by job, credential, uid,
         issued date (start_date < issued_date < end_date), and credential or job tags.
 
         More information on tags on the `VDX Core API <https://docs.vizidox.com/#tags>`__ official documentation.
 
         Results are paginated, and the pagination parameters should be provided as keyword arguments.
@@ -716,18 +722,18 @@
         :param or_job_tags: Filter Certificates issued on Jobs that contain at least one of the given tags
         :type or_job_tags: List[str], optional
 
         :param verification_status: Filter Certificates in the given verification status
         :type verification_status: str, optional
 
         :param pagination: Keyword arguments for pagination
-        :type pagination: dict
+        :type pagination: Dict[str, Any]
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         params = nndict(
             uid=optional_uuid_to_string(uid),
             job_uid=optional_uuid_to_string(job_uid),
             credential_uid=optional_uuid_to_string(cred_uid),
             issued_date_from=start_date,
             issued_date_until=end_date,
@@ -751,49 +757,49 @@
         Downloads the JSON proof file for the Certificate, containing all relevant Blockchain details as well
         as the metadata of the corresponding issued credential.
 
         :param cert_uid: UUID of the certificate to download
         :type cert_uid: :class:`uuid.UUID`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`io.BytesIO`
         """
         response = requests.get(f"{self.api_url}/certificates/{cert_uid}/download",headers=self.header)
 
         status = HTTPStatus(response.status_code)
 
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return io.BytesIO(response.content)
 
     def verify_by_uid(self, cert_uid: UUID,
-                      mapper: Callable[[dict], T] = verification_mapper) -> T:
+                      mapper: Callable[[Dict[str, Any]], Any] = verification_mapper) -> Any:
         """
         Verify a certificate via its UID.
 
         :param cert_uid: UUID of the certificate to verify
         :type cert_uid: :class:`uuid.UUID`
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         response = requests.get(f"{self.api_url}/verify/{cert_uid}", headers=self.header)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
     def verify_by_certificate(self, filename: str, file_stream: BinaryIO, file_content_type: str,
-                              mapper: Callable[[dict], T] = verification_mapper) -> T:
+                              mapper: Callable[[Dict[str, Any]], Any] = verification_mapper) -> Any:
         """
         Verify a certificate via its proof file.
 
         :param filename: Name of the file
         :type filename: str
 
         :param file_stream: Certificate proof file stream
@@ -802,29 +808,30 @@
         :param file_content_type: Content type of the file
         :type file_content_type: str
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         file_stream.seek(0)
         payload = {"file": (filename, file_stream, file_content_type)}
 
         response = requests.post(f"{self.api_url}/verify/upload/certificate", headers=self.header, files=payload)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
     def verify_by_file(self, filename: str, file_stream: BinaryIO, file_content_type: str,
-                       mapper: Callable[[dict], T] = get_paginated_mapper(verification_mapper), **pagination) -> T:
+                       mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(verification_mapper),
+                       **pagination: Dict[str, Any]) -> Any:
         """
         Verify a certificate via the credential file.
         Results are paginated, and the pagination parameters should be provided as keyword arguments.
 
         For more information on the possible parameters, check the
         `VDX Core API <https://docs.vizidox.com/#pagination>`__ official documentation.
 
@@ -837,51 +844,51 @@
         :param file_content_type: Content type of the file
         :type file_content_type: str
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :param pagination: Keyword argument containing the pagination parameters
-        :type pagination: dict
+        :type pagination: Dict[str, Any]
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         payload = {"file": (filename, file_stream, file_content_type)}
         params = {**nndict(pagination)}
 
         response = requests.post(f"{self.api_url}/verify/upload/file", headers=self.header, files=payload, params=params)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
 
         return mapper(response.json()["result"])
 
     def verify_by_credential_uid(self, cred_uid: UUID,
-                                 mapper: Callable[[dict], T] = get_paginated_mapper(verification_mapper),
-                                 **pagination) -> T:
+                                 mapper: Callable[[Dict[str, Any]], Any] = get_paginated_mapper(verification_mapper),
+                                 **pagination: Dict[str, Any]) -> Any:
         """
         Verify certificates via their credential UID.
         Results are paginated, and the pagination parameters should be provided as keyword arguments.
 
         For more information on the possible parameters, check the
         `VDX Core API <https://docs.vizidox.com/#pagination>`__ official documentation.
 
         :param cred_uid: UUID of the credential
         :type cred_uid: :class:`uuid.UUID`
 
         :param mapper: Optional mapper to change the format of the endpoint response
         :type mapper: :class:`typing.Callable`
 
         :param pagination: Keyword argument containing the pagination parameters
-        :type pagination: dict
+        :type pagination: Dict[str, Any]
 
         :return: The result of the endpoint call
-        :rtype: :class:`T`
+        :rtype: :class:`typing.Any`
         """
         params = {**nndict(pagination)}
         response = requests.get(f"{self.api_url}/verify/credential/{cred_uid}", headers=self.header, params=params)
 
         status = HTTPStatus(response.status_code)
         if status is not HTTPStatus.OK:
             raise error_from_response(status, response)
```

### Comparing `vdx-helper-3.2.3/setup.py` & `vdx_helper-3.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['vdx_helper']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['nndict==1.0.0', 'requests>=2.27,<3.0']
-
-setup_kwargs = {
-    'name': 'vdx-helper',
-    'version': '3.2.3',
-    'description': 'Python client library to connect to the VDX Core API',
-    'long_description': "[![PyPI version](https://badge.fury.io/py/vdx-helper.svg)](https://badge.fury.io/py/vdx-helper) \n[![Downloads](https://static.pepy.tech/personalized-badge/vdx-helper?period=total&units=abbreviation&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/vdx-helper)\n\n# VDX Helper\nThis repository provides a wrapper for every call made to VDX Core Api.\n\n## How it works\nThis helper first needs to be authorized by wielding valid token from the authentication server, then use that token for further requests as long as it has not expired.\n\nEach method also allows one to include their own custom mappers, enabling the method to return the result in the format the user wishes.\n\n## Prerequisites\n\n- Python Poetry\n- Docker + Docker-compose\n\n## Usage\n\n### Initialization\n\nRequired parameters: \n- api_url: The url leading to Core API server\n- auth_url: The url leading to authentication server\n- client_secret: The authentication secret\n- client_id: The ID of the client / partner\n\n\n```\nvdx_helper = VDXHelper(api_url='https://vizidox-core-api.com', auth_url='https://auth.com', client_secret=secret, client_id=client_id)\n```\n\n### Mapper example\nA mapper will receive a json-formatted parameter as their input. The following example mapper will add a field\n\n```\ndef example_mapper(json_file):\n    returned_json = copy.deepcopy(json_file)\n    returned_json['additional_field'] = 'additional_value'\n    return returned_json\n```\n\n### Usage example\n\n```\nvdx_helper.upload_file(file=the_file_to_upload, mapper=example_mapper)\n```\n\n## Running the tests\n\nYou can run the tests with poetry if you like. You can also obtain the code coverage.\n\n```\npoetry run pytest --cov=vdx_helper\n```\n\n### Run the test locally with docker-compose step-by-step\n1. Spin up the docker-containers\n```\ndocker-compose up -d\n```\n\n2. Run the tests via the vdx-helper docker container\n```\ndocker-compose run vdx-helper pytest tests\n```\n\n\n## Documentation\n\nTo build the documentation locally:\n\n```shell\ncd docs\nmake html\n```\n\nThe build files can be found in docs/build. Open the generated index.html file in the html folder, and you can now \nnavigate the documentation. Repeat the above command and refresh your browser every time you update the documentation.\nAll source files are in docs/source, with vdx_helper containing the documentation generated from docstrings.\n \n## Authors\n\n* **Tiago Santos** - *Initial work* - [Vizidox](https://vizidox.com)\n* **Joana Teixeira** - *Corrections and improvements* - [Vizidox](https://vizidox.com)\n* **Rita Mariquitos** - *Corrections and improvements* - [Vizidox](https://vizidox.com)",
-    'author': 'Joana Teixeira',
-    'author_email': 'joana.teixeira@vizidox.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://vizidox.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: vdx-helper
+Version: 3.2.4
+Summary: Python client library to connect to the VDX Core API
+Home-page: https://vizidox.com
+License: MIT
+Author: Joana Teixeira
+Author-email: joana.teixeira@vizidox.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: nndict (>=2.0.1,<3.0.0)
+Requires-Dist: requests (>=2.27,<3.0)
+Project-URL: Documentation, https://helper.vizidox.com/
+Project-URL: Repository, https://github.com/Morphotech/vdx-helper-python
+Description-Content-Type: text/markdown
+
+[![PyPI version](https://badge.fury.io/py/vdx-helper.svg)](https://badge.fury.io/py/vdx-helper) 
+[![Downloads](https://static.pepy.tech/personalized-badge/vdx-helper?period=total&units=abbreviation&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/vdx-helper)
+
+# VDX Helper
+This repository provides a wrapper for every call made to VDX Core Api.
+
+## How it works
+This helper first needs to be authorized by wielding valid token from the authentication server, then use that token for further requests as long as it has not expired.
+
+Each method also allows one to include their own custom mappers, enabling the method to return the result in the format the user wishes.
+
+## Prerequisites
+
+- Python Poetry
+- Docker + Docker-compose
+
+## Usage
+
+### Initialization
+
+Required parameters: 
+- api_url: The url leading to Core API server
+- auth_url: The url leading to authentication server
+- client_secret: The authentication secret
+- client_id: The ID of the client / partner
+
+
+```
+vdx_helper = VDXHelper(api_url='https://vizidox-core-api.com', auth_url='https://auth.com', client_secret=secret, client_id=client_id)
+```
+
+### Mapper example
+A mapper will receive a json-formatted parameter as their input. The following example mapper will add a field
+
+```
+def example_mapper(json_file):
+    returned_json = copy.deepcopy(json_file)
+    returned_json['additional_field'] = 'additional_value'
+    return returned_json
+```
+
+### Usage example
+
+```
+vdx_helper.upload_file(file=the_file_to_upload, mapper=example_mapper)
+```
+
+## Running the tests
+
+You can run the tests with poetry if you like. You can also obtain the code coverage.
+
+```
+poetry run pytest --cov=vdx_helper
+```
+
+* **Mypy:**
+```shell
+poetry run mypy --config-file conf/mypy.ini vdx_helper
+```
+
+* **Coverage:**
+```shell
+poetry run coverage run --source=vdx_helper -m pytest
+poetry run coverage report
+```
+
+* **Tox:**
+```shell
+tox -p
+```
+
+### Run the test locally with docker-compose step-by-step
+1. Spin up the docker-containers
+```
+docker-compose up -d
+```
+
+2. Run the tests via the vdx-helper docker container
+```
+docker-compose run vdx-helper pytest tests
+```
+
+
+## Documentation
+
+To build the documentation locally:
+
+```shell
+cd docs
+make html
+```
+
+The build files can be found in docs/build. Open the generated index.html file in the html folder, and you can now 
+navigate the documentation. Repeat the above command and refresh your browser every time you update the documentation.
+All source files are in docs/source, with vdx_helper containing the documentation generated from docstrings.
+ 
+## Authors
+
+* **Tiago Santos** - *Initial work* - [Vizidox](https://vizidox.com)
+* **Joana Teixeira** - *Corrections and improvements* - [Vizidox](https://vizidox.com)
+* **Rita Mariquitos** - *Corrections and improvements* - [Vizidox](https://vizidox.com)
```

