# Comparing `tmp/pytest_httpx-0.8.0.tar.gz` & `tmp/pytest_httpx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest_httpx-0.8.0.tar", last modified: Wed Aug 26 12:10:45 2020, max compression
+gzip compressed data, was "dist/pytest_httpx-0.9.0.tar", last modified: Tue Sep 22 14:00:59 2020, max compression
```

## Comparing `pytest_httpx-0.8.0.tar` & `pytest_httpx-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-26 12:10:45.000000 pytest_httpx-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25359 2020-08-26 12:10:45.000000 pytest_httpx-0.8.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-26 12:10:45.000000 pytest_httpx-0.8.0/pytest_httpx.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25359 2020-08-26 12:10:44.000000 pytest_httpx-0.8.0/pytest_httpx.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-26 12:10:44.000000 pytest_httpx-0.8.0/pytest_httpx.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-08-26 12:10:44.000000 pytest_httpx-0.8.0/pytest_httpx.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2020-08-26 12:10:44.000000 pytest_httpx-0.8.0/pytest_httpx.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-08-26 12:10:44.000000 pytest_httpx-0.8.0/pytest_httpx.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-08-26 12:10:44.000000 pytest_httpx-0.8.0/pytest_httpx.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    18884 2020-08-26 12:10:15.000000 pytest_httpx-0.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-08-26 12:10:45.000000 pytest_httpx-0.8.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-26 12:10:45.000000 pytest_httpx-0.8.0/pytest_httpx/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2020-08-26 12:10:15.000000 pytest_httpx-0.8.0/pytest_httpx/_httpx_internals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2020-08-26 12:10:15.000000 pytest_httpx-0.8.0/pytest_httpx/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13672 2020-08-26 12:10:15.000000 pytest_httpx-0.8.0/pytest_httpx/_httpx_mock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2020-08-26 12:10:15.000000 pytest_httpx-0.8.0/pytest_httpx/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2140 2020-08-26 12:10:15.000000 pytest_httpx-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25419 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18936 2020-09-22 14:00:33.000000 pytest_httpx-0.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2020-09-22 14:00:33.000000 pytest_httpx-0.9.0/pytest_httpx/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1043 2020-09-22 14:00:33.000000 pytest_httpx-0.9.0/pytest_httpx/_httpx_internals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13651 2020-09-22 14:00:33.000000 pytest_httpx-0.9.0/pytest_httpx/_httpx_mock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      371 2020-09-22 14:00:33.000000 pytest_httpx-0.9.0/pytest_httpx/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25419 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      346 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/pytest_httpx.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-09-22 14:00:59.000000 pytest_httpx-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2140 2020-09-22 14:00:33.000000 pytest_httpx-0.9.0/setup.py
```

### Comparing `pytest_httpx-0.8.0/PKG-INFO` & `pytest_httpx-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_httpx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Send responses to httpx.
 Home-page: https://colin-b.github.io/pytest_httpx/
 Author: Colin Bounouar
 Author-email: colin.bounouar.dev@gmail.com
 Maintainer: Colin Bounouar
 Maintainer-email: colin.bounouar.dev@gmail.com
 License: MIT
@@ -346,15 +346,15 @@
         
         ## Add callbacks
         
         You can perform custom manipulation upon request reception by registering callbacks.
         
         Callback should expect at least two parameters:
          * request: The received [`httpx.Request`](https://www.python-httpx.org/api/#request).
-         * timeout: The [timeouts](https://www.python-httpx.org/advanced/#timeout-configuration) linked to the request.
+         * ext: The extensions (including the [timeouts](https://www.python-httpx.org/advanced/#timeout-configuration)) linked to the request.
         
         If all callbacks are not executed during test execution, the test case will fail at teardown.
         
         This behavior can be disabled thanks to the `assert_all_responses_were_requested` fixture:
         
         ```python
         import pytest
@@ -362,15 +362,15 @@
         @pytest.fixture
         def assert_all_responses_were_requested() -> bool:
             return False
         ```
         
         ### Dynamic responses
         
-        Callback should return a httpcore response (as a tuple), you can use `pytest_httpx.to_response` function to create such a tuple.
+        Callback should return a `httpcore` response (as a tuple), you can use `pytest_httpx.to_response` function to create such a tuple.
         
         ```python
         import httpx
         from pytest_httpx import HTTPXMock, to_response
         
         
         def test_dynamic_response(httpx_mock: HTTPXMock):
@@ -396,16 +396,16 @@
         ```python
         import httpx
         import pytest
         from pytest_httpx import HTTPXMock
         
         
         def test_exception_raising(httpx_mock: HTTPXMock):
-            def raise_timeout(request, timeout):
-                raise httpx.ReadTimeout(f"Unable to read within {timeout}", request=request)
+            def raise_timeout(request, ext: dict):
+                raise httpx.ReadTimeout(f"Unable to read within {ext['timeout']}", request=request)
         
             httpx_mock.add_callback(raise_timeout)
             
             with httpx.Client() as client:
                 with pytest.raises(httpx.ReadTimeout):
                     client.get("http://test_url")
         
@@ -432,15 +432,15 @@
         
         In case all matching callbacks have been executed, the last one (according to the registration order) will be executed.
         
         You can add criteria so that callback will be sent only in case of a more specific matching.
         
         #### Matching on URL
         
-        `url` parameter can either be a string, a python [re.Pattern](https://docs.python.org/3/library/re.html) instance or a [httpx.URL](https://www.python-httpx.org/api/#url) instance.
+        `url` parameter can either be a string, a python [`re.Pattern`](https://docs.python.org/3/library/re.html) instance or a [`httpx.URL`](https://www.python-httpx.org/api/#url) instance.
         
         Matching is performed on the full URL, query parameters included.
         
         #### Matching on HTTP method
         
         Use `method` parameter to specify the HTTP method (POST, PUT, DELETE, PATCH, HEAD) executing the callback.
         
@@ -626,14 +626,15 @@
         | body (as bytes) | `body=b"sample"` | `data=b"sample"` |
         | body (as str) | `body="sample"` | `data="sample"` |
         | body (as JSON) | `payload=["sample"]` | `json=["sample"]` |
         | status code | `status=201` | `status_code=201` |
         
         Sample adding a response with `aioresponses`:
         ```python
+        import pytest
         from aioresponses import aioresponses
         
         
         @pytest.fixture
         def mock_aioresponse():
             with aioresponses() as m:
                 yield m
```

### Comparing `pytest_httpx-0.8.0/pytest_httpx.egg-info/PKG-INFO` & `pytest_httpx-0.9.0/pytest_httpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-httpx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Send responses to httpx.
 Home-page: https://colin-b.github.io/pytest_httpx/
 Author: Colin Bounouar
 Author-email: colin.bounouar.dev@gmail.com
 Maintainer: Colin Bounouar
 Maintainer-email: colin.bounouar.dev@gmail.com
 License: MIT
@@ -346,15 +346,15 @@
         
         ## Add callbacks
         
         You can perform custom manipulation upon request reception by registering callbacks.
         
         Callback should expect at least two parameters:
          * request: The received [`httpx.Request`](https://www.python-httpx.org/api/#request).
-         * timeout: The [timeouts](https://www.python-httpx.org/advanced/#timeout-configuration) linked to the request.
+         * ext: The extensions (including the [timeouts](https://www.python-httpx.org/advanced/#timeout-configuration)) linked to the request.
         
         If all callbacks are not executed during test execution, the test case will fail at teardown.
         
         This behavior can be disabled thanks to the `assert_all_responses_were_requested` fixture:
         
         ```python
         import pytest
@@ -362,15 +362,15 @@
         @pytest.fixture
         def assert_all_responses_were_requested() -> bool:
             return False
         ```
         
         ### Dynamic responses
         
-        Callback should return a httpcore response (as a tuple), you can use `pytest_httpx.to_response` function to create such a tuple.
+        Callback should return a `httpcore` response (as a tuple), you can use `pytest_httpx.to_response` function to create such a tuple.
         
         ```python
         import httpx
         from pytest_httpx import HTTPXMock, to_response
         
         
         def test_dynamic_response(httpx_mock: HTTPXMock):
@@ -396,16 +396,16 @@
         ```python
         import httpx
         import pytest
         from pytest_httpx import HTTPXMock
         
         
         def test_exception_raising(httpx_mock: HTTPXMock):
-            def raise_timeout(request, timeout):
-                raise httpx.ReadTimeout(f"Unable to read within {timeout}", request=request)
+            def raise_timeout(request, ext: dict):
+                raise httpx.ReadTimeout(f"Unable to read within {ext['timeout']}", request=request)
         
             httpx_mock.add_callback(raise_timeout)
             
             with httpx.Client() as client:
                 with pytest.raises(httpx.ReadTimeout):
                     client.get("http://test_url")
         
@@ -432,15 +432,15 @@
         
         In case all matching callbacks have been executed, the last one (according to the registration order) will be executed.
         
         You can add criteria so that callback will be sent only in case of a more specific matching.
         
         #### Matching on URL
         
-        `url` parameter can either be a string, a python [re.Pattern](https://docs.python.org/3/library/re.html) instance or a [httpx.URL](https://www.python-httpx.org/api/#url) instance.
+        `url` parameter can either be a string, a python [`re.Pattern`](https://docs.python.org/3/library/re.html) instance or a [`httpx.URL`](https://www.python-httpx.org/api/#url) instance.
         
         Matching is performed on the full URL, query parameters included.
         
         #### Matching on HTTP method
         
         Use `method` parameter to specify the HTTP method (POST, PUT, DELETE, PATCH, HEAD) executing the callback.
         
@@ -626,14 +626,15 @@
         | body (as bytes) | `body=b"sample"` | `data=b"sample"` |
         | body (as str) | `body="sample"` | `data="sample"` |
         | body (as JSON) | `payload=["sample"]` | `json=["sample"]` |
         | status code | `status=201` | `status_code=201` |
         
         Sample adding a response with `aioresponses`:
         ```python
+        import pytest
         from aioresponses import aioresponses
         
         
         @pytest.fixture
         def mock_aioresponse():
             with aioresponses() as m:
                 yield m
```

### Comparing `pytest_httpx-0.8.0/README.md` & `pytest_httpx-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
 ## Add callbacks
 
 You can perform custom manipulation upon request reception by registering callbacks.
 
 Callback should expect at least two parameters:
  * request: The received [`httpx.Request`](https://www.python-httpx.org/api/#request).
- * timeout: The [timeouts](https://www.python-httpx.org/advanced/#timeout-configuration) linked to the request.
+ * ext: The extensions (including the [timeouts](https://www.python-httpx.org/advanced/#timeout-configuration)) linked to the request.
 
 If all callbacks are not executed during test execution, the test case will fail at teardown.
 
 This behavior can be disabled thanks to the `assert_all_responses_were_requested` fixture:
 
 ```python
 import pytest
@@ -348,15 +348,15 @@
 @pytest.fixture
 def assert_all_responses_were_requested() -> bool:
     return False
 ```
 
 ### Dynamic responses
 
-Callback should return a httpcore response (as a tuple), you can use `pytest_httpx.to_response` function to create such a tuple.
+Callback should return a `httpcore` response (as a tuple), you can use `pytest_httpx.to_response` function to create such a tuple.
 
 ```python
 import httpx
 from pytest_httpx import HTTPXMock, to_response
 
 
 def test_dynamic_response(httpx_mock: HTTPXMock):
@@ -382,16 +382,16 @@
 ```python
 import httpx
 import pytest
 from pytest_httpx import HTTPXMock
 
 
 def test_exception_raising(httpx_mock: HTTPXMock):
-    def raise_timeout(request, timeout):
-        raise httpx.ReadTimeout(f"Unable to read within {timeout}", request=request)
+    def raise_timeout(request, ext: dict):
+        raise httpx.ReadTimeout(f"Unable to read within {ext['timeout']}", request=request)
 
     httpx_mock.add_callback(raise_timeout)
     
     with httpx.Client() as client:
         with pytest.raises(httpx.ReadTimeout):
             client.get("http://test_url")
 
@@ -418,15 +418,15 @@
 
 In case all matching callbacks have been executed, the last one (according to the registration order) will be executed.
 
 You can add criteria so that callback will be sent only in case of a more specific matching.
 
 #### Matching on URL
 
-`url` parameter can either be a string, a python [re.Pattern](https://docs.python.org/3/library/re.html) instance or a [httpx.URL](https://www.python-httpx.org/api/#url) instance.
+`url` parameter can either be a string, a python [`re.Pattern`](https://docs.python.org/3/library/re.html) instance or a [`httpx.URL`](https://www.python-httpx.org/api/#url) instance.
 
 Matching is performed on the full URL, query parameters included.
 
 #### Matching on HTTP method
 
 Use `method` parameter to specify the HTTP method (POST, PUT, DELETE, PATCH, HEAD) executing the callback.
 
@@ -612,14 +612,15 @@
 | body (as bytes) | `body=b"sample"` | `data=b"sample"` |
 | body (as str) | `body="sample"` | `data="sample"` |
 | body (as JSON) | `payload=["sample"]` | `json=["sample"]` |
 | status code | `status=201` | `status_code=201` |
 
 Sample adding a response with `aioresponses`:
 ```python
+import pytest
 from aioresponses import aioresponses
 
 
 @pytest.fixture
 def mock_aioresponse():
     with aioresponses() as m:
         yield m
```

### Comparing `pytest_httpx-0.8.0/pytest_httpx/_httpx_internals.py` & `pytest_httpx-0.9.0/pytest_httpx/_httpx_internals.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def stream(
     data, files, json: Any, boundary: bytes
 ) -> Union[httpcore.AsyncByteStream, httpcore.SyncByteStream]:
     if files:
         # TODO Get rid of this internal import
         # import is performed at runtime when needed to reduce impact of internal changes in httpx
-        from httpx._content_streams import MultipartStream
+        from httpx._multipart import MultipartStream
 
         return MultipartStream(data=data or {}, files=files, boundary=boundary)
 
     if json is not None:
         data = dumps(json).encode("utf-8")
     elif isinstance(data, str):
         data = data.encode("utf-8")
```

### Comparing `pytest_httpx-0.8.0/pytest_httpx/_httpx_mock.py` & `pytest_httpx-0.9.0/pytest_httpx/_httpx_mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Those types are internally defined within httpcore._types
 URL = Tuple[bytes, bytes, Optional[int], bytes]
 Headers = List[Tuple[bytes, bytes]]
 TimeoutDict = Dict[str, Optional[float]]
 
 Response = Tuple[
-    bytes, int, bytes, Headers, Union[httpcore.SyncByteStream, httpcore.AsyncByteStream]
+    int, Headers, Union[httpcore.SyncByteStream, httpcore.AsyncByteStream], dict
 ]
 
 
 def to_request(
     method: bytes,
     url: URL,
     headers: Headers = None,
@@ -149,15 +149,15 @@
     def add_callback(self, callback: Callable, **matchers):
         """
         Mock the action that will take place if a request match.
 
         :param callback: The callable that will be called upon reception of the matched request.
         It must expect at least 2 parameters:
          * request: The received httpx.Request.
-         * timeout: The timeout linked to the request.
+         * ext: The extensions linked to the request (such as timeout).
         It should return a valid httpcore response tuple, you can use pytest_httpx.to_response function to create one.
         :param url: Full URL identifying the request(s) to match.
         Can be a str, a re.Pattern instance or a httpx.URL instance.
         :param method: HTTP method identifying the request(s) to match.
         :param match_headers: HTTP headers identifying the request(s) to match. Must be a dictionary.
         :param match_content: Full HTTP body identifying the request(s) to match. Must be bytes.
         """
@@ -165,26 +165,26 @@
 
     def _handle_request(
         self,
         method: bytes,
         url: URL,
         headers: Headers = None,
         stream: Union[httpcore.SyncByteStream, httpcore.AsyncByteStream] = None,
-        timeout: TimeoutDict = None,
+        ext: dict = None,
     ) -> Response:
         request = to_request(method, url, headers, stream)
         self._requests.append(request)
 
         response = self._get_response(request)
         if response:
             return response
 
         callback = self._get_callback(request)
         if callback:
-            return callback(request=request, timeout=timeout)
+            return callback(request=request, ext=ext)
 
         raise httpx.TimeoutException(
             self._explain_that_no_response_was_found(request), request=request
         )
 
     def _explain_that_no_response_was_found(self, request: httpx.Request) -> str:
         expect_headers = set(
@@ -321,25 +321,25 @@
 
 class _PytestSyncTransport(httpcore.SyncHTTPTransport):
     def __init__(self, mock: HTTPXMock):
         self.mock = mock
 
     def request(
         self, *args, **kwargs
-    ) -> Tuple[bytes, int, bytes, List[Tuple[bytes, bytes]], httpcore.SyncByteStream]:
+    ) -> Tuple[int, List[Tuple[bytes, bytes]], httpcore.SyncByteStream, dict]:
         return self.mock._handle_request(*args, **kwargs)
 
 
 class _PytestAsyncTransport(httpcore.AsyncHTTPTransport):
     def __init__(self, mock: HTTPXMock):
         self.mock = mock
 
-    async def request(
+    async def arequest(
         self, *args, **kwargs
-    ) -> Tuple[bytes, int, bytes, List[Tuple[bytes, bytes]], httpcore.AsyncByteStream]:
+    ) -> Tuple[int, List[Tuple[bytes, bytes]], httpcore.AsyncByteStream, dict]:
         return self.mock._handle_request(*args, **kwargs)
 
 
 def to_response(
     status_code: int = 200,
     http_version: str = "HTTP/1.1",
     headers: dict = None,
@@ -362,8 +362,8 @@
     """
     headers = (
         [(header.encode(), value.encode()) for header, value in headers.items()]
         if headers
         else []
     )
     body = stream(data=data, files=files, json=json, boundary=boundary)
-    return http_version.encode(), status_code, b"", headers, body
+    return status_code, headers, body, {"http_version": http_version}
```

### Comparing `pytest_httpx-0.8.0/pytest_httpx/__init__.py` & `pytest_httpx-0.9.0/pytest_httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_httpx-0.8.0/setup.py` & `pytest_httpx-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "Topic :: Software Development :: Build Tools",
         "Topic :: Internet :: WWW/HTTP",
         "Framework :: Pytest",
     ],
     keywords=["pytest", "testing", "mock", "httpx"],
     packages=find_packages(exclude=["tests*"]),
     entry_points={"pytest11": ["pytest_httpx = pytest_httpx"]},
-    install_requires=["httpx==0.14.*", "pytest==6.*"],
+    install_requires=["httpx==0.15.*", "pytest==6.*"],
     extras_require={
         "testing": [
             # Used to run async test functions
             "pytest-asyncio==0.14.*",
             # Used to check coverage
             "pytest-cov==2.*",
         ]
```

