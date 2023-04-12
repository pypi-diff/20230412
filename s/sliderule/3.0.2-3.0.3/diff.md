# Comparing `tmp/sliderule-3.0.2.tar.gz` & `tmp/sliderule-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.0.2.tar", last modified: Tue Apr 11 21:16:11 2023, max compression
+gzip compressed data, was "sliderule-3.0.3.tar", last modified: Wed Apr 12 02:29:51 2023, max compression
```

## Comparing `sliderule-3.0.2.tar` & `sliderule-3.0.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.864435 sliderule-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-11 21:16:02.000000 sliderule-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-11 21:16:11.864435 sliderule-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-11 21:16:02.000000 sliderule-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-11 21:16:02.000000 sliderule-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 21:16:11.864435 sliderule-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-11 21:16:02.000000 sliderule-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.860435 sliderule-3.0.2/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24891 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    35898 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.860435 sliderule-3.0.2/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      953 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.864435 sliderule-3.0.2/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/_landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/hls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 02:29:51.273279 sliderule-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-12 02:29:38.000000 sliderule-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-12 02:29:51.273279 sliderule-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-12 02:29:38.000000 sliderule-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-12 02:29:38.000000 sliderule-3.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 02:29:51.273279 sliderule-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-12 02:29:38.000000 sliderule-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 02:29:51.269279 sliderule-3.0.3/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/arcticdem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24891 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35898 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-12 02:29:38.000000 sliderule-3.0.3/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 02:29:51.269279 sliderule-3.0.3/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-12 02:29:51.000000 sliderule-3.0.3/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-04-12 02:29:51.000000 sliderule-3.0.3/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 02:29:51.000000 sliderule-3.0.3/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-12 02:29:51.000000 sliderule-3.0.3/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 02:29:51.000000 sliderule-3.0.3/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 02:29:51.273279 sliderule-3.0.3/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/hls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-12 02:29:38.000000 sliderule-3.0.3/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-12 02:29:38.000000 sliderule-3.0.3/version.txt
```

### Comparing `sliderule-3.0.2/PKG-INFO` & `sliderule-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.2/README.md` & `sliderule-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/setup.py` & `sliderule-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/arcticdem.py` & `sliderule-3.0.3/sliderule/arcticdem.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/earthdata.py` & `sliderule-3.0.3/sliderule/earthdata.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/gedi.py` & `sliderule-3.0.3/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/h5.py` & `sliderule-3.0.3/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/icesat2.py` & `sliderule-3.0.3/sliderule/icesat2.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/io.py` & `sliderule-3.0.3/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/ipxapi.py` & `sliderule-3.0.3/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/ipysliderule.py` & `sliderule-3.0.3/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule/sliderule.py` & `sliderule-3.0.3/sliderule/sliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/sliderule.egg-info/PKG-INFO` & `sliderule-3.0.3/sliderule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.2/sliderule.egg-info/SOURCES.txt` & `sliderule-3.0.3/sliderule.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+version.txt
 sliderule/__init__.py
 sliderule/arcticdem.py
 sliderule/earthdata.py
 sliderule/gedi.py
 sliderule/h5.py
 sliderule/icesat2.py
 sliderule/io.py
```

### Comparing `sliderule-3.0.2/utils/_landsat.py` & `sliderule-3.0.3/utils/_landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/big_query.py` & `sliderule-3.0.3/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.0.3/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.0.3/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.0.3/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/extract_h5_dataset.py` & `sliderule-3.0.3/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/hls.py` & `sliderule-3.0.3/utils/hls.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/icepyx_region.py` & `sliderule-3.0.3/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/landsat.py` & `sliderule-3.0.3/utils/landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/monitor.py` & `sliderule-3.0.3/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/query_cmr.py` & `sliderule-3.0.3/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/query_elevations.py` & `sliderule-3.0.3/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/query_metrics.py` & `sliderule-3.0.3/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/query_photons.py` & `sliderule-3.0.3/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/query_stac.py` & `sliderule-3.0.3/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/query_version.py` & `sliderule-3.0.3/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/region_of_interest.py` & `sliderule-3.0.3/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/results_to_s3.py` & `sliderule-3.0.3/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/stac.py` & `sliderule-3.0.3/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/stream_events.py` & `sliderule-3.0.3/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/tail_events.py` & `sliderule-3.0.3/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.2/utils/utils.py` & `sliderule-3.0.3/utils/utils.py`

 * *Files identical despite different names*

