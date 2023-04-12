# Comparing `tmp/fastsim-2.0.15.tar.gz` & `tmp/fastsim-2.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsim-2.0.15.tar", last modified: Wed Apr 12 18:27:56 2023, max compression
+gzip compressed data, was "fastsim-2.0.16.tar", last modified: Wed Apr 12 20:07:24 2023, max compression
```

## Comparing `fastsim-2.0.15.tar` & `fastsim-2.0.16.tar`

### file list

```diff
@@ -1,265 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.125244 fastsim-2.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 18:27:45.000000 fastsim-2.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 18:27:45.000000 fastsim-2.0.15/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-12 18:27:45.000000 fastsim-2.0.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-04-12 18:27:56.125244 fastsim-2.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-12 18:27:45.000000 fastsim-2.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.077244 fastsim-2.0.15/fastsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    37910 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.081244 fastsim-2.0.15/fastsim/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/2017_Ford_F150_thermal_val.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/accel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/demo_abc_drag_coef_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/demo_eu_vehicle_wltp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/fusion_thermal_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/fusion_thermal_cal_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/fusion_thermal_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/mp_parallel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/stop_start_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/time_dilation_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/docs/wltc_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/inspect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.081244 fastsim-2.0.15/fastsim/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/FASTSim_py_veh_db.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.085244 fastsim-2.0.15/fastsim/resources/cycles/
--rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/NREL13.csv
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/accel.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.073244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.085244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.089244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/
--rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
--rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.089244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4105836_2/
--rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.093244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/
--rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.097244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/
--rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.097244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/
--rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.101244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/
--rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.101244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/
--rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.101244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4112082_1/
--rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
--rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.101244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4113492_1/
--rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.105244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4114555_1/
--rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.105244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_1/
--rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.105244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_2/
--rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.105244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115957_1/
--rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.105244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115985_1/
--rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.105244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116361_1/
--rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.109244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116721_2/
--rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.109244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116728_1/
--rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.109244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_1/
--rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.109244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_2/
--rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.109244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116880_1/
--rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.109244 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4118093_1/
--rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
--rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/ftpmc1b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/hwfet.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/longHaulDriveCycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/udds.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/us06.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_extra_high3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_high3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_high3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_low3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_med3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_med3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wmtc_all.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wmtc_part1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wmtc_part2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/cycles/wmtc_part3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/longparams.json
--rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/master_benchmark_vars.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/res_excel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.117244 fastsim-2.0.15/fastsim/resources/vehdb/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Focus.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Focus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Fusion.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/Class_4_Box_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/Line_Haul_Conv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/Line_Haul_Conv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/fail_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/fail_overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/legacy_template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/legacy_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/test_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/test_overrides.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.117244 fastsim-2.0.15/fastsim/resources/vehdb/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/rustext.py
--rw-r--r--   0 runner    (1001) docker     (123)   116204 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/simdrivelabel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.121244 fastsim-2.0.15/fastsim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    60185 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_coasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_eco_cruise.py
--rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_following.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_rust.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_simdrive_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_soc_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/tests/test_vs_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim/vehicle_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-04-12 18:27:45.000000 fastsim-2.0.15/fastsim-icon-web-131x172.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.077244 fastsim-2.0.15/fastsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-04-12 18:27:56.000000 fastsim-2.0.15/fastsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-04-12 18:27:56.000000 fastsim-2.0.15/fastsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:27:56.000000 fastsim-2.0.15/fastsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:27:56.000000 fastsim-2.0.15/fastsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 18:27:56.000000 fastsim-2.0.15/fastsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 18:27:56.000000 fastsim-2.0.15/fastsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 18:27:45.000000 fastsim-2.0.15/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.121244 fastsim-2.0.15/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.121244 fastsim-2.0.15/rust/fastsim-core/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.121244 fastsim-2.0.15/rust/fastsim-core/proc-macros/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/proc-macros/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.121244 fastsim-2.0.15/rust/fastsim-core/proc-macros/src/
--rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/proc-macros/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/proc-macros/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/proc-macros/src/utilities.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.125244 fastsim-2.0.15/rust/fastsim-core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/air.rs
--rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/cycle.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.125244 fastsim-2.0.15/rust/fastsim-core/src/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/html/docs-header.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/macros.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/params.rs
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/pyo3imports.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.125244 fastsim-2.0.15/rust/fastsim-core/src/simdrive/
--rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/simdrive/cyc_mods.rs
--rw-r--r--   0 runner    (1001) docker     (123)    77871 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/simdrive/simdrive_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/simdrive.rs
--rw-r--r--   0 runner    (1001) docker     (123)    41697 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/simdrivelabel.rs
--rw-r--r--   0 runner    (1001) docker     (123)    48266 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/traits.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/vehicle.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/vehicle_thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-core/src/vehicle_utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.125244 fastsim-2.0.15/rust/fastsim-py/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:27:56.125244 fastsim-2.0.15/rust/fastsim-py/src/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 18:27:45.000000 fastsim-2.0.15/rust/fastsim-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:27:56.125244 fastsim-2.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 18:27:45.000000 fastsim-2.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.675909 fastsim-2.0.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 20:07:12.000000 fastsim-2.0.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 20:07:12.000000 fastsim-2.0.16/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-12 20:07:12.000000 fastsim-2.0.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-12 20:07:24.675909 fastsim-2.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-04-12 20:07:12.000000 fastsim-2.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.627907 fastsim-2.0.16/fastsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/auxiliaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37910 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/cycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.627907 fastsim-2.0.16/fastsim/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/2017_Ford_F150_thermal_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/accel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/cav_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/cav_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/demo_abc_drag_coef_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/demo_eu_vehicle_wltp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/fusion_thermal_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/fusion_thermal_cal_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/fusion_thermal_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/mp_parallel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/stop_start_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/time_dilation_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/docs/wltc_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/inspect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.631907 fastsim-2.0.16/fastsim/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/FASTSim_py_veh_db.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.635907 fastsim-2.0.16/fastsim/resources/cycles/
+-rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/NREL13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/accel.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.619907 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.635907 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.635907 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/
+-rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.639907 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4105836_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.639907 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.647908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/
+-rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.647908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.651908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.651908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.651908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4112082_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.651908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4113492_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.655908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4114555_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.655908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.655908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.655908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115957_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.655908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115985_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.659908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116361_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.659908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116721_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.659908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116728_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.659908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.659908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.659908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116880_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.659908 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4118093_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/ftpmc1b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/hwfet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/longHaulDriveCycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/udds.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/us06.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_extra_high3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_high3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_high3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_low3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_med3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_med3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wmtc_all.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wmtc_part1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wmtc_part2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/cycles/wmtc_part3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/longparams.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/master_benchmark_vars.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/res_excel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.667908 fastsim-2.0.16/fastsim/resources/vehdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Focus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Focus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Fusion.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/Class_4_Box_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/Line_Haul_Conv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/Line_Haul_Conv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/fail_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/fail_overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/legacy_template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/legacy_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/test_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/test_overrides.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.667908 fastsim-2.0.16/fastsim/resources/vehdb/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/rustext.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116204 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/simdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/simdrivelabel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.671908 fastsim-2.0.16/fastsim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_auxiliaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_cav_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_cav_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60185 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_coasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_eco_cruise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_following.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_rust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_simdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_simdrive_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_soc_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/tests/test_vs_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-12 20:07:12.000000 fastsim-2.0.16/fastsim/vehicle_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.627907 fastsim-2.0.16/fastsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-12 20:07:24.000000 fastsim-2.0.16/fastsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-12 20:07:24.000000 fastsim-2.0.16/fastsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:07:24.000000 fastsim-2.0.16/fastsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:07:24.000000 fastsim-2.0.16/fastsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 20:07:24.000000 fastsim-2.0.16/fastsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 20:07:24.000000 fastsim-2.0.16/fastsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 20:07:12.000000 fastsim-2.0.16/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.671908 fastsim-2.0.16/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.671908 fastsim-2.0.16/rust/fastsim-core/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.671908 fastsim-2.0.16/rust/fastsim-core/proc-macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/proc-macros/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.671908 fastsim-2.0.16/rust/fastsim-core/proc-macros/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/proc-macros/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/proc-macros/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/proc-macros/src/utilities.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.675909 fastsim-2.0.16/rust/fastsim-core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/air.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/cycle.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.675909 fastsim-2.0.16/rust/fastsim-core/src/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/html/docs-header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/pyo3imports.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.675909 fastsim-2.0.16/rust/fastsim-core/src/simdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/simdrive/cyc_mods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    77871 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/simdrive/simdrive_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/simdrive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    41697 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/simdrivelabel.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    48266 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/vehicle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/vehicle_thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-core/src/vehicle_utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.675909 fastsim-2.0.16/rust/fastsim-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:24.675909 fastsim-2.0.16/rust/fastsim-py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 20:07:12.000000 fastsim-2.0.16/rust/fastsim-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:07:24.675909 fastsim-2.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 20:07:12.000000 fastsim-2.0.16/setup.py
```

### Comparing `fastsim-2.0.15/LICENSE` & `fastsim-2.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/LICENSE.md` & `fastsim-2.0.16/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/PKG-INFO` & `fastsim-2.0.16/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsim
-Version: 2.0.15
+Version: 2.0.16
 Summary: Tool for modeling vehicle powertrains
 Author-email: NREL/MTES/CIMS/MBAP Group <fastsim@nrel.gov>
 License: Future Automotive Systems Technology Simulator (FASTSim(TM)) Copyright (c) 2020 Alliance for Sustainable Energy, LLC All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -26,112 +26,79 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: LICENSE.md
 
-![FASTSim Logo](fastsim-icon-web-131x172.jpg)
+![FASTSim Logo](fastsim/docs/fastsim-icon-web-131x172.jpg)
 
 # Description
-This is the python/rust flavor of [NREL's FASTSim](https://www.nrel.gov/transportation/fastsim.html), which is based on the original Excel implementation. Effort will be made to keep the core methodology between this software and the Excel flavor in line with one another. Other FASTSim flavors may spin off as variations on this core functionality, but these should integrated back into `main` if there is any intent of persistence.
+This is the python/rust flavor of [NREL's FASTSim](https://www.nrel.gov/transportation/fastsim.html), which is based on the original Excel implementation. Effort will be made to keep the core methodology between this software and the Excel flavor in line with one another. 
 
 All classes and methods are self-documented.  
 
 # Installation
 
-## PyPI Installation
+## Python 
+Set up and activate a python environment (compatible with Python 3.8 - 3.10; we recommend Python 3.10) with the following steps.
+### [Anaconda](https://www.anaconda.com/) 
+1. Create: `conda create -n fastsim python=3.10`
+1. Activate: `conda activate fastsim`
+
+### [venv](https://docs.python.org/3/library/venv.html)
+There is some variation based on your Operating System:  
+
+- PowerShell (windows):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `fastsim-venv/Scripts/Activate.ps1`
+
+- Bash (i.e. unix/linux/mac):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `source fastsim-venv/bin/activate`
+
+- Command Prompt (windows):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `fastsim-venv/Scripts/activate.bat`
 
+## FASTSim
+### Via PyPI
 In an active Python environment (either [venv](https://docs.python.org/3/library/venv.html) or [Conda](https://www.anaconda.com/)), run `pip install fastsim`.
 
-## Installing from NREL's internal GitHub
-
-1. Clone the repository from GitHub:
-
-       git clone git@github.nrel.gov:MBAP/fastsim.git
-
-2. Set up an environment for the project. There are two ways to do this:
-
-   - Using Anaconda (with Python 3.8 or newer):
-
-         conda create -n fastsim python=3.8
-         conda activate fastsim
-         conda install -c conda-forge "rust>=1.64"
-
-   - Manually:
-     - Install [Rust](https://www.rust-lang.org/tools/install). 
-     - Then, using a virtual environment, and making sure to use Python >= 3.8:
-    
-        PowerShell:
-
-            python -m venv .venv
-            .venv/Scripts/Activate.ps1
-
-        Bash:
-
-            python -m venv .venv
-            source .venv/bin/activate
-
-        Command Prompt:
-
-            python -m venv .venv
-            .venv/Scripts/activate.bat
-    
-3. From within the top level of the FASTSim repository, install using pip:
-
-       pip install .
-
-## Developers
+### Building from Scratch
 Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  
 
-To do this, a couple of extra steps are required:
-
-1. First install the python code in place `DEVELOP_MODE=True pip install -e ".[dev]"` if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
-1. Within the same python environment, navigate to `fastsim/rust/` and run `pip install maturin`.
-1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
-1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
+- Easy way: run `sh build_and_test.sh` in root folder.  
+- Hard way (a couple of extra steps are required): 
+    1. First install the python code in place:  
+    `DEVELOP_MODE=True pip install -e ".[dev]"`   
+    if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run  
+    `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
+    1. Within the same python environment, navigate to `fastsim/rust/` and run  
+    `pip install maturin`.
+    1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
+    1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
 
 After FASTSim has been installed as editable per the above instructions, you can rebuild and test everything with `sh build_and_test.sh` in Windows bash or `./build_and_test.sh` in Linux/Unix in the `fastsim/` dir.  
 
-# Users with NREL VPN Access
-## Installation as PyPi Package
-Note: the following instructions work only if you are inside NREL VPN:  
-To install and/or update, run
-```
-pip install fastsim --upgrade --extra-index-url=https://github.nrel.gov/pages/MBAP/mbap-pypi/
-```
-
-## Adding FASTSim as a Depency in Rust
-Add this line:  
-`fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
-to your Cargo.toml file, modifying the `branch` key as appropriate.  
+### Testing
+At the root level of the git repository: `pytest -v fastsim/tests/`.  This can also be run in the python environment directly.  
 
 # Usage
 To see and run examples, navigate to fastsim/docs and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
 
-To get help in an interactive ipython or jupyter session:  
-```
-import fastsim
-fastsim.simdrive.SimDriveClassic? # or
-help(fastsim.simdrive.SimDriveClassic)
-```
-
-Help can be used in this manner on any FASTSim object.
-
-# Testing
 
-The `unittest` package has been implemented such that you can run `python -m unittest discover` from within the fastsim folder, and all tests will be automatically discovered and run.  
-
-## Against Previous Python Version
-
-To run tests, first run the command `from fastim import tests`.  
-To compare FASTSim back to the master branch version from 17 December 2019, run `tests.test26veh3cyc.main()`.  For timing comparisons, run `tests.test26veh3cyc_CPUtime.main()`.  
+# Adding FASTSim as a Depency in Rust
+## Via GitHub
+Add this line:  
+`fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
+to your Cargo.toml file, modifying the `branch` key as appropriate.  
 
-## Against Excel FASTSim
-To compare Python FASTSim results to Excel FASTSim, you can run `tests.test_vs_excel.main()` to do an experimental (i.e. beta) comparison against saved Excel results. If you have the Excel version (obtainable here: [https://www.nrel.gov/transportation/fastsim.html](https://www.nrel.gov/transportation/fastsim.html)) of FASTSim open, you can specify `rerun_excel=True` to do a live run of the Excel version.
+## Via Cargo
+This has not been implemented yet.  
 
 # List of Abbreviations
 cur = current time step  
 prev = previous time step  
 cyc = drive cycle  
 secs = seconds  
 mps = meters per second  
@@ -151,16 +118,19 @@
 lim = limit of a component  
 regen = associated with regenerative braking  
 des = desired value  
 ach = achieved value  
 in = component input  
 out = component output  
 
+# Known Issues
+Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
+
 # Release Notes
-2.0.11 - 2.0.15 -- PyPI fixes  
+2.0.11 - 2.0.16 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`  
 2.0.3 -- exposed `veh.__post_init__`  
@@ -188,20 +158,20 @@
 1.0.0 -- Implemented unittest package.  Fixed energy audit calculations to be based on achieved speed.  Updated this file.  Improved documentation.  Vehicle can be instantiated as dict.   
 0.1.5 -- Updated to be compatible with ADOPT    
 0.1.4 -- Bug fix: `mcEffMap` is now robust to having zero as first element    
 0.1.3 -- Bug fix: `fastsim.vehicle.Vehicle` method `set_init_calcs` no longer overrides `fcEffMap`.    
 0.1.2 -- Fixes os-dependency of xlwings by not running stuff that needs xlwings.  Improvements in functional test.  Refinment utomated typying of jitclass objects.    
 0.1.1 -- Now includes label fuel economy and/or battery kW-hr/mi values that match excel and test for benchmarking against Excel values and CPU time.   
 
-# Contributors
+# Contributors  
 Chad Baker -- Chad.Baker@nrel.gov  
 Aaron Brooker -- Aaron.Brooker@nrel.gov  
-Kyle Carow -- Kyle.Carow@nrel.gov
+Kyle Carow -- Kyle.Carow@nrel.gov  
 Jeffrey Gonder -- Jeff.Gonder@nrel.gov  
 Jacob Holden -- Jacob.Holden@nrel.gov  
-Jinghu Hu -- Jinghu.Hu@nrel.gov
+Jinghu Hu -- Jinghu.Hu@nrel.gov  
 Jason Lustbader -- Jason.Lustbader@nrel.gov  
 Sean Lopp -- sean@rstudio.com  
 Matthew Moniot -- Matthew.Moniot@nrel.gov  
 Grant Payne -- Grant.Payne@nrel.gov  
 Laurie Ramroth -- lramroth@ford.com  
 Eric Wood -- Eric.Wood@nrel.gov
```

### Comparing `fastsim-2.0.15/README.md` & `fastsim-2.0.16/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,72 @@
-![FASTSim Logo](fastsim-icon-web-131x172.jpg)
+![FASTSim Logo](fastsim/docs/fastsim-icon-web-131x172.jpg)
 
 # Description
-This is the python/rust flavor of [NREL's FASTSim](https://www.nrel.gov/transportation/fastsim.html), which is based on the original Excel implementation. Effort will be made to keep the core methodology between this software and the Excel flavor in line with one another. Other FASTSim flavors may spin off as variations on this core functionality, but these should integrated back into `main` if there is any intent of persistence.
+This is the python/rust flavor of [NREL's FASTSim](https://www.nrel.gov/transportation/fastsim.html), which is based on the original Excel implementation. Effort will be made to keep the core methodology between this software and the Excel flavor in line with one another. 
 
 All classes and methods are self-documented.  
 
 # Installation
 
-## PyPI Installation
+## Python 
+Set up and activate a python environment (compatible with Python 3.8 - 3.10; we recommend Python 3.10) with the following steps.
+### [Anaconda](https://www.anaconda.com/) 
+1. Create: `conda create -n fastsim python=3.10`
+1. Activate: `conda activate fastsim`
+
+### [venv](https://docs.python.org/3/library/venv.html)
+There is some variation based on your Operating System:  
+
+- PowerShell (windows):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `fastsim-venv/Scripts/Activate.ps1`
+
+- Bash (i.e. unix/linux/mac):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `source fastsim-venv/bin/activate`
+
+- Command Prompt (windows):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `fastsim-venv/Scripts/activate.bat`
 
+## FASTSim
+### Via PyPI
 In an active Python environment (either [venv](https://docs.python.org/3/library/venv.html) or [Conda](https://www.anaconda.com/)), run `pip install fastsim`.
 
-## Installing from NREL's internal GitHub
-
-1. Clone the repository from GitHub:
-
-       git clone git@github.nrel.gov:MBAP/fastsim.git
-
-2. Set up an environment for the project. There are two ways to do this:
-
-   - Using Anaconda (with Python 3.8 or newer):
-
-         conda create -n fastsim python=3.8
-         conda activate fastsim
-         conda install -c conda-forge "rust>=1.64"
-
-   - Manually:
-     - Install [Rust](https://www.rust-lang.org/tools/install). 
-     - Then, using a virtual environment, and making sure to use Python >= 3.8:
-    
-        PowerShell:
-
-            python -m venv .venv
-            .venv/Scripts/Activate.ps1
-
-        Bash:
-
-            python -m venv .venv
-            source .venv/bin/activate
-
-        Command Prompt:
-
-            python -m venv .venv
-            .venv/Scripts/activate.bat
-    
-3. From within the top level of the FASTSim repository, install using pip:
-
-       pip install .
-
-## Developers
+### Building from Scratch
 Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  
 
-To do this, a couple of extra steps are required:
-
-1. First install the python code in place `DEVELOP_MODE=True pip install -e ".[dev]"` if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
-1. Within the same python environment, navigate to `fastsim/rust/` and run `pip install maturin`.
-1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
-1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
+- Easy way: run `sh build_and_test.sh` in root folder.  
+- Hard way (a couple of extra steps are required): 
+    1. First install the python code in place:  
+    `DEVELOP_MODE=True pip install -e ".[dev]"`   
+    if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run  
+    `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
+    1. Within the same python environment, navigate to `fastsim/rust/` and run  
+    `pip install maturin`.
+    1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
+    1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
 
 After FASTSim has been installed as editable per the above instructions, you can rebuild and test everything with `sh build_and_test.sh` in Windows bash or `./build_and_test.sh` in Linux/Unix in the `fastsim/` dir.  
 
-# Users with NREL VPN Access
-## Installation as PyPi Package
-Note: the following instructions work only if you are inside NREL VPN:  
-To install and/or update, run
-```
-pip install fastsim --upgrade --extra-index-url=https://github.nrel.gov/pages/MBAP/mbap-pypi/
-```
-
-## Adding FASTSim as a Depency in Rust
-Add this line:  
-`fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
-to your Cargo.toml file, modifying the `branch` key as appropriate.  
+### Testing
+At the root level of the git repository: `pytest -v fastsim/tests/`.  This can also be run in the python environment directly.  
 
 # Usage
 To see and run examples, navigate to fastsim/docs and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
 
-To get help in an interactive ipython or jupyter session:  
-```
-import fastsim
-fastsim.simdrive.SimDriveClassic? # or
-help(fastsim.simdrive.SimDriveClassic)
-```
-
-Help can be used in this manner on any FASTSim object.
-
-# Testing
 
-The `unittest` package has been implemented such that you can run `python -m unittest discover` from within the fastsim folder, and all tests will be automatically discovered and run.  
-
-## Against Previous Python Version
-
-To run tests, first run the command `from fastim import tests`.  
-To compare FASTSim back to the master branch version from 17 December 2019, run `tests.test26veh3cyc.main()`.  For timing comparisons, run `tests.test26veh3cyc_CPUtime.main()`.  
+# Adding FASTSim as a Depency in Rust
+## Via GitHub
+Add this line:  
+`fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
+to your Cargo.toml file, modifying the `branch` key as appropriate.  
 
-## Against Excel FASTSim
-To compare Python FASTSim results to Excel FASTSim, you can run `tests.test_vs_excel.main()` to do an experimental (i.e. beta) comparison against saved Excel results. If you have the Excel version (obtainable here: [https://www.nrel.gov/transportation/fastsim.html](https://www.nrel.gov/transportation/fastsim.html)) of FASTSim open, you can specify `rerun_excel=True` to do a live run of the Excel version.
+## Via Cargo
+This has not been implemented yet.  
 
 # List of Abbreviations
 cur = current time step  
 prev = previous time step  
 cyc = drive cycle  
 secs = seconds  
 mps = meters per second  
@@ -119,16 +86,19 @@
 lim = limit of a component  
 regen = associated with regenerative braking  
 des = desired value  
 ach = achieved value  
 in = component input  
 out = component output  
 
+# Known Issues
+Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
+
 # Release Notes
-2.0.11 - 2.0.15 -- PyPI fixes  
+2.0.11 - 2.0.16 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`  
 2.0.3 -- exposed `veh.__post_init__`  
@@ -156,20 +126,20 @@
 1.0.0 -- Implemented unittest package.  Fixed energy audit calculations to be based on achieved speed.  Updated this file.  Improved documentation.  Vehicle can be instantiated as dict.   
 0.1.5 -- Updated to be compatible with ADOPT    
 0.1.4 -- Bug fix: `mcEffMap` is now robust to having zero as first element    
 0.1.3 -- Bug fix: `fastsim.vehicle.Vehicle` method `set_init_calcs` no longer overrides `fcEffMap`.    
 0.1.2 -- Fixes os-dependency of xlwings by not running stuff that needs xlwings.  Improvements in functional test.  Refinment utomated typying of jitclass objects.    
 0.1.1 -- Now includes label fuel economy and/or battery kW-hr/mi values that match excel and test for benchmarking against Excel values and CPU time.   
 
-# Contributors
+# Contributors  
 Chad Baker -- Chad.Baker@nrel.gov  
 Aaron Brooker -- Aaron.Brooker@nrel.gov  
-Kyle Carow -- Kyle.Carow@nrel.gov
+Kyle Carow -- Kyle.Carow@nrel.gov  
 Jeffrey Gonder -- Jeff.Gonder@nrel.gov  
 Jacob Holden -- Jacob.Holden@nrel.gov  
-Jinghu Hu -- Jinghu.Hu@nrel.gov
+Jinghu Hu -- Jinghu.Hu@nrel.gov  
 Jason Lustbader -- Jason.Lustbader@nrel.gov  
 Sean Lopp -- sean@rstudio.com  
 Matthew Moniot -- Matthew.Moniot@nrel.gov  
 Grant Payne -- Grant.Payne@nrel.gov  
 Laurie Ramroth -- lramroth@ford.com  
 Eric Wood -- Eric.Wood@nrel.gov
```

### Comparing `fastsim-2.0.15/fastsim/__init__.py` & `fastsim-2.0.16/fastsim/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from . import auxiliaries
 
 from pkg_resources import get_distribution
 
 __version__ = get_distribution('fastsim').version
 
 __doc__ += "\nhttps://pypi.org/project/fastsim/"
+__doc__ += "\nhttps://www.nrel.gov/transportation/fastsim.html"
 
 try:
     import fastsimrust as fsr
 except ImportError:
     logger.warn("fastsimrust not installed")
 else:
     # Enable np.array() on array structs
```

### Comparing `fastsim-2.0.15/fastsim/auxiliaries.py` & `fastsim-2.0.16/fastsim/auxiliaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import matplotlib.pyplot as plt
 from typing import Tuple, List
 
 from fastsim.utilities import get_rho_air
 
 props = params.PhysicalProperties()
 R_air = 287  # J/(kg*K)
-
+    
 
 def abc_to_drag_coeffs(veh: Vehicle,
                        a_lbf: float, b_lbf__mph: float, c_lbf__mph2: float,
                        custom_rho: bool = False,
                        custom_rho_temp_degC: float = 20.,
                        custom_rho_elevation_m: float = 180.,
                        simdrive_optimize: bool = True,
```

### Comparing `fastsim-2.0.15/fastsim/calibration.py` & `fastsim-2.0.16/fastsim/calibration.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/cycle.py` & `fastsim-2.0.16/fastsim/cycle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/2017_Ford_F150_thermal_val.py` & `fastsim-2.0.16/fastsim/docs/2017_Ford_F150_thermal_val.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/accel_demo.py` & `fastsim-2.0.16/fastsim/docs/accel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/cav_demo.py` & `fastsim-2.0.16/fastsim/docs/cav_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/cav_sweep.py` & `fastsim-2.0.16/fastsim/docs/cav_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/demo.py` & `fastsim-2.0.16/fastsim/docs/demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/demo_abc_drag_coef_conv.py` & `fastsim-2.0.16/fastsim/docs/demo_abc_drag_coef_conv.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/demo_eu_vehicle_wltp.py` & `fastsim-2.0.16/fastsim/docs/demo_eu_vehicle_wltp.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/fusion_thermal_cal.py` & `fastsim-2.0.16/fastsim/docs/fusion_thermal_cal.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/fusion_thermal_cal_post.py` & `fastsim-2.0.16/fastsim/docs/fusion_thermal_cal_post.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/fusion_thermal_demo.py` & `fastsim-2.0.16/fastsim/docs/fusion_thermal_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/mp_parallel_demo.py` & `fastsim-2.0.16/fastsim/docs/mp_parallel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/stop_start_demo.py` & `fastsim-2.0.16/fastsim/docs/stop_start_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/time_dilation_demo.py` & `fastsim-2.0.16/fastsim/docs/time_dilation_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/docs/wltc_calibration.py` & `fastsim-2.0.16/fastsim/docs/wltc_calibration.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/inspect_utils.py` & `fastsim-2.0.16/fastsim/inspect_utils.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/parameters.py` & `fastsim-2.0.16/fastsim/parameters.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resample.py` & `fastsim-2.0.16/fastsim/resample.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/FASTSim_py_veh_db.csv` & `fastsim-2.0.16/fastsim/resources/FASTSim_py_veh_db.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/HHDDTCruiseSmooth.csv` & `fastsim-2.0.16/fastsim/resources/cycles/HHDDTCruiseSmooth.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/NREL13.csv` & `fastsim-2.0.16/fastsim/resources/cycles/NREL13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv` & `fastsim-2.0.16/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/accel.csv` & `fastsim-2.0.16/fastsim/resources/cycles/accel.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv` & `fastsim-2.0.16/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/ftpmc1b.csv` & `fastsim-2.0.16/fastsim/resources/cycles/ftpmc1b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/hwfet.csv` & `fastsim-2.0.16/fastsim/resources/cycles/hwfet.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/longHaulDriveCycle.csv` & `fastsim-2.0.16/fastsim/resources/cycles/longHaulDriveCycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/udds.csv` & `fastsim-2.0.16/fastsim/resources/cycles/udds.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/us06.csv` & `fastsim-2.0.16/fastsim/resources/cycles/us06.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_extra_high3.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_extra_high3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_high3a.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_high3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_high3b.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_high3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_low3.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_low3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_med3a.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_med3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wltc_class3_med3b.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wltc_class3_med3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wmtc_all.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wmtc_all.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wmtc_part1.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wmtc_part1.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wmtc_part2.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wmtc_part2.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/cycles/wmtc_part3.csv` & `fastsim-2.0.16/fastsim/resources/cycles/wmtc_part3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/longparams.json` & `fastsim-2.0.16/fastsim/resources/longparams.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/master_benchmark_vars.csv` & `fastsim-2.0.16/fastsim/resources/master_benchmark_vars.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/res_excel.json` & `fastsim-2.0.16/fastsim/resources/res_excel.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Focus.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Focus.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Focus.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Focus.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Fusion.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Fusion.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2012_Ford_Fusion.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2012_Ford_Fusion.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/Class_4_Box_Truck.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/Class_4_Box_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/Class_4_Box_Truck.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/Class_4_Box_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/Line_Haul_Conv.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/Line_Haul_Conv.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/Line_Haul_Conv.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/Line_Haul_Conv.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/fail_overrides.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/fail_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/fail_overrides.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/fail_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/legacy_template.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/legacy_template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/legacy_template.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/legacy_template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/template.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/template.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/test_overrides.csv` & `fastsim-2.0.16/fastsim/resources/vehdb/test_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/test_overrides.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/test_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml` & `fastsim-2.0.16/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/simdrive.py` & `fastsim-2.0.16/fastsim/simdrive.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/simdrivelabel.py` & `fastsim-2.0.16/fastsim/simdrivelabel.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_auxiliaries.py` & `fastsim-2.0.16/fastsim/tests/test_auxiliaries.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_cav_demo.py` & `fastsim-2.0.16/fastsim/tests/test_cav_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_cav_sweep.py` & `fastsim-2.0.16/fastsim/tests/test_cav_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_coasting.py` & `fastsim-2.0.16/fastsim/tests/test_coasting.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_copy.py` & `fastsim-2.0.16/fastsim/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_cycle.py` & `fastsim-2.0.16/fastsim/tests/test_cycle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_demo.py` & `fastsim-2.0.16/fastsim/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_eco_cruise.py` & `fastsim-2.0.16/fastsim/tests/test_eco_cruise.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_following.py` & `fastsim-2.0.16/fastsim/tests/test_following.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_logging.py` & `fastsim-2.0.16/fastsim/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_rust.py` & `fastsim-2.0.16/fastsim/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_simdrive.py` & `fastsim-2.0.16/fastsim/tests/test_simdrive.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_simdrive_sweep.py` & `fastsim-2.0.16/fastsim/tests/test_simdrive_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_soc_correction.py` & `fastsim-2.0.16/fastsim/tests/test_soc_correction.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_vehicle.py` & `fastsim-2.0.16/fastsim/tests/test_vehicle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/tests/test_vs_excel.py` & `fastsim-2.0.16/fastsim/tests/test_vs_excel.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/utilities.py` & `fastsim-2.0.16/fastsim/utilities.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/vehicle.py` & `fastsim-2.0.16/fastsim/vehicle.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim/vehicle_base.py` & `fastsim-2.0.16/fastsim/vehicle_base.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/fastsim.egg-info/PKG-INFO` & `fastsim-2.0.16/fastsim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsim
-Version: 2.0.15
+Version: 2.0.16
 Summary: Tool for modeling vehicle powertrains
 Author-email: NREL/MTES/CIMS/MBAP Group <fastsim@nrel.gov>
 License: Future Automotive Systems Technology Simulator (FASTSim(TM)) Copyright (c) 2020 Alliance for Sustainable Energy, LLC All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -26,112 +26,79 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: LICENSE.md
 
-![FASTSim Logo](fastsim-icon-web-131x172.jpg)
+![FASTSim Logo](fastsim/docs/fastsim-icon-web-131x172.jpg)
 
 # Description
-This is the python/rust flavor of [NREL's FASTSim](https://www.nrel.gov/transportation/fastsim.html), which is based on the original Excel implementation. Effort will be made to keep the core methodology between this software and the Excel flavor in line with one another. Other FASTSim flavors may spin off as variations on this core functionality, but these should integrated back into `main` if there is any intent of persistence.
+This is the python/rust flavor of [NREL's FASTSim](https://www.nrel.gov/transportation/fastsim.html), which is based on the original Excel implementation. Effort will be made to keep the core methodology between this software and the Excel flavor in line with one another. 
 
 All classes and methods are self-documented.  
 
 # Installation
 
-## PyPI Installation
+## Python 
+Set up and activate a python environment (compatible with Python 3.8 - 3.10; we recommend Python 3.10) with the following steps.
+### [Anaconda](https://www.anaconda.com/) 
+1. Create: `conda create -n fastsim python=3.10`
+1. Activate: `conda activate fastsim`
+
+### [venv](https://docs.python.org/3/library/venv.html)
+There is some variation based on your Operating System:  
+
+- PowerShell (windows):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `fastsim-venv/Scripts/Activate.ps1`
+
+- Bash (i.e. unix/linux/mac):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `source fastsim-venv/bin/activate`
+
+- Command Prompt (windows):
+    1. Create: `python -m venv fastsim-venv` -- name is user decision
+    1. Activate: `fastsim-venv/Scripts/activate.bat`
 
+## FASTSim
+### Via PyPI
 In an active Python environment (either [venv](https://docs.python.org/3/library/venv.html) or [Conda](https://www.anaconda.com/)), run `pip install fastsim`.
 
-## Installing from NREL's internal GitHub
-
-1. Clone the repository from GitHub:
-
-       git clone git@github.nrel.gov:MBAP/fastsim.git
-
-2. Set up an environment for the project. There are two ways to do this:
-
-   - Using Anaconda (with Python 3.8 or newer):
-
-         conda create -n fastsim python=3.8
-         conda activate fastsim
-         conda install -c conda-forge "rust>=1.64"
-
-   - Manually:
-     - Install [Rust](https://www.rust-lang.org/tools/install). 
-     - Then, using a virtual environment, and making sure to use Python >= 3.8:
-    
-        PowerShell:
-
-            python -m venv .venv
-            .venv/Scripts/Activate.ps1
-
-        Bash:
-
-            python -m venv .venv
-            source .venv/bin/activate
-
-        Command Prompt:
-
-            python -m venv .venv
-            .venv/Scripts/activate.bat
-    
-3. From within the top level of the FASTSim repository, install using pip:
-
-       pip install .
-
-## Developers
+### Building from Scratch
 Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  
 
-To do this, a couple of extra steps are required:
-
-1. First install the python code in place `DEVELOP_MODE=True pip install -e ".[dev]"` if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
-1. Within the same python environment, navigate to `fastsim/rust/` and run `pip install maturin`.
-1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
-1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
+- Easy way: run `sh build_and_test.sh` in root folder.  
+- Hard way (a couple of extra steps are required): 
+    1. First install the python code in place:  
+    `DEVELOP_MODE=True pip install -e ".[dev]"`   
+    if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run  
+    `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
+    1. Within the same python environment, navigate to `fastsim/rust/` and run  
+    `pip install maturin`.
+    1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
+    1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
 
 After FASTSim has been installed as editable per the above instructions, you can rebuild and test everything with `sh build_and_test.sh` in Windows bash or `./build_and_test.sh` in Linux/Unix in the `fastsim/` dir.  
 
-# Users with NREL VPN Access
-## Installation as PyPi Package
-Note: the following instructions work only if you are inside NREL VPN:  
-To install and/or update, run
-```
-pip install fastsim --upgrade --extra-index-url=https://github.nrel.gov/pages/MBAP/mbap-pypi/
-```
-
-## Adding FASTSim as a Depency in Rust
-Add this line:  
-`fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
-to your Cargo.toml file, modifying the `branch` key as appropriate.  
+### Testing
+At the root level of the git repository: `pytest -v fastsim/tests/`.  This can also be run in the python environment directly.  
 
 # Usage
 To see and run examples, navigate to fastsim/docs and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
 
-To get help in an interactive ipython or jupyter session:  
-```
-import fastsim
-fastsim.simdrive.SimDriveClassic? # or
-help(fastsim.simdrive.SimDriveClassic)
-```
-
-Help can be used in this manner on any FASTSim object.
-
-# Testing
 
-The `unittest` package has been implemented such that you can run `python -m unittest discover` from within the fastsim folder, and all tests will be automatically discovered and run.  
-
-## Against Previous Python Version
-
-To run tests, first run the command `from fastim import tests`.  
-To compare FASTSim back to the master branch version from 17 December 2019, run `tests.test26veh3cyc.main()`.  For timing comparisons, run `tests.test26veh3cyc_CPUtime.main()`.  
+# Adding FASTSim as a Depency in Rust
+## Via GitHub
+Add this line:  
+`fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
+to your Cargo.toml file, modifying the `branch` key as appropriate.  
 
-## Against Excel FASTSim
-To compare Python FASTSim results to Excel FASTSim, you can run `tests.test_vs_excel.main()` to do an experimental (i.e. beta) comparison against saved Excel results. If you have the Excel version (obtainable here: [https://www.nrel.gov/transportation/fastsim.html](https://www.nrel.gov/transportation/fastsim.html)) of FASTSim open, you can specify `rerun_excel=True` to do a live run of the Excel version.
+## Via Cargo
+This has not been implemented yet.  
 
 # List of Abbreviations
 cur = current time step  
 prev = previous time step  
 cyc = drive cycle  
 secs = seconds  
 mps = meters per second  
@@ -151,16 +118,19 @@
 lim = limit of a component  
 regen = associated with regenerative braking  
 des = desired value  
 ach = achieved value  
 in = component input  
 out = component output  
 
+# Known Issues
+Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
+
 # Release Notes
-2.0.11 - 2.0.15 -- PyPI fixes  
+2.0.11 - 2.0.16 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`  
 2.0.3 -- exposed `veh.__post_init__`  
@@ -188,20 +158,20 @@
 1.0.0 -- Implemented unittest package.  Fixed energy audit calculations to be based on achieved speed.  Updated this file.  Improved documentation.  Vehicle can be instantiated as dict.   
 0.1.5 -- Updated to be compatible with ADOPT    
 0.1.4 -- Bug fix: `mcEffMap` is now robust to having zero as first element    
 0.1.3 -- Bug fix: `fastsim.vehicle.Vehicle` method `set_init_calcs` no longer overrides `fcEffMap`.    
 0.1.2 -- Fixes os-dependency of xlwings by not running stuff that needs xlwings.  Improvements in functional test.  Refinment utomated typying of jitclass objects.    
 0.1.1 -- Now includes label fuel economy and/or battery kW-hr/mi values that match excel and test for benchmarking against Excel values and CPU time.   
 
-# Contributors
+# Contributors  
 Chad Baker -- Chad.Baker@nrel.gov  
 Aaron Brooker -- Aaron.Brooker@nrel.gov  
-Kyle Carow -- Kyle.Carow@nrel.gov
+Kyle Carow -- Kyle.Carow@nrel.gov  
 Jeffrey Gonder -- Jeff.Gonder@nrel.gov  
 Jacob Holden -- Jacob.Holden@nrel.gov  
-Jinghu Hu -- Jinghu.Hu@nrel.gov
+Jinghu Hu -- Jinghu.Hu@nrel.gov  
 Jason Lustbader -- Jason.Lustbader@nrel.gov  
 Sean Lopp -- sean@rstudio.com  
 Matthew Moniot -- Matthew.Moniot@nrel.gov  
 Grant Payne -- Grant.Payne@nrel.gov  
 Laurie Ramroth -- lramroth@ford.com  
 Eric Wood -- Eric.Wood@nrel.gov
```

### Comparing `fastsim-2.0.15/fastsim.egg-info/SOURCES.txt` & `fastsim-2.0.16/fastsim.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 LICENSE.md
 MANIFEST.in
 README.md
-fastsim-icon-web-131x172.jpg
 pyproject.toml
 setup.py
 fastsim/__init__.py
 fastsim/auxiliaries.py
 fastsim/calibration.py
 fastsim/cycle.py
 fastsim/inspect_utils.py
```

### Comparing `fastsim-2.0.15/pyproject.toml` & `fastsim-2.0.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "setuptools-rust>=0.11.4",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastsim"
-version = "2.0.15"
+version = "2.0.16"
 authors = [{ name = "NREL/MTES/CIMS/MBAP Group", email = "fastsim@nrel.gov" }]
 description = "Tool for modeling vehicle powertrains"
 readme = "README.md"
 license = {file = "LICENSE.md"}
 requires-python = ">=3.8,<3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fastsim-2.0.15/rust/Cargo.toml` & `fastsim-2.0.16/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/Cargo.toml` & `fastsim-2.0.16/rust/fastsim-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs` & `fastsim-2.0.16/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs` & `fastsim-2.0.16/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/proc-macros/src/history_vec_derive.rs` & `fastsim-2.0.16/rust/fastsim-core/proc-macros/src/history_vec_derive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/proc-macros/src/lib.rs` & `fastsim-2.0.16/rust/fastsim-core/proc-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/proc-macros/src/utilities.rs` & `fastsim-2.0.16/rust/fastsim-core/proc-macros/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/air.rs` & `fastsim-2.0.16/rust/fastsim-core/src/air.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/cycle.rs` & `fastsim-2.0.16/rust/fastsim-core/src/cycle.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/html/docs-header.html` & `fastsim-2.0.16/rust/fastsim-core/src/html/docs-header.html`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/lib.rs` & `fastsim-2.0.16/rust/fastsim-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/macros.rs` & `fastsim-2.0.16/rust/fastsim-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/params.rs` & `fastsim-2.0.16/rust/fastsim-core/src/params.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/simdrive/cyc_mods.rs` & `fastsim-2.0.16/rust/fastsim-core/src/simdrive/cyc_mods.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/simdrive/simdrive_impl.rs` & `fastsim-2.0.16/rust/fastsim-core/src/simdrive/simdrive_impl.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/simdrive.rs` & `fastsim-2.0.16/rust/fastsim-core/src/simdrive.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/simdrivelabel.rs` & `fastsim-2.0.16/rust/fastsim-core/src/simdrivelabel.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/thermal.rs` & `fastsim-2.0.16/rust/fastsim-core/src/thermal.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/traits.rs` & `fastsim-2.0.16/rust/fastsim-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/utils.rs` & `fastsim-2.0.16/rust/fastsim-core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/vehicle.rs` & `fastsim-2.0.16/rust/fastsim-core/src/vehicle.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/vehicle_thermal.rs` & `fastsim-2.0.16/rust/fastsim-core/src/vehicle_thermal.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-core/src/vehicle_utils.rs` & `fastsim-2.0.16/rust/fastsim-core/src/vehicle_utils.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-py/Cargo.toml` & `fastsim-2.0.16/rust/fastsim-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/rust/fastsim-py/src/lib.rs` & `fastsim-2.0.16/rust/fastsim-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.15/setup.py` & `fastsim-2.0.16/setup.py`

 * *Files identical despite different names*

