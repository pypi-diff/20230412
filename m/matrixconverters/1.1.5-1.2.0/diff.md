# Comparing `tmp/matrixconverters-1.1.5.tar.gz` & `tmp/matrixconverters-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixconverters-1.1.5.tar", last modified: Sun Nov 21 02:34:31 2021, max compression
+gzip compressed data, was "matrixconverters-1.2.0.tar", last modified: Wed Apr 12 10:33:16 2023, max compression
```

## Comparing `matrixconverters-1.1.5.tar` & `matrixconverters-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2021-11-21 02:34:31.264760 matrixconverters-1.1.5/
--rw-rw-rw-   0        0        0       41 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      650 2021-11-21 02:34:31.264760 matrixconverters-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-11-21 02:34:31.264760 matrixconverters-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1725 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-21 02:34:31.233545 matrixconverters-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2021-11-21 02:34:31.249138 matrixconverters-1.1.5/src/matrixconverters/
--rw-rw-rw-   0        0        0      278 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/__init__.py
--rw-rw-rw-   0        0        0       22 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/_version.py
--rw-rw-rw-   0        0        0     3829 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/read_csv.py
--rw-rw-rw-   0        0        0    18483 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/read_ptv.py
--rw-rw-rw-   0        0        0    14919 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/save_ptv.py
-drwxrwxrwx   0        0        0        0 2021-11-21 02:34:31.264760 matrixconverters-1.1.5/src/matrixconverters/tests/
--rw-rw-rw-   0        0        0      244 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/__init__.py
--rw-rw-rw-   0        0        0       85 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix.csv
--rw-rw-rw-   0        0        0      448 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_bi_format.mtx
--rw-rw-rw-   0        0        0      658 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_bk_format.mtx
--rw-rw-rw-   0        0        0      443 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_bl_format.mtx
--rw-rw-rw-   0        0        0      344 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_e_format.mtx
--rw-rw-rw-   0        0        0      599 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_o_format.mtx
--rw-rw-rw-   0        0        0      263 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_o_format_with_dashes.mtx
--rw-rw-rw-   0        0        0      276 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_o_format_with_zeros.mtx
--rw-rw-rw-   0        0        0      492 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_o_format_without_names.mtx
--rw-rw-rw-   0        0        0      575 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_or_format.mtx
--rw-rw-rw-   0        0        0      340 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_s_format.mtx
--rw-rw-rw-   0        0        0      505 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/matrix_v_format.mtx
--rw-rw-rw-   0        0        0      831 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/test_read_csv.py
--rw-rw-rw-   0        0        0    10891 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/test_read_visum.py
--rw-rw-rw-   0        0        0     1381 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/test_save_psv.py
--rw-rw-rw-   0        0        0     1893 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/test_xarray2netcdf.py
--rw-rw-rw-   0        0        0       85 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/tests/zones.csv
--rw-rw-rw-   0        0        0     1128 2021-11-21 02:20:22.000000 matrixconverters-1.1.5/src/matrixconverters/xarray2netcdf.py
-drwxrwxrwx   0        0        0        0 2021-11-21 02:34:31.249138 matrixconverters-1.1.5/src/matrixconverters.egg-info/
--rw-rw-rw-   0        0        0      650 2021-11-21 02:34:31.000000 matrixconverters-1.1.5/src/matrixconverters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1340 2021-11-21 02:34:31.000000 matrixconverters-1.1.5/src/matrixconverters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-21 02:34:31.000000 matrixconverters-1.1.5/src/matrixconverters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-11-21 02:34:31.000000 matrixconverters-1.1.5/src/matrixconverters.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2021-11-21 02:34:31.000000 matrixconverters-1.1.5/src/matrixconverters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2021-11-21 02:34:31.000000 matrixconverters-1.1.5/src/matrixconverters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 10:33:16.310568 matrixconverters-1.2.0/
+-rw-rw-rw-   0        0        0       41 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      600 2023-04-12 10:33:16.310568 matrixconverters-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:33:16.310568 matrixconverters-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:33:16.294942 matrixconverters-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 10:33:16.294942 matrixconverters-1.2.0/src/matrixconverters/
+-rw-rw-rw-   0        0        0       33 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/_version.py
+-rw-rw-rw-   0        0        0     3829 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/read_csv.py
+-rw-rw-rw-   0        0        0    18483 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/read_ptv.py
+-rw-rw-rw-   0        0        0    14919 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/save_ptv.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:33:16.310568 matrixconverters-1.2.0/src/matrixconverters/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix.csv
+-rw-rw-rw-   0        0        0      448 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_bi_format.mtx
+-rw-rw-rw-   0        0        0      658 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_bk_format.mtx
+-rw-rw-rw-   0        0        0      443 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_bl_format.mtx
+-rw-rw-rw-   0        0        0      344 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_e_format.mtx
+-rw-rw-rw-   0        0        0      599 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_o_format.mtx
+-rw-rw-rw-   0        0        0      263 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_o_format_with_dashes.mtx
+-rw-rw-rw-   0        0        0      276 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_o_format_with_zeros.mtx
+-rw-rw-rw-   0        0        0      492 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_o_format_without_names.mtx
+-rw-rw-rw-   0        0        0      575 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_or_format.mtx
+-rw-rw-rw-   0        0        0      340 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_s_format.mtx
+-rw-rw-rw-   0        0        0      505 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/matrix_v_format.mtx
+-rw-rw-rw-   0        0        0      831 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/test_read_csv.py
+-rw-rw-rw-   0        0        0    10891 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/test_read_visum.py
+-rw-rw-rw-   0        0        0     1362 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/test_save_psv.py
+-rw-rw-rw-   0        0        0     1955 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/test_xarray2netcdf.py
+-rw-rw-rw-   0        0        0       85 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/tests/zones.csv
+-rw-rw-rw-   0        0        0     1130 2023-04-12 09:48:16.000000 matrixconverters-1.2.0/src/matrixconverters/xarray2netcdf.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:33:16.294942 matrixconverters-1.2.0/src/matrixconverters.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-04-12 10:33:16.000000 matrixconverters-1.2.0/src/matrixconverters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1340 2023-04-12 10:33:16.000000 matrixconverters-1.2.0/src/matrixconverters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:33:16.000000 matrixconverters-1.2.0/src/matrixconverters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-12 10:33:16.000000 matrixconverters-1.2.0/src/matrixconverters.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2023-04-12 10:33:16.000000 matrixconverters-1.2.0/src/matrixconverters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-12 10:33:16.000000 matrixconverters-1.2.0/src/matrixconverters.egg-info/top_level.txt
```

### Comparing `matrixconverters-1.1.5/PKG-INFO` & `matrixconverters-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Metadata-Version: 2.1
 Name: matrixconverters
-Version: 1.1.5
+Version: 1.2.0
 Summary: package to read and write PTV-Visum Matrix Formats
 Home-page: https://maxbo.github.io/cythonarrays/
 Author: Max Bohnet
 Author-email: bohnet@ggr-planung.de
-License: UNKNOWN
 Keywords: Visum PTV Matrix numpy xarray
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
-
-UNKNOWN
-
```

### Comparing `matrixconverters-1.1.5/setup.py` & `matrixconverters-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Jun 10 20:33:08 2016
 
 @author: MaxBohnet
 """
-
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 from cythoninstallhelpers.get_version import get_version
 from cythoninstallhelpers.make_cython_extensions import make_extensions
 
 
 ext_modnames = []
 
 package_name = "matrixconverters"
@@ -37,24 +36,24 @@
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
         'Programming Language :: Cython',
 
     ],
     keywords='Visum PTV Matrix numpy xarray',
 
-    packages=find_packages('src', exclude=['ez_setup']),
+    packages=find_namespace_packages('src', exclude=['ez_setup']),
     package_dir={'': 'src'},
     package_data={'': ['*.pxd', '*.mtx', '*.csv']},
     include_package_data=True,
     zip_safe=False,
     data_files=[
         ],
 
     tests_require=['pytest', ],
 
     install_requires=[
         'xarray',
-        'netCDF4',
+        'h5netcdf',
         'cythoninstallhelpers',
     ],
     ext_modules=make_extensions(ext_modnames),
 )
```

### Comparing `matrixconverters-1.1.5/src/matrixconverters/read_csv.py` & `matrixconverters-1.2.0/src/matrixconverters/read_csv.py`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/read_ptv.py` & `matrixconverters-1.2.0/src/matrixconverters/read_ptv.py`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/save_ptv.py` & `matrixconverters-1.2.0/src/matrixconverters/save_ptv.py`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/tests/matrix_bk_format.mtx` & `matrixconverters-1.2.0/src/matrixconverters/tests/matrix_bk_format.mtx`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/tests/matrix_o_format.mtx` & `matrixconverters-1.2.0/src/matrixconverters/tests/matrix_o_format.mtx`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/tests/matrix_or_format.mtx` & `matrixconverters-1.2.0/src/matrixconverters/tests/matrix_or_format.mtx`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/tests/test_read_csv.py` & `matrixconverters-1.2.0/src/matrixconverters/tests/test_read_csv.py`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/tests/test_read_visum.py` & `matrixconverters-1.2.0/src/matrixconverters/tests/test_read_visum.py`

 * *Files identical despite different names*

### Comparing `matrixconverters-1.1.5/src/matrixconverters/tests/test_save_psv.py` & `matrixconverters-1.2.0/src/matrixconverters/tests/test_save_psv.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Created on Fri Jun 10 21:00:21 2016
 
 @author: MaxBohnet
 """
 
 import pytest
 import os
-import numpy as np
 from matrixconverters.read_ptv import ReadPTVMatrix
 from matrixconverters.save_ptv import SavePTV
 from matrixconverters.tests.test_read_visum import folder, matrix_fn
 
 
 @pytest.fixture(scope='class')
 def matrix_cc(folder: str) -> str:
```

### Comparing `matrixconverters-1.1.5/src/matrixconverters/xarray2netcdf.py` & `matrixconverters-1.2.0/src/matrixconverters/xarray2netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 import xarray as xr
 
 
 def xr2netcdf(dataset: xr.Dataset,
               filepath: str,
               mode: str = 'w',
-              engine: str = 'netcdf4',
+              engine: str = 'h5netcdf',
               compressed: bool = True,
               complevel: int = 2, ):
     """
     save dataset as netcdf-file to filepath using the given compression level
 
     Parameters
     ----------
     dataset :
         the xarray-dataset to store
     filepath :
         the path where the netcdf-file shold be stored
     mode :
         write (w) or append (a)
     engine :
-        the engine to use (default is netcdf4)
+        the engine to use (default is h5netcdf)
     compressed :
         if False, the data-variables are not compressed
     complevel :
         the compression-level between 1 and 9
         1 is faster, 9 uses a more efficient compression, but is much slower
         2 is in general a good compromise
     """
```

### Comparing `matrixconverters-1.1.5/src/matrixconverters.egg-info/PKG-INFO` & `matrixconverters-1.2.0/src/matrixconverters.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Metadata-Version: 2.1
 Name: matrixconverters
-Version: 1.1.5
+Version: 1.2.0
 Summary: package to read and write PTV-Visum Matrix Formats
 Home-page: https://maxbo.github.io/cythonarrays/
 Author: Max Bohnet
 Author-email: bohnet@ggr-planung.de
-License: UNKNOWN
 Keywords: Visum PTV Matrix numpy xarray
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
-
-UNKNOWN
-
```

### Comparing `matrixconverters-1.1.5/src/matrixconverters.egg-info/SOURCES.txt` & `matrixconverters-1.2.0/src/matrixconverters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

