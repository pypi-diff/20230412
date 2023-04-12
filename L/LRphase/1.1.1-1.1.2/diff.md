# Comparing `tmp/LRphase-1.1.1.tar.gz` & `tmp/LRphase-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LRphase-1.1.1.tar", last modified: Mon Apr 10 20:03:28 2023, max compression
+gzip compressed data, was "LRphase-1.1.2.tar", last modified: Wed Apr 12 17:04:56 2023, max compression
```

## Comparing `LRphase-1.1.1.tar` & `LRphase-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     1071 2022-12-13 14:14:17.000000 LRphase-1.1.1/LICENSE
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     2031 2022-12-13 14:13:07.000000 LRphase-1.1.1/MANIFEST.in
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2023-04-10 20:03:28.442864 LRphase-1.1.1/PKG-INFO
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     5933 2023-03-07 19:40:55.000000 LRphase-1.1.1/README.md
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       91 2022-12-13 14:13:07.000000 LRphase-1.1.1/pyproject.toml
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      338 2023-04-10 20:03:28.442864 LRphase-1.1.1/setup.cfg
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     3304 2023-04-10 20:03:27.000000 LRphase-1.1.1/setup.py
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.438864 LRphase-1.1.1/src/
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/src/LRphase/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    21497 2022-12-13 14:13:07.000000 LRphase-1.1.1/src/LRphase/HeterozygousSites.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    57539 2023-03-10 18:22:15.000000 LRphase-1.1.1/src/LRphase/InputData.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    14614 2023-04-05 16:27:32.000000 LRphase-1.1.1/src/LRphase/PhasableSample.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    38006 2023-03-07 19:40:55.000000 LRphase-1.1.1/src/LRphase/PhaseSet.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    48416 2023-03-07 19:40:55.000000 LRphase-1.1.1/src/LRphase/PhasedRead.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    23245 2023-04-05 16:41:44.000000 LRphase-1.1.1/src/LRphase/SimulatePhasedData.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      202 2023-04-10 20:03:27.000000 LRphase-1.1.1/src/LRphase/__init__.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      364 2022-12-13 14:13:07.000000 LRphase-1.1.1/src/LRphase/__main__.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    64753 2023-04-10 20:03:27.000000 LRphase-1.1.1/src/LRphase/cli.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     4391 2022-12-13 14:13:07.000000 LRphase-1.1.1/src/LRphase/urls.py
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/src/LRphase.egg-info/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/PKG-INFO
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      608 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/SOURCES.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/dependency_links.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       46 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/entry_points.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2022-12-16 20:01:48.000000 LRphase-1.1.1/src/LRphase.egg-info/not-zip-safe
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      109 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/requires.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      117 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/top_level.txt
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/tests/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-13 14:13:07.000000 LRphase-1.1.1/tests/__init__.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      163 2022-12-13 14:13:07.000000 LRphase-1.1.1/tests/test_LRphase.py
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-12 17:04:56.712291 LRphase-1.1.2/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     1071 2022-12-13 14:14:17.000000 LRphase-1.1.2/LICENSE
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     2031 2022-12-13 14:13:07.000000 LRphase-1.1.2/MANIFEST.in
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2023-04-12 17:04:56.712291 LRphase-1.1.2/PKG-INFO
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     5933 2023-03-07 19:40:55.000000 LRphase-1.1.2/README.md
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       91 2022-12-13 14:13:07.000000 LRphase-1.1.2/pyproject.toml
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      338 2023-04-12 17:04:56.712291 LRphase-1.1.2/setup.cfg
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     3305 2023-04-12 17:04:56.000000 LRphase-1.1.2/setup.py
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-12 17:04:56.708291 LRphase-1.1.2/src/
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-12 17:04:56.712291 LRphase-1.1.2/src/LRphase/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    21497 2022-12-13 14:13:07.000000 LRphase-1.1.2/src/LRphase/HeterozygousSites.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    57539 2023-03-10 18:22:15.000000 LRphase-1.1.2/src/LRphase/InputData.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    14614 2023-04-11 19:27:05.000000 LRphase-1.1.2/src/LRphase/PhasableSample.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    38006 2023-03-07 19:40:55.000000 LRphase-1.1.2/src/LRphase/PhaseSet.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    48416 2023-03-07 19:40:55.000000 LRphase-1.1.2/src/LRphase/PhasedRead.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    23245 2023-04-05 16:41:44.000000 LRphase-1.1.2/src/LRphase/SimulatePhasedData.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      202 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase/__init__.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      364 2022-12-13 14:13:07.000000 LRphase-1.1.2/src/LRphase/__main__.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    64753 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase/cli.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     4391 2022-12-13 14:13:07.000000 LRphase-1.1.2/src/LRphase/urls.py
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-12 17:04:56.712291 LRphase-1.1.2/src/LRphase.egg-info/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase.egg-info/PKG-INFO
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      608 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase.egg-info/SOURCES.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase.egg-info/dependency_links.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       46 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase.egg-info/entry_points.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2022-12-16 20:01:48.000000 LRphase-1.1.2/src/LRphase.egg-info/not-zip-safe
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      110 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase.egg-info/requires.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      117 2023-04-12 17:04:56.000000 LRphase-1.1.2/src/LRphase.egg-info/top_level.txt
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-12 17:04:56.712291 LRphase-1.1.2/tests/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-13 14:13:07.000000 LRphase-1.1.2/tests/__init__.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      163 2022-12-13 14:13:07.000000 LRphase-1.1.2/tests/test_LRphase.py
```

### Comparing `LRphase-1.1.1/LICENSE` & `LRphase-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/MANIFEST.in` & `LRphase-1.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/PKG-INFO` & `LRphase-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LRphase
-Version: 1.1.1
+Version: 1.1.2
 Summary: Phasing individual long reads using known haplotype information.
 Home-page: https://github.com/Boyle-Lab/LRphase.git
 Author: Greg Farnum
 Author-email: gregfar@umich.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Boyle-Lab/LRphase/issues
 Description: # LRphase
```

### Comparing `LRphase-1.1.1/README.md` & `LRphase-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/setup.py` & `LRphase-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             return md.read()
 
 
 def main():
 
     metadata = dict(
         name = 'LRphase',
-        version = '1.1.1',
+        version = '1.1.2',
         license = 'MIT',
         description = 'Phasing individual long reads using known haplotype information.',
         description_content_type = 'text/plain',
         long_description = readme(),
         long_description_content_type = 'text/markdown',
         author = 'Greg Farnum',
         author_email = 'gregfar@umich.edu',
@@ -74,15 +74,15 @@
         ],
         python_requires = '>=3.7',
         install_requires = [
             'pysam>=0.16.0.1',
             'biopython>=1.78',
             'pyliftover>=0.4',
             'powerlaw>=1.4.6',
-            'numpy>=1.20.1'
+            'numpy>=1.20.1',
             'requests>=2.26.0'
         ],
         extras_require = {
             'mappy':['mappy'],
         },
         setup_requires=[
             'pytest-runner',
```

### Comparing `LRphase-1.1.1/src/LRphase/HeterozygousSites.py` & `LRphase-1.1.2/src/LRphase/HeterozygousSites.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/src/LRphase/InputData.py` & `LRphase-1.1.2/src/LRphase/InputData.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/src/LRphase/PhasableSample.py` & `LRphase-1.1.2/src/LRphase/PhasableSample.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/src/LRphase/PhaseSet.py` & `LRphase-1.1.2/src/LRphase/PhaseSet.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/src/LRphase/PhasedRead.py` & `LRphase-1.1.2/src/LRphase/PhasedRead.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/src/LRphase/SimulatePhasedData.py` & `LRphase-1.1.2/src/LRphase/SimulatePhasedData.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/src/LRphase/cli.py` & `LRphase-1.1.2/src/LRphase/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pysam import AlignmentFile, VariantFile
 import numpy as np
 from scipy.stats import nbinom
 import powerlaw
 import time
 from LRphase.PhaseSet import powlaw_modified, _estimate_prior_probabilities
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 # TO-DO:
 ## The main phasing function should be a wrapper that loops over samples
 # in the input VCF. Content of the current function should be moved out
 # and called once per sample in the VCF, unless args.one_sample is given.
 #@profile
 def phasing(args):
```

### Comparing `LRphase-1.1.1/src/LRphase/urls.py` & `LRphase-1.1.2/src/LRphase/urls.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.1/src/LRphase.egg-info/PKG-INFO` & `LRphase-1.1.2/src/LRphase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LRphase
-Version: 1.1.1
+Version: 1.1.2
 Summary: Phasing individual long reads using known haplotype information.
 Home-page: https://github.com/Boyle-Lab/LRphase.git
 Author: Greg Farnum
 Author-email: gregfar@umich.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Boyle-Lab/LRphase/issues
 Description: # LRphase
```

### Comparing `LRphase-1.1.1/src/LRphase.egg-info/SOURCES.txt` & `LRphase-1.1.2/src/LRphase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

