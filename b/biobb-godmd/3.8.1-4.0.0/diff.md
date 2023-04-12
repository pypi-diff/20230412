# Comparing `tmp/biobb_godmd-3.8.1.tar.gz` & `tmp/biobb_godmd-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_godmd-3.8.1.tar", last modified: Tue Sep 20 14:05:55 2022, max compression
+gzip compressed data, was "dist/biobb_godmd-4.0.0.tar", last modified: Wed Apr 12 10:57:24 2023, max compression
```

## Comparing `biobb_godmd-3.8.1.tar` & `biobb_godmd-4.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2022-09-20 14:05:55.544118 biobb_godmd-3.8.1/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)    11357 2022-09-20 11:24:37.000000 biobb_godmd-3.8.1/LICENSE
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)      905 2022-09-20 14:05:55.543959 biobb_godmd-3.8.1/PKG-INFO
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     3136 2022-09-20 11:24:37.000000 biobb_godmd-3.8.1/README.md
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2022-09-20 14:05:55.542505 biobb_godmd-3.8.1/biobb_godmd/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       62 2022-09-20 13:35:05.000000 biobb_godmd-3.8.1/biobb_godmd/__init__.py
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2022-09-20 14:05:55.543786 biobb_godmd-3.8.1/biobb_godmd/godmd/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       53 2022-09-20 11:24:37.000000 biobb_godmd-3.8.1/biobb_godmd/godmd/__init__.py
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     2070 2022-09-20 11:24:37.000000 biobb_godmd-3.8.1/biobb_godmd/godmd/common.py
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)    16284 2022-09-20 11:24:37.000000 biobb_godmd-3.8.1/biobb_godmd/godmd/godmd_prep.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)    14837 2022-09-20 11:24:37.000000 biobb_godmd-3.8.1/biobb_godmd/godmd/godmd_run.py
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2022-09-20 14:05:55.543240 biobb_godmd-3.8.1/biobb_godmd.egg-info/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)      905 2022-09-20 14:05:55.000000 biobb_godmd-3.8.1/biobb_godmd.egg-info/PKG-INFO
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)      383 2022-09-20 14:05:55.000000 biobb_godmd-3.8.1/biobb_godmd.egg-info/SOURCES.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        1 2022-09-20 14:05:55.000000 biobb_godmd-3.8.1/biobb_godmd.egg-info/dependency_links.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)      110 2022-09-20 14:05:55.000000 biobb_godmd-3.8.1/biobb_godmd.egg-info/entry_points.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       20 2022-09-20 14:05:55.000000 biobb_godmd-3.8.1/biobb_godmd.egg-info/requires.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       12 2022-09-20 14:05:55.000000 biobb_godmd-3.8.1/biobb_godmd.egg-info/top_level.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       38 2022-09-20 14:05:55.544161 biobb_godmd-3.8.1/setup.cfg
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     1391 2022-09-20 14:05:23.000000 biobb_godmd-3.8.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-04-11 11:37:10.000000 biobb_godmd-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      912 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5295 2023-04-12 10:52:11.000000 biobb_godmd-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       63 2023-04-12 10:50:04.000000 biobb_godmd-4.0.0/biobb_godmd/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       53 2023-04-11 11:37:10.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2246 2023-04-12 10:26:31.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16873 2023-04-12 10:26:31.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_prep.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15081 2023-04-12 10:27:51.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      912 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      383 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      110 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       12 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1398 2023-04-12 10:49:40.000000 biobb_godmd-4.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `biobb_godmd-3.8.1/LICENSE` & `biobb_godmd-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_godmd-3.8.1/PKG-INFO` & `biobb_godmd-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: biobb_godmd
-Version: 3.8.1
+Version: 4.0.0
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.
```

### Comparing `biobb_godmd-3.8.1/biobb_godmd/godmd/common.py` & `biobb_godmd-4.0.0/biobb_godmd/godmd/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 """ Common functions for package biobb_godmd.godmd """
 from pathlib import Path, PurePath
-import re
 from biobb_common.tools import file_utils as fu
 
+
 # CHECK INPUT PARAMETERS
 def check_input_path(path, argument, optional, out_log, classname):
-	""" Checks input file """
-	if optional and not path:
-		return None
-	if not Path(path).exists():
-		fu.log("Path: " + path)
-		fu.log("Path " + path + " --- " + classname + ': Unexisting %s file, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting %s file' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks input file """
+    if optional and not path:
+        return None
+    if not Path(path).exists():
+        fu.log("Path: " + path)
+        fu.log("Path " + path + " --- " + classname + ': Unexisting %s file, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting %s file' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def check_output_path(path, argument, optional, out_log, classname):
-	""" Checks output file """
-	if optional and not path:
-		return None
-	if PurePath(path).parent and not Path(PurePath(path).parent).exists():
-		fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting  %s folder' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks output file """
+    if optional and not path:
+        return None
+    if PurePath(path).parent and not Path(PurePath(path).parent).exists():
+        fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting  %s folder' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def is_valid_file(ext, argument):
-	""" Checks if file format is compatible """
-	formats = {
-		'input_pdb_orig_path': ['pdb'],
-		'input_pdb_target_path': ['pdb'],
-		'input_aln_orig_path': ['aln','txt'],
-		'input_aln_target_path': ['aln','txt'],
-		'input_config_path': ['in','txt'],
-		'output_aln_orig_path': ['aln','txt'],
-		'output_aln_target_path': ['aln','txt'],
-		'output_log_path': ['log', 'out','txt'],
-		'output_ene_path': ['log', 'out', 'txt'],
-		'output_trj_path': ['x','trj','crd','mdcrd'],
-	}
-	return ext in formats[argument]
+    """ Checks if file format is compatible """
+    formats = {
+        'input_pdb_orig_path': ['pdb'],
+        'input_pdb_target_path': ['pdb'],
+        'input_aln_orig_path': ['aln', 'txt'],
+        'input_aln_target_path': ['aln', 'txt'],
+        'input_config_path': ['in', 'txt'],
+        'output_aln_orig_path': ['aln', 'txt'],
+        'output_aln_target_path': ['aln', 'txt'],
+        'output_log_path': ['log', 'out', 'txt'],
+        'output_ene_path': ['log', 'out', 'txt'],
+        'output_trj_path': ['x', 'trj', 'crd', 'mdcrd'],
+    }
+    return ext in formats[argument]
```

### Comparing `biobb_godmd-3.8.1/biobb_godmd/godmd/godmd_prep.py` & `biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python3
 
 """Module containing the GOdMDPrep class and the command line interface."""
 import argparse
-import json
-import shutil, re, os
-import collections.abc
-from pathlib import Path, PurePath
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_godmd.godmd.common import *
+from biobb_godmd.godmd.common import check_input_path, check_output_path
+
 
 class GOdMDPrep(BiobbObject):
     """
     | biobb_godmd GOdMDPrep
     | Helper bb to prepare inputs for the `GOdMD tool <http://mmb.irbbarcelona.org/GOdMD/>`_ module.
     | Prepares input files for the GOdMD tool.
 
@@ -50,104 +48,110 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_orig_path: str, input_pdb_target_path: str,
-    output_aln_orig_path: str, output_aln_target_path: str, 
-    properties: dict = None, **kwargs) -> None:
+                 output_aln_orig_path: str, output_aln_target_path: str,
+                 properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         self.AA_TRANSLATOR = {'GLY': 'G',
-                        'ALA': 'A',
-                        'VAL': 'V',
-                        'LEU': 'L',
-                        'ILE': 'I',
-                        'MET': 'M',
-                        'PHE': 'F',
-                        'TRP': 'W',
-                        'PRO': 'P',
-                        'SER': 'S',
-                        'THR': 'T',
-                        'CYS': 'C',
-                        'CYX': 'C',
-                        'CYM': 'C',
-                        'TYR': 'Y',
-                        'TYM': 'Y',
-                        'ASN': 'N',
-                        'GLN': 'Q',
-                        'ASP': 'D',
-                        'ASH': 'D',
-                        'GLU': 'E',
-                        'GLH': 'E',
-                        'LYS': 'K',
-                        'LYN': 'K',
-                        'ARG': 'R',
-                        'ARN': 'R',
-                        'HIS': 'H',
-                        'HIE': 'H',
-                        'HID': 'H',
-                        'HIP': 'H'}
+                              'ALA': 'A',
+                              'VAL': 'V',
+                              'LEU': 'L',
+                              'ILE': 'I',
+                              'MET': 'M',
+                              'PHE': 'F',
+                              'TRP': 'W',
+                              'PRO': 'P',
+                              'SER': 'S',
+                              'THR': 'T',
+                              'CYS': 'C',
+                              'CYX': 'C',
+                              'CYM': 'C',
+                              'TYR': 'Y',
+                              'TYM': 'Y',
+                              'ASN': 'N',
+                              'GLN': 'Q',
+                              'ASP': 'D',
+                              'ASH': 'D',
+                              'GLU': 'E',
+                              'GLH': 'E',
+                              'LYS': 'K',
+                              'LYN': 'K',
+                              'ARG': 'R',
+                              'ARN': 'R',
+                              'HIS': 'H',
+                              'HIE': 'H',
+                              'HID': 'H',
+                              'HIP': 'H'}
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_orig_path': input_pdb_orig_path,
-                    'input_pdb_target_path': input_pdb_target_path },
-            'out': { 'output_aln_orig_path': output_aln_orig_path,
-                     'output_aln_target_path': output_aln_target_path }
+            'in': {'input_pdb_orig_path': input_pdb_orig_path,
+                   'input_pdb_target_path': input_pdb_target_path},
+            'out': {'output_aln_orig_path': output_aln_orig_path,
+                    'output_aln_target_path': output_aln_target_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.gapopen = properties.get('gapopen', "12.0")
         self.gapextend = properties.get('gapextend', "2.0")
         self.datafile = properties.get('datafile', "EPAM250")
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     def check_data_params(self, out_log, out_err):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_pdb_orig_path"] = check_input_path(self.io_dict["in"]["input_pdb_orig_path"], "input_pdb_orig_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_pdb_target_path"] = check_input_path(self.io_dict["in"]["input_pdb_target_path"], "input_pdb_target_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_aln_orig_path"] = check_output_path(self.io_dict["out"]["output_aln_orig_path"],"output_aln_orig_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_aln_target_path"] = check_output_path(self.io_dict["out"]["output_aln_target_path"],"output_aln_target_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_aln_orig_path"] = check_output_path(self.io_dict["out"]["output_aln_orig_path"], "output_aln_orig_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_aln_target_path"] = check_output_path(self.io_dict["out"]["output_aln_target_path"], "output_aln_target_path", False, out_log, self.__class__.__name__)
 
     def extract_sequence(self, pdb):
         '''
         Parses a PDB file to retrieve the sequence of a certain chain.
         '''
         seq = ''
         resids = []
         with open(pdb) as file:
             for line in file:
                 line = line.rstrip('\n')
-                record = line[:6].replace(" ","")
-                if record != 'ATOM' : continue
+                record = line[:6].replace(" ", "")
+                if record != 'ATOM':
+                    continue
                 atomname = line[12:16]
-                atomname = atomname.replace(" ","")
-                if atomname != 'CA': continue
+                atomname = atomname.replace(" ", "")
+                if atomname != 'CA':
+                    continue
                 alternate = line[16]
                 if alternate != ' ':
-                    if alternate != 'A': continue # if alt loc, only A-labeled residues
-                resname = line[17:20].replace(" ","")
-                if resname not in self.AA_TRANSLATOR: continue
-                resnum = line[22:26].replace(" ","")
+                    if alternate != 'A':
+                        continue  # if alt loc, only A-labeled residues
+                resname = line[17:20].replace(" ", "")
+                if resname not in self.AA_TRANSLATOR:
+                    continue
+                resnum = line[22:26].replace(" ", "")
                 icode = line[26:27]
                 seq += self.AA_TRANSLATOR[resname]
-                resids += [(' ',int(resnum),icode)] # BioPython's standard PDB atom id (' ',resid,insertioncode) (e.g. (' ',40,'B'))
+                resids += [(' ', int(resnum), icode)]  # BioPython's standard PDB atom id (' ',resid,insertioncode) (e.g. (' ',40,'B'))
 
         return seq, resids
 
     def retrieve_alignment(self, waterFile, resids1, resids2):
         '''
         Gets the FASTA sequence of two PDB structures and a list of their residues in Biopython residue format.
         Opens a file containing a local sequence alignment (Water program of EMBOSS package) between those two PDB structures.
@@ -202,54 +206,58 @@
 
         # Get the residues of the alignment.
         # -2 is applied because in the first iteration of next loop all values will always be increased by 1 (local alignment)
         # and we also need to convert the number into a python index to retrieve the proper token in the list
         resid_pairs = []
         idx1 = int(qstart)-2
         idx2 = int(sstart)-2
-        for i in range(len(qseq)): # it could be also len(sseq)
-            if qseq[i] != '-': idx1 += 1
-            if sseq[i] != '-': idx2 += 1
-            if qseq[i] == '-' or sseq[i] == '-': continue
-            resid_pairs += [(resids1[idx1],resids2[idx2])]
+        for i in range(len(qseq)):  # it could be also len(sseq)
+            if qseq[i] != '-':
+                idx1 += 1
+            if sseq[i] != '-':
+                idx2 += 1
+            if qseq[i] == '-' or sseq[i] == '-':
+                continue
+            resid_pairs += [(resids1[idx1], resids2[idx2])]
         # Check contents of the residues of the alignment
-        if len(resid_pairs) == 0: # Alignment file was empty or there was no possible matching residues between the PDBs
+        if len(resid_pairs) == 0:  # Alignment file was empty or there was no possible matching residues between the PDBs
             fu.log('Alignment file was empty or there was no possible matching residues between the PDBs' % self.tmp_folder, self.out_log)
             return False, False
         else:
             return seq_id, resid_pairs
 
     @launchlogger
     def launch(self):
         """Launches the execution of the GOdMDPrep module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Starting the work...
         # Parsing the input PDB files
         pdb1 = self.io_dict["in"]["input_pdb_orig_path"]
         pdb2 = self.io_dict["in"]["input_pdb_target_path"]
 
         # Generate sequence of first PDB
-        seq1,resids1 = self.extract_sequence(pdb1)
-                    
+        seq1, resids1 = self.extract_sequence(pdb1)
+
         # Generate sequence of second PDB
-        seq2,resids2 = self.extract_sequence(pdb2)
+        seq2, resids2 = self.extract_sequence(pdb2)
 
         if len(seq1) < 50:
             fu.log('WARNING: Short sequence (ORIGIN)' % self.tmp_folder, self.out_log)
-            #print("short_sequence ORIGIN",len(seq1))
+            # print("short_sequence ORIGIN",len(seq1))
         if len(seq2) < 50:
             fu.log('WARNING: Short sequence (TARGET)' % self.tmp_folder, self.out_log)
-            #print("short_sequence TARGET",len(seq2))
+            # print("short_sequence TARGET",len(seq2))
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
         fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
         # Produce FASTA files
         fasta1Filename = str(PurePath(self.tmp_folder).joinpath(pdb1 + ".fa"))
@@ -257,92 +265,102 @@
         fasta1File.write(">"+pdb1+"\n"+seq1)
         fasta1File.close()
         fasta2Filename = str(PurePath(self.tmp_folder).joinpath(pdb2 + ".fa"))
         fasta2File = open(fasta2Filename, "w")
         fasta2File.write(">"+pdb2+"\n"+seq2)
         fasta2File.close()
 
-        waterFilename = str(PurePath(self.tmp_folder).joinpath("water_align.out")) 
-  
-        # water -auto -outfile=water_align.out -asequence=1ake.chains.nolig.pdb.fa 
-        # -bsequence=4ake.chains.pdb.fa -gapopen=12 -gapextend=2 
+        waterFilename = str(PurePath(self.tmp_folder).joinpath("water_align.out"))
+
+        # water -auto -outfile=water_align.out -asequence=1ake.chains.nolig.pdb.fa
+        # -bsequence=4ake.chains.pdb.fa -gapopen=12 -gapextend=2
         # -datafile=EPAM250 -aformat=markx10
 
         # Command line
         self.cmd = ["water",
-               '-auto', 
-               '-outfile', waterFilename,
-               '-asequence', fasta1Filename,
-               '-bsequence', fasta2Filename,
-               '-gapopen', self.gapopen,
-               '-gapextend', self.gapextend,
-               '-datafile', self.datafile,
-               '-aformat', "markx10"
-               ]
+                    '-auto',
+                    '-outfile', waterFilename,
+                    '-asequence', fasta1Filename,
+                    '-bsequence', fasta2Filename,
+                    '-gapopen', self.gapopen,
+                    '-gapextend', self.gapextend,
+                    '-datafile', self.datafile,
+                    '-aformat', "markx10"
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
-        # Starting post-alignment process: generating .aln files 
+        # Starting post-alignment process: generating .aln files
 
         # Retrieve sequence identity of the pair, based on local sequence alignment
         # previously computed, and generate the pairs of residues from both structres
         # to drive the superimposition
         seq_id, resid_pairs = self.retrieve_alignment(waterFilename, resids1, resids2)
 
         aln1Filename = self.io_dict["out"]["output_aln_orig_path"]
         aln1File = open(aln1Filename, 'w')
         for pair in resid_pairs:
-            aln1File.write("%s%s\n" %(pair[0][1],pair[0][2].replace(" ","")))
+            aln1File.write("%s%s\n" % (pair[0][1], pair[0][2].replace(" ", "")))
         aln1File.close()
 
         aln2Filename = self.io_dict["out"]["output_aln_target_path"]
         aln2File = open(aln2Filename, 'w')
         for pair in resid_pairs:
-            aln2File.write("%s%s\n" %(pair[1][1],pair[1][2].replace(" ","")))
+            aln2File.write("%s%s\n" % (pair[1][1], pair[1][2].replace(" ", "")))
         aln2File.close()
 
+        # Copy files to host
+        self.copy_to_host()
+
         # remove temporary folder(s)
-        if self.remove_tmp:
-            self.tmp_files.append(self.tmp_folder)
-            self.remove_tmp_files()
+        self.tmp_files.extend([
+            self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
+        ])
+        self.remove_tmp_files()
+
+        self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def godmd_prep(input_pdb_orig_path: str, input_pdb_target_path: str,
-            output_aln_orig_path: str, output_aln_target_path: str, 
-            properties: dict = None, **kwargs) -> int:
+               output_aln_orig_path: str, output_aln_target_path: str,
+               properties: dict = None, **kwargs) -> int:
     """Create :class:`GOdMDPrep <godmd.godmd_prep.GOdMDPrep>`godmd.godmd_prep.GOdMDPrep class and
     execute :meth:`launch() <godmd.godmd_prep.GOdMDPrep.launch>` method"""
 
-    return GOdMDPrep( input_pdb_orig_path=input_pdb_orig_path,
-                    input_pdb_target_path=input_pdb_target_path,
-                    output_aln_orig_path=output_aln_orig_path,
-                    output_aln_target_path=output_aln_target_path,
-                    properties=properties).launch()
+    return GOdMDPrep(input_pdb_orig_path=input_pdb_orig_path,
+                     input_pdb_target_path=input_pdb_target_path,
+                     output_aln_orig_path=output_aln_orig_path,
+                     output_aln_target_path=output_aln_target_path,
+                     properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Prepares input files for the GOdMD tool.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pdb_orig_path', required=True, help='Input PDB file to be used as origin in the conformational transition. Accepted formats: pdb.')
     required_args.add_argument('--input_pdb_target_path', required=True, help='Input PDB file to be used as target in the conformational transition. Accepted formats: pdb.')
     required_args.add_argument('--output_aln_orig_path', required=True, help='Output GOdMD alignment file corresponding to the origin structure of the conformational transition. Accepted formats: aln, txt.')
     required_args.add_argument('--output_aln_target_path', required=True, help='Output GOdMD alignment file corresponding to the target structure of the conformational transition. Accepted formats: aln, txt.')
 
     args = parser.parse_args()
-    #config = args.config if args.config else None
+    # config = args.config if args.config else None
     args.config = args.config or "{}"
-    #properties = settings.ConfReader(config=config).get_prop_dic()
+    # properties = settings.ConfReader(config=config).get_prop_dic()
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    godmd_prep(      input_pdb_orig_path=args.input_pdb_orig_path,
-                    input_pdb_target_path=args.input_pdb_target_path,
-                    output_aln_orig_path=args.output_aln_orig_path,
-                    output_aln_target_path=args.output_aln_target_path,
-                    properties=properties)
+    godmd_prep(input_pdb_orig_path=args.input_pdb_orig_path,
+               input_pdb_target_path=args.input_pdb_target_path,
+               output_aln_orig_path=args.output_aln_orig_path,
+               output_aln_target_path=args.output_aln_target_path,
+               properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_godmd-3.8.1/biobb_godmd/godmd/godmd_run.py` & `biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
 
 """Module containing the GOdMDRun class and the command line interface."""
 import argparse
-import shutil, re, os
-from pathlib import Path, PurePath
+from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_godmd.godmd.common import *
+from biobb_godmd.godmd.common import check_input_path, check_output_path
+
 
 class GOdMDRun(BiobbObject):
     """
     | biobb_godmd GOdMDRun
     | Wrapper of the `GOdMD tool <http://mmb.irbbarcelona.org/GOdMD/>`_ module.
     | Computes conformational transition trajectories for proteins using GOdMD tool.
 
     Args:
         input_pdb_orig_path (str): Input PDB file to be used as origin in the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/1ake_A.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_pdb_target_path (str): Input PDB file to be used as target in the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/4ake_A.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_aln_orig_path (str): Input GOdMD alignment file corresponding to the origin structure of the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/1ake_A.aln>`_. Accepted formats: aln (edam:format_2330), txt (edam:format_2330).
         input_aln_target_path (str): Input GOdMD alignment file corresponding to the target structure of the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/4ake_A.aln>`_. Accepted formats: aln (edam:format_2330), txt (edam:format_2330).
         input_config_path (str) (Optional): Input GOdMD configuration file. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/params.in>`_. Accepted formats: in (edam:format_2330), txt (edam:format_2330).
         output_log_path (str): Output log file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd.log>`_. Accepted formats: log (edam:format_2330), out (edam:format_2330), txt (edam:format_2330), o (edam:format_2330).
-        output_ener_path (str): Output energy file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd_ene.out>`_. Accepted formats: log (edam:format_2330), out (edam:format_2330), txt (edam:format_2330), o (edam:format_2330).
+        output_ene_path (str): Output energy file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd_ene.out>`_. Accepted formats: log (edam:format_2330), out (edam:format_2330), txt (edam:format_2330), o (edam:format_2330).
         output_trj_path (str): Output trajectory file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd_trj.mdcrd>`_. Accepted formats: trj (edam:format_3878), crd (edam:format_3878), mdcrd (edam:format_3878), x (edam:format_3878).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
-            * **godmdin** (*dict*) - ({}) GOdMD options specification. 
+            * **godmdin** (*dict*) - ({}) GOdMD options specification.
             * **binary_path** (*str*) - ("discrete") Binary path.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
@@ -54,59 +54,59 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_orig_path: str, input_pdb_target_path: str,
-    input_aln_orig_path: str, input_aln_target_path: str, input_config_path: str,
-    output_log_path: str, output_ene_path: str, output_trj_path: str, 
-    properties: dict = None, **kwargs) -> None:
+                 input_aln_orig_path: str, input_aln_target_path: str, input_config_path: str,
+                 output_log_path: str, output_ene_path: str, output_trj_path: str,
+                 properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_orig_path': input_pdb_orig_path,
-                    'input_pdb_target_path': input_pdb_target_path,
-                    'input_aln_orig_path': input_aln_orig_path,
-                    'input_aln_target_path': input_aln_target_path,
-                    'input_config_path': input_config_path,
-            },
-            'out': { 'output_log_path': output_log_path,
-                     'output_ene_path': output_ene_path,
-                     'output_trj_path': output_trj_path 
-            }
+            'in': {'input_pdb_orig_path': input_pdb_orig_path,
+                   'input_pdb_target_path': input_pdb_target_path,
+                   'input_aln_orig_path': input_aln_orig_path,
+                   'input_aln_target_path': input_aln_target_path,
+                   'input_config_path': input_config_path},
+            'out': {'output_log_path': output_log_path,
+                    'output_ene_path': output_ene_path,
+                    'output_trj_path': output_trj_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.godmdin = {k: str(v) for k, v in properties.get('godmdin', dict()).items()}
         self.binary_path = properties.get('binary_path', "discrete")
 
         # Check the properties
         self.check_properties(properties)
+        # self.check_arguments()
 
     def check_data_params(self, out_log, out_err):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_pdb_orig_path"] = check_input_path(self.io_dict["in"]["input_pdb_orig_path"], "input_pdb_orig_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_pdb_target_path"] = check_input_path(self.io_dict["in"]["input_pdb_target_path"], "input_pdb_target_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_aln_orig_path"] = check_input_path(self.io_dict["in"]["input_aln_orig_path"], "input_aln_orig_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_aln_target_path"] = check_input_path(self.io_dict["in"]["input_aln_target_path"], "input_aln_target_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_config_path"] = check_input_path(self.io_dict["in"]["input_config_path"], "input_config_path", True, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_log_path"] = check_output_path(self.io_dict["out"]["output_log_path"],"output_log_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_ene_path"] = check_output_path(self.io_dict["out"]["output_ene_path"],"output_ene_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_trj_path"] = check_output_path(self.io_dict["out"]["output_trj_path"],"output_trj_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_log_path"] = check_output_path(self.io_dict["out"]["output_log_path"], "output_log_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_ene_path"] = check_output_path(self.io_dict["out"]["output_ene_path"], "output_ene_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_trj_path"] = check_output_path(self.io_dict["out"]["output_trj_path"], "output_trj_path", False, out_log, self.__class__.__name__)
 
     def create_godmdin(self, path: str = None) -> str:
         """Creates a GOdMD configuration file (godmdin) using the properties file settings"""
         godmdin_list = []
 
         self.output_godmdin_path = path
 
@@ -147,77 +147,83 @@
             for line in godmdin_list:
                 godmdin.write(line)
 
             godmdin.write("&END\n")
 
         return self.output_godmdin_path
 
-
     @launchlogger
     def launch(self):
         """Launches the execution of the GOdMDRun module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
         fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
         # Creating GOdMD input file
         self.output_godmdin_path = self.create_godmdin(path=str(Path(self.tmp_folder).joinpath("godmd.in")))
 
         # Command line
         # discrete -i $fileName.in -pdbin $pdbch1 -pdbtarg $pdbch2 -ener $fileName.ene -trj $fileName.crd -p1 $alignFile1 -p2 $alignFile2 -o $fileName.log >& $fileName.out
         self.cmd = [self.binary_path,
-               #'-i', self.io_dict["in"]["input_config_path"],
-               '-i', self.output_godmdin_path,
-               '-pdbin', self.io_dict["in"]["input_pdb_orig_path"],
-               '-pdbtarg', self.io_dict["in"]["input_pdb_target_path"],
-               '-p1', self.io_dict["in"]["input_aln_orig_path"],
-               '-p2', self.io_dict["in"]["input_aln_target_path"],
-               '-o', self.io_dict["out"]["output_log_path"],
-               '-ener', self.io_dict["out"]["output_ene_path"],
-               '-trj', self.io_dict["out"]["output_trj_path"]
-               ]
+                    # '-i', self.io_dict["in"]["input_config_path"],
+                    '-i', self.output_godmdin_path,
+                    '-pdbin', self.io_dict["in"]["input_pdb_orig_path"],
+                    '-pdbtarg', self.io_dict["in"]["input_pdb_target_path"],
+                    '-p1', self.io_dict["in"]["input_aln_orig_path"],
+                    '-p2', self.io_dict["in"]["input_aln_target_path"],
+                    '-o', self.io_dict["out"]["output_log_path"],
+                    '-ener', self.io_dict["out"]["output_ene_path"],
+                    '-trj', self.io_dict["out"]["output_trj_path"]
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        # Remove temporary folder(s)
-        if self.remove_tmp:
-            self.tmp_files.append(self.tmp_folder)
-            self.remove_tmp_files()
+        # remove temporary folder(s)
+        self.tmp_files.extend([
+            self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
+        ])
+        self.remove_tmp_files()
+
+        self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def godmd_run(input_pdb_orig_path: str, input_pdb_target_path: str,
-    input_aln_orig_path: str, input_aln_target_path: str, 
-    output_log_path: str, output_ene_path: str, output_trj_path: str,
-    input_config_path: str = None, properties: dict = None, **kwargs) -> int:
+              input_aln_orig_path: str, input_aln_target_path: str,
+              output_log_path: str, output_ene_path: str, output_trj_path: str,
+              input_config_path: str = None, properties: dict = None, **kwargs) -> int:
     """Create :class:`GOdMDRun <godmd.godmd_run.GOdMDRun>`godmd.godmd_run.GOdMDRun class and
     execute :meth:`launch() <godmd.godmd_run.GOdMDRun.launch>` method"""
 
-    return GOdMDRun( input_pdb_orig_path=input_pdb_orig_path,
+    return GOdMDRun(input_pdb_orig_path=input_pdb_orig_path,
                     input_pdb_target_path=input_pdb_target_path,
                     input_aln_orig_path=input_aln_orig_path,
                     input_aln_target_path=input_aln_target_path,
                     input_config_path=input_config_path,
                     output_log_path=output_log_path,
                     output_ene_path=output_ene_path,
                     output_trj_path=output_trj_path,
                     properties=properties).launch()
 
+
 def main():
     parser = argparse.ArgumentParser(description='Computing conformational transition trajectories for proteins using GOdMD tool.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pdb_orig_path', required=True, help='Input PDB file to be used as origin in the conformational transition. Accepted formats: pdb.')
@@ -226,25 +232,26 @@
     required_args.add_argument('--input_aln_target_path', required=True, help='Input GOdMD alignment file corresponding to the target structure of the conformational transition. Accepted formats: aln, txt.')
     required_args.add_argument('--input_config_path', required=False, help='Input configuration file (GOdMD run options). Accepted formats: in, txt.')
     required_args.add_argument('--output_log_path', required=True, help='Output log file. Accepted formats: log, out, txt.')
     required_args.add_argument('--output_ene_path', required=True, help='Output energy file. Accepted formats: log, out, txt.')
     required_args.add_argument('--output_trj_path', required=True, help='Output trajectory file. Accepted formats: mdcrd.')
 
     args = parser.parse_args()
-    #config = args.config if args.config else None
+    # config = args.config if args.config else None
     args.config = args.config or "{}"
-    #properties = settings.ConfReader(config=config).get_prop_dic()
+    # properties = settings.ConfReader(config=config).get_prop_dic()
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    godmd_run(      input_pdb_orig_path=args.input_pdb_orig_path,
-                    input_pdb_target_path=args.input_pdb_target_path,
-                    input_aln_orig_path=args.input_aln_orig_path,
-                    input_aln_target_path=args.input_aln_target_path,
-                    input_config_path=args.input_config_path,
-                    output_log_path=args.output_log_path,
-                    output_ene_path=args.output_ene_path,
-                    output_trj_path=args.output_trj_path,
-                    properties=properties)
+    godmd_run(input_pdb_orig_path=args.input_pdb_orig_path,
+              input_pdb_target_path=args.input_pdb_target_path,
+              input_aln_orig_path=args.input_aln_orig_path,
+              input_aln_target_path=args.input_aln_target_path,
+              input_config_path=args.input_config_path,
+              output_log_path=args.output_log_path,
+              output_ene_path=args.output_ene_path,
+              output_trj_path=args.output_trj_path,
+              properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_godmd-3.8.1/biobb_godmd.egg-info/PKG-INFO` & `biobb_godmd-4.0.0/biobb_godmd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: biobb-godmd
-Version: 3.8.1
+Version: 4.0.0
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.
```

### Comparing `biobb_godmd-3.8.1/setup.py` & `biobb_godmd-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_godmd",
-    version="3.8.1",
+    version="4.0.0",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).",
     long_description="Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD",
     url="https://github.com/bioexcel/biobb_godmd",
     project_urls={
         "Documentation": "http://biobb_godmd.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==3.8.1'],
-    python_requires='>=3.7',
+    install_requires=['biobb_common==4.0.0'],
+    python_requires='>=3.7,<=3.10',
     entry_points={
         "console_scripts": [
             "godmd_prep = biobb_godmd.godmd.godmd_prep:main",
             "godmd_run = biobb_godmd.godmd.godmd_run:main"
         ]
     },
     classifiers=(
```

