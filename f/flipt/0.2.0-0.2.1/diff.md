# Comparing `tmp/flipt-0.2.0.tar.gz` & `tmp/flipt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipt-0.2.0.tar", max compression
+gzip compressed data, was "flipt-0.2.1.tar", max compression
```

## Comparing `flipt-0.2.0.tar` & `flipt-0.2.1.tar`

### file list

```diff
@@ -1,82 +1,89 @@
--rw-r--r--   0        0        0      407 2023-04-12 13:44:28.669415 flipt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2263 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/__init__.py
--rw-r--r--   0        0        0     2197 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/client.py
--rw-r--r--   0        0        0      348 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/core/__init__.py
--rw-r--r--   0        0        0      326 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/core/remove_none_from_headers.py
--rw-r--r--   0        0        0     2284 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/__init__.py
--rw-r--r--   0        0        0      261 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth/__init__.py
--rw-r--r--   0        0        0     8839 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth/client.py
--rw-r--r--   0        0        0      369 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth/types/__init__.py
--rw-r--r--   0        0        0     1128 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth/types/authentication.py
--rw-r--r--   0        0        0      943 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth/types/authentication_list.py
--rw-r--r--   0        0        0      988 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth/types/authentication_method.py
--rw-r--r--   0        0        0     1023 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth/types/authentication_token.py
--rw-r--r--   0        0        0       65 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_k_8_s/__init__.py
--rw-r--r--   0        0        0     2838 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_k_8_s/client.py
--rw-r--r--   0        0        0      195 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/__init__.py
--rw-r--r--   0        0        0     4596 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/client.py
--rw-r--r--   0        0        0      252 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/types/__init__.py
--rw-r--r--   0        0        0      854 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/types/oidc_authorize_url_response.py
--rw-r--r--   0        0        0      931 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/types/oidc_callback_response.py
--rw-r--r--   0        0        0       65 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_token/__init__.py
--rw-r--r--   0        0        0     2974 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/auth_method_token/client.py
--rw-r--r--   0        0        0      117 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/commons/__init__.py
--rw-r--r--   0        0        0      120 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      933 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/commons/types/pageable.py
--rw-r--r--   0        0        0      279 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/constraints/__init__.py
--rw-r--r--   0        0        0     6650 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/constraints/client.py
--rw-r--r--   0        0        0      399 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/constraints/types/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint.py
--rw-r--r--   0        0        0     1215 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint_comparison_type.py
--rw-r--r--   0        0        0      913 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint_create_request.py
--rw-r--r--   0        0        0      913 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint_update_request.py
--rw-r--r--   0        0        0      237 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/distributions/__init__.py
--rw-r--r--   0        0        0     7185 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/distributions/client.py
--rw-r--r--   0        0        0      324 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/distributions/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/distributions/types/distribution.py
--rw-r--r--   0        0        0      868 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/distributions/types/distribution_create_request.py
--rw-r--r--   0        0        0      868 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/distributions/types/distribution_update_request.py
--rw-r--r--   0        0        0      365 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/__init__.py
--rw-r--r--   0        0        0     4879 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/client.py
--rw-r--r--   0        0        0      490 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/types/batch_evaluation_request.py
--rw-r--r--   0        0        0     1028 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/types/batch_evaluation_response.py
--rw-r--r--   0        0        0     1446 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/types/evaluation_reason.py
--rw-r--r--   0        0        0      999 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/types/evaluation_request.py
--rw-r--r--   0        0        0     1328 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/evaluate/types/evaluation_response.py
--rw-r--r--   0        0        0      211 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/flags/__init__.py
--rw-r--r--   0        0        0     9921 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/flags/client.py
--rw-r--r--   0        0        0      296 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/flags/types/__init__.py
--rw-r--r--   0        0        0     1047 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/flags/types/flag.py
--rw-r--r--   0        0        0      839 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/flags/types/flag_create_request.py
--rw-r--r--   0        0        0      951 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/flags/types/flag_list.py
--rw-r--r--   0        0        0      826 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/flags/types/flag_update_request.py
--rw-r--r--   0        0        0      249 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/__init__.py
--rw-r--r--   0        0        0    12303 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/client.py
--rw-r--r--   0        0        0      365 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1142 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/types/rule.py
--rw-r--r--   0        0        0      857 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/types/rule_create_request.py
--rw-r--r--   0        0        0      951 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/types/rule_list.py
--rw-r--r--   0        0        0      849 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/types/rule_order_request.py
--rw-r--r--   0        0        0      843 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/rules/types/rule_update_request.py
--rw-r--r--   0        0        0      273 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/__init__.py
--rw-r--r--   0        0        0    10155 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/client.py
--rw-r--r--   0        0        0      401 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/types/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/types/segment.py
--rw-r--r--   0        0        0      954 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/types/segment_create_request.py
--rw-r--r--   0        0        0      966 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/types/segment_list.py
--rw-r--r--   0        0        0      566 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/types/segment_match_type.py
--rw-r--r--   0        0        0      941 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/segments/types/segment_update_request.py
--rw-r--r--   0        0        0      207 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/variants/__init__.py
--rw-r--r--   0        0        0     6569 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/variants/client.py
--rw-r--r--   0        0        0      279 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/variants/types/__init__.py
--rw-r--r--   0        0        0     1035 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/variants/types/variant.py
--rw-r--r--   0        0        0      861 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/variants/types/variant_create_request.py
--rw-r--r--   0        0        0      861 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/api/resources/variants/types/variant_update_request.py
--rw-r--r--   0        0        0      158 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/environment.py
--rw-r--r--   0        0        0        0 2023-04-12 13:44:28.669415 flipt-0.2.0/src/flipt/py.typed
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 flipt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      407 2023-04-12 16:29:59.886289 flipt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2485 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/__init__.py
+-rw-r--r--   0        0        0     2419 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/__init__.py
+-rw-r--r--   0        0        0     5308 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/client.py
+-rw-r--r--   0        0        0      348 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0     2513 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/__init__.py
+-rw-r--r--   0        0        0      261 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/__init__.py
+-rw-r--r--   0        0        0     8839 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/client.py
+-rw-r--r--   0        0        0      369 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/__init__.py
+-rw-r--r--   0        0        0     1128 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication.py
+-rw-r--r--   0        0        0      943 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_list.py
+-rw-r--r--   0        0        0      988 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_method.py
+-rw-r--r--   0        0        0     1023 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_token.py
+-rw-r--r--   0        0        0       65 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_k_8_s/__init__.py
+-rw-r--r--   0        0        0     2838 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_k_8_s/client.py
+-rw-r--r--   0        0        0      195 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/__init__.py
+-rw-r--r--   0        0        0     4596 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/client.py
+-rw-r--r--   0        0        0      252 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_authorize_url_response.py
+-rw-r--r--   0        0        0      931 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_callback_response.py
+-rw-r--r--   0        0        0       65 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_token/__init__.py
+-rw-r--r--   0        0        0     2974 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_token/client.py
+-rw-r--r--   0        0        0      117 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/commons/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      933 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/commons/types/pageable.py
+-rw-r--r--   0        0        0      279 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/__init__.py
+-rw-r--r--   0        0        0     6650 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/client.py
+-rw-r--r--   0        0        0      399 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/__init__.py
+-rw-r--r--   0        0        0     1127 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint.py
+-rw-r--r--   0        0        0     1215 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_comparison_type.py
+-rw-r--r--   0        0        0      913 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_create_request.py
+-rw-r--r--   0        0        0      913 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_update_request.py
+-rw-r--r--   0        0        0      237 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/__init__.py
+-rw-r--r--   0        0        0     7185 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/client.py
+-rw-r--r--   0        0        0      324 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution.py
+-rw-r--r--   0        0        0      868 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_create_request.py
+-rw-r--r--   0        0        0      868 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_update_request.py
+-rw-r--r--   0        0        0      365 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/__init__.py
+-rw-r--r--   0        0        0     4879 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/client.py
+-rw-r--r--   0        0        0      490 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_request.py
+-rw-r--r--   0        0        0     1028 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_response.py
+-rw-r--r--   0        0        0     1446 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_reason.py
+-rw-r--r--   0        0        0      999 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_request.py
+-rw-r--r--   0        0        0     1328 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_response.py
+-rw-r--r--   0        0        0      211 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/__init__.py
+-rw-r--r--   0        0        0     9921 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/client.py
+-rw-r--r--   0        0        0      296 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/__init__.py
+-rw-r--r--   0        0        0     1047 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag.py
+-rw-r--r--   0        0        0      839 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag_create_request.py
+-rw-r--r--   0        0        0      951 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag_list.py
+-rw-r--r--   0        0        0      826 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag_update_request.py
+-rw-r--r--   0        0        0      251 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/__init__.py
+-rw-r--r--   0        0        0     9631 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/client.py
+-rw-r--r--   0        0        0      356 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/__init__.py
+-rw-r--r--   0        0        0      973 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace.py
+-rw-r--r--   0        0        0      809 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_create_request.py
+-rw-r--r--   0        0        0      976 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_list.py
+-rw-r--r--   0        0        0      796 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_update_request.py
+-rw-r--r--   0        0        0      249 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/__init__.py
+-rw-r--r--   0        0        0    12303 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/client.py
+-rw-r--r--   0        0        0      365 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1142 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule.py
+-rw-r--r--   0        0        0      857 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_create_request.py
+-rw-r--r--   0        0        0      951 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_list.py
+-rw-r--r--   0        0        0      849 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_order_request.py
+-rw-r--r--   0        0        0      843 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_update_request.py
+-rw-r--r--   0        0        0      273 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/__init__.py
+-rw-r--r--   0        0        0    10155 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/client.py
+-rw-r--r--   0        0        0      401 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/__init__.py
+-rw-r--r--   0        0        0     1165 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment.py
+-rw-r--r--   0        0        0      954 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_create_request.py
+-rw-r--r--   0        0        0      966 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_list.py
+-rw-r--r--   0        0        0      566 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_match_type.py
+-rw-r--r--   0        0        0      941 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_update_request.py
+-rw-r--r--   0        0        0      207 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/__init__.py
+-rw-r--r--   0        0        0     6569 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/client.py
+-rw-r--r--   0        0        0      279 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/__init__.py
+-rw-r--r--   0        0        0     1035 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/variant.py
+-rw-r--r--   0        0        0      861 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/variant_create_request.py
+-rw-r--r--   0        0        0      861 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/variant_update_request.py
+-rw-r--r--   0        0        0      158 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/environment.py
+-rw-r--r--   0        0        0        0 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/py.typed
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 flipt-0.2.1/PKG-INFO
```

### Comparing `flipt-0.2.0/src/flipt/__init__.py` & `flipt-0.2.1/src/flipt/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     evaluationRequest,
     evaluationResponse,
     flag,
     flagCreateRequest,
     flagList,
     flags,
     flagUpdateRequest,
+    namespace,
+    namespaceCreateRequest,
+    namespaceList,
+    namespaces,
+    namespaceUpdateRequest,
     oidcAuthorizeURLResponse,
     oidcCallbackResponse,
     rule,
     ruleCreateRequest,
     ruleList,
     ruleOrderRequest,
     rules,
@@ -80,14 +85,19 @@
     "evaluationRequest",
     "evaluationResponse",
     "flag",
     "flagCreateRequest",
     "flagList",
     "flagUpdateRequest",
     "flags",
+    "namespace",
+    "namespaceCreateRequest",
+    "namespaceList",
+    "namespaceUpdateRequest",
+    "namespaces",
     "oidcAuthorizeURLResponse",
     "oidcCallbackResponse",
     "rule",
     "ruleCreateRequest",
     "ruleList",
     "ruleOrderRequest",
     "ruleUpdateRequest",
```

### Comparing `flipt-0.2.0/src/flipt/api/__init__.py` & `flipt-0.2.1/src/flipt/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     evaluationRequest,
     evaluationResponse,
     flag,
     flagCreateRequest,
     flagList,
     flags,
     flagUpdateRequest,
+    namespace,
+    namespaceCreateRequest,
+    namespaceList,
+    namespaces,
+    namespaceUpdateRequest,
     oidcAuthorizeURLResponse,
     oidcCallbackResponse,
     rule,
     ruleCreateRequest,
     ruleList,
     ruleOrderRequest,
     rules,
@@ -78,14 +83,19 @@
     "evaluationRequest",
     "evaluationResponse",
     "flag",
     "flagCreateRequest",
     "flagList",
     "flagUpdateRequest",
     "flags",
+    "namespace",
+    "namespaceCreateRequest",
+    "namespaceList",
+    "namespaceUpdateRequest",
+    "namespaces",
     "oidcAuthorizeURLResponse",
     "oidcCallbackResponse",
     "rule",
     "ruleCreateRequest",
     "ruleList",
     "ruleOrderRequest",
     "ruleUpdateRequest",
```

### Comparing `flipt-0.2.0/src/flipt/api/client.py` & `flipt-0.2.1/src/flipt/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .resources.auth_method_k_8_s.client import AsyncAuthMethodK8SClient, AuthMethodK8SClient
 from .resources.auth_method_oidc.client import AsyncAuthMethodOidcClient, AuthMethodOidcClient
 from .resources.auth_method_token.client import AsyncAuthMethodTokenClient, AuthMethodTokenClient
 from .resources.constraints.client import AsyncConstraintsClient, ConstraintsClient
 from .resources.distributions.client import AsyncDistributionsClient, DistributionsClient
 from .resources.evaluate.client import AsyncEvaluateClient, EvaluateClient
 from .resources.flags.client import AsyncFlagsClient, FlagsClient
+from .resources.namespaces.client import AsyncNamespacesClient, NamespacesClient
 from .resources.rules.client import AsyncRulesClient, RulesClient
 from .resources.segments.client import AsyncSegmentsClient, SegmentsClient
 from .resources.variants.client import AsyncVariantsClient, VariantsClient
 
 
 class FliptApi:
     def __init__(
@@ -54,14 +55,18 @@
         return EvaluateClient(environment=self._environment, token=self._token)
 
     @cached_property
     def flags(self) -> FlagsClient:
         return FlagsClient(environment=self._environment, token=self._token)
 
     @cached_property
+    def namespaces(self) -> NamespacesClient:
+        return NamespacesClient(environment=self._environment, token=self._token)
+
+    @cached_property
     def rules(self) -> RulesClient:
         return RulesClient(environment=self._environment, token=self._token)
 
     @cached_property
     def segments(self) -> SegmentsClient:
         return SegmentsClient(environment=self._environment, token=self._token)
 
@@ -106,14 +111,18 @@
         return AsyncEvaluateClient(environment=self._environment, token=self._token)
 
     @cached_property
     def flags(self) -> AsyncFlagsClient:
         return AsyncFlagsClient(environment=self._environment, token=self._token)
 
     @cached_property
+    def namespaces(self) -> AsyncNamespacesClient:
+        return AsyncNamespacesClient(environment=self._environment, token=self._token)
+
+    @cached_property
     def rules(self) -> AsyncRulesClient:
         return AsyncRulesClient(environment=self._environment, token=self._token)
 
     @cached_property
     def segments(self) -> AsyncSegmentsClient:
         return AsyncSegmentsClient(environment=self._environment, token=self._token)
```

### Comparing `flipt-0.2.0/src/flipt/api/core/datetime_utils.py` & `flipt-0.2.1/src/flipt/api/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/core/jsonable_encoder.py` & `flipt-0.2.1/src/flipt/api/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/__init__.py` & `flipt-0.2.1/src/flipt/api/resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     auth_method_oidc,
     auth_method_token,
     commons,
     constraints,
     distributions,
     evaluate,
     flags,
+    namespaces,
     rules,
     segments,
     variants,
 )
 from .auth import authentication, authenticationList, authenticationMethod, authenticationToken
 from .auth_method_oidc import oidcAuthorizeURLResponse, oidcCallbackResponse
 from .commons import Pageable
@@ -23,14 +24,15 @@
     batchEvaluationRequest,
     batchEvaluationResponse,
     evaluationReason,
     evaluationRequest,
     evaluationResponse,
 )
 from .flags import flag, flagCreateRequest, flagList, flagUpdateRequest
+from .namespaces import namespace, namespaceCreateRequest, namespaceList, namespaceUpdateRequest
 from .rules import rule, ruleCreateRequest, ruleList, ruleOrderRequest, ruleUpdateRequest
 from .segments import segment, segmentCreateRequest, segmentList, segmentMatchType, segmentUpdateRequest
 from .variants import variant, variantCreateRequest, variantUpdateRequest
 
 __all__ = [
     "Pageable",
     "auth",
@@ -58,14 +60,19 @@
     "evaluationRequest",
     "evaluationResponse",
     "flag",
     "flagCreateRequest",
     "flagList",
     "flagUpdateRequest",
     "flags",
+    "namespace",
+    "namespaceCreateRequest",
+    "namespaceList",
+    "namespaceUpdateRequest",
+    "namespaces",
     "oidcAuthorizeURLResponse",
     "oidcCallbackResponse",
     "rule",
     "ruleCreateRequest",
     "ruleList",
     "ruleOrderRequest",
     "ruleUpdateRequest",
```

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth/client.py` & `flipt-0.2.1/src/flipt/api/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth/types/authentication.py` & `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth/types/authentication_list.py` & `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth/types/authentication_method.py` & `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_method.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth/types/authentication_token.py` & `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_token.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth_method_k_8_s/client.py` & `flipt-0.2.1/src/flipt/api/resources/auth_method_k_8_s/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/client.py` & `flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/types/oidc_authorize_url_response.py` & `flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_authorize_url_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth_method_oidc/types/oidc_callback_response.py` & `flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_callback_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/auth_method_token/client.py` & `flipt-0.2.1/src/flipt/api/resources/auth_method_token/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/commons/types/pageable.py` & `flipt-0.2.1/src/flipt/api/resources/commons/types/pageable.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/constraints/client.py` & `flipt-0.2.1/src/flipt/api/resources/constraints/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint.py` & `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint_comparison_type.py` & `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_comparison_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint_create_request.py` & `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/constraints/types/constraint_update_request.py` & `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/distributions/client.py` & `flipt-0.2.1/src/flipt/api/resources/distributions/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/distributions/types/distribution.py` & `flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/distributions/types/distribution_create_request.py` & `flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/distributions/types/distribution_update_request.py` & `flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/evaluate/client.py` & `flipt-0.2.1/src/flipt/api/resources/evaluate/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/evaluate/types/batch_evaluation_request.py` & `flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/evaluate/types/batch_evaluation_response.py` & `flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/evaluate/types/evaluation_reason.py` & `flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_reason.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/evaluate/types/evaluation_request.py` & `flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/evaluate/types/evaluation_response.py` & `flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/flags/client.py` & `flipt-0.2.1/src/flipt/api/resources/flags/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/flags/types/flag.py` & `flipt-0.2.1/src/flipt/api/resources/flags/types/flag.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/flags/types/flag_create_request.py` & `flipt-0.2.1/src/flipt/api/resources/flags/types/flag_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/flags/types/flag_list.py` & `flipt-0.2.1/src/flipt/api/resources/flags/types/flag_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/flags/types/flag_update_request.py` & `flipt-0.2.1/src/flipt/api/resources/flags/types/flag_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/rules/client.py` & `flipt-0.2.1/src/flipt/api/resources/rules/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/rules/types/rule.py` & `flipt-0.2.1/src/flipt/api/resources/rules/types/rule.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/rules/types/rule_create_request.py` & `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/rules/types/rule_list.py` & `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/rules/types/rule_order_request.py` & `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_order_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/rules/types/rule_update_request.py` & `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/segments/client.py` & `flipt-0.2.1/src/flipt/api/resources/segments/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/segments/types/segment.py` & `flipt-0.2.1/src/flipt/api/resources/segments/types/segment.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/segments/types/segment_create_request.py` & `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/segments/types/segment_list.py` & `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/segments/types/segment_match_type.py` & `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_match_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/segments/types/segment_update_request.py` & `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/variants/client.py` & `flipt-0.2.1/src/flipt/api/resources/variants/client.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/variants/types/variant.py` & `flipt-0.2.1/src/flipt/api/resources/variants/types/variant.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/variants/types/variant_create_request.py` & `flipt-0.2.1/src/flipt/api/resources/variants/types/variant_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/src/flipt/api/resources/variants/types/variant_update_request.py` & `flipt-0.2.1/src/flipt/api/resources/variants/types/variant_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.0/PKG-INFO` & `flipt-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipt
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

