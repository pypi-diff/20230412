# Comparing `tmp/openapify-0.3.2.tar.gz` & `tmp/openapify-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.2.tar", last modified: Wed Apr 12 11:49:54 2023, max compression
+gzip compressed data, was "openapify-0.3.3.tar", last modified: Wed Apr 12 18:57:10 2023, max compression
```

## Comparing `openapify-0.3.2.tar` & `openapify-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.547030 openapify-0.3.2/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.2/LICENSE
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30129 2023-04-12 11:49:54.546880 openapify-0.3.2/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29266 2023-04-11 22:14:24.000000 openapify-0.3.2/README.md
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.543689 openapify-0.3.2/openapify/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      282 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.545651 openapify-0.3.2/openapify/core/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    14772 2023-04-12 11:49:41.000000 openapify-0.3.2/openapify/core/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       92 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/const.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2002 2023-04-11 22:14:24.000000 openapify-0.3.2/openapify/core/document.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1630 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/jsonschema.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1748 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/models.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.546039 openapify-0.3.2/openapify/core/openapi/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/openapi/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5270 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/core/openapi/models.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5208 2023-04-11 22:14:24.000000 openapify-0.3.2/openapify/decorators.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.546335 openapify-0.3.2/openapify/ext/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/ext/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.546526 openapify-0.3.2/openapify/ext/web/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/ext/web/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.2/openapify/ext/web/aiohttp.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.2/openapify/py.typed
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-12 11:49:54.544514 openapify-0.3.2/openapify.egg-info/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30129 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.2/openapify.egg-info/not-zip-safe
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/requires.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-12 11:49:54.000000 openapify-0.3.2/openapify.egg-info/top_level.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.2/pyproject.toml
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-12 11:49:54.547066 openapify-0.3.2/setup.cfg
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-12 11:49:09.000000 openapify-0.3.2/setup.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.147448 openapify-0.3.3/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-04-11 15:10:01.000000 openapify-0.3.3/LICENSE
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-12 18:57:10.147319 openapify-0.3.3/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    29397 2023-04-12 18:43:50.000000 openapify-0.3.3/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.144357 openapify-0.3.3/openapify/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      488 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146237 openapify-0.3.3/openapify/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3.3/openapify/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    14809 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/core/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       92 2023-03-20 20:50:13.000000 openapify-0.3.3/openapify/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2018 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/core/document.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3.3/openapify/core/jsonschema.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3.3/openapify/core/models.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146533 openapify-0.3.3/openapify/core/openapi/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3.3/openapify/core/openapi/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5264 2023-04-12 18:44:38.000000 openapify-0.3.3/openapify/core/openapi/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5197 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/decorators.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146725 openapify-0.3.3/openapify/ext/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3.3/openapify/ext/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146899 openapify-0.3.3/openapify/ext/web/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3.3/openapify/ext/web/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3.3/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3.3/openapify/py.typed
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.145158 openapify-0.3.3/openapify.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      613 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3.3/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3.3/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-12 18:57:10.147487 openapify-0.3.3/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1298 2023-04-12 18:56:24.000000 openapify-0.3.3/setup.py
```

### Comparing `openapify-0.3.2/LICENSE` & `openapify-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openapify-0.3.2/PKG-INFO` & `openapify-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,12 @@
-Metadata-Version: 2.1
-Name: openapify
-Version: 0.3.2
-Summary: Framework agnostic OpenAPI Specification generation for code lovers
-Home-page: https://github.com/Fatal1ty/openapify
-Author: Alexander Tikhonov
-Author-email: random.gauss@gmail.com
-License: Apache License, Version 2.0
-Platform: all
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: aiohttp
-License-File: LICENSE
-
 # openapify
 
 ###### Framework agnostic OpenAPI Specification generation for code lovers
 
+[![Build Status](https://github.com/Fatal1ty/openapify/workflows/tests/badge.svg)](https://github.com/Fatal1ty/openapify/actions)
 [![Latest Version](https://img.shields.io/pypi/v/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![Python Version](https://img.shields.io/pypi/pyversions/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ---
 
 This library is designed for code-first people who don't want to bother diving
@@ -347,15 +325,15 @@
 
 Decorators
 --------------------------------------------------------------------------------
 
 Openapify has several decorators that embed necessary specific information for
 later use when building the OpenAPI document. In general, decorators will
 define the information that will be included in
-the [Operaion Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
+the [Operation Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
 which describes a single API operation on a path. We will look at what each
 decorator parameter is responsible for and how it is reflected in the final
 document.
 
 ### Generic operation info
 
 Decorator `path_docs` adds generic information about the Operation object,
```

### Comparing `openapify-0.3.2/README.md` & `openapify-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,35 @@
+Metadata-Version: 2.1
+Name: openapify
+Version: 0.3.3
+Summary: Framework agnostic OpenAPI Specification generation for code lovers
+Home-page: https://github.com/Fatal1ty/openapify
+Author: Alexander Tikhonov
+Author-email: random.gauss@gmail.com
+License: Apache License, Version 2.0
+Platform: all
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: aiohttp
+License-File: LICENSE
+
 # openapify
 
 ###### Framework agnostic OpenAPI Specification generation for code lovers
 
+[![Build Status](https://github.com/Fatal1ty/openapify/workflows/tests/badge.svg)](https://github.com/Fatal1ty/openapify/actions)
 [![Latest Version](https://img.shields.io/pypi/v/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![Python Version](https://img.shields.io/pypi/pyversions/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ---
 
 This library is designed for code-first people who don't want to bother diving
@@ -324,15 +348,15 @@
 
 Decorators
 --------------------------------------------------------------------------------
 
 Openapify has several decorators that embed necessary specific information for
 later use when building the OpenAPI document. In general, decorators will
 define the information that will be included in
-the [Operaion Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
+the [Operation Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
 which describes a single API operation on a path. We will look at what each
 decorator parameter is responsible for and how it is reflected in the final
 document.
 
 ### Generic operation info
 
 Decorator `path_docs` adds generic information about the Operation object,
```

### Comparing `openapify-0.3.2/openapify/core/builder.py` & `openapify-0.3.3/openapify/core/builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,15 +63,17 @@
         self,
         spec: Optional[apispec.APISpec] = None,
         title: str = DEFAULT_SPEC_TITLE,
         version: str = DEFAULT_SPEC_VERSION,
         openapi_version: str = DEFAULT_OPENAPI_VERSION,
         plugins: Sequence[apispec.BasePlugin] = (),
         servers: Optional[List[Union[str, openapi.Server]]] = None,
-        security_schemes: Optional[Dict[str, openapi.SecurityScheme]] = None,
+        security_schemes: Optional[
+            Mapping[str, openapi.SecurityScheme]
+        ] = None,
         **options: Any,
     ):
         if spec is None:
             spec = OpenAPIDocument(
                 title=title,
                 version=version,
                 openapi_version=openapi_version,
@@ -88,15 +90,15 @@
             key=lambda r: (r.path, METHOD_ORDER.index(r.method.lower())),
         ):
             self._process_route(route)
 
     def _process_route(self, route: RouteDef) -> None:
         method = route.method.lower()
         meta = getattr(route.handler, "__openapify__", [])
-        code_responses = {}
+        responses = openapi.Responses()
         summary = route.summary
         description = route.description
         tags = route.tags.copy() if route.tags else []
         deprecated = None
         external_docs = None
         security = None
         parameters = route.parameters.copy() if route.parameters else []
@@ -134,21 +136,15 @@
                 if headers:
                     parameters.extend(self._build_request_headers(headers))
                 cookies = args.get("cookies")
                 if cookies:
                     parameters.extend(self._build_cookies(cookies))
 
             elif args_type == "response":
-                args = args.copy()
-                http_code = args.pop("http_code")
-                body_value_type = args.pop("body")
-                if body_value_type is not None:
-                    code_responses[http_code] = self._build_response(
-                        body=body_value_type, **args
-                    )
+                self._update_responses(responses=responses, **args)
             elif args_type == "path_docs":
                 args = args.copy()
                 summary = args.get("summary")
                 description = args.get("description")
                 tags.extend(args.get("tags") or [])
                 # _merge_parameters(parameters, args.get("parameters") or {})
                 external_docs = self._build_external_docs(
@@ -162,15 +158,15 @@
         self.spec.path(
             route.path,
             operations={
                 method: openapi.Operation(
                     summary=summary,
                     description=description,
                     requestBody=request_body,
-                    responses=openapi.Responses(codes=code_responses),
+                    responses=responses,
                     deprecated=deprecated,
                     tags=tags or None,
                     parameters=parameters or None,
                     externalDocs=external_docs,
                     security=security,
                 ).to_dict()
             },
@@ -230,32 +226,30 @@
                     examples=self._build_examples(header.examples),
                 )
             )
         return result
 
     def _build_response_headers(
         self, headers: Dict[str, Union[str, Header]]
-    ) -> Sequence[openapi.Header]:
-        result = []
+    ) -> Mapping[str, openapi.Header]:
+        result = {}
         for name, header in headers.items():
             if not isinstance(header, Header):
                 header = Header(description=header)
             header_schema = build_json_schema(
                 header.value_type, self.spec, ComponentType.HEADER
             )
-            result.append(
-                openapi.Header(
-                    schema=header_schema,
-                    description=header.description,
-                    required=header.required,
-                    deprecated=header.deprecated,
-                    allowEmptyValue=header.allowEmptyValue,
-                    example=header.example,
-                    examples=self._build_examples(header.examples),
-                )
+            result[name] = openapi.Header(
+                schema=header_schema,
+                description=header.description,
+                required=header.required,
+                deprecated=header.deprecated,
+                allowEmptyValue=header.allowEmptyValue,
+                example=header.example,
+                examples=self._build_examples(header.examples),
             )
         return result
 
     def _build_cookies(
         self, cookies: Dict[str, Union[str, Cookie]]
     ) -> Sequence[openapi.Parameter]:
         result = []
@@ -297,37 +291,44 @@
                     example=example,
                     examples=self._build_examples(examples),
                 )
             },
             required=required,
         )
 
-    def _build_response(
+    def _update_responses(
         self,
-        body: Type,
+        responses: openapi.Responses,
+        http_code: openapi.HttpCode,
+        body: Optional[Type] = None,
         media_type: str = "application/json",
         description: Optional[str] = None,
         headers: Optional[Dict[str, Union[str, Header]]] = None,
         example: Optional[Any] = None,
         examples: Optional[Dict[str, Union[openapi.Example, Any]]] = None,
-    ) -> openapi.Response:
-        header_objects = {}
+    ) -> None:
+        http_code = str(http_code)
+        if responses.codes is None:
+            responses.codes = {}
+        response = responses.codes.get(http_code)
+        if not response:
+            response = openapi.Response()
+            responses.codes[http_code] = response
         if headers:
-            header_objects = self._build_response_headers(headers)
-        return openapi.Response(
-            description=description,
-            headers=header_objects or None,
-            content={
-                media_type: openapi.MediaType(
-                    schema=build_json_schema(body, self.spec),
-                    example=example,
-                    examples=self._build_examples(examples),
-                ),
-            },
-        )
+            response.headers = self._build_response_headers(headers)
+        if description:
+            response.description = description
+        if body is not None:
+            if response.content is None:
+                response.content = {}
+            response.content[media_type] = openapi.MediaType(
+                schema=build_json_schema(body, self.spec),
+                example=example,
+                examples=self._build_examples(examples),
+            )
 
     @staticmethod
     def _build_external_docs(
         data: Union[str, Tuple[str, str]]
     ) -> Optional[openapi.ExternalDocumentation]:
         if not data:
             return None
@@ -382,30 +383,30 @@
     routes: Iterable[RouteDef],
     *,
     title: str = DEFAULT_SPEC_TITLE,
     version: str = DEFAULT_SPEC_VERSION,
     openapi_version: str = DEFAULT_OPENAPI_VERSION,
     plugins: Sequence[apispec.BasePlugin] = (),
     servers: Optional[List[Union[str, openapi.Server]]] = None,
-    security_schemes: Optional[Dict[str, openapi.SecurityScheme]] = None,
+    security_schemes: Optional[Mapping[str, openapi.SecurityScheme]] = None,
     **options: Any,
 ) -> apispec.APISpec:
     ...
 
 
 def build_spec(
     routes: Iterable[RouteDef],
     spec: Optional[apispec.APISpec] = None,
     *,
     title: str = DEFAULT_SPEC_TITLE,
     version: str = DEFAULT_SPEC_VERSION,
     openapi_version: str = DEFAULT_OPENAPI_VERSION,
     plugins: Sequence[apispec.BasePlugin] = (),
     servers: Optional[List[Union[str, openapi.Server]]] = None,
-    security_schemes: Optional[Dict[str, openapi.SecurityScheme]] = None,
+    security_schemes: Optional[Mapping[str, openapi.SecurityScheme]] = None,
     **options: Any,
 ) -> apispec.APISpec:
     builder = OpenAPISpecBuilder(
         spec=spec,
         title=title,
         version=version,
         openapi_version=openapi_version,
```

### Comparing `openapify-0.3.2/openapify/core/document.py` & `openapify-0.3.3/openapify/core/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             **options,
         )
         if security_schemes:
             for name, scheme in security_schemes.items():
                 self.components.security_scheme(name, scheme.to_dict())
 
     def to_dict(self) -> Dict[str, Any]:
-        ret = {
+        ret: Dict[str, Any] = {
             "openapi": str(self.openapi_version),
             "info": {"title": self.title, "version": self.version},
         }
         servers = self.options.pop("servers", None)
         if servers:
             ret["servers"] = servers
         ret["paths"] = self._paths
```

### Comparing `openapify-0.3.2/openapify/core/jsonschema.py` & `openapify-0.3.3/openapify/core/jsonschema.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.2/openapify/core/models.py` & `openapify-0.3.3/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.2/openapify/core/openapi/models.py` & `openapify-0.3.3/openapify/core/openapi/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, List, Literal, Mapping, Optional, Union
+from typing import Any, Dict, List, Mapping, Optional, Union
 
 from mashumaro import DataClassDictMixin
 from mashumaro.config import BaseConfig
-from typing_extensions import TypeAlias
+from typing_extensions import Literal, TypeAlias
 
 HttpCode: TypeAlias = Union[str, int]
 Schema: TypeAlias = Mapping[str, Any]
 
 
 @dataclass
 class Object(DataClassDictMixin):
@@ -63,21 +63,21 @@
     required: Optional[bool] = None
 
 
 @dataclass
 class Response(Object):
     description: Optional[str] = None
     headers: Optional[Mapping[str, Header]] = None
-    content: Optional[Mapping[str, MediaType]] = None
+    content: Optional[Dict[str, MediaType]] = None
 
 
 @dataclass
 class Responses(Object):
     default: Optional[Response] = None
-    codes: Optional[Mapping[HttpCode, Response]] = None
+    codes: Optional[Dict[HttpCode, Response]] = None
 
     def __post_serialize__(self, d: Dict[Any, Any]) -> Dict[Any, Any]:
         codes = d.pop("codes", None)
         if codes:
             d.update(codes)
         return d
```

### Comparing `openapify-0.3.2/openapify/decorators.py` & `openapify-0.3.3/openapify/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from openapify.core.models import (
     Body,
     Cookie,
     Header,
     QueryParam,
     SecurityRequirement,
 )
-from openapify.core.openapi.models import Example, HttpCode, Parameter
+from openapify.core.openapi.models import Example, HttpCode
 
 __openapify__ = "__openapify__"
 
 
 Handler = TypeVar("Handler")
```

### Comparing `openapify-0.3.2/openapify/ext/web/aiohttp.py` & `openapify-0.3.3/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.2/openapify.egg-info/PKG-INFO` & `openapify-0.3.3/openapify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.2
+Version: 0.3.3
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,14 +21,15 @@
 Provides-Extra: aiohttp
 License-File: LICENSE
 
 # openapify
 
 ###### Framework agnostic OpenAPI Specification generation for code lovers
 
+[![Build Status](https://github.com/Fatal1ty/openapify/workflows/tests/badge.svg)](https://github.com/Fatal1ty/openapify/actions)
 [![Latest Version](https://img.shields.io/pypi/v/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![Python Version](https://img.shields.io/pypi/pyversions/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ---
 
 This library is designed for code-first people who don't want to bother diving
@@ -347,15 +348,15 @@
 
 Decorators
 --------------------------------------------------------------------------------
 
 Openapify has several decorators that embed necessary specific information for
 later use when building the OpenAPI document. In general, decorators will
 define the information that will be included in
-the [Operaion Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
+the [Operation Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
 which describes a single API operation on a path. We will look at what each
 decorator parameter is responsible for and how it is reflected in the final
 document.
 
 ### Generic operation info
 
 Decorator `path_docs` adds generic information about the Operation object,
```

### Comparing `openapify-0.3.2/openapify.egg-info/SOURCES.txt` & `openapify-0.3.3/openapify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapify-0.3.2/setup.py` & `openapify-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.3.2",
+    version="0.3.3",
     description=(
         "Framework agnostic OpenAPI Specification generation for code lovers"
     ),
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
```

