# Comparing `tmp/fastsim-2.0.10.tar.gz` & `tmp/fastsim-2.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsim-2.0.10.tar", last modified: Tue Apr  4 19:34:48 2023, max compression
+gzip compressed data, was "fastsim-2.0.11.tar", last modified: Wed Apr 12 16:13:21 2023, max compression
```

## Comparing `fastsim-2.0.10.tar` & `fastsim-2.0.11.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.986611 fastsim-2.0.10/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-04 19:34:36.000000 fastsim-2.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-04 19:34:36.000000 fastsim-2.0.10/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-04 19:34:36.000000 fastsim-2.0.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-04 19:34:48.982611 fastsim-2.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 19:34:36.000000 fastsim-2.0.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.898610 fastsim-2.0.10/fastsim/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    37947 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.906610 fastsim-2.0.10/fastsim/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/2017_Ford_F150_thermal_val.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/accel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/demo_abc_drag_coef_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/demo_eu_vehicle_wltp.py
--rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/fastsim-icon-web-131x172.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/fusion_thermal_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/fusion_thermal_cal_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/fusion_thermal_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/mp_parallel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/stop_start_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/time_dilation_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/docs/wltc_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/inspect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.906610 fastsim-2.0.10/fastsim/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/FASTSim_py_veh_db.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.918610 fastsim-2.0.10/fastsim/resources/cycles/
--rw-r--r--   0 runner    (1001) docker     (123)    77093 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/NREL13.csv
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/accel.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.886610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.918610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.922610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/
--rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
--rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.922610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4105836_2/
--rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.930610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/
--rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.938610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/
--rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.942610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/
--rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.942610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/
--rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.946610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/
--rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.946610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4112082_1/
--rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
--rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.946610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4113492_1/
--rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.946610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4114555_1/
--rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.950610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_1/
--rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.950610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_2/
--rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.950610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115957_1/
--rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.950610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115985_1/
--rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.950610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116361_1/
--rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.950610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116721_2/
--rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.954610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116728_1/
--rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.954610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_1/
--rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.954610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_2/
--rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.954610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116880_1/
--rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.958610 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4118093_1/
--rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
--rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/ftpmc1b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/hwfet.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/longHaulDriveCycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/udds.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/us06.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_extra_high3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_high3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_high3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_low3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_med3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_med3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wmtc_all.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wmtc_part1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wmtc_part2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/cycles/wmtc_part3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/longparams.json
--rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/master_benchmark_vars.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/res_excel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.970610 fastsim-2.0.10/fastsim/resources/vehdb/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Focus.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Focus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Fusion.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/Class_4_Box_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/Line_Haul_Conv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/Line_Haul_Conv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/fail_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/fail_overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/legacy_template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/legacy_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/test_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/test_overrides.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.970610 fastsim-2.0.10/fastsim/resources/vehdb/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/rustext.py
--rw-r--r--   0 runner    (1001) docker     (123)   116238 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    25085 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/simdrivelabel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.974610 fastsim-2.0.10/fastsim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    60185 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_coasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_eco_cruise.py
--rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_following.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_rust.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_simdrive_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_soc_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/tests/test_vs_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33327 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-04 19:34:36.000000 fastsim-2.0.10/fastsim/vehicle_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.898610 fastsim-2.0.10/fastsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-04 19:34:48.000000 fastsim-2.0.10/fastsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-04 19:34:48.000000 fastsim-2.0.10/fastsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:34:48.000000 fastsim-2.0.10/fastsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:34:48.000000 fastsim-2.0.10/fastsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-04 19:34:48.000000 fastsim-2.0.10/fastsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 19:34:48.000000 fastsim-2.0.10/fastsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-04 19:34:36.000000 fastsim-2.0.10/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.974610 fastsim-2.0.10/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.974610 fastsim-2.0.10/rust/fastsim-core/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.974610 fastsim-2.0.10/rust/fastsim-core/proc-macros/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/proc-macros/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.974610 fastsim-2.0.10/rust/fastsim-core/proc-macros/src/
--rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/proc-macros/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/proc-macros/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/proc-macros/src/utilities.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.982611 fastsim-2.0.10/rust/fastsim-core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/air.rs
--rw-r--r--   0 runner    (1001) docker     (123)    38373 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/cycle.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.982611 fastsim-2.0.10/rust/fastsim-core/src/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/html/docs-header.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/macros.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/params.rs
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/pyo3imports.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.982611 fastsim-2.0.10/rust/fastsim-core/src/simdrive/
--rw-r--r--   0 runner    (1001) docker     (123)    47410 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/simdrive/cyc_mods.rs
--rw-r--r--   0 runner    (1001) docker     (123)    77870 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/simdrive/simdrive_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/simdrive.rs
--rw-r--r--   0 runner    (1001) docker     (123)    41189 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/simdrivelabel.rs
--rw-r--r--   0 runner    (1001) docker     (123)    48266 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/traits.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/vehicle.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/vehicle_thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-core/src/vehicle_utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.982611 fastsim-2.0.10/rust/fastsim-py/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:34:48.982611 fastsim-2.0.10/rust/fastsim-py/src/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-04 19:34:36.000000 fastsim-2.0.10/rust/fastsim-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:34:48.986611 fastsim-2.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-04 19:34:36.000000 fastsim-2.0.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.156501 fastsim-2.0.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 16:13:09.000000 fastsim-2.0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 16:13:09.000000 fastsim-2.0.11/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 16:13:09.000000 fastsim-2.0.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-12 16:13:21.156501 fastsim-2.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 16:13:09.000000 fastsim-2.0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.100497 fastsim-2.0.11/fastsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/auxiliaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37947 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/cycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.104497 fastsim-2.0.11/fastsim/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/2017_Ford_F150_thermal_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/accel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/cav_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/cav_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/demo_abc_drag_coef_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/demo_eu_vehicle_wltp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/fastsim-icon-web-131x172.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/fusion_thermal_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/fusion_thermal_cal_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/fusion_thermal_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/mp_parallel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/stop_start_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/time_dilation_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/docs/wltc_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/inspect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.104497 fastsim-2.0.11/fastsim/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/FASTSim_py_veh_db.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.112498 fastsim-2.0.11/fastsim/resources/cycles/
+-rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/NREL13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/accel.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.096497 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.112498 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.112498 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/
+-rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.112498 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4105836_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.116498 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.120499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/
+-rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.124499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.124499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.128499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.128499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4112082_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.128499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4113492_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.128499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4114555_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.132499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.132499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.132499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115957_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.132499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115985_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.132499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116361_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.132499 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116721_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.136500 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116728_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.136500 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.136500 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.136500 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116880_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.136500 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4118093_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/ftpmc1b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/hwfet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/longHaulDriveCycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/udds.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/us06.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_extra_high3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_high3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_high3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_low3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_med3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_med3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wmtc_all.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wmtc_part1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wmtc_part2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/cycles/wmtc_part3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/longparams.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/master_benchmark_vars.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/res_excel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.144500 fastsim-2.0.11/fastsim/resources/vehdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Focus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Focus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Fusion.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/Class_4_Box_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/Line_Haul_Conv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/Line_Haul_Conv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/fail_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/fail_overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/legacy_template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/legacy_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/test_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/test_overrides.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.144500 fastsim-2.0.11/fastsim/resources/vehdb/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/rustext.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116240 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/simdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25085 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/simdrivelabel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.148501 fastsim-2.0.11/fastsim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_auxiliaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_cav_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_cav_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60185 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_coasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_eco_cruise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_following.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_rust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_simdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_simdrive_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_soc_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/tests/test_vs_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33327 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-12 16:13:09.000000 fastsim-2.0.11/fastsim/vehicle_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.104497 fastsim-2.0.11/fastsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-12 16:13:21.000000 fastsim-2.0.11/fastsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-12 16:13:21.000000 fastsim-2.0.11/fastsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:13:21.000000 fastsim-2.0.11/fastsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:13:21.000000 fastsim-2.0.11/fastsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 16:13:21.000000 fastsim-2.0.11/fastsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 16:13:21.000000 fastsim-2.0.11/fastsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-12 16:13:09.000000 fastsim-2.0.11/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.148501 fastsim-2.0.11/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.148501 fastsim-2.0.11/rust/fastsim-core/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.148501 fastsim-2.0.11/rust/fastsim-core/proc-macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/proc-macros/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.152501 fastsim-2.0.11/rust/fastsim-core/proc-macros/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/proc-macros/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/proc-macros/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/proc-macros/src/utilities.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.152501 fastsim-2.0.11/rust/fastsim-core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/air.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/cycle.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.156501 fastsim-2.0.11/rust/fastsim-core/src/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/html/docs-header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/pyo3imports.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.156501 fastsim-2.0.11/rust/fastsim-core/src/simdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/simdrive/cyc_mods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    77871 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/simdrive/simdrive_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/simdrive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    41736 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/simdrivelabel.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    48266 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/vehicle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/vehicle_thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-core/src/vehicle_utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.156501 fastsim-2.0.11/rust/fastsim-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:13:21.156501 fastsim-2.0.11/rust/fastsim-py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 16:13:09.000000 fastsim-2.0.11/rust/fastsim-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:13:21.156501 fastsim-2.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 16:13:09.000000 fastsim-2.0.11/setup.py
```

### Comparing `fastsim-2.0.10/LICENSE` & `fastsim-2.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/LICENSE.md` & `fastsim-2.0.11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/auxiliaries.py` & `fastsim-2.0.11/fastsim/auxiliaries.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/calibration.py` & `fastsim-2.0.11/fastsim/calibration.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/cycle.py` & `fastsim-2.0.11/fastsim/cycle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/2017_Ford_F150_thermal_val.py` & `fastsim-2.0.11/fastsim/docs/2017_Ford_F150_thermal_val.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/README.md` & `fastsim-2.0.11/fastsim/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
 regen = associated with regenerative braking  
 des = desired value  
 ach = achieved value  
 in = component input  
 out = component output  
 
 # Release Notes
+2.0.11 -- fixes related to PyPI web rendering
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes
 2.0.9 -- support for mac ARM/RISC architecture
 2.0.8 -- performance improvements
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`  
 2.0.3 -- exposed `veh.__post_init__`
```

### Comparing `fastsim-2.0.10/fastsim/docs/accel_demo.py` & `fastsim-2.0.11/fastsim/docs/accel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/cav_demo.py` & `fastsim-2.0.11/fastsim/docs/cav_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/cav_sweep.py` & `fastsim-2.0.11/fastsim/docs/cav_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/demo.py` & `fastsim-2.0.11/fastsim/docs/demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/demo_abc_drag_coef_conv.py` & `fastsim-2.0.11/fastsim/docs/demo_abc_drag_coef_conv.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/demo_eu_vehicle_wltp.py` & `fastsim-2.0.11/fastsim/docs/demo_eu_vehicle_wltp.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/fastsim-icon-web-131x172.jpg` & `fastsim-2.0.11/fastsim/docs/fastsim-icon-web-131x172.jpg`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/fusion_thermal_cal.py` & `fastsim-2.0.11/fastsim/docs/fusion_thermal_cal.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/fusion_thermal_cal_post.py` & `fastsim-2.0.11/fastsim/docs/fusion_thermal_cal_post.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/fusion_thermal_demo.py` & `fastsim-2.0.11/fastsim/docs/fusion_thermal_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/mp_parallel_demo.py` & `fastsim-2.0.11/fastsim/docs/mp_parallel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/stop_start_demo.py` & `fastsim-2.0.11/fastsim/docs/stop_start_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/time_dilation_demo.py` & `fastsim-2.0.11/fastsim/docs/time_dilation_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/docs/wltc_calibration.py` & `fastsim-2.0.11/fastsim/docs/wltc_calibration.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/inspect_utils.py` & `fastsim-2.0.11/fastsim/inspect_utils.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/parameters.py` & `fastsim-2.0.11/fastsim/parameters.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resample.py` & `fastsim-2.0.11/fastsim/resample.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/FASTSim_py_veh_db.csv` & `fastsim-2.0.11/fastsim/resources/FASTSim_py_veh_db.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/NREL13.csv` & `fastsim-2.0.11/fastsim/resources/cycles/NREL13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv` & `fastsim-2.0.11/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/accel.csv` & `fastsim-2.0.11/fastsim/resources/cycles/accel.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv` & `fastsim-2.0.11/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/ftpmc1b.csv` & `fastsim-2.0.11/fastsim/resources/cycles/ftpmc1b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/hwfet.csv` & `fastsim-2.0.11/fastsim/resources/cycles/hwfet.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/longHaulDriveCycle.csv` & `fastsim-2.0.11/fastsim/resources/cycles/longHaulDriveCycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/udds.csv` & `fastsim-2.0.11/fastsim/resources/cycles/udds.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/us06.csv` & `fastsim-2.0.11/fastsim/resources/cycles/us06.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_extra_high3.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_extra_high3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_high3a.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_high3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_high3b.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_high3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_low3.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_low3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_med3a.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_med3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wltc_class3_med3b.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wltc_class3_med3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wmtc_all.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wmtc_all.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wmtc_part1.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wmtc_part1.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wmtc_part2.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wmtc_part2.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/cycles/wmtc_part3.csv` & `fastsim-2.0.11/fastsim/resources/cycles/wmtc_part3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/longparams.json` & `fastsim-2.0.11/fastsim/resources/longparams.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/master_benchmark_vars.csv` & `fastsim-2.0.11/fastsim/resources/master_benchmark_vars.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/res_excel.json` & `fastsim-2.0.11/fastsim/resources/res_excel.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Focus.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Focus.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Focus.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Focus.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Fusion.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Fusion.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2012_Ford_Fusion.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2012_Ford_Fusion.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/Class_4_Box_Truck.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/Class_4_Box_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/Class_4_Box_Truck.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/Class_4_Box_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/Line_Haul_Conv.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/Line_Haul_Conv.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/Line_Haul_Conv.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/Line_Haul_Conv.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/fail_overrides.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/fail_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/fail_overrides.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/fail_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/legacy_template.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/legacy_template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/legacy_template.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/legacy_template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/template.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/template.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/test_overrides.csv` & `fastsim-2.0.11/fastsim/resources/vehdb/test_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/test_overrides.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/test_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml` & `fastsim-2.0.11/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/simdrive.py` & `fastsim-2.0.11/fastsim/simdrive.py`

 * *Files 0% similar despite different names*

```diff
@@ -2464,18 +2464,18 @@
         - final integrated value of all positive powers
         - final integrated value of all negative powers
         - total distance traveled
         - miles per gallon gasoline equivalent (mpgge)"""
 
         base_var_list = list(self.__dict__.keys())
         pw_var_list = [var for var in base_var_list if re.search(
-            '\w*_kw(?!h)\w*', var)]
+            r'\w*_kw(?!h)\w*', var)]
         # find all vars containing 'Kw' but not 'Kwh'
 
-        prog = re.compile('(\w*)_kw(?!h)(\w*)')
+        prog = re.compile(r'(\w*)_kw(?!h)(\w*)')
         # find all vars containing 'Kw' but not Kwh and capture parts before and after 'Kw'
         # using compile speeds up iteration
 
         # create positive and negative versions of all time series with units of kW
         # then integrate to find cycle end pos and negative energies
         tempvars = {}  # dict for contaning intermediate variables
         output = {}
```

### Comparing `fastsim-2.0.10/fastsim/simdrivelabel.py` & `fastsim-2.0.11/fastsim/simdrivelabel.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_auxiliaries.py` & `fastsim-2.0.11/fastsim/tests/test_auxiliaries.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_cav_demo.py` & `fastsim-2.0.11/fastsim/tests/test_cav_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_cav_sweep.py` & `fastsim-2.0.11/fastsim/tests/test_cav_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_coasting.py` & `fastsim-2.0.11/fastsim/tests/test_coasting.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_copy.py` & `fastsim-2.0.11/fastsim/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_cycle.py` & `fastsim-2.0.11/fastsim/tests/test_cycle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_demo.py` & `fastsim-2.0.11/fastsim/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_eco_cruise.py` & `fastsim-2.0.11/fastsim/tests/test_eco_cruise.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_following.py` & `fastsim-2.0.11/fastsim/tests/test_following.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_logging.py` & `fastsim-2.0.11/fastsim/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_rust.py` & `fastsim-2.0.11/fastsim/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_simdrive.py` & `fastsim-2.0.11/fastsim/tests/test_simdrive.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_simdrive_sweep.py` & `fastsim-2.0.11/fastsim/tests/test_simdrive_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_soc_correction.py` & `fastsim-2.0.11/fastsim/tests/test_soc_correction.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_vehicle.py` & `fastsim-2.0.11/fastsim/tests/test_vehicle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/tests/test_vs_excel.py` & `fastsim-2.0.11/fastsim/tests/test_vs_excel.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/utilities.py` & `fastsim-2.0.11/fastsim/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     if isinstance(level, str):
         level = logging._nameToLevel[level]
     # Extract previous log level and set new log level
     fastsim_logger = logging.getLogger("fastsim")
     previous_level = fastsim_logger.level
     fastsim_logger.setLevel(level)
     if RUST_AVAILABLE:
-        fastsimrust_logger = logging.getLogger("fastsimrust")
+        fastsimrust_logger = logging.getLogger("fastsim_core")
         fastsimrust_logger.setLevel(level)
     return previous_level
 
 def disable_logging() -> int:
     """
     Disable FASTSim logs from being shown by setting log level
     to CRITICAL+1 (51).
```

### Comparing `fastsim-2.0.10/fastsim/vehicle.py` & `fastsim-2.0.11/fastsim/vehicle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim/vehicle_base.py` & `fastsim-2.0.11/fastsim/vehicle_base.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/fastsim.egg-info/SOURCES.txt` & `fastsim-2.0.11/fastsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/pyproject.toml` & `fastsim-2.0.11/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = [
-"setuptools>=40.6.0",
-"wheel",
-"setuptools-rust>=0.11.4",
+    "setuptools>=40.6.0",
+    "wheel",
+    "setuptools-rust>=0.11.4",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastsim"
-version = "2.0.10"
-authors = [{ name = "MBAP Group", email = "fastsim@nrel.gov" }]
+version = "2.0.11"
+authors = [{ name = "NREL/MTES/CIMS/MBAP Group", email = "fastsim@nrel.gov" }]
 description = "Tool for modeling vehicle powertrains"
-readme = "README.md"
+readme = "docs/README.md"
+license = {file = "LICENSE.md"}
 requires-python = ">=3.8,<3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: POSIX",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `fastsim-2.0.10/rust/Cargo.toml` & `fastsim-2.0.11/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/Cargo.toml` & `fastsim-2.0.11/rust/fastsim-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs` & `fastsim-2.0.11/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs` & `fastsim-2.0.11/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/proc-macros/src/history_vec_derive.rs` & `fastsim-2.0.11/rust/fastsim-core/proc-macros/src/history_vec_derive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/proc-macros/src/lib.rs` & `fastsim-2.0.11/rust/fastsim-core/proc-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/proc-macros/src/utilities.rs` & `fastsim-2.0.11/rust/fastsim-core/proc-macros/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/air.rs` & `fastsim-2.0.11/rust/fastsim-core/src/air.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/cycle.rs` & `fastsim-2.0.11/rust/fastsim-core/src/cycle.rs`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,19 @@
         &self,
         distance_start_m: f64,
         delta_distance_m: f64,
     ) -> PyResult<f64> {
         Ok(self.average_grade_over_range(distance_start_m, delta_distance_m, None))
     }
 
+    #[pyo3(name = "build_cache")]
+    pub fn build_cache_py(&self) -> PyResult<RustCycleCache> {
+        Ok(self.build_cache())
+    }
+
     #[pyo3(name = "dt_s_at_i")]
     pub fn dt_s_at_i_py(&self, i: usize) -> PyResult<f64> {
         if i == 0 {
             Ok(0.0)
         } else {
             Ok(self.dt_s_at_i(i))
         }
```

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/html/docs-header.html` & `fastsim-2.0.11/rust/fastsim-core/src/html/docs-header.html`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/lib.rs` & `fastsim-2.0.11/rust/fastsim-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/macros.rs` & `fastsim-2.0.11/rust/fastsim-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/params.rs` & `fastsim-2.0.11/rust/fastsim-core/src/params.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/simdrive/cyc_mods.rs` & `fastsim-2.0.11/rust/fastsim-core/src/simdrive/cyc_mods.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1072,15 +1072,15 @@
                             None,
                         );
                         for idx in i_for_brake..self.cyc0.mps.len() {
                             self.impose_coast[idx] = idx < i_for_brake + num_steps;
                         }
                         adjusted_current_speed = true;
                     } else {
-                        log::warn!(target: "fastsimrust",
+                        log::warn!(
                             "final_speed_m_per_s={} not close to coast_brake_start_speed={} for i={}; i_for_brake={}, traj_n={}",
                             final_speed_m_per_s,
                             self.sim_params.coast_brake_start_speed_m_per_s,
                             i,
                             i_for_brake,
                             traj_n
                         );
```

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/simdrive/simdrive_impl.rs` & `fastsim-2.0.11/rust/fastsim-core/src/simdrive/simdrive_impl.rs`

 * *Files 1% similar despite different names*

```diff
@@ -428,15 +428,18 @@
                                 * self.veh.ess_max_kwh
                                 * 3.6e3
                                 / (fuel_kj + roadway_chg_kj))
                                 .abs();
                         } else {
                             ess_2fuel_kwh = 0.0;
                         }
-                        init_soc = min(1.0, max(0.0, *self.soc.last().unwrap()));
+                        init_soc = min(
+                            self.veh.max_soc,
+                            max(self.veh.min_soc, *self.soc.last().unwrap()),
+                        );
                     }
                     init_soc
                 } else if self.veh.veh_pt_type == PHEV || self.veh.veh_pt_type == BEV {
                     // If EV, initializing initial SOC to maximum SOC.
                     self.veh.max_soc
                 } else {
                     panic!("Failed to properly initialize SOC.");
@@ -702,19 +705,19 @@
                     self.veh.mc_max_kw,
                 );
             } else {
                 self.mc_elec_in_lim_kw[i] = min(
                     self.veh.mc_kw_out_array[first_grtr(
                         &self.veh.mc_kw_in_array,
                         min(
-                            arrmax(&self.veh.mc_kw_in_array) - 0.01,
+                            arrmax(&self.veh.mc_kw_in_array) * 0.9999,
                             self.cur_max_avail_elec_kw[i],
                         ),
                     )
-                    .unwrap_or(0)
+                    .unwrap()
                         - 1_usize],
                     self.veh.mc_max_kw,
                 )
             }
         } else {
             self.mc_elec_in_lim_kw[i] = 0.0;
         }
@@ -738,17 +741,17 @@
                 self.cur_max_mc_kw_out[i] / self.veh.mc_full_eff_array.last().unwrap();
         } else {
             self.cur_max_mc_elec_kw_in[i] = self.cur_max_mc_kw_out[i]
                 / self.veh.mc_full_eff_array[cmp::max(
                     1,
                     first_grtr(
                         &self.veh.mc_kw_out_array,
-                        min(self.veh.mc_max_kw - 0.01, self.cur_max_mc_kw_out[i]),
+                        min(self.veh.mc_max_kw * 0.9999, self.cur_max_mc_kw_out[i]),
                     )
-                    .unwrap_or(0)
+                    .unwrap()
                         - 1,
                 )]
         }
 
         if self.veh.mc_max_kw == 0.0 {
             self.ess_lim_mc_regen_perc_kw[i] = 0.0;
         } else {
@@ -770,15 +773,15 @@
                 self.veh.mc_max_kw,
                 self.cur_max_ess_chg_kw[i]
                     / self.veh.mc_full_eff_array[cmp::max(
                         1,
                         first_grtr(
                             &self.veh.mc_kw_out_array,
                             min(
-                                self.veh.mc_max_kw - 0.01,
+                                self.veh.mc_max_kw * 0.9999,
                                 self.cur_max_ess_chg_kw[i] - self.cur_max_roadway_chg_kw[i],
                             ),
                         )
                         .unwrap_or(0)
                             - 1,
                     )],
             );
@@ -1176,26 +1179,26 @@
                     -self.fc_kw_gap_fr_eff[i] / self.veh.mc_full_eff_array.last().unwrap();
             } else {
                 self.mc_elec_in_kw_for_max_fc_eff[i] = -self.fc_kw_gap_fr_eff[i]
                     / self.veh.mc_full_eff_array[cmp::max(
                         1,
                         first_grtr(
                             &self.veh.mc_kw_out_array,
-                            min(self.veh.mc_max_kw - 0.01, self.fc_kw_gap_fr_eff[i]),
+                            min(self.veh.mc_max_kw * 0.9999, self.fc_kw_gap_fr_eff[i]),
                         )
-                        .unwrap_or(0)
+                        .unwrap()
                             - 1,
                     )];
             }
         } else if self.fc_kw_gap_fr_eff[i] == self.veh.mc_max_kw {
             self.mc_elec_in_kw_for_max_fc_eff[i] = *self.veh.mc_kw_in_array.last().unwrap();
         } else {
             self.mc_elec_in_kw_for_max_fc_eff[i] = self.veh.mc_kw_in_array[first_grtr(
                 &self.veh.mc_kw_out_array,
-                min(self.veh.mc_max_kw - 0.01, self.fc_kw_gap_fr_eff[i]),
+                min(self.veh.mc_max_kw * 0.9999, self.fc_kw_gap_fr_eff[i]),
             )
             .unwrap_or(0)
                 - 1];
         }
         if self.veh.no_elec_sys {
             self.elec_kw_req_4ae[i] = 0.0;
         } else if self.trans_kw_in_ach[i] > 0.0 {
@@ -1205,17 +1208,17 @@
                     + self.aux_in_kw[i];
             } else {
                 self.elec_kw_req_4ae[i] = self.trans_kw_in_ach[i]
                     / self.veh.mc_full_eff_array[cmp::max(
                         1,
                         first_grtr(
                             &self.veh.mc_kw_out_array,
-                            min(self.veh.mc_max_kw - 0.01, self.trans_kw_in_ach[i]),
+                            min(self.veh.mc_max_kw * 0.9999, self.trans_kw_in_ach[i]),
                         )
-                        .unwrap_or(0)
+                        .unwrap()
                             - 1,
                     )]
                     + self.aux_in_kw[i];
             }
         } else {
             self.elec_kw_req_4ae[i] = 0.0;
         }
@@ -1465,37 +1468,37 @@
             } else {
                 self.mc_kw_if_fc_req[i] = self.mc_elec_kw_in_if_fc_req[i]
                     * self.veh.mc_full_eff_array[cmp::max(
                         1,
                         first_grtr(
                             &self.veh.mc_kw_in_array,
                             min(
-                                arrmax(&self.veh.mc_kw_in_array) - 0.01,
+                                arrmax(&self.veh.mc_kw_in_array) * 0.9999,
                                 self.mc_elec_kw_in_if_fc_req[i],
                             ),
                         )
-                        .unwrap_or(0)
+                        .unwrap()
                             - 1,
                     )]
             }
         } else if -self.mc_elec_kw_in_if_fc_req[i] == arrmax(&self.veh.mc_kw_in_array) {
             self.mc_kw_if_fc_req[i] =
                 self.mc_elec_kw_in_if_fc_req[i] / self.veh.mc_full_eff_array.last().unwrap();
         } else {
             self.mc_kw_if_fc_req[i] = self.mc_elec_kw_in_if_fc_req[i]
                 / self.veh.mc_full_eff_array[cmp::max(
                     1,
                     first_grtr(
                         &self.veh.mc_kw_in_array,
                         min(
-                            arrmax(&self.veh.mc_kw_in_array) - 0.01,
+                            arrmax(&self.veh.mc_kw_in_array) * 0.9999,
                             -self.mc_elec_kw_in_if_fc_req[i],
                         ),
                     )
-                    .unwrap_or(0)
+                    .unwrap()
                         - 1,
                 )];
         }
 
         if self.veh.mc_max_kw == 0.0 {
             self.mc_mech_kw_out_ach[i] = 0.0;
         } else if self.fc_forced_on[i]
@@ -1536,34 +1539,34 @@
             } else {
                 self.mc_elec_kw_in_ach[i] = self.mc_mech_kw_out_ach[i]
                     * self.veh.mc_full_eff_array[cmp::max(
                         1,
                         first_grtr(
                             &self.veh.mc_kw_in_array,
                             min(
-                                arrmax(&self.veh.mc_kw_in_array) - 0.01,
+                                arrmax(&self.veh.mc_kw_in_array) * 0.9999,
                                 -self.mc_mech_kw_out_ach[i],
                             ),
                         )
-                        .unwrap_or(0)
+                        .unwrap()
                             - 1,
                     )];
             }
         } else if self.veh.mc_max_kw == self.mc_mech_kw_out_ach[i] {
             self.mc_elec_kw_in_ach[i] =
                 self.mc_mech_kw_out_ach[i] / self.veh.mc_full_eff_array.last().unwrap()
         } else {
             self.mc_elec_kw_in_ach[i] = self.mc_mech_kw_out_ach[i]
                 / self.veh.mc_full_eff_array[cmp::max(
                     1,
                     first_grtr(
                         &self.veh.mc_kw_out_array,
-                        min(self.veh.mc_max_kw - 0.01, self.mc_mech_kw_out_ach[i]),
+                        min(self.veh.mc_max_kw * 0.9999, self.mc_mech_kw_out_ach[i]),
                     )
-                    .unwrap_or(0)
+                    .unwrap()
                         - 1,
                 )];
         }
 
         if self.cur_max_roadway_chg_kw[i] == 0.0 {
             self.roadway_chg_kw_out_ach[i] = 0.0
         } else if self.veh.fc_eff_type == H2FC {
@@ -1686,24 +1689,24 @@
         if self.fc_kw_out_ach[i] == 0.0 {
             self.fc_kw_in_ach[i] = 0.0;
             self.fc_kw_out_ach_pct[i] = 0.0;
         } else if self.veh.fc_eff_array[first_grtr(
             &self.veh.fc_kw_out_array,
             min(self.fc_kw_out_ach[i], self.veh.fc_max_kw),
         )
-        .unwrap_or(0)
+        .unwrap()
             - 1]
             != 0.0
         {
             self.fc_kw_in_ach[i] = self.fc_kw_out_ach[i]
                 / (self.veh.fc_eff_array[first_grtr(
                     &self.veh.fc_kw_out_array,
                     min(self.fc_kw_out_ach[i], self.veh.fc_max_kw),
                 )
-                .unwrap_or(0)
+                .unwrap()
                     - 1]);
         } else {
             self.fc_kw_in_ach[i] = 0.0
         }
 
         self.fs_kw_out_ach[i] = self.fc_kw_in_ach[i];
 
@@ -1788,15 +1791,15 @@
             / 1_000.0;
 
         self.energy_audit_error =
             ((self.roadway_chg_kj + self.ess_dischg_kj + self.fuel_kj + self.ke_kj) - self.net_kj)
                 / (self.roadway_chg_kj + self.ess_dischg_kj + self.fuel_kj + self.ke_kj);
 
         if self.energy_audit_error.abs() > self.sim_params.energy_audit_error_tol {
-            log::warn!(target: "fastsimrust",
+            log::warn!(
                 "problem detected with conservation of energy; \
                     energy audit error: {:.5}",
                 self.energy_audit_error
             );
         }
         for i in 1..self.cyc.len() {
             self.accel_kw[i] = self.veh.veh_kg / (2.0 * self.cyc.dt_s_at_i(i))
@@ -1814,34 +1817,34 @@
         self.trace_miss_time_frac = (self.cyc.time_s.last().unwrap()
             - self.cyc0.time_s.last().unwrap())
             / self.cyc0.time_s.last().unwrap();
 
         if !self.sim_params.missed_trace_correction {
             if self.trace_miss_dist_frac > self.sim_params.trace_miss_dist_tol {
                 self.trace_miss = true;
-                log::warn!(target: "fastsimrust",
+                log::warn!(
                     "trace miss distance fraction {:.5} exceeds tolerance of {:.5}",
                     self.trace_miss_dist_frac,
                     self.sim_params.trace_miss_dist_tol
                 );
             }
         } else if self.trace_miss_time_frac > self.sim_params.trace_miss_time_tol {
             self.trace_miss = true;
-            log::warn!(target: "fastsimrust",
+            log::warn!(
                 "trace miss time fraction {:.5} exceeds tolerance of {:.5}",
                 self.trace_miss_time_frac,
                 self.sim_params.trace_miss_time_tol
             );
         }
 
         self.trace_miss_speed_mps =
             ndarrmax(&(self.mps_ach.clone() - self.cyc.mps.clone()).map(|x| x.abs()));
         if self.trace_miss_speed_mps > self.sim_params.trace_miss_speed_mps_tol {
             self.trace_miss = true;
-            log::warn!(target: "fastsimrust",
+            log::warn!(
                 "trace miss speed {:.5} m/s exceeds tolerance of {:.5} m/s",
                 self.trace_miss_speed_mps,
                 self.sim_params.trace_miss_speed_mps_tol
             );
         }
         Ok(())
     }
```

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/simdrive.rs` & `fastsim-2.0.11/rust/fastsim-core/src/simdrive.rs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 use crate::cycle::{RustCycle, RustCycleCache};
 use crate::imports::*;
 use crate::params::RustPhysicalProperties;
 use crate::proc_macros::add_pyo3_api;
 #[cfg(feature = "pyo3")]
 use crate::pyo3imports::*;
 use crate::vehicle::*;
-pub mod simdrive_impl;
 pub mod cyc_mods;
+pub mod simdrive_impl;
 
 #[derive(Serialize, Deserialize, Debug, Clone, PartialEq)]
 #[add_pyo3_api(
     #[new]
     #[allow(clippy::too_many_arguments)]
     pub fn __new__(
         favor_grade_accuracy: bool,
```

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/simdrivelabel.rs` & `fastsim-2.0.11/rust/fastsim-core/src/simdrivelabel.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     pub uf: f64,
     pub net_accel: f64,
     pub res_found: String,
     pub phev_calcs: Option<LabelFePHEV>,
     pub adj_cs_comb_mpgge: Option<f64>,
     pub adj_cd_comb_mpgge: Option<f64>,
     pub net_phev_cd_miles: Option<f64>,
+    pub trace_miss_speed_mph: f64,
 }
 
 #[derive(Default, Serialize, Deserialize, Clone, Debug, PartialEq, ApproxEq)]
 /// Label fuel economy values for a PHEV vehicle
 pub struct LabelFePHEV {
     pub regen_soc_buffer: f64,
     pub udds: PHEVCycleCalc,
@@ -104,14 +105,47 @@
     pub adj_kwh_per_mi: f64,
     pub adj_ess_kwh_per_mi: f64,
     pub delta_soc: f64,
     /// Total number of miles in charge depletion mode, assuming constant kWh_per_mi
     pub total_cd_miles: f64,
 }
 
+pub fn make_accel_trace() -> RustCycle {
+    let accel_cyc_secs = Array::range(0., 300., 0.1);
+    let mut accel_cyc_mps = Array::ones(accel_cyc_secs.len()) * 90.0 / MPH_PER_MPS;
+    accel_cyc_mps[0] = 0.0;
+
+    RustCycle::new(
+        accel_cyc_secs.to_vec(),
+        accel_cyc_mps.to_vec(),
+        Array::zeros(accel_cyc_secs.len()).to_vec(),
+        Array::zeros(accel_cyc_secs.len()).to_vec(),
+        String::from("accel"),
+    )
+}
+
+pub fn get_net_accel(
+    sd_accel: &mut RustSimDrive,
+    scenario_name: &String,
+) -> Result<f64, anyhow::Error> {
+    log::debug!("running `sim_drive_accel`");
+    sd_accel.sim_drive_accel(None, None)?;
+    if sd_accel.mph_ach.iter().any(|&x| x >= 60.) {
+        Ok(interpolate(
+            &60.,
+            &sd_accel.mph_ach,
+            &sd_accel.cyc0.time_s,
+            false,
+        ))
+    } else {
+        log::warn!("vehicle '{}' never achieves 60 mph", scenario_name);
+        Ok(1e3)
+    }
+}
+
 pub fn get_label_fe(
     veh: &vehicle::RustVehicle,
     full_detail: Option<bool>,
     verbose: Option<bool>,
 ) -> Result<(LabelFe, Option<HashMap<&str, RustSimDrive>>), anyhow::Error> {
     // Generates label fuel economy (FE) values for a provided vehicle.
     //
@@ -129,32 +163,20 @@
     let sim_params: RustSimDriveParams = RustSimDriveParams::default();
     let props: RustPhysicalProperties = RustPhysicalProperties::default();
     let long_params: RustLongParams = RustLongParams::default();
 
     let mut cyc: HashMap<&str, RustCycle> = HashMap::new();
     let mut sd: HashMap<&str, RustSimDrive> = HashMap::new();
     let mut out: LabelFe = LabelFe::default();
+    let mut max_trace_miss_in_mph: f64 = 0.0;
 
     out.veh = veh.clone();
 
     // load the cycles and intstantiate simdrive objects
-    let accel_cyc_secs = Array::range(0., 300., 0.1);
-    let mut accel_cyc_mps = Array::ones(accel_cyc_secs.len()) * 90.0 / MPH_PER_MPS;
-    accel_cyc_mps[0] = 0.0;
-
-    cyc.insert(
-        "accel",
-        RustCycle::new(
-            accel_cyc_secs.to_vec(),
-            accel_cyc_mps.to_vec(),
-            Array::zeros(accel_cyc_secs.len()).to_vec(),
-            Array::zeros(accel_cyc_secs.len()).to_vec(),
-            String::from("accel"),
-        ),
-    );
+    cyc.insert("accel", make_accel_trace());
 
     #[cfg(not(windows))]
     macro_rules! main_separator {
         () => {
             "/"
         };
     }
@@ -206,17 +228,25 @@
         RustCycle::from_csv_string(hwy_filestring, "hwfet".to_string())?,
     );
 
     // run simdrive for non-phev powertrains
     sd.insert("udds", RustSimDrive::new(cyc["udds"].clone(), veh.clone()));
     sd.insert("hwy", RustSimDrive::new(cyc["hwy"].clone(), veh.clone()));
 
-    for (_, val) in sd.iter_mut() {
+    for (k, val) in sd.iter_mut() {
         val.sim_drive(None, None)?;
+        let key = String::from(k.clone());
+        let trace_miss_speed_mph = val.trace_miss_speed_mps * MPH_PER_MPS;
+        if (key == String::from("udds") || key == String::from("hwy"))
+            && trace_miss_speed_mph > max_trace_miss_in_mph
+        {
+            max_trace_miss_in_mph = trace_miss_speed_mph;
+        }
     }
+    out.trace_miss_speed_mph = max_trace_miss_in_mph;
 
     // find year-based adjustment parameters
     let adj_params: &AdjCoef = if veh.veh_year < 2017 {
         &long_params.ld_fe_adj_coef.adj_coef_map["2008"]
     } else {
         // assume 2017 coefficients are valid
         &long_params.ld_fe_adj_coef.adj_coef_map["2017"]
@@ -357,33 +387,17 @@
         out.net_range_miles = (veh.fs_kwh / props.kwh_per_gge
             - out.net_phev_cd_miles.unwrap() / out.adj_cd_comb_mpgge.unwrap())
             * out.adj_cs_comb_mpgge.unwrap()
             + out.net_phev_cd_miles.unwrap();
     }
 
     // run accelerating sim_drive
-    sd.insert(
-        "accel",
-        RustSimDrive::new(cyc["accel"].clone(), veh.clone()),
-    );
-    if let Some(sd_accel) = sd.get_mut("accel") {
-        log::debug!(target: "fastsimrust",
-            "running `sim_drive_accel`"
-        );
-        sd_accel.sim_drive_accel(None, None)?;
-    }
-    if sd["accel"].mph_ach.iter().any(|&x| x >= 60.) {
-        out.net_accel = interpolate(&60., &sd["accel"].mph_ach, &cyc["accel"].time_s, false);
-    } else {
-        // in case vehicle never exceeds 60 mph, penalize it a lot with a high number
-        log::warn!(target: "fastsimrust",
-            "vehicle '{}' never achieves 60 mph", veh.scenario_name
-        );
-        out.net_accel = 1e3;
-    }
+    let mut sd_accel = RustSimDrive::new(cyc["accel"].clone(), veh.clone());
+    out.net_accel = get_net_accel(&mut sd_accel, &veh.scenario_name)?;
+    sd.insert("accel", sd_accel);
 
     // success Boolean -- did all of the tests work(e.g. met trace within ~2 mph)?
     out.res_found = String::from("model needs to be implemented for this"); // this may need fancier logic than just always being true
 
     if full_detail.unwrap_or(false) && verbose.unwrap_or(false) {
         println!("{:#?}", out);
         return Ok((out, Some(sd)));
@@ -728,14 +742,15 @@
             uf: 0.,
             net_accel: 9.451683946821882,
             res_found: String::from("model needs to be implemented for this"),
             phev_calcs: None,
             adj_cs_comb_mpgge: None,
             adj_cd_comb_mpgge: None,
             net_phev_cd_miles: None,
+            trace_miss_speed_mph: 0.0,
         };
 
         println!(
             "Percent diff to Python calc: {:.3}%",
             100. * (label_fe_truth.net_accel - label_fe.net_accel) / label_fe_truth.net_accel
         );
 
@@ -1044,12 +1059,13 @@
             // net_accel: 7.962519496024332, <- Correct accel value
             net_accel: 1000.,
             res_found: String::from("model needs to be implemented for this"),
             phev_calcs: Some(phev_calcs),
             adj_cs_comb_mpgge: Some(45.06826741586106),
             adj_cd_comb_mpgge: Some(2293.5675017498143),
             net_phev_cd_miles: Some(57.04992781503185),
+            trace_miss_speed_mph: 0.0,
         };
 
         assert!(label_fe.approx_eq(&label_fe_truth, 1e-8));
     }
 }
```

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/thermal.rs` & `fastsim-2.0.11/rust/fastsim-core/src/thermal.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/traits.rs` & `fastsim-2.0.11/rust/fastsim-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/utils.rs` & `fastsim-2.0.11/rust/fastsim-core/src/utils.rs`

 * *Files 17% similar despite different names*

```diff
@@ -159,14 +159,62 @@
             yl = yr;
         }
     }
     let dydx = (yr - yl) / (xr - xl);
     yl + dydx * (x - xl)
 }
 
+/// interpolation algorithm from <http://www.cplusplus.com/forum/general/216928/>
+/// Arguments:
+/// x : value at which to interpolate
+pub fn interpolate_vectors(
+    x: &f64,
+    x_data_in: &Vec<f64>,
+    y_data_in: &Vec<f64>,
+    extrapolate: bool,
+) -> f64 {
+    assert!(x_data_in.len() == y_data_in.len());
+    let mut new_x_data: Vec<f64> = Vec::new();
+    let mut new_y_data: Vec<f64> = Vec::new();
+    let mut last_x = x_data_in[0];
+    for idx in 0..x_data_in.len() {
+        if idx == 0 || (idx > 0 && x_data_in[idx] > last_x) {
+            last_x = x_data_in[idx];
+            new_x_data.push(x_data_in[idx]);
+            new_y_data.push(y_data_in[idx]);
+        }
+    }
+    let x_data = new_x_data;
+    let y_data = new_y_data;
+    let size = x_data.len();
+
+    let mut i = 0;
+    if x >= &x_data[size - 2] {
+        i = size - 2;
+    } else {
+        while x > &x_data[i + 1] {
+            i += 1;
+        }
+    }
+    let xl = &x_data[i];
+    let mut yl = &y_data[i];
+    let xr = &x_data[i + 1];
+    let mut yr = &y_data[i + 1];
+    if !extrapolate {
+        if x < xl {
+            yr = yl;
+        }
+        if x > xr {
+            yl = yr;
+        }
+    }
+    let dydx = (yr - yl) / (xr - xl);
+    yl + dydx * (x - xl)
+}
+
 #[cfg(feature = "pyo3")]
 pub mod array_wrappers {
     use proc_macros::add_pyo3_api;
 
     use super::*;
     /// Helper struct to allow Rust to return a Python class that will indicate to the user that it's a clone.  
     #[add_pyo3_api]
@@ -299,59 +347,83 @@
     fn test_that_interpolation_works() {
         let xs = Array1::from_vec(vec![0.0, 1.0, 2.0, 3.0, 4.0]);
         let ys = Array1::from_vec(vec![0.0, 10.0, 20.0, 30.0, 40.0]);
         let x = 0.5;
         let y_lookup = interpolate(&x, &xs, &ys, false);
         let expected_y_lookup = 5.0;
         assert_eq!(expected_y_lookup, y_lookup);
+        let y_lookup = interpolate_vectors(&x, &xs.to_vec(), &ys.to_vec(), false);
+        assert_eq!(expected_y_lookup, y_lookup);
     }
 
     #[test]
     fn test_that_interpolation_works_for_irrational_number() {
         let xs = Array1::from_vec(vec![0.0, 1.0, 2.0, 3.0, 4.0]);
         let ys = Array1::from_vec(vec![0.0, 10.0, 20.0, 30.0, 40.0]);
         let x = 1.0 / 3.0;
         let y_lookup = interpolate(&x, &xs, &ys, false);
         let expected_y_lookup = 3.3333333333;
         assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
+        let y_lookup = interpolate_vectors(&x, &xs.to_vec(), &ys.to_vec(), false);
+        assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
     }
 
     #[test]
     fn test_interpolate_with_small_vectors() {
         let xs = Array1::from_vec(vec![0.0, 1.0]);
         let ys = Array1::from_vec(vec![0.0, 10.0]);
         let x = 0.5;
         let y_lookup = interpolate(&x, &xs, &ys, false);
         let expected_y_lookup = 5.0;
         assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
+        let y_lookup = interpolate_vectors(&x, &xs.to_vec(), &ys.to_vec(), false);
+        assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
     }
 
     #[test]
     fn test_interpolate_when_lookup_is_at_end() {
         let xs = Array1::from_vec(vec![0.0, 1.0]);
         let ys = Array1::from_vec(vec![0.0, 10.0]);
         let x = 1.0;
         let y_lookup = interpolate(&x, &xs, &ys, false);
         let expected_y_lookup = 10.0;
         assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
+        let y_lookup = interpolate_vectors(&x, &xs.to_vec(), &ys.to_vec(), false);
+        assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
     }
 
     #[test]
     fn test_interpolate_when_lookup_is_past_end_without_extrapolate() {
         let xs = Array1::from_vec(vec![0.0, 1.0]);
         let ys = Array1::from_vec(vec![0.0, 10.0]);
         let x = 1.01;
         let y_lookup = interpolate(&x, &xs, &ys, false);
         let expected_y_lookup = 10.0;
         assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
+        let y_lookup = interpolate_vectors(&x, &xs.to_vec(), &ys.to_vec(), false);
+        assert!((expected_y_lookup - y_lookup).abs() < 1e-6);
     }
 
     #[test]
     fn test_interpolate_with_x_data_that_repeats() {
         let xs = Array1::from_vec(vec![0.0, 1.0, 1.0]);
         let ys = Array1::from_vec(vec![0.0, 10.0, 10.0]);
         let x = 1.0;
         let y_lookup = interpolate(&x, &xs, &ys, false);
         let expected_y_lookup = 10.0;
         assert_eq!(expected_y_lookup, y_lookup);
+        let y_lookup = interpolate_vectors(&x, &xs.to_vec(), &ys.to_vec(), false);
+        assert_eq!(expected_y_lookup, y_lookup);
+    }
+
+    #[test]
+    fn test_interpolate_with_non_evenly_spaced_x_data() {
+        let xs = Array1::from_vec(vec![0.0, 10.0, 100.0, 1000.0]);
+        let ys = Array1::from_vec(vec![0.0, 1.0, 2.0, 3.0]);
+        let x = 55.0;
+        let y_lookup = interpolate(&x, &xs, &ys, false);
+        let expected_y_lookup = 1.5;
+        assert_eq!(expected_y_lookup, y_lookup);
+        let y_lookup = interpolate_vectors(&x, &xs.to_vec(), &ys.to_vec(), false);
+        assert_eq!(expected_y_lookup, y_lookup);
     }
 }
```

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/vehicle.rs` & `fastsim-2.0.11/rust/fastsim-core/src/vehicle.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/vehicle_thermal.rs` & `fastsim-2.0.11/rust/fastsim-core/src/vehicle_thermal.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-core/src/vehicle_utils.rs` & `fastsim-2.0.11/rust/fastsim-core/src/vehicle_utils.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-py/Cargo.toml` & `fastsim-2.0.11/rust/fastsim-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/rust/fastsim-py/src/lib.rs` & `fastsim-2.0.11/rust/fastsim-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.10/setup.py` & `fastsim-2.0.11/setup.py`

 * *Files identical despite different names*

