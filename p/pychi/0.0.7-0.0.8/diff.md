# Comparing `tmp/pychi-0.0.7.tar.gz` & `tmp/pychi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pychi-0.0.8.tar", last modified: Wed Apr 12 07:37:05 2023, max compression
```

## Comparing `pychi-0.0.7.tar` & `pychi-0.0.8.tar`

### file list

```diff
@@ -1,90 +1,19 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pychi-0.0.7/.gitattributes
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pychi-0.0.7/requirements.txt
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 pychi-0.0.7/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/Makefile
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/conf.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/make.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/modules.rst
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/pychi.rst
--rw-r--r--   0        0        0    81972 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0   115230 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/doctrees/pychi.doctree
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/index.html
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/modules.html
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0    38754 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/pychi.html
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/search.html
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_modules/index.html
--rw-r--r--   0        0        0    71792 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_modules/pychi/light.html
--rw-r--r--   0        0        0    57385 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_modules/pychi/materials.html
--rw-r--r--   0        0        0    77942 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_modules/pychi/models.html
--rw-r--r--   0        0        0    65241 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_modules/pychi/solvers.html
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_sources/pychi.rst.txt
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0   280364 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/jquery-3.4.1.js
--rw-r--r--   0        0        0    88145 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/jquery.js
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0    35168 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0        0        0    12140 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/underscore.js
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   129674 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 pychi-0.0.7/docs/_build/html/_static/js/theme.js
--rw-r--r--   0        0        0    33392 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/effective_index.npy
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/pychi_example.py
--rw-r--r--   0        0        0   249807 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/Cascaded Nonlinearities/cascaded.png
--rw-r--r--   0        0        0    33392 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/Cascaded Nonlinearities/effective_index.npy
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/Cascaded Nonlinearities/pychi_cascaded.py
--rw-r--r--   0        0        0    38967 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/LiNb/Experimental_vs_simulation_LiNb.png
--rw-r--r--   0        0        0    56592 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/LiNb/exp_LiNb.mat
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/LiNb/n_eff_data_LiNb.npy
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/LiNb/pychi_LiNb_exp_vs_sim.py
--rw-r--r--   0        0        0   161229 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/SPM/frequency_propagation.png
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/SPM/pychi_spm_validation.py
--rw-r--r--   0        0        0    78343 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/SPM/time_propagation.png
--rw-r--r--   0        0        0    41292 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/SiN/Experimental_vs_simulation_SiN.png
--rw-r--r--   0        0        0    56568 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/SiN/exp_SiN.mat
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/SiN/n_eff_data_SiN.npy
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pychi-0.0.7/examples/SiN/pychi_SiN_exp_vs_sim.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pychi-0.0.7/src/pychi/__init__.py
--rw-r--r--   0        0        0    14766 2020-02-02 00:00:00.000000 pychi-0.0.7/src/pychi/light.py
--rw-r--r--   0        0        0    13135 2020-02-02 00:00:00.000000 pychi-0.0.7/src/pychi/materials.py
--rw-r--r--   0        0        0    16980 2020-02-02 00:00:00.000000 pychi-0.0.7/src/pychi/models.py
--rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 pychi-0.0.7/src/pychi/solvers.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pychi-0.0.7/LICENSE
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 pychi-0.0.7/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pychi-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 pychi-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.390815 pychi-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 07:36:42.000000 pychi-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-12 07:37:05.390815 pychi-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-12 07:36:42.000000 pychi-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-12 07:36:56.000000 pychi-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:37:05.390815 pychi-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.386815 pychi-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.390815 pychi-0.0.8/src/pychi/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.390815 pychi-0.0.8/src/pychi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/top_level.txt
```

### Comparing `pychi-0.0.7/src/pychi/light.py` & `pychi-0.0.8/src/pychi/light.py`

 * *Files identical despite different names*

### Comparing `pychi-0.0.7/src/pychi/materials.py` & `pychi-0.0.8/src/pychi/materials.py`

 * *Files identical despite different names*

### Comparing `pychi-0.0.7/src/pychi/models.py` & `pychi-0.0.8/src/pychi/models.py`

 * *Files identical despite different names*

### Comparing `pychi-0.0.7/src/pychi/solvers.py` & `pychi-0.0.8/src/pychi/solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             elif self.local_error <= error < 2*self.local_error:
                 self.stock_z += self.dz
                 self.dz /= self.adaptive_factor
             elif 0.5*self.local_error <= error < self.local_error:
                 self.stock_z += self.dz
             else:
                 self.stock_z += self.dz
-                if self.max_dz is None or self.dz < self.max_dz:
+                if self.max_dz is None or self.dz*self.adaptive_factor < self.max_dz:
                     self.dz *= self.adaptive_factor
             self.stock_vec = vec_eval
     
     def solve(self):
         """
         Integrate over waveguide length with adaptive step size
         """
```

### Comparing `pychi-0.0.7/LICENSE` & `pychi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pychi-0.0.7/PKG-INFO` & `pychi-0.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-Metadata-Version: 2.1
-Name: pychi
-Version: 0.0.7
-Summary: Simulation package for the propagation of optical pulses in nonlinear media
-Project-URL: Homepage, https://github.com/pychi-code/pychi
-Project-URL: Documentation, https://pychi.readthedocs.io/en/latest/index.html
-Project-URL: PyPI, https://pypi.org/project/pychi/
-Author-email: Ultrafast Microphotonics Group - DESY <pychi@desy.de>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: matplotlib==3.1.3
-Requires-Dist: numba==0.56.0
-Requires-Dist: numpy==1.21.6
-Requires-Dist: pyfftw==0.12.0
-Requires-Dist: scipy==1.4.1
-Description-Content-Type: text/markdown
-
 # pychi
 
 A Python package for simulating the propagation of optical pulses in nonlinear materials.
 
-To install the package, run
+## Capabilities
+
+*pychi* is aimed at simulating the propagation of short pulses in nonlinear media and capturing as much physics as possible. It is based on a unidirectional propagation model, which stays valid even for sub-cycle optical pulses. In particular, this propagation model accounts for
+- Full frequency dependence of the effective refractive index
+- Quadratic nonlinear interactions (sum- and difference-frequency generation)
+- Cubic nonlinear interactions (triple sum-frequency generation, self-phase modulation, conjugated Kerr term)
+- Raman scattering
+- Self-steepening
+- Frequency-dependence of the nonlinear coefficients
+- z-dependence of the effective refractive index and nonlinear coefficients (permitting poling to be simulated)
+
+The package is built to be as user-friendly as possible, providing a relatively high-level interface for the user while still allowing for physically intricate simulation cases. It leverages a custom-made order 5 solver, although more classical solvers (such as the RK4IP) have also been implemented for completeness and versatility.
+
+## Installation
+
+First, make sure pip is up-to-date using
+```
+pip install --upgrade pip
+```
+
+Then install the package using
 ```
 pip install pychi
 ```
 
-The documentation is available under
+## Documentation
+
+The documentation is available and best viewed under
 https://pychi.readthedocs.io/en/latest/
+This documentation has been automatically generated using SPHINX, and is still a work in progress. Do not hesitate to contact us for any needed clarifications and examples.
 
+## Example
 
 Here is a typical example of the use of pychi to simulate the propagation of a short optical pulse in a nonlinear waveguide exhibiting both cubic and quadratic nonlinearities.
 
 ```python
 # -*- coding: utf-8 -*-
 """
 Created on Mon Feb 28 15:31:47 2022
@@ -75,25 +79,23 @@
 """
 Nonlinear propagation
 """
 ### Prepare waveguide
 waveguide = pychi.materials.Waveguide(wg_freq, wg_n_eff, wg_chi_2, wg_chi_3,
                                 wg_a_eff, wg_length, t_pts=t_pts)
 # Additional options:
-# One can provide beta coefficients (strongly discouraged) overwriting the refractive
-# index using waveguide.set_betas(betas, wavelength)
-#
 # wg_n_eff can be a 2 dimensional array, with first dimension the wavelength dependence
 # and second dimension the z dependence.
 #
 # chi2 and chi3 can be callables, returning a z dependent value. Alternatively, they
 # can be defined as one dimensional arrays describing their z dependence, or
-# two dimensional arrays describing their z and frequency dependence.
+# two dimensional arrays describing their z and frequency dependence. They
+# can also be callables of (z, freq).
 #
-# One can use waveguide.set_gamma(gamma) or waveguide.set_n2(n2) to provide
+# One can use waveguide.set_gamma(gamma) or waveguide.set_n2(n2) to provide a
 # nonlinear coefficient or nonlinear refractive index and overwrite chi3.
 #
 # Check documentation for more options and details.
 
 
 ### Prepare input pulse
 pulse = pychi.light.Sech(waveguide, pulse_duration, pulse_energy, pulse_wavelength)
@@ -125,15 +127,20 @@
 pulse.plot_propagation()
 # Results can also be accessed via pulse.z_save, pulse.freq, pulse.spectrum, pulse.waveform
 # The refractive index and GVD can be seen with waveguide.plot_refractive_index()
 
 
 ```
 
-Typical propagation results would look as follows:
+Typical propagation results using the above script would look as follows:
 ![grafik](https://user-images.githubusercontent.com/97957751/222731448-ff856390-4325-4f39-8817-f508898e2308.png)
 
 Check the examples folder for some specific cases and validation against experimental data.
 
+## Contact
 
 pychi has been developped at DESY by the Ultrafast Microphotonics group. If you use it for publications, please cite the associated paper
 https://doi.org/10.1063/5.0135252
+
+If you have any questions, remarks, contributions, do not hesitate to contact us at:
+pychi@desy.de
+or here on GitHub.
```

