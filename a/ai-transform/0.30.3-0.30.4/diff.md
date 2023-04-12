# Comparing `tmp/ai_transform-0.30.3.tar.gz` & `tmp/ai_transform-0.30.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.30.3.tar", last modified: Tue Apr 11 03:15:14 2023, max compression
+gzip compressed data, was "ai_transform-0.30.4.tar", last modified: Wed Apr 12 06:58:56 2023, max compression
```

## Comparing `ai_transform-0.30.3.tar` & `ai_transform-0.30.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-11 03:14:57.000000 ai_transform-0.30.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 03:15:14.023920 ai_transform-0.30.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-11 03:14:57.000000 ai_transform-0.30.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32153 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 03:15:14.023920 ai_transform-0.30.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-11 03:14:57.000000 ai_transform-0.30.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-12 06:58:38.000000 ai_transform-0.30.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 06:58:56.312854 ai_transform-0.30.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-12 06:58:38.000000 ai_transform-0.30.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.292854 ai_transform-0.30.4/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.296854 ai_transform-0.30.4/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32516 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.296854 ai_transform-0.30.4/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.300854 ai_transform-0.30.4/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.300854 ai_transform-0.30.4/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.300854 ai_transform-0.30.4/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.304854 ai_transform-0.30.4/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.304854 ai_transform-0.30.4/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.296854 ai_transform-0.30.4/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:58:56.312854 ai_transform-0.30.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-12 06:58:38.000000 ai_transform-0.30.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.30.3/LICENSE` & `ai_transform-0.30.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/README.md` & `ai_transform-0.30.4/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/__init__.py` & `ai_transform-0.30.4/ai_transform/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.30.3"
+__version__ = "0.30.4"
 
 from ai_transform.timer import Timer
 
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.30.3/ai_transform/api/api.py` & `ai_transform-0.30.4/ai_transform/api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,27 @@
                 is_random=is_random,
                 after_id=[] if after_id is None else after_id,
                 worker_number=worker_number,
             ),
         )
         return get_response(response)
 
+    def _delete_where(
+        self,
+        dataset_id: str,
+        filters: Optional[List[Filter]] = None,
+    ):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/documents/delete_where",
+            json=dict(
+                filters=[] if filters is None else filters,
+            ),
+        )
+        return get_response(response)
+
     def _update_dataset_metadata(self, dataset_id: str, metadata: Dict[str, Any]):
         """
         Edit and add metadata about a dataset. Notably description, data source, etc
         """
         response = self.post(
             suffix=f"/datasets/{dataset_id}/metadata",
             json=dict(dataset_id=dataset_id, metadata=metadata),
```

### Comparing `ai_transform-0.30.3/ai_transform/api/client.py` & `ai_transform-0.30.4/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/api/helpers.py` & `ai_transform-0.30.4/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/api/wrappers.py` & `ai_transform-0.30.4/ai_transform/api/wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/components/components.py` & `ai_transform-0.30.4/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/config.py` & `ai_transform-0.30.4/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/dataset/dataset.py` & `ai_transform-0.30.4/ai_transform/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,18 @@
             is_random=is_random,
             after_id=after_id,
             worker_number=worker_number,
         )
         res["documents"] = DocumentList(res["documents"])
         return res
 
+    def delete_documents(self, filters: Optional[List[Filter]]) -> Dict[str, Any]:
+        res = self.api._delete_where(dataset_id=self._dataset_id, filters=filters)
+        return res
+
     def get_all_documents(
         self,
         page_size: int = 64,
         filters: Optional[List[Filter]] = None,
         select_fields: Optional[List[str]] = None,
         sort: Optional[list] = None,
         include_vector: bool = True,
```

### Comparing `ai_transform-0.30.3/ai_transform/dataset/field.py` & `ai_transform-0.30.4/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/engine/abstract_engine.py` & `ai_transform-0.30.4/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.30.4/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.30.4/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/engine/multipass_engine.py` & `ai_transform-0.30.4/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.30.4/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/engine/stable_engine.py` & `ai_transform-0.30.4/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/errors.py` & `ai_transform-0.30.4/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/logger.py` & `ai_transform-0.30.4/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/operator/abstract_operator.py` & `ai_transform-0.30.4/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/operator/dense_operator.py` & `ai_transform-0.30.4/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/timer.py` & `ai_transform-0.30.4/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/types.py` & `ai_transform-0.30.4/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/utils/document.py` & `ai_transform-0.30.4/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/utils/document_list.py` & `ai_transform-0.30.4/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/utils/example_documents.py` & `ai_transform-0.30.4/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/utils/json_encoder.py` & `ai_transform-0.30.4/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/utils/keyphrase.py` & `ai_transform-0.30.4/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.30.4/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/workflow/context_manager.py` & `ai_transform-0.30.4/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform/workflow/helpers.py` & `ai_transform-0.30.4/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.30.4/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/setup.py` & `ai_transform-0.30.4/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/conftest.py` & `ai_transform-0.30.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_api/test_endpoints.py` & `ai_transform-0.30.4/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.30.4/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_api/test_wrappers.py` & `ai_transform-0.30.4/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.30.4/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_dataset/test_field.py` & `ai_transform-0.30.4/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.30.4/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.30.4/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_engine/test_engine.py` & `ai_transform-0.30.4/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.30.4/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.30.4/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.30.4/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.30.4/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.30.4/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.30.4/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.3/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.30.4/tests/core/test_workflow/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,17 @@
             additional_information=config.additional_information,
             send_email=config.send_email,
         ):
             x += 1
         assert x == 1
 
     def test_simple_workflow(self, test_client: Client):
-        simple_workflow_dataset = test_client.Dataset("test-simple-workflow-dataset")
+        simple_workflow_dataset = test_client.Dataset(
+            "test-simple-workflow-dataset", expire=True
+        )
         simple_workflow_dataset.insert_documents([{"_id": "0", "value": 0}])
 
         workflow_name = "Simple Workflow"
         time_sleep_value = 10
 
         with test_client.SimpleWorkflow(
             workflow_name=workflow_name,
```

