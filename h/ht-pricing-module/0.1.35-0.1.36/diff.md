# Comparing `tmp/ht_pricing_module-0.1.35.tar.gz` & `tmp/ht_pricing_module-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.1.35.tar", last modified: Mon Apr 10 00:35:43 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.1.36.tar", last modified: Wed Apr 12 10:50:36 2023, max compression
```

## Comparing `ht_pricing_module-0.1.35.tar` & `ht_pricing_module-0.1.36.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.864309 ht_pricing_module-0.1.35/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.1.35/MANIFEST.in
--rw-rw-rw-   0        0        0      264 2023-04-10 00:35:43.863311 ht_pricing_module-0.1.35/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.503477 ht_pricing_module-0.1.35/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.1.35/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.532510 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.542227 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.492476 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.562384 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.581201 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    45777 2023-04-03 01:09:32.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.595197 ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.604439 ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3138 2023-04-10 00:30:32.000000 ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.606385 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4419 2023-03-23 01:53:37.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.616492 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.629662 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.707738 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      506 2023-03-22 14:42:29.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4297 2023-03-20 08:02:19.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3465 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4274 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     5175 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4452 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4257 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3519 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4506 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4583 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5223 2023-04-03 01:46:37.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.709733 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     4012 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.731864 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.772114 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.775107 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1131 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2298 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.800351 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2302 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.809358 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     3634 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.812349 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2555 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2330 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.824317 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     7325 2023-02-23 05:31:40.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.835317 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2396 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.851344 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.855333 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2260 2023-03-20 08:04:04.000000 ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    43817 2023-04-03 01:07:06.000000 ht_pricing_module-0.1.35/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:35:43.520406 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      264 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4791 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-10 00:35:43.000000 ht_pricing_module-0.1.35/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 00:35:43.864309 ht_pricing_module-0.1.35/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-04-10 00:18:37.000000 ht_pricing_module-0.1.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.655034 ht_pricing_module-0.1.36/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.1.36/MANIFEST.in
+-rw-rw-rw-   0        0        0      264 2023-04-12 10:50:36.655034 ht_pricing_module-0.1.36/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.220534 ht_pricing_module-0.1.36/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.1.36/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.248459 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.257435 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.201589 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.278403 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.296673 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    45777 2023-04-03 01:09:32.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.310658 ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.320631 ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.333625 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4499 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.345593 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.360553 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.455377 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      506 2023-03-22 14:42:29.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4317 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3485 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4294 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     5195 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4472 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4277 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3539 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4526 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4603 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5243 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.463355 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     4012 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.486294 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.529179 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.533168 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1131 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2318 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.556107 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2322 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.566080 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     3714 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.586133 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2555 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2350 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     3452 2023-04-12 02:15:47.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.599098 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     7325 2023-02-23 05:31:40.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.622089 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2416 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.642069 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.646058 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2280 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    43817 2023-04-03 01:07:06.000000 ht_pricing_module-0.1.36/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.235494 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4864 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:50:36.655034 ht_pricing_module-0.1.36/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-04-12 10:50:22.000000 ht_pricing_module-0.1.36/setup.py
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/fd_grid_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..api_and_utils import np, qmc, warnings, lru_cache, wraps
 
-warnings.filterwarnings('ignore')
+# warnings.filterwarnings('ignore')
 
 
 def mc_np_cache(function):
     @lru_cache(maxsize=2)
     def cached_wrapper(qmc_flag, antithetic_flag, random_seed, M, drift, volatility, hashable_array):
         return function(qmc_flag, antithetic_flag, random_seed, M, drift, volatility,  np.array(hashable_array))
 
@@ -33,40 +33,42 @@
     cum_log_rtn = np.cumsum(log_rtn, axis=1)
     cum_log_rtn = np.hstack([np.zeros([len(cum_log_rtn), 1]), cum_log_rtn])
     exp_cum_log_rtn = np.exp(cum_log_rtn)
     return exp_cum_log_rtn
 
 
 class McPathGenerator:
-    """
-
-    蒙特卡洛路径生成函数，输出结果为spot价格为1的几何布朗运动
-    :param riskfree_rate: 无风险利率
-    :param dividend: 分红率
-    :param volatility: 波动率
-    :param intraday: 日内时间
-    :param expiry_date: 到日期离当前日收盘天数
-    :param year_base: 年化日历天数
-    :param path_num: 路径数
-    :param antithetic_flag: 是否使用对偶变量
-    :param qmc_flag: 是否使用quasi-monte carlo，使用Sobol低差异化序列
-    :param random_seed: 指定随机种子
-
-    e.g.
-    intraday = 0.2
-    expiry_date = 252
-    剩余整数天数为252天，当前日内时间为0.8天，当日剩余天数为0.2天，则剩余到期时间为251.2天。
-    生成时间序列为[0, 0.2, 1.2, 2.2, ... 251.2], 长度为253；
-    生成时间间隔dt序列为[0.2, 1, 1, 1, ... 1], 长度为252；
-    返回长度为253的几何布朗运动，其中第一列是1，为当前时刻价格，后面252列为每个观测日(日终)；
-    将返回矩阵乘以当前价格即可得到价格路径。
-    """
 
     @classmethod
     def generate(cls, riskfree_rate, dividend, volatility, intraday, expiry_date, year_base,
                  path_num=100000, antithetic_flag=True, qmc_flag=True, random_seed=None):
+
+        """
+
+          蒙特卡洛路径生成函数，输出结果为spot价格为1的几何布朗运动
+          :param riskfree_rate: 无风险利率
+          :param dividend: 分红率
+          :param volatility: 波动率
+          :param intraday: 日内时间
+          :param expiry_date: 到日期离当前日收盘天数
+          :param year_base: 年化日历天数
+          :param path_num: 路径数
+          :param antithetic_flag: 是否使用对偶变量
+          :param qmc_flag: 是否使用quasi-monte carlo，使用Sobol低差异化序列
+          :param random_seed: 指定随机种子
+
+          e.g.
+          intraday = 0.2
+          expiry_date = 252
+          剩余整数天数为252天，当前日内时间为0.8天，当日剩余天数为0.2天，则剩余到期时间为251.2天。
+          生成时间序列为[0, 0.2, 1.2, 2.2, ... 251.2], 长度为253；
+          生成时间间隔dt序列为[0.2, 1, 1, 1, ... 1], 长度为252；
+          返回长度为253的几何布朗运动，其中第一列是1，为当前时刻价格，后面252列为每个观测日(日终)；
+          将返回矩阵乘以当前价格即可得到价格路径。
+          """
+
         drift = riskfree_rate - dividend - 0.5 * volatility ** 2
         t_arr = np.arange(1, expiry_date + 1, 1) - intraday
         t_arr = np.hstack([0, t_arr])
         dt_arr = (t_arr[1:] - t_arr[:-1]) / year_base
         gmb_trn = generate_randn(qmc_flag, antithetic_flag, random_seed, path_num, drift, volatility, dt_arr)
         return gmb_trn
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
     def __init__(self, param):
         self.param = Struct(param) if isinstance(param, dict) else param
 
     def __calculate_present_value__(self) -> float:
         raise NotImplementedError()
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def present_value(self) -> float:
         return self.__calculate_present_value__()
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def delta(self, leg: int, step: float = 0.001) -> float:
         spot_price = f'spot_price{leg}'
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         if time_to_expiry <= 0:
             return 0.0
 
         if hasattr(self.param, spot_price):
@@ -27,47 +27,47 @@
             pricer_up = deepcopy(self)
             setattr(pricer_up.param, spot_price, spot_up)
             pricer_down = deepcopy(self)
             setattr(pricer_down.param, spot_price, spot_down)
             return (pricer_up.present_value() - pricer_down.present_value()) / (spot_up - spot_down)
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def gamma(self, leg: int, step: float = 0.001) -> float:
         spot_price = f'spot_price{leg}'
         if hasattr(self.param, spot_price):
             spot_up = getattr(self.param, spot_price) * (1 + step)
             spot_down = getattr(self.param, spot_price) * (1 - step)
             pricer_up = deepcopy(self)
             setattr(pricer_up.param, spot_price, spot_up)
             pricer_down = deepcopy(self)
             setattr(pricer_down.param, spot_price, spot_down)
             return (pricer_up.present_value() + pricer_down.present_value() - 2 * self.present_value()) / pow((spot_up - spot_down) / 2, 2) 
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def vega(self, leg: int, step: float = 0.01) -> float:
         volatility = f'volatility{leg}'
         if hasattr(self.param, volatility):
             vol_up = getattr(self.param, volatility) + step
             pricer_up = deepcopy(self)
             setattr(pricer_up.param, volatility, vol_up)
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def rho(self, step: float = 0.0001) -> float:
         if hasattr(self.param, 'riskfree_rate'):
             current_up = self.param.riskfree_rate + step
             pricer_up = deepcopy(self)
             pricer_up.param.riskfree_rate = current_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
@@ -79,24 +79,24 @@
             pricer_up = deepcopy(self)
             pricer_up.param.correlation = corr_up
             pricer_down = deepcopy(self)
             pricer_down.param.correlation = corr_down
             return (pricer_up.present_value() - pricer_down.present_value()) / 2
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, leg: int, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             return pricer_up.delta(leg=leg, step=price_step) - self.delta(leg=leg, step=price_step)
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadv(self, leg: int, vol_step: float = 0.01, price_step: float = 0.001):
         volatility = f'volatility{leg}'
         if hasattr(self.param, volatility):
             vol_up = getattr(self.param, volatility) + vol_step
             pricer_up = deepcopy(self)
             setattr(pricer_up.param, volatility, vol_up)
             return pricer_up.delta(leg=leg, step=price_step) - self.delta(leg=leg, step=price_step)
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,27 +53,27 @@
             param['payoff'] = self.param.payoff
             param['obs_freq'] = self.param.obs_freq
             barrier_binary = DiscreteBarrierBinary(param)
             rst = rst + (-self.param.leverage * leveraged_barrier.present_value()
                          + barrier_binary.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,27 +40,27 @@
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
             binary = Binary(param)
             rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
                          + binary.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,27 +55,27 @@
             param['year_base'] = self.param.year_base
             binary2 = Binary(param)
             rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
                          + binary1.present_value()
                          - binary2.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,27 +70,27 @@
 
             rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
                          + non_leveraged_binary1.present_value()
                          - non_leveraged_binary2.present_value()
                          + non_leveraged_vanilla.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ..one_asset_option_base import *
-from ..vanilla import Vanilla
-from ..binary import Binary
+from ..sharkfin.sharkfin_as import Sharkfin
+from ..vanilla.vanilla_as import Vanilla
 
 
-class FixedAccEnhanced(OneAssetOptionBase):
+class LinearAccEnhanced(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
         leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
                                          OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        binary_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                              OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        sharkfin_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
+                                OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         enhanced_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
                                         OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
             param['option_type'] = leveraged_vanilla_option_type
             param['exercise_type'] = self.param.exercise_type
@@ -26,26 +26,26 @@
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             leveraged_vanilla = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = binary_option_type
+            param['option_type'] = sharkfin_option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
+            param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
-            param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            binary = Binary(param)
+            sharkfin = Sharkfin(param)
 
             param = Struct({})
             param['option_type'] = enhanced_vanilla_option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
@@ -53,31 +53,31 @@
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             enhanced_vanilla = Vanilla(param)
 
             rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + binary.present_value()
+                         + sharkfin.present_value()
                          + enhanced_vanilla.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,27 +53,27 @@
             param['obs_freq'] = self.param.obs_freq
             non_leveraged_barrier = DiscreteBarrier(param)
 
             rst = rst + (-self.param.leverage * leveraged_barrier.present_value()
                          + non_leveraged_barrier.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,27 @@
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             sharkfin = Sharkfin(param)
             rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
                          + sharkfin.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ..one_asset_option_base import *
-from ..sharkfin.sharkfin_as import Sharkfin
-from ..vanilla.vanilla_as import Vanilla
+from ..vanilla import Vanilla
+from ..binary import Binary
 
 
-class LinearAccEnhanced(OneAssetOptionBase):
+class FixedAccEnhanced(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
         leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
                                          OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        sharkfin_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        binary_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
+                              OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         enhanced_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
                                         OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
             param['option_type'] = leveraged_vanilla_option_type
             param['exercise_type'] = self.param.exercise_type
@@ -26,26 +26,26 @@
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             leveraged_vanilla = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = sharkfin_option_type
+            param['option_type'] = binary_option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
-            param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
+            param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            sharkfin = Sharkfin(param)
+            binary = Binary(param)
 
             param = Struct({})
             param['option_type'] = enhanced_vanilla_option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
@@ -53,31 +53,31 @@
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             enhanced_vanilla = Vanilla(param)
 
             rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + sharkfin.present_value()
+                         + binary.present_value()
                          + enhanced_vanilla.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,27 +59,27 @@
             enhanced_binary = Binary(param)
 
             rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
                          + sharkfin.present_value()
                          + enhanced_binary.present_value())
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,27 +73,27 @@
         param['rebate'] = 0
         param['obs_freq'] = self.param.obs_freq
         fusing_barrier = DiscreteBarrier(param)
 
         rst = rst - fusing_barrier.present_value() * self.param.final_position_multiplier
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..one_asset_option_base import *
-from ..basket.basket_vanilla_as import BasketVanilla
+from ..vanilla.vanilla_as import Vanilla
 
 
-class BasketVanillaSeries(OneAssetOptionBase):
+class VanillaSeries(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
         for obs in self.param.obs_date:
             param = Struct({})
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
@@ -14,31 +14,31 @@
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            basket_vanilla = BasketVanilla(param)
-            rst = rst + basket_vanilla.present_value() / len(self.param.obs_date)
+            vanilla = Vanilla(param)
+            rst = rst + vanilla.present_value() / len(self.param.obs_date)
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,27 @@
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
             binary = Binary(param)
             rst = rst + binary.present_value() / len(self.param.obs_date)
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
     def __init__(self, param):
         self.param = Struct(param) if isinstance(param, dict) else param
 
     def __calculate_present_value__(self) -> float:
         raise NotImplementedError()
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def present_value(self) -> float:
         return self.__calculate_present_value__()
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def delta(self, step: float = 0.001) -> float:
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         if time_to_expiry <= 0:
             return 0.0
 
         if hasattr(self.param, 'spot_price'):
             spot_up = self.param.spot_price * (1 + step)
@@ -26,63 +26,63 @@
             pricer_up = deepcopy(self)
             pricer_up.param.spot_price = spot_up
             pricer_down = deepcopy(self)
             pricer_down.param.spot_price = spot_down
             return (pricer_up.present_value() - pricer_down.present_value()) / (spot_up - spot_down)
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def gamma(self, step: float = 0.001) -> float:
         if hasattr(self.param, 'spot_price'):
             spot_up = self.param.spot_price * (1 + step)
             spot_down = self.param.spot_price * (1 - step)
             pricer_up = deepcopy(self)
             pricer_up.param.spot_price = spot_up
             pricer_down = deepcopy(self)
             pricer_down.param.spot_price = spot_down
             return (pricer_up.present_value() + pricer_down.present_value() - 2 * self.present_value()) / pow((spot_up - spot_down) / 2, 2) 
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def vega(self, step: float = 0.01) -> float:
         if hasattr(self.param, 'volatility'):
             vol_up = self.param.volatility + step
             pricer_up = deepcopy(self)
             pricer_up.param.volatility = vol_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def rho(self, step: float = 0.0001) -> float:
         if hasattr(self.param, 'riskfree_rate'):
             current_up = self.param.riskfree_rate + step
             pricer_up = deepcopy(self)
             pricer_up.param.riskfree_rate = current_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             return pricer_up.delta(step=price_step) - self.delta(step=price_step)
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadv(self, vol_step: float = 0.01, price_step: float = 0.001):
         if hasattr(self.param, 'volatility') and hasattr(self.param, 'spot_price'):
             vol_up = self.param.volatility + vol_step
             pricer_up = deepcopy(self)
             pricer_up.param.volatility = vol_up
             return pricer_up.delta(step=price_step) - self.delta(step=price_step)
         return 0.0
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,27 @@
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             sharkfin = Sharkfin(param)
             rst = rst + sharkfin.present_value() / len(self.param.obs_date)
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,27 @@
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             ratio_spread = RatioSpread(param)
             rst = rst + ratio_spread.present_value() / len(self.param.obs_date)
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..one_asset_option_base import *
-from ..vanilla.vanilla_as import Vanilla
+from ..basket.basket_vanilla_as import BasketVanilla
 
 
-class VanillaSeries(OneAssetOptionBase):
+class BasketVanillaSeries(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
         for obs in self.param.obs_date:
             param = Struct({})
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
@@ -14,31 +14,31 @@
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            vanilla = Vanilla(param)
-            rst = rst + vanilla.present_value() / len(self.param.obs_date)
+            basket_vanilla = BasketVanilla(param)
+            rst = rst + basket_vanilla.present_value() / len(self.param.obs_date)
         return rst
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    # @lru_cache
+    @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
```

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.1.36/ht_pricing_module/simple_pricer_engine.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.35/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.1.36/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
 ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
 ht_pricing_module/one_asset_pricing_module/forward/__init__.py
 ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
 ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
 ht_pricing_module/one_asset_pricing_module/spread/__init__.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
 ht_pricing_module/one_asset_pricing_module/touch/__init__.py
 ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
```

### Comparing `ht_pricing_module-0.1.35/setup.py` & `ht_pricing_module-0.1.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.1.35"
+VERSION = "0.1.36"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```

