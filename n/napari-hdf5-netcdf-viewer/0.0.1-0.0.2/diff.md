# Comparing `tmp/napari-hdf5-netcdf-viewer-0.0.1.tar.gz` & `tmp/napari-hdf5-netcdf-viewer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-hdf5-netcdf-viewer-0.0.1.tar", last modified: Wed Apr 12 01:45:08 2023, max compression
+gzip compressed data, was "napari-hdf5-netcdf-viewer-0.0.2.tar", last modified: Wed Apr 12 02:28:28 2023, max compression
```

## Comparing `napari-hdf5-netcdf-viewer-0.0.1.tar` & `napari-hdf5-netcdf-viewer-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 01:45:08.002993 napari-hdf5-netcdf-viewer-0.0.1/
--rw-rw-r--   0 yunhalee   (501) staff       (20)     1517 2022-10-28 18:43:40.000000 napari-hdf5-netcdf-viewer-0.0.1/LICENSE
--rw-r--r--   0 yunhalee   (501) staff       (20)       96 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.0.1/MANIFEST.in
--rw-r--r--   0 yunhalee   (501) staff       (20)      817 2023-04-12 01:45:08.003176 napari-hdf5-netcdf-viewer-0.0.1/PKG-INFO
--rw-rw-r--   0 yunhalee   (501) staff       (20)       84 2022-10-29 03:05:16.000000 napari-hdf5-netcdf-viewer-0.0.1/README.md
--rw-r--r--   0 yunhalee   (501) staff       (20)       91 2022-10-11 15:38:42.000000 napari-hdf5-netcdf-viewer-0.0.1/pyproject.toml
--rw-r--r--   0 yunhalee   (501) staff       (20)     1290 2023-04-12 01:45:08.004470 napari-hdf5-netcdf-viewer-0.0.1/setup.cfg
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 01:45:07.993479 napari-hdf5-netcdf-viewer-0.0.1/src/
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 01:45:07.998379 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/
--rw-r--r--   0 yunhalee   (501) staff       (20)      106 2022-10-28 18:32:59.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/__init__.py
--rw-r--r--   0 yunhalee   (501) staff       (20)     8597 2023-04-11 15:54:49.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/_reader.py
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 01:45:08.002448 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/_tests/
--rw-r--r--   0 yunhalee   (501) staff       (20)        0 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/_tests/__init__.py
--rw-r--r--   0 yunhalee   (501) staff       (20)      407 2023-04-11 23:50:14.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/_tests/test_quick_hdf5_netcdf_viewer.py
--rw-r--r--   0 yunhalee   (501) staff       (20)      220 2023-04-11 17:08:17.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/_widget.py
--rw-r--r--   0 yunhalee   (501) staff       (20)      574 2023-04-11 23:39:29.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/napari.yaml
--rw-r--r--   0 yunhalee   (501) staff       (20)     9072 2023-04-11 23:43:19.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py
-drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 01:45:08.001623 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/
--rw-r--r--   0 yunhalee   (501) staff       (20)      817 2023-04-12 01:45:07.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yunhalee   (501) staff       (20)      717 2023-04-12 01:45:07.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)        1 2023-04-12 01:45:07.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       84 2023-04-12 01:45:07.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       92 2023-04-12 01:45:07.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/requires.txt
--rw-r--r--   0 yunhalee   (501) staff       (20)       26 2023-04-12 01:45:07.000000 napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.505597 napari-hdf5-netcdf-viewer-0.0.2/
+-rw-rw-r--   0 yunhalee   (501) staff       (20)     1517 2022-10-28 18:43:40.000000 napari-hdf5-netcdf-viewer-0.0.2/LICENSE
+-rw-r--r--   0 yunhalee   (501) staff       (20)       96 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.0.2/MANIFEST.in
+-rw-r--r--   0 yunhalee   (501) staff       (20)      817 2023-04-12 02:28:28.505804 napari-hdf5-netcdf-viewer-0.0.2/PKG-INFO
+-rw-rw-r--   0 yunhalee   (501) staff       (20)       84 2022-10-29 03:05:16.000000 napari-hdf5-netcdf-viewer-0.0.2/README.md
+-rw-r--r--   0 yunhalee   (501) staff       (20)       91 2022-10-11 15:38:42.000000 napari-hdf5-netcdf-viewer-0.0.2/pyproject.toml
+-rw-r--r--   0 yunhalee   (501) staff       (20)     1290 2023-04-12 02:28:28.506796 napari-hdf5-netcdf-viewer-0.0.2/setup.cfg
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.498484 napari-hdf5-netcdf-viewer-0.0.2/src/
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.501664 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/
+-rw-r--r--   0 yunhalee   (501) staff       (20)      106 2022-10-28 18:32:59.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/__init__.py
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.505178 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/_tests/
+-rw-r--r--   0 yunhalee   (501) staff       (20)        0 2023-03-30 14:07:57.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/_tests/__init__.py
+-rw-r--r--   0 yunhalee   (501) staff       (20)      407 2023-04-11 23:50:14.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/_tests/test_quick_hdf5_netcdf_viewer.py
+-rw-r--r--   0 yunhalee   (501) staff       (20)      574 2023-04-11 23:39:29.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/napari.yaml
+-rw-r--r--   0 yunhalee   (501) staff       (20)     9072 2023-04-11 23:43:19.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py
+drwxr-xr-x   0 yunhalee   (501) staff       (20)        0 2023-04-12 02:28:28.504268 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/
+-rw-r--r--   0 yunhalee   (501) staff       (20)      817 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yunhalee   (501) staff       (20)      635 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)        1 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)       84 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)       92 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/requires.txt
+-rw-r--r--   0 yunhalee   (501) staff       (20)       26 2023-04-12 02:28:28.000000 napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/top_level.txt
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.1/LICENSE` & `napari-hdf5-netcdf-viewer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-hdf5-netcdf-viewer-0.0.1/PKG-INFO` & `napari-hdf5-netcdf-viewer-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-hdf5-netcdf-viewer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A napari plugin for quick-viewing HDF5 and NetCDF files
 Home-page: https://github.com/yunhal/napari-hdf5-netcdf-viewer
 Author: Yunha Lee
 Author-email: yunha.lee.00@gmail.com
 Project-URL: Bug Tracker, https://github.com/yunhal/napari-hdf5-netcdf-viewer/issues
 Project-URL: Documentation, https://github.com/yunhal/napari-hdf5-netcdf-viewer#README.md
 Project-URL: Source Code, https://github.com/yunhal/napari-hdf5-netcdf-viewer
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.1/setup.cfg` & `napari-hdf5-netcdf-viewer-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-hdf5-netcdf-viewer
-version = 0.0.1
+version = 0.0.2
 description = A napari plugin for quick-viewing HDF5 and NetCDF files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yunhal/napari-hdf5-netcdf-viewer
 author = Yunha Lee
 author_email = yunha.lee.00@gmail.com
 classifiers =
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/_reader.py` & `napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-"""
-This module is an example of a barebones numpy reader plugin for napari.
-
-It implements the Reader specification, but your plugin may choose to
-implement multiple readers or even other plugin contributions. see:
-https://napari.org/stable/plugins/guides.html?#readers
-"""
 import napari
 import h5py
 import numpy as np
 import pathlib
 from pathlib import Path
 
 from magicgui import magicgui, magic_factory
@@ -185,15 +178,33 @@
     """
 
     curr_scale = layer.scale
     curr_scale[axis] = value
     layer.scale = curr_scale
 
 
-def napari_get_reader(path):
+'''
+need to update in future
+
+def geo_view_enabled (data):
+
+    if (data.ndim == 2):
+        print("latitude array has been inversed for napari visualization")
+        set_scale_at_axis(layer, axis = -2, value = -1)
+
+    if (data.ndim >= 3):
+        set_scale_at_axis(layer, axis = -2, value = -1)
+        viewer.dims.axis_labels = ("height", "lat", "lon") 
+        viewer.dims.ndisplay = 3
+        viewer.camera.angles = (-1.7571935971733401, -26.823353526707475, -77.73048528666025)
+
+'''
+
+def load_path(path: str):
+
     """read file structure and open the images with napari if the path file format is hdf or netcdf.
     Parameters
     ----------
     path: str
         hdf5 or netcdf file path
     -------
     """
@@ -231,7 +242,19 @@
         print("Failure: {} is recognized as neither hdf5 nor netcdf".format(path))
 
 @magic_factory
 def make_widget(file_path: "pathlib.Path" = Path()):
     filename = str(file_path)
     load_path(filename)
 
+
+if __name__ == "__main__":
+
+    fpath = '/Users/yunhalee/nc_h5_files/OMI-Aura_L3-OMTO3e_2005m1214_v002-2006m0929t143855.h5'
+
+    viewer = napari.Viewer()
+    viewer.window.add_dock_widget(make_widget(), area="right")  
+
+    napari.run()
+
+    load_path(fpath)
+
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer/napari.yaml` & `napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO` & `napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-hdf5-netcdf-viewer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A napari plugin for quick-viewing HDF5 and NetCDF files
 Home-page: https://github.com/yunhal/napari-hdf5-netcdf-viewer
 Author: Yunha Lee
 Author-email: yunha.lee.00@gmail.com
 Project-URL: Bug Tracker, https://github.com/yunhal/napari-hdf5-netcdf-viewer/issues
 Project-URL: Documentation, https://github.com/yunhal/napari-hdf5-netcdf-viewer#README.md
 Project-URL: Source Code, https://github.com/yunhal/napari-hdf5-netcdf-viewer
```

### Comparing `napari-hdf5-netcdf-viewer-0.0.1/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt` & `napari-hdf5-netcdf-viewer-0.0.2/src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/napari_hdf5_netcdf_viewer/__init__.py
-src/napari_hdf5_netcdf_viewer/_reader.py
-src/napari_hdf5_netcdf_viewer/_widget.py
 src/napari_hdf5_netcdf_viewer/napari.yaml
 src/napari_hdf5_netcdf_viewer/quick_hdf5_netcdf_viewer.py
 src/napari_hdf5_netcdf_viewer.egg-info/PKG-INFO
 src/napari_hdf5_netcdf_viewer.egg-info/SOURCES.txt
 src/napari_hdf5_netcdf_viewer.egg-info/dependency_links.txt
 src/napari_hdf5_netcdf_viewer.egg-info/entry_points.txt
 src/napari_hdf5_netcdf_viewer.egg-info/requires.txt
```

