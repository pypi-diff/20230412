# Comparing `tmp/vcap-utils-0.3.6.tar.gz` & `tmp/vcap-utils-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcap-utils-0.3.6.tar", last modified: Thu Jan  5 06:22:46 2023, max compression
+gzip compressed data, was "vcap-utils-0.3.7.tar", last modified: Wed Apr 12 04:55:04 2023, max compression
```

## Comparing `vcap-utils-0.3.6.tar` & `vcap-utils-0.3.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:46.661985 vcap-utils-0.3.6/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      393 2023-01-05 06:22:46.661985 vcap-utils-0.3.6/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-01-05 06:22:46.661985 vcap-utils-0.3.6/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      899 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:46.529985 vcap-utils-0.3.6/vcap_utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       83 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:46.533985 vcap-utils-0.3.6/vcap_utils/algorithms/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      295 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/algorithms/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1419 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/algorithms/distances.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4317 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/algorithms/iou_cost_matrix.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9520 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/algorithms/linear_assignment.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2505 2022-12-29 03:38:51.000000 vcap-utils-0.3.6/vcap_utils/algorithms/nonmax_suppression.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:46.657985 vcap-utils-0.3.6/vcap_utils/backends/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      709 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10487 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/backend_rpc_process.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      621 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/base_encoder.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10692 2023-01-01 18:54:50.000000 vcap-utils-0.3.6/vcap_utils/backends/base_openvino.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      147 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/base_tensorflow.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2364 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/crowd_density.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2142 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/depth.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1882 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/load_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3447 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/openface_encoder.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6008 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/predictions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2521 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/segmentation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6031 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/tf_image_classification.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6733 2022-12-23 01:33:25.000000 vcap-utils-0.3.6/vcap_utils/backends/tf_object_detection.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       22 2023-01-05 06:19:24.000000 vcap-utils-0.3.6/vcap_utils/version.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:46.529985 vcap-utils-0.3.6/vcap_utils.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      393 2023-01-05 06:22:46.000000 vcap-utils-0.3.6/vcap_utils.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      907 2023-01-05 06:22:46.000000 vcap-utils-0.3.6/vcap_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-01-05 06:22:46.000000 vcap-utils-0.3.6/vcap_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       26 2023-01-05 06:22:46.000000 vcap-utils-0.3.6/vcap_utils.egg-info/requires.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       11 2023-01-05 06:22:46.000000 vcap-utils-0.3.6/vcap_utils.egg-info/top_level.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:55:04.944433 vcap-utils-0.3.7/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      393 2023-04-12 04:55:04.944433 vcap-utils-0.3.7/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-04-12 04:55:04.944433 vcap-utils-0.3.7/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      899 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:55:04.820432 vcap-utils-0.3.7/vcap_utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       83 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:55:04.820432 vcap-utils-0.3.7/vcap_utils/algorithms/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      295 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/algorithms/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1419 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/algorithms/distances.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4317 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/algorithms/iou_cost_matrix.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9520 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/algorithms/linear_assignment.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2505 2022-12-29 03:38:51.000000 vcap-utils-0.3.7/vcap_utils/algorithms/nonmax_suppression.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:55:04.940433 vcap-utils-0.3.7/vcap_utils/backends/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      709 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10487 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/backend_rpc_process.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      621 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/base_encoder.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10692 2023-01-01 18:54:50.000000 vcap-utils-0.3.7/vcap_utils/backends/base_openvino.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      147 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/base_tensorflow.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2364 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/crowd_density.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2142 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/depth.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1882 2023-04-11 20:55:43.000000 vcap-utils-0.3.7/vcap_utils/backends/load_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3447 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/openface_encoder.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6008 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/predictions.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2521 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/segmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6031 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/tf_image_classification.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6733 2022-12-23 01:33:25.000000 vcap-utils-0.3.7/vcap_utils/backends/tf_object_detection.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       22 2023-04-11 23:51:04.000000 vcap-utils-0.3.7/vcap_utils/version.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:55:04.820432 vcap-utils-0.3.7/vcap_utils.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      393 2023-04-12 04:55:04.000000 vcap-utils-0.3.7/vcap_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      907 2023-04-12 04:55:04.000000 vcap-utils-0.3.7/vcap_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-04-12 04:55:04.000000 vcap-utils-0.3.7/vcap_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       26 2023-04-12 04:55:04.000000 vcap-utils-0.3.7/vcap_utils.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       11 2023-04-12 04:55:04.000000 vcap-utils-0.3.7/vcap_utils.egg-info/top_level.txt
```

### Comparing `vcap-utils-0.3.6/setup.py` & `vcap-utils-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/algorithms/distances.py` & `vcap-utils-0.3.7/vcap_utils/algorithms/distances.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/algorithms/iou_cost_matrix.py` & `vcap-utils-0.3.7/vcap_utils/algorithms/iou_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/algorithms/linear_assignment.py` & `vcap-utils-0.3.7/vcap_utils/algorithms/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/algorithms/nonmax_suppression.py` & `vcap-utils-0.3.7/vcap_utils/algorithms/nonmax_suppression.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/__init__.py` & `vcap-utils-0.3.7/vcap_utils/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/backend_rpc_process.py` & `vcap-utils-0.3.7/vcap_utils/backends/backend_rpc_process.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/base_encoder.py` & `vcap-utils-0.3.7/vcap_utils/backends/base_encoder.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/base_openvino.py` & `vcap-utils-0.3.7/vcap_utils/backends/base_openvino.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/crowd_density.py` & `vcap-utils-0.3.7/vcap_utils/backends/crowd_density.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/depth.py` & `vcap-utils-0.3.7/vcap_utils/backends/depth.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/load_utils.py` & `vcap-utils-0.3.7/vcap_utils/backends/load_utils.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/openface_encoder.py` & `vcap-utils-0.3.7/vcap_utils/backends/openface_encoder.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/predictions.py` & `vcap-utils-0.3.7/vcap_utils/backends/predictions.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/segmentation.py` & `vcap-utils-0.3.7/vcap_utils/backends/segmentation.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/tf_image_classification.py` & `vcap-utils-0.3.7/vcap_utils/backends/tf_image_classification.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils/backends/tf_object_detection.py` & `vcap-utils-0.3.7/vcap_utils/backends/tf_object_detection.py`

 * *Files identical despite different names*

### Comparing `vcap-utils-0.3.6/vcap_utils.egg-info/SOURCES.txt` & `vcap-utils-0.3.7/vcap_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

