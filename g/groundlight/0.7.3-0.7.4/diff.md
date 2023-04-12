# Comparing `tmp/groundlight-0.7.3.tar.gz` & `tmp/groundlight-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.7.3.tar", max compression
+gzip compressed data, was "groundlight-0.7.4.tar", max compression
```

## Comparing `groundlight-0.7.3.tar` & `groundlight-0.7.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1071 2023-04-12 16:14:00.431920 groundlight-0.7.3/LICENSE
--rw-r--r--   0        0        0     1606 2023-04-12 16:14:00.431920 groundlight-0.7.3/README.md
--rw-r--r--   0        0        0     3597 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/model.py
--rw-r--r--   0        0        0      723 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14018 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14322 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35591 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      539 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17643 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     4979 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13623 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13486 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11288 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13847 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11330 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12129 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12150 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11438 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79719 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1009 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14005 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/rest.py
--rw-r--r--   0        0        0      955 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/setup.py
--rw-r--r--   0        0        0        0 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0      926 2023-04-12 16:14:00.443920 groundlight-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      537 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/__init__.py
--rw-r--r--   0        0        0     1685 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0     9506 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/config.py
--rw-r--r--   0        0        0     2115 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/images.py
--rw-r--r--   0        0        0     4671 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1564 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 groundlight-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-12 20:20:27.404784 groundlight-0.7.4/LICENSE
+-rw-r--r--   0        0        0     1606 2023-04-12 20:20:27.404784 groundlight-0.7.4/README.md
+-rw-r--r--   0        0        0     3597 2023-04-12 20:20:27.408784 groundlight-0.7.4/generated/model.py
+-rw-r--r--   0        0        0      723 2023-04-12 20:20:27.408784 groundlight-0.7.4/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-12 20:20:27.408784 groundlight-0.7.4/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14018 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14322 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35591 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      539 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17643 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     4979 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11870 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13623 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13486 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11288 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13847 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11330 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12129 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12150 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11438 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79719 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1009 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14005 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0      955 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0      978 2023-04-12 20:20:27.412784 groundlight-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      537 2023-04-12 20:20:27.412784 groundlight-0.7.4/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     1685 2023-04-12 20:20:27.412784 groundlight-0.7.4/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0     9506 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/config.py
+-rw-r--r--   0        0        0     2115 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/images.py
+-rw-r--r--   0        0        0     4671 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1564 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0     2575 1970-01-01 00:00:00.000000 groundlight-0.7.4/PKG-INFO
```

### Comparing `groundlight-0.7.3/LICENSE` & `groundlight-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/README.md` & `groundlight-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/model.py` & `groundlight-0.7.4/generated/model.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/__init__.py` & `groundlight-0.7.4/generated/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/api/detectors_api.py` & `groundlight-0.7.4/generated/openapi_client/api/detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.7.4/generated/openapi_client/api/image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/api_client.py` & `groundlight-0.7.4/generated/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/apis/__init__.py` & `groundlight-0.7.4/generated/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/configuration.py` & `groundlight-0.7.4/generated/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/exceptions.py` & `groundlight-0.7.4/generated/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/classification_result.py` & `groundlight-0.7.4/generated/openapi_client/model/classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/detector.py` & `groundlight-0.7.4/generated/openapi_client/model/detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.7.4/generated/openapi_client/model/detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.7.4/generated/openapi_client/model/detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/image_query.py` & `groundlight-0.7.4/generated/openapi_client/model/image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.7.4/generated/openapi_client/model/image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.7.4/generated/openapi_client/model/paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.7.4/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.7.4/generated/openapi_client/model/result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/model_utils.py` & `groundlight-0.7.4/generated/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/models/__init__.py` & `groundlight-0.7.4/generated/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/openapi_client/rest.py` & `groundlight-0.7.4/generated/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/setup.py` & `groundlight-0.7.4/generated/setup.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_classification_result.py` & `groundlight-0.7.4/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_detector.py` & `groundlight-0.7.4/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_detector_creation_input.py` & `groundlight-0.7.4/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_detector_type_enum.py` & `groundlight-0.7.4/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_detectors_api.py` & `groundlight-0.7.4/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_image_queries_api.py` & `groundlight-0.7.4/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_image_query.py` & `groundlight-0.7.4/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_image_query_type_enum.py` & `groundlight-0.7.4/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_paginated_detector_list.py` & `groundlight-0.7.4/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_paginated_image_query_list.py` & `groundlight-0.7.4/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/generated/test/test_result_type_enum.py` & `groundlight-0.7.4/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/pyproject.toml` & `groundlight-0.7.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 [tool.poetry]
-name = "groundlight"
-version = "0.7.3"
-license = "MIT"
-readme = "README.md"
-homepage = "https://www.groundlight.ai"
-description = "Build computer vision systems from natural language with Groundlight"
 authors = ["Groundlight AI <support@groundlight.ai>"]
+description = "Build computer vision systems from natural language with Groundlight"
+homepage = "https://www.groundlight.ai"
+license = "MIT"
+name = "groundlight"
 packages = [
-    { include = "**/*.py", from = "src" },
-    { include = "**/*.py", from = "generated" },
+    {include = "**/*.py", from = "generated"},
+    {include = "**/*.py", from = "src"},
 ]
+readme = "README.md"
+version = "0.7.4"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<4.0"
-python-dateutil = "^2.8.2"
-urllib3 = "^1.26.9"
-frozendict = "^2.3.2"
 certifi = "^2021.10.8"
+frozendict = "^2.3.2"
+pillow = "^9.0.0"
 pydantic = "^1.7.4"
+python = ">=3.7.0,<4.0"
+python-dateutil = "^2.8.2"
 requests = "^2.28.2"
+urllib3 = "^1.26.9"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+autoflake = "^1.4"
 black = "^22.3.0"
-pytest-cov = "^3.0.0"
-pylint = "^2.13.9"
+datamodel-code-generator = "^0.12.1"
 flake8 = "^4.0.1"
+isort = "^5.10.1"
 mypy = "^0.950"
+pylint = "^2.13.9"
 pytest = "^7.0.1"
-isort = "^5.10.1"
-autoflake = "^1.4"
-datamodel-code-generator = "^0.12.1"
+pytest-cov = "^3.0.0"
+pytest-markdown-docs = "^0.4.3"
 pytest-mock = "^3.10.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.2.0"]
 
 [tool.black]
 line-length = 120
```

### Comparing `groundlight-0.7.3/src/groundlight/__init__.py` & `groundlight-0.7.4/src/groundlight/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/src/groundlight/binary_labels.py` & `groundlight-0.7.4/src/groundlight/binary_labels.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/src/groundlight/client.py` & `groundlight-0.7.4/src/groundlight/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             # Short-circuit
             return id
         obj = self.detectors_api.get_detector(id=id)
         return Detector.parse_obj(obj.to_dict())
 
     def get_detector_by_name(self, name: str) -> Optional[Detector]:
         # TODO: Do this on server.
-        detector_list = self.list_detectors(page_size=100)
+        detector_list = self.list_detectors(page_size=250)
         for d in detector_list.results:
             if d.name == name:
                 return d
         if detector_list.next:
             # TODO: paginate
             raise RuntimeError("You have too many detectors to use get_detector_by_name")
         return None
```

### Comparing `groundlight-0.7.3/src/groundlight/images.py` & `groundlight-0.7.4/src/groundlight/images.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/src/groundlight/internalapi.py` & `groundlight-0.7.4/src/groundlight/internalapi.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/src/groundlight/optional_imports.py` & `groundlight-0.7.4/src/groundlight/optional_imports.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.3/PKG-INFO` & `groundlight-0.7.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groundlight
-Version: 0.7.3
+Version: 0.7.4
 Summary: Build computer vision systems from natural language with Groundlight
 Home-page: https://www.groundlight.ai
 License: MIT
 Author: Groundlight AI
 Author-email: support@groundlight.ai
 Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=2021.10.8,<2022.0.0)
 Requires-Dist: frozendict (>=2.3.2,<3.0.0)
+Requires-Dist: pillow (>=9.0.0,<10.0.0)
 Requires-Dist: pydantic (>=1.7.4,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Groundlight Python SDK
```

