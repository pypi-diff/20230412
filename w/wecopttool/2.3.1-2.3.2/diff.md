# Comparing `tmp/wecopttool-2.3.1.tar.gz` & `tmp/wecopttool-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wecopttool-2.3.1.tar", last modified: Tue Apr  4 19:47:56 2023, max compression
+gzip compressed data, was "wecopttool-2.3.2.tar", last modified: Wed Apr 12 17:16:57 2023, max compression
```

## Comparing `wecopttool-2.3.1.tar` & `wecopttool-2.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:47:56.343876 wecopttool-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-04 19:47:42.000000 wecopttool-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-04 19:47:42.000000 wecopttool-2.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-04 19:47:56.343876 wecopttool-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-04 19:47:42.000000 wecopttool-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-04 19:47:42.000000 wecopttool-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:47:56.343876 wecopttool-2.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:47:56.339876 wecopttool-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    50582 2023-04-04 19:47:43.000000 wecopttool-2.3.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-04 19:47:43.000000 wecopttool-2.3.1/tests/test_hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-04 19:47:43.000000 wecopttool-2.3.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-04 19:47:43.000000 wecopttool-2.3.1/tests/test_pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-04-04 19:47:43.000000 wecopttool-2.3.1/tests/test_waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:47:56.343876 wecopttool-2.3.1/wecopttool/
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-04 19:47:43.000000 wecopttool-2.3.1/wecopttool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82645 2023-04-04 19:47:43.000000 wecopttool-2.3.1/wecopttool/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-04 19:47:43.000000 wecopttool-2.3.1/wecopttool/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-04 19:47:43.000000 wecopttool-2.3.1/wecopttool/hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33435 2023-04-04 19:47:43.000000 wecopttool-2.3.1/wecopttool/pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-04-04 19:47:43.000000 wecopttool-2.3.1/wecopttool/waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:47:56.343876 wecopttool-2.3.1/wecopttool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-04 19:47:56.000000 wecopttool-2.3.1/wecopttool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-04 19:47:56.000000 wecopttool-2.3.1/wecopttool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:47:56.000000 wecopttool-2.3.1/wecopttool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-04 19:47:56.000000 wecopttool-2.3.1/wecopttool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 19:47:56.000000 wecopttool-2.3.1/wecopttool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.304774 wecopttool-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 17:16:45.000000 wecopttool-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-12 17:16:45.000000 wecopttool-2.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-12 17:16:57.304774 wecopttool-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 17:16:45.000000 wecopttool-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-12 17:16:45.000000 wecopttool-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:16:57.304774 wecopttool-2.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.300774 wecopttool-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    50582 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.300774 wecopttool-2.3.2/wecopttool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82645 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33435 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.304774 wecopttool-2.3.2/wecopttool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/top_level.txt
```

### Comparing `wecopttool-2.3.1/LICENSE` & `wecopttool-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/NOTICE` & `wecopttool-2.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/PKG-INFO` & `wecopttool-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.3.1
+Version: 2.3.2
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://snl-waterpower.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `wecopttool-2.3.1/README.md` & `wecopttool-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/pyproject.toml` & `wecopttool-2.3.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wecopttool"
-version = "2.3.1"
+version = "2.3.2"
 description = "WEC Design Optimization Toolbox"
 readme = "README.md"
 authors = [
     {name = "Sandia National Laboratories"},
 ]
 urls = {Documentation = "https://snl-waterpower.github.io/WecOptTool/"}
 requires-python = ">=3.8"
@@ -21,15 +21,15 @@
 dependencies = [
     "numpy>=1.20",
     "scipy",
     "xarray",
     "autograd",
     "capytaine",
     "joblib",
-    "wavespectra",
+    "wavespectra>=3.13",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "sphinx",
     "sphinxcontrib-bibtex",
```

### Comparing `wecopttool-2.3.1/tests/test_core.py` & `wecopttool-2.3.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/tests/test_hydrostatics.py` & `wecopttool-2.3.2/tests/test_hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/tests/test_integration.py` & `wecopttool-2.3.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/tests/test_pto.py` & `wecopttool-2.3.2/tests/test_pto.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/tests/test_waves.py` & `wecopttool-2.3.2/tests/test_waves.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         frequency and direction."""
         return wot.waves.elevation_fd(f1, nfreq, directions)
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega']
+        coordinates = ['wave_direction', 'omega', 'freq']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
     def test_shape(self, elevation, nfreq, ndir):
         """Test that the elevation dataArray has the correct shape."""
         assert np.squeeze(elevation.values).shape == (nfreq, ndir)
 
@@ -112,15 +112,15 @@
         frequency and direction."""
         return wot.waves.regular_wave(f1, nfreq, freq, amp, phase, dir)
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega']
+        coordinates = ['wave_direction', 'omega', 'freq']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
     def test_shape(self, elevation, nfreq, ndir):
         """Test that the elevation dataArray has the correct shape."""
         assert np.squeeze(elevation.values).shape == (nfreq, )
 
@@ -219,15 +219,15 @@
         )
         return efth_xr
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega']
+        coordinates = ['wave_direction', 'omega', 'freq']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
     def test_shape(self, elevation, nfreq, ndir):
         """Test that the elevation dataArray has the correct shape."""
         assert np.squeeze(elevation.values).shape == (nfreq, )
 
@@ -286,15 +286,15 @@
         frequency and direction."""
         return wot.waves.irregular_wave(ndbc_spectrum.efth)
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega']
+        coordinates = ['wave_direction', 'omega', 'freq']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
     def test_shape(self, ndbc_spectrum, elevation):
         """Test that the elevation dataArray has the correct shape."""
         nfreq = len(ndbc_spectrum.freq)
         ndir = len(ndbc_spectrum.dir)
```

### Comparing `wecopttool-2.3.1/wecopttool/__init__.py` & `wecopttool-2.3.2/wecopttool/__init__.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/wecopttool/core.py` & `wecopttool-2.3.2/wecopttool/core.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/wecopttool/geom.py` & `wecopttool-2.3.2/wecopttool/geom.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/wecopttool/hydrostatics.py` & `wecopttool-2.3.2/wecopttool/hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/wecopttool/pto.py` & `wecopttool-2.3.2/wecopttool/pto.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.1/wecopttool/waves.py` & `wecopttool-2.3.2/wecopttool/waves.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,20 @@
     """
     directions = np.atleast_1d(degrees_to_radians(directions, sort=False))
     ndirections = len(directions)
     freq = frequency(f1, nfreq, False)
     omega = freq*2*np.pi
 
     dims = ('omega', 'wave_direction')
-    freq_attr = {'long_name': 'Wave frequency', 'units': 'rad/s'}
+    omega_attr = {'long_name': 'Radial frequency', 'units': 'rad/s'}
+    freq_attr = {'long_name': 'Frequency', 'units': 'Hz'}
     dir_attr = {'long_name': 'Wave direction', 'units': 'rad'}
-    coords = [(dims[0], omega, freq_attr), (dims[1], directions, dir_attr)]
+    coords = {'omega': (dims[0], omega, omega_attr),
+              'freq': (dims[0], freq, freq_attr),
+              'wave_direction': (dims[1], directions, dir_attr)}
 
     if amplitudes is None:
         amplitudes = np.zeros([nfreq, ndirections])
 
     if phases is None:
         phases = random_phase([nfreq, ndirections])
     else:
```

### Comparing `wecopttool-2.3.1/wecopttool.egg-info/PKG-INFO` & `wecopttool-2.3.2/wecopttool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.3.1
+Version: 2.3.2
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://snl-waterpower.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

