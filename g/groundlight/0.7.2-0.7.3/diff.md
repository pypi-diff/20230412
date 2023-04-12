# Comparing `tmp/groundlight-0.7.2.tar.gz` & `tmp/groundlight-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.7.2.tar", max compression
+gzip compressed data, was "groundlight-0.7.3.tar", max compression
```

## Comparing `groundlight-0.7.2.tar` & `groundlight-0.7.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1071 2023-04-03 00:14:28.174796 groundlight-0.7.2/LICENSE
--rw-r--r--   0        0        0     8186 2023-04-03 00:14:28.174796 groundlight-0.7.2/README.md
--rw-r--r--   0        0        0     3597 2023-04-03 00:14:28.174796 groundlight-0.7.2/generated/model.py
--rw-r--r--   0        0        0      723 2023-04-03 00:14:28.174796 groundlight-0.7.2/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-04-03 00:14:28.174796 groundlight-0.7.2/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14018 2023-04-03 00:14:28.174796 groundlight-0.7.2/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14322 2023-04-03 00:14:28.174796 groundlight-0.7.2/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35591 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      539 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17643 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     4979 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13623 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13486 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11288 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13847 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11330 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12129 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12150 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11438 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79719 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1009 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14005 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/openapi_client/rest.py
--rw-r--r--   0        0        0      955 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/setup.py
--rw-r--r--   0        0        0        0 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-04-03 00:14:28.178796 groundlight-0.7.2/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0      926 2023-04-03 00:14:28.178796 groundlight-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      537 2023-04-03 00:14:28.178796 groundlight-0.7.2/src/groundlight/__init__.py
--rw-r--r--   0        0        0     1685 2023-04-03 00:14:28.178796 groundlight-0.7.2/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0     9506 2023-04-03 00:14:28.178796 groundlight-0.7.2/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-04-03 00:14:28.178796 groundlight-0.7.2/src/groundlight/config.py
--rw-r--r--   0        0        0     2115 2023-04-03 00:14:28.178796 groundlight-0.7.2/src/groundlight/images.py
--rw-r--r--   0        0        0     4671 2023-04-03 00:14:28.178796 groundlight-0.7.2/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1564 2023-04-03 00:14:28.178796 groundlight-0.7.2/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0     9115 1970-01-01 00:00:00.000000 groundlight-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-12 16:14:00.431920 groundlight-0.7.3/LICENSE
+-rw-r--r--   0        0        0     1606 2023-04-12 16:14:00.431920 groundlight-0.7.3/README.md
+-rw-r--r--   0        0        0     3597 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/model.py
+-rw-r--r--   0        0        0      723 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14018 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14322 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35591 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      539 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17643 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     4979 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11870 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13623 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13486 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11288 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13847 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11330 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12129 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12150 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11438 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79719 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1009 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14005 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0      955 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-04-12 16:14:00.439920 groundlight-0.7.3/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0      926 2023-04-12 16:14:00.443920 groundlight-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      537 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     1685 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0     9506 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/config.py
+-rw-r--r--   0        0        0     2115 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/images.py
+-rw-r--r--   0        0        0     4671 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1564 2023-04-12 16:14:00.443920 groundlight-0.7.3/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 groundlight-0.7.3/PKG-INFO
```

### Comparing `groundlight-0.7.2/LICENSE` & `groundlight-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/model.py` & `groundlight-0.7.3/generated/model.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/__init__.py` & `groundlight-0.7.3/generated/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/api/detectors_api.py` & `groundlight-0.7.3/generated/openapi_client/api/detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.7.3/generated/openapi_client/api/image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/api_client.py` & `groundlight-0.7.3/generated/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/apis/__init__.py` & `groundlight-0.7.3/generated/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/configuration.py` & `groundlight-0.7.3/generated/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/exceptions.py` & `groundlight-0.7.3/generated/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/classification_result.py` & `groundlight-0.7.3/generated/openapi_client/model/classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/detector.py` & `groundlight-0.7.3/generated/openapi_client/model/detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.7.3/generated/openapi_client/model/detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.7.3/generated/openapi_client/model/detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/image_query.py` & `groundlight-0.7.3/generated/openapi_client/model/image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.7.3/generated/openapi_client/model/image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.7.3/generated/openapi_client/model/paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.7.3/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.7.3/generated/openapi_client/model/result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/model_utils.py` & `groundlight-0.7.3/generated/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/models/__init__.py` & `groundlight-0.7.3/generated/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/openapi_client/rest.py` & `groundlight-0.7.3/generated/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/setup.py` & `groundlight-0.7.3/generated/setup.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_classification_result.py` & `groundlight-0.7.3/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_detector.py` & `groundlight-0.7.3/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_detector_creation_input.py` & `groundlight-0.7.3/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_detector_type_enum.py` & `groundlight-0.7.3/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_detectors_api.py` & `groundlight-0.7.3/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_image_queries_api.py` & `groundlight-0.7.3/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_image_query.py` & `groundlight-0.7.3/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_image_query_type_enum.py` & `groundlight-0.7.3/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_paginated_detector_list.py` & `groundlight-0.7.3/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_paginated_image_query_list.py` & `groundlight-0.7.3/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/generated/test/test_result_type_enum.py` & `groundlight-0.7.3/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/pyproject.toml` & `groundlight-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "groundlight"
-version = "0.7.2"
+version = "0.7.3"
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.groundlight.ai"
 description = "Build computer vision systems from natural language with Groundlight"
 authors = ["Groundlight AI <support@groundlight.ai>"]
 packages = [
     { include = "**/*.py", from = "src" },
```

### Comparing `groundlight-0.7.2/src/groundlight/__init__.py` & `groundlight-0.7.3/src/groundlight/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/src/groundlight/binary_labels.py` & `groundlight-0.7.3/src/groundlight/binary_labels.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/src/groundlight/client.py` & `groundlight-0.7.3/src/groundlight/client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/src/groundlight/images.py` & `groundlight-0.7.3/src/groundlight/images.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/src/groundlight/internalapi.py` & `groundlight-0.7.3/src/groundlight/internalapi.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.2/src/groundlight/optional_imports.py` & `groundlight-0.7.3/src/groundlight/optional_imports.py`

 * *Files identical despite different names*

