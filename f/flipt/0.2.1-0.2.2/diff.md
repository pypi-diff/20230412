# Comparing `tmp/flipt-0.2.1.tar.gz` & `tmp/flipt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipt-0.2.1.tar", max compression
+gzip compressed data, was "flipt-0.2.2.tar", max compression
```

## Comparing `flipt-0.2.1.tar` & `flipt-0.2.2.tar`

### file list

```diff
@@ -1,89 +1,88 @@
--rw-r--r--   0        0        0      407 2023-04-12 16:29:59.886289 flipt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2485 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/__init__.py
--rw-r--r--   0        0        0     2419 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/__init__.py
--rw-r--r--   0        0        0     5308 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/client.py
--rw-r--r--   0        0        0      348 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/__init__.py
--rw-r--r--   0        0        0      326 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/core/remove_none_from_headers.py
--rw-r--r--   0        0        0     2513 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/__init__.py
--rw-r--r--   0        0        0      261 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/__init__.py
--rw-r--r--   0        0        0     8839 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/client.py
--rw-r--r--   0        0        0      369 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/__init__.py
--rw-r--r--   0        0        0     1128 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication.py
--rw-r--r--   0        0        0      943 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_list.py
--rw-r--r--   0        0        0      988 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_method.py
--rw-r--r--   0        0        0     1023 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_token.py
--rw-r--r--   0        0        0       65 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_k_8_s/__init__.py
--rw-r--r--   0        0        0     2838 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_k_8_s/client.py
--rw-r--r--   0        0        0      195 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/__init__.py
--rw-r--r--   0        0        0     4596 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/client.py
--rw-r--r--   0        0        0      252 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/__init__.py
--rw-r--r--   0        0        0      854 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_authorize_url_response.py
--rw-r--r--   0        0        0      931 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_callback_response.py
--rw-r--r--   0        0        0       65 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_token/__init__.py
--rw-r--r--   0        0        0     2974 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/auth_method_token/client.py
--rw-r--r--   0        0        0      117 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/commons/__init__.py
--rw-r--r--   0        0        0      120 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      933 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/commons/types/pageable.py
--rw-r--r--   0        0        0      279 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/__init__.py
--rw-r--r--   0        0        0     6650 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/client.py
--rw-r--r--   0        0        0      399 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint.py
--rw-r--r--   0        0        0     1215 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_comparison_type.py
--rw-r--r--   0        0        0      913 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_create_request.py
--rw-r--r--   0        0        0      913 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_update_request.py
--rw-r--r--   0        0        0      237 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/__init__.py
--rw-r--r--   0        0        0     7185 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/client.py
--rw-r--r--   0        0        0      324 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution.py
--rw-r--r--   0        0        0      868 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_create_request.py
--rw-r--r--   0        0        0      868 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_update_request.py
--rw-r--r--   0        0        0      365 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/__init__.py
--rw-r--r--   0        0        0     4879 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/client.py
--rw-r--r--   0        0        0      490 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_request.py
--rw-r--r--   0        0        0     1028 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_response.py
--rw-r--r--   0        0        0     1446 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_reason.py
--rw-r--r--   0        0        0      999 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_request.py
--rw-r--r--   0        0        0     1328 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_response.py
--rw-r--r--   0        0        0      211 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/__init__.py
--rw-r--r--   0        0        0     9921 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/client.py
--rw-r--r--   0        0        0      296 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/__init__.py
--rw-r--r--   0        0        0     1047 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag.py
--rw-r--r--   0        0        0      839 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag_create_request.py
--rw-r--r--   0        0        0      951 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag_list.py
--rw-r--r--   0        0        0      826 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/flags/types/flag_update_request.py
--rw-r--r--   0        0        0      251 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/__init__.py
--rw-r--r--   0        0        0     9631 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/client.py
--rw-r--r--   0        0        0      356 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/__init__.py
--rw-r--r--   0        0        0      973 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace.py
--rw-r--r--   0        0        0      809 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_create_request.py
--rw-r--r--   0        0        0      976 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_list.py
--rw-r--r--   0        0        0      796 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_update_request.py
--rw-r--r--   0        0        0      249 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/__init__.py
--rw-r--r--   0        0        0    12303 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/client.py
--rw-r--r--   0        0        0      365 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1142 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule.py
--rw-r--r--   0        0        0      857 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_create_request.py
--rw-r--r--   0        0        0      951 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_list.py
--rw-r--r--   0        0        0      849 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_order_request.py
--rw-r--r--   0        0        0      843 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/rules/types/rule_update_request.py
--rw-r--r--   0        0        0      273 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/__init__.py
--rw-r--r--   0        0        0    10155 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/client.py
--rw-r--r--   0        0        0      401 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment.py
--rw-r--r--   0        0        0      954 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_create_request.py
--rw-r--r--   0        0        0      966 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_list.py
--rw-r--r--   0        0        0      566 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_match_type.py
--rw-r--r--   0        0        0      941 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/segments/types/segment_update_request.py
--rw-r--r--   0        0        0      207 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/__init__.py
--rw-r--r--   0        0        0     6569 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/client.py
--rw-r--r--   0        0        0      279 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/__init__.py
--rw-r--r--   0        0        0     1035 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/variant.py
--rw-r--r--   0        0        0      861 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/variant_create_request.py
--rw-r--r--   0        0        0      861 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/api/resources/variants/types/variant_update_request.py
--rw-r--r--   0        0        0      158 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/environment.py
--rw-r--r--   0        0        0        0 2023-04-12 16:29:59.886289 flipt-0.2.1/src/flipt/py.typed
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 flipt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      407 2023-04-12 21:15:30.391660 flipt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2491 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/__init__.py
+-rw-r--r--   0        0        0     5307 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/client.py
+-rw-r--r--   0        0        0      348 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      158 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/environment.py
+-rw-r--r--   0        0        0        0 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/py.typed
+-rw-r--r--   0        0        0     2513 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/__init__.py
+-rw-r--r--   0        0        0      261 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/__init__.py
+-rw-r--r--   0        0        0     8838 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/client.py
+-rw-r--r--   0        0        0      369 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/__init__.py
+-rw-r--r--   0        0        0     1128 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication.py
+-rw-r--r--   0        0        0      943 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication_list.py
+-rw-r--r--   0        0        0      988 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication_method.py
+-rw-r--r--   0        0        0     1015 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth/types/authentication_token.py
+-rw-r--r--   0        0        0       65 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_k_8_s/__init__.py
+-rw-r--r--   0        0        0     2837 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_k_8_s/client.py
+-rw-r--r--   0        0        0      195 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/client.py
+-rw-r--r--   0        0        0      252 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py
+-rw-r--r--   0        0        0      923 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py
+-rw-r--r--   0        0        0       65 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_token/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/auth_method_token/client.py
+-rw-r--r--   0        0        0      117 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/commons/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      933 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/commons/types/pageable.py
+-rw-r--r--   0        0        0      279 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/__init__.py
+-rw-r--r--   0        0        0     6649 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/client.py
+-rw-r--r--   0        0        0      399 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/__init__.py
+-rw-r--r--   0        0        0     1127 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint.py
+-rw-r--r--   0        0        0     1215 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint_comparison_type.py
+-rw-r--r--   0        0        0      913 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint_create_request.py
+-rw-r--r--   0        0        0      913 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/constraints/types/constraint_update_request.py
+-rw-r--r--   0        0        0      237 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/__init__.py
+-rw-r--r--   0        0        0     7184 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/client.py
+-rw-r--r--   0        0        0      324 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/distribution.py
+-rw-r--r--   0        0        0      868 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/distribution_create_request.py
+-rw-r--r--   0        0        0      868 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/distributions/types/distribution_update_request.py
+-rw-r--r--   0        0        0      365 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/__init__.py
+-rw-r--r--   0        0        0     4878 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/client.py
+-rw-r--r--   0        0        0      490 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_request.py
+-rw-r--r--   0        0        0     1028 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_response.py
+-rw-r--r--   0        0        0     1446 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_reason.py
+-rw-r--r--   0        0        0      999 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_request.py
+-rw-r--r--   0        0        0     1328 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_response.py
+-rw-r--r--   0        0        0      211 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/flags/__init__.py
+-rw-r--r--   0        0        0     9920 2023-04-12 21:15:30.391660 flipt-0.2.2/src/flipt/resources/flags/client.py
+-rw-r--r--   0        0        0      296 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/__init__.py
+-rw-r--r--   0        0        0     1047 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag.py
+-rw-r--r--   0        0        0      839 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag_create_request.py
+-rw-r--r--   0        0        0      951 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag_list.py
+-rw-r--r--   0        0        0      826 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/flags/types/flag_update_request.py
+-rw-r--r--   0        0        0      251 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/__init__.py
+-rw-r--r--   0        0        0     9630 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/client.py
+-rw-r--r--   0        0        0      356 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/__init__.py
+-rw-r--r--   0        0        0      973 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace.py
+-rw-r--r--   0        0        0      809 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_create_request.py
+-rw-r--r--   0        0        0      976 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_list.py
+-rw-r--r--   0        0        0      796 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_update_request.py
+-rw-r--r--   0        0        0      249 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/__init__.py
+-rw-r--r--   0        0        0    12302 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/client.py
+-rw-r--r--   0        0        0      365 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1142 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule.py
+-rw-r--r--   0        0        0      857 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_create_request.py
+-rw-r--r--   0        0        0      951 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_list.py
+-rw-r--r--   0        0        0      849 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_order_request.py
+-rw-r--r--   0        0        0      843 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/rules/types/rule_update_request.py
+-rw-r--r--   0        0        0      273 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/__init__.py
+-rw-r--r--   0        0        0    10154 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/client.py
+-rw-r--r--   0        0        0      401 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/__init__.py
+-rw-r--r--   0        0        0     1165 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment.py
+-rw-r--r--   0        0        0      954 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_create_request.py
+-rw-r--r--   0        0        0      966 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_list.py
+-rw-r--r--   0        0        0      566 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_match_type.py
+-rw-r--r--   0        0        0      941 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/segments/types/segment_update_request.py
+-rw-r--r--   0        0        0      207 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/__init__.py
+-rw-r--r--   0        0        0     6568 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/client.py
+-rw-r--r--   0        0        0      279 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/__init__.py
+-rw-r--r--   0        0        0     1035 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/variant.py
+-rw-r--r--   0        0        0      861 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/variant_create_request.py
+-rw-r--r--   0        0        0      861 2023-04-12 21:15:30.395660 flipt-0.2.2/src/flipt/resources/variants/types/variant_update_request.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 flipt-0.2.2/PKG-INFO
```

### Comparing `flipt-0.2.1/src/flipt/__init__.py` & `flipt-0.2.2/src/flipt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .api import (
+from .environment import FliptApiEnvironment
+from .resources import (
     Pageable,
     auth,
     auth_method_k_8_s,
     auth_method_oidc,
     auth_method_token,
     authentication,
     authenticationList,
@@ -51,15 +52,14 @@
     segments,
     segmentUpdateRequest,
     variant,
     variantCreateRequest,
     variants,
     variantUpdateRequest,
 )
-from .environment import FliptApiEnvironment
 
 __all__ = [
     "FliptApiEnvironment",
     "Pageable",
     "auth",
     "auth_method_k_8_s",
     "auth_method_oidc",
```

### Comparing `flipt-0.2.1/src/flipt/api/client.py` & `flipt-0.2.2/src/flipt/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
 from backports.cached_property import cached_property
 
-from ..environment import FliptApiEnvironment
+from .environment import FliptApiEnvironment
 from .resources.auth.client import AsyncAuthClient, AuthClient
 from .resources.auth_method_k_8_s.client import AsyncAuthMethodK8SClient, AuthMethodK8SClient
 from .resources.auth_method_oidc.client import AsyncAuthMethodOidcClient, AuthMethodOidcClient
 from .resources.auth_method_token.client import AsyncAuthMethodTokenClient, AuthMethodTokenClient
 from .resources.constraints.client import AsyncConstraintsClient, ConstraintsClient
 from .resources.distributions.client import AsyncDistributionsClient, DistributionsClient
 from .resources.evaluate.client import AsyncEvaluateClient, EvaluateClient
```

### Comparing `flipt-0.2.1/src/flipt/api/core/datetime_utils.py` & `flipt-0.2.2/src/flipt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/core/jsonable_encoder.py` & `flipt-0.2.2/src/flipt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/__init__.py` & `flipt-0.2.2/src/flipt/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth/client.py` & `flipt-0.2.2/src/flipt/resources/auth/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.authentication import authentication
 from .types.authentication_list import authenticationList
 
 
 class AuthClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication.py` & `flipt-0.2.2/src/flipt/resources/auth/types/authentication.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_list.py` & `flipt-0.2.2/src/flipt/resources/auth/types/authentication_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_method.py` & `flipt-0.2.2/src/flipt/resources/auth/types/authentication_method.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth/types/authentication_token.py` & `flipt-0.2.2/src/flipt/resources/auth/types/authentication_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .authentication import authentication as api_resources_auth_types_authentication_authentication
+from .authentication import authentication as resources_auth_types_authentication_authentication
 
 
 class authenticationToken(pydantic.BaseModel):
     client_token: str = pydantic.Field(alias="clientToken")
-    authentication: api_resources_auth_types_authentication_authentication
+    authentication: resources_auth_types_authentication_authentication
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth_method_k_8_s/client.py` & `flipt-0.2.2/src/flipt/resources/auth_method_k_8_s/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from ..auth.types.authentication_token import authenticationToken
 
 
 class AuthMethodK8SClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/client.py` & `flipt-0.2.2/src/flipt/resources/auth_method_oidc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.oidc_authorize_url_response import oidcAuthorizeURLResponse
 from .types.oidc_callback_response import oidcCallbackResponse
 
 
 class AuthMethodOidcClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_authorize_url_response.py` & `flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth_method_oidc/types/oidc_callback_response.py` & `flipt-0.2.2/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...auth.types.authentication import authentication as api_resources_auth_types_authentication_authentication
+from ...auth.types.authentication import authentication as resources_auth_types_authentication_authentication
 
 
 class oidcCallbackResponse(pydantic.BaseModel):
-    authentication: api_resources_auth_types_authentication_authentication
+    authentication: resources_auth_types_authentication_authentication
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/auth_method_token/client.py` & `flipt-0.2.2/src/flipt/resources/auth_method_token/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from ..auth.types.authentication_token import authenticationToken
 
 
 class AuthMethodTokenClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/commons/types/pageable.py` & `flipt-0.2.2/src/flipt/resources/commons/types/pageable.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/constraints/client.py` & `flipt-0.2.2/src/flipt/resources/constraints/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.constraint import constraint
 from .types.constraint_create_request import constraintCreateRequest
 from .types.constraint_update_request import constraintUpdateRequest
 
 
 class ConstraintsClient:
     def __init__(
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint.py` & `flipt-0.2.2/src/flipt/resources/constraints/types/constraint.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_comparison_type.py` & `flipt-0.2.2/src/flipt/resources/constraints/types/constraint_comparison_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_create_request.py` & `flipt-0.2.2/src/flipt/resources/constraints/types/constraint_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/constraints/types/constraint_update_request.py` & `flipt-0.2.2/src/flipt/resources/constraints/types/constraint_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/distributions/client.py` & `flipt-0.2.2/src/flipt/resources/distributions/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.distribution import distribution
 from .types.distribution_create_request import distributionCreateRequest
 from .types.distribution_update_request import distributionUpdateRequest
 
 
 class DistributionsClient:
     def __init__(
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution.py` & `flipt-0.2.2/src/flipt/resources/distributions/types/distribution.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_create_request.py` & `flipt-0.2.2/src/flipt/resources/distributions/types/distribution_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/distributions/types/distribution_update_request.py` & `flipt-0.2.2/src/flipt/resources/distributions/types/distribution_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/evaluate/client.py` & `flipt-0.2.2/src/flipt/resources/evaluate/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.batch_evaluation_request import batchEvaluationRequest
 from .types.batch_evaluation_response import batchEvaluationResponse
 from .types.evaluation_request import evaluationRequest
 from .types.evaluation_response import evaluationResponse
 
 
 class EvaluateClient:
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_request.py` & `flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/evaluate/types/batch_evaluation_response.py` & `flipt-0.2.2/src/flipt/resources/evaluate/types/batch_evaluation_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_reason.py` & `flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_reason.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_request.py` & `flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/evaluate/types/evaluation_response.py` & `flipt-0.2.2/src/flipt/resources/evaluate/types/evaluation_response.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/flags/client.py` & `flipt-0.2.2/src/flipt/resources/flags/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.flag import flag
 from .types.flag_create_request import flagCreateRequest
 from .types.flag_list import flagList
 from .types.flag_update_request import flagUpdateRequest
 
 
 class FlagsClient:
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/flags/types/flag.py` & `flipt-0.2.2/src/flipt/resources/flags/types/flag.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/flags/types/flag_create_request.py` & `flipt-0.2.2/src/flipt/resources/flags/types/flag_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/flags/types/flag_list.py` & `flipt-0.2.2/src/flipt/resources/flags/types/flag_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/flags/types/flag_update_request.py` & `flipt-0.2.2/src/flipt/resources/flags/types/flag_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/namespaces/client.py` & `flipt-0.2.2/src/flipt/resources/namespaces/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.namespace import namespace
 from .types.namespace_create_request import namespaceCreateRequest
 from .types.namespace_list import namespaceList
 from .types.namespace_update_request import namespaceUpdateRequest
 
 
 class NamespacesClient:
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace.py` & `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_create_request.py` & `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_list.py` & `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/namespaces/types/namespace_update_request.py` & `flipt-0.2.2/src/flipt/resources/namespaces/types/namespace_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/rules/client.py` & `flipt-0.2.2/src/flipt/resources/rules/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.rule import rule
 from .types.rule_create_request import ruleCreateRequest
 from .types.rule_list import ruleList
 from .types.rule_order_request import ruleOrderRequest
 from .types.rule_update_request import ruleUpdateRequest
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/rules/types/rule.py` & `flipt-0.2.2/src/flipt/resources/rules/types/rule.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_create_request.py` & `flipt-0.2.2/src/flipt/resources/rules/types/rule_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_list.py` & `flipt-0.2.2/src/flipt/resources/rules/types/rule_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_order_request.py` & `flipt-0.2.2/src/flipt/resources/rules/types/rule_order_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/rules/types/rule_update_request.py` & `flipt-0.2.2/src/flipt/resources/rules/types/rule_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/segments/client.py` & `flipt-0.2.2/src/flipt/resources/segments/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.segment import segment
 from .types.segment_create_request import segmentCreateRequest
 from .types.segment_list import segmentList
 from .types.segment_update_request import segmentUpdateRequest
 
 
 class SegmentsClient:
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/segments/types/segment.py` & `flipt-0.2.2/src/flipt/resources/segments/types/segment.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_create_request.py` & `flipt-0.2.2/src/flipt/resources/segments/types/segment_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_list.py` & `flipt-0.2.2/src/flipt/resources/segments/types/segment_list.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_match_type.py` & `flipt-0.2.2/src/flipt/resources/segments/types/segment_match_type.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/segments/types/segment_update_request.py` & `flipt-0.2.2/src/flipt/resources/segments/types/segment_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/variants/client.py` & `flipt-0.2.2/src/flipt/resources/variants/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ....environment import FliptApiEnvironment
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import FliptApiEnvironment
 from .types.variant import variant
 from .types.variant_create_request import variantCreateRequest
 from .types.variant_update_request import variantUpdateRequest
 
 
 class VariantsClient:
     def __init__(
```

### Comparing `flipt-0.2.1/src/flipt/api/resources/variants/types/variant.py` & `flipt-0.2.2/src/flipt/resources/variants/types/variant.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/variants/types/variant_create_request.py` & `flipt-0.2.2/src/flipt/resources/variants/types/variant_create_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/src/flipt/api/resources/variants/types/variant_update_request.py` & `flipt-0.2.2/src/flipt/resources/variants/types/variant_update_request.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.1/PKG-INFO` & `flipt-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipt
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

