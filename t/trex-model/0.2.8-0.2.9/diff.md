# Comparing `tmp/trex-model-0.2.8.tar.gz` & `tmp/trex-model-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-model-0.2.8.tar", last modified: Tue Dec 27 07:14:32 2022, max compression
+gzip compressed data, was "trex-model-0.2.9.tar", last modified: Mon Feb 13 06:21:53 2023, max compression
```

## Comparing `trex-model-0.2.8.tar` & `trex-model-0.2.9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.916858 trex-model-0.2.8/
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-0.2.8/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-0.2.8/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2022-12-27 07:14:32.917010 trex-model-0.2.8/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-0.2.8/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2022-12-27 07:14:32.917474 trex-model-0.2.8/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2022-12-27 07:02:56.000000 trex-model-0.2.8/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.888065 trex-model-0.2.8/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2022-12-27 07:14:32.000000 trex-model-0.2.8/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1754 2022-12-27 07:14:32.000000 trex-model-0.2.8/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2022-12-27 07:14:32.000000 trex-model-0.2.8/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2022-12-27 07:14:32.000000 trex-model-0.2.8/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2022-12-27 07:14:32.000000 trex-model-0.2.8/trex_model.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.890608 trex-model-0.2.8/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-0.2.8/trexmodel/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-0.2.8/trexmodel/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.892765 trex-model-0.2.8/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-0.2.8/trexmodel/models/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.914368 trex-model-0.2.8/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-0.2.8/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-0.2.8/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2978 2022-09-23 06:10:25.000000 trex-model-0.2.8/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-0.2.8/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12854 2022-12-20 04:07:21.000000 trex-model-0.2.8/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    18869 2022-12-18 09:08:16.000000 trex-model-0.2.8/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-0.2.8/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-0.2.8/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9846 2021-04-16 08:20:02.000000 trex-model-0.2.8/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    55384 2022-11-07 02:48:57.000000 trex-model-0.2.8/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-0.2.8/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16899 2021-08-19 04:14:12.000000 trex-model-0.2.8/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32132 2022-11-07 02:47:58.000000 trex-model-0.2.8/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17167 2021-10-08 09:46:15.000000 trex-model-0.2.8/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    38931 2022-09-23 07:11:28.000000 trex-model-0.2.8/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    46571 2022-03-11 05:24:52.000000 trex-model-0.2.8/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22912 2022-12-23 09:34:23.000000 trex-model-0.2.8/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    28948 2022-12-20 08:06:24.000000 trex-model-0.2.8/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-0.2.8/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-0.2.8/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-0.2.8/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-0.2.8/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    23867 2021-10-08 01:01:30.000000 trex-model-0.2.8/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-0.2.8/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15362 2022-12-14 15:17:01.000000 trex-model-0.2.8/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5924 2022-11-07 03:32:26.000000 trex-model-0.2.8/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-0.2.8/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-0.2.8/trexmodel/models/prepaid_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-0.2.8/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16051 2022-12-27 05:32:23.000000 trex-model-0.2.8/trexmodel/program_conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.915056 trex-model-0.2.8/trexmodel/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.8/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.915521 trex-model-0.2.8/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.8/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-0.2.8/trexmodel/utils/gcloud/datastore_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2022-12-27 07:14:32.916344 trex-model-0.2.8/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.8/trexmodel/utils/model/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-0.2.8/trexmodel/utils/model/model_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.669288 trex-model-0.2.9/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-0.2.9/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-0.2.9/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-02-13 06:21:53.669438 trex-model-0.2.9/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-0.2.9/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-02-13 06:21:53.670018 trex-model-0.2.9/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-02-13 06:19:24.000000 trex-model-0.2.9/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.630526 trex-model-0.2.9/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1799 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-02-13 06:21:53.000000 trex-model-0.2.9/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.632822 trex-model-0.2.9/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-0.2.9/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-0.2.9/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.635959 trex-model-0.2.9/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-0.2.9/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.664366 trex-model-0.2.9/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-0.2.9/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-0.2.9/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2978 2022-09-23 06:10:25.000000 trex-model-0.2.9/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-0.2.9/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13794 2023-02-01 14:24:54.000000 trex-model-0.2.9/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    18975 2023-01-18 15:57:20.000000 trex-model-0.2.9/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-0.2.9/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-0.2.9/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5815 2022-12-30 07:12:43.000000 trex-model-0.2.9/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9846 2021-04-16 08:20:02.000000 trex-model-0.2.9/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    55368 2023-01-31 03:16:23.000000 trex-model-0.2.9/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-0.2.9/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-0.2.9/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32092 2023-01-04 03:56:36.000000 trex-model-0.2.9/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    18586 2023-02-11 04:49:58.000000 trex-model-0.2.9/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38931 2022-09-23 07:11:28.000000 trex-model-0.2.9/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    46571 2022-03-11 05:24:52.000000 trex-model-0.2.9/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24359 2023-02-10 09:00:56.000000 trex-model-0.2.9/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    29487 2023-02-08 09:23:02.000000 trex-model-0.2.9/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-0.2.9/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-0.2.9/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-0.2.9/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-0.2.9/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    25826 2023-02-12 05:38:38.000000 trex-model-0.2.9/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-0.2.9/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-0.2.9/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6173 2023-02-07 02:42:49.000000 trex-model-0.2.9/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-0.2.9/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-0.2.9/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-0.2.9/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16152 2023-01-27 07:27:16.000000 trex-model-0.2.9/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.666310 trex-model-0.2.9/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.666924 trex-model-0.2.9/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-13 06:21:53.668277 trex-model-0.2.9/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-0.2.9/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-0.2.9/trexmodel/utils/model/model_util.py
```

### Comparing `trex-model-0.2.8/LICENSE` & `trex-model-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/setup.py` & `trex-model-0.2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='0.2.8',
+     version='0.2.9',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

### Comparing `trex-model-0.2.8/trex_model.egg-info/SOURCES.txt` & `trex-model-0.2.9/trex_model.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 trexmodel/models/datastore/admin_models.py
 trexmodel/models/datastore/analytic_models.py
 trexmodel/models/datastore/coporate_models.py
 trexmodel/models/datastore/customer_model_helpers.py
 trexmodel/models/datastore/customer_models.py
 trexmodel/models/datastore/fb_subsriber_models.py
 trexmodel/models/datastore/inventory_model.py
+trexmodel/models/datastore/loyalty_models.py
 trexmodel/models/datastore/membership_models.py
 trexmodel/models/datastore/merchant_models.py
 trexmodel/models/datastore/model_decorators.py
 trexmodel/models/datastore/ndb_models.py
 trexmodel/models/datastore/pos_models.py
 trexmodel/models/datastore/prepaid_models.py
 trexmodel/models/datastore/product_models.py
```

### Comparing `trex-model-0.2.8/trexmodel/conf.py` & `trex-model-0.2.9/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/admin_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/analytic_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/analytic_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/coporate_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-0.2.9/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,38 +157,48 @@
 
 ''' --------------- Start: Update reward summary for voucher--------------'''
 def update_customer_entiteld_voucher_summary_with_customer_new_voucher(customer_entitled_voucher_summary, customer_voucher):
     merchant_voucher        = customer_voucher.entitled_voucher_entity
     voucher_key             = merchant_voucher.key_in_str
     voucher_label           = merchant_voucher.label
     voucher_image_url       = merchant_voucher.image_public_url
+    configuration           = merchant_voucher.rebuild_configuration
     redeem_info_list        = [customer_voucher.to_redeem_info()]
     
+    logger.debug('update_customer_entiteld_voucher_summary_with_customer_new_voucher debug: voucher_key=%s', voucher_key)
+    logger.debug('update_customer_entiteld_voucher_summary_with_customer_new_voucher debug: voucher_label=%s', voucher_label)
+    
+    
     return update_customer_entiteld_voucher_summary_with_new_voucher_info(customer_entitled_voucher_summary, 
                                                                           voucher_key, 
                                                                           voucher_label, 
                                                                           voucher_image_url,
-                                                                          redeem_info_list)
+                                                                          redeem_info_list,
+                                                                          configuration,
+                                                                          )
 
 def update_customer_entiteld_voucher_summary_with_new_voucher_info(customer_entitled_voucher_summary, merchant_voucher_key, voucher_label, 
-                                                              voucher_image_url, redeem_info_list):
+                                                              voucher_image_url, redeem_info_list, configuration):
     
     if customer_entitled_voucher_summary is None:
         customer_entitled_voucher_summary = {}
         
     voucher_summary     = customer_entitled_voucher_summary.get(merchant_voucher_key)
     
     if voucher_summary:
-        customer_entitled_voucher_summary[merchant_voucher_key]['redeem_info_list'].extend(redeem_info_list)  
+        customer_entitled_voucher_summary[merchant_voucher_key]['redeem_info_list'].extend(redeem_info_list)
+        customer_entitled_voucher_summary[merchant_voucher_key]['amount'] = len(customer_entitled_voucher_summary[merchant_voucher_key]['redeem_info_list'])  
     else:
         voucher_summary = {
                             'key'               : merchant_voucher_key,
                             'label'             : voucher_label,
+                            'configuration'     : configuration,
                             'image_url'         : voucher_image_url,
-                            'redeem_info_list'  : redeem_info_list 
+                            'redeem_info_list'  : redeem_info_list,
+                            'count'             : len(redeem_info_list), 
                             
                             }
         customer_entitled_voucher_summary[merchant_voucher_key] = voucher_summary
 
     return customer_entitled_voucher_summary
 
 def update_customer_entiteld_voucher_summary_after_reverted_voucher(customer_entitled_voucher_summary, reverted_customer_voucher):
@@ -217,14 +227,16 @@
                     new_redeem_info_list.append(redeem_info)
                 
             
             if len(new_redeem_info_list) ==0:
                 del customer_entitled_voucher_summary[merchant_voucher_key]
             else:
                 customer_entitled_voucher_summary[merchant_voucher_key]['redeem_info_list'] = new_redeem_info_list
+                customer_entitled_voucher_summary[merchant_voucher_key]['count']            = len(new_redeem_info_list)
+                
     return customer_entitled_voucher_summary
     
     
 def update_customer_entiteld_voucher_summary_after_redeemed_voucher(entitled_voucher_summary, redeemed_customer_voucher):
     return update_customer_entiteld_voucher_summary_after_reverted_voucher(entitled_voucher_summary, redeemed_customer_voucher)
 
 ''' --------------- End: Update reward summary for voucher--------------'''
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/customer_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/customer_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,16 @@
                password=None):
         
         created_user = User.create(name=name, email=email, mobile_phone=mobile_phone, gender=gender, birth_date=birth_date, 
                            password=password)
         
         created_user.put()
         created_customer = cls.create_from_user(outlet, created_user)
+        created_customer.merchant_reference_code = merchant_reference_code
+        created_customer.put()
         
         return created_customer
     
     @classmethod
     def update(cls, customer=None, outlet=None, **kwargs):
         if outlet:
             customer.outlet = outlet.create_ndb_key()
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/inventory_model.py` & `trex-model-0.2.9/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/membership_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/membership_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/merchant_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/merchant_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -698,15 +698,15 @@
     
     show_dinning_table_occupied     = ndb.BooleanProperty(required=False, default=False)    
     
     fulltextsearch_field_name   = 'name'
     
     dict_properties         = ['key', 'id', 'company_name', 'business_reg_no', 'name', 'address', 'office_phone', 
                                 'fax_phone', 'email', 'business_hour', 'is_physical_store', 'assigned_catalogue_key', 'assigned_dinning_table_list',
-                                'service_charge_settings', 'assigned_tax_setup', 'show_occupied',
+                                'service_charge_settings', 'assigned_tax_setup', 
                                 'geo_location', 'created_datetime']
     
     @property
     def merchant_acct_entity(self):
         return MerchantAcct.fetch(self.key.parent().urlsafe())
     
     @property
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/model_decorators.py` & `trex-model-0.2.9/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/ndb_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/ndb_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 from google.cloud.datastore.helpers import GeoPoint
  
 logger = logging.getLogger('model') 
 
 def convert_to_serializable_value(val, none_as_empty_string=False, gmt=0, 
                                   datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
                                   date_format=lib_conf.DEFAULT_DATE_FORMAT, 
-                                  time_format=lib_conf.DEFAULT_TIME_FORMAT):
+                                  time_format=lib_conf.DEFAULT_TIME_FORMAT,
+                                  excluded_dict_properties=None
+                                  ):
     
     if isinstance(val, (list, tuple)):
         _list = []
         for item in val:
-            _list.append(convert_to_serializable_value(item))
+            _list.append(convert_to_serializable_value(item, excluded_dict_properties=excluded_dict_properties))
         value = _list
     elif isinstance(val, float):
         value = format_float(val)
     elif isinstance(val, (dict, int, bool)):
         #logger.debug('>>>>found dict, int, float, bool value=%s', val)
         value = val
     elif isinstance(val, datetime):
@@ -57,33 +59,35 @@
                 value = str(val)
     #logger.debug('convert_to_serializable_value: value=%s', value)
     return value
 
 def render_dict_value(val, full=False, show_key=True, gmt=0, 
                       datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
                       date_format=lib_conf.DEFAULT_DATE_FORMAT, 
-                      time_format=lib_conf.DEFAULT_TIME_FORMAT):
+                      time_format=lib_conf.DEFAULT_TIME_FORMAT,
+                      excluded_dict_properties=None,
+                      ):
     #logger.debug('---render_dict_value---')
     value = None
     if isinstance(val, DictModel):
-        value = val.to_dict(full=full, show_key=show_key, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format)
+        value = val.to_dict(full=full, show_key=show_key, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format, excluded_dict_properties=excluded_dict_properties)
 
     elif isinstance(val, ndb.Model):
         value = val.key.urlsafe()
 
     elif isinstance(val, (list, tuple)):
         _list = []
         for item in val:
-            _list.append(render_dict_value(item, full=full, show_key=show_key, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format))
+            _list.append(render_dict_value(item, full=full, show_key=show_key, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format, excluded_dict_properties=excluded_dict_properties))
         value = _list
 
     elif isinstance(val, DictObject):
-        value = val.to_dict(gmt=gmt)
+        value = val.to_dict(gmt=gmt, excluded_dict_properties=excluded_dict_properties)
     else:
-        value = convert_to_serializable_value(val, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format)
+        value = convert_to_serializable_value(val, gmt=gmt, date_format=date_format, datetime_format=datetime_format, time_format=time_format, excluded_dict_properties=excluded_dict_properties)
     return value
 
 class DictObject(object):
     dict_properties = None
     
     def get_class_members(self, klass):
         ret = dir(klass)
@@ -94,15 +98,15 @@
     
     def uniq(self, seq ): 
         return list(set(seq))
     
     def properties(self):
         return self.__dict__
 
-    def to_dict(self, full=True, show_key=True, dict_properties=None, gmt=lib_conf.DEFAULT_GMT, 
+    def to_dict(self, full=True, show_key=True, dict_properties=None, excluded_dict_properties=None, gmt=lib_conf.DEFAULT_GMT, 
                         datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
                         date_format=lib_conf.DEFAULT_DATE_FORMAT, 
                         time_format=lib_conf.DEFAULT_TIME_FORMAT):
         logger.info('calling DictObject.to_dict')
         result = {}
         #logger.debug('properties = %s, object = %s', self.properties(), self)
 
@@ -113,15 +117,17 @@
 
                 val = getattr(self, p)
                 if val is not None:
                     #logger.debug('attribute=%s', p)
                     result[p] = render_dict_value(val, full=full, show_key=show_key, gmt=gmt, 
                                                   datetime_format=datetime_format, 
                                                   date_format=datetime_format, 
-                                                  time_format=time_format)
+                                                  time_format=time_format,
+                                                  excluded_dict_properties=excluded_dict_properties,
+                                                  )
         return result
     
 class DictModel(ndb.Model):
     
     dict_properties             = None
     dict_full_properties        = None
     show_key_in_dict            = True
@@ -132,15 +138,15 @@
             return '%s,%s' % (val.latitude, val.longitude)
         
         return val
 
     def put(self, **kwargs):
         super(DictModel, self).put(**kwargs)
 
-    def to_dict(self, full=False, show_key=True, dict_properties=None, gmt=lib_conf.DEFAULT_GMT, 
+    def to_dict(self, full=False, show_key=True, dict_properties=None, excluded_dict_properties=None, gmt=lib_conf.DEFAULT_GMT, 
                         datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
                         date_format=lib_conf.DEFAULT_DATE_FORMAT, 
                         time_format=lib_conf.DEFAULT_TIME_FORMAT):
         result = {}
         logger.debug('DictModel: full=%s', full)
         logger.debug('DictModel: show_key=%s', show_key)
         
@@ -154,14 +160,18 @@
         _dict_properties = dict_properties or self.dict_properties
 
         if full and self.dict_full_properties:
             _dict_properties = self.dict_full_properties
 
         if _dict_properties:
             for p in _dict_properties:
+                if excluded_dict_properties is not None:
+                    if p in excluded_dict_properties:
+                        continue
+                    
                 if p=='key':
                     if result.get('key'):
                         continue
                     
                 _p = p.split('.')
 
                 if len(_p)>1:
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/pos_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/pos_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,39 +15,39 @@
 logger = logging.getLogger('debug')
 
 
 class POSSetting(BaseNModel,DictModel):
     '''
     merchant_acct as ancestor
     '''
-    pos_name                = ndb.StringProperty(required=True)
+    device_name             = ndb.StringProperty(required=True)
     activation_code         = ndb.StringProperty(required=True)
     device_id               = ndb.StringProperty(required=False)
     activated               = ndb.BooleanProperty(required=True, default=False)
     assigned_outlet         = ndb.KeyProperty(name="assigned_outlet", kind=Outlet)
     #assigned_catalogue      = ndb.KeyProperty(name="assigned_outlet", kind=ProductCatalogue)
     created_datetime        = ndb.DateTimeProperty(required=True, auto_now_add=True)
     activated_datetime      = ndb.DateTimeProperty(required=False)
     
-    dict_properties = ['pos_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 'activated_datetime', 'created_datetime']
+    dict_properties = ['device_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 'activated_datetime', 'created_datetime']
     
     @property
     def assigned_outlet_key(self):
         return self.assigned_outlet.urlsafe().decode('utf-8')
     
     @property
     def assigned_outlet_entity(self):
         return Outlet.fetch(self.assigned_outlet_key)
     
     @property
     def merchant_acct_entity(self):
         return self.assigned_outlet_entity.merchant_acct_entity
     
     @staticmethod
-    def create(pos_name, merchant_acct, assign_outlet):
+    def create(device_name, merchant_acct, assign_outlet):
         activation_code = random_number(16)
         checking_activation_pos_setting = POSSetting.get_by_activation_code(activation_code)
         regenerate_activation_code = False
         
         if checking_activation_pos_setting:
             regenerate_activation_code = True
         
@@ -56,29 +56,29 @@
             checking_activation_pos_setting = POSSetting.get_by_activation_code(activation_code)
             if checking_activation_pos_setting==None:
                 regenerate_activation_code = False
             
         
         pos_setting = POSSetting(
                                 parent                  = merchant_acct.create_ndb_key(),
-                                pos_name                = pos_name,
+                                device_name             = device_name,
                                 activation_code         = activation_code,
                                 assigned_outlet         = assign_outlet.create_ndb_key(),
                                 
                                 )
         
         pos_setting.put()
         return pos_setting
     
     @staticmethod
-    def update(pos_setting_key, pos_name, assigned_outlet, device_id):
+    def update(pos_setting_key, device_name, assigned_outlet):
         pos_setting                         = POSSetting.fetch(pos_setting_key)
-        pos_setting.pos_name                = pos_name
+        pos_setting.device_name             = device_name
         pos_setting.assigned_outlet         = assigned_outlet.create_ndb_key()
-        pos_setting.device_id               = device_id
+        
         pos_setting.put()
         
         return pos_setting
     
     @staticmethod
     def get_by_activation_code(activation_code):
         pos_setting = POSSetting.query(POSSetting.activation_code ==activation_code).get()
@@ -200,15 +200,15 @@
                         'phone'                      : outlet.office_phone,
                         'website'                    : merchant_acct.website or '',  
                         'outlet_name'                : outlet.name,    
                         }
         
         return {
                 'activation_code'                   : self.activation_code,
-                'pos_name'                          : self.pos_name,
+                'device_name'                       : self.device_name,
                 'company_name'                      : merchant_acct.company_name,
                 'website'                           : merchant_acct.website,
                 'account_id'                        : self.parent_key,
                 'api_key'                           : merchant_acct.api_key,
                 'logo_image_url'                    : merchant_acct.logo_public_url,
                 'account_settings'                  : account_settings,
                 'outlet_details'                    : outlet_details,
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/prepaid_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/prepaid_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from trexmodel import conf, program_conf
 from trexlib.utils.string_util import random_string
 from datetime import datetime, timedelta
 import trexmodel.conf as model_conf
 from trexlib.utils.common.common_util import sort_dict_list
 from trexmodel.utils.model.model_util import generate_transaction_id
 
-logger = logging.getLogger('model')
+logger = logging.getLogger('debug')
 
 class PrepaidSettings(BaseNModel,DictModel):
     '''
     Merchant acct as ancestor
     '''
     label                               = ndb.StringProperty(required=True)
     
@@ -91,29 +91,33 @@
                                                 }
         if self.is_lump_sum_prepaid:
             prepaid_program_configuration['lump_sum_settings'] = self.lump_sum_settings
         
         if self.is_multi_tier_prepaid:
             prepaid_program_configuration['multitier_settings'] = self.multitier_settings
         
+        logger.debug('prepaid_program_configuration=%s', prepaid_program_configuration)
+        
         return prepaid_program_configuration
     
     @staticmethod
     def list_by_merchant_acct(merchant_acct):
         result = PrepaidSettings.query(ancestor=merchant_acct.create_ndb_key()).fetch(limit=conf.MAX_FETCH_RECORD)
         not_archive_program_list = []
         for r in result:
             if r.archived != True:
                 not_archive_program_list.append(r)
         return not_archive_program_list
     
-    def __update_merchant_account_prepaid_configuration(self):
+    def update_merchant_account_prepaid_configuration(self):
         merchant_acct = self.merchant_acct_entity    
         merchant_acct.update_prepaid_program(self.to_configuration())
         merchant_acct.put()
+        
+        
     
     @staticmethod
     def create(merchant_acct, label, start_date, end_date, is_multi_tier_prepaid=False, is_lump_sum_prepaid=True, lump_sum_settings=None, multitier_settings=None, created_by=None):
         prepaid_settings = PrepaidSettings(
                                 parent                  = merchant_acct.create_ndb_key(),
                                 label                   = label,
                                 start_date              = start_date,
@@ -127,15 +131,15 @@
                                 created_by              = created_by.create_ndb_key(),
                                 created_by_username     = created_by.username,
                                 )
         
         prepaid_settings.put()
         
         if prepaid_settings.enable:
-            prepaid_settings.__update_merchant_account_prepaid_configuration()
+            prepaid_settings.update_merchant_account_prepaid_configuration()
         
         return prepaid_settings
         
     @staticmethod
     def update(prepaid_settings, label, start_date, end_date, is_multi_tier_prepaid=False, is_lump_sum_prepaid=True, lump_sum_settings=None, multitier_settings=None, modified_by=None):
         
         prepaid_settings.label                  = label
@@ -146,25 +150,25 @@
         prepaid_settings.lump_sum_settings      = lump_sum_settings
         prepaid_settings.multitier_settings     = multitier_settings
         prepaid_settings.modified_by            = modified_by.create_ndb_key()
         prepaid_settings.modified_by_username   = modified_by.username
         prepaid_settings.put()    
     
         if prepaid_settings.enable:
-            prepaid_settings.__update_merchant_account_prepaid_configuration()
+            prepaid_settings.update_merchant_account_prepaid_configuration()
     
     
         return prepaid_settings
     
     @staticmethod
     def enable(prepaid_settings):
         prepaid_settings.enabled = True
         prepaid_settings.put()
         
-        prepaid_settings.__update_merchant_account_prepaid_configuration()
+        prepaid_settings.update_merchant_account_prepaid_configuration()
         
     @staticmethod
     def disable(prepaid_settings):
         prepaid_settings.enabled = False
         prepaid_settings.put() 
         
         merchant_acct = prepaid_settings.merchant_acct_entity    
@@ -214,14 +218,18 @@
         return self.status == program_conf.REWARD_STATUS_VALID
     
     @property
     def is_redeemed(self):
         return self.status == program_conf.REWARD_STATUS_REDEEMED
     
     @property
+    def is_used(self):
+        return self.used_prepaid_amount>0
+    
+    @property
     def prepaid_balance(self):
         return self.prepaid_amount - self.used_prepaid_amount
     
     def update_used_reward_amount(self, used_prepaid_amount):
         self.used_prepaid_amount    += used_prepaid_amount
         prepaid_balance              = self.prepaid_balance
         
@@ -248,14 +256,31 @@
         prepaid_summary =  {
                             'amount'            : self.prepaid_amount,
                             'used_amount'       : self.used_prepaid_amount,    
                             }
         
         return prepaid_summary
     
+    @property
+    def is_reach_reward_limit(self):
+        return self.status == program_conf.REWARD_STATUS_REACH_LIMIT
+    
+    @property
+    def reward_balance(self):
+        return self.prepaid_amount - self.used_prepaid_amount
+    
+    @classmethod
+    def list_by_valid_with_cursor(cls, customer, limit=50, start_cursor=None):
+        query = cls.query(ndb.AND(cls.status==program_conf.REWARD_STATUS_VALID
+            ), ancestor=customer.create_ndb_key()).order(cls.topup_datetime)
+            
+        (result, next_cursor) = cls.list_all_with_condition_query(query, start_cursor=start_cursor, return_with_cursor=True, limit=limit)
+        
+        return (result, next_cursor) 
+    
     @staticmethod
     def list_by_customer(customer, status=program_conf.REWARD_STATUS_VALID, limit = conf.MAX_FETCH_RECORD):
         return CustomerPrepaidReward.query(ndb.AND(CustomerPrepaidReward.status==status), ancestor=customer.create_ndb_key()).fetch(limit=limit)
     
     @staticmethod
     def list_all_by_customer(customer, limit = conf.MAX_FETCH_RECORD):
         return CustomerPrepaidReward.query(ancestor=customer.create_ndb_key()).fetch(limit=limit)
@@ -276,53 +301,64 @@
         
         sorted_tier_scheme      = None
         
         prepaid_scheme_details  = {
                                     'program_key'   : prepaid_program.key_in_str
                                     }
         
-        prepaid_scheme      = None
+        tier_prepaid_scheme      = None
+        found_match_scheme       = None
+        
+        logger.debug('is_multi_tier_prepaid=%s', is_multi_tier_prepaid)
         
         if is_multi_tier_prepaid:
             sorted_tier_scheme = sort_dict_list(prepaid_program.multitier_settings.values(), 'min_topup_amount')
             
             logger.debug('Get topup scheme from topup amount(%s)', topup_amount)
             
+            #look for higheest min topup amount scheme
             for scheme in sorted_tier_scheme:
                 if topup_amount>= scheme.get('min_topup_amount'):
-                    prepaid_scheme = {
+                    tier_prepaid_scheme = {
                                             'topup_amount'  : scheme.get('topup_amount'),
                                             'prepaid_amount': scheme.get('prepaid_amount'),
                                             'prepaid_rate'  : scheme.get('prepaid_amount')/scheme.get('topup_amount'),
                                             'scheme_type'   : 'tier',
                                             }
                     logger.debug('Found topup scheme for min topup amount(%s)', scheme.get('min_topup_amount'))
         
-        logger.debug('prepaid_scheme=%s', prepaid_scheme)
+        logger.debug('tier_prepaid_scheme=%s', tier_prepaid_scheme)
         
         #if topup amount is less than smallest prepaid tier minimum topup amount, thus goto lump sum scheme    
-        if prepaid_scheme is None and is_lump_sum_prepaid:
+        if tier_prepaid_scheme is None and is_lump_sum_prepaid:
+            logger.debug('going to create scheme from lump sum setting')
+            prepaid_scheme = prepaid_program.lump_sum_settings
             found_match_scheme = {
-                                            'topup_amount'  : scheme.get('topup_amount'),
-                                            'prepaid_amount': scheme.get('prepaid_amount'),
-                                            'prepaid_rate'  : scheme.get('prepaid_amount')/scheme.get('topup_amount'),
+                                            'topup_amount'  : prepaid_scheme.get('topup_amount'),
+                                            'prepaid_amount': prepaid_scheme.get('prepaid_amount'),
+                                            'prepaid_rate'  : prepaid_scheme.get('prepaid_amount')/prepaid_scheme.get('topup_amount'),
                                             'scheme_type'   : 'lump_sum',
                                             }  
         
-        if prepaid_scheme is None:
-            prepaid_scheme = {
+        else:
+            found_match_scheme = tier_prepaid_scheme
+             
+        if found_match_scheme is None:
+            logger.debug('going to create scheme default scheme')
+            
+            found_match_scheme = {
                                             'topup_amount'  : 1,
                                             'prepaid_amount': 1,
                                             'prepaid_rate'  : 1,
                                             'scheme_type'   : 'auto',
                                             }
             
-            logger.debug('create default prepaid_scheme=%s', prepaid_scheme)
+        logger.debug('create found_match_scheme=%s', found_match_scheme)
         
-        prepaid_scheme_details.update(prepaid_scheme)
+        prepaid_scheme_details.update(found_match_scheme)
         
         logger.debug('prepaid_scheme_details=%s', prepaid_scheme_details)
             
         topup_unit          = CustomerPrepaidReward.__calculate_topup_unit(topup_amount, prepaid_scheme_details)
         prepaid_amount      = CustomerPrepaidReward.__calculate_prepaid_amount(topup_unit, prepaid_scheme_details)
         topup_prepaid_rate  = CustomerPrepaidReward.__calculate_topup_prepaid_rate(prepaid_scheme_details)
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/product_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/product_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/program_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/program_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/redeem_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/redeem_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from datetime import datetime, timedelta
 from trexmodel.utils.model.model_util import generate_transaction_id
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerStampReward, CustomerEntitledVoucher
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
+from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 
 
 logger = logging.getLogger('model')
 
 
 class CustomerRedeemedItemUpstream(DictModel):
     
@@ -159,14 +160,15 @@
         return CustomerRedemption.count_with_condition_query(query, limit=limit)
     
     @staticmethod
     def create(customer, reward_format, redeemed_amount, redeemed_outlet, transaction_id=None, 
                redeemed_voucher_keys_list=None, invoice_id=None, remarks=None, redeemed_by=None, redeemed_datetime=None):
         
         reward_summary              = customer.reward_summary
+        prepaid_summary             = customer.prepaid_summary
         entitled_voucher_summary    = customer.entitled_voucher_summary
         
         if is_not_empty(redeemed_by):
             if isinstance(redeemed_by, MerchantUser):
                 redeemed_by_username = redeemed_by.username
 
         
@@ -251,14 +253,39 @@
                                 }
                 
             reward_balance = reward_summary[reward_format]['amount'] - redeemed_amount
             if reward_balance<0:
                 reward_balance = 0
                 
             reward_summary[reward_format]['amount'] = reward_balance
+            
+        elif reward_format == program_conf.REWARD_FORMAT_PREPAID:
+            total_redeemed_amount   = redeemed_amount
+            cursor                  = None
+            redeemed_items_list     = [] 
+            
+            while total_redeemed_amount>0:
+                (total_redeemed_amount, cursor, __redeemed_items_list) = __start_redeem(customer, total_redeemed_amount, cursor, 
+                                                                                        CustomerPrepaidReward)
+                redeemed_items_list.extend(__redeemed_items_list)
+            
+            redeemed_summary = {
+                                reward_format               : {
+                                    
+                                                                'amount'                    : redeemed_amount,        
+                                                                'customer_prepaid'          : redeemed_items_list
+                                                                }
+                                }
+            
+                
+            reward_balance = prepaid_summary['amount'] - redeemed_amount
+            if reward_balance<0:
+                reward_balance = 0
+                
+            prepaid_summary['amount'] = reward_balance    
                                 
             
         elif reward_format == program_conf.REWARD_FORMAT_VOUCHER:
             
             redemption_details = {
                                 'vouchers': {}
                                 }
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/reward_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/reward_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from trexmodel import conf, program_conf
 from trexlib.utils.string_util import random_string
 from datetime import datetime, timedelta
 from trexmodel.utils.model.model_util import generate_transaction_id,\
     string_to_key_property 
 from six import string_types
 from flask_babel import gettext
+from trexmodel.models.datastore.customer_models import Customer
 
 logger = logging.getLogger('model')
 
 
 class RewardEntitlement(BaseNModel, DictModel):
     effective_date              = ndb.DateProperty(required=True)
     expiry_date                 = ndb.DateProperty(required=True)
@@ -301,14 +302,28 @@
         if redeemed_datetime is None:
             redeemed_datetime = datetime.now()
         
         self.redeemed_datetime      = redeemed_datetime
         self.redeemed_by            = redeemed_by.create_ndb_key()
         self.redeemed_by_username   = redeemed_by.username
         self.put()
+    
+    def remove(self, removed_by, removed_datetime=None):
+        self.status = program_conf.REWARD_STATUS_REMOVED   
+        
+        if removed_datetime is None:
+            removed_datetime = datetime.now()
+        
+        self.removed_datetime      = removed_datetime
+        self.removed_by_username   = removed_by.username
+        self.put() 
+      
+    @property
+    def entitled_customer_entity(self):
+        return Customer.fetch(self.key.parent().urlsafe()) 
         
     @property
     def is_used(self):
         return self.status == program_conf.REWARD_STATUS_REDEEMED
     
     @property
     def is_reverted(self):
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-0.2.9/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/system_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/task_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/test_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/transaction_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/transaction_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     created_datetime            = ndb.DateTimeProperty(required=True, auto_now=True)
     
     transact_timestamp          = ndb.FloatProperty(required=False)
     
     transaction_id              = ndb.StringProperty(required=True)
     invoice_id                  = ndb.StringProperty(required=False)
     remarks                     = ndb.StringProperty(required=False)
+    system_remarks              = ndb.StringProperty(required=False)
     
     tax_amount                  = ndb.FloatProperty(required=False, default=.0)
     transact_amount             = ndb.FloatProperty(required=True)
     
     transact_by                 = ndb.KeyProperty(name="created_by", kind=MerchantUser)
     transact_by_username        = ndb.StringProperty(required=False)
     
@@ -65,19 +66,19 @@
     reverted_by                 = ndb.KeyProperty(name="reverted_by", kind=MerchantUser)
     reverted_by_username        = ndb.StringProperty(required=False)
     
     is_reward_redeemed          = ndb.BooleanProperty(required=False, default=False)
     
     is_sales_transaction        = ndb.BooleanProperty(required=False, default=True)
     
-    dict_properties         = ['transaction_id', 'invoice_id', 'remarks', 'tax_amount', 'transact_amount', 'reward_giveaway_method',
+    dict_properties         = ['transaction_id', 'invoice_id', 'remarks', 'system_remarks', 'tax_amount', 'transact_amount', 'reward_giveaway_method',
                                'entitled_reward_summary', 'entitled_voucher_summary', 'entitled_prepaid_summary', 
                                'transact_customer_acct', 'transact_outlet_details', 'transact_merchant_acct',
                                'transact_datetime', 'created_datetime',  'transact_outlet_key', 'is_revert', 'reverted_datetime',
-                               'transact_by_username', 'is_reward_redeemed', 'is_sales_transaction', 'allow_to_revert',
+                               'transact_by', 'transact_by_username', 'is_reward_redeemed', 'is_sales_transaction', 'allow_to_revert',
                                ]
     
     def to_transaction_details_json(self):
         pass
     
     @property
     def transact_customer_acct(self):
@@ -129,22 +130,22 @@
         if transaction_id:
             customer_transaction = CustomerTransaction.get_by_transaction_id(transaction_id)
             if customer_transaction:
                 customer_transaction.is_reward_redeemed = True
                 customer_transaction.put()
     
     @staticmethod
-    def create_manual_transaction(customer, remarks=None, transact_outlet=None, transact_by=None, transact_datetime=None, is_sales_transaction=False, allow_to_revert=True): 
-        return CustomerTransaction.create_system_transaction(customer, remarks=remarks, transact_outlet=transact_outlet, transact_by=transact_by, 
+    def create_manual_transaction(customer, remarks=None, system_remarks=None, transact_outlet=None, transact_by=None, transact_datetime=None, is_sales_transaction=False, allow_to_revert=True): 
+        return CustomerTransaction.create_system_transaction(customer, remarks=remarks, system_remarks=system_remarks, transact_outlet=transact_outlet, transact_by=transact_by, 
                                    transact_datetime=transact_datetime, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL,
                                    is_sales_transaction = is_sales_transaction, allow_to_revert=allow_to_revert,
                                    )
     
     @staticmethod
-    def create_system_transaction(customer, transact_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, 
+    def create_system_transaction(customer, transact_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, system_remarks=None,
                transact_outlet=None, transact_by=None, transact_datetime=None, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM,
                is_sales_transaction = False, allow_to_revert=True
                ):
         
         transact_by_username = None
         
         if is_not_empty(transact_by):
@@ -159,27 +160,29 @@
         
         logger.debug('generated transaction_id=%s', transaction_id)
         logger.debug('invoice_id=%s', invoice_id)
         logger.debug('tax_amount=%s', tax_amount)
         logger.debug('transact_amount=%s', transact_amount)
         logger.debug('transact_datetime=%s', transact_datetime)
         logger.debug('transact_by_username=%s', transact_by_username)
+        logger.debug('system_remarks=%s', system_remarks)
         
         customer_transaction = CustomerTransaction(
                                                     parent                  = customer.create_ndb_key(),
                                                     
                                                     transact_merchant       = customer.registered_merchant_acct.create_ndb_key(),
                                                     transact_outlet         = transact_outlet.create_ndb_key() if transact_outlet else None,
                                                     
                                                     tax_amount              = tax_amount,
                                                     transact_amount         = transact_amount,
                                                     
                                                     transaction_id          = transaction_id,
                                                     invoice_id              = invoice_id,
                                                     remarks                 = remarks,
+                                                    system_remarks          = system_remarks,
                                                     
                                                     transact_by             = transact_by.create_ndb_key() if transact_by else None,
                                                     transact_by_username    = transact_by_username,
                                                     
                                                     transact_datetime       = transact_datetime,
                                                     reward_giveaway_method  = reward_giveaway_method,
                                                     
@@ -271,34 +274,67 @@
                     p.reverted_by_username          = reverted_by.username
                     p.put()
                     
                     entitled_voucher_summary = update_customer_entiteld_voucher_summary_after_reverted_voucher(entitled_voucher_summary, p)
             
             updated_voucher_summary = {}
             
-            for voucher_key, count in entitled_voucher_summary.items():
-                if count>0:
-                    updated_voucher_summary[voucher_key] = count
+            logger.debug('revert transaction debug: entitled_voucher_summary=%s', entitled_voucher_summary)
+            
+            for voucher_key, details in entitled_voucher_summary.items():
+                if len(details.get('redeem_info_list'))>0:
+                    updated_voucher_summary[voucher_key] = details
                 
             customer_acct.reward_summary            = customer_reward_summary
             customer_acct.entitled_voucher_summary  = updated_voucher_summary or {}
             customer_acct.put()
             
             return True
         
         else:
             raise Exception(gettext('Transaction reward have been used'))
     
     @staticmethod
-    def list_customer_transaction(customer_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False):
-        query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(-CustomerTransaction.transact_datetime)
+    def list_customer_transaction(customer_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
+        if reverse_order:
+            query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(-CustomerTransaction.transact_datetime)
+        else:
+            query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(CustomerTransaction.transact_datetime)
         
         return CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
     
     @staticmethod
+    def list_valid_customer_transaction(customer_acct, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False, reverse_order=True):
+        if reverse_order:
+            query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(-CustomerTransaction.transact_datetime)
+        else:
+            query = CustomerTransaction.query(ancestor = customer_acct.create_ndb_key()).order(CustomerTransaction.transact_datetime)
+        
+        result                  = None
+        next_cursor             = None
+        valid_transaction_list  = []
+        
+        if return_with_cursor:
+            (result, next_cursor) = CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+        else:
+            result =  CustomerTransaction.list_all_with_condition_query(query, offset=offset, limit=limit, start_cursor=start_cursor, return_with_cursor=return_with_cursor)
+        
+        
+        if result:
+            for r in result:
+                if r.is_revert==False:
+                    valid_transaction_list.append(r)
+        
+        if return_with_cursor:
+            return (valid_transaction_list, next_cursor)
+        else:
+            return valid_transaction_list
+            
+    
+    @staticmethod
     def list_customer_transaction_by_transact_timestamp(customer_acct, transact_timestamp_from=None, transact_timestamp_to=None):
         return CustomerTransaction.query(ndb.AND(
                                                     CustomerTransaction.transact_timestamp>transact_timestamp_from,
                                                     CustomerTransaction.transact_timestamp<=transact_timestamp_to
                                                   ),ancestor = customer_acct.create_ndb_key()).fetch(limit=conf.MAX_FETCH_RECORD)
         
     @staticmethod
@@ -434,15 +470,14 @@
         self.transact_datetime              = transaction_details.transact_datetime
         self.transaction_id                 = transaction_details.transaction_id
         self.transact_amount                = transaction_details.transact_amount
         self.is_revert                      = transaction_details.is_revert
         self.reverted_datetime              = transaction_details.reverted_datetime
         self.topup_amount                   = prepaid_details.topup_amount
         self.prepaid_amount                 = prepaid_details.prepaid_amount
-        self.expiry_date                    = prepaid_details.expiry_date
         self.topup_datetime                 = prepaid_details.topup_datetime
```

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/user_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/user_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-0.2.8/trexmodel/models/datastore/voucher_models.py` & `trex-model-0.2.9/trexmodel/models/datastore/voucher_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.merchant_models import MerchantAcct, \
     MerchantUser
 import logging
 from trexmodel import program_conf
 from datetime import datetime
 from trexmodel.program_conf import VOUCHER_REWARD_TYPE,\
+    VOUCHER_REWARD_MAX_QUANTITY,\
     VOUCHER_REWARD_PRICE, VOUCHER_REWARD_BRAND,\
     VOUCHER_REWARD_MIN_SALES_AMOUNT,\
     VOUCHER_REWARD_DISCOUNT_RATE,\
     VOUCHER_REWARD_TYPE_DISCOUNT,\
     VOUCHER_REWARD_PRODUCT_SKU,\
     VOUCHER_REWARD_PRODUCT_CATEGORY, VOUCHER_REWARD_CASH,\
     VOUCHER_REWARD_TYPE_CASH,\
@@ -61,101 +62,131 @@
     def is_published(self):
         return self.completed_status == program_conf.VOUCHER_STATUS_PUBLISH
     
 class MerchantVoucher(VoucherBase):
     
     dict_properties         = ['label', 'voucher_type', 'desc', 'terms_and_conditions', 'configuration', 'created_datetime', 'modified_datetime', 'completed_status', 
                                'created_by_username', 'modified_by_username', 'is_published', 'is_archived',  
-                               'image_public_url','image_storage_filename',
+                               'image_public_url','image_storage_filename', 
                                'cash_amount', 'discount_rate', 'product_category', 'product_sku', 'min_sales_amount', 'applicable_product_category', 
-                               'applicable_product_brand', 'product_price',
+                               'applicable_product_brand', 'product_price', 'max_quantity',
                                ]
     
     @property
     def cash_amount(self):
-        if self.configuration:
+        if self.configuration and VOUCHER_REWARD_CASH in self.configuration[VOUCHER_REWARD_ACTION_DATA].keys():
             if VOUCHER_REWARD_TYPE_CASH == self.configuration[VOUCHER_REWARD_TYPE]:
                 return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_CASH]
-                
+        else:
+            return .0        
     @property
     def discount_rate(self):
         if self.configuration:
-            if VOUCHER_REWARD_TYPE_DISCOUNT == self.configuration[VOUCHER_REWARD_TYPE]:
-                return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_DISCOUNT_RATE]            
+            if VOUCHER_REWARD_TYPE_DISCOUNT == self.configuration[VOUCHER_REWARD_TYPE] and VOUCHER_REWARD_DISCOUNT_RATE in self.configuration[VOUCHER_REWARD_ACTION_DATA].keys():
+                return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_DISCOUNT_RATE]
+        
+        return .0             
     
     @property
     def product_category(self):
-        if self.configuration:
+        if self.configuration and VOUCHER_REWARD_PRODUCT_CATEGORY in self.configuration[VOUCHER_REWARD_ACTION_DATA].keys():
             if VOUCHER_REWARD_TYPE_PRODUCT == self.configuration[VOUCHER_REWARD_TYPE]:
                 return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_PRODUCT_CATEGORY]
             
     @property
     def product_sku(self):
-        if self.configuration:
+        if self.configuration and VOUCHER_REWARD_PRODUCT_SKU in self.configuration[VOUCHER_REWARD_ACTION_DATA].keys():
             if VOUCHER_REWARD_TYPE_PRODUCT == self.configuration[VOUCHER_REWARD_TYPE]:
                 return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_PRODUCT_SKU]                    
             
     
     @property
     def min_sales_amount(self):
-        if self.configuration:
+        if self.configuration and VOUCHER_REWARD_MIN_SALES_AMOUNT in self.configuration[VOUCHER_REWARD_ACTION_DATA].keys():
             return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_MIN_SALES_AMOUNT]
+        else:
+            return .0
+        
+    @property
+    def max_quantity(self):
+        if self.configuration and VOUCHER_REWARD_MAX_QUANTITY in self.configuration[VOUCHER_REWARD_ACTION_DATA].keys():
+            return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_MAX_QUANTITY]    
+        else:
+            return 1
         
     @property
     def product_price(self):
         if self.configuration:
-            if VOUCHER_REWARD_TYPE_PRODUCT == self.configuration[VOUCHER_REWARD_TYPE]:
+            if VOUCHER_REWARD_TYPE_PRODUCT == self.configuration[VOUCHER_REWARD_TYPE] and VOUCHER_REWARD_PRICE in self.configuration[VOUCHER_REWARD_ACTION_DATA].keys():
                 return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_PRICE]    
+            
+        return .0        
         
     @property
     def applicable_product_category(self):
         if self.configuration:
             return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_PRODUCT_CATEGORY]
         
     @property
     def applicable_product_brand(self):
         if self.configuration:
             return self.configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_BRAND]        
     
+    @property
+    def rebuild_configuration(self):
+        new_configuration = self.configuration
+        if new_configuration:
+            if VOUCHER_REWARD_TYPE_DISCOUNT == new_configuration[VOUCHER_REWARD_TYPE]:
+                new_configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_MAX_QUANTITY] = 1
+            elif VOUCHER_REWARD_TYPE_CASH == new_configuration[VOUCHER_REWARD_TYPE]:
+                new_configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_MAX_QUANTITY] = self.max_quantity
+            elif VOUCHER_REWARD_TYPE_PRODUCT == new_configuration[VOUCHER_REWARD_TYPE]:
+                new_configuration[VOUCHER_REWARD_ACTION_DATA][VOUCHER_REWARD_MAX_QUANTITY] = self.max_quantity
+        
+        return new_configuration
+    
     @staticmethod
-    def construct_cash_voucher_configuration(amount, category=None, brand=None, min_sales_amount=.0):
+    def construct_cash_voucher_configuration(amount, category=None, brand=None, min_sales_amount=.0, max_quantity=1):
         return {
                 VOUCHER_REWARD_TYPE         : VOUCHER_REWARD_TYPE_CASH,
                 VOUCHER_REWARD_ACTION_DATA  : {
                                                 VOUCHER_REWARD_CASH             : amount,
                                                 VOUCHER_REWARD_MIN_SALES_AMOUNT : min_sales_amount,
                                                 VOUCHER_REWARD_PRODUCT_CATEGORY : category,
                                                 VOUCHER_REWARD_BRAND            : brand,
+                                                VOUCHER_REWARD_MAX_QUANTITY     : max_quantity,    
                                                 },
                 }
     
     @staticmethod
     def construct_discount_voucher_configuration(discount_rate, category=None, brand=None, min_sales_amount=.0):
         return {
                 VOUCHER_REWARD_TYPE         : VOUCHER_REWARD_TYPE_DISCOUNT,
                 VOUCHER_REWARD_ACTION_DATA  : {
                                                 
                                                 VOUCHER_REWARD_DISCOUNT_RATE    : discount_rate,
                                                 VOUCHER_REWARD_MIN_SALES_AMOUNT : min_sales_amount,
                                                 VOUCHER_REWARD_PRODUCT_CATEGORY : category,
-                                                VOUCHER_REWARD_BRAND            : brand,    
+                                                VOUCHER_REWARD_BRAND            : brand, 
+                                                VOUCHER_REWARD_MAX_QUANTITY     : 1,    
                                                 },
                 }
         
     @staticmethod
-    def construct_product_voucher_configuration(product_sku, category=None, brand=None, min_sales_amount=.0, price=.0):
+    def construct_product_voucher_configuration(product_sku, category=None, brand=None, min_sales_amount=.0, price=.0, max_quantity=1):
         return {
                 VOUCHER_REWARD_TYPE         : VOUCHER_REWARD_TYPE_PRODUCT,
                 VOUCHER_REWARD_ACTION_DATA  : {
                                                 
                                                 VOUCHER_REWARD_PRODUCT_SKU      : product_sku,
                                                 VOUCHER_REWARD_MIN_SALES_AMOUNT : min_sales_amount,
                                                 VOUCHER_REWARD_PRODUCT_CATEGORY : category,
                                                 VOUCHER_REWARD_BRAND            : brand,
-                                                VOUCHER_REWARD_PRICE            : price,       
+                                                VOUCHER_REWARD_PRICE            : price,  
+                                                VOUCHER_REWARD_MAX_QUANTITY     : max_quantity,     
                                                 },
                 }    
     
     @property
     def merchant_acct(self):
         return MerchantAcct.fetch(self.key.parent().urlsafe())
```

### Comparing `trex-model-0.2.8/trexmodel/models/merchant_helpers.py` & `trex-model-0.2.9/trexmodel/models/merchant_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from trexmodel.models.datastore.pos_models import InvoiceNoGeneration,\
     RoundingSetup, DinningOption, PosPaymentMethod
 from trexmodel.models.datastore.merchant_models import ReceiptSetup
 
-def construct_setting_by_outlet(outlet, pos_setting=None):
+def construct_setting_by_outlet(outlet, device_setting=None):
 
 
     merchant_acct           = outlet.merchant_acct_entity
     invoice_no_generation   = InvoiceNoGeneration.getByMerchantAcct(merchant_acct)
     rounding_setup          = RoundingSetup.get_by_merchant_acct(merchant_acct)
     receipt_setup           = ReceiptSetup.get_by_merchant_acct(merchant_acct)
     dinning_option_json     = []
@@ -84,21 +84,26 @@
                     'address'                    : outlet.address,
                     'email'                      : outlet.email,
                     'phone'                      : outlet.office_phone,
                     'website'                    : merchant_acct.website or '',  
                         
                     }
     
+    program_configurations = {
+                            'prepaid_configuration': merchant_acct.prepaid_configuration,
+                            }
+    
     setting =  {
                 'company_name'                      : merchant_acct.company_name,
                 'website'                           : merchant_acct.website,
                 'account_id'                        : merchant_acct.key_in_str,
                 'api_key'                           : merchant_acct.api_key,
                 'logo_image_url'                    : merchant_acct.logo_public_url,
                 'account_settings'                  : account_settings,
                 'outlet_details'                    : outlet_details,
+                'program_configurations'            : program_configurations,
                 } 
-    if pos_setting:
-        setting['activation_code']  = pos_setting.activation_code
-        setting['pos_name']         = pos_setting.pos_name
+    if device_setting:
+        setting['activation_code']  = device_setting.activation_code
+        setting['device_name']      = device_setting.device_name
         
     return setting
```

### Comparing `trex-model-0.2.8/trexmodel/program_conf.py` & `trex-model-0.2.9/trexmodel/program_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 VOUCHER_REWARD_CASH                          = 'cash'
 VOUCHER_REWARD_PRODUCT_CATEGORY              = 'category'
 VOUCHER_REWARD_PRODUCT_SKU                   = 'SKU'
 VOUCHER_REWARD_MIN_SALES_AMOUNT              = 'min_sales_amount'
 VOUCHER_REWARD_DISCOUNT_RATE                 = 'discount_rate'
 VOUCHER_REWARD_BRAND                         = 'brand'
 VOUCHER_REWARD_PRICE                         = 'price'
+VOUCHER_REWARD_MAX_QUANTITY                  = 'max_quantity'
 
 VOUCHER_REWARD_TYPE_CASH                     = 'cash' 
 VOUCHER_REWARD_TYPE_PRODUCT                  = 'product'
 VOUCHER_REWARD_TYPE_DISCOUNT                 = 'discount'
    
 VOUCHER_TYPE                                 = [
                                                 VOUCHER_REWARD_TYPE_CASH,
@@ -205,14 +206,15 @@
 MEMBERSHIP_UPGRADE_EXPIRY_TYPE_NEW_EXPIRY                           = 'new_expiry'
 
 
 REWARD_STATUS_VALID        = 'valid'
 REWARD_STATUS_REACH_LIMIT  = 'limit'
 REWARD_STATUS_REDEEMED     = 'redeemed'
 REWARD_STATUS_REVERTED     = 'reverted'
+REWARD_STATUS_REMOVED      = 'removed'
 
 REDEEM_STATUS_VALID        = 'valid'
 REDEEM_STATUS_REVERTED     = 'reverted'
 
 
 REDEEM_CODE_LENGTH                                                  = 12
```

### Comparing `trex-model-0.2.8/trexmodel/utils/model/model_util.py` & `trex-model-0.2.9/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

