# Comparing `tmp/fides-0.7.5.tar.gz` & `tmp/fides-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fides-0.7.5.tar", last modified: Thu Feb 10 17:29:00 2022, max compression
+gzip compressed data, was "fides-0.7.6.tar", last modified: Wed Apr 12 07:09:01 2023, max compression
```

## Comparing `fides-0.7.5.tar` & `fides-0.7.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:29:00.606004 fides-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-02-10 17:29:00.606004 fides-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-02-10 17:29:00.000000 fides-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:29:00.606004 fides-0.7.5/fides/
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-02-10 17:29:00.000000 fides-0.7.5/fides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5270 2022-02-10 17:29:00.000000 fides-0.7.5/fides/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    20130 2022-02-10 17:29:00.000000 fides-0.7.5/fides/hessian_approximation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-02-10 17:29:00.000000 fides-0.7.5/fides/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    32025 2022-02-10 17:29:00.000000 fides-0.7.5/fides/minimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-02-10 17:29:00.000000 fides-0.7.5/fides/stepback.py
--rw-r--r--   0 runner    (1001) docker     (121)    17254 2022-02-10 17:29:00.000000 fides-0.7.5/fides/steps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10253 2022-02-10 17:29:00.000000 fides-0.7.5/fides/subproblem.py
--rw-r--r--   0 runner    (1001) docker     (121)     4837 2022-02-10 17:29:00.000000 fides-0.7.5/fides/trust_region.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-10 17:29:00.000000 fides-0.7.5/fides/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 17:29:00.606004 fides-0.7.5/fides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-02-10 17:29:00.000000 fides-0.7.5/fides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-02-10 17:29:00.000000 fides-0.7.5/fides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 17:29:00.000000 fides-0.7.5/fides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-10 17:29:00.000000 fides-0.7.5/fides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-10 17:29:00.000000 fides-0.7.5/fides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-02-10 17:29:00.606004 fides-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-02-10 17:29:00.000000 fides-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:09:01.442666 fides-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-04-12 07:09:01.442666 fides-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-04-12 07:09:01.000000 fides-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:09:01.442666 fides-0.7.6/fides/
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-12 07:09:01.000000 fides-0.7.6/fides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-04-12 07:09:01.000000 fides-0.7.6/fides/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20130 2023-04-12 07:09:01.000000 fides-0.7.6/fides/hessian_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-12 07:09:01.000000 fides-0.7.6/fides/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32025 2023-04-12 07:09:01.000000 fides-0.7.6/fides/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-04-12 07:09:01.000000 fides-0.7.6/fides/stepback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-04-12 07:09:01.000000 fides-0.7.6/fides/steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10253 2023-04-12 07:09:01.000000 fides-0.7.6/fides/subproblem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-04-12 07:09:01.000000 fides-0.7.6/fides/trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-12 07:09:01.000000 fides-0.7.6/fides/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:09:01.442666 fides-0.7.6/fides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-12 07:09:01.442666 fides-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1755 2023-04-12 07:09:01.000000 fides-0.7.6/setup.py
```

### Comparing `fides-0.7.5/PKG-INFO` & `fides-0.7.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fides
-Version: 0.7.5
+Version: 0.7.6
 Summary: python Trust Region Optimization
-Home-page: UNKNOWN
+Home-page: https://github.com/Fides-dev/fides
 Author: Fabian Froehlich
 Author-email: froehlichfab@gmail.com
-License: UNKNOWN
+License: BSD-3-Clause
 Description: # Fides - A python package for Trust Region Optimization
         
         <a href="https://badge.fury.io/py/fides">
           <img src="https://badge.fury.io/py/fides.svg" alt="PyPI version"></a>
         <a href="https://codecov.io/gh/fides-dev/fides">
           <img src="https://codecov.io/gh/fides-dev/fides/branch/master/graph/badge.svg" alt="Code coverage"></a>
         <a href="https://fides-optimizer.readthedocs.io/en/latest/?badge=latest">
@@ -38,9 +38,21 @@
         * Exact, 2D and CG subproblem solvers
         * BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative
          Hessian Approximation schemes
         * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian Approximations schemes
         
         
 Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,17 +1,25 @@
-Metadata-Version: 2.1 Name: fides Version: 0.7.5 Summary: python Trust Region
-Optimization Home-page: UNKNOWN Author: Fabian Froehlich Author-email:
-froehlichfab@gmail.com License: UNKNOWN Description: # Fides - A python package
-for Trust Region Optimization [PyPI_version] [Code_coverage] [ReadTheDocs
-status] [DOI] ## About Fides Fides implements an Interior Trust Region
-Reflective for boundary constrained optimization problems based on the papers
-[ColemanLi1994](https://doi.org/10.1007/BF01582221) and [ColemanLi1996](http://
-dx.doi.org/10.1137/0806023). Accordingly, Fides is named after the Roman
-goddess of trust and reliability. Fides can be installed via `pip install
-fides`. Further documentation is available at [Read the Docs](https://fides-
-optimizer.readthedocs.io/). ## Features * Boundary constrained and
-unconstrained interior trust-region optimization * Reflective, truncated and
-optimization based boundary heuristics * Exact, 2D and CG subproblem solvers *
-BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative Hessian
-Approximation schemes * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian
-Approximations schemes Platform: UNKNOWN Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: fides Version: 0.7.6 Summary: python Trust Region
+Optimization Home-page: https://github.com/Fides-dev/fides Author: Fabian
+Froehlich Author-email: froehlichfab@gmail.com License: BSD-3-Clause
+Description: # Fides - A python package for Trust Region Optimization [PyPI
+version] [Code_coverage] [ReadTheDocs_status] [DOI] ## About Fides Fides
+implements an Interior Trust Region Reflective for boundary constrained
+optimization problems based on the papers [ColemanLi1994](https://doi.org/
+10.1007/BF01582221) and [ColemanLi1996](http://dx.doi.org/10.1137/0806023).
+Accordingly, Fides is named after the Roman goddess of trust and reliability.
+Fides can be installed via `pip install fides`. Further documentation is
+available at [Read the Docs](https://fides-optimizer.readthedocs.io/). ##
+Features * Boundary constrained and unconstrained interior trust-region
+optimization * Reflective, truncated and optimization based boundary heuristics
+* Exact, 2D and CG subproblem solvers * BFGS, DFP, SR1, Broyden (good and bad)
+and Broyden class iterative Hessian Approximation schemes * SSM, TSSM, FX,
+GNSBFGS and custom hybrid Hessian Approximations schemes Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Science/Research Classifier: Topic :: Software Development ::
+Libraries Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `fides-0.7.5/README.md` & `fides-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/constants.py` & `fides-0.7.6/fides/constants.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/hessian_approximation.py` & `fides-0.7.6/fides/hessian_approximation.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/logging.py` & `fides-0.7.6/fides/logging.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/minimize.py` & `fides-0.7.6/fides/minimize.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/stepback.py` & `fides-0.7.6/fides/stepback.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/steps.py` & `fides-0.7.6/fides/steps.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/subproblem.py` & `fides-0.7.6/fides/subproblem.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides/trust_region.py` & `fides-0.7.6/fides/trust_region.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.5/fides.egg-info/PKG-INFO` & `fides-0.7.6/fides.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fides
-Version: 0.7.5
+Version: 0.7.6
 Summary: python Trust Region Optimization
-Home-page: UNKNOWN
+Home-page: https://github.com/Fides-dev/fides
 Author: Fabian Froehlich
 Author-email: froehlichfab@gmail.com
-License: UNKNOWN
+License: BSD-3-Clause
 Description: # Fides - A python package for Trust Region Optimization
         
         <a href="https://badge.fury.io/py/fides">
           <img src="https://badge.fury.io/py/fides.svg" alt="PyPI version"></a>
         <a href="https://codecov.io/gh/fides-dev/fides">
           <img src="https://codecov.io/gh/fides-dev/fides/branch/master/graph/badge.svg" alt="Code coverage"></a>
         <a href="https://fides-optimizer.readthedocs.io/en/latest/?badge=latest">
@@ -38,9 +38,21 @@
         * Exact, 2D and CG subproblem solvers
         * BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative
          Hessian Approximation schemes
         * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian Approximations schemes
         
         
 Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,17 +1,25 @@
-Metadata-Version: 2.1 Name: fides Version: 0.7.5 Summary: python Trust Region
-Optimization Home-page: UNKNOWN Author: Fabian Froehlich Author-email:
-froehlichfab@gmail.com License: UNKNOWN Description: # Fides - A python package
-for Trust Region Optimization [PyPI_version] [Code_coverage] [ReadTheDocs
-status] [DOI] ## About Fides Fides implements an Interior Trust Region
-Reflective for boundary constrained optimization problems based on the papers
-[ColemanLi1994](https://doi.org/10.1007/BF01582221) and [ColemanLi1996](http://
-dx.doi.org/10.1137/0806023). Accordingly, Fides is named after the Roman
-goddess of trust and reliability. Fides can be installed via `pip install
-fides`. Further documentation is available at [Read the Docs](https://fides-
-optimizer.readthedocs.io/). ## Features * Boundary constrained and
-unconstrained interior trust-region optimization * Reflective, truncated and
-optimization based boundary heuristics * Exact, 2D and CG subproblem solvers *
-BFGS, DFP, SR1, Broyden (good and bad) and Broyden class iterative Hessian
-Approximation schemes * SSM, TSSM, FX, GNSBFGS and custom hybrid Hessian
-Approximations schemes Platform: UNKNOWN Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: fides Version: 0.7.6 Summary: python Trust Region
+Optimization Home-page: https://github.com/Fides-dev/fides Author: Fabian
+Froehlich Author-email: froehlichfab@gmail.com License: BSD-3-Clause
+Description: # Fides - A python package for Trust Region Optimization [PyPI
+version] [Code_coverage] [ReadTheDocs_status] [DOI] ## About Fides Fides
+implements an Interior Trust Region Reflective for boundary constrained
+optimization problems based on the papers [ColemanLi1994](https://doi.org/
+10.1007/BF01582221) and [ColemanLi1996](http://dx.doi.org/10.1137/0806023).
+Accordingly, Fides is named after the Roman goddess of trust and reliability.
+Fides can be installed via `pip install fides`. Further documentation is
+available at [Read the Docs](https://fides-optimizer.readthedocs.io/). ##
+Features * Boundary constrained and unconstrained interior trust-region
+optimization * Reflective, truncated and optimization based boundary heuristics
+* Exact, 2D and CG subproblem solvers * BFGS, DFP, SR1, Broyden (good and bad)
+and Broyden class iterative Hessian Approximation schemes * SSM, TSSM, FX,
+GNSBFGS and custom hybrid Hessian Approximations schemes Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Science/Research Classifier: Topic :: Software Development ::
+Libraries Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

