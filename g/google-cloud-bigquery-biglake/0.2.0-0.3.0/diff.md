# Comparing `tmp/google-cloud-bigquery-biglake-0.2.0.tar.gz` & `tmp/google-cloud-bigquery-biglake-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-biglake-0.2.0.tar", last modified: Thu Apr  6 13:28:14 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-biglake-0.3.0.tar", last modified: Wed Apr 12 14:13:15 2023, max compression
```

## Comparing `google-cloud-bigquery-biglake-0.2.0.tar` & `google-cloud-bigquery-biglake-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,76 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4685 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3759 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.143173 google-cloud-bigquery-biglake-0.2.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.143173 google-cloud-bigquery-biglake-0.2.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.143173 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.147174 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake/
--rw-rw-r--   0 root         (0)     1003     2518 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.147174 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/
--rw-rw-r--   0 root         (0)     1003     2349 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7450 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.147174 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.147174 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    95360 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   109333 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/client.py
--rw-rw-r--   0 root         (0)     1003    20793 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.147174 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13545 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31716 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    32496 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   101231 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/types/
--rw-rw-r--   0 root         (0)     1003     2044 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    32213 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/types/metastore.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/
--rw-r--r--   0 root         (0)     1003     4685 2023-04-06 13:28:14.000000 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1859 2023-04-06 13:28:14.000000 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-06 13:28:14.000000 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2023-04-06 13:28:14.000000 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-06 13:28:14.000000 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-06 13:28:14.000000 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-06 13:28:14.000000 google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2984 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:14.151174 google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/biglake_v1alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/biglake_v1alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   451218 2023-04-06 13:25:25.000000 google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/biglake_v1alpha1/test_metastore_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4685 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3759 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.318014 google-cloud-bigquery-biglake-0.3.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.318014 google-cloud-bigquery-biglake-0.3.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.318014 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/
+-rw-rw-r--   0 root         (0)     1003     2242 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/
+-rw-rw-r--   0 root         (0)     1003     2085 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6058 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    77802 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    90452 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15709 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.322015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11893 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27356 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28003 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    82223 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1786 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26313 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/types/metastore.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003     2349 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7450 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    95360 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   109333 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/client.py
+-rw-rw-r--   0 root         (0)     1003    20793 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13545 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31716 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    32496 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   101231 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.326015 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     2044 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32213 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/metastore.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/
+-rw-r--r--   0 root         (0)     1003     4685 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2995 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       42 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-12 14:13:15.000000 google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2984 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   369886 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1/test_metastore_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:15.330016 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   451218 2023-04-12 14:10:39.000000 google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/test_metastore_service.py
```

### Comparing `google-cloud-bigquery-biglake-0.2.0/LICENSE` & `google-cloud-bigquery-biglake-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/MANIFEST.in` & `google-cloud-bigquery-biglake-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/PKG-INFO` & `google-cloud-bigquery-biglake-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-biglake
-Version: 0.2.0
+Version: 0.3.0
 Summary: Google Cloud Bigquery Biglake API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-biglake-0.2.0/README.rst` & `google-cloud-bigquery-biglake-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,85 +9,71 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.bigquery.biglake import gapic_version as package_version
+from google.cloud.bigquery.biglake_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.async_client import (
+from .services.metastore_service import (
     MetastoreServiceAsyncClient,
-)
-from google.cloud.bigquery.biglake_v1alpha1.services.metastore_service.client import (
     MetastoreServiceClient,
 )
-from google.cloud.bigquery.biglake_v1alpha1.types.metastore import (
+from .types.metastore import (
     Catalog,
-    CheckLockRequest,
     CreateCatalogRequest,
     CreateDatabaseRequest,
-    CreateLockRequest,
     CreateTableRequest,
     Database,
     DeleteCatalogRequest,
     DeleteDatabaseRequest,
-    DeleteLockRequest,
     DeleteTableRequest,
     GetCatalogRequest,
     GetDatabaseRequest,
     GetTableRequest,
     HiveDatabaseOptions,
     HiveTableOptions,
     ListCatalogsRequest,
     ListCatalogsResponse,
     ListDatabasesRequest,
     ListDatabasesResponse,
-    ListLocksRequest,
-    ListLocksResponse,
     ListTablesRequest,
     ListTablesResponse,
-    Lock,
     RenameTableRequest,
     Table,
     TableView,
     UpdateDatabaseRequest,
     UpdateTableRequest,
 )
 
 __all__ = (
-    "MetastoreServiceClient",
     "MetastoreServiceAsyncClient",
     "Catalog",
-    "CheckLockRequest",
     "CreateCatalogRequest",
     "CreateDatabaseRequest",
-    "CreateLockRequest",
     "CreateTableRequest",
     "Database",
     "DeleteCatalogRequest",
     "DeleteDatabaseRequest",
-    "DeleteLockRequest",
     "DeleteTableRequest",
     "GetCatalogRequest",
     "GetDatabaseRequest",
     "GetTableRequest",
     "HiveDatabaseOptions",
     "HiveTableOptions",
     "ListCatalogsRequest",
     "ListCatalogsResponse",
     "ListDatabasesRequest",
     "ListDatabasesResponse",
-    "ListLocksRequest",
-    "ListLocksResponse",
     "ListTablesRequest",
     "ListTablesResponse",
-    "Lock",
+    "MetastoreServiceClient",
     "RenameTableRequest",
     "Table",
+    "TableView",
     "UpdateDatabaseRequest",
     "UpdateTableRequest",
-    "TableView",
 )
```

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake/gapic_version.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/gapic_metadata.json` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/gapic_version.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/async_client.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/client.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/pagers.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1/services/metastore_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/base.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/rest.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/metastore_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/types/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google/cloud/bigquery/biglake_v1alpha1/types/metastore.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/types/metastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO` & `google-cloud-bigquery-biglake-0.3.0/google_cloud_bigquery_biglake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-biglake
-Version: 0.2.0
+Version: 0.3.0
 Summary: Google Cloud Bigquery Biglake API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-biglake-0.2.0/setup.py` & `google-cloud-bigquery-biglake-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/tests/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/google/cloud/bigquery/biglake_v1alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/tests/unit/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/biglake_v1alpha1/__init__.py` & `google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-biglake-0.2.0/tests/unit/gapic/biglake_v1alpha1/test_metastore_service.py` & `google-cloud-bigquery-biglake-0.3.0/tests/unit/gapic/biglake_v1alpha1/test_metastore_service.py`

 * *Files identical despite different names*

