# Comparing `tmp/kiss_icp-0.2.8.tar.gz` & `tmp/kiss_icp-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiss_icp-0.2.8.tar", last modified: Tue Apr 11 15:31:07 2023, max compression
+gzip compressed data, was "kiss_icp-0.2.9.tar", last modified: Wed Apr 12 19:16:10 2023, max compression
```

## Comparing `kiss_icp-0.2.8.tar` & `kiss_icp-0.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.890225 kiss_icp-0.2.8/kiss_icp/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/apollo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/boreas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/kitti.py
--rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/kitti_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/mulran.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/ncd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/nclt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/nuscenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/ouster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/paris_luco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/rosbag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/tum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/deskew.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/kiss_icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/pybind/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/kiss_icp_pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/pybind/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/pybind11/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/stl_vector_eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/pipeline_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/point_cloud2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/voxelization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-11 15:31:07.898224 kiss_icp-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.880860 kiss_icp-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-12 19:16:10.880860 kiss_icp-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.876860 kiss_icp-0.2.9/kiss_icp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.876860 kiss_icp-0.2.9/kiss_icp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.880860 kiss_icp-0.2.9/kiss_icp/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/apollo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/boreas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/kitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/kitti_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/mulran.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/ncd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/nclt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/nuscenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/ouster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/paris_luco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/datasets/tum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/deskew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/kiss_icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.880860 kiss_icp-0.2.9/kiss_icp/pybind/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/pybind/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/pybind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/pybind/kiss_icp_pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.880860 kiss_icp-0.2.9/kiss_icp/pybind/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/pybind/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/pybind/pybind11/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/pybind/stl_vector_eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.880860 kiss_icp-0.2.9/kiss_icp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/tools/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/tools/pipeline_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/tools/point_cloud2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/tools/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/tools/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/kiss_icp/voxelization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:16:10.876860 kiss_icp-0.2.9/kiss_icp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-12 19:16:10.000000 kiss_icp-0.2.9/kiss_icp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-12 19:16:10.000000 kiss_icp-0.2.9/kiss_icp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:16:10.000000 kiss_icp-0.2.9/kiss_icp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 19:16:10.000000 kiss_icp-0.2.9/kiss_icp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 19:16:10.000000 kiss_icp-0.2.9/kiss_icp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 19:16:10.000000 kiss_icp-0.2.9/kiss_icp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-12 19:16:10.880860 kiss_icp-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-12 19:15:58.000000 kiss_icp-0.2.9/setup.py
```

### Comparing `kiss_icp-0.2.8/CMakeLists.txt` & `kiss_icp-0.2.9/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 cmake_minimum_required(VERSION 3.16...3.26)
-project(kiss_icp_pybind VERSION 0.2.8 LANGUAGES CXX)
+project(kiss_icp_pybind VERSION 0.2.9 LANGUAGES CXX)
 
 # Set build type
 set(CMAKE_BUILD_TYPE Release)
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
 if(EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/../cpp/kiss_icp/)
```

### Comparing `kiss_icp-0.2.8/LICENSE` & `kiss_icp-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/PKG-INFO` & `kiss_icp-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiss_icp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Simple yet effective 3D LiDAR-Odometry registration pipeline
 Home-page: https://github.com/PRBonn/kiss-icp
 Author: Ignacio Vizzo
 Author-email: ignaciovizzo@gmail.com
 License: MIT
 Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kiss_icp Version: 0.2.8 Summary: Simple yet
+Metadata-Version: 2.1 Name: kiss_icp Version: 0.2.9 Summary: Simple yet
 effective 3D LiDAR-Odometry registration pipeline Home-page: https://
 github.com/PRBonn/kiss-icp Author: Ignacio Vizzo Author-email:
 ignaciovizzo@gmail.com License: MIT Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Programming
 Language :: C++ Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `kiss_icp-0.2.8/README.md` & `kiss_icp-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/__init__.py` & `kiss_icp-0.2.9/kiss_icp/pybind/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__version__ = "0.2.8"
```

### Comparing `kiss_icp-0.2.8/kiss_icp/config/__init__.py` & `kiss_icp-0.2.9/kiss_icp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/config/config.py` & `kiss_icp-0.2.9/kiss_icp/config/config.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/config/parser.py` & `kiss_icp-0.2.9/kiss_icp/config/parser.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/__init__.py` & `kiss_icp-0.2.9/kiss_icp/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/apollo.py` & `kiss_icp-0.2.9/kiss_icp/datasets/apollo.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/boreas.py` & `kiss_icp-0.2.9/kiss_icp/datasets/boreas.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/generic.py` & `kiss_icp-0.2.9/kiss_icp/datasets/generic.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/kitti.py` & `kiss_icp-0.2.9/kiss_icp/datasets/kitti.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/kitti_raw.py` & `kiss_icp-0.2.9/kiss_icp/datasets/kitti_raw.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/mcap.py` & `kiss_icp-0.2.9/kiss_icp/datasets/mcap.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/mulran.py` & `kiss_icp-0.2.9/kiss_icp/datasets/mulran.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/ncd.py` & `kiss_icp-0.2.9/kiss_icp/datasets/ncd.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/nclt.py` & `kiss_icp-0.2.9/kiss_icp/datasets/nclt.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/nuscenes.py` & `kiss_icp-0.2.9/kiss_icp/datasets/nuscenes.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/ouster.py` & `kiss_icp-0.2.9/kiss_icp/datasets/ouster.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/paris_luco.py` & `kiss_icp-0.2.9/kiss_icp/datasets/paris_luco.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/rosbag.py` & `kiss_icp-0.2.9/kiss_icp/datasets/rosbag.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/datasets/tum.py` & `kiss_icp-0.2.9/kiss_icp/datasets/tum.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/deskew.py` & `kiss_icp-0.2.9/kiss_icp/deskew.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/kiss_icp.py` & `kiss_icp-0.2.9/kiss_icp/kiss_icp.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/mapping.py` & `kiss_icp-0.2.9/kiss_icp/mapping.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/metrics.py` & `kiss_icp-0.2.9/kiss_icp/metrics.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/pipeline.py` & `kiss_icp-0.2.9/kiss_icp/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/preprocess.py` & `kiss_icp-0.2.9/kiss_icp/preprocess.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/pybind/CMakeLists.txt` & `kiss_icp-0.2.9/kiss_icp/pybind/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -44,8 +44,10 @@
 if(NOT USE_SYSTEM_PYBIND11 OR NOT pybind11_FOUND)
   set(USE_SYSTEM_PYBIND11 OFF)
   include(${CMAKE_CURRENT_LIST_DIR}/pybind11/pybind11.cmake)
 endif()
 
 pybind11_add_module(kiss_icp_pybind MODULE kiss_icp_pybind.cpp)
 target_link_libraries(kiss_icp_pybind PRIVATE kiss_icp::core kiss_icp::metrics)
-install(TARGETS kiss_icp_pybind DESTINATION .)
+install(TARGETS kiss_icp_pybind DESTINATION . COMPONENT python_bindings)
+add_custom_target(install_python_bindings ${CMAKE_COMMAND} -DCMAKE_INSTALL_COMPONENT=python_bindings -P
+                                          "${PROJECT_BINARY_DIR}/cmake_install.cmake" DEPENDS kiss_icp_pybind)
```

### Comparing `kiss_icp-0.2.8/kiss_icp/pybind/__init__.py` & `kiss_icp-0.2.9/kiss_icp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/pybind/kiss_icp_pybind.cpp` & `kiss_icp-0.2.9/kiss_icp/pybind/kiss_icp_pybind.cpp`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/pybind/pybind11/LICENSE` & `kiss_icp-0.2.9/kiss_icp/pybind/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/pybind/pybind11/pybind11.cmake` & `kiss_icp-0.2.9/kiss_icp/pybind/pybind11/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/pybind/stl_vector_eigen.h` & `kiss_icp-0.2.9/kiss_icp/pybind/stl_vector_eigen.h`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/registration.py` & `kiss_icp-0.2.9/kiss_icp/registration.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/threshold.py` & `kiss_icp-0.2.9/kiss_icp/threshold.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/tools/__init__.py` & `kiss_icp-0.2.9/kiss_icp/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+__version__ = "0.2.9"
```

### Comparing `kiss_icp-0.2.8/kiss_icp/tools/cmd.py` & `kiss_icp-0.2.9/kiss_icp/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/tools/pipeline_results.py` & `kiss_icp-0.2.9/kiss_icp/tools/pipeline_results.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/tools/point_cloud2.py` & `kiss_icp-0.2.9/kiss_icp/tools/point_cloud2.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/tools/progress_bar.py` & `kiss_icp-0.2.9/kiss_icp/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/tools/visualizer.py` & `kiss_icp-0.2.9/kiss_icp/tools/visualizer.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp/voxelization.py` & `kiss_icp-0.2.9/kiss_icp/voxelization.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/kiss_icp.egg-info/PKG-INFO` & `kiss_icp-0.2.9/kiss_icp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiss-icp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Simple yet effective 3D LiDAR-Odometry registration pipeline
 Home-page: https://github.com/PRBonn/kiss-icp
 Author: Ignacio Vizzo
 Author-email: ignaciovizzo@gmail.com
 License: MIT
 Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kiss-icp Version: 0.2.8 Summary: Simple yet
+Metadata-Version: 2.1 Name: kiss-icp Version: 0.2.9 Summary: Simple yet
 effective 3D LiDAR-Odometry registration pipeline Home-page: https://
 github.com/PRBonn/kiss-icp Author: Ignacio Vizzo Author-email:
 ignaciovizzo@gmail.com License: MIT Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Programming
 Language :: C++ Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `kiss_icp-0.2.8/kiss_icp.egg-info/SOURCES.txt` & `kiss_icp-0.2.9/kiss_icp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.8/setup.cfg` & `kiss_icp-0.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kiss_icp
-version = 0.2.8
+version = 0.2.9
 author = Ignacio Vizzo
 author_email = ignaciovizzo@gmail.com
 description = Simple yet effective 3D LiDAR-Odometry registration pipeline
 long_description = file:README.md,
 long_description_content_type = text/markdown
 url = https://github.com/PRBonn/kiss-icp
 license = MIT
```

### Comparing `kiss_icp-0.2.8/setup.py` & `kiss_icp-0.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     yield
 
 
 with skbuild_isolated_context():
     setup(
         packages=find_packages(),
         cmake_install_dir="kiss_icp/pybind/",
+        cmake_install_target="install_python_bindings",
         entry_points={"console_scripts": ["kiss_icp_pipeline=kiss_icp.tools.cmd:run"]},
         install_requires=[
             "natsort",
             "numpy",
             "plyfile",
             "pydantic",
             "pyquaternion",
```

