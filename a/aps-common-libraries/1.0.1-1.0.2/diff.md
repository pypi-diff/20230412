# Comparing `tmp/aps_common_libraries-1.0.1.tar.gz` & `tmp/aps_common_libraries-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps_common_libraries-1.0.1.tar", last modified: Wed Mar  1 03:56:04 2023, max compression
+gzip compressed data, was "aps_common_libraries-1.0.2.tar", last modified: Tue Apr 11 22:35:08 2023, max compression
```

## Comparing `aps_common_libraries-1.0.1.tar` & `aps_common_libraries-1.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.410349 aps_common_libraries-1.0.1/
--rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.1/LICENSE
--rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.1/LICENSE.pdf
--rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.1/MANIFEST.in
--rw-r--r--   0 bishop    (1601)      907      876 2023-03-01 03:56:04.409820 aps_common_libraries-1.0.1/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.1/README.md
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.353192 aps_common_libraries-1.0.1/aps/
--rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.1/aps/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.360106 aps_common_libraries-1.0.1/aps/common/
--rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.1/aps/common/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.362086 aps_common_libraries-1.0.1/aps/common/__test/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.1/aps/common/__test/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.1/aps/common/__test/test.py
--rw-rw-rw-   0 bishop    (1601)      907    10103 2022-11-23 21:10:21.000000 aps_common_libraries-1.0.1/aps/common/initializer.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.365973 aps_common_libraries-1.0.1/aps/common/io/
--rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.1/aps/common/io/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.1/aps/common/io/printout.py
--rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.1/aps/common/io/tcp_client.py
--rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.1/aps/common/io/tiff_file.py
--rw-rw-rw-   0 bishop    (1601)      907    20742 2023-02-17 23:08:47.000000 aps_common_libraries-1.0.1/aps/common/logger.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.366977 aps_common_libraries-1.0.1/aps/common/measurment/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.1/aps/common/measurment/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.369901 aps_common_libraries-1.0.1/aps/common/measurment/beamline/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    10298 2022-11-28 17:44:19.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/image_collector.py
--rw-rw-rw-   0 bishop    (1601)      907    24907 2022-11-27 04:13:11.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/image_processor.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.383453 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/
--rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/SPINNet_estimate.py
--rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/WXST.py
--rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/diffraction_process.py
--rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/euclidean_dist.py
--rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/func.py
--rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/func_light.py
--rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/gui_func.py
--rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/integration.py
--rw-rw-rw-   0 bishop    (1601)      907    78095 2023-02-16 16:53:27.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/main.py
--rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/pattern_find.py
--rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/pattern_propagate.py
--rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/utils.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.386367 aps_common_libraries-1.0.1/aps/common/ml/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.1/aps/common/ml/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.1/aps/common/ml/data_structures.py
--rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.1/aps/common/ml/mocks.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.389762 aps_common_libraries-1.0.1/aps/common/plot/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.1/aps/common/plot/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    44400 2023-03-01 03:46:13.000000 aps_common_libraries-1.0.1/aps/common/plot/gui.py
--rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.1/aps/common/plot/image.py
--rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.1/aps/common/plot/qt_application.py
--rw-rw-rw-   0 bishop    (1601)      907    16718 2023-02-16 16:35:31.000000 aps_common_libraries-1.0.1/aps/common/plotter.py
--rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.1/aps/common/registry.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.396462 aps_common_libraries-1.0.1/aps/common/scripts/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.1/aps/common/scripts/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.1/aps/common/scripts/abstract_command_line_script.py
--rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.1/aps/common/scripts/generic_process_manager.py
--rw-rw-rw-   0 bishop    (1601)      907     7941 2023-02-17 23:04:17.000000 aps_common_libraries-1.0.1/aps/common/scripts/generic_qt_script.py
--rw-rw-rw-   0 bishop    (1601)      907     4121 2023-02-07 23:10:48.000000 aps_common_libraries-1.0.1/aps/common/scripts/script_data.py
--rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.1/aps/common/scripts/script_registry.py
--rw-rw-rw-   0 bishop    (1601)      907     4333 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.1/aps/common/singleton.py
--rw-rw-rw-   0 bishop    (1601)      907    10071 2022-11-28 18:33:01.000000 aps_common_libraries-1.0.1/aps/common/traffic_light.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.402028 aps_common_libraries-1.0.1/aps/common/widgets/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.1/aps/common/widgets/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.1/aps/common/widgets/close_app_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.1/aps/common/widgets/context_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.1/aps/common/widgets/generic_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.1/aps/common/widgets/log_stream_widget.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-03-01 03:56:04.408744 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/
--rw-rw-rw-   0 bishop    (1601)      907      876 2023-03-01 03:56:04.000000 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907     2130 2023-03-01 03:56:04.000000 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/SOURCES.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2023-03-01 03:56:04.000000 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/dependency_links.txt
--rw-rw-rw-   0 bishop    (1601)      907       15 2023-03-01 03:56:04.000000 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/namespace_packages.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/not-zip-safe
--rw-rw-rw-   0 bishop    (1601)      907      150 2023-03-01 03:56:04.000000 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/requires.txt
--rw-rw-rw-   0 bishop    (1601)      907        4 2023-03-01 03:56:04.000000 aps_common_libraries-1.0.1/aps_common_libraries.egg-info/top_level.txt
--rw-r--r--   0 bishop    (1601)      907       38 2023-03-01 03:56:04.410579 aps_common_libraries-1.0.1/setup.cfg
--rw-r--r--   0 bishop    (1601)      907     5571 2023-03-01 03:55:45.000000 aps_common_libraries-1.0.1/setup.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.324373 aps_common_libraries-1.0.2/
+-rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.2/LICENSE
+-rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.2/LICENSE.pdf
+-rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.2/MANIFEST.in
+-rw-r--r--   0 bishop    (1601)      907      876 2023-04-11 22:35:08.323834 aps_common_libraries-1.0.2/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.2/README.md
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.254948 aps_common_libraries-1.0.2/aps/
+-rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.2/aps/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.262629 aps_common_libraries-1.0.2/aps/common/
+-rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.2/aps/common/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.265199 aps_common_libraries-1.0.2/aps/common/__test/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.2/aps/common/__test/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.2/aps/common/__test/test.py
+-rw-rw-rw-   0 bishop    (1601)      907    10103 2022-11-23 21:10:21.000000 aps_common_libraries-1.0.2/aps/common/initializer.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.270137 aps_common_libraries-1.0.2/aps/common/io/
+-rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.2/aps/common/io/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.2/aps/common/io/printout.py
+-rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.2/aps/common/io/tcp_client.py
+-rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.2/aps/common/io/tiff_file.py
+-rw-rw-rw-   0 bishop    (1601)      907    20742 2023-02-17 23:08:47.000000 aps_common_libraries-1.0.2/aps/common/logger.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.271532 aps_common_libraries-1.0.2/aps/common/measurment/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.2/aps/common/measurment/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.275503 aps_common_libraries-1.0.2/aps/common/measurment/beamline/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_collector.py
+-rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_processor.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.294013 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/
+-rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/SPINNet_estimate.py
+-rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/WXST.py
+-rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/diffraction_process.py
+-rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/euclidean_dist.py
+-rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func.py
+-rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func_light.py
+-rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/gui_func.py
+-rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/integration.py
+-rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/main.py
+-rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_find.py
+-rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_propagate.py
+-rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/utils.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.297579 aps_common_libraries-1.0.2/aps/common/ml/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.2/aps/common/ml/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.2/aps/common/ml/data_structures.py
+-rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.2/aps/common/ml/mocks.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.301579 aps_common_libraries-1.0.2/aps/common/plot/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.2/aps/common/plot/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    44717 2023-04-08 13:27:45.000000 aps_common_libraries-1.0.2/aps/common/plot/gui.py
+-rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.2/aps/common/plot/image.py
+-rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.2/aps/common/plot/qt_application.py
+-rw-rw-rw-   0 bishop    (1601)      907    16718 2023-02-16 16:35:31.000000 aps_common_libraries-1.0.2/aps/common/plotter.py
+-rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.2/aps/common/registry.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.310701 aps_common_libraries-1.0.2/aps/common/scripts/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.2/aps/common/scripts/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.2/aps/common/scripts/abstract_command_line_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.2/aps/common/scripts/generic_process_manager.py
+-rw-rw-rw-   0 bishop    (1601)      907     7941 2023-02-17 23:04:17.000000 aps_common_libraries-1.0.2/aps/common/scripts/generic_qt_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     4121 2023-02-07 23:10:48.000000 aps_common_libraries-1.0.2/aps/common/scripts/script_data.py
+-rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.2/aps/common/scripts/script_registry.py
+-rw-rw-rw-   0 bishop    (1601)      907     4333 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.2/aps/common/singleton.py
+-rw-rw-rw-   0 bishop    (1601)      907    10071 2022-11-28 18:33:01.000000 aps_common_libraries-1.0.2/aps/common/traffic_light.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.316307 aps_common_libraries-1.0.2/aps/common/widgets/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.2/aps/common/widgets/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.2/aps/common/widgets/close_app_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.2/aps/common/widgets/context_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.2/aps/common/widgets/generic_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.2/aps/common/widgets/log_stream_widget.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.322829 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/
+-rw-rw-rw-   0 bishop    (1601)      907      876 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     2130 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/SOURCES.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/dependency_links.txt
+-rw-rw-rw-   0 bishop    (1601)      907       15 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/namespace_packages.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/not-zip-safe
+-rw-rw-rw-   0 bishop    (1601)      907      150 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/requires.txt
+-rw-rw-rw-   0 bishop    (1601)      907        4 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907       38 2023-04-11 22:35:08.324585 aps_common_libraries-1.0.2/setup.cfg
+-rw-r--r--   0 bishop    (1601)      907     5571 2023-04-11 22:34:49.000000 aps_common_libraries-1.0.2/setup.py
```

### Comparing `aps_common_libraries-1.0.1/LICENSE` & `aps_common_libraries-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/LICENSE.pdf` & `aps_common_libraries-1.0.2/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/PKG-INFO` & `aps_common_libraries-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps_common_libraries
-Version: 1.0.1
+Version: 1.0.2
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.1/aps/__init__.py` & `aps_common_libraries-1.0.2/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/__init__.py` & `aps_common_libraries-1.0.2/aps/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/__test/__init__.py` & `aps_common_libraries-1.0.2/aps/common/__test/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/__test/test.py` & `aps_common_libraries-1.0.2/aps/common/__test/test.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/initializer.py` & `aps_common_libraries-1.0.2/aps/common/initializer.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/io/__init__.py` & `aps_common_libraries-1.0.2/aps/common/io/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/io/printout.py` & `aps_common_libraries-1.0.2/aps/common/io/printout.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/io/tcp_client.py` & `aps_common_libraries-1.0.2/aps/common/io/tcp_client.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/io/tiff_file.py` & `aps_common_libraries-1.0.2/aps/common/io/tiff_file.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/logger.py` & `aps_common_libraries-1.0.2/aps/common/logger.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/__init__.py` & `aps_common_libraries-1.0.2/aps/common/measurment/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/__init__.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/image_collector.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;        #
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER        #
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT      #
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN       #
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE         #
 # POSSIBILITY OF SUCH DAMAGE.                                             #
 # ----------------------------------------------------------------------- #
+import os
 import time
 from epics import PV
 import pickle
 from collections import OrderedDict
 
 from aps.common.initializer import IniMode, register_ini_instance, get_registered_ini_instance
 
@@ -57,27 +58,29 @@
                       ini_file_name="image_collector.ini",
                       application_name=APPLICATION_NAME,
                       verbose=False)
 ini_file = get_registered_ini_instance(APPLICATION_NAME)
 
 WAIT_TIME         = ini_file.get_float_from_ini(section="Execution", key="Wait-Time",     default=0.1)
 EXPOSURE_TIME     = ini_file.get_float_from_ini(section="Execution", key="Exposure-Time", default=0.3)
-FILE_NAME_PREFIX  = "sample_" + str(int(EXPOSURE_TIME*1000)) + "ms_"
 
 ini_file.set_value_at_ini(section="Execution",   key="Wait-Time",     value=WAIT_TIME)
 ini_file.set_value_at_ini(section="Execution",   key="Exposure-Time", value=EXPOSURE_TIME)
 ini_file.push()
 
 IMAGE_COLLECTOR_STATUS_FILE = "image_collector_status.pkl"
 
-class ImageCollector():
+def get_default_file_name_prefix(exposure_time=EXPOSURE_TIME):
+    return "sample_" + str(int(exposure_time * 1000)) + "ms"
 
-    def __init__(self, measurement_directory, exposure_time=EXPOSURE_TIME, detector_delay=None, mocking_mode=False):
+class ImageCollector():
+    def __init__(self, measurement_directory, exposure_time=EXPOSURE_TIME, file_name_prefix=None, detector_delay=None, mocking_mode=False):
         self.__exposure_time         = exposure_time
         self.__measurement_directory = measurement_directory
+        self.__file_name_prefix      = get_default_file_name_prefix() if file_name_prefix is None else file_name_prefix
         self.__mocking_mode          = mocking_mode
 
         if not self.__mocking_mode:
             self.__PV_dict = dict(
                 andor_cam_acquire        = PV("dp_andor3_skylark:cam1:Acquire"),  # 0="Done", 1="Acquire"
                 andor_cam_exposure_time  = PV("dp_andor3_skylark:cam1:AcquireTime"),
                 andor_cam_image_mode     = PV("dp_andor3_skylark:cam1:ImageMode"),    # "Fixed" or "Continuous"
@@ -137,15 +140,14 @@
     def restore_status(self):
         self.__detector_stop()  # 1 waiting time
         self.__from_pickle_file()
 
     def collect_single_shot_image(self, index=1):
         if not self.__mocking_mode:
             self.__initialize_current_image(index)
-
             self.__detector_acquire() # 2 waiting time + exposure time
         else:
             time.sleep(self.get_total_acquisition_time())
             print("Mocking Mode: collected image #" + str(index))
 
     def end_collection(self): # to be done at the end of the data collection
         if not self.__mocking_mode:
@@ -179,15 +181,15 @@
 
     def __set_andor_defaults(self, index):
         self.__PV_dict["andor_cam_image_mode"].put("Fixed")
         self.__PV_dict["andor_cam_exposure_time"].put(self.__exposure_time)
         self.__PV_dict["andor_tiff_filepath"].put(self.__measurement_directory)
         self.__PV_dict["andor_tiff_autosave"].put("Yes")
         self.__PV_dict["andor_tiff_autoincrement"].put("No")
-        self.__PV_dict["andor_tiff_filename"].put('sample_' + str(int(self.__exposure_time * 1000)) + 'ms')
+        self.__PV_dict["andor_tiff_filename"].put(self.__file_name_prefix)
         if index > 0: self.__PV_dict["andor_tiff_filenumber"].put(index)
 
     def __detector_delay(self):
         if not self.__has_delay:
             time.sleep(self.__exposure_time + WAIT_TIME)
         else:
             time.sleep(WAIT_TIME)  # wait for the detector to start
```

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/image_processor.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -48,36 +48,117 @@
 import glob
 import random
 import threading
 import time
 import pathlib
 import numpy
 
-from aps.common.measurment.beamline.image_collector import FILE_NAME_PREFIX
+from aps.common.initializer import IniMode, register_ini_instance, get_registered_ini_instance
+
+from aps.common.measurment.beamline.image_collector import get_default_file_name_prefix
 from aps.common.measurment.beamline.wf import SCRIPT_DIRECTORY
 
-PIXEL_SIZE           = 0.65e-6
-IMAGE_SIZE_PIXEL_HxV = [2160, 2560]
+APPLICATION_NAME = "IMAGE-PROCESSOR"
+
+register_ini_instance(IniMode.LOCAL_FILE,
+                      ini_file_name="image_processor.ini",
+                      application_name=APPLICATION_NAME,
+                      verbose=False)
+ini_file = get_registered_ini_instance(APPLICATION_NAME)
+
+PYTHON                = ini_file.get_string_from_ini( section="Python", key="Python-Executable", default="python")
+
+PIXEL_SIZE            = ini_file.get_float_from_ini(  section="Detector", key="Pixel-Size", default=0.65e-6)
+IMAGE_SIZE_PIXEL_HxV  = ini_file.get_list_from_ini(   section="Detector", key="Image-Size", default=[2160, 2560], type=int)
+
+PATTERN_SIZE          = ini_file.get_float_from_ini(  section="Mask", key="Pattern-Size",         default=4.942e-6)
+PATTERN_THICKNESS     = ini_file.get_float_from_ini(  section="Mask", key="Pattern-Thickness",    default=1.5e-6)
+PATTERN_T             = ini_file.get_float_from_ini(  section="Mask", key="Pattern-Transmission", default=0.613)
+RAN_MASK              = ini_file.get_string_from_ini( section="Mask", key="Pattern-Image",        default='RanMask5umB0.npy')
+D_PROP                = ini_file.get_float_from_ini(  section="Mask", key="Propagation-Distance", default=500e-3)
+
+SOURCE_V              = ini_file.get_float_from_ini(  section="Source", key="Source-Size-V",     default=6.925e-6)
+SOURCE_H              = ini_file.get_float_from_ini(  section="Source", key="Source-Size-H",     default=0.333e-6)
+SOURCE_DISTANCE_V     = ini_file.get_float_from_ini(  section="Source", key="Source-Distance-V", default=1.5)
+SOURCE_DISTANCE_H     = ini_file.get_float_from_ini(  section="Source", key="Source-Distance-H", default=1.5)
+
+D_SOURCE_RECAL        = ini_file.get_boolean_from_ini(section="Execution", key="Source-Distance-Recalculation", default=True)
+CROP                  = ini_file.get_list_from_ini(   section="Execution", key="Crop",                          default=[-1], type=int)
+ESTIMATION_METHOD     = ini_file.get_string_from_ini( section="Execution", key="Estimation-Method",             default='simple_speckle')
+
+MODE                  = ini_file.get_string_from_ini( section="Reconstruction", key="Mode",           default='centralLine')
+LINE_WIDTH            = ini_file.get_int_from_ini(    section="Reconstruction", key="Line-Width",     default=10)
+LINE_DIRECTION        = ini_file.get_string_from_ini( section="Reconstruction", key="Line-Direction", default='b')
+DOWN_SAMPLING         = ini_file.get_float_from_ini(  section="Reconstruction", key="Down-Sampling",  default=0.5)
+METHOD                = ini_file.get_string_from_ini( section="Reconstruction", key="Method",         default='WXST')
+USE_GPU               = ini_file.get_boolean_from_ini(section="Reconstruction", key="Use-Gpu",        default=True)
+USE_WAVELET           = ini_file.get_boolean_from_ini(section="Reconstruction", key="Use-Wavelet",    default=True)
+WAVELET_CUT           = ini_file.get_int_from_ini(    section="Reconstruction", key="Wavelet-Cut",    default=1)
+PYRAMID_LEVEL         = ini_file.get_int_from_ini(    section="Reconstruction", key="Pyramid-Level",  default=1)
+TEMPLATE_SIZE         = ini_file.get_int_from_ini(    section="Reconstruction", key="Template-Size",  default=21)
+WINDOW_SEARCH         = ini_file.get_int_from_ini(    section="Reconstruction", key="Window-Search",  default=20)
+CROP_BOUNDARY         = ini_file.get_int_from_ini(    section="Reconstruction", key="Crop-Boundary",  default=-1)
+N_CORES               = ini_file.get_int_from_ini(    section="Reconstruction", key="N-Cores",        default=16)
+N_GROUP               = ini_file.get_int_from_ini(    section="Reconstruction", key="N-Group",        default=1)
+
+IMAGE_TRANSFER_MATRIX = ini_file.get_list_from_ini(   section="Output", key="Image-Transfer-Matrix", default=[0, 1, 0], type=int)
+SHOW_ALIGN_FIGURE     = ini_file.get_boolean_from_ini(section="Output", key="Show-Align-Figure",     default=False)
+
+ini_file.set_value_at_ini(section="Python",   key="Python-Executable", value=PYTHON)
+
+ini_file.set_value_at_ini(section="Detector", key="Pixel-Size", value=PIXEL_SIZE)
+ini_file.set_list_at_ini( section="Detector", key="Image-Size", values_list=IMAGE_SIZE_PIXEL_HxV)
+
+ini_file.set_value_at_ini(section="Mask", key="Pattern-Size",         value=PATTERN_SIZE)
+ini_file.set_value_at_ini(section="Mask", key="Pattern-Thickness",    value=PATTERN_THICKNESS)
+ini_file.set_value_at_ini(section="Mask", key="Pattern-Transmission", value=PATTERN_T)
+ini_file.set_value_at_ini(section="Mask", key="Pattern-Image",        value=RAN_MASK)
+ini_file.set_value_at_ini(section="Mask", key="Propagation-Distance", value=D_PROP)
+
+ini_file.set_value_at_ini(section="Source", key="Source-Size-V",        value=SOURCE_V)
+ini_file.set_value_at_ini(section="Source", key="Source-Size-H",        value=SOURCE_H)
+ini_file.set_value_at_ini(section="Source", key="Source-Distance-V",    value=SOURCE_DISTANCE_V)
+ini_file.set_value_at_ini(section="Source", key="Source-Distance-H",    value=SOURCE_DISTANCE_H)
+
+ini_file.set_value_at_ini(section="Execution", key="Source-Distance-Recalculation", value=D_SOURCE_RECAL)
+ini_file.set_list_at_ini( section="Execution", key="Crop",                          values_list=CROP)
+ini_file.set_value_at_ini(section="Execution", key="Estimation-Method",             value=ESTIMATION_METHOD)
+
+ini_file.set_value_at_ini(section="Reconstruction", key="Mode",           value=MODE)
+ini_file.set_value_at_ini(section="Reconstruction", key="Line-Width",     value=LINE_WIDTH   )
+ini_file.set_value_at_ini(section="Reconstruction", key="Line-Direction", value=LINE_DIRECTION)
+ini_file.set_value_at_ini(section="Reconstruction", key="Down-Sampling",  value=DOWN_SAMPLING)
+ini_file.set_value_at_ini(section="Reconstruction", key="Method",         value=METHOD       )
+ini_file.set_value_at_ini(section="Reconstruction", key="Use-Gpu",        value=USE_GPU      )
+ini_file.set_value_at_ini(section="Reconstruction", key="Use-Wavelet",    value=USE_WAVELET  )
+ini_file.set_value_at_ini(section="Reconstruction", key="Wavelet-Cut",    value=WAVELET_CUT  )
+ini_file.set_value_at_ini(section="Reconstruction", key="Pyramid-Level",  value=PYRAMID_LEVEL)
+ini_file.set_value_at_ini(section="Reconstruction", key="Template-Size",  value=TEMPLATE_SIZE)
+ini_file.set_value_at_ini(section="Reconstruction", key="Window-Search",  value=WINDOW_SEARCH)
+ini_file.set_value_at_ini(section="Reconstruction", key="Crop-Boundary",  value=CROP_BOUNDARY)
+ini_file.set_value_at_ini(section="Reconstruction", key="N-Cores",        value=N_CORES      )
+ini_file.set_value_at_ini(section="Reconstruction", key="N-Group",        value=N_GROUP      )
+
+ini_file.set_list_at_ini( section="Output", key="Image-Transfer-Matrix", values_list=IMAGE_TRANSFER_MATRIX)
+ini_file.set_value_at_ini(section="Output", key="Show-Align-Figure",     value=SHOW_ALIGN_FIGURE)
+
+ini_file.push()
 
 class ImageProcessor():
     def __init__(self,
                  data_collection_directory,
-                 file_name_prefix=FILE_NAME_PREFIX,
+                 file_name_prefix=get_default_file_name_prefix(),
                  simulated_mask_directory=None,
-                 energy=20000.0,
-                 source_distance=[1.5, 1.5],
-                 image_transfer_matrix=[0, 1, 0]
-                 ):
+                 energy=20000.0):
         self.__data_collection_directory = data_collection_directory
         self.__file_name_prefix          = file_name_prefix
         self.__simulated_mask_directory  = simulated_mask_directory
         self.__energy                    = energy
-        self.__source_distance           = source_distance
-        self.__image_transfer_matrix     = image_transfer_matrix
-
+        self.__source_distance           = [SOURCE_DISTANCE_H, SOURCE_DISTANCE_V]
+        self.__image_transfer_matrix     = IMAGE_TRANSFER_MATRIX
 
     def generate_simulated_mask(self, image_index_for_mask=1, verbose=False):
         self.__image_transfer_matrix, is_new_mask = _generate_simulated_mask(data_collection_directory=self.__data_collection_directory,
                                                                              file_name_prefix=self.__file_name_prefix,
                                                                              mask_directory=self.__simulated_mask_directory,
                                                                              energy=self.__energy,
                                                                              source_distance=self.__source_distance,
@@ -164,15 +245,15 @@
                 else: image_indexes.append(int(image_directory[-5:]))
             return image_indexes
 
         max_waiting_cycles = 60
         waiting_cycles     = 0
 
         while waiting_cycles < max_waiting_cycles:
-            images_list   = glob.glob(os.path.join(self.__data_collection_directory, self.__file_name_prefix + '*.tif'), recursive=False)
+            images_list   = glob.glob(os.path.join(self.__data_collection_directory, self.__file_name_prefix + '_*.tif'), recursive=False)
             if len(images_list) == 0:
                 waiting_cycles += 1
                 print('Thread #' + str(self.__thread_id) + ' waiting for 1s for new data....')
             else:
                 image_indexes = check_new_data(images_list)
 
                 if len(image_indexes) == 0:
@@ -195,234 +276,244 @@
 
         print('Thread #' + str(self.__thread_id) + ' completed')
 
 
 def _get_image_data(data_collection_directory, file_name_prefix, mask_directory, energy, source_distance, image_transfer_matrix, image_index, verbose):
     dark = None
     flat = None
-    image_path       = os.path.join(data_collection_directory, file_name_prefix + "%05i.tif" % image_index)
+    image_path       = os.path.join(data_collection_directory, file_name_prefix + "_%05i.tif" % image_index)
     mask_directory   = os.path.join(data_collection_directory, "simulated_mask") if mask_directory is None else mask_directory
     result_directory = os.path.join(os.path.dirname(image_path), os.path.basename(image_path).split('.tif')[0])
 
     # pattern simulation parameters
-    pattern_path          = os.path.join(SCRIPT_DIRECTORY, 'mask', 'RanMask5umB0.npy')
+    pattern_path          = os.path.join(SCRIPT_DIRECTORY, 'mask', RAN_MASK)
     propagated_pattern    = os.path.join(mask_directory, 'propagated_pattern.npz')
     propagated_patternDet = os.path.join(mask_directory, 'propagated_patternDet.npz')
 
-    crop                 = ' '.join([str(k) for k in [-1]])
+    crop                 = ' '.join([str(k) for k in CROP])
     img_transfer_matrix  = ' '.join([str(k) for k in image_transfer_matrix])
     find_transfer_matrix = False
     p_x                  = PIXEL_SIZE
     det_array            = str(IMAGE_SIZE_PIXEL_HxV[1]) + " " + str(IMAGE_SIZE_PIXEL_HxV[0])
-    pattern_size         = 4.942e-6  # 4.952e-6
-    pattern_thickness    = 1.5e-6
-    pattern_T            = 0.613
-    d_prop               = 500e-3
-    source_h             = 277e-6 / (60 / 1.5)
-    source_v             = 10e-6 / (60 / 2)
+    pattern_size         = PATTERN_SIZE
+    pattern_thickness    = PATTERN_THICKNESS
+    pattern_T            = PATTERN_T
+    d_prop               = D_PROP
+    source_h             = SOURCE_H
+    source_v             = SOURCE_V
     d_source_h           = source_distance[0]
     d_source_v           = source_distance[1]
-    show_alignFigure     = False
+    show_align_figure    = SHOW_ALIGN_FIGURE
 
     # reconstruction parameter initialization
-    mode            = 'centralLine'  # area or centralLine
-    lineWidth       = 10
-    down_sampling   = 0.5
-    method          = 'WXST'
-    use_gpu         = True
-    use_wavelet     = True
-    wavelet_cut     = 1
-    pyramid_level   = 1
-    template_size   = 21
-    window_search   = 20
-    crop_boundary   = -1
-    n_cores         = 16
-    n_group         = 1
-    verbose         = 1 if verbose else 0 # NO
+    mode            = MODE  # area or centralLine
+    lineWidth       = LINE_WIDTH
+    lineDirection   = LINE_DIRECTION
+    down_sampling   = DOWN_SAMPLING
+    method          = METHOD
+    use_gpu         = USE_GPU
+    use_wavelet     = USE_WAVELET
+    wavelet_cut     = WAVELET_CUT
+    pyramid_level   = PYRAMID_LEVEL
+    template_size   = TEMPLATE_SIZE
+    window_search   = WINDOW_SEARCH
+    crop_boundary   = CROP_BOUNDARY
+    n_cores         = N_CORES
+    n_group         = N_GROUP
+    verbose         = 0 if verbose else 1 # NO
     simple_analysis = 1
 
     # alignment or not, if '', no alignment, '--alignment' with alignment
     params = ['--GPU ' if use_gpu else ''] + ['--use_wavelet ' if use_wavelet else ''] + [
-        '--show_alignFigure ' if show_alignFigure else ''] + ['--find_transferMatrix ' if find_transfer_matrix else '']
+        '--show_alignFigure ' if show_align_figure else ''] + ['--find_transferMatrix ' if find_transfer_matrix else '']
     params = ''.join([str(item) for item in params])
 
-    command = 'python ' + os.path.join(SCRIPT_DIRECTORY, 'main.py') + \
+    command = PYTHON + ' '  + os.path.join(SCRIPT_DIRECTORY, 'main.py') + \
               ' --img {} --dark {} --flat {} --result_folder {} --pattern_path {} ' \
               '--propagated_pattern {} --propagated_patternDet {} --crop {} --det_size {} ' \
               '--img_transfer_matrix {} --p_x {} --energy {} --pattern_size {} --pattern_thickness {} ' \
               '--pattern_T {} --d_source_v {} --d_source_h {} --source_v {} --source_h {} --d_prop {} ' \
-              '--mode {} --lineWidth {} --down_sampling {} --method {} --wavelet_lv_cut {} ' \
+              '--mode {} --lineWidth {} --lineDirection {} --down_sampling {} --method {} --wavelet_lv_cut {} ' \
               '--pyramid_level {} --template_size {} --window_searching {} ' \
               '--nCores {} --nGroup {} --verbose {} --simple_analysis {} --crop_boundary {} {} '.format(image_path, dark, flat, result_directory,
                                                                       pattern_path, propagated_pattern,
                                                                       propagated_patternDet, crop, det_array,
                                                                       img_transfer_matrix, p_x, energy,
                                                                       pattern_size, pattern_thickness, pattern_T,
                                                                       d_source_v, d_source_h,
-                                                                      source_v, source_h, d_prop, mode, lineWidth,
+                                                                      source_v, source_h, d_prop, mode, lineWidth, lineDirection,
                                                                       down_sampling, method,
                                                                       wavelet_cut, pyramid_level, template_size,
                                                                       window_search, n_cores,
                                                                       n_group, verbose, simple_analysis, crop_boundary, params)
-    os.system(command)
+    ret_val = os.system(command)
+
+    if ret_val != 0: raise Exception("Wavefront analysis failed")
 
     with open(os.path.join(result_directory, "raw_image.npy"), 'rb') as f: image = numpy.load(f, allow_pickle=False).T
 
     h_coord = numpy.linspace(-IMAGE_SIZE_PIXEL_HxV[0] / 2, IMAGE_SIZE_PIXEL_HxV[0] / 2, IMAGE_SIZE_PIXEL_HxV[0]) * PIXEL_SIZE * 1e3
     v_coord = numpy.linspace(-IMAGE_SIZE_PIXEL_HxV[1] / 2, IMAGE_SIZE_PIXEL_HxV[1] / 2, IMAGE_SIZE_PIXEL_HxV[1]) * PIXEL_SIZE * 1e3
 
     return image, h_coord, v_coord
 
 def _process_image(data_collection_directory, file_name_prefix, mask_directory, energy, source_distance, image_transfer_matrix, image_index, verbose):
     dark = None
     flat = None
-    image_path       = os.path.join(data_collection_directory, file_name_prefix + "%05i.tif" % image_index)
+    image_path       = os.path.join(data_collection_directory, file_name_prefix + "_%05i.tif" % image_index)
     mask_directory   = os.path.join(data_collection_directory, "simulated_mask") if mask_directory is None else mask_directory
     result_directory = os.path.join(os.path.dirname(image_path), os.path.basename(image_path).split('.tif')[0])
 
     # pattern simulation parameters
-    pattern_path          = os.path.join(SCRIPT_DIRECTORY, 'mask' , 'RanMask5umB0.npy')
+    pattern_path          = os.path.join(SCRIPT_DIRECTORY, 'mask' , RAN_MASK)
     propagated_pattern    = os.path.join(mask_directory, 'propagated_pattern.npz')
     propagated_patternDet = os.path.join(mask_directory, 'propagated_patternDet.npz')
 
-    crop                 = ' '.join([str(k) for k in [-1]])
+    crop                 = ' '.join([str(k) for k in CROP])
     img_transfer_matrix  = ' '.join([str(k) for k in image_transfer_matrix])
     find_transfer_matrix = False
     p_x                  = PIXEL_SIZE
     det_array            = str(IMAGE_SIZE_PIXEL_HxV[1]) + " " + str(IMAGE_SIZE_PIXEL_HxV[0])
-    pattern_size         = 4.942e-6  # 4.952e-6
-    pattern_thickness    = 1.5e-6
-    pattern_T            = 0.613
-    d_prop               = 500e-3
-    source_h             = 277e-6 / (60 / 1.5)
-    source_v             = 10e-6 / (60 / 2)
+    pattern_size         = PATTERN_SIZE
+    pattern_thickness    = PATTERN_THICKNESS
+    pattern_T            = PATTERN_T
+    d_prop               = D_PROP
+    source_h             = SOURCE_H
+    source_v             = SOURCE_V
     d_source_h           = source_distance[0]
     d_source_v           = source_distance[1]
-    show_alignFigure     = False
+    show_align_figure    = SHOW_ALIGN_FIGURE
 
     # reconstruction parameter initialization
-    mode            = 'centralLine'  # area or centralLine
-    lineWidth       = 10
-    down_sampling   = 0.5
-    method          = 'WXST'
-    use_gpu         = True
-    use_wavelet     = True
-    wavelet_cut     = 1
-    pyramid_level   = 1
-    template_size   = 21
-    window_search   = 20
-    crop_boundary   = -1
-    n_cores         = 16
-    n_group         = 1
-    verbose         = 1 if verbose else 0 # NO
+    mode            = MODE  # area or centralLine
+    lineWidth       = LINE_WIDTH
+    lineDirection   = LINE_DIRECTION
+    down_sampling   = DOWN_SAMPLING
+    method          = METHOD
+    use_gpu         = USE_GPU
+    use_wavelet     = USE_WAVELET
+    wavelet_cut     = WAVELET_CUT
+    pyramid_level   = PYRAMID_LEVEL
+    template_size   = TEMPLATE_SIZE
+    window_search   = WINDOW_SEARCH
+    crop_boundary   = CROP_BOUNDARY
+    n_cores         = N_CORES
+    n_group         = N_GROUP
+    verbose         = 0 if verbose else 1 # NO
     simple_analysis = 0 # NO
 
     # alignment or not, if '', no alignment, '--alignment' with alignment
     params = ['--GPU ' if use_gpu else ''] + ['--use_wavelet ' if use_wavelet else ''] + [
-        '--show_alignFigure ' if show_alignFigure else ''] + ['--find_transferMatrix ' if find_transfer_matrix else '']
+        '--show_alignFigure ' if show_align_figure else ''] + ['--find_transferMatrix ' if find_transfer_matrix else '']
     params = ''.join([str(item) for item in params])
 
-    command = 'python ' + os.path.join(SCRIPT_DIRECTORY, 'main.py') + \
+    command = PYTHON + ' '  + os.path.join(SCRIPT_DIRECTORY, 'main.py') + \
               ' --img {} --dark {} --flat {} --result_folder {} --pattern_path {} ' \
               '--propagated_pattern {} --propagated_patternDet {} --crop {} --det_size {} ' \
               '--img_transfer_matrix {} --p_x {} --energy {} --pattern_size {} --pattern_thickness {} ' \
               '--pattern_T {} --d_source_v {} --d_source_h {} --source_v {} --source_h {} --d_prop {} ' \
-              '--mode {} --lineWidth {} --down_sampling {} --method {} --wavelet_lv_cut {} ' \
+              '--mode {} --lineWidth {} --lineDirection {} --down_sampling {} --method {} --wavelet_lv_cut {} ' \
               '--pyramid_level {} --template_size {} --window_searching {} ' \
               '--nCores {} --nGroup {} --verbose {} --simple_analysis {} --crop_boundary {} {} '.format(image_path, dark, flat, result_directory,
                                                                       pattern_path, propagated_pattern,
                                                                       propagated_patternDet, crop, det_array,
                                                                       img_transfer_matrix, p_x, energy,
                                                                       pattern_size, pattern_thickness, pattern_T,
                                                                       d_source_v, d_source_h,
-                                                                      source_v, source_h, d_prop, mode, lineWidth,
+                                                                      source_v, source_h, d_prop, mode, lineWidth, lineDirection,
                                                                       down_sampling, method,
                                                                       wavelet_cut, pyramid_level, template_size,
                                                                       window_search, n_cores,
                                                                       n_group, verbose, simple_analysis, crop_boundary, params)
-    os.system(command)
+    ret_val = os.system(command)
 
-    print("Image " + file_name_prefix + "%05i.tif" % image_index + " processed")
+    if ret_val != 0: raise Exception("Wavefront analysis failed")
+    else:            print("Image " + file_name_prefix + "_%05i.tif" % image_index + " processed")
 
 def _generate_simulated_mask(data_collection_directory, file_name_prefix, mask_directory, energy, source_distance, image_index=1, verbose=False):
     dark = None
     flat = None
-    image_path      = os.path.join(data_collection_directory, file_name_prefix + "%05i.tif" % image_index)
+    image_path      = os.path.join(data_collection_directory, file_name_prefix + "_%05i.tif" % image_index)
     mask_directory  = os.path.join(data_collection_directory, "simulated_mask") if mask_directory is None else mask_directory
     is_new_mask     = True
 
     if not os.path.exists(mask_directory): os.mkdir(mask_directory)
 
     if not os.path.exists(os.path.join(mask_directory, 'propagated_pattern.npz')) or \
        not os.path.exists(os.path.join(mask_directory, 'propagated_patternDet.npz')) or \
        not os.path.exists(os.path.join(mask_directory, "image_transfer_matrix.npy")):
 
         result_directory = os.path.join(os.path.dirname(image_path), os.path.basename(image_path).split('.tif')[0])
 
         # pattern simulation parameters
-        pattern_path          = os.path.join(SCRIPT_DIRECTORY, 'mask', 'RanMask5umB0.npy')
+        pattern_path          = os.path.join(SCRIPT_DIRECTORY, 'mask', RAN_MASK)
         propagated_pattern    = None
         propagated_patternDet = None
+        estimation_method     = ESTIMATION_METHOD
 
-        crop                 = ' '.join([str(k) for k in [-1]])
+        crop                 = ' '.join([str(k) for k in CROP])
         find_transfer_matrix = True
         p_x                  = PIXEL_SIZE
         det_array            = str(IMAGE_SIZE_PIXEL_HxV[1]) + " " + str(IMAGE_SIZE_PIXEL_HxV[0])
-        pattern_size         = 4.942e-6  # 4.952e-6
-        pattern_thickness    = 1.5e-6
-        pattern_T            = 0.613
-        d_prop               = 500e-3
-        source_h             = 277e-6 / (60 / 1.5)
-        source_v             = 10e-6 / (60 / 2)
+        pattern_size         = PATTERN_SIZE
+        pattern_thickness    = PATTERN_THICKNESS
+        pattern_T            = PATTERN_T
+        d_prop               = D_PROP
+        source_h             = SOURCE_H
+        source_v             = SOURCE_V
         d_source_h           = source_distance[0]
         d_source_v           = source_distance[1]
-        show_alignFigure     = False
+        show_align_figure    = SHOW_ALIGN_FIGURE
 
         # reconstruction parameter initialization
-        mode            = 'centralLine'  # area or centralLine
-        lineWidth       = 10
-        down_sampling   = 0.5
-        method          = 'WXST'
-        use_gpu         = True
-        use_wavelet     = True
-        wavelet_cut     = 1
-        pyramid_level   = 1
-        template_size   = 21
-        window_search   = 20
-        crop_boundary   = -1
-        n_cores         = 16
-        n_group         = 1
-        verbose         = 1 if verbose else 0 # NO
+        mode = MODE  # area or centralLine
+        lineWidth = LINE_WIDTH
+        lineDirection = LINE_DIRECTION
+        down_sampling = DOWN_SAMPLING
+        method = METHOD
+        use_gpu = USE_GPU
+        use_wavelet = USE_WAVELET
+        wavelet_cut = WAVELET_CUT
+        pyramid_level = PYRAMID_LEVEL
+        template_size = TEMPLATE_SIZE
+        window_search = WINDOW_SEARCH
+        crop_boundary = CROP_BOUNDARY
+        n_cores = N_CORES
+        n_group = N_GROUP
+        verbose         = 0 if verbose else 1 # NO
         simple_analysis = 0 # NO
 
         # alignment or not, if '', no alignment, '--alignment' with alignment
-        params = ['--GPU ' if use_gpu else ''] + ['--use_wavelet ' if use_wavelet else ''] + [
-            '--show_alignFigure ' if show_alignFigure else ''] + ['--find_transferMatrix ' if find_transfer_matrix else '']
+        params = ['--GPU ' if use_gpu else ''] + ['--use_wavelet ' if use_wavelet else ''] + \
+                 ['--show_alignFigure ' if show_align_figure else ''] + \
+                 ['--find_transferMatrix ' if find_transfer_matrix else ''] + \
+                 ['--d_source_recal ' if D_SOURCE_RECAL else '']
         params = ''.join([str(item) for item in params])
 
-        command = 'python ' + os.path.join(SCRIPT_DIRECTORY, 'main.py') + \
+        command = PYTHON + ' '  + os.path.join(SCRIPT_DIRECTORY, 'main.py') + \
                   ' --img {} --dark {} --flat {} --result_folder {} --pattern_path {} ' \
-                  '--propagated_pattern {} --propagated_patternDet {} --saving_path {} --crop {} --det_size {} ' \
+                  '--propagated_pattern {} --propagated_patternDet {} --estimation_method {} --saving_path {} --crop {} --det_size {} ' \
                   '--p_x {} --energy {} --pattern_size {} --pattern_thickness {} ' \
                   '--pattern_T {} --d_source_v {} --d_source_h {} --source_v {} --source_h {} --d_prop {} ' \
-                  '--d_source_recal --find_transferMatrix --mode {} --lineWidth {} --down_sampling {} --method {} --wavelet_lv_cut {} ' \
+                  '--mode {} --lineWidth {} --lineDirection {} --down_sampling {} --method {} --wavelet_lv_cut {} ' \
                   '--pyramid_level {} --template_size {} --window_searching {} ' \
                   '--nCores {} --nGroup {} --verbose {} --simple_analysis {} --crop_boundary {} {} '.format(image_path, dark, flat, result_directory,
-                                                                          pattern_path, propagated_pattern, propagated_patternDet, mask_directory,
+                                                                          pattern_path, propagated_pattern, propagated_patternDet, estimation_method, mask_directory,
                                                                           crop, det_array, p_x, energy,
                                                                           pattern_size, pattern_thickness, pattern_T,
                                                                           d_source_v, d_source_h,
-                                                                          source_v, source_h, d_prop, mode, lineWidth,
+                                                                          source_v, source_h, d_prop, mode, lineWidth, lineDirection,
                                                                           down_sampling, method,
                                                                           wavelet_cut, pyramid_level, template_size,
                                                                           window_search, n_cores,
                                                                           n_group, verbose, simple_analysis, crop_boundary, params)
-        os.system(command)
+        ret_val = os.system(command)
 
-        print("Simulated mask generated in " + mask_directory)
+        if ret_val != 0: raise Exception("Wavefront analysis failed")
+        else:            print("Simulated mask generated in " + mask_directory)
     else:
         is_new_mask = False
         print("Simulated mask already generated in " + mask_directory)
 
     with open(os.path.join(mask_directory, "image_transfer_matrix.npy"), 'rb') as f: image_transfer_matrix = numpy.load(f, allow_pickle=False)
 
     return image_transfer_matrix.tolist(), is_new_mask
```

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/SPINNet_estimate.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/SPINNet_estimate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/WXST.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/WXST.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/__init__.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/diffraction_process.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/diffraction_process.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/euclidean_dist.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/euclidean_dist.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/func.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/func_light.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/gui_func.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/gui_func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/integration.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/integration.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/main.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         I_pattern = normalize(I_pattern)
 
         # scale for pattern pitch to detector pixel size
         scale = self.pattern_pixel / self.p_x
 
         # I_pattern = rescale(I_pattern, scale)
         size_origin = I_pattern.shape
-        I_pattern = cv2.resize(I_pattern, (int(I_pattern.shape[0]*scale), int(I_pattern.shape[1]*scale)), interpolation = cv2.INTER_NEAREST)
+        I_pattern = cv2.resize(I_pattern, (int(I_pattern.shape[1]*scale), int(I_pattern.shape[0]*scale)), interpolation = cv2.INTER_NEAREST)
         # I_pattern = cv2.resize(I_pattern, (int(I_pattern.shape[0]*scale), int(I_pattern.shape[1]*scale)))
         # I_pattern = snd.zoom(I_pattern, scale, order=0)
         # I_pattern = np.repeat(np.repeat(I_pattern, int(scale), axis=0),
         #                       int(scale),
         #                       axis=1)
         # the pixel size after repeating expanding the matrix. Should be noted that, use nearest or linear or other interplation induces extra artifacts in the propgated pattern. So use this int pixel size for propagation and then scale the propgated pattern with the correct scales
         # p_x_prop = self.pattern_pixel / int(scale)
@@ -1057,15 +1057,14 @@
             I_simu_whole, displace_x_offset, displace_y_offset = pattern_find.pattern_search(I_img_central, I_coh, image_transfer_matrix)
         else:
             I_simu_whole, displace_x_offset, displace_y_offset = pattern_find.pattern_search(I_img_central, I_coh, image_transfer_matrix)
 
         with open(os.path.join(para_pattern['saving_path'], "image_transfer_matrix.npy"), 'wb') as f: np.save(f, np.array(image_transfer_matrix), allow_pickle=False)
 
     if method == 'geometric':
-
         d_source_v, d_source_h = pattern_find.d_source_est                                          
         prColor('re-calculated source distance: {}y    {}x'.format(d_source_v, d_source_h), 'cyan')
 
         return [d_source_v, d_source_h]
     elif method == 'simple_speckle':
         I_simu = boundary_crop(I_simu_whole)
         displace_y_offset = boundary_crop(displace_y_offset)
@@ -1089,16 +1088,14 @@
         prColor('re-calculated source distance: {}y    {}x'.format(1/np.mean(curve_y), 1/np.mean(curve_x)), 'cyan')
 
         return [1/np.mean(curve_y), 1/np.mean(curve_x)]
     else:
         prColor('Wrong method for source distance re-calculation', 'red')
 
 if __name__ == "__main__":
-    print("WF ANALYSYS SCRIPT - NEW")
-
     # paremater settings
     parser = argparse.ArgumentParser(
         description='experimental data analysis for absolute phase measurement',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     # shared args
     # ============================================================
@@ -1126,15 +1123,22 @@
     parser.add_argument('--propagated_pattern',
                         type=str,
                         default='./images/1DCRL/propagated_pattern.npz',
                         help='if None, will create one in the data folder')
     parser.add_argument('--propagated_patternDet',
                         type=str,
                         default='./images/1DCRL/propagated_patternDet.npz',
-                        help='if None, will search from the propagated pattern. Its size is determined by the det_size')                    
+                        help='if None, will search from the propagated pattern. Its size is determined by the det_size')
+
+    parser.add_argument('--estimation_method',
+                        type=str,
+                        default='simple_speckle',
+                        help='simple_speckle or geometric: simple_speckle means using the slope_tracking to estimate the overall source distance;\n' + \
+                             'geometric means using the image scalling factor to get the overall source distance')
+
     parser.add_argument(
         '--saving_path',
         type=str,
         default=None,
         help='if None, will save the propagated pattern file to the data folder'
     )
 
@@ -1235,14 +1239,15 @@
                         "--mode",
                         default='area',
                         type=str,
                         help=
                         'mode for speckle tracking. area: whole crop area; centralLine: vertical and horizontal central line with a width of parser.lineWidth;'
     )
     parser.add_argument('--lineWidth', type=int, default=5, help='line width to calculate the speckle tracking in centralLine mode. The unit is pattern size. Means that 5 is actually 5*pattern_size, such as 25um width')
+    parser.add_argument('--lineDirection', type=str, default='b', help='direction to calculate the speckle tracking in centralLine mode: (v)ertical, (h)orizontal, (b)oth')
 
     parser.add_argument('--down_sampling', type=float, default=1, help='down-sample images to reduce memory cost and accelerate speed.')
     parser.add_argument('--crop_boundary', type=int, default=-1, help='crop the differential phase boundary. -1 will use the searching window. 0 means no cropping')
     parser.add_argument('--method',
                         default='WXST',
                         type=str,
                         help='speckle tracking method. simple: slope-tracking, fast but less accurate; WXST: wavelet speckle tracking.')
@@ -1297,21 +1302,18 @@
     file_img    = args.img
     file_folder = os.path.dirname(args.img)
   
     result_folder = args.result_folder
     if not os.path.exists(result_folder): os.makedirs(result_folder)
     
     para_pattern = {
-        'pattern_path':
-        args.pattern_path,  # path to raw binary pattern file
-        'propagated_pattern':
-        args.propagated_pattern,  # load saved propagated pattern or not, if None, will calculate it and save it
-        # 'propagated_pattern': None,
-        'saving_path': file_folder 
-        if args.saving_path is None else args.saving_path,  #if propagated_pattern is None, save the simulated to this path
+        'pattern_path': args.pattern_path,  # path to raw binary pattern file
+        'propagated_pattern': args.propagated_pattern,  # load saved propagated pattern or not, if None, will calculate it and save it
+        'estimation_method': args.estimation_method,
+        'saving_path': file_folder if args.saving_path is None else args.saving_path,  #if propagated_pattern is None, save the simulated to this path
         'propagated_patternDet': args.propagated_patternDet, # propagated transformed simulated reference image at detector, if None, will search from the propagated pattern.
     }
 
     # roi_img = [650, 1380, 550, 2000]
     # roi_img = [750, 1280, 1050, 1500]
     # roi_img = [450, 1000, 500, 1000]
 
@@ -1429,15 +1431,15 @@
     # to find the pattern from the reference image
     pattern_find = pattern_search(ini_para=para_simulation)
 
     # -------------------------------- do the re-calculation of source distance -------------------------------------
     if args.d_source_recal and para_pattern['propagated_pattern'] == 'None' and para_pattern['propagated_patternDet'] == 'None':
         prColor('Re-calculate the source distance according to the current value', 'cyan')
         # estimation method, simple_speckle or geometric, simple_speckle means using the slope_tracking to estimate the overall source distance; geometric means using the image scalling factor to get the overall source distance
-        est_method = 'simple_speckle'
+        est_method = para_pattern['estimation_method']
         d_source_recal = do_recal_d_source(I_img_raw, I_img, para_pattern, pattern_find, image_transfer_matrix, boundary_crop, para_XST, para_simulation, method=est_method)
     
         prColor('use the recalculated source distance to re-generate the matched pattern', 'light_gray')
 
         para_simulation['d_sv_ini'] = para_simulation['d_sv']
         para_simulation['d_sh_ini'] = para_simulation['d_sh']
         
@@ -1623,75 +1625,57 @@
                                 ['line_phase_y', line_phase[0], '[rad]'],
                                 ['line_curve_y', line_curve_filter[0], '[1/m]'],
                                 ['line_curve_x', line_curve_filter[1], '[1/m]']], path=args.result_folder, p_x=args.p_x)
         
         save_data({'displace_x': displace_x, 'displace_y': displace_y, 'phase': phase, 
                     'line_phase_y': line_phase[0], 'line_displace_y': line_displace[0], 'line_curve_y': line_curve_filter[0], 'line_phase_x': line_phase[1], 'line_displace_x': line_displace[1], 'line_curve_x': line_curve_filter[1]}, args.result_folder, args.p_x)
 
-            
     elif args.mode == 'centralLine':
         prColor('speckle tracking mode: centralLine. Will use the central linewidth of {}um for calculation.'.format(args.lineWidth*args.pattern_size*1e6), 'cyan')
         # crop the vertical and horizontal block for calculation
         block_width = int(args.lineWidth*args.pattern_size / args.p_x) + 2 * (args.window_searching + args.template_size*int(1/args.down_sampling))
 
-        I_img_v = I_img[:, int(I_img.shape[0] // 2 - block_width // 2):int(I_img.shape[0] // 2 - block_width // 2 + block_width)]
-        I_simu_v = I_simu[:, int(I_img.shape[0] // 2 - block_width // 2):int(I_img.shape[0] // 2 - block_width // 2 + block_width)]
-        displace_y_offset_v = displace_y_offset[:, int(I_img.shape[0] // 2 - block_width // 2):int(I_img.shape[0] // 2 - block_width // 2 + block_width)]
-        displace_x_offset_v = displace_x_offset[:, int(I_img.shape[0] // 2 - block_width // 2):int(I_img.shape[0] // 2 - block_width // 2 + block_width)]
-
-        displace_y, _, _, _, _, _ = speckle_tracking(
-            I_simu_v, I_img_v, para_XST, para_simulation['p_x'],
-            para_simulation['d_prop'], c_w, displace_offset=[displace_y_offset_v, displace_x_offset_v])
-
-        I_img_h = I_img[int(I_img.shape[1] // 2 - block_width // 2):int(I_img.shape[1] // 2 - block_width // 2 + block_width), :]
-        I_simu_h = I_simu[int(I_img.shape[1] // 2 - block_width // 2):int(I_img.shape[1] // 2 - block_width // 2 + block_width), :]
-        displace_y_offset_h = displace_y_offset[int(I_img.shape[1] // 2 - block_width // 2):int(I_img.shape[1] // 2 - block_width // 2 + block_width), :]
-        displace_x_offset_h = displace_x_offset[int(I_img.shape[1] // 2 - block_width // 2):int(I_img.shape[1] // 2 - block_width // 2 + block_width), :]
-
-        _, displace_x, _, _, _, _ = speckle_tracking(
-            I_simu_h, I_img_h, para_XST, para_simulation['p_x'],
-            para_simulation['d_prop'], c_w, displace_offset=[displace_y_offset_h, displace_x_offset_h])
-
+        image_pair   = []
+        result       = {}
+        data         = {}
+        avg_source_d = [np.nan, np.nan]
+
+        def process_centralLine(index=0):
+            I_img_i = I_img[:, int(I_img.shape[index] // 2 - block_width // 2):int(I_img.shape[index] // 2 - block_width // 2 + block_width)]
+            I_simu_i = I_simu[:, int(I_img.shape[index] // 2 - block_width // 2):int(I_img.shape[index] // 2 - block_width // 2 + block_width)]
+            displace_y_offset_i = displace_y_offset[:, int(I_img.shape[index] // 2 - block_width // 2):int(I_img.shape[index] // 2 - block_width // 2 + block_width)]
+            displace_x_offset_i = displace_x_offset[:, int(I_img.shape[index] // 2 - block_width // 2):int(I_img.shape[index] // 2 - block_width // 2 + block_width)]
+
+            displace_i = [None, None]
+            displace_i[0], displace_i[1], _, _, _, _ = speckle_tracking(
+                I_simu_i, I_img_i, para_XST, para_simulation['p_x'],
+                para_simulation['d_prop'], c_w, displace_offset=[displace_y_offset_i, displace_x_offset_i])
+
+            line_displace = np.mean(displace_i[index], axis=1 if index==0 else 0)
+            line_displace = line_displace - np.mean(line_displace)
+
+            # get phase and curveature for central line profile
+            line_dpc   = line_displace * para_simulation['p_x'] / para_simulation['d_prop']
+            line_phase = np.cumsum(line_dpc)*para_simulation['p_x'] * 2 * np.pi / c_w
+            line_curve = np.gradient(line_displace)/para_simulation['d_prop']
+            avg_s_d    = 1/np.mean(line_curve)
+            # filter the line curve
+            line_curve_filter = snd.gaussian_filter(line_curve, 21)
+
+            suffix = 'y' if index==0 else 'x'
+            image_pair.append(['line_displace_' + suffix, line_displace,     '[px]'])
+            image_pair.append(['line_phase_' + suffix,    line_phase,        '[rad]'])
+            image_pair.append(['line_curve_' + suffix,    line_curve_filter, '[1/m]'])
+            result['avg_source_d_' + suffix] = avg_s_d
+            data['line_displace_' + suffix]  = line_displace
+            data['line_phase_' + suffix   ]  = line_phase
+            data['line_curve_' + suffix   ]  = line_curve_filter
+            avg_source_d[index]              = avg_s_d
+
+        if args.lineDirection == 'v' or args.lineDirection == 'b': process_centralLine(0)
+        if args.lineDirection == 'h' or args.lineDirection == 'b': process_centralLine(1)
+
+        prColor('mean source distance: {}y    {}x'.format(avg_source_d[0], avg_source_d[1]), 'cyan')
+        save_figure_1D(image_pair=image_pair, path=args.result_folder, p_x=args.p_x)
+        write_json(args.result_folder, 'result', result)
+        save_data(data, args.result_folder, args.p_x)
 
-        line_displace = [np.mean(displace_y, axis=1), np.mean(displace_x, axis=0)]
-        line_displace = [line_displace[0] - np.mean(line_displace[0]), line_displace[1] - np.mean(line_displace[1])]
-        # get phase and curveature for central line profile 
-        line_dpc = [line_displace[0] * para_simulation['p_x'] / para_simulation['d_prop'], 
-                    line_displace[1] * para_simulation['p_x'] / para_simulation['d_prop']]
-        line_phase = [np.cumsum(line_dpc[0])*para_simulation['p_x'] * 2 * np.pi / c_w,
-                     np.cumsum(line_dpc[1])*para_simulation['p_x'] * 2 * np.pi / c_w]
-        line_curve = [np.gradient(line_displace[0])/para_simulation['d_prop'],
-                            np.gradient(line_displace[1])/para_simulation['d_prop']]
-        # filter the line curve
-        line_curve_filter = [snd.gaussian_filter(line_curve[0], 21), snd.gaussian_filter(line_curve[1], 21)]
-
-        prColor('mean source distance: {}y    {}x'.format(1/np.mean(line_curve[0]), 1/np.mean(line_curve[1])), 'cyan')
-
-        save_figure_1D(image_pair=[['line_displace_x', line_displace[1], '[px]'],
-                                ['line_phase_x', line_phase[1], '[rad]'],
-                                ['line_displace_y', line_displace[0], '[px]'],
-                                ['line_phase_y', line_phase[0], '[rad]'],
-                                ['line_curve_y', line_curve_filter[0], '[1/m]'],
-                                ['line_curve_x', line_curve_filter[1], '[1/m]']], path=args.result_folder, p_x=args.p_x)
-
-        write_json(args.result_folder, 'result', {'avg_source_d_x': 1/np.mean(line_curve[1]),
-                                                    'avg_source_d_y': 1/np.mean(line_curve[0])})
-
-        save_data({'line_phase_y': line_phase[0], 'line_displace_y': line_displace[0], 'line_curve_y': line_curve_filter[0], 'line_phase_x': line_phase[1], 'line_displace_x': line_displace[1], 'line_curve_x': line_curve_filter[1]}, args.result_folder, args.p_x)
-
-    # enablePrint()
-    # plt.figure(figsize=(10,3))
-    # plt.subplot(131)
-    # plt.imshow(I_img)
-    # plt.colorbar()
-
-    # plt.subplot(132)
-    # plt.imshow(I_simu)
-    # plt.colorbar()
-
-    # plt.subplot(133)
-    # plt.imshow(flat)
-    # plt.colorbar()
-
-    # plt.show()
-
-
```

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/pattern_find.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_find.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/measurment/beamline/wf/pattern_propagate.py` & `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_propagate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/ml/__init__.py` & `aps_common_libraries-1.0.2/aps/common/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/ml/data_structures.py` & `aps_common_libraries-1.0.2/aps/common/ml/data_structures.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/ml/mocks.py` & `aps_common_libraries-1.0.2/aps/common/ml/mocks.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/plot/__init__.py` & `aps_common_libraries-1.0.2/aps/common/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/plot/gui.py` & `aps_common_libraries-1.0.2/aps/common/plot/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,20 +129,24 @@
     @classmethod
     def get_value(cls, parent=None, message="Input Value", title="Input Option", default=0, width=None, height=None):
         dlg = ValueDialog(parent, message, title, default, width, height)
         if dlg.exec_() == QMessageBox.Ok: return dlg.value
         else: return None
 
 
+def selectSaveFileFromDialog(widget, message="Save File", default_file_name="", file_extension_filter="*.*"):
+    file_path = QFileDialog.getSaveFileName(widget, message, default_file_name, file_extension_filter)[0]
+    if not file_path is None and not file_path.strip() == "": return file_path
+    else: return None
+
 def selectFileFromDialog(widget, previous_file_path="", message="Select File", start_directory=".", file_extension_filter="*.*"):
     file_path = QFileDialog.getOpenFileName(widget, message, start_directory, file_extension_filter)[0]
     if not file_path is None and not file_path.strip() == "": return file_path
     else: return previous_file_path
 
-
 def selectDirectoryFromDialog(widget, previous_directory_path="", message="Select Directory", start_directory="."):
     directory_path = QFileDialog.getExistingDirectory(widget, message, start_directory)
     if not directory_path is None and not directory_path.strip() == "": return directory_path
     else: return previous_directory_path
 
 ##########################################################################
 # WIDGETS UTILS FROM OASYS
```

### Comparing `aps_common_libraries-1.0.1/aps/common/plot/image.py` & `aps_common_libraries-1.0.2/aps/common/plot/image.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/plot/qt_application.py` & `aps_common_libraries-1.0.2/aps/common/plot/qt_application.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/plotter.py` & `aps_common_libraries-1.0.2/aps/common/plotter.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/registry.py` & `aps_common_libraries-1.0.2/aps/common/registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/scripts/__init__.py` & `aps_common_libraries-1.0.2/aps/common/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/scripts/abstract_command_line_script.py` & `aps_common_libraries-1.0.2/aps/common/scripts/abstract_command_line_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/scripts/generic_process_manager.py` & `aps_common_libraries-1.0.2/aps/common/scripts/generic_process_manager.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/scripts/generic_qt_script.py` & `aps_common_libraries-1.0.2/aps/common/scripts/generic_qt_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/scripts/script_data.py` & `aps_common_libraries-1.0.2/aps/common/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/scripts/script_registry.py` & `aps_common_libraries-1.0.2/aps/common/scripts/script_registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/singleton.py` & `aps_common_libraries-1.0.2/aps/common/singleton.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/traffic_light.py` & `aps_common_libraries-1.0.2/aps/common/traffic_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/widgets/__init__.py` & `aps_common_libraries-1.0.2/aps/common/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/widgets/close_app_widget.py` & `aps_common_libraries-1.0.2/aps/common/widgets/close_app_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/widgets/context_widget.py` & `aps_common_libraries-1.0.2/aps/common/widgets/context_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/widgets/generic_widget.py` & `aps_common_libraries-1.0.2/aps/common/widgets/generic_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps/common/widgets/log_stream_widget.py` & `aps_common_libraries-1.0.2/aps/common/widgets/log_stream_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/aps_common_libraries.egg-info/PKG-INFO` & `aps_common_libraries-1.0.2/aps_common_libraries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps-common-libraries
-Version: 1.0.1
+Version: 1.0.2
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.1/aps_common_libraries.egg-info/SOURCES.txt` & `aps_common_libraries-1.0.2/aps_common_libraries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.1/setup.py` & `aps_common_libraries-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'aps_common_libraries'
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 ISRELEASED = False
 
 DESCRIPTION = 'APS Common Libraries'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
```

