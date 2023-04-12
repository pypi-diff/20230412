# Comparing `tmp/arkindex-client-1.0.8.tar.gz` & `tmp/arkindex-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arkindex-client-1.0.8.tar", last modified: Thu Jan 27 08:08:51 2022, max compression
+gzip compressed data, was "dist/arkindex-client-1.0.9.tar", last modified: Tue May 17 15:19:17 2022, max compression
```

## Comparing `arkindex-client-1.0.8.tar` & `arkindex-client-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 08:08:51.000000 arkindex-client-1.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 08:08:51.000000 arkindex-client-1.0.8/arkindex/
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/arkindex/transports.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/arkindex/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       99 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/arkindex/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8556 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/arkindex/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/arkindex/mock.py
--rw-rw-rw-   0 root         (0) root         (0)     8165 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/arkindex/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/arkindex/auth.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      111 2022-01-27 08:08:51.000000 arkindex-client-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1352 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6080 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/README.rst
--rw-r--r--   0 root         (0) root         (0)     6904 2022-01-27 08:08:51.000000 arkindex-client-1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 08:08:51.000000 arkindex-client-1.0.8/arkindex_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-27 08:08:50.000000 arkindex-client-1.0.8/arkindex_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2022-01-27 08:08:50.000000 arkindex-client-1.0.8/arkindex_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     6904 2022-01-27 08:08:50.000000 arkindex-client-1.0.8/arkindex_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2022-01-27 08:08:50.000000 arkindex-client-1.0.8/arkindex_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-01-27 08:08:50.000000 arkindex-client-1.0.8/arkindex_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-01-27 08:01:04.000000 arkindex-client-1.0.8/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/arkindex/
+-rw-rw-rw-   0 root         (0) root         (0)      298 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/arkindex/transports.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/arkindex/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       99 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/arkindex/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8556 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/arkindex/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2762 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/arkindex/mock.py
+-rw-rw-rw-   0 root         (0) root         (0)     8165 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/arkindex/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/arkindex/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      111 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6080 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)     6904 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/arkindex_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/arkindex_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/arkindex_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     6904 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/arkindex_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/arkindex_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-05-17 15:19:17.000000 arkindex-client-1.0.9/arkindex_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        6 2022-05-17 15:17:49.000000 arkindex-client-1.0.9/VERSION
```

### Comparing `arkindex-client-1.0.8/arkindex/client.py` & `arkindex-client-1.0.9/arkindex/client.py`

 * *Files identical despite different names*

### Comparing `arkindex-client-1.0.8/arkindex/mock.py` & `arkindex-client-1.0.9/arkindex/mock.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,34 @@
         self, operation_id: str, response: dict, body=None, *args, **kwargs
     ):
         """Store a new mock response for a request on an endpoint"""
         request = MockRequest(operation_id, body, args, kwargs)
         self.responses.append((request, response))
         return (request, response)
 
+    def add_error_response(
+        self,
+        operation_id: str,
+        status_code: int,
+        title="Mock error response",
+        content="Mock error response",
+        body=None,
+        *args,
+        **kwargs,
+    ):
+        """Store a new mock error response for a request on an endpoint"""
+        request = MockRequest(operation_id, body, args, kwargs)
+        error = apistar.exceptions.ErrorResponse(
+            title=title,
+            status_code=status_code,
+            content=content,
+        )
+        self.responses.append((request, error))
+        return (request, error)
+
     def next_response(self, request: MockRequest):
         """Find the next available response for a request, and remove it from the stack"""
         for request_cmp, response in self.responses:
             if request_cmp == request:
                 self.responses.remove((request_cmp, response))
                 yield response
 
@@ -42,14 +62,16 @@
         request = MockRequest(operation_id, body, args, kwargs)
         self.history.append(request)
 
         # Find the next valid response
         response = next(self.next_response(request), None)
         if response is not None:
             logger.info(f"Sending mock response for {operation_id}")
+            if isinstance(response, Exception):
+                raise response
             return response
 
         # Throw exception when no response is found
         logger.error(
             f"No mock response found for {operation_id} with body={body} args={args} kwargs={kwargs}"
         )
         raise apistar.exceptions.ErrorResponse(
```

### Comparing `arkindex-client-1.0.8/arkindex/pagination.py` & `arkindex-client-1.0.9/arkindex/pagination.py`

 * *Files identical despite different names*

### Comparing `arkindex-client-1.0.8/arkindex/auth.py` & `arkindex-client-1.0.9/arkindex/auth.py`

 * *Files identical despite different names*

### Comparing `arkindex-client-1.0.8/setup.py` & `arkindex-client-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `arkindex-client-1.0.8/README.rst` & `arkindex-client-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `arkindex-client-1.0.8/PKG-INFO` & `arkindex-client-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: API client for the Arkindex project
 Home-page: https://gitlab.com/arkindex/api-client
 Author: Teklia <contact@teklia.com>
 License: MIT
 Keywords: api client arkindex
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arkindex-client-1.0.8/arkindex_client.egg-info/PKG-INFO` & `arkindex-client-1.0.9/arkindex_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: API client for the Arkindex project
 Home-page: https://gitlab.com/arkindex/api-client
 Author: Teklia <contact@teklia.com>
 License: MIT
 Keywords: api client arkindex
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

