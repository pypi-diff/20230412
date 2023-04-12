# Comparing `tmp/discminer-0.1.0.tar.gz` & `tmp/discminer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.1.0.tar", last modified: Tue Apr  4 14:51:48 2023, max compression
+gzip compressed data, was "discminer-0.1.1.tar", last modified: Wed Apr 12 17:35:31 2023, max compression
```

## Comparing `discminer-0.1.0.tar` & `discminer-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-04 14:51:48.872094 discminer-0.1.0/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.1.0/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-04 14:51:48.872291 discminer-0.1.0/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.1.0/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-04 14:51:48.845485 discminer-0.1.0/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     4979 2023-03-19 13:26:42.000000 discminer-0.1.0/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.1.0/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:01:36.000000 discminer-0.1.0/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     4239 2023-03-07 14:28:23.000000 discminer-0.1.0/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     5101 2023-04-03 15:04:19.000000 discminer-0.1.0/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4562 2023-04-02 22:11:37.000000 discminer-0.1.0/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4511 2023-04-02 22:12:18.000000 discminer-0.1.0/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     7132 2023-04-02 22:02:07.000000 discminer-0.1.0/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    10949 2023-04-03 15:09:09.000000 discminer-0.1.0/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5592 2023-04-03 12:50:09.000000 discminer-0.1.0/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4587 2023-04-03 12:49:39.000000 discminer-0.1.0/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000     8203 2023-04-02 22:04:40.000000 discminer-0.1.0/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-04 14:51:48.858081 discminer-0.1.0/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.1.0/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-04 14:22:43.000000 discminer-0.1.0/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.1.0/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.1.0/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8108 2023-03-26 15:14:30.000000 discminer-0.1.0/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74020 2023-04-04 09:57:01.000000 discminer-0.1.0/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    70634 2023-04-04 09:46:54.000000 discminer-0.1.0/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4146 2023-03-17 13:08:01.000000 discminer-0.1.0/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-04 14:51:48.865950 discminer-0.1.0/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.1.0/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.1.0/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.1.0/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.1.0/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.1.0/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.1.0/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.1.0/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.1.0/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    24570 2023-04-02 22:22:34.000000 discminer-0.1.0/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    34863 2023-04-04 10:02:38.000000 discminer-0.1.0/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.1.0/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-04 14:51:48.868612 discminer-0.1.0/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.1.0/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.1.0/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.1.0/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.1.0/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-04 14:51:48.859711 discminer-0.1.0/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-04 14:51:48.000000 discminer-0.1.0/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-04 14:51:48.000000 discminer-0.1.0/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-04 14:51:48.000000 discminer-0.1.0/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-04 14:51:48.000000 discminer-0.1.0/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-04 14:51:48.000000 discminer-0.1.0/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.1.0/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-04 14:51:48.872779 discminer-0.1.0/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.1.0/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-04 14:51:48.871372 discminer-0.1.0/template/
--rw-r--r--   0 aizquier  (8218)     5000     8130 2023-04-04 14:41:58.000000 discminer-0.1.0/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.1.0/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.1.0/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.1.0/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.394144 discminer-0.1.1/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.1.1/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-12 17:35:31.394499 discminer-0.1.1/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.1.1/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.369120 discminer-0.1.1/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     4979 2023-03-19 13:26:42.000000 discminer-0.1.1/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.1.1/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:01:36.000000 discminer-0.1.1/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     4239 2023-03-07 14:28:23.000000 discminer-0.1.1/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     5101 2023-04-03 15:04:19.000000 discminer-0.1.1/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4562 2023-04-02 22:11:37.000000 discminer-0.1.1/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4511 2023-04-02 22:12:18.000000 discminer-0.1.1/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     7134 2023-04-12 16:20:22.000000 discminer-0.1.1/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    10949 2023-04-03 15:09:09.000000 discminer-0.1.1/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5592 2023-04-03 12:50:09.000000 discminer-0.1.1/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     4608 2023-04-12 16:36:38.000000 discminer-0.1.1/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000     8203 2023-04-02 22:04:40.000000 discminer-0.1.1/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.381277 discminer-0.1.1/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.1.1/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-12 17:33:33.000000 discminer-0.1.1/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.1.1/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.1.1/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8108 2023-03-26 15:14:30.000000 discminer-0.1.1/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74020 2023-04-04 09:57:01.000000 discminer-0.1.1/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    70761 2023-04-12 16:51:53.000000 discminer-0.1.1/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4146 2023-03-17 13:08:01.000000 discminer-0.1.1/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.385849 discminer-0.1.1/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.1.1/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.1.1/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.1.1/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    25381 2023-04-12 16:18:52.000000 discminer-0.1.1/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.1.1/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.1.1/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.388276 discminer-0.1.1/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.1.1/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.1.1/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.1.1/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.1.1/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.383393 discminer-0.1.1/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.1.1/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-12 17:35:31.395121 discminer-0.1.1/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.1.1/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.393004 discminer-0.1.1/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8130 2023-04-04 14:41:58.000000 discminer-0.1.1/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.1.1/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.1.1/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.1.1/template/prepare_data.py
```

### Comparing `discminer-0.1.0/LICENSE` & `discminer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/PKG-INFO` & `discminer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.1.0 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.1.1 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.1.0/README.md` & `discminer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/make_channels.py` & `discminer-0.1.1/_mining/make_channels.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/make_parfile.py` & `discminer-0.1.1/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/make_single_moments.py` & `discminer-0.1.1/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/plot_attributes_model.py` & `discminer-0.1.1/_mining/plot_attributes_model.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/plot_azimuthal_profiles.py` & `discminer-0.1.1/_mining/plot_azimuthal_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/plot_moment+offset.py` & `discminer-0.1.1/_mining/plot_moment+offset.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/plot_moment+residuals.py` & `discminer-0.1.1/_mining/plot_moment+residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/plot_peak_residuals.py` & `discminer-0.1.1/_mining/plot_peak_residuals.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,22 +182,22 @@
 
     elif args.surface in ['low', 'lower']:
         z_func = cart.z_lower_exp_tapered
         z_pars = best['height_lower']
     
     fig, ax = make_round_map(folded_map, levels_resid, pick.X*u.au, pick.Y*u.au, R_prof[-1]*u.au,
                              z_func=z_func, z_pars=z_pars, incl=incl, PA=PA, xc=xc, yc=yc,
-                             cmap=cmap_res, unit=unit, fmt=cfmt, 
+                             cmap=cmap_res, clabel=unit, fmt=cfmt, 
                              rings=rings,
                              mask_wedge=(90, 270)*u.deg,
                              mask_inner=R_prof[0]*u.au)
     ax.scatter(lev*cos_peak, lev*sin_peak, edgecolors='none', facecolors=color, alpha=0.2, s=100)
     ax.scatter(lev*cos_peak, lev*sin_peak, edgecolors='none', facecolors=color, alpha=1.0, s=10)
     ax.scatter(lev*cos_peak, lev*sin_peak, edgecolors='0.3', facecolors='none', alpha=1.0, s=100)
-    ax.set_title('%s, folded map'%ctitle, fontsize=12, color='k')
+    ax.set_title('%s, folded map'%ctitle, fontsize=16, color='k')
     
 
 plt.savefig('folded_residuals_deproj_%s_%s.png'%(mtags['base'], args.projection), bbox_inches='tight', dpi=200)
 plt.close()
 
 #*************
 #FIND CLUSTERS
```

### Comparing `discminer-0.1.0/_mining/plot_radial_profiles.py` & `discminer-0.1.1/_mining/plot_radial_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/plot_residuals+all.py` & `discminer-0.1.1/_mining/plot_residuals+all.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/_mining/plot_residuals+deproj.py` & `discminer-0.1.1/_mining/plot_residuals+deproj.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,24 +121,24 @@
 
     elif args.surface in ['low', 'lower']:
         z_func = cart.z_lower_exp_tapered
         z_pars = best['height_lower']
     
     fig, ax = make_round_map(residuals, levels_resid, Xproj*u.m, Yproj*u.m, Rout*u.au,
                              z_func=z_func, z_pars=z_pars, incl=incl, PA=PA, xc=xc, yc=yc,
-                             cmap=cmap_res, unit=unit, fmt=cfmt, 
+                             cmap=cmap_res, clabel=unit, fmt=cfmt, 
                              rings=rings, kinks=kinks)
 
 
 elif args.projection=='polar':
     levels_resid = np.linspace(-clim, clim, 48)    
-    fig, ax = make_polar_map(residuals, levels_resid,
-                             R[args.surface]*u.m, phi[args.surface]*u.rad, Rout*u.au,
-                             Rin = datacube.beam_size,
-                             cmap=cmap_res, unit=unit, fmt=cfmt, clabel=clabels[args.moment],
-                             gaps=gaps, rings=rings, kinks=kinks)
+    fig, ax, cbar = make_polar_map(residuals, levels_resid,
+                                   R[args.surface]*u.m, phi[args.surface]*u.rad, Rout*u.au,
+                                   Rin = datacube.beam_size,
+                                   cmap=cmap_res, fmt=cfmt, clabel=clabels[args.moment],
+                                   gaps=gaps, rings=rings, kinks=kinks)
 
-ax.set_title(ctitle, fontsize=12, color='k')
+ax.set_title(ctitle, fontsize=16, color='k')
 
 plt.savefig('residuals_deproj_%s_%s.png'%(mtags['base'], args.projection), bbox_inches='tight', dpi=200)
 plt.show()
 plt.close()
```

### Comparing `discminer-0.1.0/_mining/utils.py` & `discminer-0.1.1/_mining/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/cart.py` & `discminer-0.1.1/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/core.py` & `discminer-0.1.1/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/cube.py` & `discminer-0.1.1/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/disc2d.py` & `discminer-0.1.1/discminer/disc2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,19 +680,22 @@
             int2d_far = int2d['lower'] * v_far
             #vel nans might differ from Int nans when a z surf is zero and SG is active, then nanmax must be used: 
             int2d_full = np.nanmax([int2d_near, int2d_far], axis=0) 
             if rms is not None:
                 noise = np.random.normal(scale=rms, size=int2d_shape)
                 int2d_full += noise
 
-            if make_convolve and self.beam_kernel:
-                int2d_full[np.isnan(int2d_full)] = noise
-                int2d_full = self.beam_area*convolve(int2d_full, self.beam_kernel, preserve_nan=False)
+            if self.beam_kernel is not None:
+                if make_convolve:
+                    int2d_full[np.isnan(int2d_full)] = noise
+                    int2d_full = self.beam_area*convolve(int2d_full, self.beam_kernel, preserve_nan=False)
+                else:
+                    int2d_full *= self.beam_area
+                    int2d_full[~np.isfinite(int2d_full)] = noise
             else:
-                int2d_full *= self.beam_area
                 int2d_full[~np.isfinite(int2d_full)] = noise
                 
             cube.append(int2d_full)
             
         if return_data_only: return np.asarray(cube)
         else: return Cube(np.asarray(cube), header, vchannels, dpc, beam=self.beam_info, filename="./cube_model.fits")
```

### Comparing `discminer-0.1.0/discminer/grid.py` & `discminer-0.1.1/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/icons/button_box.png` & `discminer-0.1.1/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/icons/button_cursor.jpeg` & `discminer-0.1.1/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/icons/button_path.png` & `discminer-0.1.1/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/icons/button_return.png` & `discminer-0.1.1/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/icons/button_surface.png` & `discminer-0.1.1/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/icons/button_trash.jpg` & `discminer-0.1.1/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/pick.py` & `discminer-0.1.1/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/plottools.py` & `discminer-0.1.1/discminer/plottools.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import numpy as np
 from math import ceil
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 from collections.abc import Iterable
 from .tools.utils import weighted_std
 from .tools.fit_kernel import _gauss
-
+from .grid import GridTools
+        
 SMALL_SIZE = 10
 MEDIUM_SIZE = 15
 BIGGER_SIZE = 22
 
 _residuals_colors = {
     'velocity': ["#"+tmp for tmp in ["000b14","004f8f","1f9aff","fff7db","ff5a47","cc0033","140200"]],
     'linewidth': ["#"+tmp for tmp in ["000b14","036407","81ae71","fff7db","ff5a47","cc0033","140200"]],
@@ -184,15 +185,15 @@
         if orientation=='vertical': return fig.add_axes([x1+0.5*dx, y0+0.1*h, dx, h-0.2*h])        
     else:
         if orientation=='horizontal': return fig.add_axes([x0, y0-0.5*dy, w, dy])
         if orientation=='vertical': return fig.add_axes([x1+0.5*dx, y0, dx, h])        
         
 def make_round_cbar(ax, Rout, levels,
                     rwidth=0.06, cmap=get_discminer_cmap('velocity'),
-                    quadrant=2, unit='km/s', fmt='%4.1f'):
+                    quadrant=2, clabel='km/s', fmt='%4.1f'):
 
     sign_xy = {1: [1,1],
                2: [-1,1],
                3: [-1,-1],
                4: [1,-1],
     }[quadrant]
     
@@ -243,23 +244,42 @@
     cbar_im = ax.contourf(xx,yy, cbar_polar, levels=levels, cmap=cmap, extend='both', origin='lower') #np.ma.array(cbar_polar, mask=~mask_polar )
 
     cbar_levels_pol = np.linspace(levels[0], levels[-1], 5)
     cbar_levels_phi = cbar_lev2phi(cbar_levels_pol)
 
     for i,cbi in enumerate(cbar_levels_phi):
         Rtext = r1 + 0.03*Rout
-        ax.text(Rtext*np.cos(cbi), Rtext*np.sin(cbi), fmt%cbar_levels_pol[i], fontsize=SMALL_SIZE+1, c='0.7',
+        ax.text(Rtext*np.cos(cbi), Rtext*np.sin(cbi), fmt%cbar_levels_pol[i], fontsize=SMALL_SIZE+2, c='0.7',
                 ha=cticks_ha, va='center', weight='bold', rotation_mode='anchor', rotation=rot_quad(cbi))
 
-    ax.text(sign_xy[0]*Rtext, -sign_xy[1]*0.1*Rout, unit, fontsize=SMALL_SIZE+2, c='0.7', ha='center', va='center', weight='bold', rotation=0)
+    ax.text(sign_xy[0]*Rtext, -sign_xy[1]*0.1*Rout, clabel, fontsize=SMALL_SIZE+3, c='0.7', ha='center', va='center', weight='bold', rotation=0)
 
 #********************
 #DISC PLOT DECORATORS
 #********************
-def _make_text_substructures(ax, gaps=[], rings=[], kinks=[]):
+def _make_text_2D(ax, Rlist, posx=0.0, sposy=1, fmt='%d', va=None, **kwargs_text):
+    if va is not None:
+        _va = va
+        dy = 0
+    else:
+        if sposy<0:
+            _va = 'top'
+            dy = 2
+        elif sposy>0:
+            _va = 'bottom'
+            dy = -1
+        else:
+            return 0
+
+    kwargs = dict(fontsize=SMALL_SIZE+3, ha='center', va=_va, weight='bold', rotation=0)
+    kwargs.update(kwargs_text)
+    for Ri in Rlist:
+        ax.text(posx, sposy*(Ri+dy), fmt%Ri, **kwargs)
+        
+def _make_text_1D_substructures(ax, gaps=[], rings=[], kinks=[]):
     kwargs_text = dict(fontsize=SMALL_SIZE+2, ha='center', va='bottom', transform=ax.transAxes, weight='bold', rotation=90)    
     xlims = ax.get_xlim()
     xext = xlims[1]-xlims[0]
 
     def text_it(R, text):
         for Ri in R:
             if Ri < xlims[0]: continue
@@ -280,164 +300,173 @@
     kwargs_g.update(kwargs_gaps)
     kwargs_r.update(kwargs_rings)
     kwargs_k.update(kwargs_kinks)        
     if twodim:
         nphi = 100
         phi = np.linspace(0, 2*np.pi, nphi)
         phi_deg = np.degrees(phi-np.pi)
+        subst_fmt = zip([gaps, rings, kinks], ['D%d', 'B%d', 'K%d'])
         if polar:
             for R in gaps: ax.plot(phi_deg, [R]*nphi, **kwargs_g)
             for R in rings: ax.plot(phi_deg, [R]*nphi, **kwargs_r)
-            for R in kinks: ax.plot(phi_deg, [R]*nphi, **kwargs_k)                
+            for R in kinks: ax.plot(phi_deg, [R]*nphi, **kwargs_k)
+            if make_labels:
+                for subst, fmt in subst_fmt:
+                    _make_text_2D(ax, subst, posx=-45, fmt=fmt)                
         else:
             cos_phi = np.cos(phi)
             sin_phi = np.sin(phi)
             for R in gaps: ax.plot(R*cos_phi, R*sin_phi, **kwargs_g)
             for R in rings: ax.plot(R*cos_phi, R*sin_phi, **kwargs_r)
             for R in kinks: ax.plot(R*cos_phi, R*sin_phi, **kwargs_k)
+            if make_labels:
+                for subst, fmt in subst_fmt:
+                    _make_text_2D(ax, subst, sposy=-1, fmt=fmt)
+            
     else:
         if func1d=='axvline': func1d=ax.axvline
         elif func1d=='axhline': func1d=ax.axhline            
         for R in gaps: func1d(R, **kwargs_g)
         for R in rings: func1d(R, **kwargs_r)
         for R in kinks: func1d(R, **kwargs_k)
 
         if make_labels:
-            _make_text_substructures(ax, gaps=gaps, rings=rings, kinks=kinks)
+            _make_text_1D_substructures(ax, gaps=gaps, rings=rings, kinks=kinks)
         
     if make_legend and len(gaps)>0: ax.plot([None], [None], label='Gaps', **kwargs_g)
     if make_legend and len(rings)>0: ax.plot([None], [None], label='Rings', **kwargs_r)
     if make_legend and len(kinks)>0: ax.plot([None], [None], label='Kinks', **kwargs_k)
 
     return ax
 
+def _make_radial_grid_2D(ax, Rout, gaps=[], rings=[], kinks=[], make_labels=True, label_freq=2):
+    get_intdigits = lambda n: len(str(n).split('.')[0])
+    
+    angs = np.linspace(0, 2*np.pi, 100)
+    cos_angs = np.cos(angs)
+    sin_angs = np.sin(angs)
+    
+    subst = np.concatenate([gaps, rings, kinks], axis=None)
+    if len(subst)>0:
+        Rref = np.max(subst)
+    else:
+        Rref = 0.0
+    Rref_digits = get_intdigits(Rref)        
+        
+    R_after_ref = 10**(Rref_digits-1)*ceil(Rref/(10**(Rref_digits-1)))
+    Rgrid_polar = np.arange(R_after_ref, Rout, 50)
+    
+    for j,Ri in enumerate(Rgrid_polar[0:-1:2]):
+        if Ri == Rref: continue
+        ax.plot(Ri*cos_angs, Ri*sin_angs, color='k', lw=1.2, alpha=0.5,
+                dash_capstyle='round', dashes=(0.5, 3.5)) 
+
+    for j,Ri in enumerate(Rgrid_polar[1::2]):
+        ax.plot(Ri*cos_angs, Ri*sin_angs, color='k', ls=':', lw=0.4, alpha=1.0)
+
+    if make_labels:
+        _make_text_2D(ax, Rgrid_polar[1::label_freq], sposy=-1, fmt='%d',
+                      fontsize=SMALL_SIZE+3, color='0.1', va='center') #label in the north
+        _make_text_2D(ax, Rgrid_polar[1::label_freq], sposy=1, fmt='%d',
+                      fontsize=SMALL_SIZE+3, color='0.1', va='center') # and south
+
+    ax.plot(0.98*Rout*cos_angs, 0.98*Rout*sin_angs, color='0.4', ls='-', lw=3.0, alpha=1.0)
+    ax.plot(0.99*Rout*cos_angs, 0.99*Rout*sin_angs, color='0.2', ls='-', lw=3.0, alpha=1.0)
+    ax.plot(1.00*Rout*cos_angs, 1.00*Rout*sin_angs, color='0.0', ls='-', lw=3.0, alpha=1.0)
+    
+def _make_azimuthal_grid_2D(ax, Rout):
+    for j, phii in enumerate(np.arange(0, 2*np.pi, np.pi/6)):
+        ax.plot([0, Rout*np.cos(phii)], [0, Rout*np.sin(phii)], color='k', ls=':', lw=0.4, alpha=1.0)
+
+    for deg in np.linspace(0, 90, 4):
+        deg_rad = np.radians(deg)
+        txt = ax.text(1.04*Rout*np.cos(deg_rad), 1.04*Rout*np.sin(deg_rad), r'$%d$'%deg, c='0.0',
+                      fontsize=SMALL_SIZE, ha='center', va='center', weight='bold', rotation=-(90-deg))
+        txt.set_text(r'$%d^{\circ}$'%deg)
+
+def _make_nsky_2D(ax, Rout, xlim, z_func, z_pars, incl, PA, xc=0.0, yc=0.0):
+    ynorth = np.linspace(-1.1*Rout, 1.1*Rout, 100)
+    xnorth = np.zeros_like(ynorth)
+    xn, yn = [], []
+    
+    for i in range(len(ynorth)):
+        xni, yni = GridTools.get_disc_from_sky_coords(xnorth[i], ynorth[i], z_func, z_pars, incl, PA, xc=0, yc=0)
+        xn.append(xni)
+        yn.append(yni)
+
+    xn, yn = np.asarray(xn), np.asarray(yn)
+    ax.plot(xn, yn, color='0.0', lw=1.7, dash_capstyle='round', dashes=(1.5, 2.5))
+    
+    text_nsky = lambda x, y: ax.text(x, y, r'$\vec{\rm N}$$_{\rm sky}$', fontsize=MEDIUM_SIZE,
+                                     ha='center', va='bottom', weight='bold', rotation=np.degrees(-PA))
+
+    if yni>xni:
+        ci = yni
+        cn = yn
+    else:
+        ci = xni
+        cn = xn
+        
+    if ci>xlim:
+        ii = np.argmin(np.abs(cn-xlim))
+        text_nsky(xn[ii], yn[ii])
+    else:
+        text_nsky(xni, yni)
+
+    return xni, yni
+
 
 def make_round_map(
         map2d, levels, X, Y, Rout,
         z_func=None, z_pars=None, incl=None, PA=None, xc=0, yc=0, #Optional, make N-sky axis
         fig=None, ax=None,
-        rwidth=0.06, cmap=get_discminer_cmap('velocity'), unit='km/s', fmt='%5.2f', quadrant=None, #cbar kwargs
+        rwidth=0.06, cmap=get_discminer_cmap('velocity'), clabel='km/s', fmt='%5.2f', quadrant=None, #cbar kwargs
         gaps=[], rings=[], kinks=[],
         label_gaps=False, label_rings=True, label_kinks=True,
         mask_wedge=None, mask_inner=None
 ):
 
     #SOME DEFINITIONS
     if fig is None:
-        fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(7, 7))
+        fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
 
     X = np.nan_to_num(X.to('au').value)
     Y = np.nan_to_num(Y.to('au').value)
     Rout = Rout.to('au').value
         
     xlim_rec = 1.15*Rout
-    fill_angs_2pi = np.linspace(0, 2*np.pi, 100)
     
     cmap_c = copy.copy(cmap)
     cmap_c.set_under('0.4')
     cmap_c.set_over('0.4')
-
-    def make_text_2D(ax, Rlist, posx=0.0, sposy=-1, fmt='%d', va=None, **kwargs_text):
-        if va is not None:
-            _va = va
-            dy = 0
-        else:
-            if sposy<0:
-                _va = 'top'
-                dy = 2
-            elif sposy>0:
-                _va = 'bottom'
-                dy = -1
-            else:
-                return 0
-
-        kwargs = dict(fontsize=SMALL_SIZE+3, ha='center', va=_va, weight='bold', rotation=0)
-        kwargs.update(kwargs_text)
-        for Ri in Rlist:
-            ax.text(posx, sposy*(Ri+dy), fmt%Ri, **kwargs)
     
     #MAIN PLOT
     im = ax.contourf(X, Y, map2d, levels=levels, cmap=cmap_c, extend='both', origin='lower')
-    make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks, twodim=True)
-            
-    #RADIAL GRID
-    ax.plot(Rout*np.cos(fill_angs_2pi), Rout*np.sin(fill_angs_2pi), color='k', ls='-', lw=5.0, alpha=0.9) #Radial border 
+    make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks, twodim=True, make_labels=False)
 
-    get_intdigits = lambda n: len(str(n).split('.')[0])
-
-    R_subst = np.concatenate([gaps, rings, kinks], axis=None)
-    if len(R_subst)>0:
-        Rref = np.max(R_subst)
-    else:
-        Rref = 0.0
-    Rref_digits = get_intdigits(Rref)        
-        
-    R_after_ref = 10**(Rref_digits-1)*ceil(Rref/(10**(Rref_digits-1)))
-    Rgrid_polar = np.arange(R_after_ref, Rout, 50)
+    #RADIAL GRID
+    _make_radial_grid_2D(ax, Rout, gaps=gaps, rings=rings, kinks=kinks, label_freq=2)
     
-    for j,Ri in enumerate(Rgrid_polar[0:-1:2]):
-        if Ri == Rref: continue
-        ax.plot(Ri*np.cos(fill_angs_2pi), Ri*np.sin(fill_angs_2pi), color='k', lw=1.2, alpha=0.5, dash_capstyle='round', dashes=(0.5, 3.5)) #will be labeled
-
-    for j,Ri in enumerate(Rgrid_polar[1::2]):
-        ax.plot(Ri*np.cos(fill_angs_2pi), Ri*np.sin(fill_angs_2pi), color='k', ls=':', lw=0.4, alpha=1.0)
-
     #AZIMUTHAL GRID
-    for j,phii in enumerate(np.arange(0, 2*np.pi, np.pi/6)):
-        ax.plot([0, Rout*np.cos(phii)], [0, Rout*np.sin(phii)], color='k', ls=':', lw=0.4, alpha=1.0)
-
-    for deg in np.linspace(0, 90, 4):
-        deg_rad = np.radians(deg)
-        txt = ax.text(1.04*Rout*np.cos(deg_rad), 1.04*Rout*np.sin(deg_rad), r'$%d$'%deg, c='0.0',
-                      fontsize=SMALL_SIZE-2, ha='center', va='center', weight='bold', rotation=-(90-deg)) #rotation_mode='anchor', 
-        txt.set_text(r'$%d^{\circ}$'%deg)
+    _make_azimuthal_grid_2D(ax, Rout)
     
     #SKY AXIS
     if np.all(np.asarray([z_func, z_pars, incl, PA])!=None):
-        from .grid import GridTools
-        ynorth = np.linspace(-1.1*Rout, 1.1*Rout, 100)
-        xnorth = np.zeros_like(ynorth)
-        xn, yn = [], []
-        for i in range(len(ynorth)):
-            xni, yni = GridTools.get_disc_from_sky_coords(xnorth[i], ynorth[i], z_func, z_pars, incl, PA, xc=0, yc=0)
-            xn.append(xni)
-            yn.append(yni)
-            #plt.scatter(xn, yn, c='k', s=5)
-        xn, yn = np.asarray(xn), np.asarray(yn)
-        ax.plot(xn, yn, color='0.0', lw=1.7, dash_capstyle='round', dashes=(1.5, 2.5))
-
-        #MAKE TEXT Nsky
-        text_nsky = lambda x, y: ax.text(x, y, r'$\vec{\rm N}$$_{\rm sky}$', fontsize=SMALL_SIZE+3,
-                                         ha='center', va='bottom', weight='bold', rotation=np.degrees(-PA))
-        
-        if yni>xni:
-            ci = yni
-            cn = yn
-        else:
-            ci = xni
-            cn = xn
-
-        if ci>xlim_rec:
-            ii = np.argmin(np.abs(cn-xlim_rec))
-            text_nsky(xn[ii], yn[ii])
-        else:
-            text_nsky(xni, yni)
+        xni, yni = _make_nsky_2D(ax, Rout, xlim_rec,
+                                 z_func, z_pars, incl, PA, xc=xc, yc=yc)
     else:
         xni, yni = None, None
         
-    #MAKE TEXT FOR SUBSTRUCTURES AND RADIAL GRID
+    #SUBSTRUCTURE LABELS
     if label_gaps:
-        make_text_2D(ax, gaps, fmt='D%d')
+        _make_text_2D(ax, gaps, sposy=-1, fmt='D%d')
     if label_rings:
-        make_text_2D(ax, rings, fmt='B%d')
+        _make_text_2D(ax, rings, sposy=-1, fmt='B%d')
     if label_kinks:
-        make_text_2D(ax, kinks, fmt='K%d')
-
-    make_text_2D(ax, Rgrid_polar[2:-1:2], sposy=-1, fmt='%d', fontsize=SMALL_SIZE+3, color='0.1', va='center') #label every other radius, in the north
-    make_text_2D(ax, Rgrid_polar[2:-1:2], sposy=1, fmt='%d', fontsize=SMALL_SIZE+3, color='0.1', va='center') # and south
+        _make_text_2D(ax, kinks, sposy=-1, fmt='K%d')
 
     #SET LIMITS AND AXES
     for side in ['left','top','right']: ax.spines[side].set_visible(False)
     make_up_ax(ax,
                xlims=(-xlim_rec, xlim_rec),
                ylims=(-xlim_rec, xlim_rec),
                labelleft=False, left=False, right=False, labeltop=False, top=False, labelbottom=True, bottom=True,
@@ -451,15 +480,15 @@
         if xni is None:
             quadrant = 2
         elif (yni>0 and xni<0) or (yni<0 and xni>0):
             quadrant = 3
         else:
             quadrant = 2
             
-    make_round_cbar(ax, Rout, levels, cmap=cmap_c, unit=unit, fmt=fmt, quadrant=quadrant)
+    make_round_cbar(ax, Rout, levels, cmap=cmap_c, clabel=clabel, fmt=fmt, quadrant=quadrant)
 
     sq = {1: -1,
           2: 1,
           3: 1,
           4: -1,
     }[quadrant]
         
@@ -477,15 +506,16 @@
         
     return fig, ax
         
 def make_polar_map(
         map2d, levels, R, PHI, Rout,
         Rin = 0.0,
         fig=None, ax=None, 
-        cmap=get_discminer_cmap('velocity'), unit='km/s', fmt='%5.2f', clabel=r'$\Delta$ Centroid Velocity [km s$^{-1}$]', #cbar kwargs 
+        cmap=get_discminer_cmap('velocity'),
+        fmt='%5.2f', clabel=None, 
         gaps=[], rings=[], kinks=[] #,filaments=[],                            
 ):
     from scipy.interpolate import griddata
 
     #SOME DEFINITIONS
     if fig is None:
         fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(12, 3))
@@ -540,15 +570,15 @@
     cax = add_cbar_ax(fig, ax, orientation='vertical', subplots=False, perc=6)    
     cbar = plt.colorbar(im, cax=cax, format=fmt, orientation='vertical', ticks=np.linspace(levels.min(), levels.max(), 5))
     cbar.ax.tick_params(which='major', direction='in', width=2.7, size=4.8, pad=4, labelsize=SMALL_SIZE)
     cbar.ax.tick_params(which='minor', direction='in', width=2.7, size=3.3)
     cbar.set_label(clabel, fontsize=SMALL_SIZE, labelpad=20, rotation=270)
     mod_minor_ticks(cbar.ax)
 
-    return fig, ax
+    return fig, ax, cbar
 
 #***************************
 #PEAK RESIDUALS AND CLUSTERS
 #***************************
 def append_sigma_panel(fig, ax, values, ax_std=None, weights=None, hist=False, fit_gauss_hist=False): #attach sigma panel to AxesSubplot, based on input values
     ax = np.atleast_1d(ax)
```

### Comparing `discminer-0.1.0/discminer/rail.py` & `discminer-0.1.1/discminer/rail.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,21 +139,28 @@
         coord_list, lev_list, resid_list, color_list = [], [], [], []
         if np.sum(coord_levels==coord_ref)==0 and coord_ref is not None: coord_levels = np.append(coord_levels, coord_ref)
         for lev in coord_levels:
             contour = measure.find_contours(coords[0], lev) #, fully_connected='high', positive_orientation='high')
             if len(contour)==0:
                 print ('no contours found for phi =', lev)
                 continue
-            ind_good = np.argmin([np.abs(lev-coords[0][tuple(np.round(contour[i][0]).astype(np.int))]) for i in range(len(contour))]) #getting ind of closest contour to lev
+            ind_good = np.argmin([np.abs(lev-coords[0][tuple(np.round(contour[i][0]).astype(np.int))]) for i in range(len(contour))]) #get contour id closest to lev
             inds_cont = np.round(contour[ind_good]).astype(np.int)
             inds_cont = [tuple(f) for f in inds_cont]
             first_cont = np.array([coords[0][i] for i in inds_cont])
             second_cont = np.array([coords[1][i] for i in inds_cont])
             prop_cont = np.array([prop[i] for i in inds_cont])
-            corr_inds = np.abs(first_cont-lev) < acc_threshold
+
+            corr_inds = np.abs(first_cont-lev) < acc_threshold #clean based on acc_threshold
+            
+            _, tmp = np.unique(second_cont, return_index=True) 
+            unique_inds = np.zeros_like(second_cont).astype(bool)
+            unique_inds[tmp] = True
+            corr_inds = corr_inds & unique_inds #make sure points are not repeated
+
             if lev == coord_ref: zorder=10
             else: zorder=np.random.randint(0,10)
 
             for i,bound in enumerate(color_bounds):
                 if lev == coord_ref: 
                     lw = 2.0
                     color = 'k'
```

### Comparing `discminer-0.1.0/discminer/testyapf.py` & `discminer-0.1.1/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/tools/discminer.mplstyle` & `discminer-0.1.1/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/tools/fit_kernel.py` & `discminer-0.1.1/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer/tools/utils.py` & `discminer-0.1.1/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/discminer.egg-info/PKG-INFO` & `discminer-0.1.1/discminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.1.0 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.1.1 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.1.0/discminer.egg-info/SOURCES.txt` & `discminer-0.1.1/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/setup.py` & `discminer-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/template/README.rst` & `discminer-0.1.1/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/template/download_MAPS.sh` & `discminer-0.1.1/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.1.1/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.1.0/template/prepare_data.py` & `discminer-0.1.1/template/prepare_data.py`

 * *Files identical despite different names*

