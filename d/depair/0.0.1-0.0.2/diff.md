# Comparing `tmp/depair-0.0.1.tar.gz` & `tmp/depair-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depair-0.0.1.tar", last modified: Fri Dec 23 09:07:47 2022, max compression
+gzip compressed data, was "depair-0.0.2.tar", last modified: Wed Apr 12 06:52:28 2023, max compression
```

## Comparing `depair-0.0.1.tar` & `depair-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 chensijie   (501) staff       (20)        0 2022-12-23 09:07:47.882894 depair-0.0.1/
--rw-r--r--   0 chensijie   (501) staff       (20)     1071 2022-12-23 08:55:39.000000 depair-0.0.1/LICENSE
--rw-r--r--   0 chensijie   (501) staff       (20)      476 2022-12-23 09:07:47.882764 depair-0.0.1/PKG-INFO
--rw-r--r--   0 chensijie   (501) staff       (20)     2015 2022-12-23 07:50:24.000000 depair-0.0.1/README.md
-drwxr-xr-x   0 chensijie   (501) staff       (20)        0 2022-12-23 09:07:47.881353 depair-0.0.1/depair/
--rw-r--r--   0 chensijie   (501) staff       (20)       16 2022-12-23 08:57:51.000000 depair-0.0.1/depair/__init__.py
--rw-r--r--   0 chensijie   (501) staff       (20)    16917 2022-12-23 08:37:27.000000 depair-0.0.1/depair/eval.py
-drwxr-xr-x   0 chensijie   (501) staff       (20)        0 2022-12-23 09:07:47.882597 depair-0.0.1/depair.egg-info/
--rw-r--r--   0 chensijie   (501) staff       (20)      476 2022-12-23 09:07:47.000000 depair-0.0.1/depair.egg-info/PKG-INFO
--rw-r--r--   0 chensijie   (501) staff       (20)      180 2022-12-23 09:07:47.000000 depair-0.0.1/depair.egg-info/SOURCES.txt
--rw-r--r--   0 chensijie   (501) staff       (20)        1 2022-12-23 09:07:47.000000 depair-0.0.1/depair.egg-info/dependency_links.txt
--rw-r--r--   0 chensijie   (501) staff       (20)        7 2022-12-23 09:07:47.000000 depair-0.0.1/depair.egg-info/top_level.txt
--rw-r--r--   0 chensijie   (501) staff       (20)       38 2022-12-23 09:07:47.882936 depair-0.0.1/setup.cfg
--rw-r--r--   0 chensijie   (501) staff       (20)      598 2022-12-23 09:07:13.000000 depair-0.0.1/setup.py
+drwxr-xr-x   0 chensijie   (501) staff       (20)        0 2023-04-12 06:52:28.903148 depair-0.0.2/
+-rw-r--r--   0 chensijie   (501) staff       (20)     1071 2022-12-23 08:55:39.000000 depair-0.0.2/LICENSE
+-rw-r--r--   0 chensijie   (501) staff       (20)      476 2023-04-12 06:52:28.902990 depair-0.0.2/PKG-INFO
+-rw-r--r--   0 chensijie   (501) staff       (20)     2069 2022-12-23 09:17:10.000000 depair-0.0.2/README.md
+drwxr-xr-x   0 chensijie   (501) staff       (20)        0 2023-04-12 06:52:28.901901 depair-0.0.2/depair/
+-rw-r--r--   0 chensijie   (501) staff       (20)       16 2022-12-23 08:57:51.000000 depair-0.0.2/depair/__init__.py
+-rw-r--r--   0 chensijie   (501) staff       (20)    17017 2023-04-12 06:44:15.000000 depair-0.0.2/depair/eval.py
+drwxr-xr-x   0 chensijie   (501) staff       (20)        0 2023-04-12 06:52:28.902802 depair-0.0.2/depair.egg-info/
+-rw-r--r--   0 chensijie   (501) staff       (20)      476 2023-04-12 06:52:28.000000 depair-0.0.2/depair.egg-info/PKG-INFO
+-rw-r--r--   0 chensijie   (501) staff       (20)      180 2023-04-12 06:52:28.000000 depair-0.0.2/depair.egg-info/SOURCES.txt
+-rw-r--r--   0 chensijie   (501) staff       (20)        1 2023-04-12 06:52:28.000000 depair-0.0.2/depair.egg-info/dependency_links.txt
+-rw-r--r--   0 chensijie   (501) staff       (20)        7 2023-04-12 06:52:28.000000 depair-0.0.2/depair.egg-info/top_level.txt
+-rw-r--r--   0 chensijie   (501) staff       (20)       38 2023-04-12 06:52:28.903190 depair-0.0.2/setup.cfg
+-rw-r--r--   0 chensijie   (501) staff       (20)      599 2023-04-12 06:44:15.000000 depair-0.0.2/setup.py
```

### Comparing `depair-0.0.1/LICENSE` & `depair-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `depair-0.0.1/README.md` & `depair-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ---
 
 DEPair evaluates ligand-receptor mediated crosstalks among cell populations. 
 A interaction score as well as its significance is given for each pair of clusters with DEPair.
 DEPair also identifies the variable interactions between different groups.
 
-DEPair is really easy.
+You can install DEPair via `pip install depair`.
 
 ```
 import numpy as np,scanpy as sc,anndata as ad,pandas as pd
 import os,pickle,random
 import matplotlib.pyplot as plt
 from dfply import *
 
@@ -45,25 +45,26 @@
 
 - [x] crosstalk intensity evaluation 
 - [x] permutation-based crosstalk significance calculation
 - [x] permutation speed up
 - [x] human and mouse ligand-receptor databases
 - [ ] ligand-receptor databases for other species 
 - [ ] a tutorial as well as a document online at readthedocs
-- [ ] upload to pypi
+- [x] upload to pypi
 - [ ] spatial transcriptomics support
 - [ ] multi subunit analysis support
 - [ ] ligand-receptor database with detailed annotation
 - [ ] clustering granularity selection
 - [ ] visualization
 - [ ] scanpy support
 - [ ] supergraph exploration
 
 ---
 
 ## News
 - 2021-04-08  prerelease test version online
 - 2021-04-30  Qijin Yin contributed the permutation speed up codes
+- 2022-12-23 upload to pypi
 
 ---
 
 contributors: Sijie Chen, Qijin Yin
```

### Comparing `depair-0.0.1/depair/eval.py` & `depair-0.0.2/depair/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
                  (pseudo_expr +crosstalk[(i,j)]["intensity"].to_numpy())/ 
                  (pseudo_expr +avg_randintensity[idx_i,idx_j])  )
     
                 
     return crosstalk    
 
 
-def crosstalk(anndata, LRDB_table, groupby, n_perm=1000, n_jobs=1, 
+def crosstalk(anndata, LRDB_table, groupby, n_perm=1000, n_jobs=1, eval_significance=True,
               verbose=False, pgb_notebook=False, pseudo_expr=1e-5):
     """
     crosstalk analysis
     anndata: an AnnData object
     LRDB_table: a pandas.DataFrame contains `ligand_symbol` column and `receptor_symbol` column
     groupby: a column key in adata.obs specifying cell types
     n_perm: number of permutations to calculate crosstalk intensity significance. Default = 1000
@@ -369,26 +369,26 @@
     
     # drop the genes that are not present in the data 
     adata_trim, LRDB = __primary_trimming(anndata, LRDB_table, groupby=groupby)
     
     # get intensity scores of the cellular crosstalks
     crosstalk   = __get_crosstalk(adata_trim, groupby=groupby, LRDB=LRDB, verbose=verbose, pgb_notebook=pgb_notebook)
     
-    
-    # get the significance of the intensities
-    if verbose:
-        print("Evaluation of interaction significances: randomly permuting %d times"%n_perm)
-    else:
-        import warnings; warnings.filterwarnings("ignore");
-    
-    if n_jobs==1: # serial exec
-        if verbose: print("single-core run");
-        crosstalk = __get_significance(adata_trim, crosstalk, LRDB, n_perm=n_perm, groupby=groupby,
-                                       pseudo_expr=pseudo_expr,
-                                       verbose=verbose, pgb_notebook=pgb_notebook )
-    else:
-        if verbose: print("%d-core run"%n_jobs);
-        crosstalk = __get_significance_parallel(adata_trim, crosstalk, LRDB, n_perm=n_perm, groupby=groupby,
-                                                pseudo_expr=pseudo_expr,
-                                                n_jobs=n_jobs )
+    if eval_significance:
+        # get the significance of the intensities
+        if verbose:
+            print("Evaluation of interaction significances: randomly permuting %d times"%n_perm)
+        else:
+            import warnings; warnings.filterwarnings("ignore");
+
+        if n_jobs==1: # serial exec
+            if verbose: print("single-core run");
+            crosstalk = __get_significance(adata_trim, crosstalk, LRDB, n_perm=n_perm, groupby=groupby,
+                                           pseudo_expr=pseudo_expr,
+                                           verbose=verbose, pgb_notebook=pgb_notebook )
+        else:
+            if verbose: print("%d-core run"%n_jobs);
+            crosstalk = __get_significance_parallel(adata_trim, crosstalk, LRDB, n_perm=n_perm, groupby=groupby,
+                                                    pseudo_expr=pseudo_expr,
+                                                    n_jobs=n_jobs )
     
     return crosstalk
```

### Comparing `depair-0.0.1/setup.py` & `depair-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 long_description = "a scanpy-based single-cell crosstalk analysis package"
 
 setuptools.setup(
   name="depair",
-  version="0.0.1",
+  version="0.0.2",
   author="Sijie Chen",
   author_email="chansigit@gmail.com",
   description="A scanpy-based single-cell crosstalk analysis package",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/chansigit/depair",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
-)
+)
```

