# Comparing `tmp/moto-4.1.8.dev5.tar.gz` & `tmp/moto-4.1.8.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moto-4.1.8.dev5.tar", last modified: Wed Apr 12 11:10:57 2023, max compression
+gzip compressed data, was "moto-4.1.8.dev6.tar", last modified: Wed Apr 12 21:12:46 2023, max compression
```

## Comparing `moto-4.1.8.dev5.tar` & `moto-4.1.8.dev6.tar`

### file list

```diff
@@ -1,2077 +1,2077 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.038176 moto-4.1.8.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-12 11:10:57.038176 moto-4.1.8.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.642173 moto-4.1.8.dev5/moto/
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-12 11:10:50.000000 moto-4.1.8.dev5/moto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.642173 moto-4.1.8.dev5/moto/acm/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acm/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acm/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acm/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.642173 moto-4.1.8.dev5/moto/acmpca/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acmpca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acmpca/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acmpca/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acmpca/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/acmpca/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.646173 moto-4.1.8.dev5/moto/amp/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/amp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/amp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/amp/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/amp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/amp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.646173 moto-4.1.8.dev5/moto/apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.646173 moto-4.1.8.dev5/moto/apigateway/integration_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/integration_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/integration_parsers/aws_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/integration_parsers/http_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/integration_parsers/unknown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    91751 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.650174 moto-4.1.8.dev5/moto/apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigatewayv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    64715 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigatewayv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    36307 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigatewayv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/apigatewayv2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.650174 moto-4.1.8.dev5/moto/applicationautoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/applicationautoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/applicationautoscaling/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19977 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/applicationautoscaling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/applicationautoscaling/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/applicationautoscaling/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/applicationautoscaling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.650174 moto-4.1.8.dev5/moto/appsync/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/appsync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/appsync/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/appsync/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/appsync/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.650174 moto-4.1.8.dev5/moto/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/athena/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/athena/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/athena/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/athena/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.654173 moto-4.1.8.dev5/moto/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/autoscaling/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    61357 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/autoscaling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    65472 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/autoscaling/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/autoscaling/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.654173 moto-4.1.8.dev5/moto/awslambda/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/awslambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/awslambda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    75083 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/awslambda/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/awslambda/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/awslambda/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/awslambda/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/awslambda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/backend_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.654173 moto-4.1.8.dev5/moto/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    69404 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.654173 moto-4.1.8.dev5/moto/batch_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch_simple/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch_simple/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/batch_simple/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.658173 moto-4.1.8.dev5/moto/budgets/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/budgets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/budgets/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/budgets/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/budgets/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.658173 moto-4.1.8.dev5/moto/ce/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ce/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ce/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ce/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ce/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.658173 moto-4.1.8.dev5/moto/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    53038 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudformation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.658173 moto-4.1.8.dev5/moto/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudfront/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudfront/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudfront/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudfront/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.658173 moto-4.1.8.dev5/moto/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudtrail/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudtrail/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudtrail/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudtrail/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.662174 moto-4.1.8.dev5/moto/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudwatch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33739 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudwatch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudwatch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudwatch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cloudwatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.662174 moto-4.1.8.dev5/moto/codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codebuild/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codebuild/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codebuild/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codebuild/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.662174 moto-4.1.8.dev5/moto/codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codecommit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codecommit/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codecommit/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codecommit/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.662174 moto-4.1.8.dev5/moto/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codepipeline/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codepipeline/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codepipeline/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/codepipeline/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.666174 moto-4.1.8.dev5/moto/cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidentity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidentity/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidentity/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidentity/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidentity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.666174 moto-4.1.8.dev5/moto/cognitoidp/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    83922 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.666174 moto-4.1.8.dev5/moto/cognitoidp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/resources/jwks-private.json
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/resources/jwks-public.json
--rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/cognitoidp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.666174 moto-4.1.8.dev5/moto/comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/comprehend/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/comprehend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/comprehend/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/comprehend/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.666174 moto-4.1.8.dev5/moto/config/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    81665 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/config/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.666174 moto-4.1.8.dev5/moto/config/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   117575 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/config/resources/aws_managed_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/config/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/config/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.670174 moto-4.1.8.dev5/moto/core/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/botocore_stubber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/common_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/custom_responses_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/model_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/responses_custom_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.670174 moto-4.1.8.dev5/moto/databrew/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/databrew/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25372 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/databrew/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19227 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/databrew/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/databrew/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.670174 moto-4.1.8.dev5/moto/datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datapipeline/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datapipeline/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datapipeline/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datapipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.670174 moto-4.1.8.dev5/moto/datasync/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datasync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datasync/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datasync/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/datasync/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.674174 moto-4.1.8.dev5/moto/dax/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dax/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dax/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dax/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.674174 moto-4.1.8.dev5/moto/dms/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dms/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dms/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.674174 moto-4.1.8.dev5/moto/ds/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ds/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ds/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ds/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ds/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ds/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ds/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.674174 moto-4.1.8.dev5/moto/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42639 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/limits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.678174 moto-4.1.8.dev5/moto/dynamodb/models/
--rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/models/dynamo_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    39809 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/models/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/models/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.678174 moto-4.1.8.dev5/moto/dynamodb/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/ast_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34656 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/key_condition_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/reserved_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/reserved_keywords.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/parsing/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    44274 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.678174 moto-4.1.8.dev5/moto/dynamodb_v20111205/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb_v20111205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb_v20111205/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb_v20111205/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb_v20111205/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodb_v20111205/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.678174 moto-4.1.8.dev5/moto/dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodbstreams/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodbstreams/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/dynamodbstreams/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.678174 moto-4.1.8.dev5/moto/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ebs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ebs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ebs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.682174 moto-4.1.8.dev5/moto/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.686174 moto-4.1.8.dev5/moto/ec2/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/amis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/iam_instance_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/managed_prefixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/spot_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/transit_gateway_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/transit_gateway_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/vpc_peering_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/vpn_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/models/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.686174 moto-4.1.8.dev5/moto/ec2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/amis.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.610173 moto-4.1.8.dev5/moto/ec2/resources/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.698174 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/
--rw-r--r--   0 runner    (1001) docker     (123)   110385 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   184754 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   205924 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    76970 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   233439 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   224300 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   204442 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   236846 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   196475 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   151250 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   205418 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   205543 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   170773 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   216660 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   244124 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   219056 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   243613 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.610173 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.702174 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/
--rw-r--r--   0 runner    (1001) docker     (123)    39225 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    38329 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   112314 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    79281 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    40814 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    71563 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   100189 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   100490 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    31415 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    64924 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   102387 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23689 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    51275 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    50123 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   121525 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    71490 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    58608 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37026 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    65537 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   199785 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   111712 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147856 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.710174 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/
--rw-r--r--   0 runner    (1001) docker     (123)    37488 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   102960 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    72651 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    37400 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    68395 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    91831 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    92102 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    28787 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    60279 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    95067 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    49010 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    47906 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   117899 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    69350 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    56856 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    35385 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    63575 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   193821 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   108380 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    47322 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   143444 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.714174 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    40058 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    36117 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    34296 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    35491 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    40817 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    41549 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37729 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    41477 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)  1293784 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/instance_types.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.722174 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.730174 moto-4.1.8.dev5/moto/ec2/responses/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/account_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/egress_only_internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/iam_instance_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/spot_fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/spot_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/transit_gateway_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/transit_gateway_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/transit_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/virtual_private_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/vpc_peering_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    39221 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/responses/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    28837 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.730174 moto-4.1.8.dev5/moto/ec2instanceconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2instanceconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2instanceconnect/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2instanceconnect/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ec2instanceconnect/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.730174 moto-4.1.8.dev5/moto/ecr/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39840 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecr/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecr/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecr/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.730174 moto-4.1.8.dev5/moto/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    86634 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ecs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.730174 moto-4.1.8.dev5/moto/efs/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/efs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26760 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/efs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/efs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/efs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.734174 moto-4.1.8.dev5/moto/eks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/eks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30391 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/eks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/eks/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/eks/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/eks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.734174 moto-4.1.8.dev5/moto/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticache/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticache/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticache/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.734174 moto-4.1.8.dev5/moto/elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticbeanstalk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticbeanstalk/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    57275 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticbeanstalk/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticbeanstalk/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elasticbeanstalk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.734174 moto-4.1.8.dev5/moto/elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elastictranscoder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elastictranscoder/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elastictranscoder/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.738174 moto-4.1.8.dev5/moto/elb/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elb/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.738174 moto-4.1.8.dev5/moto/elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elbv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    69762 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elbv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    68565 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elbv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elbv2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/elbv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.738174 moto-4.1.8.dev5/moto/emr/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    65244 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emr/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emr/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.738174 moto-4.1.8.dev5/moto/emrcontainers/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrcontainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrcontainers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrcontainers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrcontainers/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrcontainers/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrcontainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.742174 moto-4.1.8.dev5/moto/emrserverless/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrserverless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrserverless/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrserverless/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrserverless/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/emrserverless/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.742174 moto-4.1.8.dev5/moto/es/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/es/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/es/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/es/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/es/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.742174 moto-4.1.8.dev5/moto/events/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    66807 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/events/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/events/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/events/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.742174 moto-4.1.8.dev5/moto/firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/firehose/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/firehose/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/firehose/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/firehose/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.746174 moto-4.1.8.dev5/moto/forecast/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/forecast/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/forecast/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/forecast/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/forecast/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.746174 moto-4.1.8.dev5/moto/glacier/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glacier/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glacier/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glacier/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glacier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.746174 moto-4.1.8.dev5/moto/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/glue_schema_registry_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/glue_schema_registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52028 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    21842 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/glue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.746174 moto-4.1.8.dev5/moto/greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/greengrass/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    54499 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/greengrass/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/greengrass/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/greengrass/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.750174 moto-4.1.8.dev5/moto/guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/guardduty/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/guardduty/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/guardduty/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/guardduty/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.754174 moto-4.1.8.dev5/moto/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)  1599363 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/aws_managed_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   118618 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)   107097 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.754174 moto-4.1.8.dev5/moto/identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/identitystore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/identitystore/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/identitystore/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/identitystore/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.754174 moto-4.1.8.dev5/moto/instance_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/instance_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/instance_metadata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/instance_metadata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/instance_metadata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.754174 moto-4.1.8.dev5/moto/iot/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    70619 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iot/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iot/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.758174 moto-4.1.8.dev5/moto/iotdata/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iotdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iotdata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iotdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iotdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/iotdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.758174 moto-4.1.8.dev5/moto/kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37257 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesis/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesis/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesis/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.758174 moto-4.1.8.dev5/moto/kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideo/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideo/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.758174 moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.762174 moto-4.1.8.dev5/moto/kms/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24509 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kms/policy_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25988 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kms/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kms/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/kms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.762174 moto-4.1.8.dev5/moto/lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/lakeformation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/lakeformation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/lakeformation/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/lakeformation/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.762174 moto-4.1.8.dev5/moto/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/logs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/logs/metric_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/logs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/logs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/logs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/logs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.766174 moto-4.1.8.dev5/moto/managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/managedblockchain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37565 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/managedblockchain/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/managedblockchain/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/managedblockchain/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/managedblockchain/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.766174 moto-4.1.8.dev5/moto/mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediaconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediaconnect/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediaconnect/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediaconnect/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.766174 moto-4.1.8.dev5/moto/medialive/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/medialive/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/medialive/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/medialive/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/medialive/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.766174 moto-4.1.8.dev5/moto/mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediapackage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediapackage/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediapackage/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediapackage/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.770174 moto-4.1.8.dev5/moto/mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastore/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastore/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastore/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.770174 moto-4.1.8.dev5/moto/mediastoredata/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastoredata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastoredata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastoredata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastoredata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mediastoredata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.770174 moto-4.1.8.dev5/moto/meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/meteringmarketplace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/meteringmarketplace/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/meteringmarketplace/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/meteringmarketplace/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.770174 moto-4.1.8.dev5/moto/moto_api/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.770174 moto-4.1.8.dev5/moto/moto_api/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/managed_state_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/moto_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.774174 moto-4.1.8.dev5/moto/moto_api/_internal/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/recorder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/recorder/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_api/_internal/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.774174 moto-4.1.8.dev5/moto/moto_server/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.774174 moto-4.1.8.dev5/moto/moto_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_server/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_server/threaded_moto_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_server/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/moto_server/werkzeug_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.774174 moto-4.1.8.dev5/moto/mq/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mq/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mq/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/mq/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.774174 moto-4.1.8.dev5/moto/neptune/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/neptune/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/neptune/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/neptune/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/neptune/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.778174 moto-4.1.8.dev5/moto/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opensearch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opensearch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opensearch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opensearch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opensearch/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.778174 moto-4.1.8.dev5/moto/opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opsworks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24989 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opsworks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opsworks/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/opsworks/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.778174 moto-4.1.8.dev5/moto/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/organizations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/organizations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/organizations/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/organizations/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/organizations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.778174 moto-4.1.8.dev5/moto/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.778174 moto-4.1.8.dev5/moto/packages/boto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.778174 moto-4.1.8.dev5/moto/packages/boto/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/ec2/blockdevicemapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/ec2/ec2object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/ec2/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/ec2/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/ec2/instancetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/boto/ec2/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.778174 moto-4.1.8.dev5/moto/packages/cfnresponse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/cfnresponse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/packages/cfnresponse/cfnresponse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.782174 moto-4.1.8.dev5/moto/personalize/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/personalize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/personalize/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/personalize/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/personalize/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.782174 moto-4.1.8.dev5/moto/pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/pinpoint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/pinpoint/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/pinpoint/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/pinpoint/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.782174 moto-4.1.8.dev5/moto/polly/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/polly/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/polly/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/polly/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/polly/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/polly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.782174 moto-4.1.8.dev5/moto/quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/quicksight/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/quicksight/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/quicksight/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/quicksight/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.786174 moto-4.1.8.dev5/moto/ram/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ram/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ram/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ram/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ram/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.786174 moto-4.1.8.dev5/moto/rds/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   175927 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.618173 moto-4.1.8.dev5/moto/rds/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.786174 moto-4.1.8.dev5/moto/rds/resources/cluster_options/
--rw-r--r--   0 runner    (1001) docker     (123)   480836 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/resources/cluster_options/aurora-postgresql.json
--rw-r--r--   0 runner    (1001) docker     (123)   133645 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/resources/cluster_options/neptune.json
--rw-r--r--   0 runner    (1001) docker     (123)    63635 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rds/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.786174 moto-4.1.8.dev5/moto/rdsdata/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rdsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rdsdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rdsdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rdsdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.790175 moto-4.1.8.dev5/moto/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshift/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshift/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29120 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshift/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshift/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.790175 moto-4.1.8.dev5/moto/redshiftdata/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshiftdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshiftdata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshiftdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshiftdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/redshiftdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.790175 moto-4.1.8.dev5/moto/rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rekognition/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rekognition/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rekognition/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/rekognition/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.790175 moto-4.1.8.dev5/moto/resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroups/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroups/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroups/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroups/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.790175 moto-4.1.8.dev5/moto/resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27328 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroupstaggingapi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroupstaggingapi/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/resourcegroupstaggingapi/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.794175 moto-4.1.8.dev5/moto/route53/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    34262 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    34372 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.794175 moto-4.1.8.dev5/moto/route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53resolver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35274 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53resolver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53resolver/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53resolver/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53resolver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/route53resolver/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.794175 moto-4.1.8.dev5/moto/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/cloud_formation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16719 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    83597 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)   115925 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/select_object_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.794175 moto-4.1.8.dev5/moto/s3bucket_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3bucket_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3bucket_path/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.798174 moto-4.1.8.dev5/moto/s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3control/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3control/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3control/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3control/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/s3control/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.798174 moto-4.1.8.dev5/moto/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sagemaker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sagemaker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28604 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sagemaker/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sagemaker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sagemaker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sagemaker/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.798174 moto-4.1.8.dev5/moto/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/scheduler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/scheduler/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/scheduler/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/scheduler/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.798174 moto-4.1.8.dev5/moto/sdb/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sdb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sdb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sdb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.802175 moto-4.1.8.dev5/moto/secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.802175 moto-4.1.8.dev5/moto/secretsmanager/list_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/list_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/list_secrets/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/secretsmanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.802175 moto-4.1.8.dev5/moto/servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicediscovery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicediscovery/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicediscovery/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicediscovery/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.802175 moto-4.1.8.dev5/moto/servicequotas/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.802175 moto-4.1.8.dev5/moto/servicequotas/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.802175 moto-4.1.8.dev5/moto/servicequotas/resources/default_quotas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/resources/default_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/resources/default_quotas/vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/servicequotas/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.806175 moto-4.1.8.dev5/moto/ses/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21690 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    31667 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.806175 moto-4.1.8.dev5/moto/signer/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/signer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/signer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/signer/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/signer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.806175 moto-4.1.8.dev5/moto/sns/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sns/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    38878 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sns/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    46551 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sns/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sns/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.806175 moto-4.1.8.dev5/moto/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sqs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sqs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41436 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sqs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sqs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sqs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sqs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.810175 moto-4.1.8.dev5/moto/ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    75789 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.810175 moto-4.1.8.dev5/moto/ssm/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.818175 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.622173 moto-4.1.8.dev5/moto/ssm/resources/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.842175 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/
--rw-r--r--   0 runner    (1001) docker     (123)   416937 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   688021 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   738181 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   360357 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   798560 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    85325 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   778515 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   239300 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   734929 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   806032 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    84904 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   717425 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   618637 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    99223 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   737073 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   737391 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   164329 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   659463 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   761741 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   823629 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   767008 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   820874 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)  1727049 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/regions.json
--rw-r--r--   0 runner    (1001) docker     (123)  1806010 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/resources/services.json
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.846175 moto-4.1.8.dev5/moto/ssoadmin/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssoadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssoadmin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssoadmin/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssoadmin/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssoadmin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/ssoadmin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.846175 moto-4.1.8.dev5/moto/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/stepfunctions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21993 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/stepfunctions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/stepfunctions/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/stepfunctions/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/stepfunctions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.846175 moto-4.1.8.dev5/moto/sts/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sts/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sts/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sts/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/sts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.846175 moto-4.1.8.dev5/moto/support/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/support/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/support/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.846175 moto-4.1.8.dev5/moto/support/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   172189 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/support/resources/describe_trusted_advisor_checks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/support/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/support/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.850175 moto-4.1.8.dev5/moto/swf/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.854175 moto-4.1.8.dev5/moto/swf/models/
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/activity_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/decision_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/generic_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/history_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30491 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/workflow_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/models/workflow_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    21829 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/swf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.854175 moto-4.1.8.dev5/moto/textract/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/textract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/textract/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/textract/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/textract/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.854175 moto-4.1.8.dev5/moto/timestreamwrite/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/timestreamwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/timestreamwrite/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/timestreamwrite/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/timestreamwrite/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/timestreamwrite/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.858175 moto-4.1.8.dev5/moto/transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/transcribe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/transcribe/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/transcribe/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/transcribe/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.858175 moto-4.1.8.dev5/moto/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/aws_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/distutils_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/docker_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/tagging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.862175 moto-4.1.8.dev5/moto/wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/wafv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/wafv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/wafv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/wafv2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/wafv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.862175 moto-4.1.8.dev5/moto/xray/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/xray/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/xray/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/xray/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/xray/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/moto/xray/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.642173 moto-4.1.8.dev5/moto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-12 11:10:56.000000 moto-4.1.8.dev5/moto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66046 2023-04-12 11:10:56.000000 moto-4.1.8.dev5/moto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:10:56.000000 moto-4.1.8.dev5/moto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 11:10:56.000000 moto-4.1.8.dev5/moto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 11:10:56.000000 moto-4.1.8.dev5/moto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 11:10:56.000000 moto-4.1.8.dev5/moto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-12 11:10:57.042176 moto-4.1.8.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.862175 moto-4.1.8.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.866175 moto-4.1.8.dev5/tests/test_acm/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.866175 moto-4.1.8.dev5/tests/test_acm/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/ca.key
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/ca.srl
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com-bad.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com.csr
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com.key
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com.pem
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acm/test_acm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.866175 moto-4.1.8.dev5/tests/test_acmpca/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acmpca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_acmpca/test_acmpca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.866175 moto-4.1.8.dev5/tests/test_amp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_amp/test_amp_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_amp/test_amp_rulegroupnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_amp/test_amp_workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.870175 moto-4.1.8.dev5/tests/test_apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.870175 moto-4.1.8.dev5/tests/test_apigateway/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/resources/petstore-swagger-v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/resources/test_api.json
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/resources/test_api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/resources/test_api_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/resources/test_api_invalid_version.json
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/resources/test_deep_api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    91558 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_gatewayresponses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_importrestapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_putrestapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_vpclink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigateway/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.874175 moto-4.1.8.dev5/tests/test_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_reimport.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_apigatewayv2/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.874175 moto-4.1.8.dev5/tests/test_applicationautoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_applicationautoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_applicationautoscaling/test_applicationautoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_applicationautoscaling/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.874175 moto-4.1.8.dev5/tests/test_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_appsync/test_appsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_appsync/test_appsync_apikeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_appsync/test_appsync_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_appsync/test_appsync_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_appsync/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.874175 moto-4.1.8.dev5/tests/test_athena/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_athena/test_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_athena/test_athena_server_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.878175 moto-4.1.8.dev5/tests/test_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48170 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_scheduledactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_elb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_launch_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_autoscaling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.882175 moto-4.1.8.dev5/tests/test_awslambda/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_awslambda_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_eventsourcemapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_function_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_lambda_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_awslambda/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.882175 moto-4.1.8.dev5/tests/test_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_compute_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    34446 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_tags_job_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_tags_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_tags_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_batch_task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.882175 moto-4.1.8.dev5/tests/test_batch_simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch_simple/test_batch_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch_simple/test_batch_compute_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_batch_simple/test_batch_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.886175 moto-4.1.8.dev5/tests/test_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_budgets/test_budgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_budgets/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_budgets/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.886175 moto-4.1.8.dev5/tests/test_ce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ce/test_ce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ce/test_ce_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.886175 moto-4.1.8.dev5/tests/test_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.890175 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/custom_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/ec2_classic_eip.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/fn_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/kms_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/route53_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/route53_roundrobin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/vpc_eip.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/vpc_eni.py
--rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_custom_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_depends_on.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_multi_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_nested_stacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    85564 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    69300 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_stack_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_stack_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_import_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_stack_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudformation/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.890175 moto-4.1.8.dev5/tests/test_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudfront/cloudfront_test_scaffolding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront_dist_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront_invalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudfront/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.894175 moto-4.1.8.dev5/tests/test_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudtrail/test_cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudtrail/test_cloudtrail_eventselectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudtrail/test_cloudtrail_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudtrail/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.894175 moto-4.1.8.dev5/tests/test_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    54006 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.894175 moto-4.1.8.dev5/tests/test_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_codebuild/test_codebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.894175 moto-4.1.8.dev5/tests/test_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_codecommit/test_codecommit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.894175 moto-4.1.8.dev5/tests/test_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_codepipeline/test_codepipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.894175 moto-4.1.8.dev5/tests/test_cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidentity/test_cognitoidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidentity/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.898175 moto-4.1.8.dev5/tests/test_cognitoidp/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161791 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidp/test_cognitoidp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidp/test_cognitoidp_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidp/test_cognitoidp_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_cognitoidp/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.898175 moto-4.1.8.dev5/tests/test_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_comprehend/test_comprehend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.898175 moto-4.1.8.dev5/tests/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83099 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_config/test_config_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_config/test_config_rules_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_config/test_config_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.906175 moto-4.1.8.dev5/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_account_id_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_backenddict.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_decorator_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_environ_patching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_importorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_instance_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_mock_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_mock_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_moto_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_request_mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_responses_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_url_base_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_url_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.906175 moto-4.1.8.dev5/tests/test_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_databrew/test_databrew_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_databrew/test_databrew_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_databrew/test_databrew_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_databrew/test_databrew_rulesets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.906175 moto-4.1.8.dev5/tests/test_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_datapipeline/test_datapipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_datapipeline/test_datapipeline_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_datapipeline/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.906175 moto-4.1.8.dev5/tests/test_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_datasync/test_datasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.910175 moto-4.1.8.dev5/tests/test_dax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dax/test_dax.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dax/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.910175 moto-4.1.8.dev5/tests/test_dms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dms/test_dms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.910175 moto-4.1.8.dev5/tests/test_ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ds/test_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ds/test_ds_ad_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ds/test_ds_microsoft_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ds/test_ds_simple_ad_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ds/test_ds_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.914175 moto-4.1.8.dev5/tests/test_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.914175 moto-4.1.8.dev5/tests/test_dynamodb/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/exceptions/test_key_length_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.914175 moto-4.1.8.dev5/tests/test_dynamodb/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/models/test_key_condition_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   205697 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_batch_get_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_condition_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_consumedcapacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_create_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39804 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_table_with_range_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_table_without_range_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_update_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_update_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.918175 moto-4.1.8.dev5/tests/test_dynamodb_v20111205/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb_v20111205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43145 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb_v20111205/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodb_v20111205/test_servermode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.918175 moto-4.1.8.dev5/tests/test_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_dynamodbstreams/test_dynamodbstreams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.918175 moto-4.1.8.dev5/tests/test_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ebs/test_ebs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.930175 moto-4.1.8.dev5/tests/test_ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_account_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_amazon_dev_pay.py
--rw-r--r--   0 runner    (1001) docker     (123)    44698 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_ec2_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_ec2_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_ec2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_egress_only_igw.py
--rw-r--r--   0 runner    (1001) docker     (123)    42808 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    41728 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24744 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_flow_logs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_iam_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_instance_type_offerings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    98932 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_placement_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_prefix_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40234 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    65961 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_security_groups_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_spot_fleet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_spot_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_transit_gateway_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_transit_gateway_peering_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_virtual_private_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_vm_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_vm_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_vpc_endpoint_services_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_vpc_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    45725 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2/test_windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.930175 moto-4.1.8.dev5/tests/test_ec2instanceconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.934176 moto-4.1.8.dev5/tests/test_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    91955 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecr/test_ecr_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecr/test_ecr_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecr/test_ecr_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecr/test_ecr_policy_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.934176 moto-4.1.8.dev5/tests/test_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/test_ecs_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   122175 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/test_ecs_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/test_ecs_capacity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/test_ecs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/test_ecs_efs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/test_ecs_task_def_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ecs/test_ecs_tasksets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.938176 moto-4.1.8.dev5/tests/test_efs/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/junk_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_access_point_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_access_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_filesystem_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_lifecycle_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_mount_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_mount_target_security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_efs/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.938176 moto-4.1.8.dev5/tests/test_eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52255 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_eks/test_eks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_eks/test_eks_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_eks/test_eks_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_eks/test_eks_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_eks/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.938176 moto-4.1.8.dev5/tests/test_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elasticache/test_elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elasticache/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.938176 moto-4.1.8.dev5/tests/test_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elasticbeanstalk/test_eb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.938176 moto-4.1.8.dev5/tests/test_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elastictranscoder/__init__
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elastictranscoder/test_elastictranscoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elastictranscoder/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.942175 moto-4.1.8.dev5/tests/test_elb/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41073 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elb/test_elb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elb/test_elb_availabilityzones.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elb/test_elb_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elb/test_elb_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elb/test_elb_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.942175 moto-4.1.8.dev5/tests/test_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65284 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_listener_rule_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_listener_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_listener_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_set_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_target_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_elbv2/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.946176 moto-4.1.8.dev5/tests/test_emr/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emr/test_emr_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emr/test_emr_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emr/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.946176 moto-4.1.8.dev5/tests/test_emrcontainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emrcontainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emrcontainers/test_emrcontainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emrcontainers/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.946176 moto-4.1.8.dev5/tests/test_emrserverless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emrserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emrserverless/test_emrserverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_emrserverless/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.946176 moto-4.1.8.dev5/tests/test_es/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_es/test_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_es/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.950176 moto-4.1.8.dev5/tests/test_events/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_events/test_event_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    81682 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_events/test_events_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_events/test_events_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_events/test_events_lambdatriggers_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.950176 moto-4.1.8.dev5/tests/test_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_firehose/test_firehose.py
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_firehose/test_firehose_destination_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_firehose/test_firehose_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_firehose/test_firehose_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_firehose/test_firehose_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_firehose/test_http_destinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.950176 moto-4.1.8.dev5/tests/test_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_forecast/test_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.954176 moto-4.1.8.dev5/tests/test_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glacier/test.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glacier/test_glacier_archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glacier/test_glacier_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glacier/test_glacier_vaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glacier/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.954176 moto-4.1.8.dev5/tests/test_glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.954176 moto-4.1.8.dev5/tests/test_glue/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/fixtures/datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/fixtures/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    48038 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/test_datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/test_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/test_glue_job_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/test_partition_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    47112 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_glue/test_schema_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.958176 moto-4.1.8.dev5/tests/test_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.958176 moto-4.1.8.dev5/tests/test_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_guardduty/test_guardduty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_guardduty/test_guardduty_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_guardduty/test_guardduty_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_guardduty/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.962176 moto-4.1.8.dev5/tests/test_iam/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   167646 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_access_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_account_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)    51772 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_password_last_used.py
--rw-r--r--   0 runner    (1001) docker     (123)    51265 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_iam_server_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iam/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.962176 moto-4.1.8.dev5/tests/test_identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_identitystore/test_identitystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.966176 moto-4.1.8.dev5/tests/test_iot/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_ca_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_deprecate_thing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_domain_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_job_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_thing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_thing_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_things.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_iot_topic_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iot/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.966176 moto-4.1.8.dev5/tests/test_iotdata/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iotdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iotdata/test_iotdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_iotdata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.970176 moto-4.1.8.dev5/tests/test_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31019 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_stream_consumers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_stream_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesis/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.970176 moto-4.1.8.dev5/tests/test_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesisvideo/test_kinesisvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesisvideo/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.970176 moto-4.1.8.dev5/tests/test_kinesisvideoarchivedmedia/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesisvideoarchivedmedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kinesisvideoarchivedmedia/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.974176 moto-4.1.8.dev5/tests/test_kms/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45373 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/test_kms_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/test_kms_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/test_kms_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/test_kms_policy_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_kms/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.974176 moto-4.1.8.dev5/tests/test_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_lakeformation/test_lakeformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.974176 moto-4.1.8.dev5/tests/test_logs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_logs/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    47011 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_logs/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_logs/test_logs_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_logs/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.978176 moto-4.1.8.dev5/tests/test_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_proposals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.978176 moto-4.1.8.dev5/tests/test_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediaconnect/test_mediaconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediaconnect/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.978176 moto-4.1.8.dev5/tests/test_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_medialive/test_medialive.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_medialive/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.978176 moto-4.1.8.dev5/tests/test_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediapackage/test_mediapackage.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediapackage/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.978176 moto-4.1.8.dev5/tests/test_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediastore/test_mediastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediastore/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_mediastoredata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediastoredata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediastoredata/test_mediastoredata.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mediastoredata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_meteringmarketplace/test_meteringmarketplace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_moto_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_moto_api/mock_random/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/mock_random/test_mock_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_moto_api/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/recorder/test_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_moto_api/state_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/state_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_moto_api/state_manager/servermode/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/state_manager/servermode/test_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/state_manager/test_batch_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/state_manager/test_managed_state_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_moto_api/state_manager/test_state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.982176 moto-4.1.8.dev5/tests/test_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mq/test_mq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mq/test_mq_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mq/test_mq_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mq/test_mq_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_mq/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.986176 moto-4.1.8.dev5/tests/test_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_neptune/test_cluster_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_neptune/test_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_neptune/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_neptune/test_global_clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.986176 moto-4.1.8.dev5/tests/test_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opensearch/test_domain_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opensearch/test_opensearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.986176 moto-4.1.8.dev5/tests/test_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opsworks/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opsworks/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opsworks/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_opsworks/test_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.986176 moto-4.1.8.dev5/tests/test_organizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_organizations/organizations_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    85363 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_organizations/test_organizations_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.986176 moto-4.1.8.dev5/tests/test_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_personalize/test_personalize_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.990176 moto-4.1.8.dev5/tests/test_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_pinpoint/test_pinpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_pinpoint/test_pinpoint_application_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_pinpoint/test_pinpoint_event_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.990176 moto-4.1.8.dev5/tests/test_polly/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_polly/test_polly.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_polly/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.990176 moto-4.1.8.dev5/tests/test_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_quicksight/test_quicksight_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_quicksight/test_quicksight_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_quicksight/test_quicksight_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.990176 moto-4.1.8.dev5/tests/test_ram/
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ram/test_ram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.994176 moto-4.1.8.dev5/tests/test_rds/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_db_cluster_param_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_db_cluster_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_global_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)    91218 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_rds_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_rds_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_rds_clusters_with_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_rds_event_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_rds_export_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rds/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.994176 moto-4.1.8.dev5/tests/test_rdsdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rdsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rdsdata/test_rdsdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.994176 moto-4.1.8.dev5/tests/test_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshift/test_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshift/test_redshift_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshift/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.998176 moto-4.1.8.dev5/tests/test_redshiftdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshiftdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshiftdata/test_redshiftdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshiftdata/test_redshiftdata_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_redshiftdata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.998176 moto-4.1.8.dev5/tests/test_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_rekognition/test_rekognition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.998176 moto-4.1.8.dev5/tests/test_resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_resourcegroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_resourcegroups/test_resourcegroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.998176 moto-4.1.8.dev5/tests/test_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_resourcegroupstaggingapi/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:56.998176 moto-4.1.8.dev5/tests/test_route53/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_change_set_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52862 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_route53.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_route53_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_route53_delegationsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_route53_healthchecks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_route53_query_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_route53_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.002176 moto-4.1.8.dev5/tests/test_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_rule_associations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.006176 moto-4.1.8.dev5/tests/test_s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_multiple_accounts_server.py
--rw-r--r--   0 runner    (1001) docker     (123)   115801 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_classdecorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_copyobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_custom_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_file_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_lambda_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    31026 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_object_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_storageclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.006176 moto-4.1.8.dev5/tests/test_s3bucket_path/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3bucket_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3bucket_path/test_s3bucket_path_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3bucket_path/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.010176 moto-4.1.8.dev5/tests/test_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3control/test_s3control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3control/test_s3control_access_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3control/test_s3control_accesspoint_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3control/test_s3control_config_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_s3control/test_s3control_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.010176 moto-4.1.8.dev5/tests/test_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/cloudformation_test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20469 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24758 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_trial_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.014176 moto-4.1.8.dev5/tests/test_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_scheduler/test_schedule_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_scheduler/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_scheduler/test_scheduler_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_scheduler/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.014176 moto-4.1.8.dev5/tests/test_sdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sdb/test_sdb_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sdb/test_sdb_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sdb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.014176 moto-4.1.8.dev5/tests/test_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_secretsmanager/test_list_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_secretsmanager/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    57270 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_secretsmanager/test_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    33144 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_secretsmanager/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.014176 moto-4.1.8.dev5/tests/test_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicediscovery/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.018176 moto-4.1.8.dev5/tests/test_servicequotas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicequotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_servicequotas/test_servicequotas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.018176 moto-4.1.8.dev5/tests/test_ses/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ses/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    52328 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ses/test_ses_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ses/test_ses_sns_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ses/test_ses_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ses/test_templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.018176 moto-4.1.8.dev5/tests/test_signer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_signer/test_signing_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_signer/test_signing_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.022176 moto-4.1.8.dev5/tests/test_sns/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/test_application_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/test_publish_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    42805 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/test_publishing_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/test_sns_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/test_subscriptions_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sns/test_topics_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.022176 moto-4.1.8.dev5/tests/test_special_cases/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_special_cases/test_custom_amis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.022176 moto-4.1.8.dev5/tests/test_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sqs/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)   110801 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sqs/test_sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sqs/test_sqs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sqs/test_sqs_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sqs/test_sqs_multiaccount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.026176 moto-4.1.8.dev5/tests/test_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71927 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_default_amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_doc_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_ec2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_ecs_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_maintenance_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_parameterstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_ssm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.026176 moto-4.1.8.dev5/tests/test_ssm/test_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssm/test_templates/good.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.026176 moto-4.1.8.dev5/tests/test_ssoadmin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssoadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssoadmin/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_ssoadmin/test_ssoadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.026176 moto-4.1.8.dev5/tests/test_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_stepfunctions/test_stepfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_stepfunctions/test_stepfunctions_cloudformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.026176 moto-4.1.8.dev5/tests/test_sts/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sts/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sts/test_sts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_sts/test_sts_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.030176 moto-4.1.8.dev5/tests/test_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_support/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_support/test_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.030176 moto-4.1.8.dev5/tests/test_swf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.030176 moto-4.1.8.dev5/tests/test_swf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_activity_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_decision_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_generic_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_history_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/models/test_workflow_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.034176 moto-4.1.8.dev5/tests/test_swf/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/test_activity_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/test_activity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21702 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/test_decision_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/test_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/test_workflow_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/responses/test_workflow_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_swf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.034176 moto-4.1.8.dev5/tests/test_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_textract/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_textract/test_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.034176 moto-4.1.8.dev5/tests/test_timestreamwrite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_timestreamwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_timestreamwrite/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_timestreamwrite/test_timestreamwrite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_timestreamwrite/test_timestreamwrite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_timestreamwrite/test_timestreamwrite_tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.034176 moto-4.1.8.dev5/tests/test_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_transcribe/test_transcribe_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.038176 moto-4.1.8.dev5/tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_utilities/test_docker_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_utilities/test_paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_utilities/test_tagging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_utilities/test_threaded_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.038176 moto-4.1.8.dev5/tests/test_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/test_wafv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/test_wafv2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/test_wafv2_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_wafv2/test_wafv2_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:57.038176 moto-4.1.8.dev5/tests/test_xray/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_xray/test_xray_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-12 11:10:48.000000 moto-4.1.8.dev5/tests/test_xray/test_xray_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.011414 moto-4.1.8.dev6/moto/
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-12 21:12:39.000000 moto-4.1.8.dev6/moto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.015414 moto-4.1.8.dev6/moto/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acm/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acm/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.015414 moto-4.1.8.dev6/moto/acmpca/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acmpca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acmpca/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acmpca/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acmpca/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/acmpca/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.015414 moto-4.1.8.dev6/moto/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/amp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/amp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/amp/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/amp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/amp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.015414 moto-4.1.8.dev6/moto/apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.015414 moto-4.1.8.dev6/moto/apigateway/integration_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/integration_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/integration_parsers/aws_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/integration_parsers/http_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/integration_parsers/unknown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91751 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.019414 moto-4.1.8.dev6/moto/apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigatewayv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64715 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigatewayv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36307 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigatewayv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/apigatewayv2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.019414 moto-4.1.8.dev6/moto/applicationautoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/applicationautoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/applicationautoscaling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19977 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/applicationautoscaling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/applicationautoscaling/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/applicationautoscaling/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/applicationautoscaling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.019414 moto-4.1.8.dev6/moto/appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/appsync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/appsync/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/appsync/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/appsync/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.019414 moto-4.1.8.dev6/moto/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/athena/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/athena/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/athena/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/athena/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.019414 moto-4.1.8.dev6/moto/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/autoscaling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61357 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/autoscaling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65472 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/autoscaling/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/autoscaling/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.023414 moto-4.1.8.dev6/moto/awslambda/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/awslambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/awslambda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75083 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/awslambda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/awslambda/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/awslambda/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/awslambda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/awslambda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/backend_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.023414 moto-4.1.8.dev6/moto/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69404 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.023414 moto-4.1.8.dev6/moto/batch_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch_simple/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch_simple/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/batch_simple/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.023414 moto-4.1.8.dev6/moto/budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/budgets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/budgets/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/budgets/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/budgets/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.027415 moto-4.1.8.dev6/moto/ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ce/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ce/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ce/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ce/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.027415 moto-4.1.8.dev6/moto/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53038 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudformation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.027415 moto-4.1.8.dev6/moto/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudfront/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudfront/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudfront/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudfront/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.027415 moto-4.1.8.dev6/moto/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudtrail/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudtrail/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudtrail/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudtrail/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.031415 moto-4.1.8.dev6/moto/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudwatch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33739 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudwatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudwatch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudwatch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cloudwatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.031415 moto-4.1.8.dev6/moto/codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codebuild/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codebuild/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codebuild/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codebuild/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.031415 moto-4.1.8.dev6/moto/codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codecommit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codecommit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codecommit/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codecommit/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.031415 moto-4.1.8.dev6/moto/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codepipeline/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codepipeline/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codepipeline/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/codepipeline/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.035415 moto-4.1.8.dev6/moto/cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidentity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidentity/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidentity/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidentity/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidentity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.035415 moto-4.1.8.dev6/moto/cognitoidp/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83922 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.035415 moto-4.1.8.dev6/moto/cognitoidp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/resources/jwks-private.json
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/resources/jwks-public.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/cognitoidp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.035415 moto-4.1.8.dev6/moto/comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/comprehend/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/comprehend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/comprehend/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/comprehend/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.035415 moto-4.1.8.dev6/moto/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81665 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/config/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.035415 moto-4.1.8.dev6/moto/config/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   117575 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/config/resources/aws_managed_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/config/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/config/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.039415 moto-4.1.8.dev6/moto/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/botocore_stubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/common_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/custom_responses_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/model_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/responses_custom_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.039415 moto-4.1.8.dev6/moto/databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/databrew/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25372 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/databrew/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19227 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/databrew/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/databrew/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.039415 moto-4.1.8.dev6/moto/datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datapipeline/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datapipeline/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datapipeline/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datapipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.043416 moto-4.1.8.dev6/moto/datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datasync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datasync/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datasync/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/datasync/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.043416 moto-4.1.8.dev6/moto/dax/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dax/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dax/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dax/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.043416 moto-4.1.8.dev6/moto/dms/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dms/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.047416 moto-4.1.8.dev6/moto/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ds/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ds/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ds/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ds/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ds/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ds/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.047416 moto-4.1.8.dev6/moto/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42639 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.047416 moto-4.1.8.dev6/moto/dynamodb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/models/dynamo_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39809 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/models/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.047416 moto-4.1.8.dev6/moto/dynamodb/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/ast_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34656 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/key_condition_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/reserved_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/reserved_keywords.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/parsing/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44274 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.051416 moto-4.1.8.dev6/moto/dynamodb_v20111205/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb_v20111205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb_v20111205/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb_v20111205/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb_v20111205/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodb_v20111205/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.051416 moto-4.1.8.dev6/moto/dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodbstreams/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodbstreams/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/dynamodbstreams/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.051416 moto-4.1.8.dev6/moto/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ebs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ebs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ebs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.051416 moto-4.1.8.dev6/moto/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.055417 moto-4.1.8.dev6/moto/ec2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/iam_instance_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/managed_prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/spot_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/transit_gateway_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/transit_gateway_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/vpc_peering_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/vpn_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/models/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.059417 moto-4.1.8.dev6/moto/ec2/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/amis.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:45.983412 moto-4.1.8.dev6/moto/ec2/resources/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.067417 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)   110385 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   184754 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205924 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76970 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233439 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224300 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   204442 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   236846 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   196475 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   151250 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205418 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205543 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   170773 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   216660 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   244124 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219056 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243613 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:45.983412 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.075418 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    39225 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38329 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112314 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79281 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40814 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71563 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100189 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100490 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31415 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64924 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   102387 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23689 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51275 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50123 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121525 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71490 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58608 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37026 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65537 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   199785 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   111712 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147856 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.079418 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/
+-rw-r--r--   0 runner    (1001) docker     (123)    37488 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   102960 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72651 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37400 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68395 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91831 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    92102 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28787 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60279 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    95067 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49010 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47906 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   117899 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    69350 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56856 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35385 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63575 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   193821 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   108380 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47322 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   143444 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.083418 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40058 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36117 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34296 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35491 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40817 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41549 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37729 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41477 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1293784 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/instance_types.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.087419 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.095419 moto-4.1.8.dev6/moto/ec2/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/account_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/egress_only_internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/iam_instance_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/reserved_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/spot_fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/spot_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/transit_gateway_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/transit_gateway_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/transit_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/virtual_private_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/vpc_peering_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39221 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/responses/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28837 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.095419 moto-4.1.8.dev6/moto/ec2instanceconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2instanceconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2instanceconnect/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2instanceconnect/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ec2instanceconnect/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.095419 moto-4.1.8.dev6/moto/ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39840 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecr/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecr/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecr/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.095419 moto-4.1.8.dev6/moto/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86634 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ecs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.095419 moto-4.1.8.dev6/moto/efs/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/efs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26760 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/efs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/efs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/efs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.099420 moto-4.1.8.dev6/moto/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/eks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30391 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/eks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/eks/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/eks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/eks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.099420 moto-4.1.8.dev6/moto/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticache/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticache/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticache/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.099420 moto-4.1.8.dev6/moto/elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticbeanstalk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticbeanstalk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57275 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticbeanstalk/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticbeanstalk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elasticbeanstalk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.099420 moto-4.1.8.dev6/moto/elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elastictranscoder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elastictranscoder/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elastictranscoder/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.099420 moto-4.1.8.dev6/moto/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elb/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.099420 moto-4.1.8.dev6/moto/elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elbv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69762 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elbv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68565 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elbv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elbv2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/elbv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.103420 moto-4.1.8.dev6/moto/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65244 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emr/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emr/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.103420 moto-4.1.8.dev6/moto/emrcontainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrcontainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrcontainers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrcontainers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrcontainers/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrcontainers/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrcontainers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.103420 moto-4.1.8.dev6/moto/emrserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrserverless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrserverless/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrserverless/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrserverless/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/emrserverless/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.103420 moto-4.1.8.dev6/moto/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/es/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/es/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/es/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/es/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.107420 moto-4.1.8.dev6/moto/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66807 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/events/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/events/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/events/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.107420 moto-4.1.8.dev6/moto/firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/firehose/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/firehose/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/firehose/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/firehose/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.107420 moto-4.1.8.dev6/moto/forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/forecast/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/forecast/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/forecast/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/forecast/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.107420 moto-4.1.8.dev6/moto/glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glacier/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glacier/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glacier/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glacier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.107420 moto-4.1.8.dev6/moto/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/glue_schema_registry_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/glue_schema_registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52028 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21842 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/glue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.107420 moto-4.1.8.dev6/moto/greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/greengrass/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54499 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/greengrass/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/greengrass/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/greengrass/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.111420 moto-4.1.8.dev6/moto/guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/guardduty/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/guardduty/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/guardduty/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/guardduty/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.111420 moto-4.1.8.dev6/moto/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1599363 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/aws_managed_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118618 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107097 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.115421 moto-4.1.8.dev6/moto/identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/identitystore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/identitystore/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/identitystore/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/identitystore/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.115421 moto-4.1.8.dev6/moto/instance_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/instance_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/instance_metadata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/instance_metadata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/instance_metadata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.115421 moto-4.1.8.dev6/moto/iot/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70619 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iot/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.115421 moto-4.1.8.dev6/moto/iotdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iotdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iotdata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iotdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iotdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/iotdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.115421 moto-4.1.8.dev6/moto/kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37257 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesis/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesis/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesis/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.119421 moto-4.1.8.dev6/moto/kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideo/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideo/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.119421 moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.119421 moto-4.1.8.dev6/moto/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24509 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kms/policy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25988 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kms/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/kms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.119421 moto-4.1.8.dev6/moto/lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/lakeformation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/lakeformation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/lakeformation/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/lakeformation/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.119421 moto-4.1.8.dev6/moto/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/logs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/logs/metric_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/logs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/logs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/logs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/logs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.123421 moto-4.1.8.dev6/moto/managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/managedblockchain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37565 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/managedblockchain/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/managedblockchain/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/managedblockchain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/managedblockchain/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.123421 moto-4.1.8.dev6/moto/mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediaconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediaconnect/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediaconnect/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediaconnect/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.123421 moto-4.1.8.dev6/moto/medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/medialive/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/medialive/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/medialive/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/medialive/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.123421 moto-4.1.8.dev6/moto/mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediapackage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediapackage/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediapackage/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediapackage/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.123421 moto-4.1.8.dev6/moto/mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastore/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastore/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastore/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.123421 moto-4.1.8.dev6/moto/mediastoredata/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastoredata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastoredata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastoredata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastoredata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mediastoredata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/meteringmarketplace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/meteringmarketplace/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/meteringmarketplace/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/meteringmarketplace/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/moto_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/moto_api/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/managed_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/moto_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/moto_api/_internal/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/recorder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/recorder/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_api/_internal/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/moto_server/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/moto_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_server/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_server/threaded_moto_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_server/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/moto_server/werkzeug_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mq/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mq/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/mq/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.127421 moto-4.1.8.dev6/moto/neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/neptune/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/neptune/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/neptune/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/neptune/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opensearch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opensearch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opensearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opensearch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opensearch/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opsworks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opsworks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opsworks/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/opsworks/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/organizations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/organizations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/organizations/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/organizations/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/organizations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/packages/boto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/packages/boto/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/ec2/blockdevicemapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/ec2/ec2object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/ec2/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/ec2/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/ec2/instancetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/boto/ec2/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/packages/cfnresponse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/cfnresponse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/packages/cfnresponse/cfnresponse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.131422 moto-4.1.8.dev6/moto/personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/personalize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/personalize/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/personalize/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/personalize/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.135422 moto-4.1.8.dev6/moto/pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/pinpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/pinpoint/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/pinpoint/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/pinpoint/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.135422 moto-4.1.8.dev6/moto/polly/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/polly/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/polly/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/polly/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/polly/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/polly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.135422 moto-4.1.8.dev6/moto/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/quicksight/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/quicksight/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/quicksight/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/quicksight/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.135422 moto-4.1.8.dev6/moto/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ram/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ram/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ram/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ram/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.135422 moto-4.1.8.dev6/moto/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182267 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:45.991412 moto-4.1.8.dev6/moto/rds/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.139422 moto-4.1.8.dev6/moto/rds/resources/cluster_options/
+-rw-r--r--   0 runner    (1001) docker     (123)   480836 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/resources/cluster_options/aurora-postgresql.json
+-rw-r--r--   0 runner    (1001) docker     (123)   133645 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/resources/cluster_options/neptune.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64354 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.139422 moto-4.1.8.dev6/moto/rdsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rdsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rdsdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rdsdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rdsdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.139422 moto-4.1.8.dev6/moto/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshift/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshift/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29120 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshift/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshift/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.139422 moto-4.1.8.dev6/moto/redshiftdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshiftdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshiftdata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshiftdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshiftdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/redshiftdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.139422 moto-4.1.8.dev6/moto/rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rekognition/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rekognition/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rekognition/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/rekognition/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.139422 moto-4.1.8.dev6/moto/resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroups/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroups/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroups/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroups/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.143423 moto-4.1.8.dev6/moto/resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27328 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroupstaggingapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroupstaggingapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/resourcegroupstaggingapi/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.143423 moto-4.1.8.dev6/moto/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34262 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34372 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.143423 moto-4.1.8.dev6/moto/route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53resolver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35274 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53resolver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53resolver/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53resolver/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53resolver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/route53resolver/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.143423 moto-4.1.8.dev6/moto/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/cloud_formation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16719 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83597 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115925 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/select_object_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.147423 moto-4.1.8.dev6/moto/s3bucket_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3bucket_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3bucket_path/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.147423 moto-4.1.8.dev6/moto/s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3control/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3control/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3control/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3control/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/s3control/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.147423 moto-4.1.8.dev6/moto/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sagemaker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sagemaker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28604 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sagemaker/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sagemaker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sagemaker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sagemaker/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.147423 moto-4.1.8.dev6/moto/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/scheduler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/scheduler/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/scheduler/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/scheduler/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.147423 moto-4.1.8.dev6/moto/sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sdb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sdb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.147423 moto-4.1.8.dev6/moto/secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.151423 moto-4.1.8.dev6/moto/secretsmanager/list_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/list_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/list_secrets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/secretsmanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.151423 moto-4.1.8.dev6/moto/servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicediscovery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicediscovery/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicediscovery/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicediscovery/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.151423 moto-4.1.8.dev6/moto/servicequotas/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.151423 moto-4.1.8.dev6/moto/servicequotas/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.151423 moto-4.1.8.dev6/moto/servicequotas/resources/default_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/resources/default_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/resources/default_quotas/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/servicequotas/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.151423 moto-4.1.8.dev6/moto/ses/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21690 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31667 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.151423 moto-4.1.8.dev6/moto/signer/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/signer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/signer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/signer/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/signer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.155423 moto-4.1.8.dev6/moto/sns/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sns/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38878 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sns/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46551 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sns/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sns/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.155423 moto-4.1.8.dev6/moto/sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sqs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sqs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41436 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sqs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sqs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sqs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/sqs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.155423 moto-4.1.8.dev6/moto/ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75789 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.159424 moto-4.1.8.dev6/moto/ssm/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.163424 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:45.991412 moto-4.1.8.dev6/moto/ssm/resources/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.183426 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)   416937 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   688021 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   738181 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   360357 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   798560 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85325 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   778515 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   239300 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   734929 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   806032 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    84904 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   717425 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   618637 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    99223 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   737073 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   737391 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   164329 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659463 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   761741 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   823629 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   767008 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   820874 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1727049 2023-04-12 21:12:36.000000 moto-4.1.8.dev6/moto/ssm/resources/regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1806010 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssm/resources/services.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssm/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssm/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.183426 moto-4.1.8.dev6/moto/ssoadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssoadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssoadmin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssoadmin/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssoadmin/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssoadmin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/ssoadmin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.187426 moto-4.1.8.dev6/moto/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/stepfunctions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21993 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/stepfunctions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/stepfunctions/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/stepfunctions/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/stepfunctions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.187426 moto-4.1.8.dev6/moto/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/sts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/sts/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/sts/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/sts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/sts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.187426 moto-4.1.8.dev6/moto/support/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/support/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/support/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.187426 moto-4.1.8.dev6/moto/support/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   172189 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/support/resources/describe_trusted_advisor_checks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/support/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/support/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.187426 moto-4.1.8.dev6/moto/swf/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.191426 moto-4.1.8.dev6/moto/swf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/activity_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/decision_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/generic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/history_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30491 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/workflow_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/models/workflow_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21829 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/swf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.191426 moto-4.1.8.dev6/moto/textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/textract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/textract/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/textract/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/textract/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.191426 moto-4.1.8.dev6/moto/timestreamwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/timestreamwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/timestreamwrite/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/timestreamwrite/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/timestreamwrite/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/timestreamwrite/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.191426 moto-4.1.8.dev6/moto/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/transcribe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/transcribe/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/transcribe/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/transcribe/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.191426 moto-4.1.8.dev6/moto/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/aws_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/distutils_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/docker_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/tagging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.195426 moto-4.1.8.dev6/moto/wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/wafv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/wafv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/wafv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/wafv2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/wafv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.195426 moto-4.1.8.dev6/moto/xray/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/xray/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/xray/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/xray/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/xray/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/moto/xray/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.011414 moto-4.1.8.dev6/moto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-12 21:12:45.000000 moto-4.1.8.dev6/moto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66046 2023-04-12 21:12:45.000000 moto-4.1.8.dev6/moto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:12:45.000000 moto-4.1.8.dev6/moto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 21:12:45.000000 moto-4.1.8.dev6/moto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 21:12:45.000000 moto-4.1.8.dev6/moto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 21:12:45.000000 moto-4.1.8.dev6/moto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-12 21:12:46.299433 moto-4.1.8.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.195426 moto-4.1.8.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.195426 moto-4.1.8.dev6/tests/test_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.195426 moto-4.1.8.dev6/tests/test_acm/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/ca.srl
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com-bad.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acm/test_acm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.195426 moto-4.1.8.dev6/tests/test_acmpca/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acmpca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_acmpca/test_acmpca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.195426 moto-4.1.8.dev6/tests/test_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_amp/test_amp_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_amp/test_amp_rulegroupnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_amp/test_amp_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.199427 moto-4.1.8.dev6/tests/test_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.199427 moto-4.1.8.dev6/tests/test_apigateway/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/resources/petstore-swagger-v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/resources/test_api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/resources/test_api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/resources/test_api_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/resources/test_api_invalid_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/resources/test_deep_api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    91558 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_gatewayresponses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_importrestapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_putrestapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_vpclink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigateway/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.199427 moto-4.1.8.dev6/tests/test_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_reimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_apigatewayv2/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.203427 moto-4.1.8.dev6/tests/test_applicationautoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_applicationautoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_applicationautoscaling/test_applicationautoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_applicationautoscaling/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.203427 moto-4.1.8.dev6/tests/test_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_appsync/test_appsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_appsync/test_appsync_apikeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_appsync/test_appsync_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_appsync/test_appsync_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_appsync/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.203427 moto-4.1.8.dev6/tests/test_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_athena/test_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_athena/test_athena_server_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.203427 moto-4.1.8.dev6/tests/test_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48170 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_scheduledactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_launch_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_autoscaling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.207427 moto-4.1.8.dev6/tests/test_awslambda/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_awslambda_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_eventsourcemapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_function_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_lambda_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_awslambda/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.207427 moto-4.1.8.dev6/tests/test_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_compute_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34446 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_tags_job_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_tags_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_tags_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_batch_task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.207427 moto-4.1.8.dev6/tests/test_batch_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch_simple/test_batch_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch_simple/test_batch_compute_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_batch_simple/test_batch_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.207427 moto-4.1.8.dev6/tests/test_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_budgets/test_budgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_budgets/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_budgets/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.207427 moto-4.1.8.dev6/tests/test_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ce/test_ce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ce/test_ce_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.211427 moto-4.1.8.dev6/tests/test_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.211427 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/custom_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/ec2_classic_eip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/fn_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/route53_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/route53_roundrobin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/vpc_eip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/vpc_eni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_custom_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_depends_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_multi_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_nested_stacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85564 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69300 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_stack_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_stack_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_import_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_stack_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudformation/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.211427 moto-4.1.8.dev6/tests/test_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudfront/cloudfront_test_scaffolding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront_dist_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront_invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudfront/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudtrail/test_cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudtrail/test_cloudtrail_eventselectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudtrail/test_cloudtrail_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudtrail/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54006 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_codebuild/test_codebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_codecommit/test_codecommit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_codepipeline/test_codepipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidentity/test_cognitoidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidentity/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_cognitoidp/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161791 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidp/test_cognitoidp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidp/test_cognitoidp_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidp/test_cognitoidp_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_cognitoidp/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_comprehend/test_comprehend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.215427 moto-4.1.8.dev6/tests/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83099 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_config/test_config_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_config/test_config_rules_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_config/test_config_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.219428 moto-4.1.8.dev6/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_account_id_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_backenddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_decorator_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_environ_patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_importorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_instance_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_mock_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_mock_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_moto_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_request_mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_responses_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_url_base_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_url_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.219428 moto-4.1.8.dev6/tests/test_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_databrew/test_databrew_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_databrew/test_databrew_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_databrew/test_databrew_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_databrew/test_databrew_rulesets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.219428 moto-4.1.8.dev6/tests/test_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_datapipeline/test_datapipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_datapipeline/test_datapipeline_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_datapipeline/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.223428 moto-4.1.8.dev6/tests/test_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_datasync/test_datasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.223428 moto-4.1.8.dev6/tests/test_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dax/test_dax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dax/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.223428 moto-4.1.8.dev6/tests/test_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dms/test_dms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.223428 moto-4.1.8.dev6/tests/test_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ds/test_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ds/test_ds_ad_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ds/test_ds_microsoft_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ds/test_ds_simple_ad_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ds/test_ds_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.227429 moto-4.1.8.dev6/tests/test_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.227429 moto-4.1.8.dev6/tests/test_dynamodb/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/exceptions/test_key_length_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.227429 moto-4.1.8.dev6/tests/test_dynamodb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/models/test_key_condition_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   205697 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_batch_get_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_condition_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_consumedcapacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39804 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_table_with_range_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_table_without_range_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_update_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_update_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.227429 moto-4.1.8.dev6/tests/test_dynamodb_v20111205/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb_v20111205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43145 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb_v20111205/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodb_v20111205/test_servermode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.227429 moto-4.1.8.dev6/tests/test_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_dynamodbstreams/test_dynamodbstreams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.227429 moto-4.1.8.dev6/tests/test_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ebs/test_ebs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.235429 moto-4.1.8.dev6/tests/test_ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_account_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_amazon_dev_pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44698 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_ec2_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_ec2_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_ec2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_egress_only_igw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42808 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41728 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24744 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_flow_logs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_iam_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_instance_type_offerings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98932 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_placement_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_prefix_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_reserved_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40234 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65961 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_security_groups_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_spot_fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_spot_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_transit_gateway_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_transit_gateway_peering_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_virtual_private_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_vm_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_vm_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_vpc_endpoint_services_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_vpc_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45725 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2/test_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.235429 moto-4.1.8.dev6/tests/test_ec2instanceconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.235429 moto-4.1.8.dev6/tests/test_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91955 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecr/test_ecr_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecr/test_ecr_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecr/test_ecr_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecr/test_ecr_policy_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.239429 moto-4.1.8.dev6/tests/test_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/test_ecs_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122175 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/test_ecs_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/test_ecs_capacity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/test_ecs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/test_ecs_efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/test_ecs_task_def_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ecs/test_ecs_tasksets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.239429 moto-4.1.8.dev6/tests/test_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/junk_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_access_point_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_access_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_filesystem_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_lifecycle_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_mount_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_mount_target_security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_efs/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.239429 moto-4.1.8.dev6/tests/test_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52255 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_eks/test_eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_eks/test_eks_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_eks/test_eks_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_eks/test_eks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_eks/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.239429 moto-4.1.8.dev6/tests/test_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elasticache/test_elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elasticache/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.239429 moto-4.1.8.dev6/tests/test_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elasticbeanstalk/test_eb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.239429 moto-4.1.8.dev6/tests/test_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elastictranscoder/__init__
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elastictranscoder/test_elastictranscoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elastictranscoder/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.243430 moto-4.1.8.dev6/tests/test_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41073 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elb/test_elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elb/test_elb_availabilityzones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elb/test_elb_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elb/test_elb_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elb/test_elb_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.243430 moto-4.1.8.dev6/tests/test_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65284 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_listener_rule_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_listener_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_listener_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_set_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_elbv2/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.243430 moto-4.1.8.dev6/tests/test_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emr/test_emr_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emr/test_emr_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emr/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.243430 moto-4.1.8.dev6/tests/test_emrcontainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emrcontainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emrcontainers/test_emrcontainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emrcontainers/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.243430 moto-4.1.8.dev6/tests/test_emrserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emrserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emrserverless/test_emrserverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_emrserverless/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.243430 moto-4.1.8.dev6/tests/test_es/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_es/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_es/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.247430 moto-4.1.8.dev6/tests/test_events/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_events/test_event_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81682 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_events/test_events_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_events/test_events_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_events/test_events_lambdatriggers_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.247430 moto-4.1.8.dev6/tests/test_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_firehose/test_firehose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_firehose/test_firehose_destination_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_firehose/test_firehose_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_firehose/test_firehose_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_firehose/test_firehose_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_firehose/test_http_destinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.247430 moto-4.1.8.dev6/tests/test_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_forecast/test_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.247430 moto-4.1.8.dev6/tests/test_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glacier/test.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glacier/test_glacier_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glacier/test_glacier_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glacier/test_glacier_vaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glacier/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.247430 moto-4.1.8.dev6/tests/test_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.247430 moto-4.1.8.dev6/tests/test_glue/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/fixtures/datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/fixtures/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48038 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/test_datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/test_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/test_glue_job_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/test_partition_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47112 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_glue/test_schema_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.251430 moto-4.1.8.dev6/tests/test_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.251430 moto-4.1.8.dev6/tests/test_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_guardduty/test_guardduty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_guardduty/test_guardduty_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_guardduty/test_guardduty_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_guardduty/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.251430 moto-4.1.8.dev6/tests/test_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167646 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_access_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_account_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51772 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_password_last_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51265 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_iam_server_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iam/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.251430 moto-4.1.8.dev6/tests/test_identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_identitystore/test_identitystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.255430 moto-4.1.8.dev6/tests/test_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_ca_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_deprecate_thing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_domain_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_job_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_thing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_thing_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_iot_topic_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iot/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.255430 moto-4.1.8.dev6/tests/test_iotdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iotdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iotdata/test_iotdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_iotdata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.255430 moto-4.1.8.dev6/tests/test_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31019 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_stream_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_stream_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesis/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.255430 moto-4.1.8.dev6/tests/test_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesisvideo/test_kinesisvideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesisvideo/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.255430 moto-4.1.8.dev6/tests/test_kinesisvideoarchivedmedia/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesisvideoarchivedmedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kinesisvideoarchivedmedia/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.259431 moto-4.1.8.dev6/tests/test_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45373 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/test_kms_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/test_kms_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/test_kms_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/test_kms_policy_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_kms/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.259431 moto-4.1.8.dev6/tests/test_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_lakeformation/test_lakeformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.259431 moto-4.1.8.dev6/tests/test_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_logs/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47011 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_logs/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_logs/test_logs_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_logs/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.259431 moto-4.1.8.dev6/tests/test_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_proposals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.259431 moto-4.1.8.dev6/tests/test_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediaconnect/test_mediaconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediaconnect/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.259431 moto-4.1.8.dev6/tests/test_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_medialive/test_medialive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_medialive/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.259431 moto-4.1.8.dev6/tests/test_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediapackage/test_mediapackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediapackage/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediastore/test_mediastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediastore/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_mediastoredata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediastoredata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediastoredata/test_mediastoredata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mediastoredata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_meteringmarketplace/test_meteringmarketplace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_moto_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_moto_api/mock_random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/mock_random/test_mock_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_moto_api/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/recorder/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_moto_api/state_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/state_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_moto_api/state_manager/servermode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/state_manager/servermode/test_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/state_manager/test_batch_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/state_manager/test_managed_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_moto_api/state_manager/test_state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mq/test_mq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mq/test_mq_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mq/test_mq_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mq/test_mq_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_mq/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_neptune/test_cluster_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_neptune/test_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_neptune/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_neptune/test_global_clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.263431 moto-4.1.8.dev6/tests/test_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opensearch/test_domain_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opensearch/test_opensearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.267431 moto-4.1.8.dev6/tests/test_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opsworks/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opsworks/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opsworks/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_opsworks/test_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.267431 moto-4.1.8.dev6/tests/test_organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_organizations/organizations_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85363 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_organizations/test_organizations_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.267431 moto-4.1.8.dev6/tests/test_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_personalize/test_personalize_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.267431 moto-4.1.8.dev6/tests/test_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_pinpoint/test_pinpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_pinpoint/test_pinpoint_application_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_pinpoint/test_pinpoint_event_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.267431 moto-4.1.8.dev6/tests/test_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_polly/test_polly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_polly/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.267431 moto-4.1.8.dev6/tests/test_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_quicksight/test_quicksight_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_quicksight/test_quicksight_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_quicksight/test_quicksight_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.267431 moto-4.1.8.dev6/tests/test_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ram/test_ram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.271432 moto-4.1.8.dev6/tests/test_rds/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_db_cluster_param_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_db_cluster_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_global_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91218 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_rds_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_rds_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_rds_clusters_with_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_rds_event_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_rds_export_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rds/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.271432 moto-4.1.8.dev6/tests/test_rdsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rdsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rdsdata/test_rdsdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.271432 moto-4.1.8.dev6/tests/test_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshift/test_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshift/test_redshift_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshift/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.271432 moto-4.1.8.dev6/tests/test_redshiftdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshiftdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshiftdata/test_redshiftdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshiftdata/test_redshiftdata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_redshiftdata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.271432 moto-4.1.8.dev6/tests/test_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_rekognition/test_rekognition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.271432 moto-4.1.8.dev6/tests/test_resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_resourcegroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_resourcegroups/test_resourcegroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.271432 moto-4.1.8.dev6/tests/test_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_resourcegroupstaggingapi/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.275432 moto-4.1.8.dev6/tests/test_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_change_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52862 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_route53_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_route53_delegationsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_route53_healthchecks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_route53_query_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_route53_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.275432 moto-4.1.8.dev6/tests/test_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_rule_associations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.279432 moto-4.1.8.dev6/tests/test_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_multiple_accounts_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115801 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_classdecorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_copyobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_custom_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_file_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_lambda_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31026 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_object_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_storageclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.279432 moto-4.1.8.dev6/tests/test_s3bucket_path/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3bucket_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3bucket_path/test_s3bucket_path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3bucket_path/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.279432 moto-4.1.8.dev6/tests/test_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3control/test_s3control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3control/test_s3control_access_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3control/test_s3control_accesspoint_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3control/test_s3control_config_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_s3control/test_s3control_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.279432 moto-4.1.8.dev6/tests/test_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/cloudformation_test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20469 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24758 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_trial_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.283432 moto-4.1.8.dev6/tests/test_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_scheduler/test_schedule_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_scheduler/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_scheduler/test_scheduler_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_scheduler/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.283432 moto-4.1.8.dev6/tests/test_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sdb/test_sdb_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sdb/test_sdb_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sdb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.283432 moto-4.1.8.dev6/tests/test_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_secretsmanager/test_list_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_secretsmanager/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57270 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_secretsmanager/test_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33144 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_secretsmanager/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.283432 moto-4.1.8.dev6/tests/test_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicediscovery/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.283432 moto-4.1.8.dev6/tests/test_servicequotas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicequotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_servicequotas/test_servicequotas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.283432 moto-4.1.8.dev6/tests/test_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ses/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52328 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ses/test_ses_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ses/test_ses_sns_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ses/test_ses_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ses/test_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.283432 moto-4.1.8.dev6/tests/test_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_signer/test_signing_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_signer/test_signing_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.287433 moto-4.1.8.dev6/tests/test_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/test_application_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/test_publish_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42805 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/test_publishing_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/test_sns_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/test_subscriptions_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sns/test_topics_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.287433 moto-4.1.8.dev6/tests/test_special_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_special_cases/test_custom_amis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.287433 moto-4.1.8.dev6/tests/test_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sqs/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110801 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sqs/test_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sqs/test_sqs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sqs/test_sqs_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sqs/test_sqs_multiaccount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.287433 moto-4.1.8.dev6/tests/test_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71927 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_default_amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_doc_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_ec2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_ecs_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_maintenance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_parameterstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_ssm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.287433 moto-4.1.8.dev6/tests/test_ssm/test_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssm/test_templates/good.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.291433 moto-4.1.8.dev6/tests/test_ssoadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssoadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssoadmin/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_ssoadmin/test_ssoadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.291433 moto-4.1.8.dev6/tests/test_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_stepfunctions/test_stepfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_stepfunctions/test_stepfunctions_cloudformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.291433 moto-4.1.8.dev6/tests/test_sts/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sts/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sts/test_sts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_sts/test_sts_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.291433 moto-4.1.8.dev6/tests/test_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_support/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_support/test_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.291433 moto-4.1.8.dev6/tests/test_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.291433 moto-4.1.8.dev6/tests/test_swf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_activity_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_decision_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_generic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_history_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/models/test_workflow_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/tests/test_swf/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/test_activity_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/test_activity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21702 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/test_decision_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/test_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/test_workflow_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/responses/test_workflow_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_swf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/tests/test_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_textract/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_textract/test_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/tests/test_timestreamwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_timestreamwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_timestreamwrite/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_timestreamwrite/test_timestreamwrite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_timestreamwrite/test_timestreamwrite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_timestreamwrite/test_timestreamwrite_tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/tests/test_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_transcribe/test_transcribe_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_utilities/test_docker_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_utilities/test_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_utilities/test_tagging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_utilities/test_threaded_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/tests/test_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/test_wafv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/test_wafv2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/test_wafv2_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_wafv2/test_wafv2_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:12:46.295433 moto-4.1.8.dev6/tests/test_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_xray/test_xray_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-12 21:12:37.000000 moto-4.1.8.dev6/tests/test_xray/test_xray_client.py
```

### Comparing `moto-4.1.8.dev5/AUTHORS.md` & `moto-4.1.8.dev6/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/LICENSE` & `moto-4.1.8.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/MANIFEST.in` & `moto-4.1.8.dev6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/PKG-INFO` & `moto-4.1.8.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moto
-Version: 4.1.8.dev5
+Version: 4.1.8.dev6
 Home-page: https://github.com/getmoto/moto
 Author: Steve Pulec
 Author-email: "spulec@gmail.com"
 License: Apache License 2.0
 Project-URL: Documentation, http://docs.getmoto.org/en/latest/
 Project-URL: Issue tracker, https://github.com/getmoto/moto/issues
 Project-URL: Changelog, https://github.com/getmoto/moto/blob/master/CHANGELOG.md
```

### Comparing `moto-4.1.8.dev5/README.md` & `moto-4.1.8.dev6/README.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/__init__.py` & `moto-4.1.8.dev6/moto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
 mock_all = MockAll
 
 # import logging
 # logging.getLogger('boto').setLevel(logging.CRITICAL)
 
 __title__ = "moto"
-__version__ = "4.1.8.dev5"
+__version__ = "4.1.8.dev6"
 
 
 try:
     # Need to monkey-patch botocore requests back to underlying urllib3 classes
     from botocore.awsrequest import (
         HTTPSConnectionPool,
         HTTPConnectionPool,
```

### Comparing `moto-4.1.8.dev5/moto/acm/models.py` & `moto-4.1.8.dev6/moto/acm/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/acm/responses.py` & `moto-4.1.8.dev6/moto/acm/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/acmpca/models.py` & `moto-4.1.8.dev6/moto/acmpca/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/acmpca/responses.py` & `moto-4.1.8.dev6/moto/acmpca/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/amp/exceptions.py` & `moto-4.1.8.dev6/moto/amp/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/amp/models.py` & `moto-4.1.8.dev6/moto/amp/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/amp/responses.py` & `moto-4.1.8.dev6/moto/amp/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/amp/urls.py` & `moto-4.1.8.dev6/moto/amp/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigateway/exceptions.py` & `moto-4.1.8.dev6/moto/apigateway/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigateway/integration_parsers/aws_parser.py` & `moto-4.1.8.dev6/moto/apigateway/integration_parsers/aws_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigateway/integration_parsers/http_parser.py` & `moto-4.1.8.dev6/moto/apigateway/integration_parsers/http_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigateway/models.py` & `moto-4.1.8.dev6/moto/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigateway/responses.py` & `moto-4.1.8.dev6/moto/apigateway/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigateway/urls.py` & `moto-4.1.8.dev6/moto/apigateway/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigateway/utils.py` & `moto-4.1.8.dev6/moto/apigateway/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigatewayv2/exceptions.py` & `moto-4.1.8.dev6/moto/apigatewayv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigatewayv2/models.py` & `moto-4.1.8.dev6/moto/apigatewayv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigatewayv2/responses.py` & `moto-4.1.8.dev6/moto/apigatewayv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/apigatewayv2/urls.py` & `moto-4.1.8.dev6/moto/apigatewayv2/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/applicationautoscaling/models.py` & `moto-4.1.8.dev6/moto/applicationautoscaling/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/applicationautoscaling/responses.py` & `moto-4.1.8.dev6/moto/applicationautoscaling/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/appsync/models.py` & `moto-4.1.8.dev6/moto/appsync/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/appsync/responses.py` & `moto-4.1.8.dev6/moto/appsync/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/appsync/urls.py` & `moto-4.1.8.dev6/moto/appsync/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/athena/exceptions.py` & `moto-4.1.8.dev6/moto/athena/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/athena/models.py` & `moto-4.1.8.dev6/moto/athena/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/athena/responses.py` & `moto-4.1.8.dev6/moto/athena/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/autoscaling/exceptions.py` & `moto-4.1.8.dev6/moto/autoscaling/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/autoscaling/models.py` & `moto-4.1.8.dev6/moto/autoscaling/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/autoscaling/responses.py` & `moto-4.1.8.dev6/moto/autoscaling/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/awslambda/exceptions.py` & `moto-4.1.8.dev6/moto/awslambda/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/awslambda/models.py` & `moto-4.1.8.dev6/moto/awslambda/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/awslambda/policy.py` & `moto-4.1.8.dev6/moto/awslambda/policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/awslambda/responses.py` & `moto-4.1.8.dev6/moto/awslambda/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/awslambda/urls.py` & `moto-4.1.8.dev6/moto/awslambda/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/awslambda/utils.py` & `moto-4.1.8.dev6/moto/awslambda/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/backend_index.py` & `moto-4.1.8.dev6/moto/backend_index.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/backends.py` & `moto-4.1.8.dev6/moto/backends.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/batch/models.py` & `moto-4.1.8.dev6/moto/batch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/batch/responses.py` & `moto-4.1.8.dev6/moto/batch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/batch/urls.py` & `moto-4.1.8.dev6/moto/batch/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/batch/utils.py` & `moto-4.1.8.dev6/moto/batch/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/batch_simple/models.py` & `moto-4.1.8.dev6/moto/batch_simple/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/budgets/exceptions.py` & `moto-4.1.8.dev6/moto/budgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/budgets/models.py` & `moto-4.1.8.dev6/moto/budgets/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/budgets/responses.py` & `moto-4.1.8.dev6/moto/budgets/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ce/models.py` & `moto-4.1.8.dev6/moto/ce/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ce/responses.py` & `moto-4.1.8.dev6/moto/ce/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudformation/custom_model.py` & `moto-4.1.8.dev6/moto/cloudformation/custom_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudformation/exceptions.py` & `moto-4.1.8.dev6/moto/cloudformation/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudformation/models.py` & `moto-4.1.8.dev6/moto/cloudformation/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudformation/parsing.py` & `moto-4.1.8.dev6/moto/cloudformation/parsing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudformation/responses.py` & `moto-4.1.8.dev6/moto/cloudformation/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudformation/utils.py` & `moto-4.1.8.dev6/moto/cloudformation/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudfront/exceptions.py` & `moto-4.1.8.dev6/moto/cloudfront/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudfront/models.py` & `moto-4.1.8.dev6/moto/cloudfront/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudfront/responses.py` & `moto-4.1.8.dev6/moto/cloudfront/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudfront/urls.py` & `moto-4.1.8.dev6/moto/cloudfront/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudtrail/exceptions.py` & `moto-4.1.8.dev6/moto/cloudtrail/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudtrail/models.py` & `moto-4.1.8.dev6/moto/cloudtrail/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudtrail/responses.py` & `moto-4.1.8.dev6/moto/cloudtrail/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudwatch/exceptions.py` & `moto-4.1.8.dev6/moto/cloudwatch/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudwatch/models.py` & `moto-4.1.8.dev6/moto/cloudwatch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cloudwatch/responses.py` & `moto-4.1.8.dev6/moto/cloudwatch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codebuild/exceptions.py` & `moto-4.1.8.dev6/moto/codebuild/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codebuild/models.py` & `moto-4.1.8.dev6/moto/codebuild/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codebuild/responses.py` & `moto-4.1.8.dev6/moto/codebuild/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codecommit/exceptions.py` & `moto-4.1.8.dev6/moto/codecommit/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codecommit/models.py` & `moto-4.1.8.dev6/moto/codecommit/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codecommit/responses.py` & `moto-4.1.8.dev6/moto/codecommit/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codepipeline/exceptions.py` & `moto-4.1.8.dev6/moto/codepipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codepipeline/models.py` & `moto-4.1.8.dev6/moto/codepipeline/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/codepipeline/responses.py` & `moto-4.1.8.dev6/moto/codepipeline/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidentity/exceptions.py` & `moto-4.1.8.dev6/moto/cognitoidentity/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidentity/models.py` & `moto-4.1.8.dev6/moto/cognitoidentity/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidentity/responses.py` & `moto-4.1.8.dev6/moto/cognitoidentity/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidp/exceptions.py` & `moto-4.1.8.dev6/moto/cognitoidp/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidp/models.py` & `moto-4.1.8.dev6/moto/cognitoidp/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidp/resources/jwks-private.json` & `moto-4.1.8.dev6/moto/cognitoidp/resources/jwks-private.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidp/responses.py` & `moto-4.1.8.dev6/moto/cognitoidp/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/cognitoidp/utils.py` & `moto-4.1.8.dev6/moto/cognitoidp/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/comprehend/models.py` & `moto-4.1.8.dev6/moto/comprehend/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/comprehend/responses.py` & `moto-4.1.8.dev6/moto/comprehend/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/config/exceptions.py` & `moto-4.1.8.dev6/moto/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/config/models.py` & `moto-4.1.8.dev6/moto/config/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/config/resources/aws_managed_rules.json` & `moto-4.1.8.dev6/moto/config/resources/aws_managed_rules.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/config/responses.py` & `moto-4.1.8.dev6/moto/config/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/base_backend.py` & `moto-4.1.8.dev6/moto/core/base_backend.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/botocore_stubber.py` & `moto-4.1.8.dev6/moto/core/botocore_stubber.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/common_models.py` & `moto-4.1.8.dev6/moto/core/common_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/custom_responses_mock.py` & `moto-4.1.8.dev6/moto/core/custom_responses_mock.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/exceptions.py` & `moto-4.1.8.dev6/moto/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/models.py` & `moto-4.1.8.dev6/moto/core/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/responses.py` & `moto-4.1.8.dev6/moto/core/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/responses_custom_registry.py` & `moto-4.1.8.dev6/moto/core/responses_custom_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/core/utils.py` & `moto-4.1.8.dev6/moto/core/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/databrew/exceptions.py` & `moto-4.1.8.dev6/moto/databrew/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/databrew/models.py` & `moto-4.1.8.dev6/moto/databrew/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/databrew/responses.py` & `moto-4.1.8.dev6/moto/databrew/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/databrew/urls.py` & `moto-4.1.8.dev6/moto/databrew/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/datapipeline/models.py` & `moto-4.1.8.dev6/moto/datapipeline/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/datapipeline/responses.py` & `moto-4.1.8.dev6/moto/datapipeline/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/datapipeline/utils.py` & `moto-4.1.8.dev6/moto/datapipeline/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/datasync/models.py` & `moto-4.1.8.dev6/moto/datasync/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/datasync/responses.py` & `moto-4.1.8.dev6/moto/datasync/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dax/exceptions.py` & `moto-4.1.8.dev6/moto/dax/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dax/models.py` & `moto-4.1.8.dev6/moto/dax/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dax/responses.py` & `moto-4.1.8.dev6/moto/dax/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dms/exceptions.py` & `moto-4.1.8.dev6/moto/dms/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dms/models.py` & `moto-4.1.8.dev6/moto/dms/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dms/responses.py` & `moto-4.1.8.dev6/moto/dms/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dms/utils.py` & `moto-4.1.8.dev6/moto/dms/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ds/exceptions.py` & `moto-4.1.8.dev6/moto/ds/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ds/models.py` & `moto-4.1.8.dev6/moto/ds/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ds/responses.py` & `moto-4.1.8.dev6/moto/ds/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ds/validations.py` & `moto-4.1.8.dev6/moto/ds/validations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/comparisons.py` & `moto-4.1.8.dev6/moto/dynamodb/comparisons.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/exceptions.py` & `moto-4.1.8.dev6/moto/dynamodb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/models/__init__.py` & `moto-4.1.8.dev6/moto/dynamodb/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/models/dynamo_type.py` & `moto-4.1.8.dev6/moto/dynamodb/models/dynamo_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/models/table.py` & `moto-4.1.8.dev6/moto/dynamodb/models/table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/ast_nodes.py` & `moto-4.1.8.dev6/moto/dynamodb/parsing/ast_nodes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/executors.py` & `moto-4.1.8.dev6/moto/dynamodb/parsing/executors.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/expressions.py` & `moto-4.1.8.dev6/moto/dynamodb/parsing/expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/key_condition_expression.py` & `moto-4.1.8.dev6/moto/dynamodb/parsing/key_condition_expression.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/reserved_keywords.py` & `moto-4.1.8.dev6/moto/dynamodb/parsing/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/reserved_keywords.txt` & `moto-4.1.8.dev6/moto/dynamodb/parsing/reserved_keywords.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/tokens.py` & `moto-4.1.8.dev6/moto/dynamodb/parsing/tokens.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/parsing/validators.py` & `moto-4.1.8.dev6/moto/dynamodb/parsing/validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb/responses.py` & `moto-4.1.8.dev6/moto/dynamodb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb_v20111205/comparisons.py` & `moto-4.1.8.dev6/moto/dynamodb_v20111205/comparisons.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb_v20111205/models.py` & `moto-4.1.8.dev6/moto/dynamodb_v20111205/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodb_v20111205/responses.py` & `moto-4.1.8.dev6/moto/dynamodb_v20111205/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodbstreams/models.py` & `moto-4.1.8.dev6/moto/dynamodbstreams/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/dynamodbstreams/responses.py` & `moto-4.1.8.dev6/moto/dynamodbstreams/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ebs/models.py` & `moto-4.1.8.dev6/moto/ebs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ebs/responses.py` & `moto-4.1.8.dev6/moto/ebs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ebs/urls.py` & `moto-4.1.8.dev6/moto/ebs/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/exceptions.py` & `moto-4.1.8.dev6/moto/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/__init__.py` & `moto-4.1.8.dev6/moto/ec2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/amis.py` & `moto-4.1.8.dev6/moto/ec2/models/amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/availability_zones_and_regions.py` & `moto-4.1.8.dev6/moto/ec2/models/availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/carrier_gateways.py` & `moto-4.1.8.dev6/moto/ec2/models/carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/core.py` & `moto-4.1.8.dev6/moto/ec2/models/core.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/customer_gateways.py` & `moto-4.1.8.dev6/moto/ec2/models/customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/dhcp_options.py` & `moto-4.1.8.dev6/moto/ec2/models/dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/elastic_block_store.py` & `moto-4.1.8.dev6/moto/ec2/models/elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/elastic_ip_addresses.py` & `moto-4.1.8.dev6/moto/ec2/models/elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/elastic_network_interfaces.py` & `moto-4.1.8.dev6/moto/ec2/models/elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/fleets.py` & `moto-4.1.8.dev6/moto/ec2/models/fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/flow_logs.py` & `moto-4.1.8.dev6/moto/ec2/models/flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/hosts.py` & `moto-4.1.8.dev6/moto/ec2/models/hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/iam_instance_profile.py` & `moto-4.1.8.dev6/moto/ec2/models/iam_instance_profile.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/instance_types.py` & `moto-4.1.8.dev6/moto/ec2/models/instance_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/instances.py` & `moto-4.1.8.dev6/moto/ec2/models/instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/internet_gateways.py` & `moto-4.1.8.dev6/moto/ec2/models/internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/key_pairs.py` & `moto-4.1.8.dev6/moto/ec2/models/key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/launch_templates.py` & `moto-4.1.8.dev6/moto/ec2/models/launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/managed_prefixes.py` & `moto-4.1.8.dev6/moto/ec2/models/managed_prefixes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/nat_gateways.py` & `moto-4.1.8.dev6/moto/ec2/models/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/network_acls.py` & `moto-4.1.8.dev6/moto/ec2/models/network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/route_tables.py` & `moto-4.1.8.dev6/moto/ec2/models/route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/security_groups.py` & `moto-4.1.8.dev6/moto/ec2/models/security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/spot_requests.py` & `moto-4.1.8.dev6/moto/ec2/models/spot_requests.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/subnets.py` & `moto-4.1.8.dev6/moto/ec2/models/subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/tags.py` & `moto-4.1.8.dev6/moto/ec2/models/tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/transit_gateway.py` & `moto-4.1.8.dev6/moto/ec2/models/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/transit_gateway_attachments.py` & `moto-4.1.8.dev6/moto/ec2/models/transit_gateway_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/transit_gateway_route_tables.py` & `moto-4.1.8.dev6/moto/ec2/models/transit_gateway_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/vpc_peering_connections.py` & `moto-4.1.8.dev6/moto/ec2/models/vpc_peering_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/vpc_service_configuration.py` & `moto-4.1.8.dev6/moto/ec2/models/vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/vpcs.py` & `moto-4.1.8.dev6/moto/ec2/models/vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/vpn_connections.py` & `moto-4.1.8.dev6/moto/ec2/models/vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/models/vpn_gateway.py` & `moto-4.1.8.dev6/moto/ec2/models/vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/amis.json` & `moto-4.1.8.dev6/moto/ec2/resources/amis.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/af-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/me-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/me-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/af-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/me-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/me-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/instance_types.json` & `moto-4.1.8.dev6/moto/ec2/resources/instance_types.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/af-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-northeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-northeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-northeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-southeast-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-southeast-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ap-southeast-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/ca-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-central-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-north-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-south-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/eu-west-3.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/me-central-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/me-south-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/sa-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-east-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-east-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-west-1.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/resources/latest_amis/us-west-2.json` & `moto-4.1.8.dev6/moto/ec2/resources/latest_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/__init__.py` & `moto-4.1.8.dev6/moto/ec2/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/_base_response.py` & `moto-4.1.8.dev6/moto/ec2/responses/_base_response.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/account_attributes.py` & `moto-4.1.8.dev6/moto/ec2/responses/account_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/amis.py` & `moto-4.1.8.dev6/moto/ec2/responses/amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/availability_zones_and_regions.py` & `moto-4.1.8.dev6/moto/ec2/responses/availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/carrier_gateways.py` & `moto-4.1.8.dev6/moto/ec2/responses/carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/customer_gateways.py` & `moto-4.1.8.dev6/moto/ec2/responses/customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/dhcp_options.py` & `moto-4.1.8.dev6/moto/ec2/responses/dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/egress_only_internet_gateways.py` & `moto-4.1.8.dev6/moto/ec2/responses/egress_only_internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/elastic_block_store.py` & `moto-4.1.8.dev6/moto/ec2/responses/elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/elastic_ip_addresses.py` & `moto-4.1.8.dev6/moto/ec2/responses/elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/elastic_network_interfaces.py` & `moto-4.1.8.dev6/moto/ec2/responses/elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/fleets.py` & `moto-4.1.8.dev6/moto/ec2/responses/fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/flow_logs.py` & `moto-4.1.8.dev6/moto/ec2/responses/flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/general.py` & `moto-4.1.8.dev6/moto/ec2/responses/general.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/hosts.py` & `moto-4.1.8.dev6/moto/ec2/responses/hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/iam_instance_profiles.py` & `moto-4.1.8.dev6/moto/ec2/responses/iam_instance_profiles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/instances.py` & `moto-4.1.8.dev6/moto/ec2/responses/instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/internet_gateways.py` & `moto-4.1.8.dev6/moto/ec2/responses/internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/key_pairs.py` & `moto-4.1.8.dev6/moto/ec2/responses/key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/launch_templates.py` & `moto-4.1.8.dev6/moto/ec2/responses/launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/nat_gateways.py` & `moto-4.1.8.dev6/moto/ec2/responses/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/network_acls.py` & `moto-4.1.8.dev6/moto/ec2/responses/network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/reserved_instances.py` & `moto-4.1.8.dev6/moto/ec2/responses/reserved_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/route_tables.py` & `moto-4.1.8.dev6/moto/ec2/responses/route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/security_groups.py` & `moto-4.1.8.dev6/moto/ec2/responses/security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/settings.py` & `moto-4.1.8.dev6/moto/ec2/responses/settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/spot_fleets.py` & `moto-4.1.8.dev6/moto/ec2/responses/spot_fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/spot_instances.py` & `moto-4.1.8.dev6/moto/ec2/responses/spot_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/subnets.py` & `moto-4.1.8.dev6/moto/ec2/responses/subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/tags.py` & `moto-4.1.8.dev6/moto/ec2/responses/tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/transit_gateway_attachments.py` & `moto-4.1.8.dev6/moto/ec2/responses/transit_gateway_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/transit_gateway_route_tables.py` & `moto-4.1.8.dev6/moto/ec2/responses/transit_gateway_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/transit_gateways.py` & `moto-4.1.8.dev6/moto/ec2/responses/transit_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/virtual_private_gateways.py` & `moto-4.1.8.dev6/moto/ec2/responses/virtual_private_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/vpc_peering_connections.py` & `moto-4.1.8.dev6/moto/ec2/responses/vpc_peering_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/vpc_service_configuration.py` & `moto-4.1.8.dev6/moto/ec2/responses/vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/vpcs.py` & `moto-4.1.8.dev6/moto/ec2/responses/vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/vpn_connections.py` & `moto-4.1.8.dev6/moto/ec2/responses/vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/responses/windows.py` & `moto-4.1.8.dev6/moto/ec2/responses/windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2/utils.py` & `moto-4.1.8.dev6/moto/ec2/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ec2instanceconnect/responses.py` & `moto-4.1.8.dev6/moto/ec2instanceconnect/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ecr/exceptions.py` & `moto-4.1.8.dev6/moto/ecr/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ecr/models.py` & `moto-4.1.8.dev6/moto/ecr/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ecr/policy_validation.py` & `moto-4.1.8.dev6/moto/ecr/policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ecr/responses.py` & `moto-4.1.8.dev6/moto/ecr/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ecs/exceptions.py` & `moto-4.1.8.dev6/moto/ecs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ecs/models.py` & `moto-4.1.8.dev6/moto/ecs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ecs/responses.py` & `moto-4.1.8.dev6/moto/ecs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/efs/exceptions.py` & `moto-4.1.8.dev6/moto/efs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/efs/models.py` & `moto-4.1.8.dev6/moto/efs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/efs/responses.py` & `moto-4.1.8.dev6/moto/efs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/efs/urls.py` & `moto-4.1.8.dev6/moto/efs/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/eks/exceptions.py` & `moto-4.1.8.dev6/moto/eks/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/eks/models.py` & `moto-4.1.8.dev6/moto/eks/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/eks/responses.py` & `moto-4.1.8.dev6/moto/eks/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/eks/urls.py` & `moto-4.1.8.dev6/moto/eks/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/eks/utils.py` & `moto-4.1.8.dev6/moto/eks/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elasticache/exceptions.py` & `moto-4.1.8.dev6/moto/elasticache/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elasticache/models.py` & `moto-4.1.8.dev6/moto/elasticache/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elasticache/responses.py` & `moto-4.1.8.dev6/moto/elasticache/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elasticbeanstalk/models.py` & `moto-4.1.8.dev6/moto/elasticbeanstalk/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elasticbeanstalk/responses.py` & `moto-4.1.8.dev6/moto/elasticbeanstalk/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elastictranscoder/models.py` & `moto-4.1.8.dev6/moto/elastictranscoder/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elastictranscoder/responses.py` & `moto-4.1.8.dev6/moto/elastictranscoder/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elb/exceptions.py` & `moto-4.1.8.dev6/moto/elb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elb/models.py` & `moto-4.1.8.dev6/moto/elb/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elb/policies.py` & `moto-4.1.8.dev6/moto/elb/policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elb/responses.py` & `moto-4.1.8.dev6/moto/elb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elb/urls.py` & `moto-4.1.8.dev6/moto/elb/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elbv2/exceptions.py` & `moto-4.1.8.dev6/moto/elbv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elbv2/models.py` & `moto-4.1.8.dev6/moto/elbv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/elbv2/responses.py` & `moto-4.1.8.dev6/moto/elbv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emr/models.py` & `moto-4.1.8.dev6/moto/emr/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emr/responses.py` & `moto-4.1.8.dev6/moto/emr/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emr/utils.py` & `moto-4.1.8.dev6/moto/emr/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrcontainers/models.py` & `moto-4.1.8.dev6/moto/emrcontainers/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrcontainers/responses.py` & `moto-4.1.8.dev6/moto/emrcontainers/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrcontainers/urls.py` & `moto-4.1.8.dev6/moto/emrcontainers/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrcontainers/utils.py` & `moto-4.1.8.dev6/moto/emrcontainers/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrserverless/models.py` & `moto-4.1.8.dev6/moto/emrserverless/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrserverless/responses.py` & `moto-4.1.8.dev6/moto/emrserverless/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrserverless/urls.py` & `moto-4.1.8.dev6/moto/emrserverless/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/emrserverless/utils.py` & `moto-4.1.8.dev6/moto/emrserverless/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/es/exceptions.py` & `moto-4.1.8.dev6/moto/es/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/es/models.py` & `moto-4.1.8.dev6/moto/es/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/es/responses.py` & `moto-4.1.8.dev6/moto/es/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/es/urls.py` & `moto-4.1.8.dev6/moto/es/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/events/exceptions.py` & `moto-4.1.8.dev6/moto/events/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/events/models.py` & `moto-4.1.8.dev6/moto/events/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/events/notifications.py` & `moto-4.1.8.dev6/moto/events/notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/events/responses.py` & `moto-4.1.8.dev6/moto/events/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/firehose/exceptions.py` & `moto-4.1.8.dev6/moto/firehose/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/firehose/models.py` & `moto-4.1.8.dev6/moto/firehose/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/firehose/responses.py` & `moto-4.1.8.dev6/moto/firehose/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/forecast/exceptions.py` & `moto-4.1.8.dev6/moto/forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/forecast/models.py` & `moto-4.1.8.dev6/moto/forecast/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/forecast/responses.py` & `moto-4.1.8.dev6/moto/forecast/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glacier/models.py` & `moto-4.1.8.dev6/moto/glacier/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glacier/responses.py` & `moto-4.1.8.dev6/moto/glacier/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glacier/urls.py` & `moto-4.1.8.dev6/moto/glacier/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glue/exceptions.py` & `moto-4.1.8.dev6/moto/glue/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glue/glue_schema_registry_constants.py` & `moto-4.1.8.dev6/moto/glue/glue_schema_registry_constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glue/glue_schema_registry_utils.py` & `moto-4.1.8.dev6/moto/glue/glue_schema_registry_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glue/models.py` & `moto-4.1.8.dev6/moto/glue/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glue/responses.py` & `moto-4.1.8.dev6/moto/glue/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/glue/utils.py` & `moto-4.1.8.dev6/moto/glue/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/greengrass/exceptions.py` & `moto-4.1.8.dev6/moto/greengrass/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/greengrass/models.py` & `moto-4.1.8.dev6/moto/greengrass/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/greengrass/responses.py` & `moto-4.1.8.dev6/moto/greengrass/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/greengrass/urls.py` & `moto-4.1.8.dev6/moto/greengrass/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/guardduty/exceptions.py` & `moto-4.1.8.dev6/moto/guardduty/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/guardduty/models.py` & `moto-4.1.8.dev6/moto/guardduty/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/guardduty/responses.py` & `moto-4.1.8.dev6/moto/guardduty/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/guardduty/urls.py` & `moto-4.1.8.dev6/moto/guardduty/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/access_control.py` & `moto-4.1.8.dev6/moto/iam/access_control.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/aws_managed_policies.py` & `moto-4.1.8.dev6/moto/iam/aws_managed_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/config.py` & `moto-4.1.8.dev6/moto/iam/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/exceptions.py` & `moto-4.1.8.dev6/moto/iam/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/models.py` & `moto-4.1.8.dev6/moto/iam/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/policy_validation.py` & `moto-4.1.8.dev6/moto/iam/policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/responses.py` & `moto-4.1.8.dev6/moto/iam/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iam/utils.py` & `moto-4.1.8.dev6/moto/iam/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/identitystore/models.py` & `moto-4.1.8.dev6/moto/identitystore/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/identitystore/responses.py` & `moto-4.1.8.dev6/moto/identitystore/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/instance_metadata/responses.py` & `moto-4.1.8.dev6/moto/instance_metadata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iot/exceptions.py` & `moto-4.1.8.dev6/moto/iot/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iot/models.py` & `moto-4.1.8.dev6/moto/iot/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iot/responses.py` & `moto-4.1.8.dev6/moto/iot/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iot/urls.py` & `moto-4.1.8.dev6/moto/iot/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iotdata/exceptions.py` & `moto-4.1.8.dev6/moto/iotdata/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iotdata/models.py` & `moto-4.1.8.dev6/moto/iotdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/iotdata/responses.py` & `moto-4.1.8.dev6/moto/iotdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesis/exceptions.py` & `moto-4.1.8.dev6/moto/kinesis/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesis/models.py` & `moto-4.1.8.dev6/moto/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesis/responses.py` & `moto-4.1.8.dev6/moto/kinesis/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesis/urls.py` & `moto-4.1.8.dev6/moto/kinesis/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesis/utils.py` & `moto-4.1.8.dev6/moto/kinesis/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesisvideo/exceptions.py` & `moto-4.1.8.dev6/moto/kinesisvideo/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesisvideo/models.py` & `moto-4.1.8.dev6/moto/kinesisvideo/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesisvideo/responses.py` & `moto-4.1.8.dev6/moto/kinesisvideo/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/models.py` & `moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kinesisvideoarchivedmedia/responses.py` & `moto-4.1.8.dev6/moto/kinesisvideoarchivedmedia/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kms/exceptions.py` & `moto-4.1.8.dev6/moto/kms/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kms/models.py` & `moto-4.1.8.dev6/moto/kms/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kms/policy_validator.py` & `moto-4.1.8.dev6/moto/kms/policy_validator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kms/responses.py` & `moto-4.1.8.dev6/moto/kms/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/kms/utils.py` & `moto-4.1.8.dev6/moto/kms/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/lakeformation/models.py` & `moto-4.1.8.dev6/moto/lakeformation/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/lakeformation/responses.py` & `moto-4.1.8.dev6/moto/lakeformation/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/lakeformation/urls.py` & `moto-4.1.8.dev6/moto/lakeformation/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/logs/exceptions.py` & `moto-4.1.8.dev6/moto/logs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/logs/metric_filters.py` & `moto-4.1.8.dev6/moto/logs/metric_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/logs/models.py` & `moto-4.1.8.dev6/moto/logs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/logs/responses.py` & `moto-4.1.8.dev6/moto/logs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/logs/utils.py` & `moto-4.1.8.dev6/moto/logs/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/managedblockchain/exceptions.py` & `moto-4.1.8.dev6/moto/managedblockchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/managedblockchain/models.py` & `moto-4.1.8.dev6/moto/managedblockchain/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/managedblockchain/responses.py` & `moto-4.1.8.dev6/moto/managedblockchain/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/managedblockchain/urls.py` & `moto-4.1.8.dev6/moto/managedblockchain/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/managedblockchain/utils.py` & `moto-4.1.8.dev6/moto/managedblockchain/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediaconnect/models.py` & `moto-4.1.8.dev6/moto/mediaconnect/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediaconnect/responses.py` & `moto-4.1.8.dev6/moto/mediaconnect/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediaconnect/urls.py` & `moto-4.1.8.dev6/moto/mediaconnect/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/medialive/models.py` & `moto-4.1.8.dev6/moto/medialive/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/medialive/responses.py` & `moto-4.1.8.dev6/moto/medialive/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/medialive/urls.py` & `moto-4.1.8.dev6/moto/medialive/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediapackage/models.py` & `moto-4.1.8.dev6/moto/mediapackage/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediapackage/responses.py` & `moto-4.1.8.dev6/moto/mediapackage/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediastore/exceptions.py` & `moto-4.1.8.dev6/moto/mediastore/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediastore/models.py` & `moto-4.1.8.dev6/moto/mediastore/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediastore/responses.py` & `moto-4.1.8.dev6/moto/mediastore/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediastoredata/models.py` & `moto-4.1.8.dev6/moto/mediastoredata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mediastoredata/responses.py` & `moto-4.1.8.dev6/moto/mediastoredata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/meteringmarketplace/models.py` & `moto-4.1.8.dev6/moto/meteringmarketplace/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/meteringmarketplace/responses.py` & `moto-4.1.8.dev6/moto/meteringmarketplace/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/managed_state_model.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/managed_state_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/models.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/moto_random.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/moto_random.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/recorder/models.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/recorder/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/recorder/responses.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/recorder/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/responses.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/state_manager.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_api/_internal/urls.py` & `moto-4.1.8.dev6/moto/moto_api/_internal/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_server/templates/dashboard.html` & `moto-4.1.8.dev6/moto/moto_server/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_server/threaded_moto_server.py` & `moto-4.1.8.dev6/moto/moto_server/threaded_moto_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_server/utilities.py` & `moto-4.1.8.dev6/moto/moto_server/utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/moto_server/werkzeug_app.py` & `moto-4.1.8.dev6/moto/moto_server/werkzeug_app.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mq/configuration.py` & `moto-4.1.8.dev6/moto/mq/configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mq/exceptions.py` & `moto-4.1.8.dev6/moto/mq/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mq/models.py` & `moto-4.1.8.dev6/moto/mq/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mq/responses.py` & `moto-4.1.8.dev6/moto/mq/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/mq/urls.py` & `moto-4.1.8.dev6/moto/mq/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/neptune/exceptions.py` & `moto-4.1.8.dev6/moto/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/neptune/models.py` & `moto-4.1.8.dev6/moto/neptune/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/neptune/responses.py` & `moto-4.1.8.dev6/moto/neptune/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/opensearch/data.py` & `moto-4.1.8.dev6/moto/opensearch/data.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/opensearch/models.py` & `moto-4.1.8.dev6/moto/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/opensearch/responses.py` & `moto-4.1.8.dev6/moto/opensearch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/opsworks/models.py` & `moto-4.1.8.dev6/moto/opsworks/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/opsworks/responses.py` & `moto-4.1.8.dev6/moto/opsworks/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/organizations/exceptions.py` & `moto-4.1.8.dev6/moto/organizations/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/organizations/models.py` & `moto-4.1.8.dev6/moto/organizations/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/organizations/responses.py` & `moto-4.1.8.dev6/moto/organizations/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/organizations/utils.py` & `moto-4.1.8.dev6/moto/organizations/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/packages/boto/ec2/blockdevicemapping.py` & `moto-4.1.8.dev6/moto/packages/boto/ec2/blockdevicemapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/packages/boto/ec2/ec2object.py` & `moto-4.1.8.dev6/moto/packages/boto/ec2/ec2object.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/packages/boto/ec2/image.py` & `moto-4.1.8.dev6/moto/packages/boto/ec2/image.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/packages/boto/ec2/instance.py` & `moto-4.1.8.dev6/moto/packages/boto/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/packages/boto/ec2/instancetype.py` & `moto-4.1.8.dev6/moto/packages/boto/ec2/instancetype.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/packages/boto/ec2/tag.py` & `moto-4.1.8.dev6/moto/packages/boto/ec2/tag.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/packages/cfnresponse/cfnresponse.py` & `moto-4.1.8.dev6/moto/packages/cfnresponse/cfnresponse.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/personalize/models.py` & `moto-4.1.8.dev6/moto/personalize/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/personalize/responses.py` & `moto-4.1.8.dev6/moto/personalize/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/pinpoint/models.py` & `moto-4.1.8.dev6/moto/pinpoint/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/pinpoint/responses.py` & `moto-4.1.8.dev6/moto/pinpoint/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/pinpoint/urls.py` & `moto-4.1.8.dev6/moto/pinpoint/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/polly/models.py` & `moto-4.1.8.dev6/moto/polly/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/polly/resources.py` & `moto-4.1.8.dev6/moto/polly/resources.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/polly/responses.py` & `moto-4.1.8.dev6/moto/polly/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/quicksight/models.py` & `moto-4.1.8.dev6/moto/quicksight/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/quicksight/responses.py` & `moto-4.1.8.dev6/moto/quicksight/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/quicksight/urls.py` & `moto-4.1.8.dev6/moto/quicksight/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ram/exceptions.py` & `moto-4.1.8.dev6/moto/ram/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ram/models.py` & `moto-4.1.8.dev6/moto/ram/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ram/responses.py` & `moto-4.1.8.dev6/moto/ram/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/rds/exceptions.py` & `moto-4.1.8.dev6/moto/rds/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from jinja2 import Template
 from moto.core.exceptions import RESTError
 
 
 class RDSClientError(RESTError):
-    def __init__(self, code, message):
+    def __init__(self, code: str, message: str):
         super().__init__(error_type=code, message=message)
         template = Template(
             """
         <ErrorResponse>
             <Error>
               <Code>{{ code }}</Code>
               <Message>{{ message }}</Message>
@@ -16,176 +16,176 @@
             <RequestId>6876f774-7273-11e4-85dc-39e55ca848d1</RequestId>
         </ErrorResponse>"""
         )
         self.description = template.render(code=code, message=message)
 
 
 class DBInstanceNotFoundError(RDSClientError):
-    def __init__(self, database_identifier):
+    def __init__(self, database_identifier: str):
         super().__init__(
             "DBInstanceNotFound", f"DBInstance {database_identifier} not found."
         )
 
 
 class DBSnapshotNotFoundError(RDSClientError):
-    def __init__(self, snapshot_identifier):
+    def __init__(self, snapshot_identifier: str):
         super().__init__(
             "DBSnapshotNotFound", f"DBSnapshot {snapshot_identifier} not found."
         )
 
 
 class DBSecurityGroupNotFoundError(RDSClientError):
-    def __init__(self, security_group_name):
+    def __init__(self, security_group_name: str):
         super().__init__(
             "DBSecurityGroupNotFound",
             f"Security Group {security_group_name} not found.",
         )
 
 
 class DBSubnetGroupNotFoundError(RDSClientError):
     code = 404
 
-    def __init__(self, subnet_group_name):
+    def __init__(self, subnet_group_name: str):
         super().__init__(
             "DBSubnetGroupNotFoundFault", f"Subnet Group {subnet_group_name} not found."
         )
 
 
 class DBParameterGroupNotFoundError(RDSClientError):
-    def __init__(self, db_parameter_group_name):
+    def __init__(self, db_parameter_group_name: str):
         super().__init__(
             "DBParameterGroupNotFound",
             f"DB Parameter Group {db_parameter_group_name} not found.",
         )
 
 
 class DBClusterParameterGroupNotFoundError(RDSClientError):
-    def __init__(self, group_name):
+    def __init__(self, group_name: str):
         super().__init__(
             "DBParameterGroupNotFound",
             f"DBClusterParameterGroup not found: {group_name}",
         )
 
 
 class OptionGroupNotFoundFaultError(RDSClientError):
-    def __init__(self, option_group_name):
+    def __init__(self, option_group_name: str):
         super().__init__(
             "OptionGroupNotFoundFault",
             f"Specified OptionGroupName: {option_group_name} not found.",
         )
 
 
 class InvalidDBClusterStateFaultError(RDSClientError):
-    def __init__(self, database_identifier):
+    def __init__(self, database_identifier: str):
         super().__init__(
             "InvalidDBClusterStateFault",
             f"Invalid DB type, when trying to perform StopDBInstance on {database_identifier}e. See AWS RDS documentation on rds.stop_db_instance",
         )
 
 
 class InvalidDBInstanceStateError(RDSClientError):
-    def __init__(self, database_identifier, istate):
+    def __init__(self, database_identifier: str, istate: str):
         estate = (
             "in available state"
             if istate == "stop"
             else "stopped, it cannot be started"
         )
         super().__init__(
             "InvalidDBInstanceState", f"Instance {database_identifier} is not {estate}."
         )
 
 
 class SnapshotQuotaExceededError(RDSClientError):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(
             "SnapshotQuotaExceeded",
             "The request cannot be processed because it would exceed the maximum number of snapshots.",
         )
 
 
 class DBSnapshotAlreadyExistsError(RDSClientError):
-    def __init__(self, database_snapshot_identifier):
+    def __init__(self, database_snapshot_identifier: str):
         super().__init__(
             "DBSnapshotAlreadyExists",
             f"Cannot create the snapshot because a snapshot with the identifier {database_snapshot_identifier} already exists.",
         )
 
 
 class InvalidParameterValue(RDSClientError):
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidParameterValue", message)
 
 
 class InvalidParameterCombination(RDSClientError):
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidParameterCombination", message)
 
 
 class InvalidDBClusterStateFault(RDSClientError):
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidDBClusterStateFault", message)
 
 
 class DBClusterNotFoundError(RDSClientError):
-    def __init__(self, cluster_identifier):
+    def __init__(self, cluster_identifier: str):
         super().__init__(
             "DBClusterNotFoundFault", f"DBCluster {cluster_identifier} not found."
         )
 
 
 class DBClusterSnapshotNotFoundError(RDSClientError):
-    def __init__(self, snapshot_identifier):
+    def __init__(self, snapshot_identifier: str):
         super().__init__(
             "DBClusterSnapshotNotFoundFault",
             f"DBClusterSnapshot {snapshot_identifier} not found.",
         )
 
 
 class DBClusterSnapshotAlreadyExistsError(RDSClientError):
-    def __init__(self, database_snapshot_identifier):
+    def __init__(self, database_snapshot_identifier: str):
         super().__init__(
             "DBClusterSnapshotAlreadyExistsFault",
             f"Cannot create the snapshot because a snapshot with the identifier {database_snapshot_identifier} already exists.",
         )
 
 
 class ExportTaskAlreadyExistsError(RDSClientError):
-    def __init__(self, export_task_identifier):
+    def __init__(self, export_task_identifier: str):
         super().__init__(
             "ExportTaskAlreadyExistsFault",
             f"Cannot start export task because a task with the identifier {export_task_identifier} already exists.",
         )
 
 
 class ExportTaskNotFoundError(RDSClientError):
-    def __init__(self, export_task_identifier):
+    def __init__(self, export_task_identifier: str):
         super().__init__(
             "ExportTaskNotFoundFault",
             f"Cannot cancel export task because a task with the identifier {export_task_identifier} is not exist.",
         )
 
 
 class InvalidExportSourceStateError(RDSClientError):
-    def __init__(self, status):
+    def __init__(self, status: str):
         super().__init__(
             "InvalidExportSourceStateFault",
             f"Export source should be 'available' but current status is {status}.",
         )
 
 
 class SubscriptionAlreadyExistError(RDSClientError):
-    def __init__(self, subscription_name):
+    def __init__(self, subscription_name: str):
         super().__init__(
             "SubscriptionAlreadyExistFault",
             f"Subscription {subscription_name} already exists.",
         )
 
 
 class SubscriptionNotFoundError(RDSClientError):
-    def __init__(self, subscription_name):
+    def __init__(self, subscription_name: str):
         super().__init__(
             "SubscriptionNotFoundFault", f"Subscription {subscription_name} not found."
         )
 
 
 class InvalidGlobalClusterStateFault(RDSClientError):
     def __init__(self, arn: str):
```

### Comparing `moto-4.1.8.dev5/moto/rds/models.py` & `moto-4.1.8.dev6/moto/rds/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import string
 
 from collections import defaultdict
 from jinja2 import Template
 from re import compile as re_compile
 from collections import OrderedDict
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional, Iterable, Tuple, Union
 from moto.core import BaseBackend, BackendDict, BaseModel, CloudFormationModel
 from moto.core.utils import iso_8601_datetime_with_milliseconds
 from moto.ec2.models import ec2_backends
 from moto.moto_api._internal import mock_random as random
 from moto.neptune.models import neptune_backends, NeptuneBackend
 from moto.utilities.utils import load_resource
 from .exceptions import (
@@ -45,44 +45,44 @@
     apply_filter,
     merge_filters,
     validate_filters,
     valid_preferred_maintenance_window,
 )
 
 
-def find_cluster(cluster_arn):
+def find_cluster(cluster_arn: str) -> "Cluster":
     arn_parts = cluster_arn.split(":")
     region, account = arn_parts[3], arn_parts[4]
     return rds_backends[account][region].describe_db_clusters(cluster_arn)[0]
 
 
 class GlobalCluster(BaseModel):
     def __init__(
         self,
         account_id: str,
         global_cluster_identifier: str,
         engine: str,
-        engine_version,
-        storage_encrypted,
-        deletion_protection,
+        engine_version: Optional[str],
+        storage_encrypted: Optional[str],
+        deletion_protection: Optional[str],
     ):
         self.global_cluster_identifier = global_cluster_identifier
         self.global_cluster_resource_id = "cluster-" + random.get_random_hex(8)
         self.global_cluster_arn = (
             f"arn:aws:rds::{account_id}:global-cluster:{global_cluster_identifier}"
         )
         self.engine = engine
         self.engine_version = engine_version or "5.7.mysql_aurora.2.11.2"
         self.storage_encrypted = (
             storage_encrypted and storage_encrypted.lower() == "true"
         )
         self.deletion_protection = (
             deletion_protection and deletion_protection.lower() == "true"
         )
-        self.members = []
+        self.members: List[str] = []
 
     def to_xml(self) -> str:
         template = Template(
             """
           <GlobalClusterIdentifier>{{ cluster.global_cluster_identifier }}</GlobalClusterIdentifier>
           <GlobalClusterResourceId>{{ cluster.global_cluster_resource_id }}</GlobalClusterResourceId>
           <GlobalClusterArn>{{ cluster.global_cluster_arn }}</GlobalClusterArn>
@@ -108,23 +108,21 @@
     SUPPORTED_FILTERS = {
         "db-cluster-id": FilterDef(
             ["db_cluster_arn", "db_cluster_identifier"], "DB Cluster Identifiers"
         ),
         "engine": FilterDef(["engine"], "Engine Names"),
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any):
         self.db_name = kwargs.get("db_name")
         self.db_cluster_identifier = kwargs.get("db_cluster_identifier")
         self.db_cluster_instance_class = kwargs.get("db_cluster_instance_class")
         self.deletion_protection = kwargs.get("deletion_protection")
         self.engine = kwargs.get("engine")
-        self.engine_version = kwargs.get("engine_version")
-        if not self.engine_version:
-            self.engine_version = Cluster.default_engine_version(self.engine)
+        self.engine_version = kwargs.get("engine_version") or Cluster.default_engine_version(self.engine)  # type: ignore
         self.engine_mode = kwargs.get("engine_mode") or "provisioned"
         self.iops = kwargs.get("iops")
         self.kms_key_id = kwargs.get("kms_key_id")
         self.network_type = kwargs.get("network_type") or "IPV4"
         self.status = "active"
         self.account_id = kwargs.get("account_id")
         self.region_name = kwargs.get("region")
@@ -136,22 +134,22 @@
             self.copy_tags_to_snapshot = True
         self.storage_type = kwargs.get("storage_type")
         if self.storage_type is None:
             self.storage_type = Cluster.default_storage_type(iops=self.iops)
         self.allocated_storage = kwargs.get("allocated_storage")
         if self.allocated_storage is None:
             self.allocated_storage = Cluster.default_allocated_storage(
-                engine=self.engine, storage_type=self.storage_type
+                engine=self.engine, storage_type=self.storage_type  # type: ignore
             )
         self.master_username = kwargs.get("master_username")
         if not self.master_username:
             raise InvalidParameterValue(
                 "The parameter MasterUsername must be provided and must not be blank."
             )
-        self.master_user_password = kwargs.get("master_user_password")
+        self.master_user_password = kwargs.get("master_user_password")  # type: ignore
 
         self.availability_zones = kwargs.get("availability_zones")
         if not self.availability_zones:
             self.availability_zones = [
                 f"{self.region_name}a",
                 f"{self.region_name}b",
                 f"{self.region_name}c",
@@ -160,32 +158,32 @@
         self.subnet_group = kwargs.get("db_subnet_group_name") or "default"
         self.status = "creating"
         self.url_identifier = "".join(
             random.choice(string.ascii_lowercase + string.digits) for _ in range(12)
         )
         self.endpoint = f"{self.db_cluster_identifier}.cluster-{self.url_identifier}.{self.region_name}.rds.amazonaws.com"
         self.reader_endpoint = f"{self.db_cluster_identifier}.cluster-ro-{self.url_identifier}.{self.region_name}.rds.amazonaws.com"
-        self.port = kwargs.get("port")
+        self.port: int = kwargs.get("port")  # type: ignore
         if self.port is None:
             self.port = Cluster.default_port(self.engine)
         self.preferred_backup_window = "01:37-02:07"
         self.preferred_maintenance_window = "wed:02:40-wed:03:10"
         # This should default to the default security group
-        self.vpc_security_groups = []
+        self.vpc_security_groups: List[str] = []
         self.hosted_zone_id = "".join(
             random.choice(string.ascii_uppercase + string.digits) for _ in range(14)
         )
         self.resource_id = "cluster-" + "".join(
             random.choice(string.ascii_uppercase + string.digits) for _ in range(26)
         )
         self.tags = kwargs.get("tags", [])
         self.enabled_cloudwatch_logs_exports = (
             kwargs.get("enable_cloudwatch_logs_exports") or []
         )
-        self.enable_http_endpoint = kwargs.get("enable_http_endpoint")
+        self.enable_http_endpoint = kwargs.get("enable_http_endpoint")  # type: ignore
         self.earliest_restorable_time = iso_8601_datetime_with_milliseconds(
             datetime.datetime.utcnow()
         )
         self.scaling_configuration = kwargs.get("scaling_configuration")
         if not self.scaling_configuration and self.engine_mode == "serverless":
             # In AWS, this default configuration only shows up when the Cluster is in a ready state, so a few minutes after creation
             self.scaling_configuration = {
@@ -193,51 +191,51 @@
                 "max_capacity": 16,
                 "auto_pause": True,
                 "seconds_until_auto_pause": 300,
                 "timeout_action": "RollbackCapacityChange",
                 "seconds_before_timeout": 300,
             }
         self.global_cluster_identifier = kwargs.get("global_cluster_identifier")
-        self.cluster_members = list()
+        self.cluster_members: List[str] = list()
         self.replication_source_identifier = kwargs.get("replication_source_identifier")
-        self.read_replica_identifiers = list()
+        self.read_replica_identifiers: List[str] = list()
 
     @property
-    def is_multi_az(self):
+    def is_multi_az(self) -> bool:
         return (
             len(self.read_replica_identifiers) > 0
             or self.replication_source_identifier is not None
         )
 
     @property
-    def db_cluster_arn(self):
+    def db_cluster_arn(self) -> str:
         return f"arn:aws:rds:{self.region_name}:{self.account_id}:cluster:{self.db_cluster_identifier}"
 
     @property
-    def master_user_password(self):
+    def master_user_password(self) -> str:
         return self._master_user_password
 
     @master_user_password.setter
-    def master_user_password(self, val):
+    def master_user_password(self, val: str) -> None:
         if not val:
             raise InvalidParameterValue(
                 "The parameter MasterUserPassword must be provided and must not be blank."
             )
         if len(val) < 8:
             raise InvalidParameterValue(
                 "The parameter MasterUserPassword is not a valid password because it is shorter than 8 characters."
             )
         self._master_user_password = val
 
     @property
-    def enable_http_endpoint(self):
+    def enable_http_endpoint(self) -> bool:
         return self._enable_http_endpoint
 
     @enable_http_endpoint.setter
-    def enable_http_endpoint(self, val):
+    def enable_http_endpoint(self, val: Optional[bool]) -> None:
         # instead of raising an error on aws rds create-db-cluster commands with
         # incompatible configurations with enable_http_endpoint
         # (e.g. engine_mode is not set to "serverless"), the API
         # automatically sets the enable_http_endpoint parameter to False
         self._enable_http_endpoint = False
         if val is not None:
             if self.engine_mode == "serverless":
@@ -256,21 +254,21 @@
                 ]:
                     self._enable_http_endpoint = val
                 elif self.engine == "aurora" and self.engine_version in [
                     "5.6.mysql_aurora.1.22.5"
                 ]:
                     self._enable_http_endpoint = val
 
-    def get_cfg(self):
+    def get_cfg(self) -> Dict[str, Any]:
         cfg = self.__dict__
         cfg["master_user_password"] = cfg.pop("_master_user_password")
         cfg["enable_http_endpoint"] = cfg.pop("_enable_http_endpoint")
         return cfg
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<DBCluster>
               <AllocatedStorage>{{ cluster.allocated_storage }}</AllocatedStorage>
               <AvailabilityZones>
               {% for zone in cluster.availability_zones %}
                   <AvailabilityZone>{{ zone }}</AvailabilityZone>
               {% endfor %}
@@ -364,60 +362,60 @@
               {%- endif -%}
               {%- if cluster.replication_source_identifier -%}<ReplicationSourceIdentifier>{{ cluster.replication_source_identifier }}</ReplicationSourceIdentifier>{%- endif -%}
             </DBCluster>"""
         )
         return template.render(cluster=self)
 
     @staticmethod
-    def default_engine_version(engine):
+    def default_engine_version(engine: str) -> str:
         return {
             "aurora": "5.6.mysql_aurora.1.22.5",
             "aurora-mysql": "5.7.mysql_aurora.2.07.2",
             "aurora-postgresql": "12.7",
             "mysql": "8.0.23",
             "postgres": "13.4",
         }[engine]
 
     @staticmethod
-    def default_port(engine):
+    def default_port(engine: str) -> int:
         return {
             "aurora": 3306,
             "aurora-mysql": 3306,
             "aurora-postgresql": 5432,
             "mysql": 3306,
             "postgres": 5432,
         }[engine]
 
     @staticmethod
-    def default_storage_type(iops):
+    def default_storage_type(iops: Any) -> str:  # type: ignore[misc]
         if iops is None:
             return "gp2"
         else:
             return "io1"
 
     @staticmethod
-    def default_allocated_storage(engine, storage_type):
+    def default_allocated_storage(engine: str, storage_type: str) -> int:
         return {
             "aurora": {"gp2": 0, "io1": 0, "standard": 0},
             "aurora-mysql": {"gp2": 20, "io1": 100, "standard": 10},
             "aurora-postgresql": {"gp2": 20, "io1": 100, "standard": 10},
             "mysql": {"gp2": 20, "io1": 100, "standard": 5},
             "postgres": {"gp2": 20, "io1": 100, "standard": 5},
         }[engine][storage_type]
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
 
 class ClusterSnapshot(BaseModel):
 
     SUPPORTED_FILTERS = {
         "db-cluster-id": FilterDef(
@@ -427,28 +425,28 @@
         "db-cluster-snapshot-id": FilterDef(
             ["snapshot_id"], "DB Cluster Snapshot Identifiers"
         ),
         "snapshot-type": FilterDef(None, "Snapshot Types"),
         "engine": FilterDef(["cluster.engine"], "Engine Names"),
     }
 
-    def __init__(self, cluster, snapshot_id, tags):
+    def __init__(self, cluster: Cluster, snapshot_id: str, tags: List[Dict[str, str]]):
         self.cluster = cluster
         self.snapshot_id = snapshot_id
         self.tags = tags
         self.status = "available"
         self.created_at = iso_8601_datetime_with_milliseconds(
             datetime.datetime.utcnow()
         )
 
     @property
-    def snapshot_arn(self):
+    def snapshot_arn(self) -> str:
         return f"arn:aws:rds:{self.cluster.region_name}:{self.cluster.account_id}:cluster-snapshot:{self.snapshot_id}"
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """
             <DBClusterSnapshot>
                 <DBClusterSnapshotIdentifier>{{ snapshot.snapshot_id }}</DBClusterSnapshotIdentifier>
                 <SnapshotCreateTime>{{ snapshot.created_at }}</SnapshotCreateTime>
                 <DBClusterIdentifier>{{ cluster.db_cluster_identifier }}</DBClusterIdentifier>
                 <ClusterCreateTime>{{ snapshot.created_at }}</ClusterCreateTime>
@@ -470,24 +468,24 @@
                 <Timezone></Timezone>
                 <LicenseModel>{{ cluster.license_model }}</LicenseModel>
             </DBClusterSnapshot>
             """
         )
         return template.render(snapshot=self, cluster=self.cluster)
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
 
 class Database(CloudFormationModel):
 
     SUPPORTED_FILTERS = {
         "db-cluster-id": FilterDef(["db_cluster_identifier"], "DB Cluster Identifiers"),
@@ -508,20 +506,20 @@
         "sqlserver-ee": "11.00.2100.60.v1",
         "sqlserver-se": "11.00.2100.60.v1",
         "sqlserver-ex": "11.00.2100.60.v1",
         "sqlserver-web": "11.00.2100.60.v1",
         "postgres": "9.3.3",
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any):
         self.status = "available"
         self.is_replica = False
-        self.replicas = []
-        self.account_id = kwargs.get("account_id")
-        self.region_name = kwargs.get("region")
+        self.replicas: List[str] = []
+        self.account_id: str = kwargs["account_id"]
+        self.region_name: str = kwargs["region"]
         self.engine = kwargs.get("engine")
         self.engine_version = kwargs.get("engine_version", None)
         if not self.engine_version and self.engine in self.default_engine_versions:
             self.engine_version = self.default_engine_versions[self.engine]
         self.iops = kwargs.get("iops")
         self.storage_encrypted = kwargs.get("storage_encrypted", False)
         if self.storage_encrypted:
@@ -535,25 +533,25 @@
         self.master_user_password = kwargs.get("master_user_password")
         self.auto_minor_version_upgrade = kwargs.get("auto_minor_version_upgrade")
         if self.auto_minor_version_upgrade is None:
             self.auto_minor_version_upgrade = True
         self.allocated_storage = kwargs.get("allocated_storage")
         if self.allocated_storage is None:
             self.allocated_storage = Database.default_allocated_storage(
-                engine=self.engine, storage_type=self.storage_type
+                engine=self.engine, storage_type=self.storage_type  # type: ignore
             )
-        self.db_cluster_identifier = kwargs.get("db_cluster_identifier")
+        self.db_cluster_identifier: Optional[str] = kwargs.get("db_cluster_identifier")
         self.db_instance_identifier = kwargs.get("db_instance_identifier")
-        self.source_db_identifier = kwargs.get(
+        self.source_db_identifier: Optional[str] = kwargs.get(
             "source_db_ide.db_cluster_identifierntifier"
         )
         self.db_instance_class = kwargs.get("db_instance_class")
         self.port = kwargs.get("port")
         if self.port is None:
-            self.port = Database.default_port(self.engine)
+            self.port = Database.default_port(self.engine)  # type: ignore
         self.db_instance_identifier = kwargs.get("db_instance_identifier")
         self.db_name = kwargs.get("db_name")
         self.instance_create_time = iso_8601_datetime_with_milliseconds(
             datetime.datetime.now()
         )
         self.publicly_accessible = kwargs.get("publicly_accessible")
         if self.publicly_accessible is None:
@@ -619,60 +617,60 @@
         self.tags = kwargs.get("tags", [])
         self.deletion_protection = kwargs.get("deletion_protection", False)
         self.enabled_cloudwatch_logs_exports = (
             kwargs.get("enable_cloudwatch_logs_exports") or []
         )
 
     @property
-    def db_instance_arn(self):
+    def db_instance_arn(self) -> str:
         return f"arn:aws:rds:{self.region_name}:{self.account_id}:db:{self.db_instance_identifier}"
 
     @property
-    def physical_resource_id(self):
+    def physical_resource_id(self) -> Optional[str]:
         return self.db_instance_identifier
 
-    def db_parameter_groups(self):
+    def db_parameter_groups(self) -> List["DBParameterGroup"]:
         if not self.db_parameter_group_name or self.is_default_parameter_group(
             self.db_parameter_group_name
         ):
             (
                 db_family,
                 db_parameter_group_name,
             ) = self.default_db_parameter_group_details()
             description = f"Default parameter group for {db_family}"
             return [
                 DBParameterGroup(
                     account_id=self.account_id,
                     name=db_parameter_group_name,
                     family=db_family,
                     description=description,
-                    tags={},
+                    tags=[],
                     region=self.region_name,
                 )
             ]
         else:
             backend = rds_backends[self.account_id][self.region_name]
             if self.db_parameter_group_name not in backend.db_parameter_groups:
                 raise DBParameterGroupNotFoundError(self.db_parameter_group_name)
 
             return [backend.db_parameter_groups[self.db_parameter_group_name]]
 
-    def is_default_parameter_group(self, param_group_name):
-        return param_group_name.startswith(f"default.{self.engine.lower()}")
+    def is_default_parameter_group(self, param_group_name: str) -> bool:
+        return param_group_name.startswith(f"default.{self.engine.lower()}")  # type: ignore
 
-    def default_db_parameter_group_details(self):
+    def default_db_parameter_group_details(self) -> Tuple[Optional[str], Optional[str]]:
         if not self.engine_version:
             return (None, None)
 
         minor_engine_version = ".".join(str(self.engine_version).rsplit(".")[:-1])
-        db_family = f"{self.engine.lower()}{minor_engine_version}"
+        db_family = f"{self.engine.lower()}{minor_engine_version}"  # type: ignore
 
         return db_family, f"default.{db_family}"
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<DBInstance>
               <AvailabilityZone>{{ database.availability_zone }}</AvailabilityZone>
               <BackupRetentionPeriod>{{ database.backup_retention_period }}</BackupRetentionPeriod>
               <DBInstanceStatus>{{ database.status }}</DBInstanceStatus>
               {% if database.db_name %}<DBName>{{ database.db_name }}</DBName>{% endif %}
               <MultiAZ>{{ 'true' if database.multi_az else 'false' }}</MultiAZ>
@@ -791,52 +789,52 @@
               </TagList>
               <DeletionProtection>{{ 'true' if database.deletion_protection else 'false' }}</DeletionProtection>
             </DBInstance>"""
         )
         return template.render(database=self)
 
     @property
-    def address(self):
+    def address(self) -> str:
         return f"{self.db_instance_identifier}.aaaaaaaaaa.{self.region_name}.rds.amazonaws.com"
 
-    def add_replica(self, replica):
+    def add_replica(self, replica: "Database") -> None:
         if self.region_name != replica.region_name:
             # Cross Region replica
             self.replicas.append(replica.db_instance_arn)
         else:
-            self.replicas.append(replica.db_instance_identifier)
+            self.replicas.append(replica.db_instance_identifier)  # type: ignore
 
-    def remove_replica(self, replica):
-        self.replicas.remove(replica.db_instance_identifier)
+    def remove_replica(self, replica: "Database") -> None:
+        self.replicas.remove(replica.db_instance_identifier)  # type: ignore
 
-    def set_as_replica(self):
+    def set_as_replica(self) -> None:
         self.is_replica = True
         self.replicas = []
 
-    def update(self, db_kwargs):
+    def update(self, db_kwargs: Dict[str, Any]) -> None:
         for key, value in db_kwargs.items():
             if value is not None:
                 setattr(self, key, value)
 
     @classmethod
-    def has_cfn_attr(cls, attr):
+    def has_cfn_attr(cls, attr: str) -> bool:
         return attr in ["Endpoint.Address", "Endpoint.Port"]
 
-    def get_cfn_attribute(self, attribute_name):
+    def get_cfn_attribute(self, attribute_name: str) -> Any:
         # Local import to avoid circular dependency with cloudformation.parsing
         from moto.cloudformation.exceptions import UnformattedGetAttTemplateException
 
         if attribute_name == "Endpoint.Address":
             return self.address
         elif attribute_name == "Endpoint.Port":
             return self.port
         raise UnformattedGetAttTemplateException()
 
     @staticmethod
-    def default_port(engine):
+    def default_port(engine: str) -> int:
         return {
             "aurora": 3306,
             "aurora-mysql": 3306,
             "aurora-postgresql": 5432,
             "mysql": 3306,
             "mariadb": 3306,
             "postgres": 5432,
@@ -847,22 +845,22 @@
             "sqlserver-ee": 1433,
             "sqlserver-ex": 1433,
             "sqlserver-se": 1433,
             "sqlserver-web": 1433,
         }[engine]
 
     @staticmethod
-    def default_storage_type(iops):
+    def default_storage_type(iops: Any) -> str:  # type: ignore[misc]
         if iops is None:
             return "gp2"
         else:
             return "io1"
 
     @staticmethod
-    def default_allocated_storage(engine, storage_type):
+    def default_allocated_storage(engine: str, storage_type: str) -> int:
         return {
             "aurora": {"gp2": 0, "io1": 0, "standard": 0},
             "aurora-mysql": {"gp2": 20, "io1": 100, "standard": 10},
             "aurora-postgresql": {"gp2": 20, "io1": 100, "standard": 10},
             "mysql": {"gp2": 20, "io1": 100, "standard": 5},
             "mariadb": {"gp2": 20, "io1": 100, "standard": 5},
             "postgres": {"gp2": 20, "io1": 100, "standard": 5},
@@ -873,26 +871,31 @@
             "sqlserver-ee": {"gp2": 200, "io1": 200, "standard": 200},
             "sqlserver-ex": {"gp2": 20, "io1": 100, "standard": 20},
             "sqlserver-se": {"gp2": 200, "io1": 200, "standard": 200},
             "sqlserver-web": {"gp2": 20, "io1": 100, "standard": 20},
         }[engine][storage_type]
 
     @staticmethod
-    def cloudformation_name_type():
+    def cloudformation_name_type() -> str:
         return "DBInstanceIdentifier"
 
     @staticmethod
-    def cloudformation_type():
+    def cloudformation_type() -> str:
         # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-rds-dbinstance.html
         return "AWS::RDS::DBInstance"
 
     @classmethod
-    def create_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name, **kwargs
-    ):
+    def create_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+        **kwargs: Any,
+    ) -> "Database":
         properties = cloudformation_json["Properties"]
 
         db_security_groups = properties.get("DBSecurityGroups")
         if not db_security_groups:
             db_security_groups = []
         security_groups = [group.group_name for group in db_security_groups]
         db_subnet_group = properties.get("DBSubnetGroupName")
@@ -938,15 +941,15 @@
             # Replica
             db_kwargs["source_db_identifier"] = source_db_identifier
             database = rds_backend.create_db_instance_read_replica(db_kwargs)
         else:
             database = rds_backend.create_db_instance(db_kwargs)
         return database
 
-    def to_json(self):
+    def to_json(self) -> str:
         template = Template(
             """{
         "AllocatedStorage": 10,
         "AutoMinorVersionUpgrade": "{{ database.auto_minor_version_upgrade }}",
         "AvailabilityZone": "{{ database.availability_zone }}",
         "BackupRetentionPeriod": "{{ database.backup_retention_period }}",
         "CharacterSetName": {%- if database.character_set_name -%}{{ database.character_set_name }}{%- else %} null{%- endif -%},
@@ -1014,27 +1017,27 @@
             {% endfor %}
         ],
         "DBInstanceArn": "{{ database.db_instance_arn }}"
       }"""
         )
         return template.render(database=self)
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
-    def delete(self, account_id, region_name):
+    def delete(self, account_id: str, region_name: str) -> None:
         backend = rds_backends[account_id][region_name]
         backend.delete_db_instance(self.db_instance_identifier)
 
 
 class DatabaseSnapshot(BaseModel):
 
     SUPPORTED_FILTERS = {
@@ -1044,26 +1047,28 @@
         ),
         "db-snapshot-id": FilterDef(["snapshot_id"], "DB Snapshot Identifiers"),
         "dbi-resource-id": FilterDef(["database.dbi_resource_id"], "Dbi Resource Ids"),
         "snapshot-type": FilterDef(None, "Snapshot Types"),
         "engine": FilterDef(["database.engine"], "Engine Names"),
     }
 
-    def __init__(self, database, snapshot_id, tags):
+    def __init__(
+        self, database: Database, snapshot_id: str, tags: List[Dict[str, str]]
+    ):
         self.database = database
         self.snapshot_id = snapshot_id
         self.tags = tags
         self.status = "available"
         self.created_at = iso_8601_datetime_with_milliseconds(datetime.datetime.now())
 
     @property
-    def snapshot_arn(self):
+    def snapshot_arn(self) -> str:
         return f"arn:aws:rds:{self.database.region_name}:{self.database.account_id}:snapshot:{self.snapshot_id}"
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<DBSnapshot>
               <DBSnapshotIdentifier>{{ snapshot.snapshot_id }}</DBSnapshotIdentifier>
               <DBInstanceIdentifier>{{ database.db_instance_identifier }}</DBInstanceIdentifier>
               <DbiResourceId>{{ database.dbi_resource_id }}</DbiResourceId>
               <SnapshotCreateTime>{{ snapshot.created_at }}</SnapshotCreateTime>
               <Engine>{{ database.engine }}</Engine>
@@ -1098,43 +1103,45 @@
               <DBSnapshotArn>{{ snapshot.snapshot_arn }}</DBSnapshotArn>
               <Timezone></Timezone>
               <IAMDatabaseAuthenticationEnabled>{{ database.enable_iam_database_authentication|lower }}</IAMDatabaseAuthenticationEnabled>
             </DBSnapshot>"""
         )
         return template.render(snapshot=self, database=self.database)
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
 
 class ExportTask(BaseModel):
-    def __init__(self, snapshot, kwargs):
+    def __init__(
+        self, snapshot: Union[DatabaseSnapshot, ClusterSnapshot], kwargs: Dict[str, Any]
+    ):
         self.snapshot = snapshot
 
         self.export_task_identifier = kwargs.get("export_task_identifier")
         self.kms_key_id = kwargs.get("kms_key_id", "default_kms_key_id")
         self.source_arn = kwargs.get("source_arn")
         self.iam_role_arn = kwargs.get("iam_role_arn")
         self.s3_bucket_name = kwargs.get("s3_bucket_name")
         self.s3_prefix = kwargs.get("s3_prefix", "")
         self.export_only = kwargs.get("export_only", [])
 
         self.status = "complete"
         self.created_at = iso_8601_datetime_with_milliseconds(datetime.datetime.now())
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """
             <ExportTaskIdentifier>{{ task.export_task_identifier }}</ExportTaskIdentifier>
             <SourceArn>{{ snapshot.snapshot_arn }}</SourceArn>
             <TaskStartTime>{{ task.created_at }}</TaskStartTime>
             <TaskEndTime>{{ task.created_at }}</TaskEndTime>
             <SnapshotTime>{{ snapshot.created_at }}</SnapshotTime>
@@ -1156,33 +1163,33 @@
             <WarningMessage></WarningMessage>
             """
         )
         return template.render(task=self, snapshot=self.snapshot)
 
 
 class EventSubscription(BaseModel):
-    def __init__(self, kwargs):
+    def __init__(self, kwargs: Dict[str, Any]):
         self.subscription_name = kwargs.get("subscription_name")
         self.sns_topic_arn = kwargs.get("sns_topic_arn")
         self.source_type = kwargs.get("source_type")
         self.event_categories = kwargs.get("event_categories", [])
         self.source_ids = kwargs.get("source_ids", [])
         self.enabled = kwargs.get("enabled", True)
         self.tags = kwargs.get("tags", True)
 
         self.region_name = ""
         self.customer_aws_id = kwargs["account_id"]
         self.status = "active"
         self.created_at = iso_8601_datetime_with_milliseconds(datetime.datetime.now())
 
     @property
-    def es_arn(self):
+    def es_arn(self) -> str:
         return f"arn:aws:rds:{self.region_name}:{self.customer_aws_id}:es:{self.subscription_name}"
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """
             <EventSubscription>
               <CustomerAwsId>{{ subscription.customer_aws_id }}</CustomerAwsId>
               <CustSubscriptionId>{{ subscription.subscription_name }}</CustSubscriptionId>
               <SnsTopicArn>{{ subscription.sns_topic_arn }}</SnsTopicArn>
               <SubscriptionCreationTime>{{ subscription.created_at }}</SubscriptionCreationTime>
@@ -1206,39 +1213,45 @@
               {%- endfor -%}
               </TagList>
             </EventSubscription>
             """
         )
         return template.render(subscription=self)
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
 
 class SecurityGroup(CloudFormationModel):
-    def __init__(self, account_id, group_name, description, tags):
+    def __init__(
+        self,
+        account_id: str,
+        group_name: str,
+        description: str,
+        tags: List[Dict[str, str]],
+    ):
         self.group_name = group_name
         self.description = description
         self.status = "authorized"
-        self.ip_ranges = []
-        self.ec2_security_groups = []
+        self.ip_ranges: List[Any] = []
+        self.ec2_security_groups: List[Any] = []
         self.tags = tags
         self.owner_id = account_id
         self.vpc_id = None
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<DBSecurityGroup>
             <EC2SecurityGroups>
             {% for security_group in security_group.ec2_security_groups %}
                 <EC2SecurityGroup>
                     <EC2SecurityGroupId>{{ security_group.id }}</EC2SecurityGroupId>
                     <EC2SecurityGroupName>{{ security_group.name }}</EC2SecurityGroupName>
@@ -1259,15 +1272,15 @@
             </IPRanges>
             <OwnerId>{{ security_group.ownder_id }}</OwnerId>
             <DBSecurityGroupName>{{ security_group.group_name }}</DBSecurityGroupName>
         </DBSecurityGroup>"""
         )
         return template.render(security_group=self)
 
-    def to_json(self):
+    def to_json(self) -> str:
         template = Template(
             """{
             "DBSecurityGroupDescription": "{{ security_group.description }}",
             "DBSecurityGroupName": "{{ security_group.group_name }}",
             "EC2SecurityGroups": {{ security_group.ec2_security_groups }},
             "IPRanges": [{%- for ip in security_group.ip_ranges -%}
                          {%- if loop.index != 1 -%},{%- endif -%}
@@ -1276,33 +1289,38 @@
                         ],
             "OwnerId": "{{ security_group.owner_id }}",
             "VpcId": "{{ security_group.vpc_id }}"
         }"""
         )
         return template.render(security_group=self)
 
-    def authorize_cidr(self, cidr_ip):
+    def authorize_cidr(self, cidr_ip: str) -> None:
         self.ip_ranges.append(cidr_ip)
 
-    def authorize_security_group(self, security_group):
+    def authorize_security_group(self, security_group: str) -> None:
         self.ec2_security_groups.append(security_group)
 
     @staticmethod
-    def cloudformation_name_type():
-        return None
+    def cloudformation_name_type() -> str:
+        return ""
 
     @staticmethod
-    def cloudformation_type():
+    def cloudformation_type() -> str:
         # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-rds-dbsecuritygroup.html
         return "AWS::RDS::DBSecurityGroup"
 
     @classmethod
-    def create_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name, **kwargs
-    ):
+    def create_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+        **kwargs: Any,
+    ) -> "SecurityGroup":
         properties = cloudformation_json["Properties"]
         group_name = resource_name.lower()
         description = properties["GroupDescription"]
         security_group_ingress_rules = properties.get("DBSecurityGroupIngress", [])
         tags = properties.get("Tags")
 
         ec2_backend = ec2_backends[account_id][region_name]
@@ -1318,47 +1336,55 @@
                     subnet = ec2_backend.get_security_group_from_name(ingress_value)
                     security_group.authorize_security_group(subnet)
                 elif ingress_type == "EC2SecurityGroupId":
                     subnet = ec2_backend.get_security_group_from_id(ingress_value)
                     security_group.authorize_security_group(subnet)
         return security_group
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
-    def delete(self, account_id, region_name):
+    def delete(self, account_id: str, region_name: str) -> None:
         backend = rds_backends[account_id][region_name]
         backend.delete_security_group(self.group_name)
 
 
 class SubnetGroup(CloudFormationModel):
-    def __init__(self, subnet_name, description, subnets, tags, region, account_id):
+    def __init__(
+        self,
+        subnet_name: str,
+        description: str,
+        subnets: List[Any],
+        tags: List[Dict[str, str]],
+        region: str,
+        account_id: str,
+    ):
         self.subnet_name = subnet_name
         self.description = description
         self.subnets = subnets
         self.status = "Complete"
         self.tags = tags
         self.vpc_id = self.subnets[0].vpc_id
         self.region = region
         self.account_id = account_id
 
     @property
-    def sg_arn(self):
+    def sg_arn(self) -> str:
         return f"arn:aws:rds:{self.region}:{self.account_id}:subgrp:{self.subnet_name}"
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<DBSubnetGroup>
               <VpcId>{{ subnet_group.vpc_id }}</VpcId>
               <SubnetGroupStatus>{{ subnet_group.status }}</SubnetGroupStatus>
               <DBSubnetGroupDescription>{{ subnet_group.description }}</DBSubnetGroupDescription>
               <DBSubnetGroupName>{{ subnet_group.subnet_name }}</DBSubnetGroupName>
               <DBSubnetGroupArn>{{ subnet_group.sg_arn }}</DBSubnetGroupArn>
@@ -1374,15 +1400,15 @@
                 </Subnet>
                 {% endfor %}
               </Subnets>
             </DBSubnetGroup>"""
         )
         return template.render(subnet_group=self)
 
-    def to_json(self):
+    def to_json(self) -> str:
         template = Template(
             """"DBSubnetGroup": {
                 "VpcId": "{{ subnet_group.vpc_id }}",
                 "SubnetGroupStatus": "{{ subnet_group.status }}",
                 "DBSubnetGroupDescription": "{{ subnet_group.description }}",
                 "DBSubnetGroupName": "{{ subnet_group.subnet_name }}",
                 "Subnets": {
@@ -1398,26 +1424,31 @@
                   ]
                 }
             }"""
         )
         return template.render(subnet_group=self)
 
     @staticmethod
-    def cloudformation_name_type():
+    def cloudformation_name_type() -> str:
         return "DBSubnetGroupName"
 
     @staticmethod
-    def cloudformation_type():
+    def cloudformation_type() -> str:
         # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-rds-dbsubnetgroup.html
         return "AWS::RDS::DBSubnetGroup"
 
     @classmethod
-    def create_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name, **kwargs
-    ):
+    def create_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+        **kwargs: Any,
+    ) -> "SubnetGroup":
         properties = cloudformation_json["Properties"]
 
         description = properties["DBSubnetGroupDescription"]
         subnet_ids = properties["SubnetIds"]
         tags = properties.get("Tags")
 
         ec2_backend = ec2_backends[account_id][region_name]
@@ -1427,82 +1458,84 @@
             resource_name,
             description,
             subnets,
             tags,
         )
         return subnet_group
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
-    def delete(self, account_id, region_name):
+    def delete(self, account_id: str, region_name: str) -> None:
         backend = rds_backends[account_id][region_name]
         backend.delete_subnet_group(self.subnet_name)
 
 
 class RDSBackend(BaseBackend):
-    def __init__(self, region_name, account_id):
+    def __init__(self, region_name: str, account_id: str):
         super().__init__(region_name, account_id)
         self.arn_regex = re_compile(
             r"^arn:aws:rds:.*:[0-9]*:(db|cluster|es|og|pg|ri|secgrp|snapshot|cluster-snapshot|subgrp):.*$"
         )
         self.clusters: Dict[str, Cluster] = OrderedDict()
-        self.global_clusters = OrderedDict()
-        self.databases = OrderedDict()
-        self.database_snapshots = OrderedDict()
-        self.cluster_snapshots = OrderedDict()
-        self.export_tasks = OrderedDict()
-        self.event_subscriptions = OrderedDict()
-        self.db_parameter_groups = {}
-        self.db_cluster_parameter_groups = {}
-        self.option_groups = {}
-        self.security_groups = {}
-        self.subnet_groups = {}
-        self._db_cluster_options = None
+        self.global_clusters: Dict[str, GlobalCluster] = OrderedDict()
+        self.databases: Dict[str, Database] = OrderedDict()
+        self.database_snapshots: Dict[str, DatabaseSnapshot] = OrderedDict()
+        self.cluster_snapshots: Dict[str, ClusterSnapshot] = OrderedDict()
+        self.export_tasks: Dict[str, ExportTask] = OrderedDict()
+        self.event_subscriptions: Dict[str, EventSubscription] = OrderedDict()
+        self.db_parameter_groups: Dict[str, DBParameterGroup] = {}
+        self.db_cluster_parameter_groups: Dict[str, DBClusterParameterGroup] = {}
+        self.option_groups: Dict[str, OptionGroup] = {}
+        self.security_groups: Dict[str, SecurityGroup] = {}
+        self.subnet_groups: Dict[str, SubnetGroup] = {}
+        self._db_cluster_options: Optional[List[Dict[str, Any]]] = None
 
-    def reset(self):
+    def reset(self) -> None:
         self.neptune.reset()
         super().reset()
 
     @property
     def neptune(self) -> NeptuneBackend:
         return neptune_backends[self.account_id][self.region_name]
 
     @property
-    def db_cluster_options(self):
+    def db_cluster_options(self) -> List[Dict[str, Any]]:  # type: ignore
         if self._db_cluster_options is None:
             from moto.rds.utils import decode_orderable_db_instance
 
             decoded_options = load_resource(
                 __name__, "resources/cluster_options/aurora-postgresql.json"
             )
             self._db_cluster_options = [
                 decode_orderable_db_instance(option) for option in decoded_options
             ]
         return self._db_cluster_options
 
     @staticmethod
-    def default_vpc_endpoint_service(service_region, zones):
+    def default_vpc_endpoint_service(
+        service_region: str, zones: List[str]
+    ) -> List[Dict[str, str]]:
         """Default VPC endpoint service."""
         return BaseBackend.default_vpc_endpoint_service_factory(
             service_region, zones, "rds"
         ) + BaseBackend.default_vpc_endpoint_service_factory(
             service_region, zones, "rds-data"
         )
 
-    def create_db_instance(self, db_kwargs):
+    def create_db_instance(self, db_kwargs: Dict[str, Any]) -> Database:
         database_id = db_kwargs["db_instance_identifier"]
         database = Database(**db_kwargs)
 
         cluster_id = database.db_cluster_identifier
         if cluster_id is not None:
             cluster = self.clusters.get(cluster_id)
             if cluster is not None:
@@ -1511,16 +1544,19 @@
                         "Instances cannot be added to Aurora Serverless clusters."
                     )
                 cluster.cluster_members.append(database_id)
         self.databases[database_id] = database
         return database
 
     def create_db_snapshot(
-        self, db_instance_identifier, db_snapshot_identifier, tags=None
-    ):
+        self,
+        db_instance_identifier: str,
+        db_snapshot_identifier: str,
+        tags: Optional[List[Dict[str, str]]] = None,
+    ) -> DatabaseSnapshot:
         database = self.databases.get(db_instance_identifier)
         if not database:
             raise DBInstanceNotFoundError(db_instance_identifier)
         if db_snapshot_identifier in self.database_snapshots:
             raise DBSnapshotAlreadyExistsError(db_snapshot_identifier)
         if len(self.database_snapshots) >= int(
             os.environ.get("MOTO_RDS_SNAPSHOT_LIMIT", "100")
@@ -1531,16 +1567,19 @@
         if database.copy_tags_to_snapshot and not tags:
             tags = database.get_tags()
         snapshot = DatabaseSnapshot(database, db_snapshot_identifier, tags)
         self.database_snapshots[db_snapshot_identifier] = snapshot
         return snapshot
 
     def copy_database_snapshot(
-        self, source_snapshot_identifier, target_snapshot_identifier, tags=None
-    ):
+        self,
+        source_snapshot_identifier: str,
+        target_snapshot_identifier: str,
+        tags: Optional[List[Dict[str, str]]] = None,
+    ) -> DatabaseSnapshot:
         if source_snapshot_identifier not in self.database_snapshots:
             raise DBSnapshotNotFoundError(source_snapshot_identifier)
         if target_snapshot_identifier in self.database_snapshots:
             raise DBSnapshotAlreadyExistsError(target_snapshot_identifier)
         if len(self.database_snapshots) >= int(
             os.environ.get("MOTO_RDS_SNAPSHOT_LIMIT", "100")
         ):
@@ -1554,30 +1593,30 @@
         target_snapshot = DatabaseSnapshot(
             source_snapshot.database, target_snapshot_identifier, tags
         )
         self.database_snapshots[target_snapshot_identifier] = target_snapshot
 
         return target_snapshot
 
-    def delete_db_snapshot(self, db_snapshot_identifier):
+    def delete_db_snapshot(self, db_snapshot_identifier: str) -> DatabaseSnapshot:
         if db_snapshot_identifier not in self.database_snapshots:
             raise DBSnapshotNotFoundError(db_snapshot_identifier)
 
         return self.database_snapshots.pop(db_snapshot_identifier)
 
-    def promote_read_replica(self, db_kwargs):
+    def promote_read_replica(self, db_kwargs: Dict[str, Any]) -> Database:
         database_id = db_kwargs["db_instance_identifier"]
-        database = self.databases.get(database_id)
+        database = self.databases[database_id]
         if database.is_replica:
             database.is_replica = False
             database.update(db_kwargs)
 
         return database
 
-    def create_db_instance_read_replica(self, db_kwargs):
+    def create_db_instance_read_replica(self, db_kwargs: Dict[str, Any]) -> Database:
         database_id = db_kwargs["db_instance_identifier"]
         source_database_id = db_kwargs["source_db_identifier"]
         primary = self.find_db_from_id(source_database_id)
         if self.arn_regex.match(source_database_id):
             db_kwargs["region"] = self.region_name
 
         # Shouldn't really copy here as the instance is duplicated. RDS replicas have different instances.
@@ -1585,29 +1624,34 @@
         replica.update(db_kwargs)
         replica.region_name = self.region_name
         replica.set_as_replica()
         self.databases[database_id] = replica
         primary.add_replica(replica)
         return replica
 
-    def describe_db_instances(self, db_instance_identifier=None, filters=None):
+    def describe_db_instances(
+        self, db_instance_identifier: Optional[str] = None, filters: Any = None
+    ) -> List[Database]:
         databases = self.databases
         if db_instance_identifier:
             filters = merge_filters(
                 filters, {"db-instance-id": [db_instance_identifier]}
             )
         if filters:
             databases = self._filter_resources(databases, filters, Database)
         if db_instance_identifier and not databases:
             raise DBInstanceNotFoundError(db_instance_identifier)
         return list(databases.values())
 
     def describe_db_snapshots(
-        self, db_instance_identifier, db_snapshot_identifier, filters=None
-    ):
+        self,
+        db_instance_identifier: Optional[str],
+        db_snapshot_identifier: str,
+        filters: Optional[Dict[str, Any]] = None,
+    ) -> List[DatabaseSnapshot]:
         snapshots = self.database_snapshots
         if db_instance_identifier:
             filters = merge_filters(
                 filters, {"db-instance-id": [db_instance_identifier]}
             )
         if db_snapshot_identifier:
             filters = merge_filters(
@@ -1615,37 +1659,40 @@
             )
         if filters:
             snapshots = self._filter_resources(snapshots, filters, DatabaseSnapshot)
         if db_snapshot_identifier and not snapshots and not db_instance_identifier:
             raise DBSnapshotNotFoundError(db_snapshot_identifier)
         return list(snapshots.values())
 
-    def modify_db_instance(self, db_instance_identifier, db_kwargs):
+    def modify_db_instance(
+        self, db_instance_identifier: str, db_kwargs: Dict[str, Any]
+    ) -> Database:
         database = self.describe_db_instances(db_instance_identifier)[0]
         if "new_db_instance_identifier" in db_kwargs:
             del self.databases[db_instance_identifier]
             db_instance_identifier = db_kwargs[
                 "db_instance_identifier"
             ] = db_kwargs.pop("new_db_instance_identifier")
             self.databases[db_instance_identifier] = database
         preferred_backup_window = db_kwargs.get("preferred_backup_window")
         preferred_maintenance_window = db_kwargs.get("preferred_maintenance_window")
         msg = valid_preferred_maintenance_window(
-            preferred_maintenance_window, preferred_backup_window
+            preferred_maintenance_window, preferred_backup_window  # type: ignore
         )
         if msg:
             raise RDSClientError("InvalidParameterValue", msg)
         database.update(db_kwargs)
         return database
 
-    def reboot_db_instance(self, db_instance_identifier):
-        database = self.describe_db_instances(db_instance_identifier)[0]
-        return database
+    def reboot_db_instance(self, db_instance_identifier: str) -> Database:
+        return self.describe_db_instances(db_instance_identifier)[0]
 
-    def restore_db_instance_from_db_snapshot(self, from_snapshot_id, overrides):
+    def restore_db_instance_from_db_snapshot(
+        self, from_snapshot_id: str, overrides: Dict[str, Any]
+    ) -> Database:
         snapshot = self.describe_db_snapshots(
             db_instance_identifier=None, db_snapshot_identifier=from_snapshot_id
         )[0]
         original_database = snapshot.database
         new_instance_props = copy.deepcopy(original_database.__dict__)
         if not original_database.option_group_supplied:
             # If the option group is not supplied originally, the 'option_group_name' will receive a default value
@@ -1654,139 +1701,153 @@
 
         for key, value in overrides.items():
             if value:
                 new_instance_props[key] = value
 
         return self.create_db_instance(new_instance_props)
 
-    def stop_db_instance(self, db_instance_identifier, db_snapshot_identifier=None):
+    def stop_db_instance(
+        self, db_instance_identifier: str, db_snapshot_identifier: Optional[str] = None
+    ) -> Database:
         database = self.describe_db_instances(db_instance_identifier)[0]
         # todo: certain rds types not allowed to be stopped at this time.
         # https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_StopInstance.html#USER_StopInstance.Limitations
         if database.is_replica or (
-            database.multi_az and database.engine.lower().startswith("sqlserver")
+            database.multi_az and database.engine.lower().startswith("sqlserver")  # type: ignore
         ):
             # todo: more db types not supported by stop/start instance api
             raise InvalidDBClusterStateFaultError(db_instance_identifier)
         if database.status != "available":
             raise InvalidDBInstanceStateError(db_instance_identifier, "stop")
         if db_snapshot_identifier:
             self.create_db_snapshot(db_instance_identifier, db_snapshot_identifier)
         database.status = "stopped"
         return database
 
-    def start_db_instance(self, db_instance_identifier):
+    def start_db_instance(self, db_instance_identifier: str) -> Database:
         database = self.describe_db_instances(db_instance_identifier)[0]
         # todo: bunch of different error messages to be generated from this api call
         if database.status != "stopped":
             raise InvalidDBInstanceStateError(db_instance_identifier, "start")
         database.status = "available"
         return database
 
-    def find_db_from_id(self, db_id):
+    def find_db_from_id(self, db_id: str) -> Database:
         if self.arn_regex.match(db_id):
             arn_breakdown = db_id.split(":")
             region = arn_breakdown[3]
             backend = rds_backends[self.account_id][region]
             db_name = arn_breakdown[-1]
         else:
             backend = self
             db_name = db_id
 
         return backend.describe_db_instances(db_name)[0]
 
-    def delete_db_instance(self, db_instance_identifier, db_snapshot_name=None):
+    def delete_db_instance(
+        self, db_instance_identifier: str, db_snapshot_name: Optional[str] = None
+    ) -> Database:
         if db_instance_identifier in self.databases:
             if self.databases[db_instance_identifier].deletion_protection:
                 raise InvalidParameterValue(
                     "Can't delete Instance with protection enabled"
                 )
             if db_snapshot_name:
                 self.create_db_snapshot(db_instance_identifier, db_snapshot_name)
             database = self.databases.pop(db_instance_identifier)
             if database.is_replica:
-                primary = self.find_db_from_id(database.source_db_identifier)
+                primary = self.find_db_from_id(database.source_db_identifier)  # type: ignore
                 primary.remove_replica(database)
             if database.db_cluster_identifier in self.clusters:
                 self.clusters[database.db_cluster_identifier].cluster_members.remove(
                     db_instance_identifier
                 )
             database.status = "deleting"
             return database
         else:
             raise DBInstanceNotFoundError(db_instance_identifier)
 
-    def create_db_security_group(self, group_name, description, tags):
+    def create_db_security_group(
+        self, group_name: str, description: str, tags: List[Dict[str, str]]
+    ) -> SecurityGroup:
         security_group = SecurityGroup(self.account_id, group_name, description, tags)
         self.security_groups[group_name] = security_group
         return security_group
 
-    def describe_security_groups(self, security_group_name):
+    def describe_security_groups(self, security_group_name: str) -> List[SecurityGroup]:
         if security_group_name:
             if security_group_name in self.security_groups:
                 return [self.security_groups[security_group_name]]
             else:
                 raise DBSecurityGroupNotFoundError(security_group_name)
-        return self.security_groups.values()
+        return list(self.security_groups.values())
 
-    def delete_security_group(self, security_group_name):
+    def delete_security_group(self, security_group_name: str) -> SecurityGroup:
         if security_group_name in self.security_groups:
             return self.security_groups.pop(security_group_name)
         else:
             raise DBSecurityGroupNotFoundError(security_group_name)
 
-    def delete_db_parameter_group(self, db_parameter_group_name):
+    def delete_db_parameter_group(
+        self, db_parameter_group_name: str
+    ) -> "DBParameterGroup":
         if db_parameter_group_name in self.db_parameter_groups:
             return self.db_parameter_groups.pop(db_parameter_group_name)
         else:
             raise DBParameterGroupNotFoundError(db_parameter_group_name)
 
-    def authorize_security_group(self, security_group_name, cidr_ip):
+    def authorize_security_group(
+        self, security_group_name: str, cidr_ip: str
+    ) -> SecurityGroup:
         security_group = self.describe_security_groups(security_group_name)[0]
         security_group.authorize_cidr(cidr_ip)
         return security_group
 
     def create_subnet_group(
         self,
-        subnet_name,
-        description,
-        subnets,
-        tags,
-    ):
+        subnet_name: str,
+        description: str,
+        subnets: List[Any],
+        tags: List[Dict[str, str]],
+    ) -> SubnetGroup:
         subnet_group = SubnetGroup(
             subnet_name, description, subnets, tags, self.region_name, self.account_id
         )
         self.subnet_groups[subnet_name] = subnet_group
         return subnet_group
 
-    def describe_db_subnet_groups(self, subnet_group_name):
+    def describe_db_subnet_groups(
+        self, subnet_group_name: str
+    ) -> Iterable[SubnetGroup]:
         if subnet_group_name:
             if subnet_group_name in self.subnet_groups:
                 return [self.subnet_groups[subnet_group_name]]
             else:
                 raise DBSubnetGroupNotFoundError(subnet_group_name)
         return self.subnet_groups.values()
 
-    def modify_db_subnet_group(self, subnet_name, description, subnets):
+    def modify_db_subnet_group(
+        self, subnet_name: str, description: str, subnets: List[str]
+    ) -> SubnetGroup:
         subnet_group = self.subnet_groups.pop(subnet_name)
         if not subnet_group:
             raise DBSubnetGroupNotFoundError(subnet_name)
         subnet_group.subnet_name = subnet_name
         subnet_group.subnets = subnets
         if description is not None:
             subnet_group.description = description
         return subnet_group
 
-    def delete_subnet_group(self, subnet_name):
+    def delete_subnet_group(self, subnet_name: str) -> SubnetGroup:
         if subnet_name in self.subnet_groups:
             return self.subnet_groups.pop(subnet_name)
         else:
             raise DBSubnetGroupNotFoundError(subnet_name)
 
-    def create_option_group(self, option_group_kwargs):
+    def create_option_group(self, option_group_kwargs: Dict[str, Any]) -> "OptionGroup":
         option_group_id = option_group_kwargs["name"]
         # This list was verified against the AWS Console on 14 Dec 2022
         # Having an automated way (using the CLI) would be nice, but AFAICS that's not possible
         #
         # Some options that are allowed in the CLI, but that do now show up in the Console:
         # - Mysql 5.5
         # - All postgres-versions
@@ -1822,15 +1883,15 @@
                 "The parameter OptionGroupDescription must be provided and must not be blank.",
             )
         if option_group_kwargs["engine_name"] not in valid_option_group_engines.keys():
             raise RDSClientError(
                 "InvalidParameterValue", "Invalid DB engine: non-existent"
             )
         if (
-            option_group_kwargs["major_engine_version"]
+            option_group_kwargs["major_engine_version"]  # type: ignore
             not in valid_option_group_engines[option_group_kwargs["engine_name"]]
         ):
             raise RDSClientError(
                 "InvalidParameterCombination",
                 f"Cannot find major version {option_group_kwargs['major_engine_version']} for {option_group_kwargs['engine_name']}",
             )
         # AWS also creates default option groups, if they do not yet exist, when creating an option group in the CLI
@@ -1849,21 +1910,23 @@
         # add region and account-id to construct the arn
         option_group_kwargs["region"] = self.region_name
         option_group_kwargs["account_id"] = self.account_id
         option_group = OptionGroup(**option_group_kwargs)
         self.option_groups[option_group_id] = option_group
         return option_group
 
-    def delete_option_group(self, option_group_name):
+    def delete_option_group(self, option_group_name: str) -> "OptionGroup":
         if option_group_name in self.option_groups:
             return self.option_groups.pop(option_group_name)
         else:
             raise OptionGroupNotFoundFaultError(option_group_name)
 
-    def describe_option_groups(self, option_group_kwargs):
+    def describe_option_groups(
+        self, option_group_kwargs: Dict[str, Any]
+    ) -> List["OptionGroup"]:
         option_group_list = []
 
         if option_group_kwargs["marker"]:
             marker = option_group_kwargs["marker"]
         else:
             marker = 0
         if option_group_kwargs["max_records"]:
@@ -1899,15 +1962,17 @@
             else:
                 option_group_list.append(option_group)
         if not len(option_group_list):
             raise OptionGroupNotFoundFaultError(option_group_kwargs["name"])
         return option_group_list[marker : max_records + marker]
 
     @staticmethod
-    def describe_option_group_options(engine_name, major_engine_version=None):
+    def describe_option_group_options(
+        engine_name: str, major_engine_version: Optional[str] = None
+    ) -> str:
         default_option_group_options = {
             "mysql": {
                 "5.6": '<DescribeOptionGroupOptionsResponse xmlns="http://rds.amazonaws.com/doc/2014-09-01/">\n  <DescribeOptionGroupOptionsResult>\n    <OptionGroupOptions>\n    \n      <OptionGroupOption><MajorEngineVersion>5.6</MajorEngineVersion><DefaultPort>11211</DefaultPort><PortRequired>True</PortRequired><OptionsDependedOn></OptionsDependedOn><Description>Innodb Memcached for MySQL</Description><Name>MEMCACHED</Name><OptionGroupOptionSettings><OptionGroupOptionSetting><AllowedValues>1-4294967295</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies how many memcached read operations (get) to perform before doing a COMMIT to start a new transaction</SettingDescription><SettingName>DAEMON_MEMCACHED_R_BATCH_SIZE</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-4294967295</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies how many memcached write operations, such as add, set, or incr, to perform before doing a COMMIT to start a new transaction</SettingDescription><SettingName>DAEMON_MEMCACHED_W_BATCH_SIZE</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-1073741824</AllowedValues><ApplyType>DYNAMIC</ApplyType><DefaultValue>5</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies how often to auto-commit idle connections that use the InnoDB memcached interface.</SettingDescription><SettingName>INNODB_API_BK_COMMIT_INTERVAL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Disables the use of row locks when using the InnoDB memcached interface.</SettingDescription><SettingName>INNODB_API_DISABLE_ROWLOCK</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Locks the table used by the InnoDB memcached plugin, so that it cannot be dropped or altered by DDL through the SQL interface.</SettingDescription><SettingName>INNODB_API_ENABLE_MDL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0-3</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Lets you control the transaction isolation level on queries processed by the memcached interface.</SettingDescription><SettingName>INNODB_API_TRX_LEVEL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>auto,ascii,binary</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>auto</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>The binding protocol to use which can be either auto, ascii, or binary. The default is auto which means the server automatically negotiates the protocol with the client.</SettingDescription><SettingName>BINDING_PROTOCOL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-2048</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1024</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>The backlog queue configures how many network connections can be waiting to be processed by memcached</SettingDescription><SettingName>BACKLOG_QUEUE_LIMIT</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Disable the use of compare and swap (CAS) which reduces the per-item size by 8 bytes.</SettingDescription><SettingName>CAS_DISABLED</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-48</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>48</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Minimum chunk size in bytes to allocate for the smallest item\'s key, value, and flags. The default is 48 and you can get a significant memory efficiency gain with a lower value.</SettingDescription><SettingName>CHUNK_SIZE</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-2</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1.25</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Chunk size growth factor that controls the size of each successive chunk with each chunk growing times this amount larger than the previous chunk.</SettingDescription><SettingName>CHUNK_SIZE_GROWTH_FACTOR</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>If enabled when there is no more memory to store items, memcached will return an error rather than evicting items.</SettingDescription><SettingName>ERROR_ON_MEMORY_EXHAUSTED</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>10-1024</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1024</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Maximum number of concurrent connections. Setting this value to anything less than 10 prevents MySQL from starting.</SettingDescription><SettingName>MAX_SIMULTANEOUS_CONNECTIONS</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>v,vv,vvv</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>v</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Verbose level for memcached.</SettingDescription><SettingName>VERBOSITY</SettingName></OptionGroupOptionSetting></OptionGroupOptionSettings><EngineName>mysql</EngineName></OptionGroupOption>\n    \n    </OptionGroupOptions>\n  </DescribeOptionGroupOptionsResult>\n  <ResponseMetadata>\n    <RequestId>457f7bb8-9fbf-11e4-9084-5754f80d5144</RequestId>\n  </ResponseMetadata>\n</DescribeOptionGroupOptionsResponse>',
                 "all": '<DescribeOptionGroupOptionsResponse xmlns="http://rds.amazonaws.com/doc/2014-09-01/">\n  <DescribeOptionGroupOptionsResult>\n    <OptionGroupOptions>\n    \n      <OptionGroupOption><MajorEngineVersion>5.6</MajorEngineVersion><DefaultPort>11211</DefaultPort><PortRequired>True</PortRequired><OptionsDependedOn></OptionsDependedOn><Description>Innodb Memcached for MySQL</Description><Name>MEMCACHED</Name><OptionGroupOptionSettings><OptionGroupOptionSetting><AllowedValues>1-4294967295</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies how many memcached read operations (get) to perform before doing a COMMIT to start a new transaction</SettingDescription><SettingName>DAEMON_MEMCACHED_R_BATCH_SIZE</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-4294967295</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies how many memcached write operations, such as add, set, or incr, to perform before doing a COMMIT to start a new transaction</SettingDescription><SettingName>DAEMON_MEMCACHED_W_BATCH_SIZE</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-1073741824</AllowedValues><ApplyType>DYNAMIC</ApplyType><DefaultValue>5</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies how often to auto-commit idle connections that use the InnoDB memcached interface.</SettingDescription><SettingName>INNODB_API_BK_COMMIT_INTERVAL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Disables the use of row locks when using the InnoDB memcached interface.</SettingDescription><SettingName>INNODB_API_DISABLE_ROWLOCK</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Locks the table used by the InnoDB memcached plugin, so that it cannot be dropped or altered by DDL through the SQL interface.</SettingDescription><SettingName>INNODB_API_ENABLE_MDL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0-3</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Lets you control the transaction isolation level on queries processed by the memcached interface.</SettingDescription><SettingName>INNODB_API_TRX_LEVEL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>auto,ascii,binary</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>auto</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>The binding protocol to use which can be either auto, ascii, or binary. The default is auto which means the server automatically negotiates the protocol with the client.</SettingDescription><SettingName>BINDING_PROTOCOL</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-2048</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1024</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>The backlog queue configures how many network connections can be waiting to be processed by memcached</SettingDescription><SettingName>BACKLOG_QUEUE_LIMIT</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Disable the use of compare and swap (CAS) which reduces the per-item size by 8 bytes.</SettingDescription><SettingName>CAS_DISABLED</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-48</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>48</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Minimum chunk size in bytes to allocate for the smallest item\'s key, value, and flags. The default is 48 and you can get a significant memory efficiency gain with a lower value.</SettingDescription><SettingName>CHUNK_SIZE</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>1-2</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1.25</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Chunk size growth factor that controls the size of each successive chunk with each chunk growing times this amount larger than the previous chunk.</SettingDescription><SettingName>CHUNK_SIZE_GROWTH_FACTOR</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>0,1</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>0</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>If enabled when there is no more memory to store items, memcached will return an error rather than evicting items.</SettingDescription><SettingName>ERROR_ON_MEMORY_EXHAUSTED</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>10-1024</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>1024</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Maximum number of concurrent connections. Setting this value to anything less than 10 prevents MySQL from starting.</SettingDescription><SettingName>MAX_SIMULTANEOUS_CONNECTIONS</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>v,vv,vvv</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>v</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Verbose level for memcached.</SettingDescription><SettingName>VERBOSITY</SettingName></OptionGroupOptionSetting></OptionGroupOptionSettings><EngineName>mysql</EngineName></OptionGroupOption>\n    \n    </OptionGroupOptions>\n  </DescribeOptionGroupOptionsResult>\n  <ResponseMetadata>\n    <RequestId>457f7bb8-9fbf-11e4-9084-5754f80d5144</RequestId>\n  </ResponseMetadata>\n</DescribeOptionGroupOptionsResponse>',
             },
             "oracle-ee": {
                 "11.2": '<DescribeOptionGroupOptionsResponse xmlns="http://rds.amazonaws.com/doc/2014-09-01/">\n  <DescribeOptionGroupOptionsResult>\n    <OptionGroupOptions>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><OptionsDependedOn><OptionName>XMLDB</OptionName></OptionsDependedOn><Description>Oracle Application Express Runtime Environment</Description><Name>APEX</Name><OptionGroupOptionSettings></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><OptionsDependedOn><OptionName>APEX</OptionName></OptionsDependedOn><Description>Oracle Application Express Development Environment</Description><Name>APEX-DEV</Name><OptionGroupOptionSettings></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><OptionsDependedOn></OptionsDependedOn><Description>Oracle Advanced Security - Native Network Encryption</Description><Name>NATIVE_NETWORK_ENCRYPTION</Name><OptionGroupOptionSettings><OptionGroupOptionSetting><AllowedValues>ACCEPTED,REJECTED,REQUESTED,REQUIRED</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>REQUESTED</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies the desired encryption behavior</SettingDescription><SettingName>SQLNET.ENCRYPTION_SERVER</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>ACCEPTED,REJECTED,REQUESTED,REQUIRED</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>REQUESTED</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies the desired data integrity behavior</SettingDescription><SettingName>SQLNET.CRYPTO_CHECKSUM_SERVER</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>RC4_256,AES256,AES192,3DES168,RC4_128,AES128,3DES112,RC4_56,DES,RC4_40,DES40</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>RC4_256,AES256,AES192,3DES168,RC4_128,AES128,3DES112,RC4_56,DES,RC4_40,DES40</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies list of encryption algorithms in order of intended use</SettingDescription><SettingName>SQLNET.ENCRYPTION_TYPES_SERVER</SettingName></OptionGroupOptionSetting><OptionGroupOptionSetting><AllowedValues>SHA1,MD5</AllowedValues><ApplyType>STATIC</ApplyType><DefaultValue>SHA1,MD5</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies list of checksumming algorithms in order of intended use</SettingDescription><SettingName>SQLNET.CRYPTO_CHECKSUM_TYPES_SERVER</SettingName></OptionGroupOptionSetting></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><DefaultPort>1158</DefaultPort><PortRequired>True</PortRequired><OptionsDependedOn></OptionsDependedOn><Description>Oracle Enterprise Manager (Database Control only)</Description><Name>OEM</Name><OptionGroupOptionSettings></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><OptionsDependedOn></OptionsDependedOn><Description>Oracle Statspack</Description><Name>STATSPACK</Name><OptionGroupOptionSettings></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><Persistent>True</Persistent><OptionsDependedOn></OptionsDependedOn><Permanent>True</Permanent><Description>Oracle Advanced Security - Transparent Data Encryption</Description><Name>TDE</Name><OptionGroupOptionSettings></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><Persistent>True</Persistent><OptionsDependedOn></OptionsDependedOn><Permanent>True</Permanent><Description>Oracle Advanced Security - TDE with HSM</Description><Name>TDE_HSM</Name><OptionGroupOptionSettings></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><Persistent>True</Persistent><OptionsDependedOn></OptionsDependedOn><Permanent>True</Permanent><Description>Change time zone</Description><Name>Timezone</Name><OptionGroupOptionSettings><OptionGroupOptionSetting><AllowedValues>Africa/Cairo,Africa/Casablanca,Africa/Harare,Africa/Monrovia,Africa/Nairobi,Africa/Tripoli,Africa/Windhoek,America/Araguaina,America/Asuncion,America/Bogota,America/Caracas,America/Chihuahua,America/Cuiaba,America/Denver,America/Fortaleza,America/Guatemala,America/Halifax,America/Manaus,America/Matamoros,America/Monterrey,America/Montevideo,America/Phoenix,America/Santiago,America/Tijuana,Asia/Amman,Asia/Ashgabat,Asia/Baghdad,Asia/Baku,Asia/Bangkok,Asia/Beirut,Asia/Calcutta,Asia/Damascus,Asia/Dhaka,Asia/Irkutsk,Asia/Jerusalem,Asia/Kabul,Asia/Karachi,Asia/Kathmandu,Asia/Krasnoyarsk,Asia/Magadan,Asia/Muscat,Asia/Novosibirsk,Asia/Riyadh,Asia/Seoul,Asia/Shanghai,Asia/Singapore,Asia/Taipei,Asia/Tehran,Asia/Tokyo,Asia/Ulaanbaatar,Asia/Vladivostok,Asia/Yakutsk,Asia/Yerevan,Atlantic/Azores,Australia/Adelaide,Australia/Brisbane,Australia/Darwin,Australia/Hobart,Australia/Perth,Australia/Sydney,Brazil/East,Canada/Newfoundland,Canada/Saskatchewan,Europe/Amsterdam,Europe/Athens,Europe/Dublin,Europe/Helsinki,Europe/Istanbul,Europe/Kaliningrad,Europe/Moscow,Europe/Paris,Europe/Prague,Europe/Sarajevo,Pacific/Auckland,Pacific/Fiji,Pacific/Guam,Pacific/Honolulu,Pacific/Samoa,US/Alaska,US/Central,US/Eastern,US/East-Indiana,US/Pacific,UTC</AllowedValues><ApplyType>DYNAMIC</ApplyType><DefaultValue>UTC</DefaultValue><IsModifiable>True</IsModifiable><SettingDescription>Specifies the timezone the user wants to change the system time to</SettingDescription><SettingName>TIME_ZONE</SettingName></OptionGroupOptionSetting></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n      <OptionGroupOption><MajorEngineVersion>11.2</MajorEngineVersion><OptionsDependedOn></OptionsDependedOn><Description>Oracle XMLDB Repository</Description><Name>XMLDB</Name><OptionGroupOptionSettings></OptionGroupOptionSettings><EngineName>oracle-ee</EngineName></OptionGroupOption>\n    \n    </OptionGroupOptions>\n  </DescribeOptionGroupOptionsResult>\n  <ResponseMetadata>\n    <RequestId>457f7bb8-9fbf-11e4-9084-5754f80d5144</RequestId>\n  </ResponseMetadata>\n</DescribeOptionGroupOptionsResponse>',
@@ -1941,30 +2006,35 @@
                 f"Cannot find major version {major_engine_version} for {engine_name}",
             )
         if major_engine_version:
             return default_option_group_options[engine_name][major_engine_version]
         return default_option_group_options[engine_name]["all"]
 
     def modify_option_group(
-        self, option_group_name, options_to_include=None, options_to_remove=None
-    ):
+        self,
+        option_group_name: str,
+        options_to_include: Optional[List[Dict[str, Any]]] = None,
+        options_to_remove: Optional[List[Dict[str, Any]]] = None,
+    ) -> "OptionGroup":
         if option_group_name not in self.option_groups:
             raise OptionGroupNotFoundFaultError(option_group_name)
         if not options_to_include and not options_to_remove:
             raise RDSClientError(
                 "InvalidParameterValue",
                 "At least one option must be added, modified, or removed.",
             )
         if options_to_remove:
             self.option_groups[option_group_name].remove_options(options_to_remove)
         if options_to_include:
             self.option_groups[option_group_name].add_options(options_to_include)
         return self.option_groups[option_group_name]
 
-    def create_db_parameter_group(self, db_parameter_group_kwargs):
+    def create_db_parameter_group(
+        self, db_parameter_group_kwargs: Dict[str, Any]
+    ) -> "DBParameterGroup":
         db_parameter_group_id = db_parameter_group_kwargs["name"]
         if db_parameter_group_id in self.db_parameter_groups:
             raise RDSClientError(
                 "DBParameterGroupAlreadyExistsFault",
                 f"A DB parameter group named {db_parameter_group_id} already exists.",
             )
         if not db_parameter_group_kwargs.get("description"):
@@ -1979,15 +2049,17 @@
             )
         db_parameter_group_kwargs["region"] = self.region_name
         db_parameter_group_kwargs["account_id"] = self.account_id
         db_parameter_group = DBParameterGroup(**db_parameter_group_kwargs)
         self.db_parameter_groups[db_parameter_group_id] = db_parameter_group
         return db_parameter_group
 
-    def describe_db_parameter_groups(self, db_parameter_group_kwargs):
+    def describe_db_parameter_groups(
+        self, db_parameter_group_kwargs: Dict[str, Any]
+    ) -> List["DBParameterGroup"]:
         db_parameter_group_list = []
 
         if db_parameter_group_kwargs.get("marker"):
             marker = db_parameter_group_kwargs["marker"]
         else:
             marker = 0
         if db_parameter_group_kwargs.get("max_records"):
@@ -2010,51 +2082,56 @@
                 db_parameter_group_list.append(db_parameter_group)
             else:
                 continue
 
         return db_parameter_group_list[marker : max_records + marker]
 
     def modify_db_parameter_group(
-        self, db_parameter_group_name, db_parameter_group_parameters
-    ):
+        self,
+        db_parameter_group_name: str,
+        db_parameter_group_parameters: Iterable[Dict[str, Any]],
+    ) -> "DBParameterGroup":
         if db_parameter_group_name not in self.db_parameter_groups:
             raise DBParameterGroupNotFoundError(db_parameter_group_name)
 
         db_parameter_group = self.db_parameter_groups[db_parameter_group_name]
         db_parameter_group.update_parameters(db_parameter_group_parameters)
 
         return db_parameter_group
 
-    def describe_db_cluster_parameters(self):
+    def describe_db_cluster_parameters(self) -> List[Dict[str, Any]]:
         return []
 
-    def create_db_cluster(self, kwargs):
+    def create_db_cluster(self, kwargs: Dict[str, Any]) -> Cluster:
         cluster_id = kwargs["db_cluster_identifier"]
         kwargs["account_id"] = self.account_id
         cluster = Cluster(**kwargs)
         self.clusters[cluster_id] = cluster
 
-        if (cluster.global_cluster_identifier or "") in self.global_clusters:
+        if (
+            cluster.global_cluster_identifier
+            and cluster.global_cluster_identifier in self.global_clusters
+        ):
             global_cluster = self.global_clusters[cluster.global_cluster_identifier]
             global_cluster.members.append(cluster.db_cluster_arn)
 
         if cluster.replication_source_identifier:
             cluster_identifier = cluster.replication_source_identifier
             original_cluster = find_cluster(cluster_identifier)
             original_cluster.read_replica_identifiers.append(cluster.db_cluster_arn)
 
         initial_state = copy.deepcopy(cluster)  # Return status=creating
         cluster.status = "available"  # Already set the final status in the background
         return initial_state
 
-    def modify_db_cluster(self, kwargs):
+    def modify_db_cluster(self, kwargs: Dict[str, Any]) -> Cluster:
         cluster_id = kwargs["db_cluster_identifier"]
 
         if cluster_id in self.neptune.clusters:
-            return self.neptune.modify_db_cluster(kwargs)
+            return self.neptune.modify_db_cluster(kwargs)  # type: ignore
 
         cluster = self.clusters[cluster_id]
         del self.clusters[cluster_id]
 
         kwargs["db_cluster_identifier"] = kwargs.pop("new_db_cluster_identifier")
         for k, v in kwargs.items():
             if v is not None:
@@ -2072,22 +2149,25 @@
 
         initial_state = copy.deepcopy(cluster)  # Return status=creating
         cluster.status = "available"  # Already set the final status in the background
         return initial_state
 
     def promote_read_replica_db_cluster(self, db_cluster_identifier: str) -> Cluster:
         cluster = self.clusters[db_cluster_identifier]
-        source_cluster = find_cluster(cluster.replication_source_identifier)
+        source_cluster = find_cluster(cluster.replication_source_identifier)  # type: ignore
         source_cluster.read_replica_identifiers.remove(cluster.db_cluster_arn)
         cluster.replication_source_identifier = None
         return cluster
 
     def create_db_cluster_snapshot(
-        self, db_cluster_identifier, db_snapshot_identifier, tags=None
-    ):
+        self,
+        db_cluster_identifier: str,
+        db_snapshot_identifier: str,
+        tags: Optional[List[Dict[str, str]]] = None,
+    ) -> ClusterSnapshot:
         cluster = self.clusters.get(db_cluster_identifier)
         if cluster is None:
             raise DBClusterNotFoundError(db_cluster_identifier)
         if db_snapshot_identifier in self.cluster_snapshots:
             raise DBClusterSnapshotAlreadyExistsError(db_snapshot_identifier)
         if len(self.cluster_snapshots) >= int(
             os.environ.get("MOTO_RDS_SNAPSHOT_LIMIT", "100")
@@ -2098,74 +2178,84 @@
         if cluster.copy_tags_to_snapshot:
             tags += cluster.get_tags()
         snapshot = ClusterSnapshot(cluster, db_snapshot_identifier, tags)
         self.cluster_snapshots[db_snapshot_identifier] = snapshot
         return snapshot
 
     def copy_cluster_snapshot(
-        self, source_snapshot_identifier, target_snapshot_identifier, tags=None
-    ):
+        self,
+        source_snapshot_identifier: str,
+        target_snapshot_identifier: str,
+        tags: Optional[List[Dict[str, str]]] = None,
+    ) -> ClusterSnapshot:
         if source_snapshot_identifier not in self.cluster_snapshots:
             raise DBClusterSnapshotNotFoundError(source_snapshot_identifier)
         if target_snapshot_identifier in self.cluster_snapshots:
             raise DBClusterSnapshotAlreadyExistsError(target_snapshot_identifier)
         if len(self.cluster_snapshots) >= int(
             os.environ.get("MOTO_RDS_SNAPSHOT_LIMIT", "100")
         ):
             raise SnapshotQuotaExceededError()
         source_snapshot = self.cluster_snapshots[source_snapshot_identifier]
         if tags is None:
             tags = source_snapshot.tags
         else:
-            tags = self._merge_tags(source_snapshot.tags, tags)
+            tags = self._merge_tags(source_snapshot.tags, tags)  # type: ignore
         target_snapshot = ClusterSnapshot(
             source_snapshot.cluster, target_snapshot_identifier, tags
         )
         self.cluster_snapshots[target_snapshot_identifier] = target_snapshot
         return target_snapshot
 
-    def delete_db_cluster_snapshot(self, db_snapshot_identifier):
+    def delete_db_cluster_snapshot(
+        self, db_snapshot_identifier: str
+    ) -> ClusterSnapshot:
         if db_snapshot_identifier not in self.cluster_snapshots:
             raise DBClusterSnapshotNotFoundError(db_snapshot_identifier)
 
         return self.cluster_snapshots.pop(db_snapshot_identifier)
 
     def describe_db_clusters(
-        self, cluster_identifier=None, filters=None
+        self, cluster_identifier: Optional[str] = None, filters: Any = None
     ) -> List[Cluster]:
         clusters = self.clusters
         clusters_neptune = self.neptune.clusters
         if cluster_identifier:
             filters = merge_filters(filters, {"db-cluster-id": [cluster_identifier]})
         if filters:
             clusters = self._filter_resources(clusters, filters, Cluster)
             clusters_neptune = self._filter_resources(
                 clusters_neptune, filters, Cluster
             )
         if cluster_identifier and not (clusters or clusters_neptune):
             raise DBClusterNotFoundError(cluster_identifier)
-        return list(clusters.values()) + list(clusters_neptune.values())
+        return list(clusters.values()) + list(clusters_neptune.values())  # type: ignore
 
     def describe_db_cluster_snapshots(
-        self, db_cluster_identifier, db_snapshot_identifier, filters=None
-    ):
+        self,
+        db_cluster_identifier: Optional[str],
+        db_snapshot_identifier: str,
+        filters: Any = None,
+    ) -> List[ClusterSnapshot]:
         snapshots = self.cluster_snapshots
         if db_cluster_identifier:
             filters = merge_filters(filters, {"db-cluster-id": [db_cluster_identifier]})
         if db_snapshot_identifier:
             filters = merge_filters(
                 filters, {"db-cluster-snapshot-id": [db_snapshot_identifier]}
             )
         if filters:
             snapshots = self._filter_resources(snapshots, filters, ClusterSnapshot)
         if db_snapshot_identifier and not snapshots and not db_cluster_identifier:
             raise DBClusterSnapshotNotFoundError(db_snapshot_identifier)
         return list(snapshots.values())
 
-    def delete_db_cluster(self, cluster_identifier, snapshot_name=None):
+    def delete_db_cluster(
+        self, cluster_identifier: str, snapshot_name: Optional[str] = None
+    ) -> Cluster:
         if cluster_identifier in self.clusters:
             cluster = self.clusters[cluster_identifier]
             if cluster.deletion_protection:
                 raise InvalidParameterValue(
                     "Can't delete Cluster with protection enabled"
                 )
 
@@ -2173,56 +2263,58 @@
             if global_id in self.global_clusters:
                 self.remove_from_global_cluster(global_id, cluster_identifier)
 
             if snapshot_name:
                 self.create_db_cluster_snapshot(cluster_identifier, snapshot_name)
             return self.clusters.pop(cluster_identifier)
         if cluster_identifier in self.neptune.clusters:
-            return self.neptune.delete_db_cluster(cluster_identifier)
+            return self.neptune.delete_db_cluster(cluster_identifier)  # type: ignore
         raise DBClusterNotFoundError(cluster_identifier)
 
-    def start_db_cluster(self, cluster_identifier):
+    def start_db_cluster(self, cluster_identifier: str) -> Cluster:
         if cluster_identifier not in self.clusters:
-            return self.neptune.start_db_cluster(cluster_identifier)
+            return self.neptune.start_db_cluster(cluster_identifier)  # type: ignore
             raise DBClusterNotFoundError(cluster_identifier)
         cluster = self.clusters[cluster_identifier]
         if cluster.status != "stopped":
             raise InvalidDBClusterStateFault(
                 "DbCluster cluster-id is not in stopped state."
             )
         temp_state = copy.deepcopy(cluster)
         temp_state.status = "started"
         cluster.status = "available"  # This is the final status - already setting it in the background
         return temp_state
 
-    def restore_db_cluster_from_snapshot(self, from_snapshot_id, overrides):
+    def restore_db_cluster_from_snapshot(
+        self, from_snapshot_id: str, overrides: Dict[str, Any]
+    ) -> Cluster:
         snapshot = self.describe_db_cluster_snapshots(
             db_cluster_identifier=None, db_snapshot_identifier=from_snapshot_id
         )[0]
         original_cluster = snapshot.cluster
         new_cluster_props = copy.deepcopy(original_cluster.get_cfg())
         for key, value in overrides.items():
             if value:
                 new_cluster_props[key] = value
 
         return self.create_db_cluster(new_cluster_props)
 
-    def stop_db_cluster(self, cluster_identifier):
+    def stop_db_cluster(self, cluster_identifier: str) -> "Cluster":
         if cluster_identifier not in self.clusters:
             raise DBClusterNotFoundError(cluster_identifier)
         cluster = self.clusters[cluster_identifier]
         if cluster.status not in ["available"]:
             raise InvalidDBClusterStateFault(
                 "DbCluster cluster-id is not in available state."
             )
         previous_state = copy.deepcopy(cluster)
         cluster.status = "stopped"
         return previous_state
 
-    def start_export_task(self, kwargs):
+    def start_export_task(self, kwargs: Dict[str, Any]) -> ExportTask:
         export_task_id = kwargs["export_task_identifier"]
         source_arn = kwargs["source_arn"]
         snapshot_id = source_arn.split(":")[-1]
         snapshot_type = source_arn.split(":")[-2]
 
         if export_task_id in self.export_tasks:
             raise ExportTaskAlreadyExistsError(export_task_id)
@@ -2231,68 +2323,74 @@
         elif (
             snapshot_type == "cluster-snapshot"
             and snapshot_id not in self.cluster_snapshots
         ):
             raise DBClusterSnapshotNotFoundError(snapshot_id)
 
         if snapshot_type == "snapshot":
-            snapshot = self.database_snapshots[snapshot_id]
+            snapshot: Union[
+                DatabaseSnapshot, ClusterSnapshot
+            ] = self.database_snapshots[snapshot_id]
         else:
             snapshot = self.cluster_snapshots[snapshot_id]
 
         if snapshot.status not in ["available"]:
             raise InvalidExportSourceStateError(snapshot.status)
 
         export_task = ExportTask(snapshot, kwargs)
         self.export_tasks[export_task_id] = export_task
 
         return export_task
 
-    def cancel_export_task(self, export_task_identifier):
+    def cancel_export_task(self, export_task_identifier: str) -> ExportTask:
         if export_task_identifier in self.export_tasks:
             export_task = self.export_tasks[export_task_identifier]
             export_task.status = "canceled"
             self.export_tasks[export_task_identifier] = export_task
             return export_task
         raise ExportTaskNotFoundError(export_task_identifier)
 
-    def describe_export_tasks(self, export_task_identifier):
+    def describe_export_tasks(
+        self, export_task_identifier: str
+    ) -> Iterable[ExportTask]:
         if export_task_identifier:
             if export_task_identifier in self.export_tasks:
                 return [self.export_tasks[export_task_identifier]]
             else:
                 raise ExportTaskNotFoundError(export_task_identifier)
         return self.export_tasks.values()
 
-    def create_event_subscription(self, kwargs):
+    def create_event_subscription(self, kwargs: Any) -> EventSubscription:
         subscription_name = kwargs["subscription_name"]
 
         if subscription_name in self.event_subscriptions:
             raise SubscriptionAlreadyExistError(subscription_name)
 
         kwargs["account_id"] = self.account_id
         subscription = EventSubscription(kwargs)
         self.event_subscriptions[subscription_name] = subscription
 
         return subscription
 
-    def delete_event_subscription(self, subscription_name):
+    def delete_event_subscription(self, subscription_name: str) -> EventSubscription:
         if subscription_name in self.event_subscriptions:
             return self.event_subscriptions.pop(subscription_name)
         raise SubscriptionNotFoundError(subscription_name)
 
-    def describe_event_subscriptions(self, subscription_name):
+    def describe_event_subscriptions(
+        self, subscription_name: str
+    ) -> Iterable[EventSubscription]:
         if subscription_name:
             if subscription_name in self.event_subscriptions:
                 return [self.event_subscriptions[subscription_name]]
             else:
                 raise SubscriptionNotFoundError(subscription_name)
         return self.event_subscriptions.values()
 
-    def list_tags_for_resource(self, arn):
+    def list_tags_for_resource(self, arn: str) -> List[Dict[str, str]]:
         if self.arn_regex.match(arn):
             arn_breakdown = arn.split(":")
             resource_type = arn_breakdown[len(arn_breakdown) - 2]
             resource_name = arn_breakdown[len(arn_breakdown) - 1]
             if resource_type == "db":  # Database
                 if resource_name in self.databases:
                     return self.databases[resource_name].get_tags()
@@ -2328,56 +2426,56 @@
                     return self.subnet_groups[resource_name].get_tags()
         else:
             raise RDSClientError(
                 "InvalidParameterValue", f"Invalid resource name: {arn}"
             )
         return []
 
-    def remove_tags_from_resource(self, arn, tag_keys):
+    def remove_tags_from_resource(self, arn: str, tag_keys: List[str]) -> None:
         if self.arn_regex.match(arn):
             arn_breakdown = arn.split(":")
             resource_type = arn_breakdown[len(arn_breakdown) - 2]
             resource_name = arn_breakdown[len(arn_breakdown) - 1]
             if resource_type == "db":  # Database
                 if resource_name in self.databases:
-                    return self.databases[resource_name].remove_tags(tag_keys)
+                    self.databases[resource_name].remove_tags(tag_keys)
             elif resource_type == "es":  # Event Subscription
                 if resource_name in self.event_subscriptions:
-                    return self.event_subscriptions[resource_name].remove_tags(tag_keys)
+                    self.event_subscriptions[resource_name].remove_tags(tag_keys)
             elif resource_type == "og":  # Option Group
                 if resource_name in self.option_groups:
-                    return self.option_groups[resource_name].remove_tags(tag_keys)
+                    self.option_groups[resource_name].remove_tags(tag_keys)
             elif resource_type == "pg":  # Parameter Group
                 if resource_name in self.db_parameter_groups:
-                    return self.db_parameter_groups[resource_name].remove_tags(tag_keys)
+                    self.db_parameter_groups[resource_name].remove_tags(tag_keys)
             elif resource_type == "ri":  # Reserved DB instance
                 return None
             elif resource_type == "secgrp":  # DB security group
                 if resource_name in self.security_groups:
-                    return self.security_groups[resource_name].remove_tags(tag_keys)
+                    self.security_groups[resource_name].remove_tags(tag_keys)
             elif resource_type == "snapshot":  # DB Snapshot
                 if resource_name in self.database_snapshots:
-                    return self.database_snapshots[resource_name].remove_tags(tag_keys)
+                    self.database_snapshots[resource_name].remove_tags(tag_keys)
             elif resource_type == "cluster":
                 if resource_name in self.clusters:
-                    return self.clusters[resource_name].remove_tags(tag_keys)
+                    self.clusters[resource_name].remove_tags(tag_keys)
                 if resource_name in self.neptune.clusters:
-                    return self.neptune.clusters[resource_name].remove_tags(tag_keys)
+                    self.neptune.clusters[resource_name].remove_tags(tag_keys)
             elif resource_type == "cluster-snapshot":  # DB Cluster Snapshot
                 if resource_name in self.cluster_snapshots:
-                    return self.cluster_snapshots[resource_name].remove_tags(tag_keys)
+                    self.cluster_snapshots[resource_name].remove_tags(tag_keys)
             elif resource_type == "subgrp":  # DB subnet group
                 if resource_name in self.subnet_groups:
-                    return self.subnet_groups[resource_name].remove_tags(tag_keys)
+                    self.subnet_groups[resource_name].remove_tags(tag_keys)
         else:
             raise RDSClientError(
                 "InvalidParameterValue", f"Invalid resource name: {arn}"
             )
 
-    def add_tags_to_resource(self, arn, tags):
+    def add_tags_to_resource(self, arn: str, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:  # type: ignore[return]
         if self.arn_regex.match(arn):
             arn_breakdown = arn.split(":")
             resource_type = arn_breakdown[-2]
             resource_name = arn_breakdown[-1]
             if resource_type == "db":  # Database
                 if resource_name in self.databases:
                     return self.databases[resource_name].add_tags(tags)
@@ -2411,33 +2509,35 @@
                     return self.subnet_groups[resource_name].add_tags(tags)
         else:
             raise RDSClientError(
                 "InvalidParameterValue", f"Invalid resource name: {arn}"
             )
 
     @staticmethod
-    def _filter_resources(resources, filters, resource_class):
+    def _filter_resources(resources: Any, filters: Any, resource_class: Any) -> Any:  # type: ignore[misc]
         try:
             filter_defs = resource_class.SUPPORTED_FILTERS
             validate_filters(filters, filter_defs)
             return apply_filter(resources, filters, filter_defs)
         except KeyError as e:
             # https://stackoverflow.com/questions/24998968/why-does-strkeyerror-add-extra-quotes
             raise InvalidParameterValue(e.args[0])
         except ValueError as e:
             raise InvalidParameterCombination(str(e))
 
     @staticmethod
-    def _merge_tags(old_tags: list, new_tags: list):
+    def _merge_tags(old_tags: List[Dict[str, Any]], new_tags: List[Dict[str, Any]]) -> List[Dict[str, Any]]:  # type: ignore[misc]
         tags_dict = dict()
         tags_dict.update({d["Key"]: d["Value"] for d in old_tags})
         tags_dict.update({d["Key"]: d["Value"] for d in new_tags})
         return [{"Key": k, "Value": v} for k, v in tags_dict.items()]
 
-    def describe_orderable_db_instance_options(self, engine, engine_version):
+    def describe_orderable_db_instance_options(
+        self, engine: str, engine_version: str
+    ) -> List[Dict[str, Any]]:
         """
         Only the Aurora-Postgresql and Neptune-engine is currently implemented
         """
         if engine == "neptune":
             return self.neptune.describe_orderable_db_instance_options(engine_version)
         if engine == "aurora-postgresql":
             if engine_version:
@@ -2447,46 +2547,48 @@
                     if option["EngineVersion"] == engine_version
                 ]
             return self.db_cluster_options
         return []
 
     def create_db_cluster_parameter_group(
         self,
-        group_name,
-        family,
-        description,
-    ):
+        group_name: str,
+        family: str,
+        description: str,
+    ) -> "DBClusterParameterGroup":
         group = DBClusterParameterGroup(
             account_id=self.account_id,
             region=self.region_name,
             name=group_name,
             family=family,
             description=description,
         )
         self.db_cluster_parameter_groups[group_name] = group
         return group
 
-    def describe_db_cluster_parameter_groups(self, group_name):
+    def describe_db_cluster_parameter_groups(
+        self, group_name: str
+    ) -> List["DBClusterParameterGroup"]:
         if group_name is not None:
             if group_name not in self.db_cluster_parameter_groups:
                 raise DBClusterParameterGroupNotFoundError(group_name)
             return [self.db_cluster_parameter_groups[group_name]]
         return list(self.db_cluster_parameter_groups.values())
 
-    def delete_db_cluster_parameter_group(self, group_name):
+    def delete_db_cluster_parameter_group(self, group_name: str) -> None:
         self.db_cluster_parameter_groups.pop(group_name)
 
     def create_global_cluster(
         self,
         global_cluster_identifier: str,
         source_db_cluster_identifier: Optional[str],
         engine: Optional[str],
         engine_version: Optional[str],
-        storage_encrypted: Optional[bool],
-        deletion_protection: Optional[bool],
+        storage_encrypted: Optional[str],
+        deletion_protection: Optional[str],
     ) -> GlobalCluster:
         source_cluster = None
         if source_db_cluster_identifier is not None:
             # validate our source cluster exists
             if not source_db_cluster_identifier.startswith("arn:aws:rds"):
                 raise InvalidParameterValue("Malformed db cluster arn dbci")
             source_cluster = self.describe_db_clusters(
@@ -2502,182 +2604,199 @@
         elif engine is None:
             raise InvalidParameterValue(
                 "When creating standalone global cluster, value for engineName should be specified"
             )
         global_cluster = GlobalCluster(
             account_id=self.account_id,
             global_cluster_identifier=global_cluster_identifier,
-            engine=engine,
+            engine=engine,  # type: ignore
             engine_version=engine_version,
             storage_encrypted=storage_encrypted,
             deletion_protection=deletion_protection,
         )
         self.global_clusters[global_cluster_identifier] = global_cluster
         if source_cluster is not None:
             source_cluster.global_cluster_identifier = global_cluster.global_cluster_arn
             global_cluster.members.append(source_cluster.db_cluster_arn)
         return global_cluster
 
-    def describe_global_clusters(self):
+    def describe_global_clusters(self) -> List[GlobalCluster]:
         return (
             list(self.global_clusters.values())
-            + self.neptune.describe_global_clusters()
+            + self.neptune.describe_global_clusters()  # type: ignore
         )
 
     def delete_global_cluster(self, global_cluster_identifier: str) -> GlobalCluster:
         try:
-            return self.neptune.delete_global_cluster(global_cluster_identifier)
+            return self.neptune.delete_global_cluster(global_cluster_identifier)  # type: ignore
         except:  # noqa: E722 Do not use bare except
             pass  # It's not a Neptune Global Cluster - assume it's an RDS cluster instead
         global_cluster = self.global_clusters[global_cluster_identifier]
         if global_cluster.members:
             raise InvalidGlobalClusterStateFault(global_cluster.global_cluster_arn)
         return self.global_clusters.pop(global_cluster_identifier)
 
     def remove_from_global_cluster(
         self, global_cluster_identifier: str, db_cluster_identifier: str
-    ) -> GlobalCluster:
+    ) -> Optional[GlobalCluster]:
         try:
             global_cluster = self.global_clusters[global_cluster_identifier]
             cluster = self.describe_db_clusters(
                 cluster_identifier=db_cluster_identifier
             )[0]
             global_cluster.members.remove(cluster.db_cluster_arn)
             return global_cluster
         except:  # noqa: E722 Do not use bare except
             pass
         return None
 
 
-class OptionGroup(object):
+class OptionGroup:
     def __init__(
         self,
-        name,
-        engine_name,
-        major_engine_version,
-        region,
-        account_id,
-        description=None,
+        name: str,
+        engine_name: str,
+        major_engine_version: str,
+        region: str,
+        account_id: str,
+        description: Optional[str] = None,
     ):
         self.engine_name = engine_name
         self.major_engine_version = major_engine_version
         self.description = description
         self.name = name
         self.vpc_and_non_vpc_instance_memberships = False
-        self.options = {}
+        self.options: Dict[str, Any] = {}
         self.vpcId = "null"
-        self.tags = []
+        self.tags: List[Dict[str, str]] = []
         self.arn = f"arn:aws:rds:{region}:{account_id}:og:{name}"
 
-    def to_json(self):
+    def to_json(self) -> str:
         template = Template(
             """{
     "VpcId": null,
     "MajorEngineVersion": "{{ option_group.major_engine_version }}",
     "OptionGroupDescription": "{{ option_group.description }}",
     "AllowsVpcAndNonVpcInstanceMemberships": "{{ option_group.vpc_and_non_vpc_instance_memberships }}",
     "EngineName": "{{ option_group.engine_name }}",
     "Options": [],
     "OptionGroupName": "{{ option_group.name }},
     "OptionGroupArn": "{{ option_group.arn }}
 }"""
         )
         return template.render(option_group=self)
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<OptionGroup>
           <OptionGroupName>{{ option_group.name }}</OptionGroupName>
           <AllowsVpcAndNonVpcInstanceMemberships>{{ option_group.vpc_and_non_vpc_instance_memberships }}</AllowsVpcAndNonVpcInstanceMemberships>
           <MajorEngineVersion>{{ option_group.major_engine_version }}</MajorEngineVersion>
           <EngineName>{{ option_group.engine_name }}</EngineName>
           <OptionGroupDescription>{{ option_group.description }}</OptionGroupDescription>
           <OptionGroupArn>{{ option_group.arn }}</OptionGroupArn>
           <Options/>
         </OptionGroup>"""
         )
         return template.render(option_group=self)
 
-    def remove_options(self, options_to_remove):  # pylint: disable=unused-argument
+    def remove_options(
+        self, options_to_remove: Any  # pylint: disable=unused-argument
+    ) -> None:
         # TODO: Check for option in self.options and remove if exists. Raise
         # error otherwise
         return
 
-    def add_options(self, options_to_add):  # pylint: disable=unused-argument
+    def add_options(
+        self, options_to_add: Any  # pylint: disable=unused-argument
+    ) -> None:
         # TODO: Validate option and add it to self.options. If invalid raise
         # error
         return
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, str]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, str]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
 
 class DBParameterGroup(CloudFormationModel):
-    def __init__(self, account_id, name, description, family, tags, region):
+    def __init__(
+        self,
+        account_id: str,
+        name: Optional[str],
+        description: str,
+        family: Optional[str],
+        tags: List[Dict[str, str]],
+        region: str,
+    ):
         self.name = name
         self.description = description
         self.family = family
         self.tags = tags
-        self.parameters = defaultdict(dict)
+        self.parameters: Dict[str, Any] = defaultdict(dict)
         self.arn = f"arn:aws:rds:{region}:{account_id}:pg:{name}"
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<DBParameterGroup>
           <DBParameterGroupName>{{ param_group.name }}</DBParameterGroupName>
           <DBParameterGroupFamily>{{ param_group.family }}</DBParameterGroupFamily>
           <Description>{{ param_group.description }}</Description>
           <DBParameterGroupArn>{{ param_group.arn }}</DBParameterGroupArn>
         </DBParameterGroup>"""
         )
         return template.render(param_group=self)
 
-    def get_tags(self):
+    def get_tags(self) -> List[Dict[str, Any]]:
         return self.tags
 
-    def add_tags(self, tags):
+    def add_tags(self, tags: List[Dict[str, str]]) -> List[Dict[str, Any]]:
         new_keys = [tag_set["Key"] for tag_set in tags]
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in new_keys]
         self.tags.extend(tags)
         return self.tags
 
-    def remove_tags(self, tag_keys):
+    def remove_tags(self, tag_keys: List[str]) -> None:
         self.tags = [tag_set for tag_set in self.tags if tag_set["Key"] not in tag_keys]
 
-    def update_parameters(self, new_parameters):
+    def update_parameters(self, new_parameters: Iterable[Dict[str, Any]]) -> None:
         for new_parameter in new_parameters:
             parameter = self.parameters[new_parameter["ParameterName"]]
             parameter.update(new_parameter)
 
-    def delete(self, account_id, region_name):
+    def delete(self, account_id: str, region_name: str) -> None:
         backend = rds_backends[account_id][region_name]
         backend.delete_db_parameter_group(self.name)
 
     @staticmethod
-    def cloudformation_name_type():
-        return None
+    def cloudformation_name_type() -> str:
+        return ""
 
     @staticmethod
-    def cloudformation_type():
+    def cloudformation_type() -> str:
         # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-rds-dbparametergroup.html
         return "AWS::RDS::DBParameterGroup"
 
     @classmethod
-    def create_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name, **kwargs
-    ):
+    def create_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+        **kwargs: Any,
+    ) -> "DBParameterGroup":
         properties = cloudformation_json["Properties"]
 
         db_parameter_group_kwargs = {
             "description": properties["Description"],
             "family": properties["Family"],
             "name": resource_name.lower(),
             "tags": properties.get("Tags"),
@@ -2695,22 +2814,24 @@
             db_parameter_group_kwargs
         )
         db_parameter_group.update_parameters(db_parameter_group_parameters)
         return db_parameter_group
 
 
 class DBClusterParameterGroup(CloudFormationModel):
-    def __init__(self, account_id, region, name, description, family):
+    def __init__(
+        self, account_id: str, region: str, name: str, description: str, family: str
+    ):
         self.name = name
         self.description = description
         self.family = family
-        self.parameters = defaultdict(dict)
+        self.parameters: Dict[str, Any] = defaultdict(dict)
         self.arn = f"arn:aws:rds:{region}:{account_id}:cpg:{name}"
 
-    def to_xml(self):
+    def to_xml(self) -> str:
         template = Template(
             """<DBClusterParameterGroup>
           <DBClusterParameterGroupName>{{ param_group.name }}</DBClusterParameterGroupName>
           <DBParameterGroupFamily>{{ param_group.family }}</DBParameterGroupFamily>
           <Description>{{ param_group.description }}</Description>
           <DBClusterParameterGroupArn>{{ param_group.arn }}</DBClusterParameterGroupArn>
         </DBClusterParameterGroup>"""
```

### Comparing `moto-4.1.8.dev5/moto/rds/resources/cluster_options/aurora-postgresql.json` & `moto-4.1.8.dev6/moto/rds/resources/cluster_options/aurora-postgresql.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/rds/resources/cluster_options/neptune.json` & `moto-4.1.8.dev6/moto/rds/resources/cluster_options/neptune.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/rds/responses.py` & `moto-4.1.8.dev6/moto/rds/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Any
+from typing import Any, Dict, List, Iterable
 
 from moto.core.common_types import TYPE_RESPONSE
 from moto.core.responses import BaseResponse
 from moto.ec2.models import ec2_backends
 from moto.neptune.responses import NeptuneResponse
 from moto.neptune.responses import (
     CREATE_GLOBAL_CLUSTER_TEMPLATE,
@@ -12,36 +12,36 @@
     REMOVE_FROM_GLOBAL_CLUSTER_TEMPLATE,
 )
 from .models import rds_backends, RDSBackend
 from .exceptions import DBParameterGroupNotFoundError
 
 
 class RDSResponse(BaseResponse):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(service_name="rds")
         # Neptune and RDS share a HTTP endpoint RDS is the lucky guy that catches all requests
         # So we have to determine whether we can handle an incoming request here, or whether it needs redirecting to Neptune
         self.neptune = NeptuneResponse()
 
     @property
     def backend(self) -> RDSBackend:
         return rds_backends[self.current_account][self.region]
 
     def _dispatch(self, request: Any, full_url: str, headers: Any) -> TYPE_RESPONSE:
         # Because some requests are send through to Neptune, we have to prepare the NeptuneResponse-class
         self.neptune.setup_class(request, full_url, headers)
         return super()._dispatch(request, full_url, headers)
 
-    def __getattribute__(self, name: str):
+    def __getattribute__(self, name: str) -> Any:
         if name in ["create_db_cluster", "create_global_cluster"]:
             if self._get_param("Engine") == "neptune":
                 return object.__getattribute__(self.neptune, name)
         return object.__getattribute__(self, name)
 
-    def _get_db_kwargs(self):
+    def _get_db_kwargs(self) -> Dict[str, Any]:
         args = {
             "auto_minor_version_upgrade": self._get_param("AutoMinorVersionUpgrade"),
             "allocated_storage": self._get_int_param("AllocatedStorage"),
             "availability_zone": self._get_param("AvailabilityZone"),
             "backup_retention_period": self._get_param("BackupRetentionPeriod"),
             "copy_tags_to_snapshot": self._get_param("CopyTagsToSnapshot"),
             "db_instance_class": self._get_param("DBInstanceClass"),
@@ -86,15 +86,15 @@
             ),
             "tags": list(),
             "deletion_protection": self._get_bool_param("DeletionProtection"),
         }
         args["tags"] = self.unpack_list_params("Tags", "Tag")
         return args
 
-    def _get_modify_db_cluster_kwargs(self):
+    def _get_modify_db_cluster_kwargs(self) -> Dict[str, Any]:
         args = {
             "auto_minor_version_upgrade": self._get_param("AutoMinorVersionUpgrade"),
             "allocated_storage": self._get_int_param("AllocatedStorage"),
             "availability_zone": self._get_param("AvailabilityZone"),
             "backup_retention_period": self._get_param("BackupRetentionPeriod"),
             "copy_tags_to_snapshot": self._get_param("CopyTagsToSnapshot"),
             "db_instance_class": self._get_param("DBInstanceClass"),
@@ -142,46 +142,46 @@
             ),
             "tags": list(),
             "deletion_protection": self._get_bool_param("DeletionProtection"),
         }
         args["tags"] = self.unpack_list_params("Tags", "Tag")
         return args
 
-    def _get_db_replica_kwargs(self):
+    def _get_db_replica_kwargs(self) -> Dict[str, Any]:
         return {
             "auto_minor_version_upgrade": self._get_param("AutoMinorVersionUpgrade"),
             "availability_zone": self._get_param("AvailabilityZone"),
             "db_instance_class": self._get_param("DBInstanceClass"),
             "db_instance_identifier": self._get_param("DBInstanceIdentifier"),
             "db_subnet_group_name": self._get_param("DBSubnetGroupName"),
             "iops": self._get_int_param("Iops"),
             # OptionGroupName
             "port": self._get_param("Port"),
             "publicly_accessible": self._get_param("PubliclyAccessible"),
             "source_db_identifier": self._get_param("SourceDBInstanceIdentifier"),
             "storage_type": self._get_param("StorageType"),
         }
 
-    def _get_option_group_kwargs(self):
+    def _get_option_group_kwargs(self) -> Dict[str, Any]:
         return {
             "major_engine_version": self._get_param("MajorEngineVersion"),
             "description": self._get_param("OptionGroupDescription"),
             "engine_name": self._get_param("EngineName"),
             "name": self._get_param("OptionGroupName"),
         }
 
-    def _get_db_parameter_group_kwargs(self):
+    def _get_db_parameter_group_kwargs(self) -> Dict[str, Any]:
         return {
             "description": self._get_param("Description"),
             "family": self._get_param("DBParameterGroupFamily"),
             "name": self._get_param("DBParameterGroupName"),
             "tags": self.unpack_list_params("Tags", "Tag"),
         }
 
-    def _get_db_cluster_kwargs(self):
+    def _get_db_cluster_kwargs(self) -> Dict[str, Any]:
         return {
             "availability_zones": self._get_multi_param(
                 "AvailabilityZones.AvailabilityZone"
             ),
             "enable_cloudwatch_logs_exports": self._get_params().get(
                 "EnableCloudwatchLogsExports"
             ),
@@ -209,61 +209,63 @@
             "tags": self.unpack_list_params("Tags", "Tag"),
             "scaling_configuration": self._get_dict_param("ScalingConfiguration."),
             "replication_source_identifier": self._get_param(
                 "ReplicationSourceIdentifier"
             ),
         }
 
-    def _get_export_task_kwargs(self):
+    def _get_export_task_kwargs(self) -> Dict[str, Any]:
         return {
             "export_task_identifier": self._get_param("ExportTaskIdentifier"),
             "source_arn": self._get_param("SourceArn"),
             "s3_bucket_name": self._get_param("S3BucketName"),
             "iam_role_arn": self._get_param("IamRoleArn"),
             "kms_key_id": self._get_param("KmsKeyId"),
             "s3_prefix": self._get_param("S3Prefix"),
             "export_only": self.unpack_list_params("ExportOnly", "member"),
         }
 
-    def _get_event_subscription_kwargs(self):
+    def _get_event_subscription_kwargs(self) -> Dict[str, Any]:
         return {
             "subscription_name": self._get_param("SubscriptionName"),
             "sns_topic_arn": self._get_param("SnsTopicArn"),
             "source_type": self._get_param("SourceType"),
             "event_categories": self.unpack_list_params(
                 "EventCategories", "EventCategory"
             ),
             "source_ids": self.unpack_list_params("SourceIds", "SourceId"),
             "enabled": self._get_param("Enabled"),
             "tags": self.unpack_list_params("Tags", "Tag"),
         }
 
-    def unpack_list_params(self, label, child_label):
+    def unpack_list_params(self, label: str, child_label: str) -> List[Dict[str, Any]]:
         root = self._get_multi_param_dict(label) or {}
         return root.get(child_label, [])
 
-    def create_db_instance(self):
+    def create_db_instance(self) -> str:
         db_kwargs = self._get_db_kwargs()
         database = self.backend.create_db_instance(db_kwargs)
         template = self.response_template(CREATE_DATABASE_TEMPLATE)
         return template.render(database=database)
 
-    def create_db_instance_read_replica(self):
+    def create_db_instance_read_replica(self) -> str:
         db_kwargs = self._get_db_replica_kwargs()
 
         database = self.backend.create_db_instance_read_replica(db_kwargs)
         template = self.response_template(CREATE_DATABASE_REPLICA_TEMPLATE)
         return template.render(database=database)
 
-    def describe_db_instances(self):
+    def describe_db_instances(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         filters = self._get_multi_param("Filters.Filter.")
-        filters = {f["Name"]: f["Values"] for f in filters}
+        filter_dict = {f["Name"]: f["Values"] for f in filters}
         all_instances = list(
-            self.backend.describe_db_instances(db_instance_identifier, filters=filters)
+            self.backend.describe_db_instances(
+                db_instance_identifier, filters=filter_dict
+            )
         )
         marker = self._get_param("Marker")
         all_ids = [instance.db_instance_identifier for instance in all_instances]
         if marker:
             start = all_ids.index(marker) + 1
         else:
             start = 0
@@ -274,231 +276,230 @@
         next_marker = None
         if len(all_instances) > start + page_size:
             next_marker = instances_resp[-1].db_instance_identifier
 
         template = self.response_template(DESCRIBE_DATABASES_TEMPLATE)
         return template.render(databases=instances_resp, marker=next_marker)
 
-    def modify_db_instance(self):
+    def modify_db_instance(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         db_kwargs = self._get_db_kwargs()
         # NOTE modify_db_instance does not support tags
         del db_kwargs["tags"]
         new_db_instance_identifier = self._get_param("NewDBInstanceIdentifier")
         if new_db_instance_identifier:
             db_kwargs["new_db_instance_identifier"] = new_db_instance_identifier
         database = self.backend.modify_db_instance(db_instance_identifier, db_kwargs)
         template = self.response_template(MODIFY_DATABASE_TEMPLATE)
         return template.render(database=database)
 
-    def delete_db_instance(self):
+    def delete_db_instance(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         db_snapshot_name = self._get_param("FinalDBSnapshotIdentifier")
         database = self.backend.delete_db_instance(
             db_instance_identifier, db_snapshot_name
         )
         template = self.response_template(DELETE_DATABASE_TEMPLATE)
         return template.render(database=database)
 
-    def reboot_db_instance(self):
+    def reboot_db_instance(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         database = self.backend.reboot_db_instance(db_instance_identifier)
         template = self.response_template(REBOOT_DATABASE_TEMPLATE)
         return template.render(database=database)
 
-    def create_db_snapshot(self):
+    def create_db_snapshot(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         db_snapshot_identifier = self._get_param("DBSnapshotIdentifier")
         tags = self.unpack_list_params("Tags", "Tag")
         snapshot = self.backend.create_db_snapshot(
             db_instance_identifier, db_snapshot_identifier, tags
         )
         template = self.response_template(CREATE_SNAPSHOT_TEMPLATE)
         return template.render(snapshot=snapshot)
 
-    def copy_db_snapshot(self):
+    def copy_db_snapshot(self) -> str:
         source_snapshot_identifier = self._get_param("SourceDBSnapshotIdentifier")
         target_snapshot_identifier = self._get_param("TargetDBSnapshotIdentifier")
         tags = self.unpack_list_params("Tags", "Tag")
         snapshot = self.backend.copy_database_snapshot(
             source_snapshot_identifier, target_snapshot_identifier, tags
         )
         template = self.response_template(COPY_SNAPSHOT_TEMPLATE)
         return template.render(snapshot=snapshot)
 
-    def describe_db_snapshots(self):
+    def describe_db_snapshots(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         db_snapshot_identifier = self._get_param("DBSnapshotIdentifier")
         filters = self._get_multi_param("Filters.Filter.")
-        filters = {f["Name"]: f["Values"] for f in filters}
+        filter_dict = {f["Name"]: f["Values"] for f in filters}
         snapshots = self.backend.describe_db_snapshots(
-            db_instance_identifier, db_snapshot_identifier, filters
+            db_instance_identifier, db_snapshot_identifier, filter_dict
         )
         template = self.response_template(DESCRIBE_SNAPSHOTS_TEMPLATE)
         return template.render(snapshots=snapshots)
 
-    def promote_read_replica(self):
+    def promote_read_replica(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         db_kwargs = self._get_db_kwargs()
         database = self.backend.promote_read_replica(db_kwargs)
         database = self.backend.modify_db_instance(db_instance_identifier, db_kwargs)
         template = self.response_template(PROMOTE_REPLICA_TEMPLATE)
         return template.render(database=database)
 
-    def delete_db_snapshot(self):
+    def delete_db_snapshot(self) -> str:
         db_snapshot_identifier = self._get_param("DBSnapshotIdentifier")
         snapshot = self.backend.delete_db_snapshot(db_snapshot_identifier)
         template = self.response_template(DELETE_SNAPSHOT_TEMPLATE)
         return template.render(snapshot=snapshot)
 
-    def restore_db_instance_from_db_snapshot(self):
+    def restore_db_instance_from_db_snapshot(self) -> str:
         db_snapshot_identifier = self._get_param("DBSnapshotIdentifier")
         db_kwargs = self._get_db_kwargs()
         new_instance = self.backend.restore_db_instance_from_db_snapshot(
             db_snapshot_identifier, db_kwargs
         )
         template = self.response_template(RESTORE_INSTANCE_FROM_SNAPSHOT_TEMPLATE)
         return template.render(database=new_instance)
 
-    def list_tags_for_resource(self):
+    def list_tags_for_resource(self) -> str:
         arn = self._get_param("ResourceName")
         template = self.response_template(LIST_TAGS_FOR_RESOURCE_TEMPLATE)
         tags = self.backend.list_tags_for_resource(arn)
         return template.render(tags=tags)
 
-    def add_tags_to_resource(self):
+    def add_tags_to_resource(self) -> str:
         arn = self._get_param("ResourceName")
         tags = self.unpack_list_params("Tags", "Tag")
         tags = self.backend.add_tags_to_resource(arn, tags)
         template = self.response_template(ADD_TAGS_TO_RESOURCE_TEMPLATE)
         return template.render(tags=tags)
 
-    def remove_tags_from_resource(self):
+    def remove_tags_from_resource(self) -> str:
         arn = self._get_param("ResourceName")
         tag_keys = self.unpack_list_params("TagKeys", "member")
-        self.backend.remove_tags_from_resource(arn, tag_keys)
+        self.backend.remove_tags_from_resource(arn, tag_keys)  # type: ignore
         template = self.response_template(REMOVE_TAGS_FROM_RESOURCE_TEMPLATE)
         return template.render()
 
-    def stop_db_instance(self):
+    def stop_db_instance(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         db_snapshot_identifier = self._get_param("DBSnapshotIdentifier")
         database = self.backend.stop_db_instance(
             db_instance_identifier, db_snapshot_identifier
         )
         template = self.response_template(STOP_DATABASE_TEMPLATE)
         return template.render(database=database)
 
-    def start_db_instance(self):
+    def start_db_instance(self) -> str:
         db_instance_identifier = self._get_param("DBInstanceIdentifier")
         database = self.backend.start_db_instance(db_instance_identifier)
         template = self.response_template(START_DATABASE_TEMPLATE)
         return template.render(database=database)
 
-    def create_db_security_group(self):
+    def create_db_security_group(self) -> str:
         group_name = self._get_param("DBSecurityGroupName")
         description = self._get_param("DBSecurityGroupDescription")
         tags = self.unpack_list_params("Tags", "Tag")
         security_group = self.backend.create_db_security_group(
             group_name, description, tags
         )
         template = self.response_template(CREATE_SECURITY_GROUP_TEMPLATE)
         return template.render(security_group=security_group)
 
-    def describe_db_security_groups(self):
+    def describe_db_security_groups(self) -> str:
         security_group_name = self._get_param("DBSecurityGroupName")
         security_groups = self.backend.describe_security_groups(security_group_name)
         template = self.response_template(DESCRIBE_SECURITY_GROUPS_TEMPLATE)
         return template.render(security_groups=security_groups)
 
-    def delete_db_security_group(self):
+    def delete_db_security_group(self) -> str:
         security_group_name = self._get_param("DBSecurityGroupName")
         security_group = self.backend.delete_security_group(security_group_name)
         template = self.response_template(DELETE_SECURITY_GROUP_TEMPLATE)
         return template.render(security_group=security_group)
 
-    def authorize_db_security_group_ingress(self):
+    def authorize_db_security_group_ingress(self) -> str:
         security_group_name = self._get_param("DBSecurityGroupName")
         cidr_ip = self._get_param("CIDRIP")
         security_group = self.backend.authorize_security_group(
             security_group_name, cidr_ip
         )
         template = self.response_template(AUTHORIZE_SECURITY_GROUP_TEMPLATE)
         return template.render(security_group=security_group)
 
-    def create_db_subnet_group(self):
+    def create_db_subnet_group(self) -> str:
         subnet_name = self._get_param("DBSubnetGroupName")
         description = self._get_param("DBSubnetGroupDescription")
         subnet_ids = self._get_multi_param("SubnetIds.SubnetIdentifier")
         tags = self.unpack_list_params("Tags", "Tag")
         subnets = [
             ec2_backends[self.current_account][self.region].get_subnet(subnet_id)
             for subnet_id in subnet_ids
         ]
         subnet_group = self.backend.create_subnet_group(
             subnet_name, description, subnets, tags
         )
         template = self.response_template(CREATE_SUBNET_GROUP_TEMPLATE)
         return template.render(subnet_group=subnet_group)
 
-    def describe_db_subnet_groups(self):
+    def describe_db_subnet_groups(self) -> str:
         subnet_name = self._get_param("DBSubnetGroupName")
         subnet_groups = self.backend.describe_db_subnet_groups(subnet_name)
         template = self.response_template(DESCRIBE_SUBNET_GROUPS_TEMPLATE)
         return template.render(subnet_groups=subnet_groups)
 
-    def modify_db_subnet_group(self):
+    def modify_db_subnet_group(self) -> str:
         subnet_name = self._get_param("DBSubnetGroupName")
         description = self._get_param("DBSubnetGroupDescription")
         subnet_ids = self._get_multi_param("SubnetIds.SubnetIdentifier")
         subnets = [
             ec2_backends[self.current_account][self.region].get_subnet(subnet_id)
             for subnet_id in subnet_ids
         ]
         subnet_group = self.backend.modify_db_subnet_group(
             subnet_name, description, subnets
         )
         template = self.response_template(MODIFY_SUBNET_GROUPS_TEMPLATE)
         return template.render(subnet_group=subnet_group)
 
-    def delete_db_subnet_group(self):
+    def delete_db_subnet_group(self) -> str:
         subnet_name = self._get_param("DBSubnetGroupName")
         subnet_group = self.backend.delete_subnet_group(subnet_name)
         template = self.response_template(DELETE_SUBNET_GROUP_TEMPLATE)
         return template.render(subnet_group=subnet_group)
 
-    def create_option_group(self):
+    def create_option_group(self) -> str:
         kwargs = self._get_option_group_kwargs()
         option_group = self.backend.create_option_group(kwargs)
         template = self.response_template(CREATE_OPTION_GROUP_TEMPLATE)
         return template.render(option_group=option_group)
 
-    def delete_option_group(self):
+    def delete_option_group(self) -> str:
         kwargs = self._get_option_group_kwargs()
         option_group = self.backend.delete_option_group(kwargs["name"])
         template = self.response_template(DELETE_OPTION_GROUP_TEMPLATE)
         return template.render(option_group=option_group)
 
-    def describe_option_groups(self):
+    def describe_option_groups(self) -> str:
         kwargs = self._get_option_group_kwargs()
         kwargs["max_records"] = self._get_int_param("MaxRecords")
         kwargs["marker"] = self._get_param("Marker")
         option_groups = self.backend.describe_option_groups(kwargs)
         template = self.response_template(DESCRIBE_OPTION_GROUP_TEMPLATE)
         return template.render(option_groups=option_groups)
 
-    def describe_option_group_options(self):
+    def describe_option_group_options(self) -> str:
         engine_name = self._get_param("EngineName")
         major_engine_version = self._get_param("MajorEngineVersion")
-        option_group_options = self.backend.describe_option_group_options(
+        return self.backend.describe_option_group_options(
             engine_name, major_engine_version
         )
-        return option_group_options
 
-    def modify_option_group(self):
+    def modify_option_group(self) -> str:
         option_group_name = self._get_param("OptionGroupName")
         count = 1
         options_to_include = []
         # TODO: This can probably be refactored with a single call to super.get_multi_param, but there are not enough tests (yet) to verify this
         while self._get_param(f"OptionsToInclude.member.{count}.OptionName"):
             options_to_include.append(
                 {
@@ -526,279 +527,279 @@
             count += 1
         option_group = self.backend.modify_option_group(
             option_group_name, options_to_include, options_to_remove
         )
         template = self.response_template(MODIFY_OPTION_GROUP_TEMPLATE)
         return template.render(option_group=option_group)
 
-    def create_db_parameter_group(self):
+    def create_db_parameter_group(self) -> str:
         kwargs = self._get_db_parameter_group_kwargs()
         db_parameter_group = self.backend.create_db_parameter_group(kwargs)
         template = self.response_template(CREATE_DB_PARAMETER_GROUP_TEMPLATE)
         return template.render(db_parameter_group=db_parameter_group)
 
-    def describe_db_parameter_groups(self):
+    def describe_db_parameter_groups(self) -> str:
         kwargs = self._get_db_parameter_group_kwargs()
         kwargs["max_records"] = self._get_int_param("MaxRecords")
         kwargs["marker"] = self._get_param("Marker")
         db_parameter_groups = self.backend.describe_db_parameter_groups(kwargs)
         template = self.response_template(DESCRIBE_DB_PARAMETER_GROUPS_TEMPLATE)
         return template.render(db_parameter_groups=db_parameter_groups)
 
-    def modify_db_parameter_group(self):
+    def modify_db_parameter_group(self) -> str:
         db_parameter_group_name = self._get_param("DBParameterGroupName")
         db_parameter_group_parameters = self._get_db_parameter_group_parameters()
         db_parameter_group = self.backend.modify_db_parameter_group(
             db_parameter_group_name, db_parameter_group_parameters
         )
         template = self.response_template(MODIFY_DB_PARAMETER_GROUP_TEMPLATE)
         return template.render(db_parameter_group=db_parameter_group)
 
-    def _get_db_parameter_group_parameters(self):
-        parameter_group_parameters = defaultdict(dict)
+    def _get_db_parameter_group_parameters(self) -> Iterable[Dict[str, Any]]:
+        parameter_group_parameters: Dict[str, Any] = defaultdict(dict)
         for param_name, value in self.querystring.items():
             if not param_name.startswith("Parameters.Parameter"):
                 continue
 
             split_param_name = param_name.split(".")
             param_id = split_param_name[2]
             param_setting = split_param_name[3]
 
             parameter_group_parameters[param_id][param_setting] = value[0]
 
         return parameter_group_parameters.values()
 
-    def describe_db_parameters(self):
+    def describe_db_parameters(self) -> str:
         db_parameter_group_name = self._get_param("DBParameterGroupName")
         db_parameter_groups = self.backend.describe_db_parameter_groups(
             {"name": db_parameter_group_name}
         )
         if not db_parameter_groups:
             raise DBParameterGroupNotFoundError(db_parameter_group_name)
 
         template = self.response_template(DESCRIBE_DB_PARAMETERS_TEMPLATE)
         return template.render(db_parameter_group=db_parameter_groups[0])
 
-    def delete_db_parameter_group(self):
+    def delete_db_parameter_group(self) -> str:
         kwargs = self._get_db_parameter_group_kwargs()
         db_parameter_group = self.backend.delete_db_parameter_group(kwargs["name"])
         template = self.response_template(DELETE_DB_PARAMETER_GROUP_TEMPLATE)
         return template.render(db_parameter_group=db_parameter_group)
 
-    def describe_db_cluster_parameters(self):
+    def describe_db_cluster_parameters(self) -> str:
         db_parameter_group_name = self._get_param("DBParameterGroupName")
         db_parameter_groups = self.backend.describe_db_cluster_parameters()
         if db_parameter_groups is None:
             raise DBParameterGroupNotFoundError(db_parameter_group_name)
 
         template = self.response_template(DESCRIBE_DB_CLUSTER_PARAMETERS_TEMPLATE)
         return template.render(db_parameter_group=db_parameter_groups)
 
-    def create_db_cluster(self):
+    def create_db_cluster(self) -> str:
         kwargs = self._get_db_cluster_kwargs()
         cluster = self.backend.create_db_cluster(kwargs)
         template = self.response_template(CREATE_DB_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
-    def modify_db_cluster(self):
+    def modify_db_cluster(self) -> str:
         kwargs = self._get_modify_db_cluster_kwargs()
         cluster = self.backend.modify_db_cluster(kwargs)
         template = self.response_template(MODIFY_DB_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
-    def describe_db_clusters(self):
+    def describe_db_clusters(self) -> str:
         _id = self._get_param("DBClusterIdentifier")
         filters = self._get_multi_param("Filters.Filter.")
-        filters = {f["Name"]: f["Values"] for f in filters}
+        filter_dict = {f["Name"]: f["Values"] for f in filters}
         clusters = self.backend.describe_db_clusters(
-            cluster_identifier=_id, filters=filters
+            cluster_identifier=_id, filters=filter_dict
         )
         template = self.response_template(DESCRIBE_CLUSTERS_TEMPLATE)
         return template.render(clusters=clusters)
 
-    def delete_db_cluster(self):
+    def delete_db_cluster(self) -> str:
         _id = self._get_param("DBClusterIdentifier")
         snapshot_name = self._get_param("FinalDBSnapshotIdentifier")
         cluster = self.backend.delete_db_cluster(
             cluster_identifier=_id, snapshot_name=snapshot_name
         )
         template = self.response_template(DELETE_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
-    def start_db_cluster(self):
+    def start_db_cluster(self) -> str:
         _id = self._get_param("DBClusterIdentifier")
         cluster = self.backend.start_db_cluster(cluster_identifier=_id)
         template = self.response_template(START_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
-    def stop_db_cluster(self):
+    def stop_db_cluster(self) -> str:
         _id = self._get_param("DBClusterIdentifier")
         cluster = self.backend.stop_db_cluster(cluster_identifier=_id)
         template = self.response_template(STOP_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
-    def create_db_cluster_snapshot(self):
+    def create_db_cluster_snapshot(self) -> str:
         db_cluster_identifier = self._get_param("DBClusterIdentifier")
         db_snapshot_identifier = self._get_param("DBClusterSnapshotIdentifier")
         tags = self.unpack_list_params("Tags", "Tag")
         snapshot = self.backend.create_db_cluster_snapshot(
             db_cluster_identifier, db_snapshot_identifier, tags
         )
         template = self.response_template(CREATE_CLUSTER_SNAPSHOT_TEMPLATE)
         return template.render(snapshot=snapshot)
 
-    def copy_db_cluster_snapshot(self):
+    def copy_db_cluster_snapshot(self) -> str:
         source_snapshot_identifier = self._get_param(
             "SourceDBClusterSnapshotIdentifier"
         )
         target_snapshot_identifier = self._get_param(
             "TargetDBClusterSnapshotIdentifier"
         )
         tags = self.unpack_list_params("Tags", "Tag")
         snapshot = self.backend.copy_cluster_snapshot(
             source_snapshot_identifier, target_snapshot_identifier, tags
         )
         template = self.response_template(COPY_CLUSTER_SNAPSHOT_TEMPLATE)
         return template.render(snapshot=snapshot)
 
-    def describe_db_cluster_snapshots(self):
+    def describe_db_cluster_snapshots(self) -> str:
         db_cluster_identifier = self._get_param("DBClusterIdentifier")
         db_snapshot_identifier = self._get_param("DBClusterSnapshotIdentifier")
         filters = self._get_multi_param("Filters.Filter.")
-        filters = {f["Name"]: f["Values"] for f in filters}
+        filter_dict = {f["Name"]: f["Values"] for f in filters}
         snapshots = self.backend.describe_db_cluster_snapshots(
-            db_cluster_identifier, db_snapshot_identifier, filters
+            db_cluster_identifier, db_snapshot_identifier, filter_dict
         )
         template = self.response_template(DESCRIBE_CLUSTER_SNAPSHOTS_TEMPLATE)
         return template.render(snapshots=snapshots)
 
-    def delete_db_cluster_snapshot(self):
+    def delete_db_cluster_snapshot(self) -> str:
         db_snapshot_identifier = self._get_param("DBClusterSnapshotIdentifier")
         snapshot = self.backend.delete_db_cluster_snapshot(db_snapshot_identifier)
         template = self.response_template(DELETE_CLUSTER_SNAPSHOT_TEMPLATE)
         return template.render(snapshot=snapshot)
 
-    def restore_db_cluster_from_snapshot(self):
+    def restore_db_cluster_from_snapshot(self) -> str:
         db_snapshot_identifier = self._get_param("SnapshotIdentifier")
         db_kwargs = self._get_db_cluster_kwargs()
         new_cluster = self.backend.restore_db_cluster_from_snapshot(
             db_snapshot_identifier, db_kwargs
         )
         template = self.response_template(RESTORE_CLUSTER_FROM_SNAPSHOT_TEMPLATE)
         return template.render(cluster=new_cluster)
 
-    def start_export_task(self):
+    def start_export_task(self) -> str:
         kwargs = self._get_export_task_kwargs()
         export_task = self.backend.start_export_task(kwargs)
         template = self.response_template(START_EXPORT_TASK_TEMPLATE)
         return template.render(task=export_task)
 
-    def cancel_export_task(self):
+    def cancel_export_task(self) -> str:
         export_task_identifier = self._get_param("ExportTaskIdentifier")
         export_task = self.backend.cancel_export_task(export_task_identifier)
         template = self.response_template(CANCEL_EXPORT_TASK_TEMPLATE)
         return template.render(task=export_task)
 
-    def describe_export_tasks(self):
+    def describe_export_tasks(self) -> str:
         export_task_identifier = self._get_param("ExportTaskIdentifier")
         tasks = self.backend.describe_export_tasks(export_task_identifier)
         template = self.response_template(DESCRIBE_EXPORT_TASKS_TEMPLATE)
         return template.render(tasks=tasks)
 
-    def create_event_subscription(self):
+    def create_event_subscription(self) -> str:
         kwargs = self._get_event_subscription_kwargs()
         subscription = self.backend.create_event_subscription(kwargs)
         template = self.response_template(CREATE_EVENT_SUBSCRIPTION_TEMPLATE)
         return template.render(subscription=subscription)
 
-    def delete_event_subscription(self):
+    def delete_event_subscription(self) -> str:
         subscription_name = self._get_param("SubscriptionName")
         subscription = self.backend.delete_event_subscription(subscription_name)
         template = self.response_template(DELETE_EVENT_SUBSCRIPTION_TEMPLATE)
         return template.render(subscription=subscription)
 
-    def describe_event_subscriptions(self):
+    def describe_event_subscriptions(self) -> str:
         subscription_name = self._get_param("SubscriptionName")
         subscriptions = self.backend.describe_event_subscriptions(subscription_name)
         template = self.response_template(DESCRIBE_EVENT_SUBSCRIPTIONS_TEMPLATE)
         return template.render(subscriptions=subscriptions)
 
-    def describe_orderable_db_instance_options(self):
+    def describe_orderable_db_instance_options(self) -> str:
         engine = self._get_param("Engine")
         engine_version = self._get_param("EngineVersion")
         options = self.backend.describe_orderable_db_instance_options(
             engine, engine_version
         )
         template = self.response_template(DESCRIBE_ORDERABLE_CLUSTER_OPTIONS)
         return template.render(options=options, marker=None)
 
-    def describe_global_clusters(self):
+    def describe_global_clusters(self) -> str:
         clusters = self.backend.describe_global_clusters()
         template = self.response_template(DESCRIBE_GLOBAL_CLUSTERS_TEMPLATE)
         return template.render(clusters=clusters)
 
-    def create_global_cluster(self):
+    def create_global_cluster(self) -> str:
         params = self._get_params()
         cluster = self.backend.create_global_cluster(
             global_cluster_identifier=params["GlobalClusterIdentifier"],
             source_db_cluster_identifier=params.get("SourceDBClusterIdentifier"),
             engine=params.get("Engine"),
             engine_version=params.get("EngineVersion"),
             storage_encrypted=params.get("StorageEncrypted"),
             deletion_protection=params.get("DeletionProtection"),
         )
         template = self.response_template(CREATE_GLOBAL_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
-    def delete_global_cluster(self):
+    def delete_global_cluster(self) -> str:
         params = self._get_params()
         cluster = self.backend.delete_global_cluster(
             global_cluster_identifier=params["GlobalClusterIdentifier"],
         )
         template = self.response_template(DELETE_GLOBAL_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
-    def remove_from_global_cluster(self):
+    def remove_from_global_cluster(self) -> str:
         params = self._get_params()
         global_cluster = self.backend.remove_from_global_cluster(
             global_cluster_identifier=params["GlobalClusterIdentifier"],
             db_cluster_identifier=params["DbClusterIdentifier"],
         )
         template = self.response_template(REMOVE_FROM_GLOBAL_CLUSTER_TEMPLATE)
         return template.render(cluster=global_cluster)
 
-    def create_db_cluster_parameter_group(self):
+    def create_db_cluster_parameter_group(self) -> str:
         group_name = self._get_param("DBClusterParameterGroupName")
         family = self._get_param("DBParameterGroupFamily")
         desc = self._get_param("Description")
         db_cluster_parameter_group = self.backend.create_db_cluster_parameter_group(
             group_name=group_name,
             family=family,
             description=desc,
         )
         template = self.response_template(CREATE_DB_CLUSTER_PARAMETER_GROUP_TEMPLATE)
         return template.render(db_cluster_parameter_group=db_cluster_parameter_group)
 
-    def describe_db_cluster_parameter_groups(self):
+    def describe_db_cluster_parameter_groups(self) -> str:
         group_name = self._get_param("DBClusterParameterGroupName")
         db_parameter_groups = self.backend.describe_db_cluster_parameter_groups(
             group_name=group_name,
         )
         template = self.response_template(DESCRIBE_DB_CLUSTER_PARAMETER_GROUPS_TEMPLATE)
         return template.render(db_parameter_groups=db_parameter_groups)
 
-    def delete_db_cluster_parameter_group(self):
+    def delete_db_cluster_parameter_group(self) -> str:
         group_name = self._get_param("DBClusterParameterGroupName")
         self.backend.delete_db_cluster_parameter_group(
             group_name=group_name,
         )
         template = self.response_template(DELETE_DB_CLUSTER_PARAMETER_GROUP_TEMPLATE)
         return template.render()
 
-    def promote_read_replica_db_cluster(self):
+    def promote_read_replica_db_cluster(self) -> str:
         db_cluster_identifier = self._get_param("DBClusterIdentifier")
         cluster = self.backend.promote_read_replica_db_cluster(db_cluster_identifier)
         template = self.response_template(PROMOTE_READ_REPLICA_DB_CLUSTER_TEMPLATE)
         return template.render(cluster=cluster)
 
 
 CREATE_DATABASE_TEMPLATE = """<CreateDBInstanceResponse xmlns="http://rds.amazonaws.com/doc/2014-09-01/">
```

### Comparing `moto-4.1.8.dev5/moto/rds/utils.py` & `moto-4.1.8.dev6/moto/rds/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 from collections import namedtuple
-from typing import Any, Dict
+from typing import Any, Dict, Tuple, Optional
 
 from botocore.utils import merge_dicts
 
 from collections import OrderedDict
 import datetime
 import re
 
@@ -18,15 +18,15 @@
         # Description of the filter, e.g. 'Object Identifiers'.
         # Used in filter error messaging.
         "description",
     ],
 )
 
 
-def get_object_value(obj, attr):
+def get_object_value(obj: Any, attr: str) -> Any:
     """Retrieves an arbitrary attribute value from an object.
 
     Nested attributes can be specified using dot notation,
     e.g. 'parent.child'.
 
     :param object obj:
         A valid Python object.
@@ -43,15 +43,17 @@
         if hasattr(val, key):
             val = getattr(val, key)
         else:
             return None
     return val
 
 
-def merge_filters(filters_to_update, filters_to_merge):
+def merge_filters(
+    filters_to_update: Optional[Dict[str, Any]], filters_to_merge: Dict[str, Any]
+) -> Dict[str, Any]:
     """Given two groups of filters, merge the second into the first.
 
     List values are appended instead of overwritten:
 
     >>> merge_filters({'filter-name': ['value1']}, {'filter-name':['value2']})
     >>> {'filter-name': ['value1', 'value2']}
 
@@ -72,15 +74,17 @@
         filters_to_update = {}
     if filters_to_merge is None:
         filters_to_merge = {}
     merge_dicts(filters_to_update, filters_to_merge, append_lists=True)
     return filters_to_update
 
 
-def validate_filters(filters, filter_defs):
+def validate_filters(
+    filters: Dict[str, Any], filter_defs: Dict[str, FilterDef]
+) -> None:
     """Validates filters against a set of filter definitions.
 
     Raises standard Python exceptions which should be caught
     and translated to an appropriate AWS/Moto exception higher
     up the call stack.
 
     :param dict[str, list] filters:
@@ -104,15 +108,15 @@
             raise ValueError(f"The list of {filter_def.description} must not be empty.")
         if filter_def.attrs_to_check is None:
             raise NotImplementedError(
                 f"{filter_name} filter has not been implemented in Moto yet."
             )
 
 
-def apply_filter(resources, filters, filter_defs):
+def apply_filter(resources: Any, filters: Any, filter_defs: Any) -> Any:
     """Apply an arbitrary filter to a group of resources.
 
     :param dict[str, object] resources:
         A dictionary mapping resource identifiers to resource objects.
     :param dict[str, list] filters:
         The filters to apply.
     :param dict[str, FilterDef] filter_defs:
@@ -136,15 +140,17 @@
             if not matches_filter:
                 break
         if matches_filter:
             resources_filtered[identifier] = obj
     return resources_filtered
 
 
-def get_start_date_end_date(base_date, window):
+def get_start_date_end_date(
+    base_date: str, window: str
+) -> Tuple[datetime.datetime, datetime.datetime]:
     """Gets the start date and end date given DDD:HH24:MM-DDD:HH24:MM.
 
     :param base_date:
         type datetime
     :param window:
         DDD:HH24:MM-DDD:HH24:MM
     :returns:
@@ -158,19 +164,19 @@
     ) + datetime.timedelta(days=days[window[0:3]])
     end = datetime.datetime.strptime(
         base_date + " " + window[14::], "%d/%m/%y %H:%M"
     ) + datetime.timedelta(days=days[window[10:13]])
     return start, end
 
 
-def get_start_date_end_date_from_time(base_date, window):
+def get_start_date_end_date_from_time(
+    base_date: str, window: str
+) -> Tuple[datetime.datetime, datetime.datetime, bool]:
     """Gets the start date and end date given HH24:MM-HH24:MM.
 
-    :param base_date:
-        type datetime
     :param window:
         HH24:MM-HH24:MM
     :returns:
         Start and End Date in datetime format
         along with flag for spills over a day
         This is useful when determine time overlaps
     :rtype:
@@ -183,39 +189,31 @@
     if end < start:
         end += datetime.timedelta(days=1)
         spillover = True
     return start, end, spillover
 
 
 def get_overlap_between_two_date_ranges(
-    start_time_1, end_time_1, start_time_2, end_time_2
-):
-    """Determines overlap between 2 date ranges.
-
-    :param start_time_1:
-        type datetime
-    :param start_time_2:
-        type datetime
-    :param end_time_1:
-        type datetime
-    :param end_time_2:
-        type datetime
-    :returns:
-        overlap in seconds
-    :rtype:
-        int
+    start_time_1: datetime.datetime,
+    end_time_1: datetime.datetime,
+    start_time_2: datetime.datetime,
+    end_time_2: datetime.datetime,
+) -> int:
+    """
+    Determines overlap between 2 date ranges. Returns the overlap in seconds.
     """
     latest_start = max(start_time_1, start_time_2)
     earliest_end = min(end_time_1, end_time_2)
     delta = earliest_end - latest_start
-    overlap = (delta.days * SECONDS_IN_ONE_DAY) + delta.seconds
-    return overlap
+    return (delta.days * SECONDS_IN_ONE_DAY) + delta.seconds
 
 
-def valid_preferred_maintenance_window(maintenance_window, backup_window):
+def valid_preferred_maintenance_window(
+    maintenance_window: Any, backup_window: Any
+) -> Optional[str]:
     """Determines validity of preferred_maintenance_window
 
     :param maintenance_windown:
         type DDD:HH24:MM-DDD:HH24:MM
     :param backup_window:
         type HH24:MM-HH24:MM
     :returns:
@@ -279,15 +277,15 @@
 
         maintenance_window_start, maintenance_window_end = get_start_date_end_date(
             base_date, maintenance_window
         )
         delta = maintenance_window_end - maintenance_window_start
         delta_seconds = delta.seconds + (delta.days * SECONDS_IN_ONE_DAY)
         if delta_seconds >= MINUTES_30 and delta_seconds <= HOURS_24:
-            return
+            return None
         elif delta_seconds >= 0 and delta_seconds <= MINUTES_30:
             return "The maintenance window must be at least 30 minutes."
         else:
             return "Maintenance window must be less than 24 hours."
     except Exception:
         return f"Invalid day:hour:minute value: {maintenance_window}"
```

### Comparing `moto-4.1.8.dev5/moto/rdsdata/models.py` & `moto-4.1.8.dev6/moto/rdsdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/rdsdata/responses.py` & `moto-4.1.8.dev6/moto/rdsdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/redshift/exceptions.py` & `moto-4.1.8.dev6/moto/redshift/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/redshift/models.py` & `moto-4.1.8.dev6/moto/redshift/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/redshift/responses.py` & `moto-4.1.8.dev6/moto/redshift/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/redshiftdata/models.py` & `moto-4.1.8.dev6/moto/redshiftdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/redshiftdata/responses.py` & `moto-4.1.8.dev6/moto/redshiftdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/rekognition/models.py` & `moto-4.1.8.dev6/moto/rekognition/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/rekognition/responses.py` & `moto-4.1.8.dev6/moto/rekognition/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/resourcegroups/models.py` & `moto-4.1.8.dev6/moto/resourcegroups/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/resourcegroups/responses.py` & `moto-4.1.8.dev6/moto/resourcegroups/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/resourcegroups/urls.py` & `moto-4.1.8.dev6/moto/resourcegroups/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/resourcegroupstaggingapi/models.py` & `moto-4.1.8.dev6/moto/resourcegroupstaggingapi/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/resourcegroupstaggingapi/responses.py` & `moto-4.1.8.dev6/moto/resourcegroupstaggingapi/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53/exceptions.py` & `moto-4.1.8.dev6/moto/route53/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53/models.py` & `moto-4.1.8.dev6/moto/route53/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53/responses.py` & `moto-4.1.8.dev6/moto/route53/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53/urls.py` & `moto-4.1.8.dev6/moto/route53/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53resolver/exceptions.py` & `moto-4.1.8.dev6/moto/route53resolver/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53resolver/models.py` & `moto-4.1.8.dev6/moto/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53resolver/responses.py` & `moto-4.1.8.dev6/moto/route53resolver/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53resolver/utils.py` & `moto-4.1.8.dev6/moto/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/route53resolver/validations.py` & `moto-4.1.8.dev6/moto/route53resolver/validations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/cloud_formation.py` & `moto-4.1.8.dev6/moto/s3/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/config.py` & `moto-4.1.8.dev6/moto/s3/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/exceptions.py` & `moto-4.1.8.dev6/moto/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/models.py` & `moto-4.1.8.dev6/moto/s3/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/notifications.py` & `moto-4.1.8.dev6/moto/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/responses.py` & `moto-4.1.8.dev6/moto/s3/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/select_object_content.py` & `moto-4.1.8.dev6/moto/s3/select_object_content.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/urls.py` & `moto-4.1.8.dev6/moto/s3/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3/utils.py` & `moto-4.1.8.dev6/moto/s3/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3control/config.py` & `moto-4.1.8.dev6/moto/s3control/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3control/exceptions.py` & `moto-4.1.8.dev6/moto/s3control/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3control/models.py` & `moto-4.1.8.dev6/moto/s3control/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3control/responses.py` & `moto-4.1.8.dev6/moto/s3control/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/s3control/urls.py` & `moto-4.1.8.dev6/moto/s3control/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sagemaker/exceptions.py` & `moto-4.1.8.dev6/moto/sagemaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sagemaker/models.py` & `moto-4.1.8.dev6/moto/sagemaker/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sagemaker/responses.py` & `moto-4.1.8.dev6/moto/sagemaker/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sagemaker/utils.py` & `moto-4.1.8.dev6/moto/sagemaker/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sagemaker/validators.py` & `moto-4.1.8.dev6/moto/sagemaker/validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/scheduler/models.py` & `moto-4.1.8.dev6/moto/scheduler/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/scheduler/responses.py` & `moto-4.1.8.dev6/moto/scheduler/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/scheduler/urls.py` & `moto-4.1.8.dev6/moto/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sdb/exceptions.py` & `moto-4.1.8.dev6/moto/sdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sdb/models.py` & `moto-4.1.8.dev6/moto/sdb/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sdb/responses.py` & `moto-4.1.8.dev6/moto/sdb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/secretsmanager/exceptions.py` & `moto-4.1.8.dev6/moto/secretsmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/secretsmanager/list_secrets/filters.py` & `moto-4.1.8.dev6/moto/secretsmanager/list_secrets/filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/secretsmanager/models.py` & `moto-4.1.8.dev6/moto/secretsmanager/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/secretsmanager/responses.py` & `moto-4.1.8.dev6/moto/secretsmanager/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/secretsmanager/utils.py` & `moto-4.1.8.dev6/moto/secretsmanager/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/server.py` & `moto-4.1.8.dev6/moto/server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/servicediscovery/exceptions.py` & `moto-4.1.8.dev6/moto/servicediscovery/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/servicediscovery/models.py` & `moto-4.1.8.dev6/moto/servicediscovery/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/servicediscovery/responses.py` & `moto-4.1.8.dev6/moto/servicediscovery/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/servicequotas/models.py` & `moto-4.1.8.dev6/moto/servicequotas/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/servicequotas/resources/default_quotas/vpc.py` & `moto-4.1.8.dev6/moto/servicequotas/resources/default_quotas/vpc.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/servicequotas/responses.py` & `moto-4.1.8.dev6/moto/servicequotas/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ses/exceptions.py` & `moto-4.1.8.dev6/moto/ses/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ses/feedback.py` & `moto-4.1.8.dev6/moto/ses/feedback.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ses/models.py` & `moto-4.1.8.dev6/moto/ses/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ses/responses.py` & `moto-4.1.8.dev6/moto/ses/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ses/template.py` & `moto-4.1.8.dev6/moto/ses/template.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ses/utils.py` & `moto-4.1.8.dev6/moto/ses/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/settings.py` & `moto-4.1.8.dev6/moto/settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/signer/models.py` & `moto-4.1.8.dev6/moto/signer/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/signer/responses.py` & `moto-4.1.8.dev6/moto/signer/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sns/exceptions.py` & `moto-4.1.8.dev6/moto/sns/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sns/models.py` & `moto-4.1.8.dev6/moto/sns/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sns/responses.py` & `moto-4.1.8.dev6/moto/sns/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sqs/exceptions.py` & `moto-4.1.8.dev6/moto/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sqs/models.py` & `moto-4.1.8.dev6/moto/sqs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sqs/responses.py` & `moto-4.1.8.dev6/moto/sqs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sqs/utils.py` & `moto-4.1.8.dev6/moto/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/exceptions.py` & `moto-4.1.8.dev6/moto/ssm/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/models.py` & `moto-4.1.8.dev6/moto/ssm/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/af-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/me-central-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/me-south-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-1.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-2.json` & `moto-4.1.8.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/regions.json` & `moto-4.1.8.dev6/moto/ssm/resources/regions.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/resources/services.json` & `moto-4.1.8.dev6/moto/ssm/resources/services.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/responses.py` & `moto-4.1.8.dev6/moto/ssm/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssm/utils.py` & `moto-4.1.8.dev6/moto/ssm/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssoadmin/models.py` & `moto-4.1.8.dev6/moto/ssoadmin/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/ssoadmin/responses.py` & `moto-4.1.8.dev6/moto/ssoadmin/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/stepfunctions/exceptions.py` & `moto-4.1.8.dev6/moto/stepfunctions/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/stepfunctions/models.py` & `moto-4.1.8.dev6/moto/stepfunctions/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/stepfunctions/responses.py` & `moto-4.1.8.dev6/moto/stepfunctions/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/stepfunctions/utils.py` & `moto-4.1.8.dev6/moto/stepfunctions/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sts/models.py` & `moto-4.1.8.dev6/moto/sts/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sts/responses.py` & `moto-4.1.8.dev6/moto/sts/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/sts/utils.py` & `moto-4.1.8.dev6/moto/sts/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/support/models.py` & `moto-4.1.8.dev6/moto/support/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/support/resources/describe_trusted_advisor_checks.json` & `moto-4.1.8.dev6/moto/support/resources/describe_trusted_advisor_checks.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/support/responses.py` & `moto-4.1.8.dev6/moto/support/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/constants.py` & `moto-4.1.8.dev6/moto/swf/constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/exceptions.py` & `moto-4.1.8.dev6/moto/swf/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/models/__init__.py` & `moto-4.1.8.dev6/moto/swf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/models/activity_task.py` & `moto-4.1.8.dev6/moto/swf/models/activity_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/models/decision_task.py` & `moto-4.1.8.dev6/moto/swf/models/decision_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/models/domain.py` & `moto-4.1.8.dev6/moto/swf/models/domain.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/models/generic_type.py` & `moto-4.1.8.dev6/moto/swf/models/generic_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/models/history_event.py` & `moto-4.1.8.dev6/moto/swf/models/history_event.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/models/workflow_execution.py` & `moto-4.1.8.dev6/moto/swf/models/workflow_execution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/swf/responses.py` & `moto-4.1.8.dev6/moto/swf/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/textract/exceptions.py` & `moto-4.1.8.dev6/moto/textract/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/textract/models.py` & `moto-4.1.8.dev6/moto/textract/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/textract/responses.py` & `moto-4.1.8.dev6/moto/textract/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/timestreamwrite/models.py` & `moto-4.1.8.dev6/moto/timestreamwrite/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/timestreamwrite/responses.py` & `moto-4.1.8.dev6/moto/timestreamwrite/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/transcribe/models.py` & `moto-4.1.8.dev6/moto/transcribe/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/transcribe/responses.py` & `moto-4.1.8.dev6/moto/transcribe/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/utilities/aws_headers.py` & `moto-4.1.8.dev6/moto/utilities/aws_headers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/utilities/distutils_version.py` & `moto-4.1.8.dev6/moto/utilities/distutils_version.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/utilities/docker_utilities.py` & `moto-4.1.8.dev6/moto/utilities/docker_utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/utilities/paginator.py` & `moto-4.1.8.dev6/moto/utilities/paginator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/utilities/tagging_service.py` & `moto-4.1.8.dev6/moto/utilities/tagging_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/utilities/tokenizer.py` & `moto-4.1.8.dev6/moto/utilities/tokenizer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/utilities/utils.py` & `moto-4.1.8.dev6/moto/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/wafv2/exceptions.py` & `moto-4.1.8.dev6/moto/wafv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/wafv2/models.py` & `moto-4.1.8.dev6/moto/wafv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/wafv2/responses.py` & `moto-4.1.8.dev6/moto/wafv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/xray/exceptions.py` & `moto-4.1.8.dev6/moto/xray/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/xray/mock_client.py` & `moto-4.1.8.dev6/moto/xray/mock_client.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/xray/models.py` & `moto-4.1.8.dev6/moto/xray/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto/xray/responses.py` & `moto-4.1.8.dev6/moto/xray/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto.egg-info/PKG-INFO` & `moto-4.1.8.dev6/moto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moto
-Version: 4.1.8.dev5
+Version: 4.1.8.dev6
 Home-page: https://github.com/getmoto/moto
 Author: Steve Pulec
 Author-email: "spulec@gmail.com"
 License: Apache License 2.0
 Project-URL: Documentation, http://docs.getmoto.org/en/latest/
 Project-URL: Issue tracker, https://github.com/getmoto/moto/issues
 Project-URL: Changelog, https://github.com/getmoto/moto/blob/master/CHANGELOG.md
```

### Comparing `moto-4.1.8.dev5/moto.egg-info/SOURCES.txt` & `moto-4.1.8.dev6/moto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/moto.egg-info/requires.txt` & `moto-4.1.8.dev6/moto.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/setup.cfg` & `moto-4.1.8.dev6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = moto
-version = 4.1.8.dev5
+version = 4.1.8.dev6
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Steve Pulec
 author_email = "spulec@gmail.com"
 url = https://github.com/getmoto/moto
 license = Apache License 2.0
 test_suite = tests
@@ -228,15 +228,15 @@
 ignore-paths = moto/packages
 
 [pylint.'MESSAGES CONTROL']
 disable = W,C,R,E
 enable = anomalous-backslash-in-string, arguments-renamed, dangerous-default-value, deprecated-module, function-redefined, import-self, redefined-builtin, redefined-outer-name, reimported, pointless-statement, super-with-arguments, unused-argument, unused-import, unused-variable, useless-else-on-loop, wildcard-import
 
 [mypy]
-files = moto/a*,moto/b*,moto/c*,moto/d*,moto/e*,moto/f*,moto/g*,moto/i*,moto/k*,moto/l*,moto/m*,moto/n*,moto/o*,moto/p*,moto/q*,moto/ram,moto/rdsdata,moto/scheduler
+files = moto/a*,moto/b*,moto/c*,moto/d*,moto/e*,moto/f*,moto/g*,moto/i*,moto/k*,moto/l*,moto/m*,moto/n*,moto/o*,moto/p*,moto/q*,moto/ram,moto/rds,moto/rdsdata,moto/scheduler
 show_column_numbers = True
 show_error_codes = True
 disable_error_code = abstract
 disallow_any_unimported = False
 disallow_any_expr = False
 disallow_any_decorated = True
 disallow_any_explicit = False
```

### Comparing `moto-4.1.8.dev5/tests/__init__.py` & `moto-4.1.8.dev6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/helpers.py` & `moto-4.1.8.dev6/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/resources/README.md` & `moto-4.1.8.dev6/tests/test_acm/resources/README.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/resources/ca.key` & `moto-4.1.8.dev6/tests/test_acm/resources/ca.key`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/resources/ca.pem` & `moto-4.1.8.dev6/tests/test_acm/resources/ca.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com-bad.pem` & `moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com-bad.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com.csr` & `moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com.csr`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com.key` & `moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com.key`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/resources/star_moto_com.pem` & `moto-4.1.8.dev6/tests/test_acm/resources/star_moto_com.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acm/test_acm.py` & `moto-4.1.8.dev6/tests/test_acm/test_acm.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_acmpca/test_acmpca.py` & `moto-4.1.8.dev6/tests/test_acmpca/test_acmpca.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_amp/test_amp_logging_config.py` & `moto-4.1.8.dev6/tests/test_amp/test_amp_logging_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_amp/test_amp_rulegroupnamespaces.py` & `moto-4.1.8.dev6/tests/test_amp/test_amp_rulegroupnamespaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_amp/test_amp_workspaces.py` & `moto-4.1.8.dev6/tests/test_amp/test_amp_workspaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/resources/petstore-swagger-v3.yaml` & `moto-4.1.8.dev6/tests/test_apigateway/resources/petstore-swagger-v3.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/resources/test_api.json` & `moto-4.1.8.dev6/tests/test_apigateway/resources/test_api.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/resources/test_api.yaml` & `moto-4.1.8.dev6/tests/test_apigateway/resources/test_api.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/resources/test_api_invalid.json` & `moto-4.1.8.dev6/tests/test_apigateway/resources/test_api_invalid.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/resources/test_api_invalid_version.json` & `moto-4.1.8.dev6/tests/test_apigateway/resources/test_api_invalid_version.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/resources/test_deep_api.yaml` & `moto-4.1.8.dev6/tests/test_apigateway/resources/test_deep_api.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_cloudformation.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_deployments.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_deployments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_export.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_export.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_gatewayresponses.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_gatewayresponses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_importrestapi.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_importrestapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_integration.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_putrestapi.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_putrestapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_stage.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_stage.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_validators.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_apigateway_vpclink.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_apigateway_vpclink.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigateway/test_server.py` & `moto-4.1.8.dev6/tests/test_apigateway/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_domains.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrations.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_mappings.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_mappings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_models.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_reimport.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_reimport.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_routes.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_routes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_tags.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py` & `moto-4.1.8.dev6/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_applicationautoscaling/test_applicationautoscaling.py` & `moto-4.1.8.dev6/tests/test_applicationautoscaling/test_applicationautoscaling.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_applicationautoscaling/test_validation.py` & `moto-4.1.8.dev6/tests/test_applicationautoscaling/test_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_appsync/test_appsync.py` & `moto-4.1.8.dev6/tests/test_appsync/test_appsync.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_appsync/test_appsync_apikeys.py` & `moto-4.1.8.dev6/tests/test_appsync/test_appsync_apikeys.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_appsync/test_appsync_schema.py` & `moto-4.1.8.dev6/tests/test_appsync/test_appsync_schema.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_appsync/test_appsync_tags.py` & `moto-4.1.8.dev6/tests/test_appsync/test_appsync_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_athena/test_athena.py` & `moto-4.1.8.dev6/tests/test_athena/test_athena.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_athena/test_athena_server_api.py` & `moto-4.1.8.dev6/tests/test_athena/test_athena_server_api.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_cloudformation.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_groups.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_metrics.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_metrics.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_scheduledactions.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_scheduledactions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_autoscaling_tags.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_autoscaling_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_elb.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_elb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_elbv2.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_elbv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_launch_configurations.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_launch_configurations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/test_policies.py` & `moto-4.1.8.dev6/tests/test_autoscaling/test_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_autoscaling/utils.py` & `moto-4.1.8.dev6/tests/test_autoscaling/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_awslambda_cloudformation.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_awslambda_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_alias.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_alias.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_concurrency.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_concurrency.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_eventsourcemapping.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_eventsourcemapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_function_urls.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_function_urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_invoke.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_invoke.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_layers.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_layers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_policy.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_lambda_tags.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_lambda_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/test_policy.py` & `moto-4.1.8.dev6/tests/test_awslambda/test_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_awslambda/utilities.py` & `moto-4.1.8.dev6/tests/test_awslambda/utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/__init__.py` & `moto-4.1.8.dev6/tests/test_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_cloudformation.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_compute_envs.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_compute_envs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_job_queue.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_job_queue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_jobs.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_scheduling_policy.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_scheduling_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_tags_job_definition.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_tags_job_definition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_tags_job_queue.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_tags_job_queue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch/test_batch_task_definition.py` & `moto-4.1.8.dev6/tests/test_batch/test_batch_task_definition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch_simple/test_batch_cloudformation.py` & `moto-4.1.8.dev6/tests/test_batch_simple/test_batch_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch_simple/test_batch_compute_envs.py` & `moto-4.1.8.dev6/tests/test_batch_simple/test_batch_compute_envs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_batch_simple/test_batch_jobs.py` & `moto-4.1.8.dev6/tests/test_batch_simple/test_batch_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_budgets/test_budgets.py` & `moto-4.1.8.dev6/tests/test_budgets/test_budgets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_budgets/test_notifications.py` & `moto-4.1.8.dev6/tests/test_budgets/test_notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_budgets/test_server.py` & `moto-4.1.8.dev6/tests/test_budgets/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ce/test_ce.py` & `moto-4.1.8.dev6/tests/test_ce/test_ce.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ce/test_ce_tags.py` & `moto-4.1.8.dev6/tests/test_ce/test_ce_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/custom_lambda.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/custom_lambda.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/kms_key.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/kms_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/redshift.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/redshift.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/route53_health_check.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/route53_health_check.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/route53_roundrobin.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/route53_roundrobin.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/vpc_eni.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/vpc_eni.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py` & `moto-4.1.8.dev6/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_custom_resources.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_custom_resources.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_depends_on.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_depends_on.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_multi_accounts.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_multi_accounts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_nested_stacks.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_nested_stacks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_stack_integration.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_stack_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_cloudformation_stack_policies.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_cloudformation_stack_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_import_value.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_import_value.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_server.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_stack_parsing.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_stack_parsing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudformation/test_validate.py` & `moto-4.1.8.dev6/tests/test_cloudformation/test_validate.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudfront/cloudfront_test_scaffolding.py` & `moto-4.1.8.dev6/tests/test_cloudfront/cloudfront_test_scaffolding.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront.py` & `moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront_dist_tags.py` & `moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront_dist_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront_distributions.py` & `moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront_distributions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudfront/test_cloudfront_invalidation.py` & `moto-4.1.8.dev6/tests/test_cloudfront/test_cloudfront_invalidation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudtrail/test_cloudtrail.py` & `moto-4.1.8.dev6/tests/test_cloudtrail/test_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudtrail/test_cloudtrail_eventselectors.py` & `moto-4.1.8.dev6/tests/test_cloudtrail/test_cloudtrail_eventselectors.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudtrail/test_cloudtrail_tags.py` & `moto-4.1.8.dev6/tests/test_cloudtrail/test_cloudtrail_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudtrail/test_server.py` & `moto-4.1.8.dev6/tests/test_cloudtrail/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_alarms.py` & `moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_alarms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_boto3.py` & `moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_dashboards.py` & `moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_dashboards.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cloudwatch/test_cloudwatch_tags.py` & `moto-4.1.8.dev6/tests/test_cloudwatch/test_cloudwatch_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_codebuild/test_codebuild.py` & `moto-4.1.8.dev6/tests/test_codebuild/test_codebuild.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_codecommit/test_codecommit.py` & `moto-4.1.8.dev6/tests/test_codecommit/test_codecommit.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_codepipeline/test_codepipeline.py` & `moto-4.1.8.dev6/tests/test_codepipeline/test_codepipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cognitoidentity/test_cognitoidentity.py` & `moto-4.1.8.dev6/tests/test_cognitoidentity/test_cognitoidentity.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cognitoidentity/test_server.py` & `moto-4.1.8.dev6/tests/test_cognitoidentity/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cognitoidp/test_cognitoidp.py` & `moto-4.1.8.dev6/tests/test_cognitoidp/test_cognitoidp.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cognitoidp/test_cognitoidp_exceptions.py` & `moto-4.1.8.dev6/tests/test_cognitoidp/test_cognitoidp_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cognitoidp/test_cognitoidp_replay.py` & `moto-4.1.8.dev6/tests/test_cognitoidp/test_cognitoidp_replay.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_cognitoidp/test_server.py` & `moto-4.1.8.dev6/tests/test_cognitoidp/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_comprehend/test_comprehend.py` & `moto-4.1.8.dev6/tests/test_comprehend/test_comprehend.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_config/test_config.py` & `moto-4.1.8.dev6/tests/test_config/test_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_config/test_config_rules.py` & `moto-4.1.8.dev6/tests/test_config/test_config_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_config/test_config_rules_integration.py` & `moto-4.1.8.dev6/tests/test_config/test_config_rules_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_config/test_config_tags.py` & `moto-4.1.8.dev6/tests/test_config/test_config_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_account_id_resolution.py` & `moto-4.1.8.dev6/tests/test_core/test_account_id_resolution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_auth.py` & `moto-4.1.8.dev6/tests/test_core/test_auth.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_backenddict.py` & `moto-4.1.8.dev6/tests/test_core/test_backenddict.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_decorator_calls.py` & `moto-4.1.8.dev6/tests/test_core/test_decorator_calls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_docker.py` & `moto-4.1.8.dev6/tests/test_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_environ_patching.py` & `moto-4.1.8.dev6/tests/test_core/test_environ_patching.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_importorder.py` & `moto-4.1.8.dev6/tests/test_core/test_importorder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_instance_metadata.py` & `moto-4.1.8.dev6/tests/test_core/test_instance_metadata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_mock_all.py` & `moto-4.1.8.dev6/tests/test_core/test_mock_all.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_mock_regions.py` & `moto-4.1.8.dev6/tests/test_core/test_mock_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_moto_api.py` & `moto-4.1.8.dev6/tests/test_core/test_moto_api.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_nested.py` & `moto-4.1.8.dev6/tests/test_core/test_nested.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_request_mocking.py` & `moto-4.1.8.dev6/tests/test_core/test_request_mocking.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_responses.py` & `moto-4.1.8.dev6/tests/test_core/test_responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_responses_module.py` & `moto-4.1.8.dev6/tests/test_core/test_responses_module.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_server.py` & `moto-4.1.8.dev6/tests/test_core/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_settings.py` & `moto-4.1.8.dev6/tests/test_core/test_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_url_base_regex.py` & `moto-4.1.8.dev6/tests/test_core/test_url_base_regex.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_url_mapping.py` & `moto-4.1.8.dev6/tests/test_core/test_url_mapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_core/test_utils.py` & `moto-4.1.8.dev6/tests/test_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_databrew/test_databrew_datasets.py` & `moto-4.1.8.dev6/tests/test_databrew/test_databrew_datasets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_databrew/test_databrew_jobs.py` & `moto-4.1.8.dev6/tests/test_databrew/test_databrew_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_databrew/test_databrew_recipes.py` & `moto-4.1.8.dev6/tests/test_databrew/test_databrew_recipes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_databrew/test_databrew_rulesets.py` & `moto-4.1.8.dev6/tests/test_databrew/test_databrew_rulesets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_datapipeline/test_datapipeline.py` & `moto-4.1.8.dev6/tests/test_datapipeline/test_datapipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_datapipeline/test_datapipeline_cloudformation.py` & `moto-4.1.8.dev6/tests/test_datapipeline/test_datapipeline_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_datapipeline/test_server.py` & `moto-4.1.8.dev6/tests/test_datapipeline/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_datasync/test_datasync.py` & `moto-4.1.8.dev6/tests/test_datasync/test_datasync.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dax/test_dax.py` & `moto-4.1.8.dev6/tests/test_dax/test_dax.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dms/test_dms.py` & `moto-4.1.8.dev6/tests/test_dms/test_dms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ds/test_ds.py` & `moto-4.1.8.dev6/tests/test_ds/test_ds.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ds/test_ds_ad_connect.py` & `moto-4.1.8.dev6/tests/test_ds/test_ds_ad_connect.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ds/test_ds_microsoft_ad.py` & `moto-4.1.8.dev6/tests/test_ds/test_ds_microsoft_ad.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ds/test_ds_simple_ad_directory.py` & `moto-4.1.8.dev6/tests/test_ds/test_ds_simple_ad_directory.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ds/test_ds_tags.py` & `moto-4.1.8.dev6/tests/test_ds/test_ds_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/conftest.py` & `moto-4.1.8.dev6/tests/test_dynamodb/conftest.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py` & `moto-4.1.8.dev6/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/exceptions/test_key_length_exceptions.py` & `moto-4.1.8.dev6/tests/test_dynamodb/exceptions/test_key_length_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/models/test_key_condition_expression_parser.py` & `moto-4.1.8.dev6/tests/test_dynamodb/models/test_key_condition_expression_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_batch_get_item.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_batch_get_item.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_cloudformation.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_condition_expressions.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_condition_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_consumedcapacity.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_consumedcapacity.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_create_table.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_create_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_executor.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_executor.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_expressions.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_table_with_range_key.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_table_with_range_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_table_without_range_key.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_table_without_range_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_update_expressions.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_update_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_update_table.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_update_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_dynamodb_validation.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_dynamodb_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb/test_server.py` & `moto-4.1.8.dev6/tests/test_dynamodb/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb_v20111205/test_server.py` & `moto-4.1.8.dev6/tests/test_dynamodb_v20111205/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodb_v20111205/test_servermode.py` & `moto-4.1.8.dev6/tests/test_dynamodb_v20111205/test_servermode.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_dynamodbstreams/test_dynamodbstreams.py` & `moto-4.1.8.dev6/tests/test_dynamodbstreams/test_dynamodbstreams.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ebs/test_ebs.py` & `moto-4.1.8.dev6/tests/test_ebs/test_ebs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_account_attributes.py` & `moto-4.1.8.dev6/tests/test_ec2/test_account_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_amis.py` & `moto-4.1.8.dev6/tests/test_ec2/test_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_availability_zones_and_regions.py` & `moto-4.1.8.dev6/tests/test_ec2/test_availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_carrier_gateways.py` & `moto-4.1.8.dev6/tests/test_ec2/test_carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_customer_gateways.py` & `moto-4.1.8.dev6/tests/test_ec2/test_customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_dhcp_options.py` & `moto-4.1.8.dev6/tests/test_ec2/test_dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_ec2_cloudformation.py` & `moto-4.1.8.dev6/tests/test_ec2/test_ec2_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_ec2_integration.py` & `moto-4.1.8.dev6/tests/test_ec2/test_ec2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_egress_only_igw.py` & `moto-4.1.8.dev6/tests/test_ec2/test_egress_only_igw.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_elastic_block_store.py` & `moto-4.1.8.dev6/tests/test_ec2/test_elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_elastic_ip_addresses.py` & `moto-4.1.8.dev6/tests/test_ec2/test_elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_elastic_network_interfaces.py` & `moto-4.1.8.dev6/tests/test_ec2/test_elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_fleets.py` & `moto-4.1.8.dev6/tests/test_ec2/test_fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_flow_logs.py` & `moto-4.1.8.dev6/tests/test_ec2/test_flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_flow_logs_cloudformation.py` & `moto-4.1.8.dev6/tests/test_ec2/test_flow_logs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_general.py` & `moto-4.1.8.dev6/tests/test_ec2/test_general.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_hosts.py` & `moto-4.1.8.dev6/tests/test_ec2/test_hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_iam_integration.py` & `moto-4.1.8.dev6/tests/test_ec2/test_iam_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_instance_type_offerings.py` & `moto-4.1.8.dev6/tests/test_ec2/test_instance_type_offerings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_instance_types.py` & `moto-4.1.8.dev6/tests/test_ec2/test_instance_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_instances.py` & `moto-4.1.8.dev6/tests/test_ec2/test_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_internet_gateways.py` & `moto-4.1.8.dev6/tests/test_ec2/test_internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_key_pairs.py` & `moto-4.1.8.dev6/tests/test_ec2/test_key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_launch_templates.py` & `moto-4.1.8.dev6/tests/test_ec2/test_launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_nat_gateway.py` & `moto-4.1.8.dev6/tests/test_ec2/test_nat_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_network_acls.py` & `moto-4.1.8.dev6/tests/test_ec2/test_network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_prefix_lists.py` & `moto-4.1.8.dev6/tests/test_ec2/test_prefix_lists.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_regions.py` & `moto-4.1.8.dev6/tests/test_ec2/test_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_route_tables.py` & `moto-4.1.8.dev6/tests/test_ec2/test_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_security_groups.py` & `moto-4.1.8.dev6/tests/test_ec2/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_security_groups_cloudformation.py` & `moto-4.1.8.dev6/tests/test_ec2/test_security_groups_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_server.py` & `moto-4.1.8.dev6/tests/test_ec2/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_settings.py` & `moto-4.1.8.dev6/tests/test_ec2/test_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_spot_fleet.py` & `moto-4.1.8.dev6/tests/test_ec2/test_spot_fleet.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_spot_instances.py` & `moto-4.1.8.dev6/tests/test_ec2/test_spot_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_subnets.py` & `moto-4.1.8.dev6/tests/test_ec2/test_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_tags.py` & `moto-4.1.8.dev6/tests/test_ec2/test_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_transit_gateway.py` & `moto-4.1.8.dev6/tests/test_ec2/test_transit_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_transit_gateway_cloudformation.py` & `moto-4.1.8.dev6/tests/test_ec2/test_transit_gateway_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_transit_gateway_peering_attachments.py` & `moto-4.1.8.dev6/tests/test_ec2/test_transit_gateway_peering_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_utils.py` & `moto-4.1.8.dev6/tests/test_ec2/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_virtual_private_gateways.py` & `moto-4.1.8.dev6/tests/test_ec2/test_virtual_private_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_vpc_endpoint_services_integration.py` & `moto-4.1.8.dev6/tests/test_ec2/test_vpc_endpoint_services_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_vpc_peering.py` & `moto-4.1.8.dev6/tests/test_ec2/test_vpc_peering.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_vpc_service_configuration.py` & `moto-4.1.8.dev6/tests/test_ec2/test_vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_vpcs.py` & `moto-4.1.8.dev6/tests/test_ec2/test_vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_vpn_connections.py` & `moto-4.1.8.dev6/tests/test_ec2/test_vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2/test_windows.py` & `moto-4.1.8.dev6/tests/test_ec2/test_windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py` & `moto-4.1.8.dev6/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecr/test_ecr_boto3.py` & `moto-4.1.8.dev6/tests/test_ecr/test_ecr_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecr/test_ecr_cloudformation.py` & `moto-4.1.8.dev6/tests/test_ecr/test_ecr_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecr/test_ecr_helpers.py` & `moto-4.1.8.dev6/tests/test_ecr/test_ecr_helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecr/test_ecr_policy_validation.py` & `moto-4.1.8.dev6/tests/test_ecr/test_ecr_policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecs/test_ecs_account_settings.py` & `moto-4.1.8.dev6/tests/test_ecs/test_ecs_account_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecs/test_ecs_boto3.py` & `moto-4.1.8.dev6/tests/test_ecs/test_ecs_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecs/test_ecs_capacity_provider.py` & `moto-4.1.8.dev6/tests/test_ecs/test_ecs_capacity_provider.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecs/test_ecs_cloudformation.py` & `moto-4.1.8.dev6/tests/test_ecs/test_ecs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecs/test_ecs_efs.py` & `moto-4.1.8.dev6/tests/test_ecs/test_ecs_efs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecs/test_ecs_task_def_tags.py` & `moto-4.1.8.dev6/tests/test_ecs/test_ecs_task_def_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ecs/test_ecs_tasksets.py` & `moto-4.1.8.dev6/tests/test_ecs/test_ecs_tasksets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_access_point_tagging.py` & `moto-4.1.8.dev6/tests/test_efs/test_access_point_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_access_points.py` & `moto-4.1.8.dev6/tests/test_efs/test_access_points.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_file_system.py` & `moto-4.1.8.dev6/tests/test_efs/test_file_system.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_filesystem_tagging.py` & `moto-4.1.8.dev6/tests/test_efs/test_filesystem_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_lifecycle_config.py` & `moto-4.1.8.dev6/tests/test_efs/test_lifecycle_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_mount_target.py` & `moto-4.1.8.dev6/tests/test_efs/test_mount_target.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_mount_target_security_groups.py` & `moto-4.1.8.dev6/tests/test_efs/test_mount_target_security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_efs/test_server.py` & `moto-4.1.8.dev6/tests/test_efs/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_eks/test_eks.py` & `moto-4.1.8.dev6/tests/test_eks/test_eks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_eks/test_eks_constants.py` & `moto-4.1.8.dev6/tests/test_eks/test_eks_constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_eks/test_eks_ec2.py` & `moto-4.1.8.dev6/tests/test_eks/test_eks_ec2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_eks/test_eks_utils.py` & `moto-4.1.8.dev6/tests/test_eks/test_eks_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_eks/test_server.py` & `moto-4.1.8.dev6/tests/test_eks/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elasticache/test_elasticache.py` & `moto-4.1.8.dev6/tests/test_elasticache/test_elasticache.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elasticbeanstalk/test_eb.py` & `moto-4.1.8.dev6/tests/test_elasticbeanstalk/test_eb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elastictranscoder/test_elastictranscoder.py` & `moto-4.1.8.dev6/tests/test_elastictranscoder/test_elastictranscoder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elb/test_elb.py` & `moto-4.1.8.dev6/tests/test_elb/test_elb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elb/test_elb_availabilityzones.py` & `moto-4.1.8.dev6/tests/test_elb/test_elb_availabilityzones.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elb/test_elb_cloudformation.py` & `moto-4.1.8.dev6/tests/test_elb/test_elb_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elb/test_elb_policies.py` & `moto-4.1.8.dev6/tests/test_elb/test_elb_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elb/test_elb_subnets.py` & `moto-4.1.8.dev6/tests/test_elb/test_elb_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_cloudformation.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_integration.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_listener_rule_tags.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_listener_rule_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_listener_rules.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_listener_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_listener_tags.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_listener_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_set_subnets.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_set_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_elbv2/test_elbv2_target_groups.py` & `moto-4.1.8.dev6/tests/test_elbv2/test_elbv2_target_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_emr/test_emr_boto3.py` & `moto-4.1.8.dev6/tests/test_emr/test_emr_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_emr/test_emr_integration.py` & `moto-4.1.8.dev6/tests/test_emr/test_emr_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_emr/test_utils.py` & `moto-4.1.8.dev6/tests/test_emr/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_emrcontainers/test_emrcontainers.py` & `moto-4.1.8.dev6/tests/test_emrcontainers/test_emrcontainers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_emrserverless/test_emrserverless.py` & `moto-4.1.8.dev6/tests/test_emrserverless/test_emrserverless.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_es/test_es.py` & `moto-4.1.8.dev6/tests/test_es/test_es.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_events/test_event_pattern.py` & `moto-4.1.8.dev6/tests/test_events/test_event_pattern.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_events/test_events.py` & `moto-4.1.8.dev6/tests/test_events/test_events.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_events/test_events_cloudformation.py` & `moto-4.1.8.dev6/tests/test_events/test_events_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_events/test_events_integration.py` & `moto-4.1.8.dev6/tests/test_events/test_events_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_events/test_events_lambdatriggers_integration.py` & `moto-4.1.8.dev6/tests/test_events/test_events_lambdatriggers_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_firehose/test_firehose.py` & `moto-4.1.8.dev6/tests/test_firehose/test_firehose.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_firehose/test_firehose_destination_types.py` & `moto-4.1.8.dev6/tests/test_firehose/test_firehose_destination_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_firehose/test_firehose_encryption.py` & `moto-4.1.8.dev6/tests/test_firehose/test_firehose_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_firehose/test_firehose_put.py` & `moto-4.1.8.dev6/tests/test_firehose/test_firehose_put.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_firehose/test_firehose_tags.py` & `moto-4.1.8.dev6/tests/test_firehose/test_firehose_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_firehose/test_http_destinations.py` & `moto-4.1.8.dev6/tests/test_firehose/test_http_destinations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_forecast/test_forecast.py` & `moto-4.1.8.dev6/tests/test_forecast/test_forecast.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glacier/test_glacier_archives.py` & `moto-4.1.8.dev6/tests/test_glacier/test_glacier_archives.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glacier/test_glacier_jobs.py` & `moto-4.1.8.dev6/tests/test_glacier/test_glacier_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glacier/test_glacier_vaults.py` & `moto-4.1.8.dev6/tests/test_glacier/test_glacier_vaults.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/fixtures/datacatalog.py` & `moto-4.1.8.dev6/tests/test_glue/fixtures/datacatalog.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/fixtures/schema_registry.py` & `moto-4.1.8.dev6/tests/test_glue/fixtures/schema_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/helpers.py` & `moto-4.1.8.dev6/tests/test_glue/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/test_datacatalog.py` & `moto-4.1.8.dev6/tests/test_glue/test_datacatalog.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/test_glue.py` & `moto-4.1.8.dev6/tests/test_glue/test_glue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/test_glue_job_runs.py` & `moto-4.1.8.dev6/tests/test_glue/test_glue_job_runs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/test_partition_filter.py` & `moto-4.1.8.dev6/tests/test_glue/test_partition_filter.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_glue/test_schema_registry.py` & `moto-4.1.8.dev6/tests/test_glue/test_schema_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_core.py` & `moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_core.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_deployment.py` & `moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_deployment.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_device.py` & `moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_device.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_functions.py` & `moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_functions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_groups.py` & `moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_resource.py` & `moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_resource.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_greengrass/test_greengrass_subscriptions.py` & `moto-4.1.8.dev6/tests/test_greengrass/test_greengrass_subscriptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_guardduty/test_guardduty.py` & `moto-4.1.8.dev6/tests/test_guardduty/test_guardduty.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_guardduty/test_guardduty_filters.py` & `moto-4.1.8.dev6/tests/test_guardduty/test_guardduty_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_guardduty/test_guardduty_organization.py` & `moto-4.1.8.dev6/tests/test_guardduty/test_guardduty_organization.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_access_integration.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_access_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_account_aliases.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_account_aliases.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_cloudformation.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_groups.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_oidc.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_oidc.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_password_last_used.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_password_last_used.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_policies.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_iam_server_certificates.py` & `moto-4.1.8.dev6/tests/test_iam/test_iam_server_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iam/test_server.py` & `moto-4.1.8.dev6/tests/test_iam/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_identitystore/test_identitystore.py` & `moto-4.1.8.dev6/tests/test_identitystore/test_identitystore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_ca_certificates.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_ca_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_certificates.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_deprecate_thing_type.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_deprecate_thing_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_domain_configuration.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_domain_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_job_executions.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_job_executions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_jobs.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_policies.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_search.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_search.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_thing_groups.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_thing_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_thing_types.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_thing_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_things.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_things.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_iot_topic_rules.py` & `moto-4.1.8.dev6/tests/test_iot/test_iot_topic_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iot/test_server.py` & `moto-4.1.8.dev6/tests/test_iot/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iotdata/test_iotdata.py` & `moto-4.1.8.dev6/tests/test_iotdata/test_iotdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_iotdata/test_server.py` & `moto-4.1.8.dev6/tests/test_iotdata/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesis/test_kinesis.py` & `moto-4.1.8.dev6/tests/test_kinesis/test_kinesis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_boto3.py` & `moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_cloudformation.py` & `moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_encryption.py` & `moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_monitoring.py` & `moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_monitoring.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_stream_consumers.py` & `moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_stream_consumers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesis/test_kinesis_stream_limits.py` & `moto-4.1.8.dev6/tests/test_kinesis/test_kinesis_stream_limits.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesisvideo/test_kinesisvideo.py` & `moto-4.1.8.dev6/tests/test_kinesisvideo/test_kinesisvideo.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py` & `moto-4.1.8.dev6/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kms/test_kms_boto3.py` & `moto-4.1.8.dev6/tests/test_kms/test_kms_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kms/test_kms_encrypt.py` & `moto-4.1.8.dev6/tests/test_kms/test_kms_encrypt.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kms/test_kms_grants.py` & `moto-4.1.8.dev6/tests/test_kms/test_kms_grants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kms/test_kms_policy_enforcement.py` & `moto-4.1.8.dev6/tests/test_kms/test_kms_policy_enforcement.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kms/test_model.py` & `moto-4.1.8.dev6/tests/test_kms/test_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_kms/test_utils.py` & `moto-4.1.8.dev6/tests/test_kms/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_lakeformation/test_lakeformation.py` & `moto-4.1.8.dev6/tests/test_lakeformation/test_lakeformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_logs/test_integration.py` & `moto-4.1.8.dev6/tests/test_logs/test_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_logs/test_logs.py` & `moto-4.1.8.dev6/tests/test_logs/test_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_logs/test_logs_filter.py` & `moto-4.1.8.dev6/tests/test_logs/test_logs_filter.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_logs/test_models.py` & `moto-4.1.8.dev6/tests/test_logs/test_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_managedblockchain/helpers.py` & `moto-4.1.8.dev6/tests/test_managedblockchain/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_invitations.py` & `moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_invitations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_members.py` & `moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_members.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_networks.py` & `moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_networks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_nodes.py` & `moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_nodes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_proposals.py` & `moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_proposals.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py` & `moto-4.1.8.dev6/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mediaconnect/test_mediaconnect.py` & `moto-4.1.8.dev6/tests/test_mediaconnect/test_mediaconnect.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_medialive/test_medialive.py` & `moto-4.1.8.dev6/tests/test_medialive/test_medialive.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_medialive/test_server.py` & `moto-4.1.8.dev6/tests/test_medialive/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mediapackage/test_mediapackage.py` & `moto-4.1.8.dev6/tests/test_mediapackage/test_mediapackage.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mediapackage/test_server.py` & `moto-4.1.8.dev6/tests/test_mediapackage/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mediastore/test_mediastore.py` & `moto-4.1.8.dev6/tests/test_mediastore/test_mediastore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mediastoredata/test_mediastoredata.py` & `moto-4.1.8.dev6/tests/test_mediastoredata/test_mediastoredata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_meteringmarketplace/test_meteringmarketplace.py` & `moto-4.1.8.dev6/tests/test_meteringmarketplace/test_meteringmarketplace.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_moto_api/mock_random/test_mock_random.py` & `moto-4.1.8.dev6/tests/test_moto_api/mock_random/test_mock_random.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_moto_api/recorder/test_recorder.py` & `moto-4.1.8.dev6/tests/test_moto_api/recorder/test_recorder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py` & `moto-4.1.8.dev6/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_moto_api/state_manager/servermode/test_state_manager.py` & `moto-4.1.8.dev6/tests/test_moto_api/state_manager/servermode/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_moto_api/state_manager/test_batch_integration.py` & `moto-4.1.8.dev6/tests/test_moto_api/state_manager/test_batch_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_moto_api/state_manager/test_managed_state_model.py` & `moto-4.1.8.dev6/tests/test_moto_api/state_manager/test_managed_state_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_moto_api/state_manager/test_state_manager.py` & `moto-4.1.8.dev6/tests/test_moto_api/state_manager/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mq/test_mq.py` & `moto-4.1.8.dev6/tests/test_mq/test_mq.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mq/test_mq_configuration.py` & `moto-4.1.8.dev6/tests/test_mq/test_mq_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mq/test_mq_tags.py` & `moto-4.1.8.dev6/tests/test_mq/test_mq_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_mq/test_mq_users.py` & `moto-4.1.8.dev6/tests/test_mq/test_mq_users.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_neptune/test_cluster_options.py` & `moto-4.1.8.dev6/tests/test_neptune/test_cluster_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_neptune/test_cluster_tags.py` & `moto-4.1.8.dev6/tests/test_neptune/test_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_neptune/test_clusters.py` & `moto-4.1.8.dev6/tests/test_neptune/test_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_neptune/test_global_clusters.py` & `moto-4.1.8.dev6/tests/test_neptune/test_global_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_opensearch/test_domain_tags.py` & `moto-4.1.8.dev6/tests/test_opensearch/test_domain_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_opensearch/test_opensearch.py` & `moto-4.1.8.dev6/tests/test_opensearch/test_opensearch.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_opsworks/test_apps.py` & `moto-4.1.8.dev6/tests/test_opsworks/test_apps.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_opsworks/test_instances.py` & `moto-4.1.8.dev6/tests/test_opsworks/test_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_opsworks/test_layers.py` & `moto-4.1.8.dev6/tests/test_opsworks/test_layers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_opsworks/test_stack.py` & `moto-4.1.8.dev6/tests/test_opsworks/test_stack.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_organizations/organizations_test_utils.py` & `moto-4.1.8.dev6/tests/test_organizations/organizations_test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_organizations/test_organizations_boto3.py` & `moto-4.1.8.dev6/tests/test_organizations/test_organizations_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_personalize/test_personalize_schema.py` & `moto-4.1.8.dev6/tests/test_personalize/test_personalize_schema.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_pinpoint/test_pinpoint.py` & `moto-4.1.8.dev6/tests/test_pinpoint/test_pinpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_pinpoint/test_pinpoint_application_tags.py` & `moto-4.1.8.dev6/tests/test_pinpoint/test_pinpoint_application_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_pinpoint/test_pinpoint_event_stream.py` & `moto-4.1.8.dev6/tests/test_pinpoint/test_pinpoint_event_stream.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_polly/test_polly.py` & `moto-4.1.8.dev6/tests/test_polly/test_polly.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_quicksight/test_quicksight_datasets.py` & `moto-4.1.8.dev6/tests/test_quicksight/test_quicksight_datasets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_quicksight/test_quicksight_groups.py` & `moto-4.1.8.dev6/tests/test_quicksight/test_quicksight_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_quicksight/test_quicksight_users.py` & `moto-4.1.8.dev6/tests/test_quicksight/test_quicksight_users.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ram/test_ram.py` & `moto-4.1.8.dev6/tests/test_ram/test_ram.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_db_cluster_param_group.py` & `moto-4.1.8.dev6/tests/test_rds/test_db_cluster_param_group.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_filters.py` & `moto-4.1.8.dev6/tests/test_rds/test_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_global_clusters.py` & `moto-4.1.8.dev6/tests/test_rds/test_global_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_rds.py` & `moto-4.1.8.dev6/tests/test_rds/test_rds.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_rds_cloudformation.py` & `moto-4.1.8.dev6/tests/test_rds/test_rds_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_rds_clusters.py` & `moto-4.1.8.dev6/tests/test_rds/test_rds_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_rds_clusters_with_instances.py` & `moto-4.1.8.dev6/tests/test_rds/test_rds_clusters_with_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_rds_event_subscriptions.py` & `moto-4.1.8.dev6/tests/test_rds/test_rds_event_subscriptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_rds_export_tasks.py` & `moto-4.1.8.dev6/tests/test_rds/test_rds_export_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_server.py` & `moto-4.1.8.dev6/tests/test_rds/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rds/test_utils.py` & `moto-4.1.8.dev6/tests/test_rds/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rdsdata/test_rdsdata.py` & `moto-4.1.8.dev6/tests/test_rdsdata/test_rdsdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_redshift/test_redshift.py` & `moto-4.1.8.dev6/tests/test_redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_redshift/test_redshift_cloudformation.py` & `moto-4.1.8.dev6/tests/test_redshift/test_redshift_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_redshift/test_server.py` & `moto-4.1.8.dev6/tests/test_redshift/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_redshiftdata/test_redshiftdata.py` & `moto-4.1.8.dev6/tests/test_redshiftdata/test_redshiftdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_redshiftdata/test_server.py` & `moto-4.1.8.dev6/tests/test_redshiftdata/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_rekognition/test_rekognition.py` & `moto-4.1.8.dev6/tests/test_rekognition/test_rekognition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_resourcegroups/test_resourcegroups.py` & `moto-4.1.8.dev6/tests/test_resourcegroups/test_resourcegroups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py` & `moto-4.1.8.dev6/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_resourcegroupstaggingapi/test_server.py` & `moto-4.1.8.dev6/tests/test_resourcegroupstaggingapi/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_change_set_model.py` & `moto-4.1.8.dev6/tests/test_route53/test_change_set_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_route53.py` & `moto-4.1.8.dev6/tests/test_route53/test_route53.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_route53_cloudformation.py` & `moto-4.1.8.dev6/tests/test_route53/test_route53_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_route53_delegationsets.py` & `moto-4.1.8.dev6/tests/test_route53/test_route53_delegationsets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_route53_healthchecks.py` & `moto-4.1.8.dev6/tests/test_route53/test_route53_healthchecks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_route53_query_logging_config.py` & `moto-4.1.8.dev6/tests/test_route53/test_route53_query_logging_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_route53_vpcs.py` & `moto-4.1.8.dev6/tests/test_route53/test_route53_vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53/test_server.py` & `moto-4.1.8.dev6/tests/test_route53/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_endpoint.py` & `moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_rule.py` & `moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_rule.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_rule_associations.py` & `moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_rule_associations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_route53resolver/test_route53resolver_tags.py` & `moto-4.1.8.dev6/tests/test_route53resolver/test_route53resolver_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_multiple_accounts_server.py` & `moto-4.1.8.dev6/tests/test_s3/test_multiple_accounts_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_acl.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_acl.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_auth.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_auth.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_bucket_policy.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_classdecorator.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_classdecorator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_cloudformation.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_config.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_copyobject.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_copyobject.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_custom_endpoint.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_custom_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_encryption.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_file_handles.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_file_handles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_lambda_integration.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_lambda_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_lifecycle.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_lifecycle.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_lock.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_lock.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_logging.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_logging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_metadata.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_metadata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_multipart.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_multipart.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_object_attributes.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_object_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_ownership.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_ownership.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_replication.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_replication.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_select.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_select.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_storageclass.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_storageclass.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_tagging.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_s3_utils.py` & `moto-4.1.8.dev6/tests/test_s3/test_s3_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3/test_server.py` & `moto-4.1.8.dev6/tests/test_s3/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3bucket_path/test_server.py` & `moto-4.1.8.dev6/tests/test_s3bucket_path/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3control/test_s3control.py` & `moto-4.1.8.dev6/tests/test_s3control/test_s3control.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3control/test_s3control_access_points.py` & `moto-4.1.8.dev6/tests/test_s3control/test_s3control_access_points.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3control/test_s3control_accesspoint_policy.py` & `moto-4.1.8.dev6/tests/test_s3control/test_s3control_accesspoint_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3control/test_s3control_config_integration.py` & `moto-4.1.8.dev6/tests/test_s3control/test_s3control_config_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_s3control/test_s3control_s3.py` & `moto-4.1.8.dev6/tests/test_s3control/test_s3control_s3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/cloudformation_test_configs.py` & `moto-4.1.8.dev6/tests/test_sagemaker/cloudformation_test_configs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_cloudformation.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_endpoint.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_experiment.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_experiment.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_models.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_notebooks.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_notebooks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_pipeline.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_pipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_processing.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_processing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_search.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_search.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_training.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_training.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_trial.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_trial.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sagemaker/test_sagemaker_trial_component.py` & `moto-4.1.8.dev6/tests/test_sagemaker/test_sagemaker_trial_component.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_scheduler/test_schedule_groups.py` & `moto-4.1.8.dev6/tests/test_scheduler/test_schedule_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_scheduler/test_scheduler.py` & `moto-4.1.8.dev6/tests/test_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_scheduler/test_scheduler_tags.py` & `moto-4.1.8.dev6/tests/test_scheduler/test_scheduler_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sdb/test_sdb_attributes.py` & `moto-4.1.8.dev6/tests/test_sdb/test_sdb_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sdb/test_sdb_domains.py` & `moto-4.1.8.dev6/tests/test_sdb/test_sdb_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_secretsmanager/test_list_secrets.py` & `moto-4.1.8.dev6/tests/test_secretsmanager/test_list_secrets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_secretsmanager/test_policy.py` & `moto-4.1.8.dev6/tests/test_secretsmanager/test_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_secretsmanager/test_secretsmanager.py` & `moto-4.1.8.dev6/tests/test_secretsmanager/test_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_secretsmanager/test_server.py` & `moto-4.1.8.dev6/tests/test_secretsmanager/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py` & `moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_operations.py` & `moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_operations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_service.py` & `moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_servicediscovery/test_servicediscovery_tags.py` & `moto-4.1.8.dev6/tests/test_servicediscovery/test_servicediscovery_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_servicequotas/test_servicequotas.py` & `moto-4.1.8.dev6/tests/test_servicequotas/test_servicequotas.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ses/test_server.py` & `moto-4.1.8.dev6/tests/test_ses/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ses/test_ses_boto3.py` & `moto-4.1.8.dev6/tests/test_ses/test_ses_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ses/test_ses_sns_boto3.py` & `moto-4.1.8.dev6/tests/test_ses/test_ses_sns_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ses/test_templating.py` & `moto-4.1.8.dev6/tests/test_ses/test_templating.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_signer/test_signing_platforms.py` & `moto-4.1.8.dev6/tests/test_signer/test_signing_platforms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_signer/test_signing_profiles.py` & `moto-4.1.8.dev6/tests/test_signer/test_signing_profiles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sns/test_application_boto3.py` & `moto-4.1.8.dev6/tests/test_sns/test_application_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sns/test_publish_batch.py` & `moto-4.1.8.dev6/tests/test_sns/test_publish_batch.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sns/test_publishing_boto3.py` & `moto-4.1.8.dev6/tests/test_sns/test_publishing_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sns/test_server.py` & `moto-4.1.8.dev6/tests/test_sns/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sns/test_sns_cloudformation.py` & `moto-4.1.8.dev6/tests/test_sns/test_sns_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sns/test_subscriptions_boto3.py` & `moto-4.1.8.dev6/tests/test_sns/test_subscriptions_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sns/test_topics_boto3.py` & `moto-4.1.8.dev6/tests/test_sns/test_topics_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_special_cases/test_custom_amis.py` & `moto-4.1.8.dev6/tests/test_special_cases/test_custom_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sqs/test_server.py` & `moto-4.1.8.dev6/tests/test_sqs/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sqs/test_sqs.py` & `moto-4.1.8.dev6/tests/test_sqs/test_sqs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sqs/test_sqs_cloudformation.py` & `moto-4.1.8.dev6/tests/test_sqs/test_sqs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sqs/test_sqs_integration.py` & `moto-4.1.8.dev6/tests/test_sqs/test_sqs_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sqs/test_sqs_multiaccount.py` & `moto-4.1.8.dev6/tests/test_sqs/test_sqs_multiaccount.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_boto3.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_cloudformation.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_default_amis.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_default_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_defaults.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_defaults.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_doc_permissions.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_doc_permissions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_docs.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_docs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_ecs_images.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_ecs_images.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_maintenance_windows.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_maintenance_windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_parameterstore.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_parameterstore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_secretsmanager.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_ssm_utils.py` & `moto-4.1.8.dev6/tests/test_ssm/test_ssm_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssm/test_templates/good.yaml` & `moto-4.1.8.dev6/tests/test_ssm/test_templates/good.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssoadmin/test_server.py` & `moto-4.1.8.dev6/tests/test_ssoadmin/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_ssoadmin/test_ssoadmin.py` & `moto-4.1.8.dev6/tests/test_ssoadmin/test_ssoadmin.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_stepfunctions/test_stepfunctions.py` & `moto-4.1.8.dev6/tests/test_stepfunctions/test_stepfunctions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_stepfunctions/test_stepfunctions_cloudformation.py` & `moto-4.1.8.dev6/tests/test_stepfunctions/test_stepfunctions_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sts/test_server.py` & `moto-4.1.8.dev6/tests/test_sts/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sts/test_sts.py` & `moto-4.1.8.dev6/tests/test_sts/test_sts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_sts/test_sts_integration.py` & `moto-4.1.8.dev6/tests/test_sts/test_sts_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_support/test_server.py` & `moto-4.1.8.dev6/tests/test_support/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_support/test_support.py` & `moto-4.1.8.dev6/tests/test_support/test_support.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_activity_task.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_activity_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_decision_task.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_decision_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_domain.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_domain.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_generic_type.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_generic_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_history_event.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_history_event.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_timeout.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_timeout.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_timer.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_timer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/models/test_workflow_execution.py` & `moto-4.1.8.dev6/tests/test_swf/models/test_workflow_execution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/responses/test_activity_tasks.py` & `moto-4.1.8.dev6/tests/test_swf/responses/test_activity_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/responses/test_activity_types.py` & `moto-4.1.8.dev6/tests/test_swf/responses/test_activity_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/responses/test_decision_tasks.py` & `moto-4.1.8.dev6/tests/test_swf/responses/test_decision_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/responses/test_domains.py` & `moto-4.1.8.dev6/tests/test_swf/responses/test_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/responses/test_timeouts.py` & `moto-4.1.8.dev6/tests/test_swf/responses/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/responses/test_workflow_executions.py` & `moto-4.1.8.dev6/tests/test_swf/responses/test_workflow_executions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/responses/test_workflow_types.py` & `moto-4.1.8.dev6/tests/test_swf/responses/test_workflow_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/test_exceptions.py` & `moto-4.1.8.dev6/tests/test_swf/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_swf/utils.py` & `moto-4.1.8.dev6/tests/test_swf/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_textract/test_server.py` & `moto-4.1.8.dev6/tests/test_textract/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_textract/test_textract.py` & `moto-4.1.8.dev6/tests/test_textract/test_textract.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_timestreamwrite/test_server.py` & `moto-4.1.8.dev6/tests/test_timestreamwrite/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_timestreamwrite/test_timestreamwrite_database.py` & `moto-4.1.8.dev6/tests/test_timestreamwrite/test_timestreamwrite_database.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_timestreamwrite/test_timestreamwrite_table.py` & `moto-4.1.8.dev6/tests/test_timestreamwrite/test_timestreamwrite_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_timestreamwrite/test_timestreamwrite_tagging.py` & `moto-4.1.8.dev6/tests/test_timestreamwrite/test_timestreamwrite_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_transcribe/test_transcribe_boto3.py` & `moto-4.1.8.dev6/tests/test_transcribe/test_transcribe_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_utilities/test_docker_utilities.py` & `moto-4.1.8.dev6/tests/test_utilities/test_docker_utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_utilities/test_paginator.py` & `moto-4.1.8.dev6/tests/test_utilities/test_paginator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_utilities/test_tagging_service.py` & `moto-4.1.8.dev6/tests/test_utilities/test_tagging_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_utilities/test_threaded_server.py` & `moto-4.1.8.dev6/tests/test_utilities/test_threaded_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_wafv2/test_server.py` & `moto-4.1.8.dev6/tests/test_wafv2/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_wafv2/test_utils.py` & `moto-4.1.8.dev6/tests/test_wafv2/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_wafv2/test_wafv2.py` & `moto-4.1.8.dev6/tests/test_wafv2/test_wafv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_wafv2/test_wafv2_integration.py` & `moto-4.1.8.dev6/tests/test_wafv2/test_wafv2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_wafv2/test_wafv2_tags.py` & `moto-4.1.8.dev6/tests/test_wafv2/test_wafv2_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_xray/test_xray_boto3.py` & `moto-4.1.8.dev6/tests/test_xray/test_xray_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.8.dev5/tests/test_xray/test_xray_client.py` & `moto-4.1.8.dev6/tests/test_xray/test_xray_client.py`

 * *Files identical despite different names*

