# Comparing `tmp/live-fast-api-0.0.0.tar.gz` & `tmp/live-fast-api-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-fast-api-0.0.0.tar", last modified: Tue Mar 28 10:17:41 2023, max compression
+gzip compressed data, was "live-fast-api-0.0.1.tar", last modified: Wed Apr 12 14:24:16 2023, max compression
```

## Comparing `live-fast-api-0.0.0.tar` & `live-fast-api-0.0.1.tar`

### file list

```diff
@@ -1,27 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 10:17:41.601117 live-fast-api-0.0.0/
--rw-rw-rw-   0        0        0      215 2023-03-28 10:17:41.000000 live-fast-api-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2040 2023-03-28 10:17:41.601117 live-fast-api-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1231 2023-02-04 16:28:03.000000 live-fast-api-0.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:17:41.586973 live-fast-api-0.0.0/live_api/
--rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.0/live_api/__init__.py
--rw-rw-rw-   0        0        0     8981 2023-03-09 10:59:33.000000 live-fast-api-0.0.0/live_api/base.py
--rw-rw-rw-   0        0        0      279 2023-02-04 16:29:06.000000 live-fast-api-0.0.0/live_api/document.py
--rw-rw-rw-   0        0        0    15239 2023-03-10 07:32:08.000000 live-fast-api-0.0.0/live_api/endpoint.py
--rw-rw-rw-   0        0        0    18796 2023-03-10 07:32:41.000000 live-fast-api-0.0.0/live_api/engine.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:17:41.572858 live-fast-api-0.0.0/live_api/source/
-drwxrwxrwx   0        0        0        0 2023-03-28 10:17:41.572858 live-fast-api-0.0.0/live_api/source/assets/
-drwxrwxrwx   0        0        0        0 2023-03-28 10:17:41.587972 live-fast-api-0.0.0/live_api/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.0/live_api/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.0/live_api/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-03-28 10:17:41.600117 live-fast-api-0.0.0/live_fast_api.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-03-28 10:17:41.000000 live-fast-api-0.0.0/live_fast_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-03-28 10:17:41.000000 live-fast-api-0.0.0/live_fast_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 10:17:41.000000 live-fast-api-0.0.0/live_fast_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-03-28 10:17:41.000000 live-fast-api-0.0.0/live_fast_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-28 10:17:41.000000 live-fast-api-0.0.0/live_fast_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-03-28 10:17:41.000000 live-fast-api-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       77 2023-03-28 10:14:28.000000 live-fast-api-0.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       68 2023-03-28 10:14:28.000000 live-fast-api-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 10:17:41.601117 live-fast-api-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1580 2023-03-28 10:17:38.000000 live-fast-api-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.029597 live-fast-api-0.0.1/
+-rw-rw-rw-   0        0        0      215 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2054 2023-04-12 14:24:16.028597 live-fast-api-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.1/build.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.014595 live-fast-api-0.0.1/live_api/
+-rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.1/live_api/__init__.py
+-rw-rw-rw-   0        0        0     8981 2023-03-09 10:59:33.000000 live-fast-api-0.0.1/live_api/base.py
+-rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.1/live_api/document.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.018597 live-fast-api-0.0.1/live_api/endpoints/
+-rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.1/live_api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.1/live_api/endpoints/data.py
+-rw-rw-rw-   0        0        0    10886 2023-04-12 14:24:12.000000 live-fast-api-0.0.1/live_api/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.1/live_api/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.1/live_api/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.021597 live-fast-api-0.0.1/live_api/service/
+-rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.1/live_api/service/__init__.py
+-rw-rw-rw-   0        0        0    18136 2023-04-12 14:16:50.000000 live-fast-api-0.0.1/live_api/service/rest.py
+-rw-rw-rw-   0        0        0    22076 2023-04-12 14:21:27.000000 live-fast-api-0.0.1/live_api/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.005497 live-fast-api-0.0.1/live_api/source/
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.005643 live-fast-api-0.0.1/live_api/source/assets/
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.022596 live-fast-api-0.0.1/live_api/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.1/live_api/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.1/live_api/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-04-12 14:24:16.028597 live-fast-api-0.0.1/live_fast_api.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 14:24:15.000000 live-fast-api-0.0.1/live_fast_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-04-12 14:23:27.000000 live-fast-api-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       77 2023-03-28 10:14:28.000000 live-fast-api-0.0.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       68 2023-03-28 10:14:28.000000 live-fast-api-0.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:24:16.029597 live-fast-api-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-04-12 14:23:23.000000 live-fast-api-0.0.1/setup.py
```

### Comparing `live-fast-api-0.0.0/PKG-INFO` & `live-fast-api-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.0
+Version: 0.0.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # live-api
 
-> A framework for developing responsive, live and dynamic REST APIs with python.
+> A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
@@ -34,15 +34,15 @@
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
 
-- A framework for developing responsive, live and dynamic REST APIs with python.
+- A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 #### dependencies:
 
 - opening:
   As for this is a really complex program, which uses a lot of modules, there are required dependencies needed
   in order to run the program. keep in mined the program was writen in python 3.9, so any python version lower
   than 3.8 might not work properly. Moreover, built-in python modules are being used, so keep that in mind.
```

### Comparing `live-fast-api-0.0.0/README.md` & `live-fast-api-0.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # live-api
 
-> A framework for developing responsive, live and dynamic REST APIs with python.
+> A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
@@ -13,15 +13,15 @@
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
 
-- A framework for developing responsive, live and dynamic REST APIs with python.
+- A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 #### dependencies:
 
 - opening:
   As for this is a really complex program, which uses a lot of modules, there are required dependencies needed
   in order to run the program. keep in mined the program was writen in python 3.9, so any python version lower
   than 3.8 might not work properly. Moreover, built-in python modules are being used, so keep that in mind.
```

### Comparing `live-fast-api-0.0.0/build.py` & `live-fast-api-0.0.1/build.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.0/live_api/base.py` & `live-fast-api-0.0.1/live_api/base.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.0/live_api/endpoint.py` & `live-fast-api-0.0.1/live_api/endpoints/engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,237 +3,32 @@
 import datetime as dt
 from functools import wraps
 from pathlib import Path
 from typing import (
     List, Any, Union, Dict, Optional, Tuple, Callable
 )
 
-import dill
-import codecs
-
 from fastapi.openapi.docs import get_swagger_ui_html
-from fastapi.responses import (
-    RedirectResponse, Response, FileResponse,
-    JSONResponse, HTMLResponse, StreamingResponse,
-    PlainTextResponse, UJSONResponse, ORJSONResponse
-)
 
 from represent import Modifiers, BaseModel
 
+from live_api.endpoints.process import copy
+from live_api.endpoints.data import DOCS
+
 __all__ = [
-    "Responses",
     "BaseEndpoint",
     "DocsEndpoint",
-    "GET",
-    "POST",
-    "DELETE",
-    "UPLOAD",
-    "HEAD",
-    "PATCH",
-    "PUT",
-    "DOCS",
-    "FAVICON",
-    "METHODS",
-    "EndpointRedirectResponse",
-    "EndpointResponse",
-    "EndpointFileResponse",
-    "EndpointJSONResponse",
-    "EndpointHTMLResponse",
-    "EndpointStreamingResponse",
-    "EndpointPlainTextResponse",
-    "EndpointUJSONResponse",
-    "EndpointORJSONResponse",
-    "RESPONSES",
-    "loads",
-    "dumps",
-    "decode",
-    "encode",
     "Record",
     "DataContainer",
-    "UnSerializableObjectError",
-    "UnDeserializableObjectError"
+    "valid_endpoints"
 ]
 
-DOCS = '/docs'
-FAVICON = '/favicon.ico'
-
-class Methods(BaseModel):
-    """A class to contain the methods of the service."""
-
-    GET = "GET"
-    POST = "POST"
-    DELETE = "DELETE"
-    UPLOAD = "UPLOAD"
-    HEAD = "HEAD"
-    PATCH = "PATCH"
-    PUT = "PUT"
-
-    METHODS = (
-        GET, POST, DELETE, UPLOAD,
-        HEAD, PATCH, PUT
-    )
-# end Methods
-
-GET = Methods.GET
-POST = Methods.POST
-DELETE = Methods.DELETE
-UPLOAD = Methods.UPLOAD
-HEAD = Methods.HEAD
-PATCH = Methods.PATCH
-PUT = Methods.PUT
-
-METHODS = Methods.METHODS
-
-class Responses(BaseModel):
-    """A class to contain the response types."""
-
-    EndpointRedirectResponse = RedirectResponse
-    EndpointResponse = Response
-    EndpointFileResponse = FileResponse
-    EndpointJSONResponse = JSONResponse
-    EndpointHTMLResponse = HTMLResponse
-    EndpointStreamingResponse = StreamingResponse
-    EndpointPlainTextResponse = PlainTextResponse
-    EndpointUJSONResponse = UJSONResponse
-    EndpointORJSONResponse = ORJSONResponse
-
-    RESPONSES = (
-        EndpointRedirectResponse, EndpointResponse,
-        EndpointFileResponse, EndpointJSONResponse,
-        EndpointHTMLResponse, EndpointStreamingResponse,
-        EndpointPlainTextResponse, EndpointUJSONResponse,
-        EndpointORJSONResponse
-    )
-# end Responses
-
-EndpointRedirectResponse = Responses.EndpointRedirectResponse
-EndpointResponse = Responses.EndpointResponse
-EndpointFileResponse = Responses.EndpointFileResponse
-EndpointJSONResponse = Responses.EndpointJSONResponse
-EndpointHTMLResponse = Responses.EndpointHTMLResponse
-EndpointStreamingResponse = Responses.EndpointStreamingResponse
-EndpointPlainTextResponse = Responses.EndpointPlainTextResponse
-EndpointUJSONResponse = Responses.EndpointUJSONResponse
-EndpointORJSONResponse = Responses.EndpointORJSONResponse
-
-RESPONSES = Responses.RESPONSES
-
 Method = str
 Methods = List[Method]
 
-SerializationExceptions = (
-    TypeError, ValueError, AttributeError,
-    dill.PicklingError, dill.PickleError
-)
-
-class UnSerializableObjectError(ValueError):
-    """A class to represent an exception."""
-
-    def __init__(self, data: Optional[Any] = None) -> None:
-        """
-        Defines the class attributes.
-
-        :param data: The commands to collect for the exception.
-        """
-
-        message = f" {repr(data)} of type {type(data)}" if data is not None else ""
-
-        super().__init__(
-            f"Couldn't serialize the object{message}. "
-            f"Probably due to the object having weak "
-            f"references or C-type pointers."
-        )
-    # end __init__
-# end UnSerializableObjectError
-
-class UnDeserializableObjectError(ValueError):
-    """A class to represent an exception."""
-
-    def __init__(self, data: Optional[Any] = None) -> None:
-        """
-        Defines the class attributes.
-
-        :param data: The commands to collect for the exception.
-        """
-
-        message = f" {repr(data)} of type {type(data)}" if data is not None else ""
-
-        super().__init__(
-            f"Couldn't deserialize the object{message}. "
-            f"Probably due to the object having weak "
-            f"references or C-type pointers."
-        )
-    # end __init__
-# end UnDeserializableObjectError
-
-def dumps(data) -> bytes:
-    """
-    Encodes the object commands to a bytes string.
-
-    :param data: The data to dump.
-
-    :return: The bytes string commands.
-    """
-
-    try:
-        return dill.dumps(data)
-
-    except SerializationExceptions:
-        raise UnSerializableObjectError(data)
-    # end try
-# end dumps
-
-def loads(data: bytes) -> Any:
-    """
-    Decodes the object commands from a bytes string, to the object.
-
-    :param data: The commands to load into a string.
-
-    :return: The bytes string commands as object.
-    """
-
-    return dill.loads(data)
-# end loads
-
-def decode(data: str) -> bytes:
-    """
-    Decodes the object from a string.
-
-    :param data: The commands to load into a string.
-
-    :return: The object's commands.
-    """
-
-    return loads(codecs.decode(data.encode(), "base64"))
-# end decode
-
-def copy(data: Any) -> Any:
-    """
-    Copies the object.
-
-    :param data: The data to load into a copy.
-
-    :return: The object's copy.
-    """
-
-    return loads(dumps(data))
-# end copy
-
-def encode(data: Any) -> str:
-    """
-    Encodes the object into a string.
-
-    :param data: The data to load into a copy.
-
-    :return: An encoded string for the commands.
-    """
-
-    return codecs.encode(dumps(data), "base64").decode()
-# end encode
-
 class Record(BaseModel):
     """A class to represent a result object for commands and conditions calls."""
 
     def __init__(
             self, *,
             args: Optional[Tuple] = None,
             kwargs: Optional[Dict[str, Any]] = None,
@@ -362,15 +157,15 @@
 
     - path:
         The path to the endpoint through the api.
 
     - root:
         The root of the path to the endpoint, when not ''.
 
-    >>> from live_api.endpoint import BaseEndpoint, GET
+    >>> from live_api.endpoints import BaseEndpoint, GET
     >>>
     >>> class MyEndpoint(BaseEndpoint):
     >>>     ...
     >>>
     >>>     def endpoint(self, *args: Any, **kwargs: Any) -> Any:
     >>>         ...
     >>>
@@ -573,8 +368,42 @@
             ),
             swagger_favicon_url=(
                 self.icon if self.icon is not None else
                 "https://fastapi.tiangolo.com/img/favicon.png"
             )
         )
     # end answer
-# end DocsEndpoint
+# end DocsEndpoint
+
+def valid_endpoints(endpoints: Optional[Any] = None) -> Dict[str, BaseEndpoint]:
+    """
+    Process the endpoints' commands to validate and modify it.
+
+    :param endpoints: The endpoints object to check.
+
+    :return: The valid endpoints object.
+    """
+
+    if endpoints is None:
+        endpoints = {}
+
+    elif isinstance(endpoints, dict):
+        endpoints = {**endpoints}
+
+    else:
+        try:
+            endpoints = {
+                endpoint.path: endpoint for endpoint in endpoints
+            }
+
+        except ValueError:
+            raise ValueError(
+                f"Endpoints parameter must be either a dictionary "
+                f"with paths as keys and endpoint objects with matching "
+                f"paths as values, or an iterable object with endpoint objects, "
+                f"not: {endpoints}"
+            )
+        # end try
+    # end if
+
+    return endpoints
+# end valid_endpoints
```

### Comparing `live-fast-api-0.0.0/live_api/engine.py` & `live-fast-api-0.0.1/live_api/service/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# engine.py
+# rest.py
 
 import os
 import time
 import logging
 import threading
 import datetime as dt
 from typing import Any, Union, Iterable, Optional, Dict
 
 from uvicorn import Server, Config as ServiceConfig
 from fastapi import FastAPI, APIRouter
 
 from live_api.base import (
     terminate_thread, override_signature, icons
 )
-from live_api.endpoint import (
+from live_api.endpoints import (
     EndpointFileResponse, BaseEndpoint,
     GET, EndpointRedirectResponse,
-    DocsEndpoint, FAVICON, DOCS
+    DocsEndpoint, FAVICON, DOCS, valid_endpoints
 )
 
 from represent import BaseModel, Modifiers
 
 __all__ = [
-    "BaseService"
+    "RESTService"
 ]
 
 Port = Union[str, int]
 Host = str
 
 Endpoints = Dict[str, BaseEndpoint]
 EndpointsContainer = Union[
     Iterable[BaseEndpoint],
     Endpoints
 ]
 
-class BaseService(BaseModel):
+class RESTService(BaseModel):
     """
     A class to represent a service object.
 
     The BaseService is the parent class of service class.
     The service class creates a service object to deploy
     functionality of endpoint objects as a REST API.
 
@@ -58,26 +58,26 @@
 
     - home:
         The path to the home page of the web interface.
 
     - debug:
         The value to set the home page as the test page.
 
-    >>> from live_api.endpoint import BaseEndpoint, GET
-    >>> from live_api.engine import BaseService
+    >>> from live_api.endpoints import BaseEndpoint, GET
+    >>> from live_api.service.rest import RESTService
     >>>
     >>> class MyEndpoint(BaseEndpoint):
     >>>     ...
     >>>
     >>>     def endpoint(self, *args: Any, **kwargs: Any) -> Any:
     >>>         ...
     >>>
     >>> endpoint = MyEndpoint(path="/my_endpoint", methods=[GET])
     >>>
-    >>> service = BaseService(
+    >>> service = RESTService(
     >>>     name="service", path="<PATH TO THE SERVICE>",
     >>>     endpoints=[endpoint]
     >>> )
     >>>
     >>> service.run()
     """
 
@@ -195,37 +195,15 @@
         Process the endpoints' commands to validate and modify it.
 
         :param endpoints: The endpoints object to check.
 
         :return: The valid endpoints object.
         """
 
-        if endpoints is None:
-            endpoints = {}
-
-        elif isinstance(endpoints, dict):
-            endpoints = {**endpoints}
-
-        else:
-            try:
-                endpoints = {
-                    endpoint.path: endpoint for endpoint in endpoints
-                }
-
-            except ValueError:
-                raise ValueError(
-                    f"Endpoints parameter must be either a dictionary "
-                    f"with paths as keys and endpoint objects with matching "
-                    f"paths as values, or an iterable object with endpoint objects, "
-                    f"not: {endpoints}"
-                )
-            # end try
-        # end if
-
-        return endpoints
+        return valid_endpoints(endpoints=endpoints)
     # end valid_endpoints
 
     @property
     def root(self) -> str:
         """
         Gets the root path of the service.
```

### Comparing `live-fast-api-0.0.0/live_api/source/assets/icon/icon.ico` & `live-fast-api-0.0.1/live_api/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.0/live_api/source/assets/icon/icon.png` & `live-fast-api-0.0.1/live_api/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.0/live_fast_api.egg-info/PKG-INFO` & `live-fast-api-0.0.1/live_fast_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.0
+Version: 0.0.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # live-api
 
-> A framework for developing responsive, live and dynamic REST APIs with python.
+> A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
@@ -34,15 +34,15 @@
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
 
-- A framework for developing responsive, live and dynamic REST APIs with python.
+- A framework for developing responsive, live and dynamic RESTService APIs with python.
 
 #### dependencies:
 
 - opening:
   As for this is a really complex program, which uses a lot of modules, there are required dependencies needed
   in order to run the program. keep in mined the program was writen in python 3.9, so any python version lower
   than 3.8 might not work properly. Moreover, built-in python modules are being used, so keep that in mind.
```

### Comparing `live-fast-api-0.0.0/pyproject.toml` & `live-fast-api-0.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'live-fast-api'
-version = '0.0.0'
+version = '0.0.1'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `live-fast-api-0.0.0/setup.py` & `live-fast-api-0.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "live_api/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='live-fast-api',
-        version='0.0.0',
+        version='0.0.1',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

