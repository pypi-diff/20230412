# Comparing `tmp/LFPykit-0.5.1.tar.gz` & `tmp/LFPykit-0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LFPykit-0.5.1.tar", last modified: Wed Apr 12 07:10:51 2023, max compression
+gzip compressed data, was "LFPykit-0.5rc0.tar", last modified: Wed Dec 14 23:06:50 2022, max compression
```

## Comparing `LFPykit-0.5.1.tar` & `LFPykit-0.5rc0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:10:51.646725 LFPykit-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:10:51.638725 LFPykit-0.5.1/LFPykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-04-12 07:10:51.000000 LFPykit-0.5.1/LFPykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 07:10:51.000000 LFPykit-0.5.1/LFPykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:10:51.000000 LFPykit-0.5.1/LFPykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:10:45.000000 LFPykit-0.5.1/LFPykit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-12 07:10:51.000000 LFPykit-0.5.1/LFPykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 07:10:51.000000 LFPykit-0.5.1/LFPykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 07:10:37.000000 LFPykit-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 07:10:37.000000 LFPykit-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-04-12 07:10:51.646725 LFPykit-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-04-12 07:10:37.000000 LFPykit-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:10:51.638725 LFPykit-0.5.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:10:51.638725 LFPykit-0.5.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-12 07:10:37.000000 LFPykit-0.5.1/doc/source/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 07:10:37.000000 LFPykit-0.5.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 07:10:37.000000 LFPykit-0.5.1/doc/source/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-12 07:10:37.000000 LFPykit-0.5.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 07:10:37.000000 LFPykit-0.5.1/doc/source/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 07:10:37.000000 LFPykit-0.5.1/doc/source/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:10:51.646725 LFPykit-0.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   199748 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_Arbor.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   111528 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_Arbor_swc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   533087 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_EEG_NYHead.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   243354 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_LFPy.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   140581 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_LFPy_MEG.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   301874 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_LFPy_compare_forwardmodels.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   272429 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_LFPy_pt3d.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   137819 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_LFPy_swc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   247814 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_NEURON.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   106541 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_Neuron_swc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1279544 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/Example_SphericallySymmetricVolCondMEG_vs_InfiniteHomogeneousVolCondMEG.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   136918 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/L5_Mainen96_LFPy.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   385595 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/LFPykit_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 07:10:37.000000 LFPykit-0.5.1/examples/sinsyn.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:10:51.646725 LFPykit-0.5.1/lfpykit/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/cellgeometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    58491 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/eegmegcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/lfpcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83990 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:10:51.646725 LFPykit-0.5.1/lfpykit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/tests/fem_mix_dip.npz
--rw-r--r--   0 runner    (1001) docker     (123)    40337 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/tests/test_eegmegcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/tests/test_lfpcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34196 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 07:10:37.000000 LFPykit-0.5.1/lfpykit/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 07:10:51.646725 LFPykit-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-12 07:10:37.000000 LFPykit-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 23:06:50.451153 LFPykit-0.5rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 23:06:50.439153 LFPykit-0.5rc0/LFPykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14946 2022-12-14 23:06:50.000000 LFPykit-0.5rc0/LFPykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-14 23:06:50.000000 LFPykit-0.5rc0/LFPykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 23:06:50.000000 LFPykit-0.5rc0/LFPykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 23:06:44.000000 LFPykit-0.5rc0/LFPykit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-14 23:06:50.000000 LFPykit-0.5rc0/LFPykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-14 23:06:50.000000 LFPykit-0.5rc0/LFPykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14946 2022-12-14 23:06:50.451153 LFPykit-0.5rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 23:06:50.435153 LFPykit-0.5rc0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 23:06:50.439153 LFPykit-0.5rc0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/doc/source/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/doc/source/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/doc/source/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/doc/source/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 23:06:50.447153 LFPykit-0.5rc0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   199748 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_Arbor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   111528 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_Arbor_swc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   533087 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_EEG_NYHead.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   243354 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_LFPy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   140581 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_LFPy_MEG.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   301874 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_LFPy_compare_forwardmodels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   272429 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_LFPy_pt3d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   137819 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_LFPy_swc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   247814 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_NEURON.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   106541 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_Neuron_swc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1279544 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/Example_SphericallySymmetricVolCondMEG_vs_InfiniteHomogeneousVolCondMEG.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   136918 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/L5_Mainen96_LFPy.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)   385595 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/LFPykit_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/examples/sinsyn.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 23:06:50.447153 LFPykit-0.5rc0/lfpykit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/cellgeometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58148 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/eegmegcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/lfpcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83990 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 23:06:50.451153 LFPykit-0.5rc0/lfpykit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/tests/fem_mix_dip.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    40337 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/tests/test_eegmegcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23248 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/tests/test_lfpcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34196 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/lfpykit/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-14 23:06:50.451153 LFPykit-0.5rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-14 23:06:28.000000 LFPykit-0.5rc0/setup.py
```

### Comparing `LFPykit-0.5.1/LFPykit.egg-info/PKG-INFO` & `LFPykit-0.5rc0/LFPykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LFPykit
-Version: 0.5.1
+Version: 0.5rc0
 Summary: Electrostatic models for multicompartment neuron models
 Home-page: https://github.com/LFPy/LFPykit
 Author: LFPy-team
 Author-email: lfpy@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LFPykit-0.5.1/LFPykit.egg-info/SOURCES.txt` & `LFPykit-0.5rc0/LFPykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/LICENSE` & `LFPykit-0.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/PKG-INFO` & `LFPykit-0.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LFPykit
-Version: 0.5.1
+Version: 0.5rc0
 Summary: Electrostatic models for multicompartment neuron models
 Home-page: https://github.com/LFPy/LFPykit
 Author: LFPy-team
 Author-email: lfpy@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LFPykit-0.5.1/README.md` & `LFPykit-0.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/doc/source/Makefile` & `LFPykit-0.5rc0/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/doc/source/conf.py` & `LFPykit-0.5rc0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/doc/source/index.rst` & `LFPykit-0.5rc0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/doc/source/make.bat` & `LFPykit-0.5rc0/doc/source/make.bat`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_Arbor.ipynb` & `LFPykit-0.5rc0/examples/Example_Arbor.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_Arbor_swc.ipynb` & `LFPykit-0.5rc0/examples/Example_Arbor_swc.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_EEG_NYHead.ipynb` & `LFPykit-0.5rc0/examples/Example_EEG_NYHead.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_LFPy.ipynb` & `LFPykit-0.5rc0/examples/Example_LFPy.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_LFPy_MEG.ipynb` & `LFPykit-0.5rc0/examples/Example_LFPy_MEG.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_LFPy_compare_forwardmodels.ipynb` & `LFPykit-0.5rc0/examples/Example_LFPy_compare_forwardmodels.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_LFPy_pt3d.ipynb` & `LFPykit-0.5rc0/examples/Example_LFPy_pt3d.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_LFPy_swc.ipynb` & `LFPykit-0.5rc0/examples/Example_LFPy_swc.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_NEURON.ipynb` & `LFPykit-0.5rc0/examples/Example_NEURON.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_Neuron_swc.ipynb` & `LFPykit-0.5rc0/examples/Example_Neuron_swc.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/Example_SphericallySymmetricVolCondMEG_vs_InfiniteHomogeneousVolCondMEG.ipynb` & `LFPykit-0.5rc0/examples/Example_SphericallySymmetricVolCondMEG_vs_InfiniteHomogeneousVolCondMEG.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/L5_Mainen96_LFPy.hoc` & `LFPykit-0.5rc0/examples/L5_Mainen96_LFPy.hoc`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/LFPykit_demo.ipynb` & `LFPykit-0.5rc0/examples/LFPykit_demo.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/examples/sinsyn.mod` & `LFPykit-0.5rc0/examples/sinsyn.mod`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/__init__.py` & `LFPykit-0.5rc0/lfpykit/__init__.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/cellgeometry.py` & `LFPykit-0.5rc0/lfpykit/cellgeometry.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/eegmegcalc.py` & `LFPykit-0.5rc0/lfpykit/eegmegcalc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1402,39 +1402,30 @@
             raise ImportError("The package h5py was not found. "
                               "It is needed for loading New York Head model.")
 
         if nyhead_file is None:
             nyhead_file = os.path.join(os.getcwd(), "sa_nyhead.mat")
         self.head_file = os.path.abspath(nyhead_file)
         if not os.path.isfile(self.head_file):
-
-            print(f"New York head model file not found: {self.head_file}")
-            print(f"Now downloading as {self.head_file} (710 MB). "
-                  + "This might take a while ...")
-            import urllib
             from urllib.request import urlopen
             import ssl
-            try:
+            print("New York head-model file not found: %s" % self.head_file)
+            yn = input(f"Download as {self.head_file} (710 MB)? [y/n]: ")
+            if yn == 'y':
+                print("Now downloading. This might take a while ...")
                 nyhead_url = 'https://www.parralab.org/nyhead/sa_nyhead.mat'
                 u = urlopen(nyhead_url,
                             context=ssl._create_unverified_context())
                 localFile = open(self.head_file, 'wb')
                 localFile.write(u.read())
                 localFile.close()
                 print("Download done!")
-            except urllib.error.URLError:
-                print("URLError: Is the internet connection working?")
-                raise
-            except PermissionError:
-                print("PermissionError: Write access is needed "
-                      + "for downloading head model.")
-                raise
-            except Exception:
-                print("Unable to find or download New York head model file")
-                raise
+            else:
+                print("Exiting program ...")
+                sys.exit()
 
         self.head_data = h5py.File(self.head_file, 'r')["sa"]
         self.cortex = np.array(self.head_data["cortex75K"]["vc"])
         self.lead_field = np.array(self.head_data["cortex75K"]["V_fem"])
         self.lead_field_normal = np.array(
             self.head_data["cortex75K"]["V_fem_normal"])
         self.cortex_normals = np.array(self.head_data["cortex75K"]["normals"])
```

### Comparing `LFPykit-0.5.1/lfpykit/lfpcalc.py` & `LFPykit-0.5rc0/lfpykit/lfpcalc.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/models.py` & `LFPykit-0.5rc0/lfpykit/models.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/tests/fem_mix_dip.npz` & `LFPykit-0.5rc0/lfpykit/tests/fem_mix_dip.npz`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/tests/test_eegmegcalc.py` & `LFPykit-0.5rc0/lfpykit/tests/test_eegmegcalc.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/tests/test_lfpcalc.py` & `LFPykit-0.5rc0/lfpykit/tests/test_lfpcalc.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/lfpykit/tests/test_module.py` & `LFPykit-0.5rc0/lfpykit/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `LFPykit-0.5.1/setup.py` & `LFPykit-0.5rc0/setup.py`

 * *Files identical despite different names*

