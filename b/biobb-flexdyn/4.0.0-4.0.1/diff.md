# Comparing `tmp/biobb_flexdyn-4.0.0.tar.gz` & `tmp/biobb_flexdyn-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_flexdyn-4.0.0.tar", last modified: Tue Apr 11 14:35:38 2023, max compression
+gzip compressed data, was "dist/biobb_flexdyn-4.0.1.tar", last modified: Wed Apr 12 15:47:58 2023, max compression
```

## Comparing `biobb_flexdyn-4.0.0.tar` & `biobb_flexdyn-4.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1004 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5623 2023-04-11 14:26:22.000000 biobb_flexdyn-4.0.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       66 2023-04-11 14:26:05.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      111 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15390 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/concoord_disco.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10851 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/concoord_dist.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5556 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/imod_imode.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6315 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/imod_imove.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6903 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/nolb_nma.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6197 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/prody_anm.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1004 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      530 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      332 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       14 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 14:35:38.000000 biobb_flexdyn-4.0.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1803 2023-04-11 14:25:50.000000 biobb_flexdyn-4.0.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.1/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1004 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5623 2023-04-12 15:46:02.000000 biobb_flexdyn-4.0.1/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       67 2023-04-12 15:45:49.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      128 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15411 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_disco.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11996 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_dist.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6914 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imc.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5537 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imode.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6228 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imove.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6927 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/nolb_nma.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6114 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/prody_anm.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1004 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      564 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      379 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       14 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-12 15:47:58.000000 biobb_flexdyn-4.0.1/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1865 2023-04-12 15:45:38.000000 biobb_flexdyn-4.0.1/setup.py
```

### Comparing `biobb_flexdyn-4.0.0/LICENSE` & `biobb_flexdyn-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.0/PKG-INFO` & `biobb_flexdyn-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_flexdyn
-Version: 4.0.0
+Version: 4.0.1
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexdyn-4.0.0/README.md` & `biobb_flexdyn-4.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_flexdyn?label=Version)](https://GitHub.com/bioexcel/biobb_flexdyn/tags/)
 [![](https://img.shields.io/pypi/v/biobb-flexdyn.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-flexdyn/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_flexdyn?label=Conda)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_flexdyn?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_flexdyn?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_flexdyn)
 [![](https://img.shields.io/pypi/pyversions/biobb-flexdyn.svg?label=Python%20Versions)](https://pypi.org/project/biobb-flexdyn/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_flexdyn)
 
 [![](https://readthedocs.org/projects/biobb-flexdyn/badge/?version=latest&label=Docs)](https://biobb-flexdyn.readthedocs.io/en/latest/?badge=latest)
@@ -30,60 +30,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_flexdyn.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_flexdyn>=4.0.0"
+        pip install "biobb_flexdyn>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_flexdyn>=4.0.0"
+        conda install -c bioconda "biobb_flexdyn>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-flexdyn.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_flexdyn:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_flexdyn:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_flexdyn:4.0.0--pyhdfd78af_0
+        docker run quay.io/biocontainers/biobb_flexdyn:4.0.1--pyhdfd78af_0
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.0--pyhdfd78af_0
+        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_flexdyn.sif <command>
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/concoord_disco.py` & `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_disco.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 
 """Module containing the concoord_disco class and the command line interface."""
-import argparse, os, shutil
+import argparse
+import os
+import shutil
 from pathlib import Path
 from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class ConcoordDisco(BiobbObject):
     """
     | biobb_flexdyn ConcoordDisco
     | Wrapper of the Disco tool from the Concoord package.
     | Structure generation based on a set of geometric constraints extracted with the Concoord Dist tool.
 
     Args:
@@ -21,29 +24,29 @@
         output_rmsd_path (str): Output rmsd file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/disco_rmsd.dat>`_. Accepted formats: dat (edam:format_1637).
         output_bfactor_path (str): Output B-factor file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/disco_bfactor.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **binary_path** (*str*) - ("disco") Concoord disco binary path to be used.
             * **vdw** (*int*) - (1) Select a set of Van der Waals parameters. Values: 1 (OPLS-UA -united atoms- parameters), 2 (OPLS-AA -all atoms- parameters), 3 (PROLSQ repel parameters), 4 (Yamber2 parameters), 5 (Li et al. parameters), 6 (OPLS-X parameters -recommended for NMR structure determination-)
             * **num_structs** (*int*) - (500) Number of structures to be generated
             * **num_iterations** (*int*) - (2500) Maximum number of iterations per structure
-            * **chirality_check** (*int*) - (2) Chirality check. Values: 0 (no chirality checks), 1 (only check afterwards), 2 (check on the fly) 
+            * **chirality_check** (*int*) - (2) Chirality check. Values: 0 (no chirality checks), 1 (only check afterwards), 2 (check on the fly)
             * **bs** (*int*) - (0) Number of rounds of triangular bound smoothing (default 0), (if >= 6, tetragonal BS is activated)
-            * **nofit** (*bool*) - (False) Do not fit generated structures to reference 
-            * **seed** (*int*) - (741265) Initial random seed 
+            * **nofit** (*bool*) - (False) Do not fit generated structures to reference
+            * **seed** (*int*) - (741265) Initial random seed
             * **violation** (*float*) - (1.0) Maximal acceptable sum of violations (nm)
-            * **nofit** (*bool*) - (False) Do not fit generated structures to reference 
+            * **nofit** (*bool*) - (False) Do not fit generated structures to reference
             * **convergence** (*int*) - (50) Consider convergence failed after this number of non-productive iterations
             * **trials** (*int*) - (25) Maximum number of trials per run
             * **damp** (*int*) - (1) Damping factor for distance corrections. Values: 1 (default), 2 (for cases with convergence problems)
             * **dyn** (*int*) - (1) Number of rounds to dynamically set tolerances
             * **bump** (*bool*) - (False) Do extra bump check
             * **pairlist_freq** (*int*) - (10) Pairlist update frequency in steps (only valid together with bump)
             * **cutoff** (*float*) - (0.5) Cut-off radius for pairlist (nm) (only valid together with bump)
             * **ref** (*bool*) - (False) Use input coordinates instead of random starting coordinates
-            * **scale** (*int*) - (1) Pre-scale coordinates with this factor 
+            * **scale** (*int*) - (1) Pre-scale coordinates with this factor
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_flexdyn.flexdyn.concoord_disco import concoord_disco
@@ -56,40 +59,38 @@
                                 output_traj_path='/path/to/disco_out_traj.pdb',
                                 output_rmsd_path='/path/to/disco_out_rmsd.dat',
                                 output_bfactor_path='/path/to/disco_out_bfactor.pdb',
                                 properties=prop)
 
     Info:
         * wrapped_software:
-            * name: Concoord 
+            * name: Concoord
             * version: >=2.1.2
             * license: other
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, input_dat_path: str, output_traj_path: str,
-    output_rmsd_path: str, output_bfactor_path: str, properties: dict = None, **kwargs) -> None:
+                 output_rmsd_path: str, output_bfactor_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path,
-                    'input_dat_path': input_dat_path,
-             },
-            'out': {    'output_traj_path': output_traj_path,
-                        'output_rmsd_path': output_rmsd_path,
-                        'output_bfactor_path': output_bfactor_path
-            }
+            'in': {'input_pdb_path': input_pdb_path,
+                   'input_dat_path': input_dat_path},
+            'out': {'output_traj_path': output_traj_path,
+                    'output_rmsd_path': output_rmsd_path,
+                    'output_bfactor_path': output_bfactor_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'disco')
 
         self.vdw = properties.get('vdw')
@@ -115,62 +116,63 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexDyn ConcoordDisco module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
-        # Copy auxiliary files (MARGINS, ATOMS, BONDS) according to the VdW property to the working dir 
+        # Copy auxiliary files (MARGINS, ATOMS, BONDS) according to the VdW property to the working dir
         concoord_lib = os.getenv("CONCOORDLIB")
 
         # MARGINS_li.DAT, MARGINS_oplsaa.DAT, MARGINS_oplsua.DAT, MARGINS_oplsx.DAT, MARGINS_repel.DAT, MARGINS_yamber2.DAT
         # 1 (OPLS-UA -united atoms- parameters), 2 (OPLS-AA -all atoms- parameters), 3 (PROLSQ repel parameters), 4 (Yamber2 parameters), 5 (Li et al. parameters), 6 (OPLS-X parameters -recommended for NMR structure determination-).
-        vdw_values = ["vdw_values","oplsua","oplsaa","repel","yamber2","li","oplsx"]
+        vdw_values = ["vdw_values", "oplsua", "oplsaa", "repel", "yamber2", "li", "oplsx"]
         margins_file = concoord_lib + "/MARGINS_" + vdw_values[self.vdw] + ".DAT"
         atoms_file = concoord_lib + "/ATOMS_" + vdw_values[self.vdw] + ".DAT"
         bonds_file = concoord_lib + "/BONDS.DAT"
         shutil.copy2(margins_file, self.stage_io_dict.get("unique_dir"))
         shutil.copy2(margins_file, self.stage_io_dict.get("unique_dir")+"/MARGINS.DAT")
         shutil.copy2(atoms_file, self.stage_io_dict.get("unique_dir"))
         shutil.copy2(bonds_file, self.stage_io_dict.get("unique_dir"))
 
         # Command line
-        # (concoord) OROZCO67:biobb_flexdyn hospital$ disco -d biobb_flexdyn/test/reference/flexdyn/dist.dat 
-        # -p biobb_flexdyn/test/reference/flexdyn/dist.pdb  -op patata.pdb 
-        self.cmd = ["cd ", self.stage_io_dict.get('unique_dir'), ";", self.binary_path, 
- #               "-p", str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
- #               "-d", str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path.cwd())),
- #               "-or", str(Path(self.stage_io_dict["out"]["output_rmsd_path"]).relative_to(Path.cwd())),
- #               "-of", str(Path(self.stage_io_dict["out"]["output_bfactor_path"]).relative_to(Path.cwd()))
-                "-p", str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
-                "-d", str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
-                "-or", str(Path(self.stage_io_dict["out"]["output_rmsd_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
-                "-of", str(Path(self.stage_io_dict["out"]["output_bfactor_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir'))))
-                ]
+        # (concoord) OROZCO67:biobb_flexdyn hospital$ disco -d biobb_flexdyn/test/reference/flexdyn/dist.dat
+        # -p biobb_flexdyn/test/reference/flexdyn/dist.pdb  -op patata.pdb
+        self.cmd = ["cd ", self.stage_io_dict.get('unique_dir'), ";", self.binary_path,
+                    #  "-p", str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
+                    #  "-d", str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path.cwd())),
+                    #  "-or", str(Path(self.stage_io_dict["out"]["output_rmsd_path"]).relative_to(Path.cwd())),
+                    #  "-of", str(Path(self.stage_io_dict["out"]["output_bfactor_path"]).relative_to(Path.cwd()))
+                    "-p", str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
+                    "-d", str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
+                    "-or", str(Path(self.stage_io_dict["out"]["output_rmsd_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
+                    "-of", str(Path(self.stage_io_dict["out"]["output_bfactor_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir'))))
+                    ]
 
         # Output structure formats:
         file_extension = Path(self.stage_io_dict["out"]["output_traj_path"]).suffix
         if file_extension == ".pdb":
-            self.cmd.append('-on') # NMR-PDB format (multi-model)
+            self.cmd.append('-on')  # NMR-PDB format (multi-model)
 #            self.cmd.append(str(Path(self.stage_io_dict["out"]["output_traj_path"]).relative_to(Path.cwd())))
             self.cmd.append(str(Path(self.stage_io_dict["out"]["output_traj_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))))
         elif file_extension == ".gro":
             self.cmd.append('-ot')
 #            self.cmd.append(str(Path(self.stage_io_dict["out"]["output_traj_path"]).relative_to(Path.cwd())))
             self.cmd.append(str(Path(self.stage_io_dict["out"]["output_traj_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))))
         elif file_extension == ".xtc":
             self.cmd.append('-ox')
 #            self.cmd.append(str(Path(self.stage_io_dict["out"]["output_traj_path"]).relative_to(Path.cwd())))
             self.cmd.append(str(Path(self.stage_io_dict["out"]["output_traj_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))))
         else:
             fu.log("ERROR: output_traj_path ({}) must be a PDB, GRO or XTC formatted file ({})".format(self.io_dict["out"]["output_traj_path"], file_extension), self.out_log, self.global_log)
-        
+
         # Properties
         if self.num_structs:
             self.cmd.append('-n')
             self.cmd.append(str(self.num_structs))
 
         if self.num_iterations:
             self.cmd.append('-i')
@@ -241,26 +243,28 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def concoord_disco(input_pdb_path: str, input_dat_path: str,
-            output_traj_path: str, output_rmsd_path: str, output_bfactor_path: str,
-            properties: dict = None, **kwargs) -> int:
+                   output_traj_path: str, output_rmsd_path: str, output_bfactor_path: str,
+                   properties: dict = None, **kwargs) -> int:
     """Create :class:`ConcoordDisco <flexdyn.concoord_disco.ConcoordDisco>`flexdyn.concoord_disco.ConcoordDisco class and
     execute :meth:`launch() <flexdyn.concoord_disco.ConcoordDisco.launch>` method"""
 
-    return ConcoordDisco(   input_pdb_path=input_pdb_path,
-                            input_dat_path=input_dat_path,
-                            output_traj_path=output_traj_path,
-                            output_rmsd_path=output_rmsd_path,
-                            output_bfactor_path=output_bfactor_path,
-                            properties=properties).launch()
+    return ConcoordDisco(input_pdb_path=input_pdb_path,
+                         input_dat_path=input_dat_path,
+                         output_traj_path=output_traj_path,
+                         output_rmsd_path=output_rmsd_path,
+                         output_bfactor_path=output_bfactor_path,
+                         properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Structure generation based on a set of geometric constraints extracted with the Concoord Dist tool.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -271,16 +275,17 @@
     required_args.add_argument('--output_bfactor_path', required=True, help='Output B-factor file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    concoord_disco( input_pdb_path=args.input_pdb_path,
-                    input_dat_path=args.input_dat_path,
-                    output_traj_path=args.output_traj_path,
-                    output_rmsd_path=args.output_rmsd_path,
-                    output_bfactor_path=args.output_bfactor_path,
-                    properties=properties)
+    concoord_disco(input_pdb_path=args.input_pdb_path,
+                   input_dat_path=args.input_dat_path,
+                   output_traj_path=args.output_traj_path,
+                   output_rmsd_path=args.output_rmsd_path,
+                   output_bfactor_path=args.output_bfactor_path,
+                   properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/concoord_dist.py` & `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/concoord_dist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 
 """Module containing the concoord_dist class and the command line interface."""
 import argparse
+import os
+import shutil
 from pathlib import Path
 from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class ConcoordDist(BiobbObject):
     """
     | biobb_flexdyn ConcoordDist
     | Wrapper of the Dist tool from the Concoord package.
     | Structure interpretation and bond definitions from a PDB/GRO file.
 
     Args:
@@ -22,17 +25,17 @@
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **binary_path** (*str*) - ("dist") Concoord dist binary path to be used.
             * **vdw** (*int*) - (1) Select a set of Van der Waals parameters. Values: 1 (OPLS-UA -united atoms- parameters), 2 (OPLS-AA -all atoms- parameters), 3 (PROLSQ repel parameters), 4 (Yamber2 parameters), 5 (Li et al. parameters), 6 (OPLS-X parameters -recommended for NMR structure determination-).
             * **bond_angle** (*int*) - (1) Select a set of bond/angle parameters. Values: 1 (Concoord default parameters), 2 (Engh-Huber parameters).
             * **retain_hydrogens** (*bool*) - (False) Retain hydrogen atoms
             * **nb_interactions** (*bool*) - (False) Try to find alternatives for non-bonded interactions (by default the native contacts will be preserved)
             * **cutoff** (*float*) - (4.0) cut-off radius (Angstroms) for non-bonded interacting pairs (the cut-off distances are additional to the sum of VDW radii)
-            * **min_distances** (*int*) - (50) Minimum number of distances to be defined for each atom 
+            * **min_distances** (*int*) - (50) Minimum number of distances to be defined for each atom
             * **damp** (*float*) - (1.0) Multiply each distance margin by this value
-            * **fixed_atoms** (*bool*) - (False) Interpret zero occupancy as atoms to keep fixed 
+            * **fixed_atoms** (*bool*) - (False) Interpret zero occupancy as atoms to keep fixed
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_flexdyn.flexdyn.concoord_dist import concoord_dist
@@ -44,38 +47,37 @@
                             output_pdb_path='/path/to/output.pdb',
                             output_gro_path='/path/to/output.gro',
                             output_dat_path='/path/to/output.dat',
                             properties=prop)
 
     Info:
         * wrapped_software:
-            * name: Concoord 
+            * name: Concoord
             * version: >=2.1.2
             * license: other
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_structure_path: str, output_pdb_path: str,
-    output_gro_path: str, output_dat_path: str, properties: dict = None, **kwargs) -> None:
+                 output_gro_path: str, output_dat_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_structure_path': input_structure_path },
-            'out': {    'output_pdb_path': output_pdb_path,
-                        'output_gro_path': output_gro_path,
-                        'output_dat_path': output_dat_path
-            }
+            'in': {'input_structure_path': input_structure_path},
+            'out': {'output_pdb_path': output_pdb_path,
+                    'output_gro_path': output_gro_path,
+                    'output_dat_path': output_dat_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'dist')
         self.retain_hydrogens = properties.get('retain_hydrogens', False)
         self.nb_interactions = properties.get('nb_interactions', False)
@@ -95,20 +97,27 @@
     def launch(self):
         """Launches the execution of the FlexDyn ConcoordDist module."""
 
         # Set input params
         self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.vdw}\n{self.bond_angle}\n')
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
+        # Copy auxiliary file (HBONDS) to the working dir
+        concoord_lib = os.getenv("CONCOORDLIB")
+
+        hbonds_file = concoord_lib + "/HBONDS.DAT"
+        shutil.copy2(hbonds_file, self.stage_io_dict.get("unique_dir"))
+
         # Command line
-        # (concoord) OROZCO67:biobb_flexdyn hospital$ dist -p biobb_flexdyn/test/data/flexdyn/structure.pdb 
-        # -op dist.pdb -og dist.gro -od dist.dat 
+        # (concoord) OROZCO67:biobb_flexdyn hospital$ dist -p biobb_flexdyn/test/data/flexdyn/structure.pdb
+        # -op dist.pdb -og dist.gro -od dist.dat
         # Select a set of Van der Waals parameters:
         # 1: OPLS-UA (united atoms) parameters
         # 2: OPLS-AA (all atoms) parameters
         # 3: PROLSQ repel parameters
         # 4: Yamber2 parameters
         # 5: Li et al. parameters
         # 6: OPLS-X parameters (recommended for NMR structure determination)
@@ -119,28 +128,34 @@
         # Select a set of bond/angle parameters:
         # 1: Concoord default parameters
         # 2: Engh-Huber parameters
         # 1
         # Selected parameter set 1
         # copying /opt/anaconda3/envs/concoord/share/concoord/lib/BONDS.DAT.noeh to BONDS.DAT in current working directory
 
-        self.cmd = [self.binary_path, 
-                "-op", self.stage_io_dict["out"]["output_pdb_path"], 
-                "-og", self.stage_io_dict["out"]["output_gro_path"], 
-                "-od", self.stage_io_dict["out"]["output_dat_path"]
-                ]
-
+        self.cmd = ["cd ", self.stage_io_dict.get('unique_dir'), ";", self.binary_path,
+                    #  "-op", self.stage_io_dict["out"]["output_pdb_path"],
+                    #  "-og", self.stage_io_dict["out"]["output_gro_path"],
+                    #  "-od", self.stage_io_dict["out"]["output_dat_path"]
+                    "-op", str(Path(self.stage_io_dict["out"]["output_pdb_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
+                    "-og", str(Path(self.stage_io_dict["out"]["output_gro_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))),
+                    "-od", str(Path(self.stage_io_dict["out"]["output_dat_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir'))))
+                    ]
         # If input structure in pdb format:
         file_extension = Path(self.stage_io_dict["in"]["input_structure_path"]).suffix
         if file_extension == ".pdb":
             self.cmd.append('-p')
-            self.cmd.append(self.stage_io_dict["in"]["input_structure_path"])
+            # self.cmd.append(self.stage_io_dict["in"]["input_structure_path"])
+            self.cmd.append(str(Path(self.stage_io_dict["in"]["input_structure_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))))
+
         elif file_extension == ".gro":
             self.cmd.append('-g')
-            self.cmd.append(self.stage_io_dict["in"]["input_structure_path"])
+            # self.cmd.append(self.stage_io_dict["in"]["input_structure_path"])
+            self.cmd.append(str(Path(self.stage_io_dict["in"]["input_structure_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))))
+
         else:
             fu.log("ERROR: input_structure_path ({}) must be a PDB or a GRO formatted file ({})".format(self.io_dict["in"]["input_structure_path"], file_extension), self.out_log, self.global_log)
 
         if self.retain_hydrogens:
             self.cmd.append('-r')
 
         if self.nb_interactions:
@@ -156,18 +171,19 @@
         if self.min_distances:
             self.cmd.append('-m')
             self.cmd.append(str(self.min_distances))
 
         if self.damp:
             self.cmd.append('-damp')
             self.cmd.append(str(self.damp))
-            
+
         # Add stdin input file
         self.cmd.append('<')
-        self.cmd.append(self.stage_io_dict["in"]["stdin_file_path"])
+        # self.cmd.append(self.stage_io_dict["in"]["stdin_file_path"])
+        self.cmd.append(str(Path(self.stage_io_dict["in"]["stdin_file_path"]).relative_to(Path(self.stage_io_dict.get('unique_dir')))))
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -178,25 +194,27 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def concoord_dist(input_structure_path: str,
-            output_pdb_path: str, output_gro_path: str, output_dat_path: str,
-            properties: dict = None, **kwargs) -> int:
+                  output_pdb_path: str, output_gro_path: str, output_dat_path: str,
+                  properties: dict = None, **kwargs) -> int:
     """Create :class:`ConcoordDist <flexdyn.concoord_dist.ConcoordDist>`flexdyn.concoord_dist.ConcoordDist class and
     execute :meth:`launch() <flexdyn.concoord_dist.ConcoordDist.launch>` method"""
 
-    return ConcoordDist(    input_structure_path=input_structure_path,
-                            output_pdb_path=output_pdb_path,
-                            output_gro_path=output_gro_path,
-                            output_dat_path=output_dat_path,
-                            properties=properties).launch()
+    return ConcoordDist(input_structure_path=input_structure_path,
+                        output_pdb_path=output_pdb_path,
+                        output_gro_path=output_gro_path,
+                        output_dat_path=output_dat_path,
+                        properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Structure interpretation and bond definitions from a PDB/GRO file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -206,15 +224,16 @@
     required_args.add_argument('--output_dat_path', required=True, help='Output dat file with structure interpretation and bond definitions. Accepted formats: dat, txt.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    concoord_dist(  input_structure_path=args.input_structure_path,
-                    output_pdb_path=args.output_pdb_path,
-                    output_gro_path=args.output_gro_path,
-                    output_dat_path=args.output_dat_path,
-                    properties=properties)
+    concoord_dist(input_structure_path=args.input_structure_path,
+                  output_pdb_path=args.output_pdb_path,
+                  output_gro_path=args.output_gro_path,
+                  output_dat_path=args.output_dat_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/imod_imode.py` & `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 #!/usr/bin/env python3
 
 """Module containing the imode class and the command line interface."""
 import argparse
 import shutil
 from pathlib import Path
-from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class ImodImode(BiobbObject):
     """
     | biobb_flexdyn imod_imode
-    | Wrapper of the imode tool 
+    | Wrapper of the imode tool
     | Compute the normal modes of a macromolecule using the imode tool from the iMODS package.
 
     Args:
         input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/structure.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_dat_path (str): Output dat with normal modes. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/imod_imode_evecs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **cg** (*int*) - (2) Coarse-Grained model. Values: 0 (CA), 1 (C5), 2 (Heavy atoms).
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
-            * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist. 
+            * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_flexdyn.flexdyn.imod_imode import imod_imode
             prop = {
                 'cg' : 2
             }
             imod_imode(   input_pdb_path='/path/to/structure.pdb',
                     output_dat_path='/path/to/output_evecs.dat',
                     properties=prop)
 
     Info:
         * wrapped_software:
-            * name: iMODS 
+            * name: iMODS
             * version: >=1.0.4
             * license: other
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, output_dat_path: str,
-    properties: dict = None, **kwargs) -> None:
+                 properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path },
-            'out': { 'output_dat_path': output_dat_path }
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_dat_path': output_dat_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'imode_gcc')
 
         self.cg = properties.get('cg', 2)
@@ -70,28 +70,29 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexDyn iMOD imode module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Output temporary file
-        out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs") 
-        out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs_ic.evec") 
+        out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs")
+        out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs_ic.evec")
 
         # Command line
         # imode_gcc  1ake_backbone.pdb -m 0 -o patata.evec
-        self.cmd = [self.binary_path, 
-                str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
-                "-o", str(out_file_prefix),
-                "-m", str(self.cg) 
-                ]
+        self.cmd = [self.binary_path,
+                    str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
+                    "-o", str(out_file_prefix),
+                    "-m", str(self.cg)
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copying generated output file to the final (user-given) file name
         shutil.copy2(out_file, self.stage_io_dict["out"]["output_dat_path"])
 
@@ -104,22 +105,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def imod_imode(input_pdb_path: str, output_dat_path: str, 
-            properties: dict = None, **kwargs) -> int:
+
+def imod_imode(input_pdb_path: str, output_dat_path: str,
+               properties: dict = None, **kwargs) -> int:
     """Create :class:`ImodImode <flexdyn.imod_imode.ImodImode>`flexdyn.imod_imode.ImodImode class and
     execute :meth:`launch() <flexdyn.imod_imode.ImodImode.launch>` method"""
 
-    return ImodImode(    input_pdb_path=input_pdb_path,
-                        output_dat_path=output_dat_path,
-                        properties=properties).launch()
+    return ImodImode(input_pdb_path=input_pdb_path,
+                     output_dat_path=output_dat_path,
+                     properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Compute the normal modes of a macromolecule using the imode tool from the iMODS package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -127,13 +130,14 @@
     required_args.add_argument('--output_dat_path', required=True, help='Output evecs dat file. Accepted formats: dat.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    imod_imode(  input_pdb_path=args.input_pdb_path,
-            output_dat_path=args.output_dat_path,
-            properties=properties)
+    imod_imode(input_pdb_path=args.input_pdb_path,
+               output_dat_path=args.output_dat_path,
+               properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/imod_imove.py` & `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/imod_imove.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python3
 
 """Module containing the imode class and the command line interface."""
 import argparse
-import shutil
 from pathlib import Path
-from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class ImodImove(BiobbObject):
     """
     | biobb_flexdyn imod_imove
-    | Wrapper of the imove tool 
+    | Wrapper of the imove tool
     | Compute the normal modes of a macromolecule using the imove tool from the iMODS package.
 
     Args:
         input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/structure_cleaned.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_dat_path (str): Input dat with normal modes. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/imod_imode_evecs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
         output_pdb_path (str): Output multi-model PDB file with the generated animation by Principal Component. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/imod_imove_output.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **pc** (*int*) - (1) Principal Component.
+            * **num_frames** (*int*) - (11) Number of frames to be generated
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
-            * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist. 
+            * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_flexdyn.flexdyn.imod_imove import imod_imove
             prop = {
                 'pc' : 1
@@ -34,96 +34,98 @@
             imod_imove(   input_pdb_path='/path/to/structure.pdb',
                           input_dat_path='/path/to/input_evecs.dat',
                           output_pdb_path='/path/to/output_anim.pdb',
                           properties=prop)
 
     Info:
         * wrapped_software:
-            * name: iMODS 
+            * name: iMODS
             * version: >=1.0.4
             * license: other
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, input_dat_path: str, output_pdb_path: str,
-    properties: dict = None, **kwargs) -> None:
+                 properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path, 'input_dat_path': input_dat_path, },
-            'out': { 'output_pdb_path': output_pdb_path }
+            'in': {'input_pdb_path': input_pdb_path, 'input_dat_path': input_dat_path},
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'imove')
 
         self.pc = properties.get('pc', 1)
+        self.num_frames = properties.get('num_frames', 11)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexDyn iMOD imove module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
-        # Output temporary file
-        out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_pc") 
-        out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_pc_ic.pdb") 
-
         # Command line
-        # imode_gcc  1ake_backbone.pdb -m 0 -o patata.evec
-        self.cmd = [self.binary_path, 
-                str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
-                str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path.cwd())),
-                str(Path(self.stage_io_dict["out"]["output_pdb_path"]).relative_to(Path.cwd())),
-                str(self.pc)
-                ]
+        # imove 1ake_backbone.pdb  1ake_backbone_evecs.dat -o 1ake_backbone.ensemble.pdb 1 -c 500
+        self.cmd = [self.binary_path,
+                    str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
+                    str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path.cwd())),
+                    str(Path(self.stage_io_dict["out"]["output_pdb_path"]).relative_to(Path.cwd())),
+                    str(self.pc)
+                    ]
+
+        # Properties
+        if self.num_frames:
+            self.cmd.append('-c')
+            self.cmd.append(str(self.num_frames))
 
         # Run Biobb block
         self.run_biobb()
 
-        # Copying generated output file to the final (user-given) file name
-        #shutil.copy2(out_file, self.stage_io_dict["out"]["output_dat_path"])
-
         # Copy files to host
         self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir")
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def imod_imove(input_pdb_path: str, input_dat_path: str, output_pdb_path: str, 
-            properties: dict = None, **kwargs) -> int:
+
+def imod_imove(input_pdb_path: str, input_dat_path: str, output_pdb_path: str,
+               properties: dict = None, **kwargs) -> int:
     """Create :class:`ImodImove <flexdyn.imod_imove.ImodImove>`flexdyn.imod_imove.ImodImove class and
     execute :meth:`launch() <flexdyn.imod_imove.ImodImove.launch>` method"""
 
-    return ImodImove(   input_pdb_path=input_pdb_path,
-                        input_dat_path=input_dat_path,
-                        output_pdb_path=output_pdb_path,
-                        properties=properties).launch()
+    return ImodImove(input_pdb_path=input_pdb_path,
+                     input_dat_path=input_dat_path,
+                     output_pdb_path=output_pdb_path,
+                     properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Animate the normal modes of a macromolecule using the imove tool from the iMODS package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -132,14 +134,15 @@
     required_args.add_argument('--output_pdb_path', required=True, help='Output pdb file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    imod_imove(  input_pdb_path=args.input_pdb_path,
-            input_dat_path=args.input_dat_path,
-            output_pdb_path=args.output_pdb_path,
-            properties=properties)
+    imod_imove(input_pdb_path=args.input_pdb_path,
+               input_dat_path=args.input_dat_path,
+               output_pdb_path=args.output_pdb_path,
+               properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/nolb_nma.py` & `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/nolb_nma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/env python3
 
 """Module containing the nolb class and the command line interface."""
 import argparse
 import shutil
 from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class Nolb_nma(BiobbObject):
     """
     | biobb_flexdyn Nolb_nma
-    | Wrapper of the NOLB tool 
+    | Wrapper of the NOLB tool
     | Generate an ensemble of structures using the NOLB (NOn-Linear rigid Block) NMA tool.
 
     Args:
         input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/structure.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_pdb_path (str): Output multi-model PDB file with the generated ensemble. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/nolb_output.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **num_structs** (*int*) - (500) Number of structures to be generated
-            * **cutoff** (*float*) - (5.0) This options specifies the interaction cutoff distance for the elastic network models (in angstroms), 5 by default. The Hessian matrix is constructed according to this interaction distance. Some artifacts should be expected for too short distances (< 5 Å). 
-            * **rmsd** (*float*) - (1.0) Maximum RMSd for decoy generation. 
+            * **cutoff** (*float*) - (5.0) This options specifies the interaction cutoff distance for the elastic network models (in angstroms), 5 by default. The Hessian matrix is constructed according to this interaction distance. Some artifacts should be expected for too short distances (< 5 Å).
+            * **rmsd** (*float*) - (1.0) Maximum RMSd for decoy generation.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_flexdyn.flexdyn.nolb_nma import nolb_nma
@@ -33,90 +34,91 @@
             }
             nolb_nma(   input_pdb_path='/path/to/structure.pdb',
                     output_pdb_path='/path/to/output.pdb',
                     properties=prop)
 
     Info:
         * wrapped_software:
-            * name: NOLB 
+            * name: NOLB
             * version: >=1.9
             * license: other
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, output_pdb_path: str,
-    properties: dict = None, **kwargs) -> None:
+                 properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path },
-            'out': { 'output_pdb_path': output_pdb_path }
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'NOLB')
 
         self.num_structs = properties.get('num_structs', 500)
-        #self.num_modes = properties.get('num_modes', 10)
+        # self.num_modes = properties.get('num_modes', 10)
         self.cutoff = properties.get('cutoff', 5.0)
         self.rmsd = properties.get('rmsd', 1.0)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexDyn NOLB module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Output temporary file
-        out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("nolb_ensemble") 
-        out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("nolb_ensemble_nlb_decoys.pdb") 
+        out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("nolb_ensemble")
+        out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("nolb_ensemble_nlb_decoys.pdb")
 
         # Command line
         # ./NOLB 1ake_monomer.pdb -s 100 --rmsd 5 -m  -o patata # Output: patata_nlb_decoys.pdb
-        self.cmd = [self.binary_path, 
-                str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
-                "-o", str(out_file_prefix),
-                "-m" # Minimizing the generated structures by default
-                ]
+        self.cmd = [self.binary_path,
+                    str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
+                    "-o", str(out_file_prefix),
+                    "-m"  # Minimizing the generated structures by default
+                    ]
 
         # Properties
         if self.num_structs:
             self.cmd.append('-s')
             self.cmd.append(str(self.num_structs))
 
         # Num modes is deactivated for the decoys generation. CHECK!
         #  * **num_modes** (*int*) - (10) Number of non-trivial modes to compute, 10 by default. If this number exceeds the size of the Hessian matrix, it will be adapted accordingly.
-        #if self.num_modes:
+        # if self.num_modes:
         #    self.cmd.append('-n')
         #    self.cmd.append(str(self.num_modes))
 
         if self.cutoff:
             self.cmd.append('-c')
             self.cmd.append(str(self.cutoff))
 
         if self.rmsd:
             self.cmd.append('--rmsd')
             self.cmd.append(str(self.rmsd))
 
-        #--dist 1 -m --nSteps 5000 --tol 0.001
+        # --dist 1 -m --nSteps 5000 --tol 0.001
         self.cmd.append("--dist 1 --nSteps 5000 --tol 0.001")
 
         # Run Biobb block
         self.run_biobb()
 
         # Copying generated output file to the final (user-given) file name
         shutil.copy2(out_file, self.stage_io_dict["out"]["output_pdb_path"])
@@ -130,22 +132,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def nolb_nma(input_pdb_path: str, output_pdb_path: str, 
-            properties: dict = None, **kwargs) -> int:
+
+def nolb_nma(input_pdb_path: str, output_pdb_path: str,
+             properties: dict = None, **kwargs) -> int:
     """Create :class:`Nolb_nma <flexdyn.nolb_nma.Nolb_nma>`flexdyn.nolb_nma.Nolb_nma class and
     execute :meth:`launch() <flexdyn.nolb_nma.Nolb_nma.launch>` method"""
 
-    return Nolb_nma(    input_pdb_path=input_pdb_path,
-                        output_pdb_path=output_pdb_path,
-                        properties=properties).launch()
+    return Nolb_nma(input_pdb_path=input_pdb_path,
+                    output_pdb_path=output_pdb_path,
+                    properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Generate an ensemble of structures using the NOLB (NOn-Linear rigid Block) NMA tool.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -153,13 +157,14 @@
     required_args.add_argument('--output_pdb_path', required=True, help='Output pdb file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    nolb_nma(   input_pdb_path=args.input_pdb_path,
-            output_pdb_path=args.output_pdb_path,
-            properties=properties)
+    nolb_nma(input_pdb_path=args.input_pdb_path,
+             output_pdb_path=args.output_pdb_path,
+             properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn/flexdyn/prody_anm.py` & `biobb_flexdyn-4.0.1/biobb_flexdyn/flexdyn/prody_anm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the prody_anm class and the command line interface."""
 import argparse
 import prody
-from pathlib import Path
-from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class ProdyANM(BiobbObject):
     """
     | biobb_flexdyn ProdyANM
     | Wrapper of the ANM tool from the Prody package.
     | Generate an ensemble of structures using the Prody Anisotropic Network Model (ANM), for coarse-grained NMA.
 
     Args:
@@ -37,35 +36,35 @@
             }
             prody_anm(  input_pdb_path='/path/to/structure.pdb',
                         output_pdb_path='/path/to/output.pdb',
                         properties=prop)
 
     Info:
         * wrapped_software:
-            * name: Prody 
+            * name: Prody
             * version: >=2.2.0
             * license: MIT
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, output_pdb_path: str,
-    properties: dict = None, **kwargs) -> None:
+                 properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path },
-            'out': { 'output_pdb_path': output_pdb_path }
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
 
         self.num_structs = properties.get('num_structs', 500)
         self.selection = properties.get('selection', 'calpha')
@@ -78,15 +77,16 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexDyn ConcoordDist module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         prot = prody.parsePDB(self.stage_io_dict["in"]["input_pdb_path"],)
 
         # http://prody.csb.pitt.edu/manual/reference/atomic/select.html
         prot_sel = prot.select(self.selection)
 
@@ -98,15 +98,15 @@
 
         bb_enm, bb_atoms = prody.extendModel(enm, prot_sel, prot_sel)
 
         ensemble = prody.sampleModes(bb_enm[:3], bb_atoms, n_confs=self.num_structs, rmsd=self.rmsd)
 
         nmastruct = bb_atoms.copy()
         nmastruct.addCoordset(ensemble)
-                
+
         prody.writePDB(self.stage_io_dict["out"]["output_pdb_path"], nmastruct)
 
         # Copy files to host
         self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
@@ -114,22 +114,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def prody_anm(input_pdb_path: str, output_pdb_path: str, 
-            properties: dict = None, **kwargs) -> int:
+
+def prody_anm(input_pdb_path: str, output_pdb_path: str,
+              properties: dict = None, **kwargs) -> int:
     """Create :class:`ProdyANM <flexdyn.prody_anm.ProdyANM>`flexdyn.prody_anm.ProdyANM class and
     execute :meth:`launch() <flexdyn.prody_anm.ProdyANM.launch>` method"""
 
-    return ProdyANM(    input_pdb_path=input_pdb_path,
-                        output_pdb_path=output_pdb_path,
-                        properties=properties).launch()
+    return ProdyANM(input_pdb_path=input_pdb_path,
+                    output_pdb_path=output_pdb_path,
+                    properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Generate an ensemble of structures using the Prody Anisotropic Network Model (ANM), for coarse-grained NMA.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -137,13 +139,14 @@
     required_args.add_argument('--output_pdb_path', required=True, help='Output pdb file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    prody_anm(  input_pdb_path=args.input_pdb_path,
-                output_pdb_path=args.output_pdb_path,
-                properties=properties)
+    prody_anm(input_pdb_path=args.input_pdb_path,
+              output_pdb_path=args.output_pdb_path,
+              properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/PKG-INFO` & `biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-flexdyn
-Version: 4.0.0
+Version: 4.0.1
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexdyn-4.0.0/biobb_flexdyn.egg-info/SOURCES.txt` & `biobb_flexdyn-4.0.1/biobb_flexdyn.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,11 +7,12 @@
 biobb_flexdyn.egg-info/dependency_links.txt
 biobb_flexdyn.egg-info/entry_points.txt
 biobb_flexdyn.egg-info/requires.txt
 biobb_flexdyn.egg-info/top_level.txt
 biobb_flexdyn/flexdyn/__init__.py
 biobb_flexdyn/flexdyn/concoord_disco.py
 biobb_flexdyn/flexdyn/concoord_dist.py
+biobb_flexdyn/flexdyn/imod_imc.py
 biobb_flexdyn/flexdyn/imod_imode.py
 biobb_flexdyn/flexdyn/imod_imove.py
 biobb_flexdyn/flexdyn/nolb_nma.py
 biobb_flexdyn/flexdyn/prody_anm.py
```

### Comparing `biobb_flexdyn-4.0.0/setup.py` & `biobb_flexdyn-4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexdyn",
-    version="4.0.0",
+    version="4.0.1",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.",
     long_description="biobb_flexdyn allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexdyn",
@@ -23,14 +23,15 @@
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "concoord_dist = biobb_flexdyn.flexdyn.concoord_dist:main",
             "concoord_disco = biobb_flexdyn.flexdyn.concoord_disco:main",
             "imod_imode = biobb_flexdyn.flexdyn.imod_imode:main",
             "imod_imove = biobb_flexdyn.flexdyn.imod_imove:main",
+            "imod_imc = biobb_flexdyn.flexdyn.imod_imc:main",
             "nolb_nma = biobb_flexdyn.flexdyn.nolb_nma:main",
             "prody_anm = biobb_flexdyn.flexdyn.prody_anm:main"
         ]
     },
     classifiers=(
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.7",
```

