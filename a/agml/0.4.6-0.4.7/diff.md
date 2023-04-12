# Comparing `tmp/agml-0.4.6.tar.gz` & `tmp/agml-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agml-0.4.6.tar", last modified: Sun Dec 18 20:50:42 2022, max compression
+gzip compressed data, was "agml-0.4.7.tar", last modified: Wed Apr 12 01:45:36 2023, max compression
```

## Comparing `agml-0.4.6.tar` & `agml-0.4.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.496667 agml-0.4.6/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)       81 2022-03-29 13:30:39.000000 agml-0.4.6/AUTHORS
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    11357 2022-05-19 21:35:28.000000 agml-0.4.6/LICENSE
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      196 2022-10-14 14:32:05.000000 agml-0.4.6/MANIFEST.in
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10988 2022-12-18 20:50:42.496043 agml-0.4.6/PKG-INFO
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10008 2022-09-28 14:07:51.000000 agml-0.4.6/README.md
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.378409 agml-0.4.6/agml/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1304 2022-12-18 20:50:06.000000 agml-0.4.6/agml/__init__.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.395241 agml-0.4.6/agml/_assets/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6398 2022-10-06 00:40:28.000000 agml-0.4.6/agml/_assets/model_benchmarks.json
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    32276 2022-10-06 00:40:28.000000 agml-0.4.6/agml/_assets/public_datasources.json
--rw-r--r--   0 amoghjoshi   (501) staff       (20)   413453 2022-09-20 20:03:52.000000 agml-0.4.6/agml/_assets/shape_info.pickle
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    27471 2022-10-06 00:40:28.000000 agml-0.4.6/agml/_assets/source_citations.json
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      318 2022-10-23 01:02:40.000000 agml-0.4.6/agml/_assets/viz_colormaps.json
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.396201 agml-0.4.6/agml/_helios/
--rwxr-xr-x   0 amoghjoshi   (501) staff       (20)     1098 2022-10-06 00:40:28.000000 agml-0.4.6/agml/_helios/helios_install.sh
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.400781 agml-0.4.6/agml/backend/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1371 2022-10-06 00:40:28.000000 agml-0.4.6/agml/backend/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7916 2022-10-06 00:40:28.000000 agml-0.4.6/agml/backend/config.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2252 2022-10-06 00:40:28.000000 agml-0.4.6/agml/backend/experimental.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      983 2022-10-06 00:40:28.000000 agml-0.4.6/agml/backend/random.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     9958 2022-10-06 00:40:28.000000 agml-0.4.6/agml/backend/tftorch.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.422122 agml-0.4.6/agml/data/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      826 2022-03-18 21:25:35.000000 agml-0.4.6/agml/data/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    15378 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/builder.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3748 2022-03-29 13:30:39.000000 agml-0.4.6/agml/data/experimental.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.425216 agml-0.4.6/agml/data/exporters/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)        0 2022-03-29 13:30:39.000000 agml-0.4.6/agml/data/exporters/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     9639 2022-05-19 21:43:54.000000 agml-0.4.6/agml/data/exporters/tensorflow.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    72408 2022-10-31 22:25:12.000000 agml-0.4.6/agml/data/loader.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    16042 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/manager.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.429979 agml-0.4.6/agml/data/managers/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2022-03-29 13:30:39.000000 agml-0.4.6/agml/data/managers/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    14583 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/managers/resize.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    15928 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/managers/training.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     5471 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/managers/transform_helpers.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    23180 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/managers/transforms.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    13387 2022-10-31 19:23:43.000000 agml-0.4.6/agml/data/metadata.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    66025 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/multi_loader.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     9127 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/object.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6681 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/public.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7351 2022-10-06 00:40:28.000000 agml-0.4.6/agml/data/tools.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3137 2022-10-06 00:40:28.000000 agml-0.4.6/agml/framework.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.449161 agml-0.4.6/agml/models/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      953 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6551 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/base.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2624 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/benchmarks.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8556 2022-10-31 22:25:12.000000 agml-0.4.6/agml/models/classification.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    21631 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/detection.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2104 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/losses.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.451585 agml-0.4.6/agml/models/metrics/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      729 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/metrics/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2632 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/metrics/accuracy.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     9795 2022-10-31 22:25:12.000000 agml-0.4.6/agml/models/metrics/map.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8321 2022-10-31 22:25:12.000000 agml-0.4.6/agml/models/preprocessing.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    13532 2022-10-31 22:25:09.000000 agml-0.4.6/agml/models/segmentation.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     4238 2022-10-06 00:40:28.000000 agml-0.4.6/agml/models/tools.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.468032 agml-0.4.6/agml/synthetic/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1009 2022-12-18 20:48:17.000000 agml-0.4.6/agml/synthetic/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8579 2022-12-18 20:48:17.000000 agml-0.4.6/agml/synthetic/compilation.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    12018 2022-10-14 14:32:05.000000 agml-0.4.6/agml/synthetic/config.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    16098 2022-12-18 20:45:23.000000 agml-0.4.6/agml/synthetic/converter.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    18922 2022-12-18 20:48:17.000000 agml-0.4.6/agml/synthetic/generator.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    13066 2022-12-18 20:48:17.000000 agml-0.4.6/agml/synthetic/manual.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    15709 2022-12-18 20:48:17.000000 agml-0.4.6/agml/synthetic/options.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.469981 agml-0.4.6/agml/synthetic/synthetic_data_generation/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1734 2022-10-02 14:31:11.000000 agml-0.4.6/agml/synthetic/synthetic_data_generation/CMakeLists.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7175 2022-10-02 14:31:11.000000 agml-0.4.6/agml/synthetic/synthetic_data_generation/generate.cpp
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7806 2022-12-18 20:48:17.000000 agml-0.4.6/agml/synthetic/tools.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.483757 agml-0.4.6/agml/utils/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2021-10-22 20:11:12.000000 agml-0.4.6/agml/utils/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     4429 2022-10-06 00:40:28.000000 agml-0.4.6/agml/utils/data.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6589 2022-10-06 00:40:28.000000 agml-0.4.6/agml/utils/downloads.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3973 2022-12-18 20:48:17.000000 agml-0.4.6/agml/utils/general.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3567 2022-10-06 00:40:28.000000 agml-0.4.6/agml/utils/image.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3754 2022-12-18 20:48:17.000000 agml-0.4.6/agml/utils/io.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2688 2022-10-06 00:40:28.000000 agml-0.4.6/agml/utils/logging.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2371 2022-10-06 00:40:28.000000 agml-0.4.6/agml/utils/random.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.494811 agml-0.4.6/agml/viz/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1249 2022-12-18 20:48:17.000000 agml-0.4.6/agml/viz/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8178 2022-10-06 00:40:28.000000 agml-0.4.6/agml/viz/boxes.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3837 2022-12-18 20:48:17.000000 agml-0.4.6/agml/viz/general.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     5428 2022-10-02 14:31:11.000000 agml-0.4.6/agml/viz/inspection.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     4692 2022-12-18 20:48:17.000000 agml-0.4.6/agml/viz/labels.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8585 2022-10-11 22:08:15.000000 agml-0.4.6/agml/viz/masks.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7834 2022-12-18 20:48:17.000000 agml-0.4.6/agml/viz/tools.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2022-12-18 20:50:42.383352 agml-0.4.6/agml.egg-info/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10988 2022-12-18 20:50:42.000000 agml-0.4.6/agml.egg-info/PKG-INFO
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1936 2022-12-18 20:50:42.000000 agml-0.4.6/agml.egg-info/SOURCES.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)        1 2022-12-18 20:50:42.000000 agml-0.4.6/agml.egg-info/dependency_links.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      367 2022-12-18 20:50:42.000000 agml-0.4.6/agml.egg-info/requires.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)        5 2022-12-18 20:50:42.000000 agml-0.4.6/agml.egg-info/top_level.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)       38 2022-12-18 20:50:42.496853 agml-0.4.6/setup.cfg
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2551 2022-10-14 14:32:05.000000 agml-0.4.6/setup.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.151524 agml-0.4.7/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)       81 2022-03-29 13:30:39.000000 agml-0.4.7/AUTHORS
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    11357 2022-05-19 21:35:28.000000 agml-0.4.7/LICENSE
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      196 2022-10-14 14:32:05.000000 agml-0.4.7/MANIFEST.in
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    10988 2023-04-12 01:45:36.150870 agml-0.4.7/PKG-INFO
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    10008 2022-09-28 14:07:51.000000 agml-0.4.7/README.md
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.015937 agml-0.4.7/agml/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1304 2023-04-12 01:45:21.000000 agml-0.4.7/agml/__init__.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.031516 agml-0.4.7/agml/_assets/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6398 2022-10-06 00:40:28.000000 agml-0.4.7/agml/_assets/model_benchmarks.json
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    34168 2023-04-12 00:58:07.000000 agml-0.4.7/agml/_assets/public_datasources.json
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)   413744 2023-04-12 00:58:07.000000 agml-0.4.7/agml/_assets/shape_info.pickle
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    27671 2023-04-12 00:58:07.000000 agml-0.4.7/agml/_assets/source_citations.json
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      318 2022-10-23 01:02:40.000000 agml-0.4.7/agml/_assets/viz_colormaps.json
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.032319 agml-0.4.7/agml/_helios/
+-rwxr-xr-x   0 amoghjoshi   (501) staff       (20)     1098 2022-10-06 00:40:28.000000 agml-0.4.7/agml/_helios/helios_install.sh
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.037009 agml-0.4.7/agml/backend/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1371 2022-10-06 00:40:28.000000 agml-0.4.7/agml/backend/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7916 2022-10-06 00:40:28.000000 agml-0.4.7/agml/backend/config.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2252 2022-10-06 00:40:28.000000 agml-0.4.7/agml/backend/experimental.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      983 2022-10-06 00:40:28.000000 agml-0.4.7/agml/backend/random.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     9958 2022-10-06 00:40:28.000000 agml-0.4.7/agml/backend/tftorch.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.054669 agml-0.4.7/agml/data/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      826 2022-03-18 21:25:35.000000 agml-0.4.7/agml/data/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    15378 2023-04-12 00:58:07.000000 agml-0.4.7/agml/data/builder.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3748 2022-03-29 13:30:39.000000 agml-0.4.7/agml/data/experimental.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.057521 agml-0.4.7/agml/data/exporters/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)        0 2022-03-29 13:30:39.000000 agml-0.4.7/agml/data/exporters/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     9639 2022-05-19 21:43:54.000000 agml-0.4.7/agml/data/exporters/tensorflow.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    72409 2023-04-12 00:58:07.000000 agml-0.4.7/agml/data/loader.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    16042 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/manager.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.105277 agml-0.4.7/agml/data/managers/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2022-03-29 13:30:39.000000 agml-0.4.7/agml/data/managers/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    14583 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/managers/resize.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    15928 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/managers/training.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     5471 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/managers/transform_helpers.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    23180 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/managers/transforms.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    13454 2023-04-12 00:58:07.000000 agml-0.4.7/agml/data/metadata.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    66025 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/multi_loader.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     9127 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/object.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6681 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/public.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7351 2022-10-06 00:40:28.000000 agml-0.4.7/agml/data/tools.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3137 2022-10-06 00:40:28.000000 agml-0.4.7/agml/framework.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.116011 agml-0.4.7/agml/models/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      953 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6551 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/base.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2624 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/benchmarks.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8636 2023-01-28 16:15:15.000000 agml-0.4.7/agml/models/classification.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    21631 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/detection.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2104 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/losses.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.121315 agml-0.4.7/agml/models/metrics/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      729 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/metrics/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2632 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/metrics/accuracy.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     9795 2022-10-31 22:25:12.000000 agml-0.4.7/agml/models/metrics/map.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8321 2022-10-31 22:25:12.000000 agml-0.4.7/agml/models/preprocessing.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    13532 2022-10-31 22:25:09.000000 agml-0.4.7/agml/models/segmentation.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     4238 2022-10-06 00:40:28.000000 agml-0.4.7/agml/models/tools.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.131746 agml-0.4.7/agml/synthetic/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1009 2023-01-12 19:08:43.000000 agml-0.4.7/agml/synthetic/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8579 2023-01-12 19:08:43.000000 agml-0.4.7/agml/synthetic/compilation.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    12018 2022-10-14 14:32:05.000000 agml-0.4.7/agml/synthetic/config.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    16172 2023-04-12 00:58:07.000000 agml-0.4.7/agml/synthetic/converter.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    19257 2023-04-12 01:43:01.000000 agml-0.4.7/agml/synthetic/generator.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    13066 2023-01-12 19:08:43.000000 agml-0.4.7/agml/synthetic/manual.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    16153 2023-04-12 01:44:11.000000 agml-0.4.7/agml/synthetic/options.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.133446 agml-0.4.7/agml/synthetic/synthetic_data_generation/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1734 2022-10-02 14:31:11.000000 agml-0.4.7/agml/synthetic/synthetic_data_generation/CMakeLists.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7502 2023-04-12 01:16:21.000000 agml-0.4.7/agml/synthetic/synthetic_data_generation/generate.cpp
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7806 2023-01-12 19:08:43.000000 agml-0.4.7/agml/synthetic/tools.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.142324 agml-0.4.7/agml/utils/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2021-10-22 20:11:12.000000 agml-0.4.7/agml/utils/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     4429 2022-10-06 00:40:28.000000 agml-0.4.7/agml/utils/data.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6589 2022-10-06 00:40:28.000000 agml-0.4.7/agml/utils/downloads.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3973 2023-01-12 19:08:43.000000 agml-0.4.7/agml/utils/general.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3585 2023-04-12 00:58:07.000000 agml-0.4.7/agml/utils/image.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3754 2023-01-12 19:08:43.000000 agml-0.4.7/agml/utils/io.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2688 2022-10-06 00:40:28.000000 agml-0.4.7/agml/utils/logging.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2371 2022-10-06 00:40:28.000000 agml-0.4.7/agml/utils/random.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.149972 agml-0.4.7/agml/viz/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1249 2023-01-12 19:08:43.000000 agml-0.4.7/agml/viz/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8178 2022-10-06 00:40:28.000000 agml-0.4.7/agml/viz/boxes.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3837 2023-01-12 19:08:43.000000 agml-0.4.7/agml/viz/general.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     5428 2022-10-02 14:31:11.000000 agml-0.4.7/agml/viz/inspection.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     4692 2023-01-12 19:08:43.000000 agml-0.4.7/agml/viz/labels.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8585 2022-10-11 22:08:15.000000 agml-0.4.7/agml/viz/masks.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7834 2023-01-12 19:08:43.000000 agml-0.4.7/agml/viz/tools.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-04-12 01:45:36.020387 agml-0.4.7/agml.egg-info/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    10988 2023-04-12 01:45:35.000000 agml-0.4.7/agml.egg-info/PKG-INFO
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1936 2023-04-12 01:45:35.000000 agml-0.4.7/agml.egg-info/SOURCES.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)        1 2023-04-12 01:45:35.000000 agml-0.4.7/agml.egg-info/dependency_links.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      367 2023-04-12 01:45:35.000000 agml-0.4.7/agml.egg-info/requires.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)        5 2023-04-12 01:45:35.000000 agml-0.4.7/agml.egg-info/top_level.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)       38 2023-04-12 01:45:36.151772 agml-0.4.7/setup.cfg
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2551 2022-10-14 14:32:05.000000 agml-0.4.7/setup.py
```

### Comparing `agml-0.4.6/LICENSE` & `agml-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/PKG-INFO` & `agml-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agml
-Version: 0.4.6
+Version: 0.4.7
 Summary: A comprehensive library for agricultural deep learning
 Home-page: https://github.com/plant-ai-biophysics-lab/AgML
 Author: UC Davis Plant AI and Biophysics Lab
 Author-email: jmearles@ucdavis.edu
 Maintainer: Amogh Joshi
 Maintainer-email: amnjoshi@ucdavis.edu
 License: UNKNOWN
```

### Comparing `agml-0.4.6/README.md` & `agml-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/__init__.py` & `agml-0.4.7/agml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.4.6'
+__version__ = '0.4.7'
 __all__ = ['data', 'synthetic', 'backend', 'viz']
 
 
 # If AgML is being imported for the first time, then we need to setup
 # the module, namely prepping the config file.
 def _setup():
     import os as _os
```

### Comparing `agml-0.4.6/agml/_assets/model_benchmarks.json` & `agml-0.4.7/agml/_assets/model_benchmarks.json`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/_assets/public_datasources.json` & `agml-0.4.7/agml/_assets/public_datasources.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9354838709677419%*

 * *Differences: {"'ghai_green_cabbage_detection'": "OrderedDict([('classes', OrderedDict([('1', "*

 * *                                   "'green_cabbage')])), ('ml_task', 'object_detection'), "*

 * *                                   "('ag_task', 'crop_detection'), ('location', "*

 * *                                   "OrderedDict([('continent', 'north_america'), ('country', "*

 * *                                   "'usa')])), ('sensor_modality', 'rgb'), ('real_synthetic', "*

 * *                                   "'real'), ('platform', 'handhe […]*

```diff
@@ -324,14 +324,76 @@
             "std": [
                 0.2306382656097412,
                 0.22500208020210266,
                 0.2183498740196228
             ]
         }
     },
+    "ghai_green_cabbage_detection": {
+        "ag_task": "crop_detection",
+        "annotation_format": "coco_json",
+        "classes": {
+            "1": "green_cabbage"
+        },
+        "docs_url": "https://github.com/AxisAg/GHAIDatasets/blob/main/datasets/green_cabbage.md",
+        "external_image_sources": [],
+        "input_data_format": "jpg",
+        "location": {
+            "continent": "north_america",
+            "country": "usa"
+        },
+        "ml_task": "object_detection",
+        "n_images": "500",
+        "platform": "handheld/ground",
+        "real_synthetic": "real",
+        "sensor_modality": "rgb",
+        "stats": {
+            "mean": [
+                0.4649180769920349,
+                0.49569201469421387,
+                0.46829652786254883
+            ],
+            "std": [
+                0.28846681118011475,
+                0.27976617217063904,
+                0.276553213596344
+            ]
+        }
+    },
+    "ghai_romaine_detection": {
+        "ag_task": "crop_detection",
+        "annotation_format": "coco_json",
+        "classes": {
+            "1": "romaine"
+        },
+        "docs_url": "https://github.com/AxisAg/GHAIDatasets/blob/main/datasets/romaine.md",
+        "external_image_sources": [],
+        "input_data_format": "jpg",
+        "location": {
+            "continent": "north_america",
+            "country": "usa"
+        },
+        "ml_task": "object_detection",
+        "n_images": "500",
+        "platform": "handheld/ground",
+        "real_synthetic": "real",
+        "sensor_modality": "rgb",
+        "stats": {
+            "mean": [
+                0.3551516532897949,
+                0.4719887971878052,
+                0.33378446102142334
+            ],
+            "std": [
+                0.253168523311615,
+                0.26515713334083557,
+                0.2393222600221634
+            ]
+        }
+    },
     "grape_detection_californiaday": {
         "ag_task": "fruit_detection",
         "annotation_format": "image",
         "classes": {
             "1": "grape"
         },
         "docs_url": "",
```

### Comparing `agml-0.4.6/agml/_assets/shape_info.pickle` & `agml-0.4.7/agml/_assets/shape_info.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -22693,15 +22693,15 @@
 00058a40: 0001 0000 0000 0000 0001 0000 0000 0000  ................
 00058a50: 0002 0000 0000 0000 0002 0000 0000 0000  ................
 00058a60: 0001 0000 0000 0000 0001 0000 0000 0000  ................
 00058a70: 0001 0000 0000 0000 0001 0000 0000 0000  ................
 00058a80: 0001 0000 0000 0000 0001 0000 0000 0000  ................
 00058a90: 0001 0000 0000 0000 0003 0000 0000 0000  ................
 00058aa0: 0001 0000 0000 0000 0094 7494 6286 9495  ..........t.b...
-00058ab0: 55c4 0000 0000 0000 8c20 6175 746f 6e6f  U........ autono
+00058ab0: 78c5 0000 0000 0000 8c20 6175 746f 6e6f  x........ autono
 00058ac0: 6d6f 7573 5f67 7265 656e 686f 7573 655f  mous_greenhouse_
 00058ad0: 7265 6772 6573 7369 6f6e 9468 0468 074b  regression.h.h.K
 00058ae0: 0085 9468 0987 9452 9428 4b01 4b01 4b03  ...h...R.(K.K.K.
 00058af0: 8694 680e 8c02 6938 9489 8887 9452 9428  ..h...i8.....R.(
 00058b00: 4b03 6812 4e4e 4e4a ffff ffff 4aff ffff  K.h.NNNJ....J...
 00058b10: ff4b 0074 9462 8943 1838 0400 0000 0000  .K.t.b.C.8......
 00058b20: 0080 0700 0000 0000 0003 0000 0000 0000  ................
@@ -25834,8 +25834,26 @@
 00064e90: 9452 9428 4b01 4b02 4b03 8694 6ac2 0100  .R.(K.K.K...j...
 00064ea0: 0089 4330 e000 0000 0000 0000 e000 0000  ..C0............
 00064eb0: 0000 0000 0300 0000 0000 0000 0001 0000  ................
 00064ec0: 0000 0000 0001 0000 0000 0000 0300 0000  ................
 00064ed0: 0000 0000 9474 9462 6804 6807 4b00 8594  .....t.bh.h.K...
 00064ee0: 6809 8794 5294 284b 014b 0285 946a c201  h...R.(K.K...j..
 00064ef0: 0000 8943 10ff 0000 0000 0000 0003 0000  ...C............
-00064f00: 0000 0000 0094 7494 6286 9475 2e         ......t.b..u.
+00064f00: 0000 0000 0094 7494 6286 948c 1c67 6861  ......t.b....gha
+00064f10: 695f 6772 6565 6e5f 6361 6262 6167 655f  i_green_cabbage_
+00064f20: 6465 7465 6374 696f 6e94 6804 6807 4b00  detection.h.h.K.
+00064f30: 8594 6809 8794 5294 284b 014b 014b 0386  ..h...R.(K.K.K..
+00064f40: 9468 0e8c 0269 3894 8988 8794 5294 284b  .h...i8.....R.(K
+00064f50: 0368 124e 4e4e 4aff ffff ff4a ffff ffff  .h.NNNJ....J....
+00064f60: 4b00 7494 6289 4318 3804 0000 0000 0000  K.t.b.C.8.......
+00064f70: 8007 0000 0000 0000 0300 0000 0000 0000  ................
+00064f80: 9474 9462 6804 6807 4b00 8594 6809 8794  .t.bh.h.K...h...
+00064f90: 5294 284b 014b 0185 946a e201 0000 8943  R.(K.K...j.....C
+00064fa0: 08f4 0100 0000 0000 0094 7494 6286 948c  ..........t.b...
+00064fb0: 1667 6861 695f 726f 6d61 696e 655f 6465  .ghai_romaine_de
+00064fc0: 7465 6374 696f 6e94 6804 6807 4b00 8594  tection.h.h.K...
+00064fd0: 6809 8794 5294 284b 014b 014b 0386 946a  h...R.(K.K.K...j
+00064fe0: e201 0000 8943 1838 0400 0000 0000 0080  .....C.8........
+00064ff0: 0700 0000 0000 0003 0000 0000 0000 0094  ................
+00065000: 7494 6268 0468 074b 0085 9468 0987 9452  t.bh.h.K...h...R
+00065010: 9428 4b01 4b01 8594 6ae2 0100 0089 4308  .(K.K...j.....C.
+00065020: f401 0000 0000 0000 9474 9462 8694 752e  .........t.b..u.
```

### Comparing `agml-0.4.6/agml/_assets/source_citations.json` & `agml-0.4.7/agml/_assets/source_citations.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9354838709677419%*

 * *Differences: {"'ghai_green_cabbage_detection'": "OrderedDict([('license', 'CC BY-SA 4.0'), ('citation', '')])",*

 * * "'ghai_romaine_detection'": "OrderedDict([('license', 'CC BY-SA 4.0'), ('citation', '')])"}*

```diff
@@ -35,14 +35,22 @@
         "citation": "@article{ESPEJOGARCIA2020105306,\n  title = {Towards weeds identification assistance through transfer learning},\n  journal = {Computers and Electronics in Agriculture},\n  volume = {171},\n  pages = {105306},\n  year = {2020},\n  issn = {0168-1699},\n  doi = {https://doi.org/10.1016/j.compag.2020.105306},\n  url = {https://www.sciencedirect.com/science/article/pii/S0168169919319854},\n  author = {Borja Espejo-Garcia and Nikos Mylonas and Loukas Athanasakos and Spyros Fountas and Ioannis Vasilakoglou},\n  keywords = {Weed identification, Deep learning, Transfer learning, Open data, Precision agriculture},\n  abstract = {Reducing the use of pesticides through selective spraying is an important component towards a more sustainable computer-assisted agriculture. Weed identification at early growth stage contributes to reduced herbicide rates. However, while computer vision alongside deep learning have overcome the performance of approaches that use hand-crafted features, there are still some open challenges in the development of a reliable automatic plant identification system. These type of systems have to take into account different sources of variability, such as growth stages and soil conditions, with the added constraint of the limited size of usual datasets. This study proposes a novel crop/weed identification system that relies on a combination of fine-tuning pre-trained convolutional networks (Xception, Inception-Resnet, VGNets, Mobilenet and Densenet) with the \u201ctraditional\u201d machine learning classifiers (Support Vector Machines, XGBoost and Logistic Regression) trained with the previously deep extracted features. The aim of this approach was to avoid overfitting and to obtain a robust and consistent performance. To evaluate this approach, an open access dataset of two crop [tomato (Solanum lycopersicum L.) and cotton (Gossypium hirsutum L.)] and two weed species [black nightshade (Solanum nigrum L.) and velvetleaf (Abutilon theophrasti Medik.)] was generated. The pictures were taken by different production sites across Greece under natural variable light conditions from RGB cameras. The results revealed that a combination of fine-tuned Densenet and Support Vector Machine achieved a micro F1 score of 99.29% with a very low performance difference between train and test sets. Other evaluated approaches also obtained repeatedly more than 95% F1 score. Additionally, our results analysis provides some heuristics for designing transfer-learning based systems to avoid overfitting without decreasing performance.}\n}",
         "license": "MIT"
     },
     "fruit_detection_worldwide": {
         "citation": "@Article{s16081222,\n  AUTHOR = {Sa, Inkyu and Ge, Zongyuan and Dayoub, Feras and Upcroft, Ben and Perez, Tristan and McCool, Chris},\n  TITLE = {DeepFruits: A Fruit Detection System Using Deep Neural Networks},\n  JOURNAL = {Sensors},\n  VOLUME = {16},\n  YEAR = {2016},\n  NUMBER = {8},\n  ARTICLE-NUMBER = {1222},\n  URL = {https://www.mdpi.com/1424-8220/16/8/1222},\n  ISSN = {1424-8220},\n  ABSTRACT = {This paper presents a novel approach to fruit detection using deep convolutional neural networks. The aim is to build an accurate, fast and reliable fruit detection system, which is a vital element of an autonomous agricultural robotic platform; it is a key element for fruit yield estimation and automated harvesting. Recent work in deep neural networks has led to the development of a state-of-the-art object detector termed Faster Region-based CNN (Faster R-CNN). We adapt this model, through transfer learning, for the task of fruit detection using imagery obtained from two modalities: colour (RGB) and Near-Infrared (NIR). Early and late fusion methods are explored for combining the multi-modal (RGB and NIR) information. This leads to a novel multi-modal Faster R-CNN model, which achieves state-of-the-art results compared to prior work with the F1 score, which takes into account both precision and recall performances improving from     0 . 807     to     0 . 838     for the detection of sweet pepper. In addition to improved accuracy, this approach is also much quicker to deploy for new fruits, as it requires bounding box annotation rather than pixel-level annotation (annotating bounding boxes is approximately an order of magnitude quicker to perform). The model is retrained to perform the detection of seven fruits, with the entire process taking four hours to annotate and train the new model per fruit.},\n  DOI = {10.3390/s16081222}\n}",
         "license": ""
     },
+    "ghai_green_cabbage_detection": {
+        "citation": "",
+        "license": "CC BY-SA 4.0"
+    },
+    "ghai_romaine_detection": {
+        "citation": "",
+        "license": "CC BY-SA 4.0"
+    },
     "grape_detection_californiaday": {
         "citation": "@misc{GrapeDay,\n  author    = {Plant AI and Biophysics Lab},\n  title     = {Grape Detection 2019 Day},\n  year      = {2019},\n  url       = {https://github.com/plant-ai-biophysics-lab/AgML} \n ",
         "license": ""
     },
     "grape_detection_californianight": {
         "citation": "@misc{GrapeNight,\n  author    = {Plant AI and Biophysics Lab},\n  title     = {Grape Detection 2020 Night},\n  year      = {2020},\n  url       = {https://github.com/plant-ai-biophysics-lab/AgML} \n ",
         "license": ""
```

### Comparing `agml-0.4.6/agml/_helios/helios_install.sh` & `agml-0.4.7/agml/_helios/helios_install.sh`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/backend/__init__.py` & `agml-0.4.7/agml/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/backend/config.py` & `agml-0.4.7/agml/backend/config.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/backend/experimental.py` & `agml-0.4.7/agml/backend/experimental.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/backend/random.py` & `agml-0.4.7/agml/backend/random.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/backend/tftorch.py` & `agml-0.4.7/agml/backend/tftorch.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/__init__.py` & `agml-0.4.7/agml/data/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/builder.py` & `agml-0.4.7/agml/data/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 image_coco.append(c)
                 image_id_tracker += 1
 
         # Update the image IDs for the annotations
         for image_id, (_, annotation) in enumerate(data.items()):
             for a in annotation:
                 a['id'] = image_id
-            annotation_coco.append(annotation)
+            annotation_coco.extend(annotation)
 
         # Update the complete COCO dictionary.
         ret_coco = coco.copy()
         ret_coco['images'] = image_coco
         ret_coco['annotations'] = annotation_coco
         return ret_coco
```

### Comparing `agml-0.4.6/agml/data/experimental.py` & `agml-0.4.7/agml/data/experimental.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/exporters/tensorflow.py` & `agml-0.4.7/agml/data/exporters/tensorflow.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/loader.py` & `agml-0.4.7/agml/data/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1604,7 +1604,8 @@
 
 
 
 
 
 
 
+
```

### Comparing `agml-0.4.6/agml/data/manager.py` & `agml-0.4.7/agml/data/manager.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/managers/__init__.py` & `agml-0.4.7/agml/data/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/managers/resize.py` & `agml-0.4.7/agml/data/managers/resize.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/managers/training.py` & `agml-0.4.7/agml/data/managers/training.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/managers/transform_helpers.py` & `agml-0.4.7/agml/data/managers/transform_helpers.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/managers/transforms.py` & `agml-0.4.7/agml/data/managers/transforms.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/metadata.py` & `agml-0.4.7/agml/data/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     """Creates the metadata object for the dataset.
 
     For datasets in the AgML public data repository, this simply returns
     a regular `DatasetMetadata` object with a full set of information for
     the dataset. Otherwise, it returns a `CustomDatasetMetadata` object,
     containing only the provided information in a `meta` dictionary.
     """
+    if isinstance(name, DatasetMetadata):
+        name = name.name
     if isinstance(name, (list, tuple, set, frozenset)): # a single dataset
         name = next(iter(name))
     if name in load_public_sources().keys():
         return DatasetMetadata(name)
     return CustomDatasetMetadata(name, meta)
```

### Comparing `agml-0.4.6/agml/data/multi_loader.py` & `agml-0.4.7/agml/data/multi_loader.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/object.py` & `agml-0.4.7/agml/data/object.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/public.py` & `agml-0.4.7/agml/data/public.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/data/tools.py` & `agml-0.4.7/agml/data/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/framework.py` & `agml-0.4.7/agml/framework.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/__init__.py` & `agml-0.4.7/agml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/base.py` & `agml-0.4.7/agml/models/base.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/benchmarks.py` & `agml-0.4.7/agml/models/benchmarks.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/classification.py` & `agml-0.4.7/agml/models/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,21 @@
     actual transfer `EfficientNetB4` model can be accessed through the
     parameter `net`, and you'll need to implement methods like `training_step`,
     `configure_optimizers`, etc. See PyTorch Lightning for more information.
     """
     serializable = frozenset(("model", "regression"))
     state_override = frozenset(("model",))
 
-    def __init__(self, num_classes, regression = False):
+    def __init__(self, num_classes = None, regression = False, **kwargs):
         # Construct the network and load in pretrained weights.
         super(ClassificationModel, self).__init__()
-        self._num_classes = num_classes
-        self._regression = regression
-        self.net = self._construct_sub_net(num_classes)
+        if kwargs.get('model_initialized', False):
+            self._num_classes = num_classes
+            self._regression = regression
+            self.net = self._construct_sub_net(num_classes)
 
     @auto_move_data
     def forward(self, batch):
         return self.net(batch)
 
     @staticmethod
     def _construct_sub_net(num_classes):
```

### Comparing `agml-0.4.6/agml/models/detection.py` & `agml-0.4.7/agml/models/detection.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/losses.py` & `agml-0.4.7/agml/models/losses.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/metrics/__init__.py` & `agml-0.4.7/agml/models/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/metrics/accuracy.py` & `agml-0.4.7/agml/models/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/metrics/map.py` & `agml-0.4.7/agml/models/metrics/map.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/preprocessing.py` & `agml-0.4.7/agml/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/segmentation.py` & `agml-0.4.7/agml/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/models/tools.py` & `agml-0.4.7/agml/models/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/synthetic/__init__.py` & `agml-0.4.7/agml/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/synthetic/compilation.py` & `agml-0.4.7/agml/synthetic/compilation.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/synthetic/config.py` & `agml-0.4.7/agml/synthetic/config.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/synthetic/converter.py` & `agml-0.4.7/agml/synthetic/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 
         # Generate the image COCO JSON contents.
         image_coco, image_id_map = [], {}
         for indx, image in enumerate(image_annotation_map.keys()):
             image_id_map[image] = indx + 1
             fpath = os.path.basename(image_new_map[image])
             image_coco.append({
-                'file_name': fpath, 'height': self._meta.image_size[0],
-                'width': self._meta.image_size[1], 'id': indx + 1})
+                'file_name': fpath, 'width': self._meta.image_size[0],
+                'height': self._meta.image_size[1], 'id': indx + 1})
 
         # Generate the annotation COCO JSON contents.
         annotation_coco = []
         for indx, (image, annotation) in enumerate(image_annotation_map.items()):
             image_box_tracker = 1
             for label, bboxes in annotation.items():
                 for box in bboxes:
@@ -196,15 +196,15 @@
         with open(os.path.join(self._meta.path, 'annotations.json'), 'w') as f:
             json.dump({
                 'images': image_coco, 'annotations': annotation_coco,
                 'categories': category_coco, 'info': info_coco}, f, indent = 4)
 
     def _convert_text_files_to_object_annotations(self, image_dir):
         """Converts text file annotations to COCO JSON object annotations."""
-        height, width = self._meta.image_size
+        width, height = self._meta.image_size
         txt_fmt = os.path.join(image_dir, 'rectangular_labels_{0}.txt')
 
         # Read each of the files corresponding to the given labels.
         bboxes = {}
         for indx, label in enumerate(self._meta.labels):
             # Get the path to the specific text file and check for its existence.
             path = txt_fmt.format(label)
@@ -219,26 +219,28 @@
                 else:
                     raise err
 
             # Read the text file and get all of the lines in float format.
             with open(path, 'r') as f:
                 annotations = np.array(
                     [line.replace('\n', '').strip().split(' ') for line in f.readlines()])
+
+            if len(annotations) > 0:
                 annotations = annotations[:, 1:].astype(np.float32)
 
-            # Convert the bounding boxes to COCO JSON format.
-            x_c, y_c, w, h = np.rollaxis(annotations, 1)
-            x_min = (x_c - w / 2) * width
-            y_min = ((1 - y_c) - h / 2) * height
-            w = w * width
-            h = h * height
-            coords = np.dstack([x_min, y_min, w, h])[0].astype(np.int32)
+                # Convert the bounding boxes to COCO JSON format.
+                x_c, y_c, w, h = np.rollaxis(annotations, 1)
+                x_min = (x_c - w / 2) * width
+                y_min = ((1 - y_c) - h / 2) * height
+                w = w * width
+                h = h * height
+                coords = np.dstack([x_min, y_min, w, h])[0].astype(np.int32)
 
-            # Update the bounding box dictionary.
-            bboxes[indx + 1] = coords
+                # Update the bounding box dictionary.
+                bboxes[indx + 1] = coords
 
         # Return the bounding box dictionary.
         return bboxes
 
     def _create_output_directory_structure(self):
         """Builds the output directory structure for the dataset."""
         if self._meta.annotation_type == 'object_detection':
```

### Comparing `agml-0.4.6/agml/synthetic/generator.py` & `agml-0.4.7/agml/synthetic/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,25 +38,25 @@
 from agml.utils.logging import log
 
 
 @dataclass
 class GenerationInstanceOptions:
     canopy: str
     num_images: int
-    annotation_type: Union[AnnotationType, str]
+    annotation_type: List[Union[AnnotationType, str]]
     simulation_type: Union[SimulationType, str]
     labels: List[str]
     output_dir: str
 
     def __post_init__(self):
         if self.num_images < 1:
             raise ValueError("The number of images cannot be negative.")
 
         try:
-            self.annotation_type = AnnotationType(self.annotation_type)
+            self.annotation_type = [AnnotationType(a) for a in self.annotation_type]
         except ValueError:
             raise ValueError(
                 "Expected either an `AnnotationType` parameter "
                 "or corresponding string for 'annotation_type'. "
                 "Valid annotation types: `object_detection`, "
                 "`semantic_segmentation`, `instance_segmentation`, "
                 "or for no annotations at all, `none`.")
@@ -233,15 +233,15 @@
             os.makedirs(output_path)
 
     def _write_config(self, *, cfg_file, xml_file):
         """Writes the config file that Helios loads from."""
         # Construct the string with the output.
         xml_file = os.path.realpath(xml_file)
         cfg = f"{self._generation_options.num_images}\n" \
-              f"{self._generation_options.annotation_type.value}\n" \
+              f"{' '.join([i.value for i in self._generation_options.annotation_type])}\n" \
               f"{self._generation_options.simulation_type.value}\n" \
               f"{' '.join(self._generation_options.labels)}\n" \
               f"{xml_file}\n{self._generation_options.output_dir}"
 
         # Write the configuration file to its output path.
         with open(os.path.join(PROJECT_PATH, cfg_file), 'w') as f:
             f.write(cfg)
@@ -286,15 +286,17 @@
 
         NOte that this is only the post-Helios output structure. By default, after
         the dataset is generated, the annotations will be converted from the Helios
         format to the relevant format within AgML. For example, annotation text files
         will be converted to COCO JSON, and the directory structure of the dataset
         will also be changed accordingly. If you want to maintain the integrity of
         the generated data for Helios, then you can provide the optional parameter
-        `convert_data = False`, which will leave data as generated by Helios.
+        `convert_data = False`, which will leave data as generated by Helios. Note that
+        if multiple annotation types are being generated at once, then you cannot
+        use data conversion into the AgML format.
 
         Regardless of whether annotations are converted to the AgML format from the
         Helios format, the output directory will contain an extra hidden directory
         `.metadata`, which will contain a few extra files:
 
             1. The XML file which contains the parameters in the `HeliosOptions`.
             2. The `config.txt` file which is used for generation.
@@ -408,10 +410,13 @@
                               f"passing a smaller environment for generation.")
             else:
                 raise OSError(f"Encountered an error when generating synthetic "
                               f"data. Process returned code {process.returncode}.")
 
         # Convert the dataset format.
         if convert_data:
+            if len(self.options.annotation_type) > 1:
+                log("Cannot convert data for multiple annotation types.")
+                return
             cvt = HeliosDataFormatConverter(output_dir)
             cvt.convert()
```

### Comparing `agml-0.4.6/agml/synthetic/manual.py` & `agml-0.4.7/agml/synthetic/manual.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/synthetic/options.py` & `agml-0.4.7/agml/synthetic/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,20 +325,27 @@
         return self._camera_parameters
 
     @property
     def lidar(self) -> LiDARParameters:
         return self._lidar_parameters
     
     @property
-    def annotation_type(self) -> str:
-        return self._annotation_type
+    def annotation_type(self) -> List:
+        # The returned annotation type needs to be a list. If there is only
+        # one type of annotation (the most common situation), then this makes sure
+        # that it is passed in a list format to the Helios data generator.
+        at = self._annotation_type
+        return at if isinstance(at, list) else [at]
     
     @annotation_type.setter
-    def annotation_type(self, value: Union[AnnotationType, str]):
-        self._annotation_type = AnnotationType(value)
+    def annotation_type(self, value: Union[AnnotationType, str, List[Union[AnnotationType, str]]]):
+        if isinstance(value, list):
+            self._annotation_type = [AnnotationType(v) for v in value]
+        else:
+            self._annotation_type = AnnotationType(value)
 
     @property
     def simulation_type(self) -> str:
         return self._simulation_type
 
     @simulation_type.setter
     def simulation_type(self, value: Union[SimulationType, str]):
```

### Comparing `agml-0.4.6/agml/synthetic/synthetic_data_generation/CMakeLists.txt` & `agml-0.4.7/agml/synthetic/synthetic_data_generation/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/synthetic/synthetic_data_generation/generate.cpp` & `agml-0.4.7/agml/synthetic/synthetic_data_generation/generate.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 using namespace std;
 using namespace helios;
 
 
 struct SyntheticAnnotationConfig {
 public:
     int num_images;
-    string annotation_type;
+    vector<string> annotation_type;
     string simulation_type;
     vector<string> labels;
     string xml_path;
     string output_path;
     void load_config(const char* path);
 };
 
@@ -40,14 +40,20 @@
 
     string line;
     for (int i = 0; i < 6; i++) {
         getline(file, line);
         if (i == 0) {
             this->num_images = stoi(line);
         } else if (i == 1) {
+            string delimeter = " "; size_t pos;
+            vector<string> annotation_types;
+            while ((pos = line.find(' ')) != string::npos) {
+                annotation_types.push_back(line.substr(0, pos));
+                line.erase(0, pos + delimeter.length());
+            }
             this->annotation_type = line;
         } else if (i == 2) {
             this->simulation_type = line;
         } else if (i == 3) {
             string delimeter = " "; size_t pos;
             vector<string> labels;
             while ((pos = line.find(' ')) != string::npos) {
@@ -139,42 +145,43 @@
         cgen.loadXML(config.xml_path.c_str());
 
         // Declare the Synthetic Annotation class.
         SyntheticAnnotation annotation(&context);
 
         if (config.annotation_type != "none") {
             // Set the annotation type based on the configuration.
-            if (config.annotation_type != "semantic_segmentation") {
+            vector<string> va = config.annotation_type;
+            if (!contains(va, "semantic_segmentation")) {
                 annotation.disableSemanticSegmentation();
             }
-            if (config.annotation_type != "object_detection") {
+            if (!contains(va, "object_detection")) {
                 annotation.disableObjectDetection();
             }
-            if (config.annotation_type != "instance_segmentation") {
+            if (!contains(va, "instance_segmentation")) {
                 annotation.disableInstanceSegmentation();
             }
 
             // Add labels according to whatever scheme we want.
-            vector<string> v = config.labels;
+            vector<string> vl = config.labels;
             for(int p = 0; p < cgen.getPlantCount(); p++) { // loop over vines
                 if (config.simulation_type == "rgb") {
-                    if (contains(v, "trunks")) {
+                    if (contains(vl, "trunks")) {
                         annotation.labelPrimitives(cgen.getTrunkUUIDs(p), "trunks");
                     }
-                    if (contains(v, "branches")) {
+                    if (contains(vl, "branches")) {
                         annotation.labelPrimitives(cgen.getBranchUUIDs(p), "branches");
                     }
-                    if (contains(v, "cordon")) {
+                    if (contains(vl, "cordon")) {
                         // Not implemented?
                         // annotation.labelPrimitives(cgen.getCordonUUIDs(p), "cordon");
                     }
-                    if (contains(v, "leaves")) {
+                    if (contains(vl, "leaves")) {
                         annotation.labelPrimitives(cgen.getLeafUUIDs(p), "leaves");
                     }
-                    if (contains(v, "fruits")) {
+                    if (contains(vl, "fruits")) {
                         std::vector<std::vector<std::vector<uint>>> fruitUUIDs = cgen.getFruitUUIDs(p);
                         for(int c = 0; c < fruitUUIDs.size(); c++){ // loop over fruit clusters
                             annotation.labelPrimitives( flatten(fruitUUIDs.at(c)), "clusters" );
                         }
                     }
                 }
             }
```

### Comparing `agml-0.4.6/agml/synthetic/tools.py` & `agml-0.4.7/agml/synthetic/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/utils/__init__.py` & `agml-0.4.7/agml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/utils/data.py` & `agml-0.4.7/agml/utils/data.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/utils/downloads.py` & `agml-0.4.7/agml/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/utils/general.py` & `agml-0.4.7/agml/utils/general.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/utils/image.py` & `agml-0.4.7/agml/utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-
+import numpy as np
 import cv2
 
 
 def consistent_shapes(objects):
     """Determines whether the shapes of the objects are consistent."""
     try:
         shapes = [i.shape for i in objects]
```

### Comparing `agml-0.4.6/agml/utils/io.py` & `agml-0.4.7/agml/utils/io.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/utils/logging.py` & `agml-0.4.7/agml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/utils/random.py` & `agml-0.4.7/agml/utils/random.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/viz/__init__.py` & `agml-0.4.7/agml/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/viz/boxes.py` & `agml-0.4.7/agml/viz/boxes.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/viz/general.py` & `agml-0.4.7/agml/viz/general.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/viz/inspection.py` & `agml-0.4.7/agml/viz/inspection.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/viz/labels.py` & `agml-0.4.7/agml/viz/labels.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/viz/masks.py` & `agml-0.4.7/agml/viz/masks.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml/viz/tools.py` & `agml-0.4.7/agml/viz/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/agml.egg-info/PKG-INFO` & `agml-0.4.7/agml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agml
-Version: 0.4.6
+Version: 0.4.7
 Summary: A comprehensive library for agricultural deep learning
 Home-page: https://github.com/plant-ai-biophysics-lab/AgML
 Author: UC Davis Plant AI and Biophysics Lab
 Author-email: jmearles@ucdavis.edu
 Maintainer: Amogh Joshi
 Maintainer-email: amnjoshi@ucdavis.edu
 License: UNKNOWN
```

### Comparing `agml-0.4.6/agml.egg-info/SOURCES.txt` & `agml-0.4.7/agml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agml-0.4.6/setup.py` & `agml-0.4.7/setup.py`

 * *Files identical despite different names*

