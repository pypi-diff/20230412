# Comparing `tmp/generic-dataset-1.4.1.tar.gz` & `tmp/generic-dataset-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-dataset-1.4.1.tar", last modified: Mon Sep 20 17:11:47 2021, max compression
+gzip compressed data, was "generic-dataset-1.5.0.tar", last modified: Wed Apr 12 10:09:58 2023, max compression
```

## Comparing `generic-dataset-1.4.1.tar` & `generic-dataset-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 17:11:47.058488 generic-dataset-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    20074 2021-09-20 17:11:47.058488 generic-dataset-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19599 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 17:11:47.054489 generic-dataset-1.4.1/generic_dataset/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8445 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    17633 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/dataset_folder_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/generic_sample.py
--rw-r--r--   0 runner    (1001) docker     (121)    21973 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/sample_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 17:11:47.058488 generic-dataset-1.4.1/generic_dataset/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/utilities/color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/utilities/engine_selector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/generic_dataset/utilities/save_load_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 17:11:47.054489 generic-dataset-1.4.1/generic_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20074 2021-09-20 17:11:46.000000 generic-dataset-1.4.1/generic_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-09-20 17:11:46.000000 generic-dataset-1.4.1/generic_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-20 17:11:46.000000 generic-dataset-1.4.1/generic_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-09-20 17:11:46.000000 generic-dataset-1.4.1/generic_dataset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-20 17:11:46.000000 generic-dataset-1.4.1/generic_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-20 17:11:46.000000 generic-dataset-1.4.1/generic_dataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-20 17:11:47.058488 generic-dataset-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2021-09-20 17:11:33.000000 generic-dataset-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:09:58.308568 generic-dataset-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-04-12 10:09:58.308568 generic-dataset-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:09:58.304568 generic-dataset-1.5.0/generic_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/dataset_folder_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/generic_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/sample_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:09:58.308568 generic-dataset-1.5.0/generic_dataset/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/utilities/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/utilities/engine_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/generic_dataset/utilities/save_load_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:09:58.308568 generic-dataset-1.5.0/generic_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-04-12 10:09:58.000000 generic-dataset-1.5.0/generic_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 10:09:58.000000 generic-dataset-1.5.0/generic_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:09:58.000000 generic-dataset-1.5.0/generic_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 10:09:58.000000 generic-dataset-1.5.0/generic_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 10:09:58.000000 generic-dataset-1.5.0/generic_dataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:09:58.308568 generic-dataset-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-12 10:09:47.000000 generic-dataset-1.5.0/setup.py
```

### Comparing `generic-dataset-1.4.1/LICENSE` & `generic-dataset-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/PKG-INFO` & `generic-dataset-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: generic-dataset
-Version: 1.4.1
+Version: 1.5.0
 Summary: Gibson dataset
 Home-page: https://github.com/micheleantonazzi/generic-dataset
 Author: Michele Antonazzi
 Author-email: micheleantonazzi@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -277,9 +276,7 @@
     .add_operation(lambda data, engine: (data[..., [2, 1, 0]], engine))
 
 bgr_image = pipeline_rgb_to_bgr.run(use_gpu=run_pipeline_on_gpu).get_data()
 ```
 
 
 
-
-
```

### Comparing `generic-dataset-1.4.1/README.md` & `generic-dataset-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset/data_pipeline.py` & `generic-dataset-1.5.0/generic_dataset/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset/dataset_folder_manager.py` & `generic-dataset-1.5.0/generic_dataset/dataset_folder_manager.py`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset/dataset_manager.py` & `generic-dataset-1.5.0/generic_dataset/dataset_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         :return: a pandas dataframe contaning all samples information.
         """
 
         dataframe = pd.DataFrame(columns=['folder_name', 'folder_absolute_count', 'label'])
         for folder in self._dataset_folder_managers.keys():
             samples_information = self._dataset_folder_managers[folder].get_samples_information()
             values = [[folder, i, label] for (i, (label, _)) in enumerate(samples_information)]
-            dataframe = dataframe.append(pd.DataFrame(values, columns=dataframe.columns), ignore_index=True)
+            dataframe = pd.concat([dataframe, pd.DataFrame(values, columns=dataframe.columns)], ignore_index=True)
         return dataframe.sort_values(['folder_name', 'folder_absolute_count'])
 
     def load_sample(self, folder_name: str, absolute_count: int, use_thread: bool = False) -> Union[GenericSample, Future]:
         """
         Loads sample using the folder name where it is stored and it absoulte count inside it.
         :param folder_name: the name of the directory where it is stored
         :param absolute_count: the absolute count of the sample
```

### Comparing `generic-dataset-1.4.1/generic_dataset/generic_sample.py` & `generic-dataset-1.5.0/generic_dataset/generic_sample.py`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset/sample_generator.py` & `generic-dataset-1.5.0/generic_dataset/sample_generator.py`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset/utilities/color.py` & `generic-dataset-1.5.0/generic_dataset/utilities/color.py`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset/utilities/engine_selector.py` & `generic-dataset-1.5.0/generic_dataset/utilities/engine_selector.py`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset/utilities/save_load_methods.py` & `generic-dataset-1.5.0/generic_dataset/utilities/save_load_methods.py`

 * *Files identical despite different names*

### Comparing `generic-dataset-1.4.1/generic_dataset.egg-info/PKG-INFO` & `generic-dataset-1.5.0/generic_dataset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: generic-dataset
-Version: 1.4.1
+Version: 1.5.0
 Summary: Gibson dataset
 Home-page: https://github.com/micheleantonazzi/generic-dataset
 Author: Michele Antonazzi
 Author-email: micheleantonazzi@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -277,9 +276,7 @@
     .add_operation(lambda data, engine: (data[..., [2, 1, 0]], engine))
 
 bgr_image = pipeline_rgb_to_bgr.run(use_gpu=run_pipeline_on_gpu).get_data()
 ```
 
 
 
-
-
```

### Comparing `generic-dataset-1.4.1/generic_dataset.egg-info/SOURCES.txt` & `generic-dataset-1.5.0/generic_dataset.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,13 @@
 generic_dataset/dataset_folder_manager.py
 generic_dataset/dataset_manager.py
 generic_dataset/generic_sample.py
 generic_dataset/sample_generator.py
 generic_dataset.egg-info/PKG-INFO
 generic_dataset.egg-info/SOURCES.txt
 generic_dataset.egg-info/dependency_links.txt
-generic_dataset.egg-info/entry_points.txt
 generic_dataset.egg-info/requires.txt
 generic_dataset.egg-info/top_level.txt
 generic_dataset/utilities/__init__.py
 generic_dataset/utilities/color.py
 generic_dataset/utilities/engine_selector.py
 generic_dataset/utilities/save_load_methods.py
```

### Comparing `generic-dataset-1.4.1/setup.py` & `generic-dataset-1.5.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import re
 import subprocess
+import sys
+import platform
 
 # To use a consistent encoding
 from codecs import open as copen
 
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
@@ -47,20 +49,24 @@
         regex = r'release (\S+),'
         match = re.search(regex, res)
         if match:
             return str(match.group(1)).replace('.', '')
 
     return ''
 
-try:
-    cuda_version = get_cuda_version()
-    if not cuda_version == '':
-        cuda_version = 'cupy-cuda' + cuda_version
-except:
+# On python 3.6 and aarch64, install cupy (requires a long build)
+if sys.version_info[0] == 3 and sys.version_info[1] == 6 and platform.machine() == 'aarch64':
     cuda_version = ''
+else:
+    try:
+        cuda_version = get_cuda_version()
+        if not cuda_version == '':
+            cuda_version = 'cupy-cuda' + cuda_version
+    except:
+        cuda_version = ''
 
 setup(
     name='generic-dataset',
     version=__version__,
     description="Gibson dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -75,15 +81,16 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
     ],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     tests_require=test_deps,
     # Add here the package dependencies
     install_requires=[
-        'opencv-python',
+        'opencv-python<4.7; python_version == "3.6"',
+        'opencv-python; python_version > "3.6"',
         'numpy',
         'pandas',
         cuda_version,
         'termcolor',
         'stub-generator'
     ],
     entry_points={
```

