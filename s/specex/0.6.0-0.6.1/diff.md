# Comparing `tmp/specex-0.6.0.tar.gz` & `tmp/specex-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specex-0.6.0.tar", last modified: Fri Apr  7 11:00:50 2023, max compression
+gzip compressed data, was "specex-0.6.1.tar", last modified: Wed Apr 12 15:11:06 2023, max compression
```

## Comparing `specex-0.6.0.tar` & `specex-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-07 11:00:50.568760 specex-0.6.0/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2022-04-01 11:26:21.000000 specex-0.6.0/LICENSE
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3919 2023-04-07 11:00:50.568760 specex-0.6.0/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1407 2022-12-16 07:04:36.000000 specex-0.6.0/README.md
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1635 2023-02-12 09:24:28.000000 specex-0.6.0/pyproject.toml
--rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2023-04-07 11:00:50.568760 specex-0.6.0/setup.cfg
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-07 11:00:50.565426 specex-0.6.0/src/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-07 11:00:50.565426 specex-0.6.0/src/specex/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1918 2023-03-06 07:50:03.000000 specex-0.6.0/src/specex/__init__.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    53480 2023-02-13 13:15:40.000000 specex-0.6.0/src/specex/cube.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     5175 2022-12-15 19:17:38.000000 specex-0.6.0/src/specex/lines.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    12965 2023-02-21 15:30:58.000000 specex-0.6.0/src/specex/plot.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    20267 2022-12-15 19:17:38.000000 specex-0.6.0/src/specex/rrspecex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    24593 2022-12-15 19:17:38.000000 specex-0.6.0/src/specex/sources.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    42648 2023-03-06 07:49:53.000000 specex-0.6.0/src/specex/specex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     8345 2023-02-14 07:35:23.000000 specex-0.6.0/src/specex/stack.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    38123 2023-02-14 07:38:24.000000 specex-0.6.0/src/specex/utils.py
--rwxr-xr-x   0 daddona   (1000) daddona   (1000)     4550 2022-12-15 19:17:38.000000 specex-0.6.0/src/specex/zeropoints.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-07 11:00:50.565426 specex-0.6.0/src/specex.egg-info/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3919 2023-04-07 11:00:50.000000 specex-0.6.0/src/specex.egg-info/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)      607 2023-04-07 11:00:50.000000 specex-0.6.0/src/specex.egg-info/SOURCES.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2023-04-07 11:00:50.000000 specex-0.6.0/src/specex.egg-info/dependency_links.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)      287 2023-04-07 11:00:50.000000 specex-0.6.0/src/specex.egg-info/entry_points.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)       46 2023-04-07 11:00:50.000000 specex-0.6.0/src/specex.egg-info/requires.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        7 2023-04-07 11:00:50.000000 specex-0.6.0/src/specex.egg-info/top_level.txt
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-07 11:00:50.568760 specex-0.6.0/test/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2022-12-15 19:17:38.000000 specex-0.6.0/test/test_cubestack.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1970 2022-12-15 19:17:38.000000 specex-0.6.0/test/test_cutout.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1524 2022-12-15 19:17:38.000000 specex-0.6.0/test/test_rrspecex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      583 2022-12-15 19:17:38.000000 specex-0.6.0/test/test_sources.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1133 2022-12-15 19:17:38.000000 specex-0.6.0/test/test_specex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      706 2022-12-15 19:17:38.000000 specex-0.6.0/test/test_specexplot.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      756 2022-12-15 19:17:38.000000 specex-0.6.0/test/test_zeropointinfo.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2022-04-01 11:26:21.000000 specex-0.6.1/LICENSE
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4025 2023-04-12 15:11:06.738803 specex-0.6.1/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1513 2023-04-07 11:12:08.000000 specex-0.6.1/README.md
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1635 2023-04-12 13:06:36.000000 specex-0.6.1/pyproject.toml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2023-04-12 15:11:06.738803 specex-0.6.1/setup.cfg
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.735470 specex-0.6.1/src/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/src/specex/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1918 2023-03-06 07:50:03.000000 specex-0.6.1/src/specex/__init__.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    53746 2023-04-12 13:12:36.000000 specex-0.6.1/src/specex/cube.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     5175 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/lines.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    13737 2023-04-12 13:18:00.000000 specex-0.6.1/src/specex/plot.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    20267 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/rrspecex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    24593 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/sources.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    42648 2023-03-06 07:49:53.000000 specex-0.6.1/src/specex/specex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     8345 2023-02-14 07:35:23.000000 specex-0.6.1/src/specex/stack.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    38211 2023-04-12 15:03:32.000000 specex-0.6.1/src/specex/utils.py
+-rwxr-xr-x   0 daddona   (1000) daddona   (1000)     4550 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/zeropoints.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/src/specex.egg-info/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4025 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      607 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/SOURCES.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/dependency_links.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      287 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/entry_points.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       46 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/requires.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        7 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/top_level.txt
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/test/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_cubestack.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1970 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_cutout.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1524 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_rrspecex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      583 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_sources.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1133 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_specex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      706 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_specexplot.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      756 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_zeropointinfo.py
```

### Comparing `specex-0.6.0/LICENSE` & `specex-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/PKG-INFO` & `specex-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specex
-Version: 0.6.0
+Version: 0.6.1
 Summary: Extract spectra from fits cubes
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
         
@@ -44,15 +44,15 @@
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# python-specex [![Build Status](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml/badge.svg)](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml) [![Documentation Status](https://readthedocs.org/projects/python-specex/badge/?version=latest)](https://python-specex.readthedocs.io/en/latest/?badge=latest)
+# python-specex [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7808292.svg)](https://doi.org/10.5281/zenodo.7808292) [![Build Status](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml/badge.svg)](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml) [![Documentation Status](https://readthedocs.org/projects/python-specex/badge/?version=latest)](https://python-specex.readthedocs.io/en/latest/?badge=latest)
 
 Extract spectra from fits cubes
 
 # SETUP
 
 To install the latest stable version of specex, just use pip:
```

### Comparing `specex-0.6.0/README.md` & `specex-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# python-specex [![Build Status](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml/badge.svg)](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml) [![Documentation Status](https://readthedocs.org/projects/python-specex/badge/?version=latest)](https://python-specex.readthedocs.io/en/latest/?badge=latest)
+# python-specex [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7808292.svg)](https://doi.org/10.5281/zenodo.7808292) [![Build Status](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml/badge.svg)](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml) [![Documentation Status](https://readthedocs.org/projects/python-specex/badge/?version=latest)](https://python-specex.readthedocs.io/en/latest/?badge=latest)
 
 Extract spectra from fits cubes
 
 # SETUP
 
 To install the latest stable version of specex, just use pip:
```

### Comparing `specex-0.6.0/pyproject.toml` & `specex-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "specex"
-version = "0.6.0"
+version = "0.6.1"
 description = "Extract spectra from fits cubes"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["spectroscopy", "spectra", "spectrum", "spectral cubes"]
 authors = [
  {name = "Maurizio D'Addona"},
```

### Comparing `specex-0.6.0/src/specex/__init__.py` & `specex-0.6.1/src/specex/__init__.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/src/specex/cube.py` & `specex-0.6.1/src/specex/cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,14 +443,15 @@
 
     return cutout_dict
 
 
 def get_rgb_cutout(data: Union[tuple, list, np.ndarray],
                    center: Union[SkyCoord, tuple],
                    size: Union[tuple, list],
+                   angle: Optional[Union[float, units.Quantity]] = 0,
                    data_wcs: Optional[Union[WCS, list, tuple]] = None,
                    resample_to_wcs: bool = False):
     """
     Get a cutout from a bigger RGB.
 
     Parameters
     ----------
@@ -464,14 +465,17 @@
         case, if no WCS is specified, the values are assumed to be in pixels,
         else if a WCS is provided then the values are assumed to be in degrees.
     size : tuple
         The first two values in the tuple are interpreted as the width and
         height of the cutout. if no WCS is specified, the values are assumed to
         be in pixels, else if a WCS is provided then the values are assumed to
         be in degrees. Astropy.units.Quantity values are also supported.
+    angle : float or astropy.units.Quantity, optional
+        The rotation angle of the cutout. If it is a float, then it is
+        interpreted in degrees. The default is 0.
     data_wcs : astropy.wcs.WCS or None, optional
         A WCS associated with the image data. The default is None.
     reample_to_wcs : bool, optional
         If true reample the red, green and blue data to share the same WCS.
         In order to use this option, the WCSs for the input data must be
         provided, otherwise this option will be ignored and a warning message
         is outputed. The default is False.
@@ -537,17 +541,17 @@
         data_g = data[1]
         data_b = data[2]
     else:
         raise ValueError(
             "Parameter 'data' only supports ndarray or list/tuple of ndarrays."
         )
 
-    cutout_data_r = get_gray_cutout(data_r, center, size, data_wcs_r)
-    cutout_data_g = get_gray_cutout(data_g, center, size, data_wcs_g)
-    cutout_data_b = get_gray_cutout(data_b, center, size, data_wcs_b)
+    cutout_data_r = get_gray_cutout(data_r, center, size, angle, data_wcs_r)
+    cutout_data_g = get_gray_cutout(data_g, center, size, angle, data_wcs_g)
+    cutout_data_b = get_gray_cutout(data_b, center, size, angle, data_wcs_b)
 
     if not resample_to_wcs:
         cutout_dict = {
             'data': (
                 cutout_data_r['data'],
                 cutout_data_g['data'],
                 cutout_data_b['data']
```

### Comparing `specex-0.6.0/src/specex/lines.py` & `specex-0.6.1/src/specex/lines.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/src/specex/plot.py` & `specex-0.6.1/src/specex/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,22 @@
         '--key-z', metavar='KEY_Z', type=str, default='Z',
         help='Set the name of the column in the zcat that contains the '
         'redshift the spectra. See --zcat for more info. If this option is not'
         ' specified, then he default value %(metavar)s = %(default)s is used.'
     )
 
     parser.add_argument(
+        '--key-wrange', metavar='WAVE_RANGE', type=str, default=None,
+        help='Set the name of the column in the zcat that contains the range'
+        'of wavelength to plot. If not specified then the whole spectrum is '
+        'plotted. If specified and the range value is empty no plot is '
+        'produced for the object.'
+    )
+
+    parser.add_argument(
         '--restframe', default=False, action='store_true',
         help='If this option is specified, spectra will be plotted as if they '
         'were in the observer restframe (ie. they are de-redshifted). '
         'In order to use this option, a zcat must be specified.'
     )
 
     parser.add_argument(
@@ -149,15 +157,14 @@
             sys.exit(1)
         elif args.key_z not in zcat.colnames:
             print(
                 f"ERROR: z catalog does not have z column '{args.key_z}'",
                 file=sys.stderr
             )
             sys.exit(1)
-        zcat = zcat[args.key_id, args.key_z].copy()
 
         # Remove objects with masked or undefined IDs
         if isinstance(zcat[args.key_id], MaskedColumn):
             zcat = zcat[~zcat[args.key_id].mask]
 
         zcat.add_index(args.key_id)
     else:
@@ -257,14 +264,15 @@
                 flux_units = None
 
             try:
                 wavelenght_units = spec_hdu.header['CUNIT1']
             except KeyError:
                 wavelenght_units = None
 
+            wave_range = None
             if zcat is not None:
                 try:
                     object_z = zcat.loc[object_id][args.key_z]
                 except KeyError:
                     print(
                         f"WARNING: '{object_id}' not in zcat, skipping...",
                         file=sys.stderr
@@ -273,14 +281,24 @@
                 else:
                     try:
                         # In case of repeated objects
                         object_z = object_z[0]
                     except IndexError:
                         # Otherwise just go ahead
                         pass
+
+                    if args.key_wrange is not None:
+                        str_wrange = zcat.loc[object_id][args.key_wrange]
+                        try:
+                            wave_range = [
+                                float(x) for x in str_wrange.split('-')
+                            ]
+                        except Exception:
+                            continue
+
                 restframe = args.restframe
                 info_dict['Z'] = object_z
             else:
                 # If no zcat is provided, check if redshift information is
                 # stored in the spectrum itself
                 if 'Z' in info_dict:
                     object_z = float(info_dict['Z'])
@@ -302,28 +320,28 @@
             pixel = np.arange(len(flux_data))
             wavelenghts = spec_wcs.pixel_to_world(pixel).Angstrom
 
             if big_image is not None:
                 if big_image['type'] == 'rgb':
                     cutout_dict = get_rgb_cutout(
                         big_image['data'],
-                        position=obj_center,
+                        center=obj_center,
                         size=cutout_size,
                         data_wcs=big_image['wcs']
                     )
-                    cutout = np.array(cutout_dict['data'])
+                    cutout = np.asarray(cutout_dict['data']).transpose(1, 2, 0)
                     cutout_wcs = cutout_dict['wcs'][0]
                 else:
                     cutout_dict = get_gray_cutout(
                         big_image['data'],
-                        position=obj_center,
+                        center=obj_center,
                         size=cutout_size,
                         data_wcs=big_image['wcs']
                     )
-                    cutout = cutout_dict['data'].transpose(1, 2, 0)
+                    cutout = np.array(cutout_dict['data'])
                     cutout_wcs = cutout_dict['wcs']
                 cutout_vmin = np.nanmin(big_image['data'])
                 cutout_vmax = np.nanmax(big_image['data'])
             else:
                 cutout = None
                 cutout_wcs = None
                 cutout_vmin = None
@@ -345,15 +363,16 @@
                 smoothing=args.smoothing,
                 extra_info=info_dict,
                 extraction_info={
                     'mode': extraction_mode,
                     'apertures': specex_apertures,
                     'aperture_ra': object_ra,
                     'aperture_dec': object_dec,
-                }
+                },
+                wave_range=wave_range
             )
 
             if args.outdir is None:
                 outdir = os.path.dirname(spectrum_fits_file)
             else:
                 outdir = args.outdir
                 if not os.path.isdir(outdir):
```

### Comparing `specex-0.6.0/src/specex/rrspecex.py` & `specex-0.6.1/src/specex/rrspecex.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/src/specex/sources.py` & `specex-0.6.1/src/specex/sources.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/src/specex/specex.py` & `specex-0.6.1/src/specex/specex.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/src/specex/stack.py` & `specex-0.6.1/src/specex/stack.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/src/specex/utils.py` & `specex-0.6.1/src/specex/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
     return ellipse_points
 
 
 def plot_spectrum(wavelengths, flux, variance=None, nan_mask=None,
                   restframe=False, cutout=None, cutout_vmin=None,
                   cutout_vmax=None, cutout_wcs=None, redshift=None,
                   smoothing=None, wavelengt_units=None, flux_units=None,
-                  extra_info={}, extraction_info={}):
+                  extra_info={}, extraction_info={}, wave_range=None):
     """
     Plot a spectrum.
 
     Parameters
     ----------
     wavelengths : numpy.ndarray 1D
         An array containing the wavelengths.
@@ -567,16 +567,20 @@
         if lam_mask is not None:
             lam_mask = lam_mask / (1 + redshift)
         lines_z = 0
     else:
         wavelengths = wavelengths
         lines_z = redshift
 
-    w_min = np.nanmin(wavelengths)
-    w_max = np.nanmax(wavelengths)
+    if wave_range is None:
+        w_min = np.nanmin(wavelengths)
+        w_max = np.nanmax(wavelengths)
+    else:
+        w_min = np.min(wave_range)
+        w_max = np.max(wave_range)
 
     if wavelengt_units:
         x_label = f'Wavelenght [{wavelengt_units}]'
     else:
         x_label = 'Wavelenght'
 
     if flux_units:
@@ -634,15 +638,16 @@
 
         ax1.axis('off')
         ax1.imshow(
             cutout,
             origin='lower',
             aspect='equal',
             vmin=cutout_vmin,
-            vmax=cutout_vmax
+            vmax=cutout_vmax,
+            zorder=0
         )
         ax1.set_aspect(1)
 
         # Check if there are info about the specex extraction
         try:
             ext_mode = extraction_info['mode']
             ext_apertures = extraction_info['apertures']
@@ -669,41 +674,40 @@
                     e_cc,
                     a=0.5*e_hei,
                     b=0.5*e_wid,
                     angle=e_ang
                 )
 
                 e_world_points_values = np.array([
-                    [x.ra.value, x.dec.value] for x in e_world_points
+                    [x.ra.value, x.dec.value]
+                    for x in e_world_points
                 ])
 
                 ax1.plot(
                     e_world_points_values[..., 0],
                     e_world_points_values[..., 1],
                     color='#0000ff',
                     ls='-',
                     lw=0.8,
                     alpha=0.7,
+                    zorder=1,
                     transform=ax1.get_transform(
-                        ax1.get_transform(
-                            apwcs.utils.wcs_to_celestial_frame(cutout_wcs)
-                        )
+                        apwcs.utils.wcs_to_celestial_frame(cutout_wcs)
                     )
                 )
                 ax1.plot(
                     e_world_points_values[..., 0],
                     e_world_points_values[..., 1],
                     color='#00ff00',
                     ls='--',
                     lw=0.8,
                     alpha=0.7,
+                    zorder=2,
                     transform=ax1.get_transform(
-                        ax1.get_transform(
-                            apwcs.utils.wcs_to_celestial_frame(cutout_wcs)
-                        )
+                        apwcs.utils.wcs_to_celestial_frame(cutout_wcs)
                     )
                 )
     else:
         ax1 = None
         ax2 = fig.add_subplot(gs[:, -1])
 
     ax0.set_aspect('auto')
```

### Comparing `specex-0.6.0/src/specex/zeropoints.py` & `specex-0.6.1/src/specex/zeropoints.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/src/specex.egg-info/PKG-INFO` & `specex-0.6.1/src/specex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specex
-Version: 0.6.0
+Version: 0.6.1
 Summary: Extract spectra from fits cubes
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
         
@@ -44,15 +44,15 @@
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# python-specex [![Build Status](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml/badge.svg)](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml) [![Documentation Status](https://readthedocs.org/projects/python-specex/badge/?version=latest)](https://python-specex.readthedocs.io/en/latest/?badge=latest)
+# python-specex [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7808292.svg)](https://doi.org/10.5281/zenodo.7808292) [![Build Status](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml/badge.svg)](https://github.com/mauritiusdadd/python-specex/actions/workflows/build-and-check.yml) [![Documentation Status](https://readthedocs.org/projects/python-specex/badge/?version=latest)](https://python-specex.readthedocs.io/en/latest/?badge=latest)
 
 Extract spectra from fits cubes
 
 # SETUP
 
 To install the latest stable version of specex, just use pip:
```

### Comparing `specex-0.6.0/src/specex.egg-info/SOURCES.txt` & `specex-0.6.1/src/specex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/test/test_cubestack.py` & `specex-0.6.1/test/test_cubestack.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/test/test_cutout.py` & `specex-0.6.1/test/test_cutout.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/test/test_rrspecex.py` & `specex-0.6.1/test/test_rrspecex.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/test/test_sources.py` & `specex-0.6.1/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/test/test_specex.py` & `specex-0.6.1/test/test_specex.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/test/test_specexplot.py` & `specex-0.6.1/test/test_specexplot.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.0/test/test_zeropointinfo.py` & `specex-0.6.1/test/test_zeropointinfo.py`

 * *Files identical despite different names*

