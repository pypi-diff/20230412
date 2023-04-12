# Comparing `tmp/slabdip-4.1.macosx-11.0-arm64.tar.gz` & `tmp/slabdip-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slabdip-4.1.macosx-11.0-arm64.tar", last modified: Wed Apr 12 09:43:20 2023, max compression
+gzip compressed data, was "slabdip-4.1.1.tar", last modified: Wed Apr 12 10:49:12 2023, max compression
```

## Comparing `slabdip-4.1.macosx-11.0-arm64.tar` & `slabdip-4.1.1.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410265 ./
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410315 ./Users/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410364 ./Users/ben/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410404 ./Users/ben/miniforge3/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410452 ./Users/ben/miniforge3/envs/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410512 ./Users/ben/miniforge3/envs/mapping/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410564 ./Users/ben/miniforge3/envs/mapping/lib/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.410613 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.445150 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.413743 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/
--rw-r--r--   0 ben        (501) staff       (20)      160 2023-02-21 01:12:14.000000 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.414263 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/__pycache__/
--rw-r--r--   0 ben        (501) staff       (20)      340 2023-04-12 09:43:20.414215 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 ben        (501) staff       (20)     9675 2023-04-12 09:43:20.413898 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/__pycache__/predictor.cpython-39.pyc
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.411317 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/data/
--rw-r--r--   0 ben        (501) staff       (20)   555736 2023-02-21 01:12:14.000000 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/data/subduction_data.csv
--rw-r--r--   0 ben        (501) staff       (20)    14035 2023-04-11 21:12:26.000000 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/predictor.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-12 09:43:20.445873 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip-4.1-py3.9.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     4721 2023-04-12 09:43:20.165463 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip-4.1-py3.9.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      246 2023-04-12 09:43:20.346999 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip-4.1-py3.9.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-04-12 09:43:20.190028 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip-4.1-py3.9.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       66 2023-04-12 09:43:20.317648 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip-4.1-py3.9.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)        8 2023-04-12 09:43:20.341963 ./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip-4.1-py3.9.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:49:12.689771 slabdip-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-12 10:49:12.689771 slabdip-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-12 10:49:01.000000 slabdip-4.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:49:12.689771 slabdip-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-12 10:49:01.000000 slabdip-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:49:12.689771 slabdip-4.1.1/slabdip/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 10:49:01.000000 slabdip-4.1.1/slabdip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:49:12.689771 slabdip-4.1.1/slabdip/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   555736 2023-04-12 10:49:01.000000 slabdip-4.1.1/slabdip/data/subduction_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-12 10:49:01.000000 slabdip-4.1.1/slabdip/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:49:12.689771 slabdip-4.1.1/slabdip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-12 10:49:12.000000 slabdip-4.1.1/slabdip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 10:49:12.000000 slabdip-4.1.1/slabdip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:49:12.000000 slabdip-4.1.1/slabdip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 10:49:12.000000 slabdip-4.1.1/slabdip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 10:49:12.000000 slabdip-4.1.1/slabdip.egg-info/top_level.txt
```

### Comparing `./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/data/subduction_data.csv` & `slabdip-4.1.1/slabdip/data/subduction_data.csv`

 * *Files identical despite different names*

### Comparing `./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip/predictor.py` & `slabdip-4.1.1/slabdip/predictor.py`

 * *Files identical despite different names*

### Comparing `./Users/ben/miniforge3/envs/mapping/lib/python3.9/site-packages/slabdip-4.1-py3.9.egg-info/PKG-INFO` & `slabdip-4.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: slabdip
-Version: 4.1
+Version: 4.1.1
 Summary: Setting up a python package
 Home-page: https://github.com/brmather/Slab-Dip
 Author: Ben Mather
 Author-email: ben.mather@sydney.edu.au
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -94,9 +92,7 @@
 dataFrame = dipper.tessellate_slab_dip(0)
 ```
 
 #### References
 
 - Clennett, E. J., Sigloch, K., Mihalynuk, M. G., Seton, M., Henderson, M. A., Hosseini, K., et al. (2020). A Quantitative Tomotectonic Plate Reconstruction of Western North America and the Eastern Pacific Basin. Geochemistry, Geophysics, Geosystems, 21(8), 1–25. https://doi.org/10.1029/2020GC009117
 - Müller, R. D., Zahirovic, S., Williams, S. E., Cannon, J., Seton, M., Bower, D. J., et al. (2019). A Global Plate Model Including Lithospheric Deformation Along Major Rifts and Orogens Since the Triassic. Tectonics, 38(6), 1884–1907. https://doi.org/10.1029/2018TC005462
-
-
```

