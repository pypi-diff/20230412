# Comparing `tmp/trex-analytic-0.1.2.tar.gz` & `tmp/trex-analytic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-analytic-0.1.2.tar", last modified: Mon Mar 27 08:06:27 2023, max compression
+gzip compressed data, was "dist/trex-analytic-0.1.3.tar", last modified: Wed Apr 12 07:07:14 2023, max compression
```

## Comparing `trex-analytic-0.1.2.tar` & `trex-analytic-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/
--rw-r--r--   0 jacklok    (501) staff       (20)      359 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     2622 2021-01-11 01:11:49.000000 trex-analytic-0.1.2/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      707 2023-03-27 08:05:25.000000 trex-analytic-0.1.2/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/tests/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 08:40:47.000000 trex-analytic-0.1.2/tests/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      974 2021-01-18 02:08:03.000000 trex-analytic-0.1.2/tests/test_chart_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      559 2021-01-21 09:11:07.000000 trex-analytic-0.1.2/tests/test_cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3063 2021-01-20 07:30:52.000000 trex-analytic-0.1.2/tests/test_create_bigquery_table.py
--rw-r--r--   0 jacklok    (501) staff       (20)      595 2021-01-15 01:14:30.000000 trex-analytic-0.1.2/tests/test_delete_bigquery_dataset.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1325 2021-01-15 06:16:18.000000 trex-analytic-0.1.2/tests/test_import_customer_data.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2343 2021-01-20 01:23:38.000000 trex-analytic-0.1.2/tests/test_import_merchant_customer_data.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1320 2021-01-15 06:16:09.000000 trex-analytic-0.1.2/tests/test_import_merchant_data.py
--rw-r--r--   0 jacklok    (501) staff       (20)      748 2021-01-15 01:23:07.000000 trex-analytic-0.1.2/tests/test_list_table_from_dataset.py
--rw-r--r--   0 jacklok    (501) staff       (20)      380 2021-01-19 07:00:13.000000 trex-analytic-0.1.2/tests/test_main_app.py
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2021-07-01 02:28:22.000000 trex-analytic-0.1.2/tests/test_query_customer.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trex_analytic.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      359 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trex_analytic.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1892 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trex_analytic.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trex_analytic.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       98 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trex_analytic.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       20 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trex_analytic.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:25:07.000000 trex-analytic-0.1.2/trexanalytics/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9229 2023-02-10 11:21:00.000000 trex-analytic-0.1.2/trexanalytics/bigquery_table_template_config.py
--rw-r--r--   0 jacklok    (501) staff       (20)    18149 2023-03-06 07:44:32.000000 trex-analytic-0.1.2/trexanalytics/bigquery_upstream_data_config.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4484 2023-02-23 10:06:43.000000 trex-analytic-0.1.2/trexanalytics/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:45:04.000000 trex-analytic-0.1.2/trexanalytics/controllers/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/controllers/bigquery/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-18 05:12:38.000000 trex-analytic-0.1.2/trexanalytics/controllers/bigquery/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14411 2023-03-07 02:42:00.000000 trex-analytic-0.1.2/trexanalytics/controllers/bigquery/customer_query_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2540 2023-03-07 04:22:38.000000 trex-analytic-0.1.2/trexanalytics/controllers/bigquery/query_base_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5383 2021-07-01 02:13:45.000000 trex-analytic-0.1.2/trexanalytics/controllers/bigquery/redemption_query_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5566 2021-07-01 02:13:41.000000 trex-analytic-0.1.2/trexanalytics/controllers/bigquery/rewarding_query_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14535 2021-08-30 06:35:04.000000 trex-analytic-0.1.2/trexanalytics/controllers/bigquery/transaction_query_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-12 02:42:37.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19860 2022-09-29 03:34:40.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_customer_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14404 2023-02-27 08:40:04.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_data_base_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6544 2021-08-20 10:27:07.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_merchant_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8306 2021-08-20 10:27:16.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_transaction_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17823 2023-02-27 07:41:18.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_upstream_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)       49 2021-01-21 07:31:55.000000 trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_user_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2473 2022-09-23 07:30:35.000000 trex-analytic-0.1.2/trexanalytics/controllers/main_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/controllers/template/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:02:49.000000 trex-analytic-0.1.2/trexanalytics/controllers/template/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      907 2021-01-20 09:34:38.000000 trex-analytic-0.1.2/trexanalytics/controllers/template/table_template_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/controllers/upstreamdata/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-26 10:02:40.000000 trex-analytic-0.1.2/trexanalytics/controllers/upstreamdata/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/helper/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-03-27 04:02:29.000000 trex-analytic-0.1.2/trexanalytics/helper/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2787 2023-03-27 07:33:27.000000 trex-analytic-0.1.2/trexanalytics/helper/bigquery_upstream_helpers.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-27 08:06:27.000000 trex-analytic-0.1.2/trexanalytics/util/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:16:58.000000 trex-analytic-0.1.2/trexanalytics/util/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      537 2021-01-18 02:07:17.000000 trex-analytic-0.1.2/trexanalytics/util/chart_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/
+-rw-r--r--   0 jacklok    (501) staff       (20)      359 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     2622 2021-01-11 01:11:49.000000 trex-analytic-0.1.3/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      707 2023-04-12 06:57:34.000000 trex-analytic-0.1.3/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/tests/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 08:40:47.000000 trex-analytic-0.1.3/tests/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      974 2021-01-18 02:08:03.000000 trex-analytic-0.1.3/tests/test_chart_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      559 2021-01-21 09:11:07.000000 trex-analytic-0.1.3/tests/test_cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3063 2021-01-20 07:30:52.000000 trex-analytic-0.1.3/tests/test_create_bigquery_table.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      595 2021-01-15 01:14:30.000000 trex-analytic-0.1.3/tests/test_delete_bigquery_dataset.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1325 2021-01-15 06:16:18.000000 trex-analytic-0.1.3/tests/test_import_customer_data.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2343 2021-01-20 01:23:38.000000 trex-analytic-0.1.3/tests/test_import_merchant_customer_data.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1320 2021-01-15 06:16:09.000000 trex-analytic-0.1.3/tests/test_import_merchant_data.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      748 2021-01-15 01:23:07.000000 trex-analytic-0.1.3/tests/test_list_table_from_dataset.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      380 2021-01-19 07:00:13.000000 trex-analytic-0.1.3/tests/test_main_app.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2021-07-01 02:28:22.000000 trex-analytic-0.1.3/tests/test_query_customer.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trex_analytic.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      359 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trex_analytic.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1892 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trex_analytic.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trex_analytic.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       98 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trex_analytic.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       20 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trex_analytic.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:25:07.000000 trex-analytic-0.1.3/trexanalytics/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9229 2023-02-10 11:21:00.000000 trex-analytic-0.1.3/trexanalytics/bigquery_table_template_config.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    18968 2023-04-11 07:52:10.000000 trex-analytic-0.1.3/trexanalytics/bigquery_upstream_data_config.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4484 2023-02-23 10:06:43.000000 trex-analytic-0.1.3/trexanalytics/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:45:04.000000 trex-analytic-0.1.3/trexanalytics/controllers/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/controllers/bigquery/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-18 05:12:38.000000 trex-analytic-0.1.3/trexanalytics/controllers/bigquery/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14411 2023-03-07 02:42:00.000000 trex-analytic-0.1.3/trexanalytics/controllers/bigquery/customer_query_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2540 2023-03-07 04:22:38.000000 trex-analytic-0.1.3/trexanalytics/controllers/bigquery/query_base_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5383 2021-07-01 02:13:45.000000 trex-analytic-0.1.3/trexanalytics/controllers/bigquery/redemption_query_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5566 2021-07-01 02:13:41.000000 trex-analytic-0.1.3/trexanalytics/controllers/bigquery/rewarding_query_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14535 2021-08-30 06:35:04.000000 trex-analytic-0.1.3/trexanalytics/controllers/bigquery/transaction_query_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-12 02:42:37.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19860 2022-09-29 03:34:40.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_customer_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14404 2023-02-27 08:40:04.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_data_base_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6544 2021-08-20 10:27:07.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_merchant_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8306 2021-08-20 10:27:16.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_transaction_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17823 2023-02-27 07:41:18.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_upstream_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)       49 2021-01-21 07:31:55.000000 trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_user_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2473 2022-09-23 07:30:35.000000 trex-analytic-0.1.3/trexanalytics/controllers/main_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/controllers/template/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:02:49.000000 trex-analytic-0.1.3/trexanalytics/controllers/template/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      907 2021-01-20 09:34:38.000000 trex-analytic-0.1.3/trexanalytics/controllers/template/table_template_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/controllers/upstreamdata/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-26 10:02:40.000000 trex-analytic-0.1.3/trexanalytics/controllers/upstreamdata/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/helper/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-03-27 04:02:29.000000 trex-analytic-0.1.3/trexanalytics/helper/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3549 2023-03-27 10:56:12.000000 trex-analytic-0.1.3/trexanalytics/helper/bigquery_upstream_helpers.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-12 07:07:14.000000 trex-analytic-0.1.3/trexanalytics/util/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:16:58.000000 trex-analytic-0.1.3/trexanalytics/util/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      537 2021-01-18 02:07:17.000000 trex-analytic-0.1.3/trexanalytics/util/chart_util.py
```

### Comparing `trex-analytic-0.1.2/README.md` & `trex-analytic-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/setup.py` & `trex-analytic-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pip._vendor.pkg_resources import require
 
 setuptools.setup(
      name='trex-analytic',  
-     version='0.1.2',
+     version='0.1.3',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex analytics package",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
```

### Comparing `trex-analytic-0.1.2/tests/test_chart_util.py` & `trex-analytic-0.1.3/tests/test_chart_util.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_cloud_tasks_util.py` & `trex-analytic-0.1.3/tests/test_cloud_tasks_util.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_create_bigquery_table.py` & `trex-analytic-0.1.3/tests/test_create_bigquery_table.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_delete_bigquery_dataset.py` & `trex-analytic-0.1.3/tests/test_delete_bigquery_dataset.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_import_customer_data.py` & `trex-analytic-0.1.3/tests/test_import_customer_data.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_import_merchant_customer_data.py` & `trex-analytic-0.1.3/tests/test_import_merchant_customer_data.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_import_merchant_data.py` & `trex-analytic-0.1.3/tests/test_import_merchant_data.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_list_table_from_dataset.py` & `trex-analytic-0.1.3/tests/test_list_table_from_dataset.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/tests/test_query_customer.py` & `trex-analytic-0.1.3/tests/test_query_customer.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trex_analytic.egg-info/SOURCES.txt` & `trex-analytic-0.1.3/trex_analytic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/bigquery_table_template_config.py` & `trex-analytic-0.1.3/trexanalytics/bigquery_table_template_config.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/bigquery_upstream_data_config.py` & `trex-analytic-0.1.3/trexanalytics/bigquery_upstream_data_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,140 +116,150 @@
                             MERCHANT_CUSTOMER_REWARD_TEMPLATE       : __CUSTOMER_REWARD_DATA_TEMPLATE_UPSTREAM_SCHEMA,
                             MERCHANT_CUSTOMER_PREPAID_TEMPLATE      : __CUSTOMER_PREPAID_DATA_TEMPLATE_UPSTREAM_SCHEMA,
                             MERCHANT_CUSTOMER_REDEMPTION_TEMPLATE   : __CUSTOMER_REDEMPTION_DATA_TEMPLATE_UPSTREAM_SCHEMA,
                             }
 
 logger = logging.getLogger('upstream')
 
-def __create_upstream(upstream_entity, upstream_template, dataset_name, table_name, streamed_datetime=None, **kwargs):
+def __create_upstream(upstream_entity, merchant_acct, upstream_template, dataset_name, table_name, streamed_datetime=None, **kwargs):
     upstream_json = {}
     if upstream_entity:
         schema = upstream_schema_config.get(upstream_template)
         for upstrem_field_name, attr_name in schema.items():
             logger.debug('upstream_entity classname=%s', upstream_entity.__class__.__name__)
             upstream_json[upstrem_field_name] = default_serializable(getattr(upstream_entity, attr_name))
     
     if streamed_datetime is None:
         streamed_datetime = datetime.utcnow()
             
     upstream_json['Key'] = uuid.uuid1().hex
-    upstream_json[UPSTREAM_UPDATED_DATETIME_FIELD_NAME] = default_serializable(streamed_datetime)
+    
+    if (UPSTREAM_UPDATED_DATETIME_FIELD_NAME in upstream_json) == False:
+        upstream_json[UPSTREAM_UPDATED_DATETIME_FIELD_NAME] = default_serializable(streamed_datetime)
     
     #year = update_datetime.yeaar
     
     #dataset_with_year_prefix = '{year}_{dataset}'.format(year=year, dataset=dataset_name)
     
     for key, value in kwargs.items():
         upstream_json[key] = convert_to_serializable_value(value, datetime_format='%Y-%m-%d %H:%M:%S', date_format='%Y-%m-%d', time_format='%H:%M:%S')
     
     logger.debug('-------------------------------------------------')
     logger.debug('dataset_name=%s', dataset_name)
     logger.debug('table_name=%s', table_name)
     logger.debug('upstream_template=%s', upstream_template)
     logger.debug('upstream_json=%s', upstream_json)
     logger.debug('-------------------------------------------------')
-    UpstreamData.create(dataset_name, table_name, upstream_template, [upstream_json])
+    UpstreamData.create(merchant_acct, dataset_name, table_name, upstream_template, [upstream_json])
     
 
 def create_registered_customer_upstream_for_system(customer):
     streamed_datetime = datetime.utcnow()
     
     table_name          = REGISTERED_CUSTOMER_TEMPLATE
     final_table_name    = '{}_{}'.format(table_name, streamed_datetime.strftime('%Y%m%d'))
-    
-    __create_upstream(customer, REGISTERED_CUSTOMER_TEMPLATE, SYSTEM_DATASET, final_table_name, streamed_datetime=streamed_datetime)
+    merchant_acct       = customer.registered_merchant_acct
+    __create_upstream(customer, merchant_acct, REGISTERED_CUSTOMER_TEMPLATE, SYSTEM_DATASET, final_table_name, streamed_datetime=streamed_datetime)
 
 def create_merchant_registered_customer_upstream_for_merchant(customer):
     streamed_datetime = datetime.utcnow()
     
     table_name          = MERCHANT_REGISTERED_CUSTOMER_TEMPLATE
     merchant_acct       = customer.registered_merchant_acct
     account_code        = merchant_acct.account_code.replace('-','')
     final_table_name    = '{}_{}_{}'.format(table_name, account_code, streamed_datetime.strftime('%Y%m%d'))
     
-    __create_upstream(customer, MERCHANT_REGISTERED_CUSTOMER_TEMPLATE, MERCHANT_DATASET, final_table_name, streamed_datetime=streamed_datetime)    
+    __create_upstream(customer, merchant_acct, MERCHANT_REGISTERED_CUSTOMER_TEMPLATE, MERCHANT_DATASET, final_table_name, streamed_datetime=streamed_datetime)    
     
 def create_merchant_customer_transaction_upstream_for_merchant(transaction_details, streamed_datetime=None):
     if streamed_datetime is None:
         streamed_datetime     = transaction_details.transact_datetime
         
     table_name          = CUSTOMER_TRANSACTION_TEMPLATE
     merchant_acct       = transaction_details.transact_merchant_acct
     account_code        = merchant_acct.account_code.replace('-','')
     final_table_name    = '{}_{}_{}'.format(table_name, account_code, streamed_datetime.strftime('%Y%m%d'))
     
-    __create_upstream(transaction_details, CUSTOMER_TRANSACTION_TEMPLATE, MERCHANT_DATASET, final_table_name, 
+    __create_upstream(transaction_details, merchant_acct, CUSTOMER_TRANSACTION_TEMPLATE, MERCHANT_DATASET, final_table_name, 
                       streamed_datetime=streamed_datetime, Reverted=False, RevertedDateTime=None)
     
 def create_merchant_customer_transaction_reverted_upstream_for_merchant(transaction_details, reverted_datetime):
     partition_datetime = transaction_details.transact_datetime
         
     table_name          = CUSTOMER_TRANSACTION_TEMPLATE
     merchant_acct       = transaction_details.transact_merchant_acct
     account_code        = merchant_acct.account_code.replace('-','')
     final_table_name    = '{}_{}_{}'.format(table_name, account_code, partition_datetime.strftime('%Y%m%d'))
     
-    __create_upstream(transaction_details, CUSTOMER_TRANSACTION_TEMPLATE, MERCHANT_DATASET, final_table_name, 
+    __create_upstream(transaction_details, merchant_acct, CUSTOMER_TRANSACTION_TEMPLATE, MERCHANT_DATASET, final_table_name, 
                       streamed_datetime=reverted_datetime, Reverted=True, RevertedDateTime=reverted_datetime)    
 
 def create_merchant_customer_reward_upstream_for_merchant(transaction_details, reward_details, streamed_datetime=None):
     if streamed_datetime is None:
         streamed_datetime = datetime.utcnow()
     
     table_name          = MERCHANT_CUSTOMER_REWARD_TEMPLATE
     merchant_acct       = transaction_details.transact_merchant_acct
     account_code        = merchant_acct.account_code.replace('-','')
     final_table_name    = '{}_{}_{}'.format(table_name, account_code, streamed_datetime.strftime('%Y%m%d'))
     
     transaction_details_with_reward_details = CustomerTransactionWithRewardDetails(transaction_details, reward_details)
     
-    __create_upstream(transaction_details_with_reward_details, MERCHANT_CUSTOMER_REWARD_TEMPLATE, MERCHANT_DATASET, final_table_name, 
-                      streamed_datetime=streamed_datetime, Reverted=False, RevertedDateTime=None)
+    updated_datetime = transaction_details.transact_datetime
+    
+    __create_upstream(transaction_details_with_reward_details, merchant_acct, MERCHANT_CUSTOMER_REWARD_TEMPLATE, MERCHANT_DATASET, final_table_name, 
+                      streamed_datetime=streamed_datetime, Reverted=False, RevertedDateTime=None,
+                      UpdatedDateTime=updated_datetime,
+                      )
     
 def create_merchant_customer_prepaid_upstream_for_merchant(transaction_details, prepaid_details, streamed_datetime=None):
     if streamed_datetime is None:
         streamed_datetime = datetime.utcnow()
     
     table_name          = MERCHANT_CUSTOMER_PREPAID_TEMPLATE
     merchant_acct       = transaction_details.transact_merchant_acct
     account_code        = merchant_acct.account_code.replace('-','')
     final_table_name    = '{}_{}_{}'.format(table_name, account_code, streamed_datetime.strftime('%Y%m%d'))
     
     transaction_details_with_prepaid_details = CustomerTransactionWithPrepaidDetails(transaction_details, prepaid_details)
     
-    __create_upstream(transaction_details_with_prepaid_details, MERCHANT_CUSTOMER_PREPAID_TEMPLATE, MERCHANT_DATASET, final_table_name, 
+    __create_upstream(transaction_details_with_prepaid_details, merchant_acct, MERCHANT_CUSTOMER_PREPAID_TEMPLATE, MERCHANT_DATASET, final_table_name, 
                       streamed_datetime=streamed_datetime, Reverted=False, RevertedDateTime=None)    
     
 def create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, reward_details, reverted_datetime):
     partition_datetime = transaction_details.transact_datetime
     
     
     table_name          = MERCHANT_CUSTOMER_REWARD_TEMPLATE
     merchant_acct       = transaction_details.transact_merchant_acct
     account_code        = merchant_acct.account_code.replace('-','')
     final_table_name    = '{}_{}_{}'.format(table_name, account_code, partition_datetime.strftime('%Y%m%d'))
     
     transaction_details_with_reward_details = CustomerTransactionWithRewardDetails(transaction_details, reward_details)
     
-    __create_upstream(transaction_details_with_reward_details, MERCHANT_CUSTOMER_REWARD_TEMPLATE, MERCHANT_DATASET, final_table_name, 
-                      streamed_datetime=reverted_datetime, Reverted=True, RevertedDateTime=reverted_datetime)    
+    updated_datetime = transaction_details.reverted_datetime
+
+    __create_upstream(transaction_details_with_reward_details, merchant_acct, MERCHANT_CUSTOMER_REWARD_TEMPLATE, MERCHANT_DATASET, final_table_name, 
+                      streamed_datetime=reverted_datetime, Reverted=True, RevertedDateTime=reverted_datetime,
+                      UpdatedDateTime=updated_datetime,
+                      )    
 
 
 def create_merchant_customer_prepaid_reverted_upstream_for_merchant(transaction_details, prepaid_details, reverted_datetime):
     partition_datetime = transaction_details.transact_datetime
     
     
     table_name          = MERCHANT_CUSTOMER_PREPAID_TEMPLATE
     merchant_acct       = transaction_details.transact_merchant_acct
     account_code        = merchant_acct.account_code.replace('-','')
     final_table_name    = '{}_{}_{}'.format(table_name, account_code, partition_datetime.strftime('%Y%m%d'))
     
     transaction_details_with_prepaid_details = CustomerTransactionWithPrepaidDetails(transaction_details, prepaid_details)
     
-    __create_upstream(transaction_details_with_prepaid_details, MERCHANT_CUSTOMER_PREPAID_TEMPLATE, MERCHANT_DATASET, final_table_name, 
+    __create_upstream(transaction_details_with_prepaid_details, merchant_acct, MERCHANT_CUSTOMER_PREPAID_TEMPLATE, MERCHANT_DATASET, final_table_name, 
                       streamed_datetime=reverted_datetime, Reverted=True, RevertedDateTime=reverted_datetime) 
 
 def create_merchant_customer_redemption_upstream_for_merchant(customer_redemption, streamed_datetime=None, reverted=False, reverted_datetime=None):
     if streamed_datetime is None:
         streamed_datetime = datetime.utcnow()
     
     logger.debug('customer_redemption.merchant_acct=%s', customer_redemption.merchant_acct)
@@ -264,15 +274,21 @@
     if customer_redemption.reward_format in (program_conf.REWARD_FORMAT_POINT, program_conf.REWARD_FORMAT_STAMP, program_conf.REWARD_FORMAT_PREPAID):
         upstream_data_list.append(customer_redemption.to_upstream_info())
     
     elif customer_redemption.reward_format == program_conf.REWARD_FORMAT_VOUCHER:
         upstream_data_list.extend(customer_redemption.to_voucher_upstream_info_list())
             
     for upstream_data in upstream_data_list:
-        __create_upstream(upstream_data, MERCHANT_CUSTOMER_REDEMPTION_TEMPLATE, MERCHANT_DATASET, final_table_name, 
-                      streamed_datetime=streamed_datetime, Reverted=reverted, RevertedDateTime=reverted_datetime)
+        updated_datetime = customer_redemption.redeemed_datetime
+        if reverted:
+            updated_datetime = customer_redemption.reverted_datetime
+            
+        __create_upstream(upstream_data, merchant_acct, MERCHANT_CUSTOMER_REDEMPTION_TEMPLATE, MERCHANT_DATASET, final_table_name, 
+                      streamed_datetime=streamed_datetime, Reverted=reverted, RevertedDateTime=reverted_datetime, 
+                      UpdatedDateTime=updated_datetime
+                      )
     
-def create_merchant_customer_redemption_reverted_upstream_for_merchant(redemption_details, reverted_datetime):
+def create_merchant_customer_redemption_reverted_upstream_for_merchant(redemption_details):
     create_merchant_customer_redemption_upstream_for_merchant(redemption_details, 
                                                               streamed_datetime=redemption_details.redeemed_datetime, 
                                                               reverted=True, 
                                                               reverted_datetime=redemption_details.reverted_datetime)
```

### Comparing `trex-analytic-0.1.2/trexanalytics/conf.py` & `trex-analytic-0.1.3/trexanalytics/conf.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/bigquery/customer_query_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/bigquery/customer_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/bigquery/query_base_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/bigquery/query_base_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/bigquery/redemption_query_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/bigquery/redemption_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/bigquery/rewarding_query_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/bigquery/rewarding_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/bigquery/transaction_query_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/bigquery/transaction_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_customer_data_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_customer_data_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_data_base_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_data_base_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_merchant_data_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_merchant_data_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_transaction_data_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_transaction_data_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/importdata/import_upstream_data_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/importdata/import_upstream_data_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/main_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/main_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/controllers/template/table_template_routes.py` & `trex-analytic-0.1.3/trexanalytics/controllers/template/table_template_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-0.1.2/trexanalytics/helper/bigquery_upstream_helpers.py` & `trex-analytic-0.1.3/trexanalytics/helper/bigquery_upstream_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerStampReward, CustomerEntitledVoucher
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
-from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_reward_upstream_for_merchant
+from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_reward_upstream_for_merchant,\
+    create_merchant_customer_reward_reverted_upstream_for_merchant,\
+    create_merchant_customer_redemption_upstream_for_merchant,\
+    create_merchant_customer_redemption_reverted_upstream_for_merchant
 from trexlib.utils.string_util import is_not_empty
 import logging    
+from trexmodel.models.datastore.redeem_models import CustomerRedemption
     
     
 logger = logging.getLogger('debug')
     
 def create_transction_reward_upstream(transaction_details):        
     
     rewards_list = list_transction_reward(transaction_details)
     
     if rewards_list and is_not_empty(rewards_list):
         for r in rewards_list:
+            
             create_merchant_customer_reward_upstream_for_merchant(transaction_details, r)
             
+            if transaction_details.is_revert:
+                create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, r)
+            
 def list_transction_reward(transaction_details):
     all_rewards_list = []
             
     if isinstance(transaction_details, CustomerTransaction):
         transaction_id = transaction_details.transaction_id
         
         logger.debug('transaction_id=%s', transaction_id)
@@ -59,7 +67,14 @@
             logger.debug('rewards_list=%s', rewards_list)
             
             if rewards_list and is_not_empty(rewards_list):
                 all_rewards_list.extend(rewards_list) 
                 
     return all_rewards_list                  
         
+def create_redemption_upstream(redemption_details):        
+    
+    create_merchant_customer_redemption_upstream_for_merchant(redemption_details)
+            
+    if redemption_details.is_revert:
+        create_merchant_customer_redemption_reverted_upstream_for_merchant(redemption_details)
+
```

### Comparing `trex-analytic-0.1.2/trexanalytics/util/chart_util.py` & `trex-analytic-0.1.3/trexanalytics/util/chart_util.py`

 * *Files identical despite different names*

