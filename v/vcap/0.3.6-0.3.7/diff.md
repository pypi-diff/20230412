# Comparing `tmp/vcap-0.3.6.tar.gz` & `tmp/vcap-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcap-0.3.6.tar", last modified: Thu Jan  5 06:22:29 2023, max compression
+gzip compressed data, was "vcap-0.3.7.tar", last modified: Wed Apr 12 04:54:49 2023, max compression
```

## Comparing `vcap-0.3.6.tar` & `vcap-0.3.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.201909 vcap-0.3.6/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      401 2023-01-05 06:22:29.201909 vcap-0.3.6/PKG-INFO
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.149909 vcap-0.3.6/examples/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.161909 vcap-0.3.6/examples/classifier_gait_example/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      186 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/classifier_gait_example/README.md
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      874 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/classifier_gait_example/backend.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1604 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/classifier_gait_example/capsule.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      111 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/classifier_gait_example/config.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       89 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/classifier_gait_example/dataset_metadata.json
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       40 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/classifier_gait_example/meta.conf
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.173909 vcap-0.3.6/examples/detector_person_example/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1035 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/detector_person_example/README.md
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1496 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/detector_person_example/backend.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2305 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/detector_person_example/capsule.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1685 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/detector_person_example/dataset_metadata.json
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       40 2022-12-23 01:33:25.000000 vcap-0.3.6/examples/detector_person_example/meta.conf
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-01-05 06:22:29.201909 vcap-0.3.6/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1051 2022-12-23 01:33:25.000000 vcap-0.3.6/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.197909 vcap-0.3.6/vcap/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      824 2023-01-05 06:00:06.000000 vcap-0.3.6/vcap/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4135 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/backend.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5195 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/batch_executor.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      561 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/caching.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9736 2023-01-01 18:54:50.000000 vcap-0.3.6/vcap/capsule.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1501 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/deprecation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6457 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/detection_node.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4003 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/device_mapping.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.197909 vcap-0.3.6/vcap/loading/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14439 2023-01-05 05:58:46.000000 vcap-0.3.6/vcap/loading/capsule_loading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      899 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/loading/crypto_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      684 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/loading/errors.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5599 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/loading/import_hacks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2383 2022-12-29 03:38:51.000000 vcap-0.3.6/vcap/loading/vcap_packaging.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14406 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/modifiers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7576 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/node_description.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5606 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/options.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      210 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/stream_state.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.197909 vcap-0.3.6/vcap/testing/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      174 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/testing/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1344 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/testing/capsule_loading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11869 2023-01-05 06:01:08.000000 vcap-0.3.6/vcap/testing/input_output_validation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1068 2022-12-23 01:33:25.000000 vcap-0.3.6/vcap/testing/thread_validation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       22 2023-01-05 06:19:12.000000 vcap-0.3.6/vcap/version.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-01-05 06:22:29.197909 vcap-0.3.6/vcap.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      401 2023-01-05 06:22:28.000000 vcap-0.3.6/vcap.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1173 2023-01-05 06:22:29.000000 vcap-0.3.6/vcap.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-01-05 06:22:28.000000 vcap-0.3.6/vcap.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      147 2023-01-05 06:22:28.000000 vcap-0.3.6/vcap.egg-info/requires.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        5 2023-01-05 06:22:28.000000 vcap-0.3.6/vcap.egg-info/top_level.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.296336 vcap-0.3.7/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      401 2023-04-12 04:54:49.296336 vcap-0.3.7/PKG-INFO
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.292336 vcap-0.3.7/examples/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.296336 vcap-0.3.7/examples/classifier_gait_example/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      186 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/classifier_gait_example/README.md
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      874 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/classifier_gait_example/backend.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1604 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/classifier_gait_example/capsule.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      111 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/classifier_gait_example/config.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       89 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/classifier_gait_example/dataset_metadata.json
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       40 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/classifier_gait_example/meta.conf
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.296336 vcap-0.3.7/examples/detector_person_example/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1035 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/detector_person_example/README.md
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1496 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/detector_person_example/backend.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2305 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/detector_person_example/capsule.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1685 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/detector_person_example/dataset_metadata.json
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       40 2022-12-23 01:33:25.000000 vcap-0.3.7/examples/detector_person_example/meta.conf
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-04-12 04:54:49.296336 vcap-0.3.7/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1051 2022-12-23 01:33:25.000000 vcap-0.3.7/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.296336 vcap-0.3.7/vcap/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      824 2023-01-05 06:00:06.000000 vcap-0.3.7/vcap/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4135 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/backend.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5195 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/batch_executor.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      561 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/caching.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9736 2023-01-01 18:54:50.000000 vcap-0.3.7/vcap/capsule.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1501 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/deprecation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6457 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/detection_node.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4003 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/device_mapping.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.296336 vcap-0.3.7/vcap/loading/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14475 2023-03-08 18:24:51.000000 vcap-0.3.7/vcap/loading/capsule_loading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      899 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/loading/crypto_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      684 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/loading/errors.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5599 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/loading/import_hacks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4639 2023-04-11 23:47:08.000000 vcap-0.3.7/vcap/loading/vcap_packaging.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14406 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/modifiers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7576 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/node_description.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5606 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/options.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      210 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/stream_state.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.296336 vcap-0.3.7/vcap/testing/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      174 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/testing/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1344 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/testing/capsule_loading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11869 2023-01-05 06:01:08.000000 vcap-0.3.7/vcap/testing/input_output_validation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1068 2022-12-23 01:33:25.000000 vcap-0.3.7/vcap/testing/thread_validation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       22 2023-04-11 23:50:46.000000 vcap-0.3.7/vcap/version.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-12 04:54:49.296336 vcap-0.3.7/vcap.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      401 2023-04-12 04:54:49.000000 vcap-0.3.7/vcap.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1173 2023-04-12 04:54:49.000000 vcap-0.3.7/vcap.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-04-12 04:54:49.000000 vcap-0.3.7/vcap.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      147 2023-04-12 04:54:49.000000 vcap-0.3.7/vcap.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        5 2023-04-12 04:54:49.000000 vcap-0.3.7/vcap.egg-info/top_level.txt
```

### Comparing `vcap-0.3.6/examples/classifier_gait_example/backend.py` & `vcap-0.3.7/examples/classifier_gait_example/backend.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/examples/classifier_gait_example/capsule.py` & `vcap-0.3.7/examples/classifier_gait_example/capsule.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/examples/detector_person_example/README.md` & `vcap-0.3.7/examples/detector_person_example/README.md`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/examples/detector_person_example/backend.py` & `vcap-0.3.7/examples/detector_person_example/backend.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/examples/detector_person_example/capsule.py` & `vcap-0.3.7/examples/detector_person_example/capsule.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/examples/detector_person_example/dataset_metadata.json` & `vcap-0.3.7/examples/detector_person_example/dataset_metadata.json`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/setup.py` & `vcap-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/__init__.py` & `vcap-0.3.7/vcap/__init__.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/backend.py` & `vcap-0.3.7/vcap/backend.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/batch_executor.py` & `vcap-0.3.7/vcap/batch_executor.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/caching.py` & `vcap-0.3.7/vcap/caching.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/capsule.py` & `vcap-0.3.7/vcap/capsule.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/deprecation.py` & `vcap-0.3.7/vcap/deprecation.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/detection_node.py` & `vcap-0.3.7/vcap/detection_node.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/device_mapping.py` & `vcap-0.3.7/vcap/device_mapping.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/loading/capsule_loading.py` & `vcap-0.3.7/vcap/loading/capsule_loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from types import ModuleType
 from typing import Any, Callable, List, Optional, Union
 from zipfile import ZipFile
 
 from vcap import BaseCapsule, BaseBackend, BaseStreamState, NodeDescription
 from vcap.loading.errors import IncompatibleCapsuleError, InvalidCapsuleError
 
-from .crypto_utils import decrypt
-from .import_hacks import ZipFinder
-from .vcap_packaging import CAPSULE_FILE_NAME, META_FILE_NAME
+from vcap.loading.crypto_utils import decrypt
+from vcap.loading.import_hacks import ZipFinder
+from vcap.loading.vcap_packaging import CAPSULE_FILE_NAME, META_FILE_NAME
 
 MAJOR_COMPATIBLE_VERSION = 0
 MINOR_COMPATIBLE_VERSION = 3
 """The capsule version that this version of the library supports."""
 
 MAJOR_MINOR_SEMVER_PATTERN = re.compile(r"([0-9]+)\.([0-9]+)")
```

### Comparing `vcap-0.3.6/vcap/loading/crypto_utils.py` & `vcap-0.3.7/vcap/loading/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/loading/errors.py` & `vcap-0.3.7/vcap/loading/errors.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/loading/import_hacks.py` & `vcap-0.3.7/vcap/loading/import_hacks.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/modifiers.py` & `vcap-0.3.7/vcap/modifiers.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/node_description.py` & `vcap-0.3.7/vcap/node_description.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/options.py` & `vcap-0.3.7/vcap/options.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/testing/capsule_loading.py` & `vcap-0.3.7/vcap/testing/capsule_loading.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/testing/input_output_validation.py` & `vcap-0.3.7/vcap/testing/input_output_validation.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap/testing/thread_validation.py` & `vcap-0.3.7/vcap/testing/thread_validation.py`

 * *Files identical despite different names*

### Comparing `vcap-0.3.6/vcap.egg-info/SOURCES.txt` & `vcap-0.3.7/vcap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

