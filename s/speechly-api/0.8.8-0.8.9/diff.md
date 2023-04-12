# Comparing `tmp/speechly_api-0.8.8.tar.gz` & `tmp/speechly_api-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/markus_speechgrinder_com/sg/api/python/dist/tmpf21p_25l/speechly_api-0.8.8.tar", last modified: Mon Oct  3 13:36:02 2022, max compression
+gzip compressed data, was "/home/markus_speechgrinder_com/sg/api/python/dist/.tmp-g69cnn66/speechly_api-0.8.9.tar", last modified: Thu Dec  1 13:43:13 2022, max compression
```

## Comparing `speechly_api-0.8.8.tar` & `speechly_api-0.8.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.497326 speechly_api-0.8.8/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     4512 2022-10-03 13:36:02.497326 speechly_api-0.8.8/PKG-INFO
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3937 2022-05-04 11:23:48.000000 speechly_api-0.8.8/README.md
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)      104 2021-12-21 11:58:03.000000 speechly_api-0.8.8/pyproject.toml
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       38 2022-10-03 13:36:02.497326 speechly_api-0.8.8/setup.cfg
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1089 2022-10-03 13:35:55.000000 speechly_api-0.8.8/setup.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.485325 speechly_api-0.8.8/src/google/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/google/api/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     2142 2022-10-03 13:35:34.000000 speechly_api-0.8.8/src/google/api/annotations_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-10-03 13:35:34.000000 speechly_api-0.8.8/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    11487 2022-10-03 13:35:34.000000 speechly_api-0.8.8/src/google/api/http_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-10-03 13:35:34.000000 speechly_api-0.8.8/src/google/api/http_pb2_grpc.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/speechly/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/speechly/analytics/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/speechly/analytics/v1/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    21961 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/analytics/v1/analytics_api_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3834 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/analytics/v1/analytics_api_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    11315 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/analytics/v1/analytics_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/analytics/v1/analytics_pb2_grpc.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/speechly/config/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.493326 speechly_api-0.8.8/src/speechly/config/v1/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    59081 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/config/v1/config_api_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    13684 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/config/v1/config_api_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    11664 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/config/v1/model_api_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3152 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/config/v1/model_api_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3390 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/config/v1/model_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-10-03 13:35:30.000000 speechly_api-0.8.8/src/speechly/config/v1/model_pb2_grpc.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/speechly/identity/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.493326 speechly_api-0.8.8/src/speechly/identity/v1/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     6085 2022-10-03 13:35:31.000000 speechly_api-0.8.8/src/speechly/identity/v1/identity_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1728 2022-10-03 13:35:31.000000 speechly_api-0.8.8/src/speechly/identity/v1/identity_pb2_grpc.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.493326 speechly_api-0.8.8/src/speechly/identity/v2/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     8250 2022-10-03 13:35:32.000000 speechly_api-0.8.8/src/speechly/identity/v2/identity_api_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1776 2022-10-03 13:35:32.000000 speechly_api-0.8.8/src/speechly/identity/v2/identity_api_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     4402 2022-10-03 13:35:32.000000 speechly_api-0.8.8/src/speechly/identity/v2/identity_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-10-03 13:35:32.000000 speechly_api-0.8.8/src/speechly/identity/v2/identity_pb2_grpc.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/speechly/sal/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.493326 speechly_api-0.8.8/src/speechly/sal/v1/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    27167 2022-10-03 13:35:32.000000 speechly_api-0.8.8/src/speechly/sal/v1/compiler_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     4965 2022-10-03 13:35:32.000000 speechly_api-0.8.8/src/speechly/sal/v1/compiler_pb2_grpc.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.489326 speechly_api-0.8.8/src/speechly/slu/
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.493326 speechly_api-0.8.8/src/speechly/slu/v1/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    15333 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/batch_api_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3160 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/batch_api_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    21074 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/batch_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/batch_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    47978 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/slu_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3422 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/slu_pb2_grpc.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    18328 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/wlu_pb2.py
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3113 2022-10-03 13:35:33.000000 speechly_api-0.8.8/src/speechly/slu/v1/wlu_pb2_grpc.py
-drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-10-03 13:36:02.497326 speechly_api-0.8.8/src/speechly_api.egg-info/
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     4512 2022-10-03 13:36:02.000000 speechly_api-0.8.8/src/speechly_api.egg-info/PKG-INFO
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1433 2022-10-03 13:36:02.000000 speechly_api-0.8.8/src/speechly_api.egg-info/SOURCES.txt
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        1 2022-10-03 13:36:02.000000 speechly_api-0.8.8/src/speechly_api.egg-info/dependency_links.txt
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       26 2022-10-03 13:36:02.000000 speechly_api-0.8.8/src/speechly_api.egg-info/requires.txt
--rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       16 2022-10-03 13:36:02.000000 speechly_api-0.8.8/src/speechly_api.egg-info/top_level.txt
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.821067 speechly_api-0.8.9/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     6216 2022-12-01 13:43:13.821067 speechly_api-0.8.9/PKG-INFO
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     5641 2022-12-01 13:40:49.000000 speechly_api-0.8.9/README.md
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)      104 2021-12-21 11:58:03.000000 speechly_api-0.8.9/pyproject.toml
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       38 2022-12-01 13:43:13.821067 speechly_api-0.8.9/setup.cfg
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1089 2022-12-01 13:43:06.000000 speechly_api-0.8.9/setup.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.813067 speechly_api-0.8.9/src/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.809066 speechly_api-0.8.9/src/google/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.813067 speechly_api-0.8.9/src/google/api/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     2142 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/google/api/annotations_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-12-01 13:41:40.000000 speechly_api-0.8.9/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    11487 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/google/api/http_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-12-01 13:41:40.000000 speechly_api-0.8.9/src/google/api/http_pb2_grpc.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.813067 speechly_api-0.8.9/src/speechly/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.809066 speechly_api-0.8.9/src/speechly/analytics/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.817067 speechly_api-0.8.9/src/speechly/analytics/v1/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    21961 2022-12-01 13:41:40.000000 speechly_api-0.8.9/src/speechly/analytics/v1/analytics_api_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3834 2022-12-01 13:41:40.000000 speechly_api-0.8.9/src/speechly/analytics/v1/analytics_api_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    11315 2022-12-01 13:41:40.000000 speechly_api-0.8.9/src/speechly/analytics/v1/analytics_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-12-01 13:41:40.000000 speechly_api-0.8.9/src/speechly/analytics/v1/analytics_pb2_grpc.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.813067 speechly_api-0.8.9/src/speechly/config/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.817067 speechly_api-0.8.9/src/speechly/config/v1/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    59081 2022-12-01 13:41:36.000000 speechly_api-0.8.9/src/speechly/config/v1/config_api_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    13684 2022-12-01 13:41:36.000000 speechly_api-0.8.9/src/speechly/config/v1/config_api_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    11664 2022-12-01 13:41:36.000000 speechly_api-0.8.9/src/speechly/config/v1/model_api_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3152 2022-12-01 13:41:36.000000 speechly_api-0.8.9/src/speechly/config/v1/model_api_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3390 2022-12-01 13:41:36.000000 speechly_api-0.8.9/src/speechly/config/v1/model_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-12-01 13:41:36.000000 speechly_api-0.8.9/src/speechly/config/v1/model_pb2_grpc.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.813067 speechly_api-0.8.9/src/speechly/identity/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.817067 speechly_api-0.8.9/src/speechly/identity/v1/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     6085 2022-12-01 13:41:37.000000 speechly_api-0.8.9/src/speechly/identity/v1/identity_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1728 2022-12-01 13:41:37.000000 speechly_api-0.8.9/src/speechly/identity/v1/identity_pb2_grpc.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.817067 speechly_api-0.8.9/src/speechly/identity/v2/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     8250 2022-12-01 13:41:37.000000 speechly_api-0.8.9/src/speechly/identity/v2/identity_api_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1776 2022-12-01 13:41:37.000000 speechly_api-0.8.9/src/speechly/identity/v2/identity_api_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     4402 2022-12-01 13:41:37.000000 speechly_api-0.8.9/src/speechly/identity/v2/identity_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-12-01 13:41:37.000000 speechly_api-0.8.9/src/speechly/identity/v2/identity_pb2_grpc.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.813067 speechly_api-0.8.9/src/speechly/sal/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.817067 speechly_api-0.8.9/src/speechly/sal/v1/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    27167 2022-12-01 13:41:38.000000 speechly_api-0.8.9/src/speechly/sal/v1/compiler_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     4965 2022-12-01 13:41:38.000000 speechly_api-0.8.9/src/speechly/sal/v1/compiler_pb2_grpc.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.813067 speechly_api-0.8.9/src/speechly/slu/
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.821067 speechly_api-0.8.9/src/speechly/slu/v1/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    15333 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/batch_api_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3160 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/batch_api_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    21544 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/batch_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       83 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/batch_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    47978 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/slu_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3422 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/slu_pb2_grpc.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)    18328 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/wlu_pb2.py
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     3113 2022-12-01 13:41:39.000000 speechly_api-0.8.9/src/speechly/slu/v1/wlu_pb2_grpc.py
+drwxr-xr-x   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        0 2022-12-01 13:43:13.821067 speechly_api-0.8.9/src/speechly_api.egg-info/
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     6216 2022-12-01 13:43:13.000000 speechly_api-0.8.9/src/speechly_api.egg-info/PKG-INFO
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)     1433 2022-12-01 13:43:13.000000 speechly_api-0.8.9/src/speechly_api.egg-info/SOURCES.txt
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)        1 2022-12-01 13:43:13.000000 speechly_api-0.8.9/src/speechly_api.egg-info/dependency_links.txt
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       26 2022-12-01 13:43:13.000000 speechly_api-0.8.9/src/speechly_api.egg-info/requires.txt
+-rw-r--r--   0 markus_speechgrinder_com (1556644975) markus_speechgrinder_com (1556644975)       16 2022-12-01 13:43:13.000000 speechly_api-0.8.9/src/speechly_api.egg-info/top_level.txt
```

### Comparing `speechly_api-0.8.8/PKG-INFO` & `speechly_api-0.8.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechly_api
-Version: 0.8.8
+Version: 0.8.9
 Summary: Speechly Public Protobuf Stubs
 Home-page: https://github.com/speechly/api/tree/master/python
 Author: Speechly
 Project-URL: Speechly, https://www.speechly.com/
 Project-URL: Source, https://github.com/speechly/api
 Keywords: speech,asr,language,nlp
 Classifier: Development Status :: 4 - Beta
@@ -112,7 +112,65 @@
             intent, entities, transcript = r[0]
             print('Intent:', intent)
             print('Entities:', ', '.join(entities))
             print('Transcript:', ' '.join(transcript))
         except grpc.aio.AioRpcError as e:
             print('Error in SLU', str(e.code()), e.details())
 ```
+
+# Using the HTTP REST API
+
+The gRPC API is available also as JSON-based HTTP version. The following is an example of calling the `BatchAPI` with python `requests` library:
+
+
+```python
+import requests
+import uuid
+import base64
+import time
+
+# read an audio file in memory (note that the it should be PCM 16Khz 1 channels to get good results)
+with open('test1_en.wav', 'rb') as f:
+    audio_data = f.read()
+
+# create a device ID (uuid)
+deviceId = uuid.uuid4()
+
+# get a Speechly access token to use the correct Speechly app
+r = requests.post(
+    'https://api.speechly.com/speechly.identity.v2.IdentityAPI/Login',
+    json={'deviceId': str(deviceId), 'application': {'appId': 'YOUR_APP_ID'}}
+)
+token = r.json()['token']
+
+# send the file to the BatchAPI to create a batch transcribe operation
+batch_req = [{
+    'config': {
+        'encoding': 1,
+        'channels': 1,
+        'sampleRateHertz': 16000
+    },
+    'audio': base64.b64encode(audio_data).decode('ascii')
+}]
+r = requests.post(
+    'https://api.speechly.com/speechly.slu.v1.BatchAPI/ProcessAudio',
+    headers={'authorization':f'Bearer {token}'},
+    json=batch_req
+)
+op = r.json()['operation']
+
+# poll the BatchAPI, waiting for the batch operation to be done
+while op['status'] != 'STATUS_DONE':
+    time.sleep(1)
+    r = requests.post(
+        'https://api.speechly.com/speechly.slu.v1.BatchAPI/QueryStatus',
+        headers={'authorization':f'Bearer {token}'},
+        json={'id': op['id']}
+    )
+    op = r.json()['operation']
+    if op['error'] != '':
+        raise Exception('error in transcribe: ' + op['error'])
+
+# collect the words from the transcripts
+transcript = [w['word'] for w in op['transcripts']]
+print(' '.join(transcript))
+```
```

### Comparing `speechly_api-0.8.8/setup.py` & `speechly_api-0.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='speechly_api',
-    version='0.8.8',
+    version='0.8.9',
     description='Speechly Public Protobuf Stubs',
     include_package_data=True,
-    install_requires=['grpcio>1.30', 'protobuf>3.14'],
+    install_requires=['grpcio>1.40', 'protobuf>3.20'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/speechly/api/tree/master/python',
     author='Speechly',
     keywords=['speech', 'asr', 'language', 'nlp'],
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `speechly_api-0.8.8/src/google/api/annotations_pb2.py` & `speechly_api-0.8.9/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/google/api/http_pb2.py` & `speechly_api-0.8.9/src/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/analytics/v1/analytics_api_pb2.py` & `speechly_api-0.8.9/src/speechly/analytics/v1/analytics_api_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/analytics/v1/analytics_api_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/analytics/v1/analytics_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/analytics/v1/analytics_pb2.py` & `speechly_api-0.8.9/src/speechly/analytics/v1/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/config/v1/config_api_pb2.py` & `speechly_api-0.8.9/src/speechly/config/v1/config_api_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/config/v1/config_api_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/config/v1/config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/config/v1/model_api_pb2.py` & `speechly_api-0.8.9/src/speechly/config/v1/model_api_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/config/v1/model_api_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/config/v1/model_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/config/v1/model_pb2.py` & `speechly_api-0.8.9/src/speechly/config/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/identity/v1/identity_pb2.py` & `speechly_api-0.8.9/src/speechly/identity/v1/identity_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/identity/v1/identity_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/identity/v1/identity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/identity/v2/identity_api_pb2.py` & `speechly_api-0.8.9/src/speechly/identity/v2/identity_api_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/identity/v2/identity_api_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/identity/v2/identity_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/identity/v2/identity_pb2.py` & `speechly_api-0.8.9/src/speechly/identity/v2/identity_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/sal/v1/compiler_pb2.py` & `speechly_api-0.8.9/src/speechly/sal/v1/compiler_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/sal/v1/compiler_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/sal/v1/compiler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/slu/v1/batch_api_pb2.py` & `speechly_api-0.8.9/src/speechly/slu/v1/batch_api_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/slu/v1/batch_api_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/slu/v1/batch_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/slu/v1/batch_pb2.py` & `speechly_api-0.8.9/src/speechly/slu/v1/batch_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='speechly/slu/v1/batch.proto',
   package='speechly.slu.v1',
   syntax='proto3',
   serialized_options=b'\n\023com.speechly.slu.v1B\nBatchProtoP\001Z\025speechly/slu/v1;sluv1\242\002\003SSX\252\002\017Speechly.Slu.V1\312\002\017Speechly\\Slu\\V1',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1bspeechly/slu/v1/batch.proto\x12\x0fspeechly.slu.v1\"\xd2\x01\n\x12\x41udioConfiguration\x12>\n\x08\x65ncoding\x18\x01 \x01(\x0e\x32,.speechly.slu.v1.AudioConfiguration.Encoding\x12\x10\n\x08\x63hannels\x18\x02 \x01(\x05\x12\x19\n\x11sample_rate_hertz\x18\x03 \x01(\x05\x12\x16\n\x0elanguage_codes\x18\x04 \x03(\t\"7\n\x08\x45ncoding\x12\x14\n\x10\x45NCODING_INVALID\x10\x00\x12\x15\n\x11\x45NCODING_LINEAR16\x10\x01\"\xfe\x01\n\x0cHttpResource\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x34\n\x06method\x18\x02 \x01(\x0e\x32$.speechly.slu.v1.HttpResource.Method\x12\x35\n\x07headers\x18\x03 \x03(\x0b\x32$.speechly.slu.v1.HttpResource.Header\x1a%\n\x06Header\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"M\n\x06Method\x12\x12\n\x0eMETHOD_INVALID\x10\x00\x12\x0e\n\nMETHOD_GET\x10\x01\x12\x0f\n\x0bMETHOD_POST\x10\x02\x12\x0e\n\nMETHOD_PUT\x10\x03\"\xc3\x02\n\tOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\x12\x31\n\x06status\x18\x03 \x01(\x0e\x32!.speechly.slu.v1.Operation.Status\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12\x11\n\tdevice_id\x18\x06 \x01(\t\x12\x30\n\x0btranscripts\x18\x07 \x03(\x0b\x32\x1b.speechly.slu.v1.Transcript\x12\r\n\x05\x65rror\x18\x08 \x01(\t\"i\n\x06Status\x12\x12\n\x0eSTATUS_INVALID\x10\x00\x12\x11\n\rSTATUS_QUEUED\x10\x01\x12\x15\n\x11STATUS_PROCESSING\x10\x02\x12\x0f\n\x0bSTATUS_DONE\x10\x03\x12\x10\n\x0cSTATUS_ERROR\x10\x04\"O\n\nTranscript\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\r\n\x05index\x18\x02 \x01(\x05\x12\x12\n\nstart_time\x18\x03 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\x05\"$\n\x06Option\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x03(\tBd\n\x13\x63om.speechly.slu.v1B\nBatchProtoP\x01Z\x15speechly/slu/v1;sluv1\xa2\x02\x03SSX\xaa\x02\x0fSpeechly.Slu.V1\xca\x02\x0fSpeechly\\Slu\\V1b\x06proto3'
+  serialized_pb=b'\n\x1bspeechly/slu/v1/batch.proto\x12\x0fspeechly.slu.v1\"\xd2\x01\n\x12\x41udioConfiguration\x12>\n\x08\x65ncoding\x18\x01 \x01(\x0e\x32,.speechly.slu.v1.AudioConfiguration.Encoding\x12\x10\n\x08\x63hannels\x18\x02 \x01(\x05\x12\x19\n\x11sample_rate_hertz\x18\x03 \x01(\x05\x12\x16\n\x0elanguage_codes\x18\x04 \x03(\t\"7\n\x08\x45ncoding\x12\x14\n\x10\x45NCODING_INVALID\x10\x00\x12\x15\n\x11\x45NCODING_LINEAR16\x10\x01\"\xfe\x01\n\x0cHttpResource\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x34\n\x06method\x18\x02 \x01(\x0e\x32$.speechly.slu.v1.HttpResource.Method\x12\x35\n\x07headers\x18\x03 \x03(\x0b\x32$.speechly.slu.v1.HttpResource.Header\x1a%\n\x06Header\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"M\n\x06Method\x12\x12\n\x0eMETHOD_INVALID\x10\x00\x12\x0e\n\nMETHOD_GET\x10\x01\x12\x0f\n\x0bMETHOD_POST\x10\x02\x12\x0e\n\nMETHOD_PUT\x10\x03\"\xf6\x02\n\tOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\x12\x31\n\x06status\x18\x03 \x01(\x0e\x32!.speechly.slu.v1.Operation.Status\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12\x11\n\tdevice_id\x18\x06 \x01(\t\x12\x30\n\x0btranscripts\x18\x07 \x03(\x0b\x32\x1b.speechly.slu.v1.Transcript\x12\r\n\x05\x65rror\x18\x08 \x01(\t\"\x9b\x01\n\x06Status\x12\x12\n\x0eSTATUS_INVALID\x10\x00\x12\x11\n\rSTATUS_QUEUED\x10\x01\x12\x15\n\x11STATUS_PROCESSING\x10\x02\x12\x0f\n\x0bSTATUS_DONE\x10\x03\x12\x10\n\x0cSTATUS_ERROR\x10\x04\x12\x14\n\x10STATUS_ANALYSING\x10\x05\x12\x1a\n\x16STATUS_WAITING_DECODER\x10\x06\"O\n\nTranscript\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\r\n\x05index\x18\x02 \x01(\x05\x12\x12\n\nstart_time\x18\x03 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\x05\"$\n\x06Option\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x03(\tBd\n\x13\x63om.speechly.slu.v1B\nBatchProtoP\x01Z\x15speechly/slu/v1;sluv1\xa2\x02\x03SSX\xaa\x02\x0fSpeechly.Slu.V1\xca\x02\x0fSpeechly\\Slu\\V1b\x06proto3'
 )
 
 
 
 _AUDIOCONFIGURATION_ENCODING = _descriptor.EnumDescriptor(
   name='Encoding',
   full_name='speechly.slu.v1.AudioConfiguration.Encoding',
@@ -112,19 +112,29 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='STATUS_ERROR', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='STATUS_ANALYSING', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='STATUS_WAITING_DECODER', index=6, number=6,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=737,
-  serialized_end=842,
+  serialized_start=738,
+  serialized_end=893,
 )
 _sym_db.RegisterEnumDescriptor(_OPERATION_STATUS)
 
 
 _AUDIOCONFIGURATION = _descriptor.Descriptor(
   name='AudioConfiguration',
   full_name='speechly.slu.v1.AudioConfiguration',
@@ -338,15 +348,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=519,
-  serialized_end=842,
+  serialized_end=893,
 )
 
 
 _TRANSCRIPT = _descriptor.Descriptor(
   name='Transcript',
   full_name='speechly.slu.v1.Transcript',
   filename=None,
@@ -390,16 +400,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=844,
-  serialized_end=923,
+  serialized_start=895,
+  serialized_end=974,
 )
 
 
 _OPTION = _descriptor.Descriptor(
   name='Option',
   full_name='speechly.slu.v1.Option',
   filename=None,
@@ -429,16 +439,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=925,
-  serialized_end=961,
+  serialized_start=976,
+  serialized_end=1012,
 )
 
 _AUDIOCONFIGURATION.fields_by_name['encoding'].enum_type = _AUDIOCONFIGURATION_ENCODING
 _AUDIOCONFIGURATION_ENCODING.containing_type = _AUDIOCONFIGURATION
 _HTTPRESOURCE_HEADER.containing_type = _HTTPRESOURCE
 _HTTPRESOURCE.fields_by_name['method'].enum_type = _HTTPRESOURCE_METHOD
 _HTTPRESOURCE.fields_by_name['headers'].message_type = _HTTPRESOURCE_HEADER
```

### Comparing `speechly_api-0.8.8/src/speechly/slu/v1/slu_pb2.py` & `speechly_api-0.8.9/src/speechly/slu/v1/slu_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/slu/v1/slu_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/slu/v1/slu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/slu/v1/wlu_pb2.py` & `speechly_api-0.8.9/src/speechly/slu/v1/wlu_pb2.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly/slu/v1/wlu_pb2_grpc.py` & `speechly_api-0.8.9/src/speechly/slu/v1/wlu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechly_api-0.8.8/src/speechly_api.egg-info/PKG-INFO` & `speechly_api-0.8.9/src/speechly_api.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechly-api
-Version: 0.8.8
+Version: 0.8.9
 Summary: Speechly Public Protobuf Stubs
 Home-page: https://github.com/speechly/api/tree/master/python
 Author: Speechly
 Project-URL: Speechly, https://www.speechly.com/
 Project-URL: Source, https://github.com/speechly/api
 Keywords: speech,asr,language,nlp
 Classifier: Development Status :: 4 - Beta
@@ -112,7 +112,65 @@
             intent, entities, transcript = r[0]
             print('Intent:', intent)
             print('Entities:', ', '.join(entities))
             print('Transcript:', ' '.join(transcript))
         except grpc.aio.AioRpcError as e:
             print('Error in SLU', str(e.code()), e.details())
 ```
+
+# Using the HTTP REST API
+
+The gRPC API is available also as JSON-based HTTP version. The following is an example of calling the `BatchAPI` with python `requests` library:
+
+
+```python
+import requests
+import uuid
+import base64
+import time
+
+# read an audio file in memory (note that the it should be PCM 16Khz 1 channels to get good results)
+with open('test1_en.wav', 'rb') as f:
+    audio_data = f.read()
+
+# create a device ID (uuid)
+deviceId = uuid.uuid4()
+
+# get a Speechly access token to use the correct Speechly app
+r = requests.post(
+    'https://api.speechly.com/speechly.identity.v2.IdentityAPI/Login',
+    json={'deviceId': str(deviceId), 'application': {'appId': 'YOUR_APP_ID'}}
+)
+token = r.json()['token']
+
+# send the file to the BatchAPI to create a batch transcribe operation
+batch_req = [{
+    'config': {
+        'encoding': 1,
+        'channels': 1,
+        'sampleRateHertz': 16000
+    },
+    'audio': base64.b64encode(audio_data).decode('ascii')
+}]
+r = requests.post(
+    'https://api.speechly.com/speechly.slu.v1.BatchAPI/ProcessAudio',
+    headers={'authorization':f'Bearer {token}'},
+    json=batch_req
+)
+op = r.json()['operation']
+
+# poll the BatchAPI, waiting for the batch operation to be done
+while op['status'] != 'STATUS_DONE':
+    time.sleep(1)
+    r = requests.post(
+        'https://api.speechly.com/speechly.slu.v1.BatchAPI/QueryStatus',
+        headers={'authorization':f'Bearer {token}'},
+        json={'id': op['id']}
+    )
+    op = r.json()['operation']
+    if op['error'] != '':
+        raise Exception('error in transcribe: ' + op['error'])
+
+# collect the words from the transcripts
+transcript = [w['word'] for w in op['transcripts']]
+print(' '.join(transcript))
+```
```

### Comparing `speechly_api-0.8.8/src/speechly_api.egg-info/SOURCES.txt` & `speechly_api-0.8.9/src/speechly_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

