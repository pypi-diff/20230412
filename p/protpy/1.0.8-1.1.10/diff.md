# Comparing `tmp/protpy-1.0.8.tar.gz` & `tmp/protpy-1.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protpy-1.0.8.tar", last modified: Thu Feb 23 15:37:09 2023, max compression
+gzip compressed data, was "protpy-1.1.10.tar", last modified: Wed Apr 12 15:00:15 2023, max compression
```

## Comparing `protpy-1.0.8.tar` & `protpy-1.1.10.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:37:09.102317 protpy-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-23 15:36:44.000000 protpy-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 15:36:44.000000 protpy-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-02-23 15:37:09.102317 protpy-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-02-23 15:36:44.000000 protpy-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:37:09.098317 protpy-1.0.8/protpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/conjoint_triad.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/ctd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:37:09.102317 protpy-1.0.8/protpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/data/grantham-physiochemical-distance-matrix.json
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/data/schneider-wrede-physiochemical-distance-matrix.json
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-02-23 15:36:44.000000 protpy-1.0.8/protpy/sequence_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:37:09.102317 protpy-1.0.8/protpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-02-23 15:37:09.000000 protpy-1.0.8/protpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-23 15:37:09.000000 protpy-1.0.8/protpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 15:37:09.000000 protpy-1.0.8/protpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 15:37:07.000000 protpy-1.0.8/protpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-23 15:37:09.000000 protpy-1.0.8/protpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-23 15:37:09.000000 protpy-1.0.8/protpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-23 15:37:09.102317 protpy-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-02-23 15:36:44.000000 protpy-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:37:09.102317 protpy-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 15:36:44.000000 protpy-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-02-23 15:36:44.000000 protpy-1.0.8/tests/test_autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26020 2023-02-23 15:36:44.000000 protpy-1.0.8/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-02-23 15:36:44.000000 protpy-1.0.8/tests/test_conjoint_triad.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-02-23 15:36:44.000000 protpy-1.0.8/tests/test_ctd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-02-23 15:36:44.000000 protpy-1.0.8/tests/test_protpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-02-23 15:36:44.000000 protpy-1.0.8/tests/test_sequence_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:15.246240 protpy-1.1.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 14:59:52.000000 protpy-1.1.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 14:59:52.000000 protpy-1.1.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-04-12 15:00:15.246240 protpy-1.1.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-04-12 14:59:52.000000 protpy-1.1.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:15.246240 protpy-1.1.10/protpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/conjoint_triad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/ctd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:15.246240 protpy-1.1.10/protpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/data/grantham-physiochemical-distance-matrix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/data/schneider-wrede-physiochemical-distance-matrix.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16989 2023-04-12 14:59:52.000000 protpy-1.1.10/protpy/sequence_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:15.246240 protpy-1.1.10/protpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-04-12 15:00:15.000000 protpy-1.1.10/protpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-12 15:00:15.000000 protpy-1.1.10/protpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:00:15.000000 protpy-1.1.10/protpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:00:14.000000 protpy-1.1.10/protpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 15:00:15.000000 protpy-1.1.10/protpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 15:00:15.000000 protpy-1.1.10/protpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-12 15:00:15.250239 protpy-1.1.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-12 14:59:52.000000 protpy-1.1.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:15.246240 protpy-1.1.10/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:59:52.000000 protpy-1.1.10/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-12 14:59:52.000000 protpy-1.1.10/tests/test_autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33856 2023-04-12 14:59:52.000000 protpy-1.1.10/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-12 14:59:52.000000 protpy-1.1.10/tests/test_conjoint_triad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-04-12 14:59:52.000000 protpy-1.1.10/tests/test_ctd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-12 14:59:52.000000 protpy-1.1.10/tests/test_protpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31746 2023-04-12 14:59:52.000000 protpy-1.1.10/tests/test_sequence_order.py
```

### Comparing `protpy-1.0.8/LICENSE` & `protpy-1.1.10/LICENSE`

 * *Files identical despite different names*

### Comparing `protpy-1.0.8/PKG-INFO` & `protpy-1.1.10/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: protpy
-Version: 1.0.8
+Version: 1.1.10
 Summary: Python package for generating various biochemical, physiochemical and structural descriptors/features of protein sequences.
 Home-page: https://github.com/amckenna41/protPy
 Author: MIT
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/protPy/archive/refs/heads/main.zip
 Description: 
         # protpy - Package for generating protein physiochemical, biochemical and structural descriptors using their constituent amino acids. #
         [![PyPI](https://img.shields.io/pypi/v/protpy)](https://pypi.org/project/protpy/)
         [![pytest](https://github.com/amckenna41/protpy/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/protpy/actions?query=workflowBuilding%20and%20Testing)
         [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/protpy/)
         [![PythonV](https://img.shields.io/pypi/pyversions/protpy?logo=2)](https://pypi.org/project/protpy/)
         [![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://opensource.org/licenses/MIT)
-        <!-- [![Build](https://img.shields.io/github/workflow/status/amckenna41/protpy/Deploy%20to%20PyPI%20%F0%9F%93%A6)](https://github.com/amckenna41/protpy/actions) -->
-        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/pySAR.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/pySAR) -->
-        <!-- [![DOI](https://zenodo.org/badge/344290370.svg)](https://zenodo.org/badge/latestdoi/344290370) -->
-        <!-- [![codecov](https://codecov.io/gh/amckenna41/DCBLSTM_PSP/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/DCBLSTM_PSP) -->
         [![Issues](https://img.shields.io/github/issues/amckenna41/protpy)](https://github.com/amckenna41/protpy/issues)
         [![Size](https://img.shields.io/github/repo-size/amckenna41/protpy)](https://github.com/amckenna41/protpy)
         [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/protpy)](https://github.com/amckenna41/protpy)
-        
+        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/pySAR.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/pySAR) -->
+        <!-- [![DOI](https://zenodo.org/badge/344290370.svg)](https://zenodo.org/badge/latestdoi/344290370) -->
+        <!-- [![codecov](https://codecov.io/gh/amckenna41/DCBLSTM_PSP/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/DCBLSTM_PSP) -->
         <!-- <p align="center">
         <img src="https://images.newscientist.com/wp-content/uploads/2021/07/22155326/22-july_deepmind-proteome.jpg?width=300" alt="protpyLogo" height="200"/>
         </p> -->
         
         Table of Contents
         -----------------
```

### Comparing `protpy-1.0.8/README.md` & `protpy-1.1.10/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 
 # protpy - Package for generating protein physiochemical, biochemical and structural descriptors using their constituent amino acids. #
 [![PyPI](https://img.shields.io/pypi/v/protpy)](https://pypi.org/project/protpy/)
 [![pytest](https://github.com/amckenna41/protpy/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/protpy/actions?query=workflowBuilding%20and%20Testing)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/protpy/)
 [![PythonV](https://img.shields.io/pypi/pyversions/protpy?logo=2)](https://pypi.org/project/protpy/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://opensource.org/licenses/MIT)
-<!-- [![Build](https://img.shields.io/github/workflow/status/amckenna41/protpy/Deploy%20to%20PyPI%20%F0%9F%93%A6)](https://github.com/amckenna41/protpy/actions) -->
-<!-- [![CircleCI](https://circleci.com/gh/amckenna41/pySAR.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/pySAR) -->
-<!-- [![DOI](https://zenodo.org/badge/344290370.svg)](https://zenodo.org/badge/latestdoi/344290370) -->
-<!-- [![codecov](https://codecov.io/gh/amckenna41/DCBLSTM_PSP/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/DCBLSTM_PSP) -->
 [![Issues](https://img.shields.io/github/issues/amckenna41/protpy)](https://github.com/amckenna41/protpy/issues)
 [![Size](https://img.shields.io/github/repo-size/amckenna41/protpy)](https://github.com/amckenna41/protpy)
 [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/protpy)](https://github.com/amckenna41/protpy)
-
+<!-- [![CircleCI](https://circleci.com/gh/amckenna41/pySAR.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/pySAR) -->
+<!-- [![DOI](https://zenodo.org/badge/344290370.svg)](https://zenodo.org/badge/latestdoi/344290370) -->
+<!-- [![codecov](https://codecov.io/gh/amckenna41/DCBLSTM_PSP/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/DCBLSTM_PSP) -->
 <!-- <p align="center">
 <img src="https://images.newscientist.com/wp-content/uploads/2021/07/22155326/22-july_deepmind-proteome.jpg?width=300" alt="protpyLogo" height="200"/>
 </p> -->
 
 Table of Contents
 -----------------
```

### Comparing `protpy-1.0.8/protpy/__init__.py` & `protpy-1.1.10/protpy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# from .autocorrelation import moreaubroto_autocorrelation, moran_autocorrelation, geary_autocorrelation
 from .autocorrelation import *
 from .composition import *
 from .conjoint_triad import *
 from .ctd import *
 from .sequence_order import *
 
 #protPy package metadata
 __name__ = 'protpy'
-__version__ = "1.0.8"
+__version__ = "1.1.10"
 __description__ = "Python package for generating various biochemical, physiochemical and structural descriptors/features of protein sequences."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __maintainer__ = "AJ McKenna"
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/protPy'
 __download_url__ = "https://github.com/amckenna41/protPy/archive/refs/heads/main.zip"
 __status__ = "Production"
 __keywords__ = ["bioinformatics", "protein engineering", "python", "pypi", "machine learning", \
                 "aaindex", "protein descriptors", "physiochemical descriptors", "biochemical descriptors"
                 "structural descriptors"]
 __test_suite__ = "tests"
 
 #list of all available descriptors in protPy
-all_descriptors = ["aa_composition", "dipeptide_composition", "tripeptide_composition",
+all_descriptors = ["amino_acid_composition", "dipeptide_composition", "tripeptide_composition",
     "moreaubroto_autocorrelation", "moran_autocorrelation", "geary_autocorrelation",
     "pseudo_amino_acid_composition", "amphiphilic_pseudo_amino_acid_composition", 
     "sequence_order_coupling_number", "conjoint_triad", "ctd_composition", 
     "ctd_transition", "ctd_distribution", "quasi_sequence_order"
     ]
```

### Comparing `protpy-1.0.8/protpy/autocorrelation.py` & `protpy-1.1.10/protpy/autocorrelation.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,32 +22,36 @@
     J. Math. Chem., vol. 33, no. 2, pp. 91–101, 2003.
 """
 
 #list of amino acids
 amino_acids = ["A", "C", "D", "E", "F", "G", "H", "I", "K", "L", "M", "N", "P", 
     "Q", "R", "S", "T", "V", "W", "Y"]
     
+############################### MoreauBroto Autocorrelation ###############################
+
 def moreaubroto_autocorrelation(sequence, lag=30, 
     properties=["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
     "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"], normalize=True):
     """
-    Calculate Normalized MoreauBrotoAuto Autocorrelation (NMBAuto) descriptor.
+    Calculate MoreauBrotoAuto Autocorrelation (MBAuto) descriptor for sequence.
     Autocorrelation descriptors are a class of topological descriptors,
     also known as molecular connectivity indices, that describe the level of
     correlation between two objects (protein or peptide sequences) in terms of
     their specific structural or physicochemical properties, which are
     defined based on the distribution of amino acid properties along the sequence.
-    By default, 8 amino acid properties are used for deriving the descriptors. The derivations
-    and detailed explanations of this type of descriptor is outlind in [2].
-    The NMBAuto descriptor is a type of Autocorrelation descriptor that uses
-    the property values as the basis for measurement. Each autocorrelation will
-    generate the number of features depending on the lag value and number of
-    properties input with total features = lag * number of properties. Using 
-    the default 8 properties with default lag value of 30, 240 features are 
-    generated, the default 8 properties are:
+    By default, 8 amino acid properties are used for deriving the descriptors. 
+    The derivations and detailed explanations of this type of descriptor is 
+    outlind in [2]. The MBAuto descriptor is a type of Autocorrelation 
+    descriptor that uses the property values as the basis for measurement. 
+    Each autocorrelation will generate the number of features depending on the 
+    lag value and number of properties input with total features = lag * number 
+    of properties. The output autocorrelation can also be normalized by setting
+    the normalize parameter to true, this occurs by default. Using the default 8 
+    properties with default lag value of 30, 240 features are generated, 
+    the default 8 properties are:
 
     AccNo. CIDH920105 - Normalized Average Hydrophobicity Scales
     AccNo. BHAR880101 - Average Flexibility Indices
     AccNo. CHAM820101 - Polarizability Parameter
     AccNo. CHAM820102 - Free Energy of Solution in Water, kcal/mole
     AccNo. CHOC760101 - Residue Accessible Surface Area in Tripeptide
     AccNo. BIGC670101 - Residue Volume
@@ -59,37 +63,37 @@
     :sequence : str
         protein sequence.
     :lag : int (default=30)
         A value for a lag, the max value is equal to the length of shortest peptide minus one.
     :properties : list (default=["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
             "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"])
         list of AAI index record codes/accession numbers for the physiochemical properties to 
-        use in the calculation of descriptor.
+        use in the calculation of the descriptor.
     :normalize : bool (default=True)
         rescale/normalize MoreauBroto Autocorrelation values into range of 0-1.
 
     Returns
     -------
     :moreaubroto_autocorrelation_df : pd.Dataframe
-        pandas Dataframe of NMBAuto values for protein sequence. Output will
+        pandas Dataframe of MBAuto values for protein sequence. Output will
         be of the shape N x 1, where N is the number of features calculated from
         the descriptor. By default, the shape will be 240 x 1 (30 features per 
-        property - using 8 properties).
+        property - using 8 properties and lag=30).
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     #validate lag, set default lag if invalid value input
     if (lag>=len(sequence) or (lag<0) or not (isinstance(lag, int))):
         lag = 30
 
     #validate that at least 1 property input to function
     if (properties == "" or properties == []):
@@ -98,93 +102,94 @@
     #if 1 property passed into function, wrap it to an iterable list
     if (isinstance(properties, str)):
         properties = [properties]
     
     #initialise dicts to store AAI properties and values
     aai_properties = {}
     for prop in properties:
-        #go to next iteration if invalid accession number in aaindex1
+        #raise value error if accession number not found in aaindex1
         if not (prop in aaindex1.record_codes()):
-            continue
+            raise ValueError("Property {} not found in list of available properties in the aaindex1.".format(prop))
         aai_properties[prop] = {}
 
     #iterate through list of properties, getting property values from AAIndex
     for prop in list(aai_properties.keys()):
         #get property values from AAIndex 
         aaindex1[prop].values.pop('-', None)
         prop_amino_acid_values = aaindex1[prop].values
      
         #normalise property values if applicable, calculate mean and std dev
         aai_property_vals = {}
         if (normalize):
             for i, j in prop_amino_acid_values.items():
                 aai_property_vals[i] = (j - (sum(prop_amino_acid_values.values()) / 
                     len(prop_amino_acid_values.values()))) / _std(prop_amino_acid_values.values(), ddof=0)
-
         aa_counter = 0
 
         #assign property and associated amino acid values to aai_property_vals array
         for i, j in aai_property_vals.items():
             aai_property_vals[amino_acids[aa_counter]] = aai_property_vals[i]
             aa_counter+=1
         aai_properties[prop] = aai_property_vals
 
     #store resultant autocorrelation values
     moreaubroto_autocorrelation = {}
 
     #iterate through list of properties, calculating autocorrelation values for the sequence, append to results dict
     for key in aai_properties:
         temp = 0
-        for i in range(1,lag+1):
+        for i in range(1, lag+1):
             for j in range(len(sequence)-i):
                 temp = temp + aai_properties[key][sequence[j]] * aai_properties[key][sequence[j+1]]
-            if len(sequence) - i == 0:
+            if (len(sequence) - i == 0):
                 moreaubroto_autocorrelation["MBAuto_" + key + "_" + str(i)] = round(
                     temp / (len(sequence)), 3)
             else:
                 moreaubroto_autocorrelation["MBAuto_" + key + "_" + str(i)] = round(
                     temp / (len(sequence) - i), 3)
 
     #transform values and columns to DataFrame
     moreaubroto_autocorrelation_df = pd.DataFrame([list(moreaubroto_autocorrelation.values())], 
         columns=list(moreaubroto_autocorrelation.keys()))
 
     return moreaubroto_autocorrelation_df
 
+################################## Moran Autocorrelation ##################################
+
 def moran_autocorrelation(sequence, lag=30, 
     properties=["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
     "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"], normalize=True):
     """
-    **refer to NMBAuto docstring for autocorrelation description.
+    **refer to MBAuto docstring for autocorrelation description.
     Moran autocorrelation (MAuto) utilizes property deviations from the
     average values.
 
     Parameters
     ----------
-    **refer to NMBAuto docstring for autocorrelation parameters.
+    **refer to MBAuto docstring for autocorrelation parameters.
 
     Returns
     -------
     :moran_autocorrelation_df : pd.DataFrame
         pandas Dataframe of MAuto values for protein sequence. Output will
         be of the shape N x 1, where N is the number of features calculated from
         the descriptor. By default, the shape will be 240 x 1 (30 features per 
-        property - using 8 properties).  
+        property - using 8 properties and lag=30).  
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     #validate lag, set default lag if invalid value input
     if (lag>=len(sequence) or (lag<0) or not (isinstance(lag, int))):
         lag = 30
 
     #validate at least 1 property input to function
     if (properties == "" or properties == []):
@@ -193,17 +198,17 @@
     #if 1 property passed into function, wrap it to an iterable list
     if (isinstance(properties, str)):
         properties = [properties]
 
     #initialise dicts to store AAI properties and values
     aai_properties = {}
     for prop in properties:
-        #go to next iteration if invalid accession number in aaindex1
+        #raise value error if accession number not found in aaindex1
         if not (prop in aaindex1.record_codes()):
-            continue
+            raise ValueError("Property {} not found in list of available properties in the aaindex1.".format(prop))
         aai_properties[prop] = {}
 
     #iterate through list of properties, getting property values from AAIndex
     for prop in list(aai_properties.keys()):
         #get property values from AAIndex
         aaindex1[prop].values.pop('-', None)
         prop_aminoacid_values = aaindex1[prop].values
@@ -211,15 +216,14 @@
         aai_property_vals = {}
 
         #normalise property values, calculate mean and std dev        
         if (normalize):
             for i, j in prop_aminoacid_values.items():
                 aai_property_vals[i] = (j - (sum(prop_aminoacid_values.values()) / 
                     len(prop_aminoacid_values.values()))) / _std(prop_aminoacid_values.values(), ddof=0)
-
         aa_counter = 0
 
         #assign property and associated amino acid values to aai_property_vals array
         for i, j in aai_property_vals.items():
             aai_property_vals[amino_acids[aa_counter]] = aai_property_vals[i]
             aa_counter+=1
         aai_properties[prop] = aai_property_vals
@@ -233,15 +237,15 @@
         for aa in amino_acids:
             cds = cds + sequence.count(aa) * aai_properties[key][aa]
         prop_mean = cds / len(sequence)
         cc = []
         for aa in sequence:
             cc.append(aai_properties[key][aa])
         k = (_std(cc, ddof=0)) ** 2
-        for i in range(1,lag+1):
+        for i in range(1, lag+1):
             temp = 0
             for j in range(len(sequence) - i):
                 temp = temp + aai_properties[key][sequence[j]] - prop_mean * (
                     aai_properties[key][sequence[j+i]] - prop_mean)
             if len(sequence) - i == 0:
                 moran_autocorrelation["MAuto_" + key + "_" + str(i)] = round(
                     temp / ((len(sequence)) / k), 5)
@@ -251,45 +255,47 @@
 
     #transform values and columns to DataFrame
     moran_autocorrelation_df = pd.DataFrame([list(moran_autocorrelation.values())], 
         columns=list(moran_autocorrelation.keys()))
 
     return moran_autocorrelation_df
 
+################################## Geary Autocorrelation ##################################
+
 def geary_autocorrelation(sequence, lag=30, 
     properties=["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
     "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"], normalize=True):
     """
-    **refer to NMBAuto docstring for autocorrelation description.
+    **refer to MBAuto docstring for autocorrelation description.
     Geary Autocorrelation (GAuto) utilizes the square-difference of property
     values instead of vector-products (of property values or deviations).
     
     Parameters
     ----------
-    **refer to NMBAuto docstring for autocorrelation parameters.
+    **refer to MBAuto docstring for autocorrelation parameters.
 
     Returns
     -------
     :geary_autocorrelation_df : pd.DataFrame
         pandas DataFrame of GAuto values for protein sequence. Output will
         be of the shape N x 1, where N is the number of features calculated from
         the descriptor. By default, the shape will be 240 x 1 (30 features per 
-        property - using 8 properties).
+        property - using 8 properties and lag=30).
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
             
     #validate lag, set default lag if invalid value input
     if (lag>=len(sequence) or (lag<0) or not (isinstance(lag, int))):
         lag = 30
 
     #validate at least 1 property input to function
     if (properties == "" or properties == []):
@@ -298,17 +304,17 @@
     #if 1 property passed into function, wrap it to an iterable list
     if (isinstance(properties, str)):
         properties = [properties]
         
     #initialise dicts to store AAI properties and values
     aai_properties = {}
     for prop in properties:
-        #go to next iteration if invalid accession number in aaindex1
+        #raise value error if accession number not found in aaindex1
         if not (prop in aaindex1.record_codes()):
-            continue
+            raise ValueError("Property {} not found in list of available properties in the aaindex1.".format(prop))
         aai_properties[prop] = {}
 
     #iterate through list of properties, getting property values from AAIndex
     for prop in list(aai_properties.keys()):
         #get property values from AAIndex & reshape
         aaindex1[prop].values.pop('-', None)
         prop_aminoacid_values = aaindex1[prop].values
@@ -316,15 +322,14 @@
         aai_property_vals = {}
 
         #normalise property values, calculate mean and std dev
         if (normalize):
             for i, j in prop_aminoacid_values.items():
                 aai_property_vals[i] = (j - (sum(prop_aminoacid_values.values()) / 
                     len(prop_aminoacid_values.values()))) / _std(prop_aminoacid_values.values(), ddof=0)
-
         aa_counter = 0
 
         #assign property and associated amino acid values to aai_property_vals array
         for i, j in aai_property_vals.items():
             aai_property_vals[amino_acids[aa_counter]] = aai_property_vals[i]
             aa_counter+=1
         aai_properties[prop] = aai_property_vals
@@ -334,19 +339,19 @@
 
     #iterate through list of properties, calculating autocorrelation values for the sequence, append to results dict
     for key in aai_properties:
         cc = []
         for aa in sequence:
             cc.append(aai_properties[key][aa])
         k = ((np.std(cc, ddof=0)) ** 2) * len(sequence) / (len(sequence) - 1)
-        for i in range(1,lag+1):
+        for i in range(1, lag+1):
             temp = 0
             for j in range(len(sequence) - i):
                 temp = (temp + (
-                    aai_properties[key][sequence[j]] - aai_properties[key][sequence[j+i]]) **2)
+                    aai_properties[key][sequence[j]] - aai_properties[key][sequence[j+i]]) ** 2)
             if len(sequence) - i == 0:
                 geary_autocorrelation["GAuto_" + key + "_" + str(i)] = round(
                     temp / (2* (len(sequence))) / k, 3)
             else:
                 geary_autocorrelation["GAuto_" + key + "_" + str(i)] = round(
                     temp / (2* (len(sequence) -i)) / k, 3)
 
@@ -370,8 +375,8 @@
 
     Returns
     -------
     :result : np.array
         input array after standard deviation transformation.
     """
     return math.sqrt(sum([math.pow(i - sum(array) / len(array), 2) for i in array]) 
-        / (len(array) - ddof))
+        / (len(array) - ddof))
```

### Comparing `protpy-1.0.8/protpy/composition.py` & `protpy-1.1.10/protpy/composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,29 @@
 import pandas as pd
 import math
 from aaindex import aaindex1
 
 """
 References
 ----------
-[1] Reczko, M. and Bohr, H. (1994) The DEF data base of sequence based protein
-    fold class predictions. Nucleic Acids Res, 22, 3616-3619.
-
+[1] Gromiha, M. M. (2010). Protein Sequence Analysis. In M. M. Gromiha (Ed.), 
+    Protein Bioinformatics (pp. 29–62). Elsevier.
 [2] Hua, S. and Sun, Z. (2001) Support vector machine approach for protein
     subcellular localization prediction. Bioinformatics, 17, 721-728.
-
 [3] Grassmann, J., Reczko, M., Suhai, S. and Edler, L. (1999) Protein fold
     class prediction: new methods of statistical classification. Proc Int Conf
     Intell Syst Mol Biol, 106-112.
 [4] Kuo-Chen Chou. Prediction of Protein Cellular Attributes Using Pseudo-Amino Acid
     Composition. PROTEINS: Structure, Function, and Genetics, 2001, 43: 246-255.
-
 [5] Kuo-Chen Chou, Using amphiphilic pseudo amino acid composition to predict enzyme 
     subfamily classes, Bioinformatics, Volume 21, Issue 1, January 2005, Pages 10–19, 
     https://doi.org/10.1093/bioinformatics/bth466
-
 [6] http://www.csbio.sjtu.edu.cn/bioinf/PseAAC/ParaValue.htm.
+[7] Reczko, M. and Bohr, H. (1994) The DEF data base of sequence based protein
+    fold class predictions. Nucleic Acids Res, 22, 3616-3619.
 """
 #list of amino acids
 amino_acids = ["A", "C", "D", "E", "F", "G", "H", "I", "K", "L", "M", "N", "P", 
     "Q", "R", "S", "T", "V", "W", "Y"]
 
 #physiochemical values for all amino acids for hydrophobicity, hydrophilicty and residue mass
 #values taken from http://www.csbio.sjtu.edu.cn/bioinf/PseAAC/ParaValue.htm
@@ -53,25 +51,27 @@
 residue_mass_ = {
         "A": 15.0, "C": 47.0, "D": 59.0, "E": 73.0, "F": 91.0, "G": 1.000, 
         "H": 82.0, "I": 57.0, "K": 73.0, "L": 57.0,  "M": 75.0, "N": 58.0, 
         "P": 42.0, "Q": 72.0, "R": 101.0, "S": 31.0, "T": 45.0, "V": 43.0, 
         "W": 130.0, "Y": 107.0
 }
 
+################################# Amino Acid Composition ##################################
+
 def amino_acid_composition(sequence):
     """
     Calculate Amino Acid Composition (AAComp) of protein sequence. AAComp
     describes the fraction of each amino acid type within a protein sequence,
     and is calculated as:
 
     AA_Comp(s) = AA(t)/N(s)
 
     where AA_Comp(s) is the AAComp of protein sequence s, AA(t) is the number
     of amino acid types t (where t = 1,2,..,20) and N(s) is the length of the
-    sequence s.
+    sequence s [1].
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
 
     Returns
@@ -87,42 +87,44 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     amino_acid_composition = {}
 
     #iterate through each amino acid, calculating each composition
     for aa in amino_acids:
         amino_acid_composition[aa] = round(float(sequence.count(aa)) / len(sequence) * 100, 3)
 
     #transform values and columns to DataFrame
     amino_acid_composition_df = pd.DataFrame([list(amino_acid_composition.values())], 
         columns=list(amino_acid_composition.keys()))
 
     return amino_acid_composition_df
 
+################################## Dipeptide Composition ##################################
+
 def dipeptide_composition(sequence):
     """
     Calculate Dipeptide Composition (DPComp) for protein sequence.
     Dipeptide composition is the fraction of each dipeptide type within a
     protein sequence. With dipeptides being of length 2 and there being 20
     canonical amino acids this creates 20^2 different combinations, thus a
     400-Dimensional vector will be produced such that:
 
     DPComp(s,t) = AA(s,t) / N -1
 
     where DPComp(s,t) is the dipeptide composition of the protein sequence
     for amino acid type s and t (where s and t = 1,2,..,20), AA(s,t) is the number
     of dipeptides represented by amino acid type s and t and N is the total number
-    of dipeptides.
+    of dipeptides [1].
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
 
     Returns
@@ -138,15 +140,15 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     dipeptide_composition = {}
 
     #iterate through each amino acid, calculating each dipeptide combination's composition
     for i in amino_acids:
         for j in amino_acids:
             dipep = i + j
@@ -155,28 +157,30 @@
 
     #transform values and columns to DataFrame
     dipeptide_composition_df = pd.DataFrame([list(dipeptide_composition.values())], 
         columns=list(dipeptide_composition.keys()))
 
     return dipeptide_composition_df
 
+################################## Tripeptide Composition #################################
+
 def tripeptide_composition(sequence):
     """
     Calculate Tripeptide Composition (TPComp) of protein sequence.
     Tripeptide composition is the fraction of each tripeptide type within a
     protein sequence. With tripeptides being of length 3 and there being 20
     canonical amino acids this creates 20^3 different combinations, thus a
     8000-Dimensional vector will be produced such that:
 
     TPComp(s,t,u) = AA(s,t,u) / N -1
 
     where TPComp(s,t,u) is the tripeptide composition of the protein sequence
     for amino acid type s, t and u (where s, t and u = 1,2,..,20), AA(s,t,u) is
     the number of tripeptides represented by amino acid type s and t, and N is
-    the total number of tripeptides.
+    the total number of tripeptides [1].
 
     Parameters
     ----------
     :sequence : str
         protein sequence in str form.
 
     Returns
@@ -192,15 +196,15 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     tripeptide_composition = {}
     tripeptides = []    
 
     #get list of tripeptides
     for i in amino_acids:
         for j in amino_acids:
@@ -219,26 +223,26 @@
 
 ############################## Pseudo Amino Acid Composition ##############################
 
 def pseudo_amino_acid_composition(sequence, lamda=30, weight=0.05, properties=[]):
     """
     Pseudo amino acid composition (PAAComp) combines the vanilla amino acid composition descriptor with 
     additional local features, such as correlation between residues of a certain distance, as
-    amino acid composition doesn't take into accont sequence order info. The pseudo 
+    amino acid composition doesn't take into account sequence order info. The pseudo 
     components of the descriptor are a series rank-different correlation factors [5].
     The first 20 components are a weighted sum of the amino acid composition and 30 are 
     physiochemical square correlations as dictated by the lamda and properties parameters.
     This generates an output of [1, (20 + lamda)] = 1 x 50 when using the default lamda of 30. 
     By default, the physiochemical properties used are hydrophobicity and hydrophillicity, with 
     a lamda of 30 and weight of 0.05.
 
     Parameters
     ----------
     :lamda: int
-        rank of correlation. Number of calculable descriptors depends on lamda.
+        rank of correlation. Number of calculable descriptors depends on lamda value.
     :weight: float
         weighting factor.
     :properties : list 
         list of dicts of physiochemical/structural property values for amino acids.
 
     Returns
     -------
@@ -252,32 +256,32 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
-    #set lamda to its default value if <0, or > sequence len or not an int
+    #set lamda to its default value of 30 if <0, or > sequence len or not an int
     if ((lamda < 0) or (lamda > len(sequence)) or not isinstance(lamda, int)):
         lamda = 30  
 
-    #validate weight, set default weight if invalid value input
+    #validate weight, set default weight of 0.05 if invalid value input
     if ((weight<0) or not (isinstance(weight, float)) or not (isinstance(weight, int))):
         weight = 0.05
 
     #cast properties to list 
     if not (isinstance(properties, list)):
         properties = [properties]
     
     property_values = []
 
     #by default use properties (hydrphocity, hydrophilicty, residue mass),
-    #otherwise get the individual property values from aaindex1 using accession number
+    #otherwise get the individual property values from aaindex1 using accession numbers
     if (properties == []):
         property_values = [hydrophobicity_, hydrophilicity_, residue_mass_]
     else:
         for prop in properties:
             if (prop not in aaindex1.record_codes()):
                 raise ValueError('Accession number not found in aaindex1: {}.'.format(prop))
             property_values.append(aaindex1[prop].values)
@@ -307,15 +311,16 @@
     #append descriptor values to dict
     temp = 1 + weight * sum(rightpart)
     for index in range(20, 20 + lamda):
         psuedo_aac["PAAC_" + str(index + 1)] = round(
             weight * rightpart[index - 20] / temp * 100, 3)
 
     #transform values and columns to DataFrame
-    psuedo_amino_acid_composition_df = pd.DataFrame([list(psuedo_aac.values())], columns=list(psuedo_aac.keys()))
+    psuedo_amino_acid_composition_df = pd.DataFrame([list(psuedo_aac.values())], 
+        columns=list(psuedo_aac.keys()))
 
     return psuedo_amino_acid_composition_df 
 
 def sequence_order_correlation_factor(sequence, k=1, properties=[]):
     """
     Calculating sequence order correlation factor with gap equal to k based on
     the given input properities for a protein sequence.
@@ -410,15 +415,15 @@
     Parameters
     ----------
     :prop : dict
         dictionary of property values for each amino acid.
     :mean : float
         mean of physiochemical property values.
     :ddof : int (default=1)
-        delta degrees of freedom
+        delta degrees of freedom.
         
     Returns
     -------
     :std_ : float
         calculated standard deviation. 
     """
     temp = [math.pow(i - mean, 2) for i in prop]
@@ -426,28 +431,28 @@
     return std_
 
 ######################## Amphiphilic Pseudo Amino Acid Composition ########################
 
 def amphiphilic_pseudo_amino_acid_composition(sequence, lamda=30, weight=0.5, 
     properties=[hydrophobicity_, hydrophilicity_]):
     """
-    Amphiphillic pseudo amino acid composition has the same form as the amino
+    Amphiphillic pseudo amino acid composition (APAAComp) has the same form as the amino
     acid composition, but contains much more information that is related to the 
     sequence order of a protein and the distribution of the hydrophobic and 
     hydrophilic amino acids along its chain. The first 20 numbers in the 
     descriptor are the components of the conventional amino acid composition; 
     the next 2*λ numbers are a set of correlation factors that reflect different 
-    hydrophobicity and hydrophilicity distribution patterns along a protein chain
+    hydrophobicity and hydrophilicity distribution patterns along a protein chain [5].
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
     :lamda: int
-        rank of correlation. Number of calculable descriptors depends on lamda.
+        rank of correlation. Number of calculable descriptors depends on lambda value.
     :weight: float
         weighting factor.
     :properties : list (default=[hydrophobicity_, hydrophilicity_])
         list of dicts of physiochemical/structural property values for amino acids.
 
     Returns
     -------    
@@ -461,21 +466,21 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
-    #set lamda to its default value if <0, or > sequence len or not an int
+    #set lamda to its default value of 30 if <0, or > sequence len or not an int
     if ((lamda < 0) or (lamda > len(sequence)) or not isinstance(lamda, int)):
         lamda = 30  
 
-    #validate weight, set default weight if invalid value input
+    #validate weight, set default weight of 0.5 if invalid value input
     if ((weight<0) or not (isinstance(weight, float)) or not (isinstance(weight, int))):
         weight = 0.5
 
     #cast properties to list 
     if not (isinstance(properties, list)):
         properties = [properties]
 
@@ -491,15 +496,14 @@
     aa_composition = amino_acid_composition(sequence)
 
     #compute first 20 pseudo amino acid descriptor components based on properties
     temp = 1 + weight * rightpart
     for index, i in enumerate(amino_acids):
         amp_pseudo_amino_acid_composition["APAAC_" + str(index + 1)] = round(aa_composition[i].values[0] / temp, 3)
 
-
     #calculate correlation factor in protein sequence
     rightpart = []
     for i in range(lamda):
         temp = amphiphilic_sequence_order_correllation_factor(sequence, k=i + 1)
         rightpart.append(temp[0])
         rightpart.append(temp[1])
 
@@ -509,20 +513,19 @@
         amp_pseudo_amino_acid_composition["APAAC_" + str(index + 1)] = round(
             weight * rightpart[index - 20] / temp * 100, 3)
 
     #transform values and columns to DataFrame
     amp_pseudo_amino_acid_composition_df = pd.DataFrame([list(amp_pseudo_amino_acid_composition.values())], 
         columns=list(amp_pseudo_amino_acid_composition.keys()))
 
-
     return amp_pseudo_amino_acid_composition_df
 
 def amphiphilic_sequence_order_correllation_factor(sequence, k=1):
     """ 
-    Calculate Amphipilic sequence order correlation factor for sequence
+    Calculate Amphipillic sequence order correlation factor for sequence
     with gap=k.
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
     :k : int (default=1)
```

### Comparing `protpy-1.0.8/protpy/conjoint_triad.py` & `protpy-1.1.10/protpy/conjoint_triad.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,28 +39,28 @@
     :sequence : str
         protein sequence.
 
     Returns
     -------
     :conjoint_triad_df : pd.Dataframe
         pandas Dataframe of CTriad descriptor values for all protein sequences. Dataframe
-        will be of the shape 343 x 1, where 343 is the number of features calculated 
+        will be of the shape 1 x 343, where 343 is the number of features calculated 
         from the descriptor for a sequence.
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     conjoint_triad = {}
     _aa_triads = {}
 
     #expand aa_triads into form {AminoAcid: triad}
     for i in aa_triads:
         for j in aa_triads[i]:
```

### Comparing `protpy-1.0.8/protpy/ctd.py` & `protpy-1.1.10/protpy/ctd.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 """
 References
 ----------
 [1] Inna Dubchak, Ilya Muchink, Stephen R.Holbrook and Sung-Hou Kim.
     Prediction of protein folding class using global description of amino
     acid sequence. Proc.Natl. Acad.Sci.USA, 1995, 92, 8700-8704.
-
 [2] Inna Dubchak, Ilya Muchink, Christopher Mayor, Igor Dralyuk and Sung-Hou
     Kim. Recognition of a Protein Fold in the Context of the SCOP
     classification. Proteins: Structure, Function and
     Genetics, 1999, 35, 401-407.
 """
 
 hydrophobicity = {"name": "hydrophobicity", "1": "RKEDQN", "2": "GASTPHY", "3": "CLVIMFW"}
@@ -78,41 +77,46 @@
         raise TypeError('Input sequence must be a string, got input of type {}'.format(type(sequence)))
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
             raise ValueError("Invalid amino acid in protein sequence: {}".format(aa))
 
+    #create deep copy of sequence
     sequence_converted = copy.deepcopy(sequence)
 
     #convert amino acid into corresponding CTD keys
     for key, value in list(property.items()):
         if (key == "name"):
             continue
         for index in value:
             sequence_converted = sequence_converted.replace(index, key)
 
     return sequence_converted
 
+##################################### CTD Composition #####################################
+
 def ctd_composition(sequence, property="hydrophobicity"):
     """
-    Calculate composition physiochemical/structural descriptor.
+    Calculate composition physiochemical/structural descriptor. The shape of the
+    output will be 1 x 3, with 3 features being generated per sequence.
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
     :property : str (default="hydrophocity")
         physiochemical property name to use when calculating descriptor.
 
     Returns
     -------
     :ctd_composition_df : pd.DataFrame
         dataframe of calculated composition values for sequence using
-        selected physiochemical property.
+        selected physiochemical property. Output will be of shape 1 x 3,
+        with 3 features being generated per sequence.
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #uppercase protein sequence 
     sequence = sequence.upper()
@@ -142,30 +146,34 @@
     ctd_composition_['CTD_C_03_' + prop["name"]] = round(float(seq.count("3"))/len(sequence), 3)
 
     #transform values and columns to DataFrame
     ctd_composition_df = pd.DataFrame([list(ctd_composition_.values())], columns=list(ctd_composition_.keys()))
 
     return ctd_composition_df
 
+##################################### CTD Transition ######################################
+
 def ctd_transition(sequence, property="hydrophobicity"):
     """
-    Calculate transition physiochemical/structural descriptor.
+    Calculate transition physiochemical/structural descriptor. The shape of the
+    output will be 1 x 3, with 3 features being generated per sequence.
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
     :property : str (default="hydrophocity")
         physiochemical property name to use when calculating descriptor.
 
     Returns
     -------
     :ctd_transition_df : pd.DataFrame
         dataframe of calculated transition values for sequence using
-        selected physiochemical property.
+        selected physiochemical property. Output will be of shape 1 x 3,
+        with 3 features being generated per sequence.
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #uppercase protein sequence 
     sequence = sequence.upper()
@@ -198,30 +206,34 @@
         float(seq.count("23") + seq.count("32")) / (len(sequence)-1), 3)
 
     #transform values and columns to DataFrame
     ctd_transition_df = pd.DataFrame([list(ctd_transition_.values())], columns=list(ctd_transition_.keys()))
 
     return ctd_transition_df
 
+#################################### CTD Distribution #####################################
+
 def ctd_distribution(sequence, property="hydrophobicity"):
     """
-    Calculate distribution physiochemical/structural descriptor.
+    Calculate distribution physiochemical/structural descriptor. The shape of the
+    output will be 1 x 15, with 15 features being generated per sequence.
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
     :property : str (default="hydrophocity")
         physiochemical property name to use when calculating descriptor.
 
     Returns
     -------
     :ctd_distribution_df : pd.DataFrame
         dataframe of calculated distribution values for sequence using
-        selected physiochemical property.
+        selected physiochemical property. Output will be of shape 1 x 15,
+        with 15 features being generated per sequence.
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
@@ -279,41 +291,43 @@
     #transform values and columns to DataFrame
     ctd_distribution_df = pd.DataFrame([list(ctd_distribution_.values())], columns=list(ctd_distribution_.keys()))
 
     return ctd_distribution_df
 
 def ctd_(sequence, property="hydrophobicity", all_ctd=True):
     """
-    Calculate Composition, transition and distribution (CTD) features of protein sequences.
+    Calculate all Composition, Transition and Distribution (CTD) features of protein sequences.
     Composition is the number of amino acids of a particular property (e.g., hydrophobicity)
     divided by the total number of amino acids in a protein sequence. Transition
     characterizes the percent frequency with which amino acids of a particular
     property is followed by amino acids of a different property. Distribution
     measures the chain length within which the first, 25%, 50%, 75%, and 100% of
-    the amino acids of a particular property are located, respectively [6].
-    CTD properties used are: Polarizability, Solvent Accessibility, Secondary 
-    Structure, Charge, Polarity, Normalized VDWV, Hydrophobicity. The output 
-    will be of shape 1 x 147. 21/147 will be
-    composition, 21/147 will be transition and the remaining 105 are distribution.
+    the amino acids of a particular property are located, respectively [1, 2].
+    CTD properties available are: Polarizability, Solvent Accessibility, Secondary 
+    Structure, Charge, Polarity, Normalized VDWV, Hydrophobicity. Each property generates an 
+    output of shape 1 x 21, 3/21 will be Composition, 3/21 will be Transition, 15/21 will be
+    Distribution. When Calculating all available features the generated output will be of shape 
+    1 x 147, 21/147 will be composition, 21/147 will be transition and the remaining 105 are 
+    distribution.
     
     Parameters
     ----------
     :sequence : str
         protein sequence.
     :property : str (default="hydrophocity")
         physiochemical property name to use when calculating descriptor.
     :ctd : bool
         calculate all CTD descriptors and concatenate together.
 
     Returns
     -------
     :ctd_df : pd.DataFrame
         dataframe of CTD descriptor values for all protein sequences. DataFrame will
-        be of the shape 1 x 147, where 147 is the number of features calculated from t
-        he descriptors.
+        be of the shape 1 x 147, where 147 is the total number of features calculated from
+        the CTD descriptors, with each property generating an output of 1 x 21.
     """
     #check input sequence is a string, if not raise type error
     if not isinstance(sequence, str):
         raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
```

### Comparing `protpy-1.0.8/protpy/data/README.md` & `protpy-1.1.10/protpy/data/README.md`

 * *Files identical despite different names*

### Comparing `protpy-1.0.8/protpy/data/grantham-physiochemical-distance-matrix.json` & `protpy-1.1.10/protpy/data/grantham-physiochemical-distance-matrix.json`

 * *Files identical despite different names*

### Comparing `protpy-1.0.8/protpy/data/schneider-wrede-physiochemical-distance-matrix.json` & `protpy-1.1.10/protpy/data/schneider-wrede-physiochemical-distance-matrix.json`

 * *Files identical despite different names*

### Comparing `protpy-1.0.8/protpy/sequence_order.py` & `protpy-1.1.10/protpy/sequence_order.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,21 +28,23 @@
     doi:10.1126/science.185.4154.862. ISSN 0036-8075. PMID 4843792. S2CID 35388307.
 """
 
 #list of amino acids
 amino_acids = ["A", "C", "D", "E", "F", "G", "H", "I", "K", "L", "M", "N", "P", 
     "Q", "R", "S", "T", "V", "W", "Y"]
 
+############################# Sequence Order Coupling Number ##############################
+
 def sequence_order_coupling_number_(sequence, d=1, distance_matrix="schneider-wrede-physiochemical-distance-matrix"):
     """
     Calculate Sequence Order Coupling Number (SOCN) features for input protein sequence.
     SOCN computes the dissimilarity between amino acid pairs. The distance between 
     amino acid pairs is determined by d which varies between 1 to lag. For each d, it 
     computes the sum of the dissimilarities of all amino acid pairs. The output will be 
-    a single float value representing the SOCN.
+    a single float value representing the SOCN [1].
     
     This function should not be confused with sequence_order_coupling_number() below 
     which calculates the multiple SOCN descriptor values for the input sequence 
     according to the value of lag; with the default of lag=30, 30 SOCN's will be 
     calculated.
 
     Parameters
@@ -65,15 +67,15 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     #append extension if missing from input
     if (os.path.splitext(distance_matrix)[1] == ''):
         distance_matrix = distance_matrix + '.json'
     
     #get filepath to distance matrix json
     if not (os.path.isfile(distance_matrix)):
@@ -91,15 +93,15 @@
             distance_matrix = json.load(f)
     except:
         raise JSONDecodeError('Error getting config JSON file: {}.'.format(distance_matrix))
 
     tau = 0.0
 
     #iterate over length of sequence minus gap, incrementing the SOCN at each iteration using
-    # the values from the distance matrix with the current and next amino acid, round to 2 dp
+    #the values from the distance matrix with the current and next amino acid, round to 2 dp
     for aa in range(len(sequence) - d):
         current_aa = sequence[aa]
         next_aa = sequence[aa + d]
         tau = tau + math.pow(distance_matrix[current_aa + next_aa], 2)
 
     return round(tau, 3)
 
@@ -136,34 +138,34 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
     #raise value error if int cant be parsed from input lag
     try:
         lag = int(lag)
     except:
         raise ValueError("Invalid lag value input, integer cannot be parsed: {}.".format(lag))
 
-    #validate lag, set default lag if invalid value input
+    #validate lag, set default lag of 30 if invalid value input
     if (not (isinstance(lag, int) or int(lag)>=len(sequence) or (int(lag)<0))):
         lag = 30
 
     #set dataframe column name prefixes based on input distance matrix
     col_prefix = ""
     if (os.path.splitext(distance_matrix)[0] == "schneider-wrede-physiochemical-distance-matrix"):
         col_prefix = "SOCN_SW"
     elif (os.path.splitext(distance_matrix)[0] == "grantham-physiochemical-distance-matrix"):
         col_prefix = "SOCN_Grant"
 
-    #set default lag if invalid value input
+    #set default lag of 30 if invalid value input
     if (lag>=len(sequence) or (lag<0) or not (isinstance(lag, int))):
         lag = 30
 
     seq_order = {}
 
     #iterate over sequence with lag, calculating SOCN using input distance matrix values
     for i in range(lag):
@@ -176,15 +178,15 @@
     sequence_order_df = pd.DataFrame([list(seq_order.values())], columns=list(seq_order.keys()))
 
     return sequence_order_df
 
 def sequence_order_coupling_number_all(sequence, lag=30):
     """
     Calculate Sequence Order Coupling Number (SOCN) descriptor values of input protein 
-    sequence using both matrices (schneider-wrede & grantham). The distance between 
+    sequence using both matrices (schneider-wrede & grantham) [3]. The distance between 
     amino acid pairs is determined by d which varies between 1 to lag. For each d, it 
     computes the sum of the dissimilarities of all amino acid pairs. Each matrix generates
     an output of 1 x N, where N is the lag, so the concatenated output will be 1 x (N * 2).
     With a default lag of 30, this will generate an output of 1 x 60.
 
     Parameters
     ----------
@@ -210,52 +212,54 @@
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #raise value error if int cant be parsed from input lag
     try:
         lag = int(lag)
     except:
-        raise ValueError("Invalid lag value input, integer cannot be parsed: {}.".format(lag))
+        raise TypeError("Invalid lag value input, integer cannot be parsed: {}.".format(lag))
 
-    #validate lag, set default lag if invalid value input
+    #validate lag, set default lag of 30 if invalid value input
     if (lag>=len(sequence) or (lag<0) or not (isinstance(lag, int))):
         lag = 30
 
     #calculate SOCN using schneider-wrede distance matrix
     socn_schneider = sequence_order_coupling_number(sequence, lag, "schneider-wrede-physiochemical-distance-matrix.json")
     
     #calculate SOCN using grantham distance matrix
     socn_grantham = sequence_order_coupling_number(sequence, lag, "grantham-physiochemical-distance-matrix.json")
 
     #merge 2 dataframes 
     socn_all = pd.concat([socn_schneider, socn_grantham], axis=1)
 
     return socn_all
 
+################################## Quasi Sequence Order ###################################
+
 def quasi_sequence_order(sequence, lag=30, weight=0.1,
     distance_matrix="schneider-wrede-physiochemical-distance-matrix.json"):
     """
     Calculate Quasi Sequence Order (QSO) features for the protein sequences.
     The quasi-sequence-order descriptors were proposed by K.C. Chou, et.al. [1].
     They are derived from the distance matrix between the 20 amino acids. By default,
     the Scheider-Wrede physicochemical distance matrix was used. Also utilised in
     the descriptor calculation is the Grantham chemical distance matrix. Both of
     these matrices are used by Grantham et. al. in the calculation
-    of the descriptor [4]. N + 20 values are calculated per sequence, where N is the
+    of the descriptor [3, 4]. N + 20 values are calculated per sequence, where N is the
     lag, with a default lag of 30, the output will be 1 x 50.
 
     Parameters
     ----------
     :sequence : str
         protein sequence.
     :lag : int (default=30)
         maximum gap betwwen 2 amino acids; the length of the protein should be larger
         than lag. Default set to 30.
     :weight: float (default = 0.1)
-        weighting factor
+        weighting factor.
     :distance_matrix : str (default="schneider-wrede-physicochemical-distance-matrix")
         path to physiochemical distance matrix for calculating quasi sequence order.
 
     Returns
     -------
     :quasi_sequence_order_df : pd.Dataframe
         dataframe of quasi-sequence-order descriptor values for the protein sequences, 
@@ -268,27 +272,27 @@
 
     #uppercase protein sequence 
     sequence = sequence.upper()
 
     #if invalid amino acids in sequence, raise value error
     for aa in sequence:
         if (aa not in amino_acids):
-            raise ValueError("Invalid amino acid in protein sequence: .".format(aa))
+            raise ValueError("Invalid amino acid in protein sequence: {}.".format(aa))
 
-    #raise value error if int cant be parsed from input lag
+    #raise value error if int can't be parsed from input lag
     try:
         lag = int(lag)
     except:
         raise ValueError("Invalid lag value input, integer cannot be parsed: {}.".format(lag))
 
-    #validate lag, set default lag if invalid value input
+    #validate lag, set default lag of 30 if invalid value input
     if (lag>=len(sequence) or (lag<0) or not (isinstance(lag, int))):
         lag = 30
 
-    #validate weight, set default weight if invalid value input
+    #validate weight, set default weight of 0.1 if invalid value input
     if ((weight<0) or not (isinstance(lag, float)) or not (isinstance(lag, int))):
         weight = 0.1
 
     #set dataframe column name prefixes based on input distance matrix
     col_prefix = ""
     if (os.path.splitext(distance_matrix)[0] == "schneider-wrede-physiochemical-distance-matrix"):
         col_prefix = "QSO_SW"
@@ -305,28 +309,25 @@
 
     #get amino acid composition
     aa_comp = composition.amino_acid_composition(sequence)
 
     #iterate over amino acids, calculating descriptor value 
     temp = 1 + weight * right_part
     for index, aa in enumerate(amino_acids):
-        # quasi_sequence_order[col_prefix + "_1_" + str(index + 1)] = round(aa_comp[aa].values[0] / temp, 6)
         quasi_sequence_order[col_prefix + str(index + 1)] = round(aa_comp[aa].values[0] / temp, 6)
     
     #calculate SOCN up until maxlag
     _right_part = []
     for i in range(lag):
         _right_part.append(
             sequence_order_coupling_number_(sequence, i+1, distance_matrix))
 
     #calculate the last maxlag descriptor values
     temp = 1 + weight * sum(_right_part)
     for index in range(20, 20 + lag):
-        # quasi_sequence_order[col_prefix + "_2" + str(index + 1)] = round(
-        #     weight * right_part[index - 20] / temp, 6)
         quasi_sequence_order[col_prefix + str(index + 1)] = round(
             weight * _right_part[index - 20] / temp, 6)
     
     #transform descriptor data into pandas dataframe
     quasi_sequence_order_df = pd.DataFrame([list(quasi_sequence_order.values())], 
         columns=list(quasi_sequence_order.keys()))
     
@@ -354,24 +355,28 @@
     -------
     :quasi_sequence_order_all_df : pd.Dataframe
         dataframe of quasi-sequence-order descriptor values for the
         protein sequences, with output shape 1 x ((N + 20)*2) where ((N + 20)*2) is the 
         quasi sequence order output from one matrix and N is the lag. The output  
         is multiplied by two to take into account the 2 matrices being concatenated. 
     """
+    #check input sequence is a string, if not raise type error
+    if not isinstance(sequence, str):
+        raise TypeError('Input sequence must be a string, got input of type {}.'.format(type(sequence)))
+    
     #uppercase protein sequence 
     sequence = sequence.upper()
 
-    #raise value error if int cant be parsed from input lag
+    #raise value error if int can't be parsed from input lag
     try:
         lag = int(lag)
     except:
         raise ValueError("Invalid lag value input, integer cannot be parsed: {}.".format(lag))
 
-    #validate lag, set default lag if invalid value input
+    #validate lag, set default lag of 30 if invalid value input
     if (lag>=len(sequence) or (lag<0) or not (isinstance(lag, int))):
         lag = 30
 
     #validate weight, set default weight if invalid value input
     if ((weight<0) or not (isinstance(weight, float)) or not (isinstance(weight, int))):
         weight = 0.1
```

### Comparing `protpy-1.0.8/protpy.egg-info/PKG-INFO` & `protpy-1.1.10/protpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: protpy
-Version: 1.0.8
+Version: 1.1.10
 Summary: Python package for generating various biochemical, physiochemical and structural descriptors/features of protein sequences.
 Home-page: https://github.com/amckenna41/protPy
 Author: MIT
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/protPy/archive/refs/heads/main.zip
 Description: 
         # protpy - Package for generating protein physiochemical, biochemical and structural descriptors using their constituent amino acids. #
         [![PyPI](https://img.shields.io/pypi/v/protpy)](https://pypi.org/project/protpy/)
         [![pytest](https://github.com/amckenna41/protpy/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/protpy/actions?query=workflowBuilding%20and%20Testing)
         [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/protpy/)
         [![PythonV](https://img.shields.io/pypi/pyversions/protpy?logo=2)](https://pypi.org/project/protpy/)
         [![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://opensource.org/licenses/MIT)
-        <!-- [![Build](https://img.shields.io/github/workflow/status/amckenna41/protpy/Deploy%20to%20PyPI%20%F0%9F%93%A6)](https://github.com/amckenna41/protpy/actions) -->
-        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/pySAR.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/pySAR) -->
-        <!-- [![DOI](https://zenodo.org/badge/344290370.svg)](https://zenodo.org/badge/latestdoi/344290370) -->
-        <!-- [![codecov](https://codecov.io/gh/amckenna41/DCBLSTM_PSP/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/DCBLSTM_PSP) -->
         [![Issues](https://img.shields.io/github/issues/amckenna41/protpy)](https://github.com/amckenna41/protpy/issues)
         [![Size](https://img.shields.io/github/repo-size/amckenna41/protpy)](https://github.com/amckenna41/protpy)
         [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/protpy)](https://github.com/amckenna41/protpy)
-        
+        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/pySAR.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/pySAR) -->
+        <!-- [![DOI](https://zenodo.org/badge/344290370.svg)](https://zenodo.org/badge/latestdoi/344290370) -->
+        <!-- [![codecov](https://codecov.io/gh/amckenna41/DCBLSTM_PSP/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/DCBLSTM_PSP) -->
         <!-- <p align="center">
         <img src="https://images.newscientist.com/wp-content/uploads/2021/07/22155326/22-july_deepmind-proteome.jpg?width=300" alt="protpyLogo" height="200"/>
         </p> -->
         
         Table of Contents
         -----------------
```

### Comparing `protpy-1.0.8/protpy.egg-info/SOURCES.txt` & `protpy-1.1.10/protpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protpy-1.0.8/setup.cfg` & `protpy-1.1.10/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = protpy
-version = 1.0.8
+version = 1.1.10
 description = Python package for generating various biochemical, physiochemical and structural descriptors/features of protein sequences.
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/amckenna41/protpy
 download_url = https://github.com/amckenna41/protpy/archive/refs/heads/main.zip
@@ -45,14 +45,15 @@
 python_requires = >=3.6
 include_package_data = True
 install_requies = 
 	numpy
 	pandas
 	varname
 	aaindex
+	biopython
 
 [options.extras_require]
 test_suite = tests
 test = 
 	pytest
 	pytest-cov
 	pytest-flake8
```

### Comparing `protpy-1.0.8/setup.py` & `protpy-1.1.10/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 ###############################################################################
 #####   Setup.py - installs all the required packages and dependancies    #####
 ###############################################################################
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
-import protpy
 
 #ensure python version is greater than 3
 if (sys.version_info[0] < 3):
     sys.exit('Python 3 is the minimum version requirement.')
 
 #get path to README file
 HERE = pathlib.Path(__file__).parent
 README = (HERE / 'README.md').read_text()
 
-setup(name=protpy.__name__,
-      version=protpy.__version__,
-      description=protpy.__description__,
+#protPy package metadata
+__name__ = 'protpy'
+__version__ = "1.1.10"
+__description__ = "Python package for generating various biochemical, physiochemical and structural descriptors/features of protein sequences."
+__author__ = 'AJ McKenna, https://github.com/amckenna41'
+__authorEmail__ = 'amckenna41@qub.ac.uk'
+__maintainer__ = "AJ McKenna"
+__license__ = 'MIT'
+__url__ = 'https://github.com/amckenna41/protPy'
+__download_url__ = "https://github.com/amckenna41/protPy/archive/refs/heads/main.zip"
+__status__ = "Production"
+__keywords__ = ["bioinformatics", "protein engineering", "python", "pypi", "machine learning", \
+                "aaindex", "protein descriptors", "physiochemical descriptors", "biochemical descriptors"
+                "structural descriptors"]
+__test_suite__ = "tests"
+
+setup(name=__name__,
+      version=__version__,
+      description=__description__,
       long_description = README,
       long_description_content_type = "text/markdown",
-      author=protpy.__license__,
-      author_email=protpy.__authorEmail__,
-      maintainer=protpy.__maintainer__,
-      license=protpy.__license__,
-      url=protpy.__url__,
-      download_url=protpy.__download_url__,
-      keywords=protpy.__keywords__,
+      author=__license__,
+      author_email=__authorEmail__,
+      maintainer=__maintainer__,
+      license=__license__,
+      url=__url__,
+      download_url=__download_url__,
+      keywords=__keywords__,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Healthcare Industry',
         'Intended Audience :: Information Technology',
@@ -47,14 +62,15 @@
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development :: Libraries :: Python Modules'
       ],
       install_requires=[
         "aaindex",
         "numpy",
         "pandas",
-        "varname"
+        "varname",
+        "biopython"
       ],
-      test_suite=protpy.__test_suite__,
+      test_suite=__test_suite__,
       # packages=find_packages(), #create Manifest file to ignore results folder in dist
       packages=find_packages(),
       include_package_data=True,
       zip_safe=False)
```

### Comparing `protpy-1.0.8/tests/test_ctd.py` & `protpy-1.1.10/tests/test_ctd.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from Bio import SeqIO
 unittest.TestLoader.sortTestMethodsUsing = None
 import protpy as protpy
 
 class ProtPyCTDTests(unittest.TestCase):
     """
     Test suite for testing CTD (Composition, Transition, Distribution) 
-    module and functionality in protpy package. 
+    module and functionality in protpy package, including the CTD 
+    descriptors.
 
     Test Cases
     ----------
     test_ctd:
         testing correct protpy CTD functionality.
     test_ctd_composition:
         testing correct protpy composition functionality.
@@ -38,113 +39,151 @@
         
         with open(os.path.join("tests", "test_fasta3.fasta")) as pro:
             self.protein_seq3 = str(next(SeqIO.parse(pro,'fasta')).seq)
 
         with open(os.path.join("tests", "test_fasta4.fasta")) as pro:
             self.protein_seq4 = str(next(SeqIO.parse(pro,'fasta')).seq)
 
+        self.all_protein_seqs = [self.protein_seq1, self.protein_seq2, self.protein_seq3, self.protein_seq4]
+
     def test_ctd(self):
         """ Testing CTD descriptor attributes and functionality. """   
         properties = ["hydrophobicity", "normalized_vdwv", "polarity", "charge",
             "secondary_struct", "solvent_accessibility", "polarizability"]
  #1.)
-        ctd_seq1 = protpy.ctd_(self.protein_seq1,  all_ctd=True) #using all properties
+        for seq in self.all_protein_seqs:
+            ctd_seq1 = protpy.ctd_(seq, all_ctd=True) #using all properties
 
-        self.assertEqual(ctd_seq1.shape, (1, 147), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(ctd_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
-        self.assertTrue(ctd_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')  
-        self.assertTrue(all(col == np.float64 for col in list(ctd_seq1.dtypes)), "")
-        
-        #iterate over all columns, checking they follow naming convention using regex
-        for col in list(ctd_seq1.columns):
-            matching_col = False
-            for prop in properties:
-                if (col.endswith(prop)):
-                    matching_col = True
-                    self.assertTrue(((bool(re.search(r"CTD_[A-Z]_[0-9]{2}_" + prop, col))) or 
-                        (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{2}_" + prop, col))) or 
-                        (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{3}_" + prop, col)))), 
-                            "Column name does not follow expected format: {}.".format(col))
-            self.assertTrue(matching_col, "Column name's property name not found and doesn't match format: {}.".format(col))
-#2.)    
-        for prop in properties:
-            ctd_seq2 = protpy.ctd_(self.protein_seq2, property=prop, all_ctd=False) #using one property at a time
+            self.assertIsInstance(ctd_seq1, pd.DataFrame,
+                'Expected output to be a DataFrame, got {}.'.format(type(ctd_seq1)))
+            self.assertEqual(ctd_seq1.shape, (1, 147), 
+                'Expected output to be of shape {}, got {}.'.format((1, 147), ctd_seq1.shape)) 
+            self.assertTrue(ctd_seq1.any().isnull().sum()==0,
+                'Expected output to contain no null values.')        
+            self.assertTrue(all(col == np.float64 for col in list(ctd_seq1.dtypes)),
+                "Expected output values to be of datatype np.float64, got {}.".format(list(ctd_seq1.dtypes)))
 
-            self.assertEqual(ctd_seq2.shape, (1, 21), 'Descriptor not of correct shape.') 
-            self.assertIsInstance(ctd_seq2, pd.DataFrame, 'Descriptor not of type DataFrame.')
-            self.assertTrue(ctd_seq2.any().isnull().sum()==0, 'Descriptor should not contain any null values.')  
-            self.assertTrue(all(col == np.float64 for col in list(ctd_seq2.dtypes)), "")
-            
             #iterate over all columns, checking they follow naming convention using regex
-            for col in list(ctd_seq2.columns):
-                self.assertTrue(col.endswith(prop), "")
-                self.assertTrue(((bool(re.search(r"CTD_[A-Z]_[0-9]{2}_" + prop, col))) or 
-                    (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{2}_" + prop, col))) or 
-                    (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{3}_" + prop, col)))), 
-                        "Column name does not follow expected format: {}.".format(col))
+            for col in list(ctd_seq1.columns):
+                matching_col = False
+                for prop in properties:
+                    if (col.endswith(prop)):
+                        matching_col = True
+                        self.assertTrue(((bool(re.search(r"CTD_[A-Z]_[0-9]{2}_" + prop, col))) or 
+                            (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{2}_" + prop, col))) or 
+                            (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{3}_" + prop, col)))), 
+                                "Column name does not follow expected regex format: {}.".format(col))
+                self.assertTrue(matching_col, 
+                    "Column name {} not found in list of available properties:\n{}.".format(col, properties))
+#2.)    
+            for prop in properties:
+                ctd_seq2 = protpy.ctd_(seq, property=prop, all_ctd=False) #using one property at a time
+
+                self.assertIsInstance(ctd_seq2, pd.DataFrame,
+                    'Expected output to be a DataFrame, got {}.'.format(type(ctd_seq2)))
+                self.assertEqual(ctd_seq2.shape, (1, 21), 
+                    'Expected output to be of shape {}, got {}.'.format((1, 21), ctd_seq2.shape))
+                self.assertTrue(ctd_seq2.any().isnull().sum()==0,
+                    'Expected output to contain no null values.')        
+                self.assertTrue(all(col == np.float64 for col in list(ctd_seq2.dtypes)),
+                    "Expected output values to be of datatype np.float64, got {}.".format(list(ctd_seq2.dtypes)))
+
+                #iterate over all columns, checking they follow naming convention using regex
+                for col in list(ctd_seq2.columns):
+                    matching_col = False
+                    for prop in properties:
+                        if (col.endswith(prop)):
+                            matching_col = True
+                            self.assertTrue(((bool(re.search(r"CTD_[A-Z]_[0-9]{2}_" + prop, col))) or 
+                                (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{2}_" + prop, col))) or 
+                                (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{3}_" + prop, col)))), 
+                                    "Column name does not follow expected regex format: {}.".format(col))
+                    self.assertTrue(matching_col, 
+                        "Column name {} not found in list of available properties:\n{}.".format(col, properties))
 
     def test_ctd_composition(self):
         """ Testing CTD Composition descriptor attributes and functionality. """   
         properties = ["hydrophobicity", "normalized_vdwv", "polarity", "charge",
             "secondary_struct", "solvent_accessibility", "polarizability"]
 #1.)
-        for prop in properties:
-            ctd_composition_seq1 = protpy.ctd_composition(self.protein_seq1, property=prop)
+        for seq in self.all_protein_seqs:
+            for prop in properties:
+                ctd_composition_seq1 = protpy.ctd_composition(seq, property=prop)
 
-            self.assertEqual(ctd_composition_seq1.shape, (1, 3), 'Descriptor not of correct shape.') 
-            self.assertIsInstance(ctd_composition_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
-            self.assertTrue(ctd_composition_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')  
-            self.assertTrue(all(col == np.float64 for col in list(ctd_composition_seq1.dtypes)), "")
-            
-            #iterate over all columns, checking they follow naming convention using regex
-            for col in list(ctd_composition_seq1.columns):
-                matching_col = False
-                if (col.endswith(prop)):
-                    matching_col = True
-                    self.assertTrue((bool(re.search(r"CTD_[A-Z]_[0-9]{2}_" + prop, col))), 
-                        "Column name does not follow expected format: {}.".format(col))
-                self.assertTrue(matching_col, "Column name's property name not found and doesn't match format: {}.".format(col))
+                self.assertIsInstance(ctd_composition_seq1, pd.DataFrame,
+                    'Expected output to be a DataFrame, got {}.'.format(type(ctd_composition_seq1)))
+                self.assertEqual(ctd_composition_seq1.shape, (1, 3), 
+                    'Expected output to be of shape {}, got {}.'.format((1, 3), ctd_composition_seq1.shape)) 
+                self.assertTrue(ctd_composition_seq1.any().isnull().sum()==0,
+                    'Expected output to contain no null values.')        
+                self.assertTrue(all(col == np.float64 for col in list(ctd_composition_seq1.dtypes)),
+                    "Expected output values to be of datatype np.float64, got {}.".format(list(ctd_composition_seq1.dtypes)))
+
+                #iterate over all columns, checking they follow naming convention using regex
+                for col in list(ctd_composition_seq1.columns):
+                    matching_col = False
+                    for prop in properties:
+                        if (col.endswith(prop)):
+                            matching_col = True
+                            self.assertTrue(((bool(re.search(r"CTD_C_[0-9]{2}_" + prop, col))) or 
+                                (bool(re.search(r"CTD_C_[0-9]{2}_[0-9]{2}_" + prop, col))) or 
+                                (bool(re.search(r"CTD_C_[0-9]{2}_[0-9]{3}_" + prop, col)))), 
+                                    "Column name does not follow expected regex format: {}.".format(col))
+                    self.assertTrue(matching_col, 
+                        "Column name {} not found in list of available properties:\n{}.".format(col, properties))
 
-    def test_ctd_distribution(self):
-        """ Testing CTD Distribution descriptor attributes and functionality. """   
+    def test_ctd_transition(self):
+        """ Testing CTD Transition descriptor attributes and functionality. """   
         properties = ["hydrophobicity", "normalized_vdwv", "polarity", "charge",
             "secondary_struct", "solvent_accessibility", "polarizability"]
-#1.)
-        for prop in properties:
-            ctd_distribution_seq1 = protpy.ctd_distribution(self.protein_seq1, property=prop)
+#1.)    
+        for seq in self.all_protein_seqs:
+            for prop in properties:
+                ctd_transition_seq1 = protpy.ctd_transition(seq, property=prop)
 
-            self.assertEqual(ctd_distribution_seq1.shape, (1, 15), 'Descriptor not of correct shape.') 
-            self.assertIsInstance(ctd_distribution_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
-            self.assertTrue(ctd_distribution_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')  
-            self.assertTrue(all(col == np.float64 for col in list(ctd_distribution_seq1.dtypes)), "")
-            
-            #iterate over all columns, checking they follow naming convention using regex
-            for col in list(ctd_distribution_seq1.columns):
-                matching_col = False
-                if (col.endswith(prop)):
-                    matching_col = True
-                    self.assertTrue((bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{3}_" + prop, col))), 
-                        "Column name does not follow expected format: {}.".format(col))
-                self.assertTrue(matching_col, "Column name's property name not found and doesn't match format: {}.".format(col))
+                self.assertIsInstance(ctd_transition_seq1, pd.DataFrame, 
+                    'Expected output to be a DataFrame, got {}.'.format(type(ctd_transition_seq1)))
+                self.assertEqual(ctd_transition_seq1.shape, (1, 3), 
+                    'Expected output to be of shape {}, got {}.'.format((1, 3), ctd_transition_seq1.shape))
+                self.assertTrue(ctd_transition_seq1.any().isnull().sum()==0,
+                    'Expected output to contain no null values.')        
+                self.assertTrue(all(col == np.float64 for col in list(ctd_transition_seq1.dtypes)), 
+                    "Expected output values to be of datatype np.float64, got {}.".format(list(ctd_transition_seq1.dtypes)))
+#2.)
+                #iterate over all columns and check its name follows expected format
+                for col in list(ctd_transition_seq1.columns):
+                    matching_col = False
+                    if (col.endswith(prop)):
+                        matching_col = True
+                        self.assertTrue(((bool(re.search(r"CTD_T_[0-9]{2}_" + prop, col))) or 
+                            (bool(re.search(r"CTD_T_[0-9]{2}_[0-9]{2}_" + prop, col)))), 
+                                "Column name does not follow expected regex format: {}.".format(col))
+            self.assertTrue(matching_col, 
+                "Column name {} not found in list of available properties:\n{}.".format(col, properties))
 
-    def test_ctd_transition(self):
-        """ Testing CTD Transition descriptor attributes and functionality. """   
+    def test_ctd_distribution(self):
+        """ Testing CTD Distribution descriptor attributes and functionality. """   
         properties = ["hydrophobicity", "normalized_vdwv", "polarity", "charge",
             "secondary_struct", "solvent_accessibility", "polarizability"]
-#1.)    
-        for prop in properties:
-            ctd_transition_seq1 = protpy.ctd_transition(self.protein_seq1, property=prop)
+#1.)
+        for seq in self.all_protein_seqs:
+            for prop in properties:
+                ctd_distribution_seq1 = protpy.ctd_distribution(seq, property=prop)
 
-            self.assertEqual(ctd_transition_seq1.shape, (1, 3), 'Descriptor not of correct shape.') 
-            self.assertIsInstance(ctd_transition_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
-            self.assertTrue(ctd_transition_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')  
-            self.assertTrue(all(col == np.float64 for col in list(ctd_transition_seq1.dtypes)), "")
-            
-            #iterate over all columns and check its name follows expected format
-            for col in list(ctd_transition_seq1.columns):
-                matching_col = False
-                if (col.endswith(prop)):
-                    matching_col = True
-                    self.assertTrue(((bool(re.search(r"CTD_[A-Z]_[0-9]{2}_" + prop, col))) or 
-                        (bool(re.search(r"CTD_[A-Z]_[0-9]{2}_[0-9]{2}_" + prop, col)))), 
+                self.assertIsInstance(ctd_distribution_seq1, pd.DataFrame, 
+                    'Expected output to be a DataFrame, got {}.'.format(type(ctd_distribution_seq1)))
+                self.assertEqual(ctd_distribution_seq1.shape, (1, 15), 
+                    'Expected output to be of shape {}, got {}.'.format((1, 15), ctd_distribution_seq1.shape)) 
+                self.assertTrue(ctd_distribution_seq1.any().isnull().sum()==0,
+                    'Expected output to contain no null values.')        
+                self.assertTrue(all(col == np.float64 for col in list(ctd_distribution_seq1.dtypes)), 
+                    "Expected output values to be of datatype np.float64, got {}.".format(list(ctd_distribution_seq1.dtypes)))
+                
+                #iterate over all columns and check its name follows expected format
+                for col in list(ctd_distribution_seq1.columns):
+                    matching_col = False
+                    if (col.endswith(prop)):
+                        matching_col = True
+                        self.assertTrue(((bool(re.search(r"CTD_D_[0-9][0-9]_" + prop, col))) or (bool(re.search(r"CTD_D_[0-9]{2}_[0-9]{3}_" + prop, col)))), 
                             "Column name does not follow expected format: {}.".format(col))
-                self.assertTrue(matching_col, "Column name's property name not found and doesn't match format: {}.".format(col))
+            self.assertTrue(matching_col, 
+                "Column name {} not found in list of available properties:\n{}.".format(col, properties))
```

### Comparing `protpy-1.0.8/tests/test_protpy.py` & `protpy-1.1.10/tests/test_protpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         #list of canonical amino acids
         self.amino_acids = ["A", "C", "D", "E", "F", "G", "H", "I", "K", "L", "M", "N", "P", 
             "Q", "R", "S", "T", "V", "W", "Y"]
 
     def test_protpy_metadata(self):
         """ Testing correct protpy version and metadata. """
-        self.assertEqual(protpy.__version__, "1.0.8", 
+        self.assertEqual(protpy.__version__, "1.1.10", 
             "protpy version is not correct, got: {}".format(protpy.__version__))
         self.assertEqual(protpy.__name__, "protpy", 
             "protpy software name is not correct, got: {}".format(protpy.__name__))
         self.assertEqual(protpy.__author__, "AJ McKenna, https://github.com/amckenna41", 
             "protpy author is not correct, got: {}".format(protpy.__author__))
         self.assertEqual(protpy.__authorEmail__, "amckenna41@qub.ac.uk", 
             "protpy author email is not correct, got: {}".format(protpy.__authorEmail__))
@@ -66,15 +66,15 @@
 
     def test_valid_descriptors(self):
         """ Testing correct list of available descriptors is included in package attribute. """
         self.assertEqual(len(protpy.all_descriptors), 14, 
             "Expected there to be 14 total descriptors, got {}".format(len(protpy.all_descriptors)))
         self.assertIsInstance(protpy.all_descriptors, list, 
             "all_descriptors should be of type list, got {}.".format(type(protpy.all_descriptors)))
-        self.assertIn('aa_composition', protpy.all_descriptors, 
+        self.assertIn('amino_acid_composition', protpy.all_descriptors, 
             "aa_composition should be in available descriptors list.")
         self.assertIn('dipeptide_composition', protpy.all_descriptors, 
             "dipeptide_composition should be in available descriptors list.")
         self.assertIn('tripeptide_composition', protpy.all_descriptors,
             "tripeptide_composition should be in available descriptors list.")
         self.assertIn('pseudo_amino_acid_composition', protpy.all_descriptors,
             "pseudo_amino_acid_composition should be in available descriptors list.")
@@ -93,8 +93,8 @@
         self.assertIn('ctd_transition', protpy.all_descriptors,
             "ctd_transition should be in available descriptors list.")
         self.assertIn('ctd_distribution', protpy.all_descriptors,
             "ctd_distribution should be in available descriptors list.")
         self.assertIn('sequence_order_coupling_number', protpy.all_descriptors,
             "sequence_order_coupling_number should be in available descriptors list.")
         self.assertIn('quasi_sequence_order', protpy.all_descriptors,
-            "quasi_sequence_order should be in available descriptors list.")
+            "quasi_sequence_order should be in available descriptors list.")
```

### Comparing `protpy-1.0.8/tests/test_sequence_order.py` & `protpy-1.1.10/tests/test_sequence_order.py`

 * *Files 25% similar despite different names*

```diff
@@ -51,138 +51,169 @@
         with open(os.path.join("tests", "test_fasta4.fasta")) as pro:
             self.protein_seq4 = str(next(SeqIO.parse(pro,'fasta')).seq)
 
         self.distance_matrix_schneider_wrede = "schneider-wrede-physiochemical-distance-matrix"
         self.distance_matrix_grantham = "grantham-physiochemical-distance-matrix"
 
         #list of all test protein sequences
-        # self.all_seqs = [self.protein_seq1, self.protein_seq2, 
-        #     self.protein_seq3, self.protein_seq4]
+        # self.all_seqs = [self.protein_seq1, self.protein_seq2, self.protein_seq3, self.protein_seq4]
 
     def test_sequence_order_coupling_number_(self):
         """ Testing SOCN function that calculates the individial SOCN value. """
         lag = 15
 
         #expected outputs from SOCN function for 4 test sequences, using both matrices
         socn1_expected_grantham = [401.387, 409.243, 376.946, 393.042, 396.196, 384.772, 383.711, 
             391.951, 386.081, 386.139, 389.241, 393.244, 404.283, 385.307, 379.764]
         socn2_expected_grantham = [140.587, 142.97, 137.385, 139.629, 150.663, 145.954, 148.194, 
-            147.217, 153.02 ,153.583, 148.249, 151.87, 147.762, 141.598, 148.125]
+            147.217, 153.02, 153.583, 148.249, 151.87, 147.762, 141.598, 148.125]
         socn3_expected_grantham = [17.252, 16.808, 17.018, 16.892, 17.204, 15.861, 16.668, 12.764, 
             16.279, 13.025, 16.401, 14.546, 15.033, 14.816, 12.769]
-        socn4_expected_grantham = [138.258, 142.37, 137.803, 139.443, 148.422, 146.01 ,146.63, 
+        socn4_expected_grantham = [138.258, 142.37, 137.803, 139.443, 148.422, 146.01, 146.63, 
             149.337, 150.478, 148.856, 149.214, 154.144, 146.718, 139.508, 149.819]
 
         socn1_expected_sw = [401.387, 409.243, 376.946, 393.042, 396.196, 384.772, 383.711, 391.951, 
             386.081, 386.139, 389.241, 393.244, 404.283, 385.307, 379.764]
         socn2_expected_sw = [140.587, 142.97, 137.385, 139.629, 150.663, 145.954, 148.194, 147.217, 
             153.02, 153.583, 148.249, 151.87, 147.762, 141.598, 148.125]
         socn3_expected_sw = [17.252, 16.808, 17.018, 16.892, 17.204, 15.861, 16.668, 12.764, 16.279, 
             13.025, 16.401, 14.546, 15.033, 14.816, 12.769]
         socn4_expected_sw = [138.258, 142.37, 137.803, 139.443, 148.422, 146.01, 146.63, 149.337, 
             150.478, 148.856, 149.214, 154.144, 146.718, 139.508, 149.819]
 
         for i in range(lag):
 #1.)        #testing using schneider wrede distance matrix
             socn1_grantham = protpy.sequence_order_coupling_number_(self.protein_seq1, i+1, self.distance_matrix_schneider_wrede)
-            self.assertIsInstance(socn1_grantham, float, 'Descriptor should be of type float, got {}.'.format(type(socn1_grantham)))
-            self.assertEqual(socn1_grantham, socn1_expected_grantham[i], "Output from function doesnt match expected:\n {}".format(socn1_grantham))
+            self.assertIsInstance(socn1_grantham, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn1_grantham)))
+            self.assertEqual(socn1_grantham, socn1_expected_grantham[i], 
+                "Output from function doesnt match expected:\n{}".format(socn1_grantham))
 #2.)
             socn2_grantham = protpy.sequence_order_coupling_number_(self.protein_seq2, i+1, self.distance_matrix_schneider_wrede)
-            self.assertIsInstance(socn2_grantham, float, 'Descriptor should be of type float, got {}.'.format(type(socn2_grantham)))
-            self.assertEqual(socn2_grantham, socn2_expected_grantham[i], "Output from function doesnt match expected:\n {}".format(socn2_grantham))
+            self.assertIsInstance(socn2_grantham, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn2_grantham)))
+            self.assertEqual(socn2_grantham, socn2_expected_grantham[i], 
+                "Output from function doesnt match expected:\n{}".format(socn2_grantham))
 #3.)
             socn3_grantham = protpy.sequence_order_coupling_number_(self.protein_seq3, i+1, self.distance_matrix_schneider_wrede)
-            self.assertIsInstance(socn3_grantham, float, 'Descriptor should be of type float, got {}.'.format(type(socn3_grantham)))
-            self.assertEqual(socn3_grantham, socn3_expected_grantham[i], "Output from function doesnt match expected:\n {}".format(socn3_grantham))
+            self.assertIsInstance(socn3_grantham, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn3_grantham)))
+            self.assertEqual(socn3_grantham, socn3_expected_grantham[i], 
+                "Output from function doesnt match expected:\n{}".format(socn3_grantham))
 #4.)
             socn4_grantham = protpy.sequence_order_coupling_number_(self.protein_seq4, i+1, self.distance_matrix_schneider_wrede)
-            self.assertIsInstance(socn4_grantham, float, 'Descriptor should be of type float, got {}.'.format(type(socn4_grantham)))
-            self.assertEqual(socn4_grantham, socn4_expected_grantham[i], "Output from function doesnt match expected:\n {}".format(socn4_grantham))
-
+            self.assertIsInstance(socn4_grantham, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn4_grantham)))
+            self.assertEqual(socn4_grantham, socn4_expected_grantham[i], 
+                "Output from function doesnt match expected:\n {}".format(socn4_grantham))
 #5.)        #testing using grantham distance matrix
             socn1_sw = protpy.sequence_order_coupling_number_(self.protein_seq1, i+1, self.distance_matrix_grantham)
-            self.assertIsInstance(socn1_sw, float, 'Descriptor should be of type float, got {}.'.format(type(socn1_sw)))
-            self.assertEqual(socn1_sw, socn1_expected_sw[i], "Output from function doesnt match expected:\n {}".format(socn1_sw))
+            self.assertIsInstance(socn1_sw, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn1_sw)))
+            self.assertEqual(socn1_sw, socn1_expected_sw[i], 
+                "Output from function doesnt match expected:\n{}".format(socn1_sw))
 #6.)
             socn2_sw = protpy.sequence_order_coupling_number_(self.protein_seq2, i+1, self.distance_matrix_grantham)
-            self.assertIsInstance(socn2_sw, float, 'Descriptor should be of type float, got {}.'.format(type(socn2_sw)))
-            self.assertEqual(socn2_sw, socn2_expected_sw[i], "Output from function doesnt match expected:\n {}".format(socn2_sw))
+            self.assertIsInstance(socn2_sw, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn2_sw)))
+            self.assertEqual(socn2_sw, socn2_expected_sw[i], 
+                "Output from function doesnt match expected:\n{}".format(socn2_sw))
 #7.)
             socn3_sw = protpy.sequence_order_coupling_number_(self.protein_seq3, i+1, self.distance_matrix_grantham)
-            self.assertIsInstance(socn3_sw, float, 'Descriptor should be of type float, got {}.'.format(type(socn3_sw)))
-            self.assertEqual(socn3_sw, socn3_expected_sw[i], "Output from function doesnt match expected:\n {}".format(socn3_sw))
+            self.assertIsInstance(socn3_sw, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn3_sw)))
+            self.assertEqual(socn3_sw, socn3_expected_sw[i], 
+                "Output from function doesnt match expected:\n{}".format(socn3_sw))
 #8.)
             socn4_sw = protpy.sequence_order_coupling_number_(self.protein_seq4, i+1, self.distance_matrix_grantham)
-            self.assertIsInstance(socn4_sw, float, 'Descriptor should be of type float, got {}.'.format(type(socn4_sw)))
-            self.assertEqual(socn4_sw, socn4_expected_sw[i], "Output from function doesnt match expected:\n {}".format(socn4_sw))
+            self.assertIsInstance(socn4_sw, float, 
+                'Expected descriptor to be of type float, got {}.'.format(type(socn4_sw)))
+            self.assertEqual(socn4_sw, socn4_expected_sw[i], 
+                "Output from function doesnt match expected:\n{}".format(socn4_sw))
 #9.)
             invalid_seq5 = "ABCDEF"
             with (self.assertRaises(ValueError)):
                 socn_seq5 = protpy.sequence_order_coupling_number_(invalid_seq5, i+1, 
                     distance_matrix=self.distance_matrix_schneider_wrede)
 #10.)
             invalid_seq6 = "OOOOO"
             with (self.assertRaises(ValueError)):
                 socn_seq6 = protpy.sequence_order_coupling_number_(invalid_seq6, i+1, 
                     distance_matrix=self.distance_matrix_grantham)
+#11.)
+            invalid_seq7 = 1234
+            with (self.assertRaises(TypeError)):
+                socn_seq6 = protpy.sequence_order_coupling_number_(invalid_seq7, i+1, 
+                    distance_matrix=self.distance_matrix_grantham)
 
     def test_sequence_order_coupling_number(self):
         """ Testing sequence order coupling number descriptor attributes and functionality. """
 #1.)
         socn_seq1 = protpy.sequence_order_coupling_number(self.protein_seq1, lag=5, 
             distance_matrix=self.distance_matrix_schneider_wrede)
 
-        self.assertEqual(socn_seq1.shape, (1, 5), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(socn_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_seq1, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_seq1)))
+        self.assertEqual(socn_seq1.shape, (1, 5), 
+            'Expected output to be of shape {}, got {}.'.format((1, 5), socn_seq1.shape)) 
         for col in list(socn_seq1.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_seq1.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_seq1.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_seq1.dtypes)))
 #2.)
         socn_seq2 = protpy.sequence_order_coupling_number(self.protein_seq2, lag=10, 
             distance_matrix=self.distance_matrix_schneider_wrede)
 
-        self.assertEqual(socn_seq2.shape, (1, 10), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(socn_seq2, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_seq2, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_seq2)))
+        self.assertEqual(socn_seq2.shape, (1, 10), 
+            'Expected output to be of shape {}, got {}.'.format((1, 10), socn_seq2.shape)) 
         for col in list(socn_seq2.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_seq2.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_seq2.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_seq2.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_seq2.dtypes)))
 #3.)
         socn_seq3 = protpy.sequence_order_coupling_number(self.protein_seq3, lag=15, 
             distance_matrix=self.distance_matrix_schneider_wrede)
 
-        self.assertEqual(socn_seq3.shape, (1, 15), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(socn_seq3, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_seq3, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_seq3)))
+        self.assertEqual(socn_seq3.shape, (1, 15), 
+            'Expected output to be of shape {}, got {}.'.format((1, 15), socn_seq3.shape)) 
         for col in list(socn_seq3.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_seq3.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_seq3.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_seq3.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_seq3.dtypes)))
 #4.)
         invalid_lag = 500 #greater than len of protein sequence
         socn_seq4 = protpy.sequence_order_coupling_number(self.protein_seq4, lag=invalid_lag, 
             distance_matrix=self.distance_matrix_schneider_wrede)
 
-        self.assertEqual(socn_seq4.shape, (1, 30), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(socn_seq4, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_seq4, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_seq4)))
+        self.assertEqual(socn_seq4.shape, (1, 30), 
+            'Expected output to be of shape {}, got {}.'.format((1, 30), socn_seq4.shape)) 
         for col in list(socn_seq4.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_seq4.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_seq4.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_seq4.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_seq4.dtypes)))
 #5.)
         invalid_seq5 = "ABCDEF"
         with (self.assertRaises(ValueError)):
             socn_seq5 = protpy.sequence_order_coupling_number(invalid_seq5, lag=10, 
                 distance_matrix=self.distance_matrix_schneider_wrede)
@@ -192,133 +223,177 @@
             socn_seq6 = protpy.sequence_order_coupling_number(invalid_seq6, lag=10, 
                 distance_matrix=self.distance_matrix_schneider_wrede)
 #7.)
         invalid_lag = "BLAHBLAH"
         with (self.assertRaises(ValueError)):
             socn_seq7 = protpy.sequence_order_coupling_number(self.protein_seq4, lag=invalid_lag, 
                 distance_matrix=self.distance_matrix_schneider_wrede)
+#8.)
+        invalid_seq7 = 12345
+        with (self.assertRaises(TypeError)):
+            socn_seq7 = protpy.sequence_order_coupling_number(invalid_seq7, lag=10, 
+                distance_matrix=self.distance_matrix_schneider_wrede)
 
     def test_sequence_order_coupling_number_all(self):
         """ Testing function that calculates SOCN using both matrices for a sequence and lag. """
 #1.)
         lag = 30
         socn_all_seq1 = protpy.sequence_order_coupling_number_all(self.protein_seq1, lag=lag)
 
-        self.assertEqual(socn_all_seq1.shape, (1, lag*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(socn_all_seq1.shape)) 
-        self.assertIsInstance(socn_all_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_all_seq1, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_all_seq1)))
+        self.assertEqual(socn_all_seq1.shape, (1, lag*2), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag*2), socn_all_seq1.shape))
         for col in list(socn_all_seq1.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col)) or
                 bool(re.match(r'SOCN_Grant[0-9]', col)) or bool(re.match(r'SOCN_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_all_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_all_seq1.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_all_seq1.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_all_seq1.dtypes)))
 #2.)
         lag = 15
         socn_all_seq2 = protpy.sequence_order_coupling_number_all(self.protein_seq2, lag=lag)
 
-        self.assertEqual(socn_all_seq2.shape, (1, lag*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(socn_all_seq2.shape)) 
-        self.assertIsInstance(socn_all_seq2, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_all_seq2, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_all_seq2)))
+        self.assertEqual(socn_all_seq2.shape, (1, lag*2), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag*2), socn_all_seq2.shape))
         for col in list(socn_all_seq2.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col)) or
                 bool(re.match(r'SOCN_Grant[0-9]', col)) or bool(re.match(r'SOCN_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_all_seq2.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_all_seq2.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_all_seq2.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_all_seq2.dtypes)))
 #3.)
         lag = 10
         socn_all_seq3 = protpy.sequence_order_coupling_number_all(self.protein_seq3, lag=lag)
 
-        self.assertEqual(socn_all_seq3.shape, (1, lag*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(socn_all_seq3.shape)) 
-        self.assertIsInstance(socn_all_seq3, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_all_seq3, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_all_seq3)))
+        self.assertEqual(socn_all_seq3.shape, (1, lag*2), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag*2), socn_all_seq3.shape)) 
         for col in list(socn_all_seq3.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col)) or
                 bool(re.match(r'SOCN_Grant[0-9]', col)) or bool(re.match(r'SOCN_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_all_seq3.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_all_seq3.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_all_seq3.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_all_seq3.dtypes)))
 #4.)
         lag = 5
         socn_all_seq4 = protpy.sequence_order_coupling_number_all(self.protein_seq4, lag=lag)
 
-        self.assertEqual(socn_all_seq4.shape, (1, lag*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(socn_all_seq4.shape)) 
-        self.assertIsInstance(socn_all_seq4, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(socn_all_seq4, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(socn_all_seq4)))
+        self.assertEqual(socn_all_seq4.shape, (1, lag*2), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag*2), socn_all_seq4.shape))
         for col in list(socn_all_seq4.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'SOCN_SW[0-9]', col)) or bool(re.match(r'SOCN_SW[0-9][0-9]', col)) or
                 bool(re.match(r'SOCN_Grant[0-9]', col)) or bool(re.match(r'SOCN_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(socn_all_seq4.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(socn_all_seq4.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(socn_all_seq4.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(socn_all_seq4.dtypes)))
+#5.)
+        invalid_seq5 = "ABCDEF"
+        with (self.assertRaises(ValueError)):
+            socn_all_seq5 = protpy.sequence_order_coupling_number_all(invalid_seq5, lag=lag)
+#6.)
+        invalid_seq6 = "OOOOO"
+        with (self.assertRaises(ValueError)):
+            socn_all_seq6 = protpy.sequence_order_coupling_number_all(invalid_seq6, lag=lag)
+#7.)
+        invalid_seq7 = 1234
+        with (self.assertRaises(TypeError)):
+            socn_all_seq7 = protpy.sequence_order_coupling_number_all(invalid_seq7, lag=lag)
+#8.)
+        invalid_lag = "BLAHBLAH"
+        with (self.assertRaises(TypeError)):
+            socn_all_seq8 = protpy.sequence_order_coupling_number_all(invalid_seq7, lag=invalid_lag)
 
     def test_quasi_sequence_order(self):
         """ Testing quasi sequence order descriptor attributes and functionality. """
 #1.)    #testing using distance_matrix_schneider_wrede distance matrix
         lag = 30
         quasi_sequence_order_seq1 = protpy.quasi_sequence_order(self.protein_seq1, lag=lag, 
             distance_matrix=self.distance_matrix_schneider_wrede)
         
-        self.assertEqual(quasi_sequence_order_seq1.shape, (1, lag+20), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(quasi_sequence_order_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(quasi_sequence_order_seq1, pd.DataFrame,
+            'Expected output to be a DataFrame, got {}.'.format(type(quasi_sequence_order_seq1)))
+        self.assertEqual(quasi_sequence_order_seq1.shape, (1, lag+20), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag+20), quasi_sequence_order_seq1.shape)) 
         for col in list(quasi_sequence_order_seq1.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(quasi_sequence_order_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(quasi_sequence_order_seq1.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(quasi_sequence_order_seq1.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(quasi_sequence_order_seq1.dtypes)))
 #2.)
         lag = 20
         quasi_sequence_order_seq2 = protpy.quasi_sequence_order(self.protein_seq2, lag=lag, 
             distance_matrix=self.distance_matrix_schneider_wrede)
         
-        self.assertEqual(quasi_sequence_order_seq2.shape, (1, lag+20), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(quasi_sequence_order_seq2, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(quasi_sequence_order_seq2, pd.DataFrame,
+            'Expected output to be a DataFrame, got {}.'.format(type(quasi_sequence_order_seq2)))
+        self.assertEqual(quasi_sequence_order_seq2.shape, (1, lag+20), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag+20), quasi_sequence_order_seq2.shape)) 
         for col in list(quasi_sequence_order_seq2.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col))), 
-                "Column name doesn't match expected regex pattern: {}.".format(col))      
-        self.assertTrue(quasi_sequence_order_seq2.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+                "Column name doesn't match expected regex pattern: {}.".format(col))     
+        self.assertTrue(quasi_sequence_order_seq2.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(quasi_sequence_order_seq2.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(quasi_sequence_order_seq2.dtypes)))
 #3.)
         lag = 10
         quasi_sequence_order_seq3 = protpy.quasi_sequence_order(self.protein_seq3, lag=lag, 
             distance_matrix=self.distance_matrix_schneider_wrede)
 
-        self.assertEqual(quasi_sequence_order_seq3.shape, (1, lag+20), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(quasi_sequence_order_seq3, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(quasi_sequence_order_seq3, pd.DataFrame,
+            'Expected output to be a DataFrame, got {}.'.format(type(quasi_sequence_order_seq3)))
+        self.assertEqual(quasi_sequence_order_seq3.shape, (1, lag+20), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag+20), quasi_sequence_order_seq3.shape)) 
         for col in list(quasi_sequence_order_seq3.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col))), 
-                "Column name doesn't match expected regex pattern: {}.".format(col))      
-        self.assertTrue(quasi_sequence_order_seq3.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+                "Column name doesn't match expected regex pattern: {}.".format(col))     
+        self.assertTrue(quasi_sequence_order_seq3.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(quasi_sequence_order_seq3.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(quasi_sequence_order_seq3.dtypes)))
 #4.)
         lag = 5
         quasi_sequence_order_seq4 = protpy.quasi_sequence_order(self.protein_seq4, lag=lag, 
             distance_matrix=self.distance_matrix_schneider_wrede)
 
-        self.assertEqual(quasi_sequence_order_seq4.shape, (1, lag+20), 'Descriptor not of correct shape.') 
-        self.assertIsInstance(quasi_sequence_order_seq4, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(quasi_sequence_order_seq4, pd.DataFrame,
+            'Expected output to be a DataFrame, got {}.'.format(type(quasi_sequence_order_seq4)))
+        self.assertEqual(quasi_sequence_order_seq4.shape, (1, lag+20), 
+            'Expected output to be of shape {}, got {}.'.format((1, lag+20), quasi_sequence_order_seq4.shape)) 
         for col in list(quasi_sequence_order_seq4.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col))), 
-                "Column name doesn't match expected regex pattern: {}.".format(col))      
-        self.assertTrue(quasi_sequence_order_seq4.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+                "Column name doesn't match expected regex pattern: {}.".format(col))     
+        self.assertTrue(quasi_sequence_order_seq4.any().isnull().sum()==0, 
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(quasi_sequence_order_seq4.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(quasi_sequence_order_seq4.dtypes)))
-
 #5.)
         invalid_seq4 = "ABCDEF"
         with (self.assertRaises(ValueError)):
             quasi_sequence_order_seq5 = protpy.quasi_sequence_order(invalid_seq4, lag=30, 
                 distance_matrix=self.distance_matrix_schneider_wrede)
 #6.)
         invalid_seq5 = "OOOOO"
@@ -326,65 +401,98 @@
             quasi_sequence_order_seq6 = protpy.quasi_sequence_order(invalid_seq5, lag=10, 
                 distance_matrix=self.distance_matrix_schneider_wrede)
 #7.)
         invalid_lag = "BLAHBLAH"
         with (self.assertRaises(ValueError)):
             quasi_sequence_order_seq7 = protpy.quasi_sequence_order(self.protein_seq4, lag=invalid_lag, 
                 distance_matrix=self.distance_matrix_schneider_wrede)
+#8.)
+        invalid_seq6 = 1234
+        with (self.assertRaises(TypeError)):
+            quasi_sequence_order_seq6 = protpy.quasi_sequence_order(invalid_seq6, lag=20, 
+                distance_matrix=self.distance_matrix_schneider_wrede)
 
     def test_quasi_sequence_order_all(self):
         """ Testing function that calculates QSO using both matrices for a sequence and lag. """
         lag = 30
         qso_all_seq1 = protpy.quasi_sequence_order_all(self.protein_seq1, lag=lag)
 #1.)
-        self.assertEqual(qso_all_seq1.shape, (1, (lag+20)*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(qso_all_seq1.shape)) 
-        self.assertIsInstance(qso_all_seq1, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(qso_all_seq1, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(qso_all_seq1)))
+        self.assertEqual(qso_all_seq1.shape, (1, (lag+20)*2),
+            'Expected output to be of shape {}, got {}.'.format((1, (lag+20)*2), qso_all_seq1.shape)) 
         for col in list(qso_all_seq1.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col)) or
                 bool(re.match(r'QSO_Grant[0-9]', col)) or bool(re.match(r'QSO_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(qso_all_seq1.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(qso_all_seq1.any().isnull().sum()==0,
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(qso_all_seq1.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(qso_all_seq1.dtypes)))
 #2.)
         lag = 15
         qso_all_seq2 = protpy.quasi_sequence_order_all(self.protein_seq2, lag=lag)
 
-        self.assertEqual(qso_all_seq2.shape, (1, (lag+20)*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(qso_all_seq2.shape)) 
-        self.assertIsInstance(qso_all_seq2, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(qso_all_seq2, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(qso_all_seq2)))
+        self.assertEqual(qso_all_seq2.shape, (1, (lag+20)*2),
+            'Expected output to be of shape {}, got {}.'.format((1, (lag+20)*2), qso_all_seq2.shape)) 
         for col in list(qso_all_seq2.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col)) or
                 bool(re.match(r'QSO_Grant[0-9]', col)) or bool(re.match(r'QSO_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(qso_all_seq2.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(qso_all_seq2.any().isnull().sum()==0,
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(qso_all_seq2.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(qso_all_seq2.dtypes)))
 #3.)
         lag = 10
         qso_all_seq3 = protpy.quasi_sequence_order_all(self.protein_seq3, lag=lag)
 
-        self.assertEqual(qso_all_seq3.shape, (1, (lag+20)*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(qso_all_seq3.shape)) 
-        self.assertIsInstance(qso_all_seq3, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(qso_all_seq3, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(qso_all_seq3)))
+        self.assertEqual(qso_all_seq3.shape, (1, (lag+20)*2),
+            'Expected output to be of shape {}, got {}.'.format((1, (lag+20)*2), qso_all_seq3.shape)) 
         for col in list(qso_all_seq3.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col)) or
                 bool(re.match(r'QSO_Grant[0-9]', col)) or bool(re.match(r'QSO_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(qso_all_seq3.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(qso_all_seq3.any().isnull().sum()==0,
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(qso_all_seq3.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(qso_all_seq3.dtypes)))
 #4.)
         lag = 5
         qso_all_seq4 = protpy.quasi_sequence_order_all(self.protein_seq4, lag=lag)
 
-        self.assertEqual(qso_all_seq4.shape, (1, (lag+20)*2), 'Descriptor not of correct shape, expected (1, 60), got {}.'.format(qso_all_seq4.shape)) 
-        self.assertIsInstance(qso_all_seq4, pd.DataFrame, 'Descriptor not of type DataFrame.')
+        self.assertIsInstance(qso_all_seq4, pd.DataFrame, 
+            'Expected output to be a DataFrame, got {}.'.format(type(qso_all_seq4)))
+        self.assertEqual(qso_all_seq4.shape, (1, (lag+20)*2),
+            'Expected output to be of shape {}, got {}.'.format((1, (lag+20)*2), qso_all_seq4.shape)) 
         for col in list(qso_all_seq4.columns):
             #check all columns follow pattern of SOCNX or SOCNXY where x & y integers between 0 and 9
             self.assertTrue((bool(re.match(r'QSO_SW[0-9]', col)) or bool(re.match(r'QSO_SW[0-9][0-9]', col)) or
                 bool(re.match(r'QSO_Grant[0-9]', col)) or bool(re.match(r'QSO_Grant[0-9][0-9]', col))), 
                 "Column name doesn't match expected regex pattern: {}.".format(col))     
-        self.assertTrue(qso_all_seq4.any().isnull().sum()==0, 'Descriptor should not contain any null values.')
+        self.assertTrue(qso_all_seq4.any().isnull().sum()==0,
+            'Expected output to contain no null values.')        
         self.assertTrue(all(col == np.float64 for col in list(qso_all_seq4.dtypes)), 
             "Descriptor dataframe dtypes expected to be np.float64, got {}.".format(list(qso_all_seq4.dtypes)))
+#5.)
+        invalid_seq5 = "ABCDEF"
+        with (self.assertRaises(ValueError)):
+            quasi_sequence_order_seq5 = protpy.quasi_sequence_order_all(invalid_seq5, lag=30) 
+#6.)
+        invalid_seq6 = "OOOOO"
+        with (self.assertRaises(ValueError)):
+            quasi_sequence_order_seq6 = protpy.quasi_sequence_order_all(invalid_seq6, lag=30) 
+#7.)
+        invalid_seq7 = "BLAHBLAH"
+        with (self.assertRaises(ValueError)):
+            quasi_sequence_order_seq7 = protpy.quasi_sequence_order_all(invalid_seq7, lag=30) 
+#8.)
+        invalid_seq8 = 1234
+        with (self.assertRaises(TypeError)):
+            quasi_sequence_order_seq8 = protpy.quasi_sequence_order_all(invalid_seq8, lag=30)
```

