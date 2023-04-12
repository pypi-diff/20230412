# Comparing `tmp/khloraascaf-1.3.0.tar.gz` & `tmp/khloraascaf-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf-1.3.0.tar", last modified: Thu Mar 30 10:00:30 2023, max compression
+gzip compressed data, was "khloraascaf-1.4.1.tar", last modified: Wed Apr 12 09:22:50 2023, max compression
```

## Comparing `khloraascaf-1.3.0.tar` & `khloraascaf-1.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:30.007979 khloraascaf-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)    45979 2023-03-30 10:00:30.007979 khloraascaf-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4599 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 10:00:30.007979 khloraascaf-1.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:29.988977 khloraascaf-1.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:29.996978 khloraascaf-1.3.0/src/khloraascaf/
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    12407 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5164 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:30.004979 khloraascaf-1.3.0/src/khloraascaf/ilp/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10755 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/dirf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)    10725 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/invf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3350 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_max_dirf.py
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_max_invf.py
--rw-rw-rw-   0 root         (0) root         (0)     3722 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_max_presscore.py
--rw-rw-rw-   0 root         (0) root         (0)    11579 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_to_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10798 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_var_db.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12862 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/multiplied_doubled_contig_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     8303 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    27131 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/result.py
--rw-rw-rw-   0 root         (0) root         (0)     9071 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/run_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    20364 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/scaffolding_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7104 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/src/khloraascaf/utils_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:29.998978 khloraascaf-1.3.0/src/khloraascaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45979 2023-03-30 10:00:29.000000 khloraascaf-1.3.0/src/khloraascaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1148 2023-03-30 10:00:29.000000 khloraascaf-1.3.0/src/khloraascaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 10:00:29.000000 khloraascaf-1.3.0/src/khloraascaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-03-30 10:00:29.000000 khloraascaf-1.3.0/src/khloraascaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-30 10:00:29.000000 khloraascaf-1.3.0/src/khloraascaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:30.006979 khloraascaf-1.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13426 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/tests/test_assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/tests/test_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    22646 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/tests/test_toy_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-03-30 10:00:05.000000 khloraascaf-1.3.0/tests/test_utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.244232 khloraascaf-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    45979 2023-04-12 09:22:50.244232 khloraascaf-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4599 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 09:22:50.244232 khloraascaf-1.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.226231 khloraascaf-1.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.235231 khloraascaf-1.4.1/src/khloraascaf/
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12407 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5164 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.241232 khloraascaf-1.4.1/src/khloraascaf/ilp/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10970 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/dirf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/invf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_dirf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_invf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_presscore.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_repeated_fragments.py
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_to_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_var_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/multiplied_doubled_contig_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     8303 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    27131 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/result.py
+-rw-rw-rw-   0 root         (0) root         (0)     9071 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/run_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    20366 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/scaffolding_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7104 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.237232 khloraascaf-1.4.1/src/khloraascaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45979 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.243232 khloraascaf-1.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13426 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    22646 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_toy_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.3.0/LICENCE` & `khloraascaf-1.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/PKG-INFO` & `khloraascaf-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.3.0
+Version: 1.4.1
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf-1.3.0/README.md` & `khloraascaf-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/pyproject.toml` & `khloraascaf-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf"
-version = "1.3.0"
+version = "1.4.1"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/__init__.py` & `khloraascaf-1.4.1/src/khloraascaf/__init__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/__main__.py` & `khloraascaf-1.4.1/src/khloraascaf/__main__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/assembly_graph.py` & `khloraascaf-1.4.1/src/khloraascaf/assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/cli.py` & `khloraascaf-1.4.1/src/khloraascaf/cli.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/exceptions.py` & `khloraascaf-1.4.1/src/khloraascaf/exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/dirf_sets.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/dirf_sets.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     mdcg : MDCGraph
         Multiplied doubled contig graph
     v_ind : IndexT
         Vertex' index
 
     Yields
     ------
-    PInvFT
+    PDirFT
         Consecutive pairs of direct fragments
     """
     mult_v = mdcg.vertices().attr(v_ind, MULT_ATTR)
     for (i, j) in v_dirf(mdcg, v_ind):
         if j[COCC_IND] + 2 < mult_v:
             yield (
                 (i, j),
@@ -361,15 +361,17 @@
     Yields
     ------
     ForbiddenPairDirFT
         Forbidden pairing cases for direct fragments,
         enriched with an index
     """
     (i, j), (k, l) = p_dirf
-    yield 0, i, k, l, j
-    yield 1, i, l, k, j
-    yield 2, j, k, l, i
-    yield 3, j, l, k, i
-    yield 4, k, i, j, l
-    yield 5, k, j, i, l
-    yield 6, l, i, j, k
-    yield 7, l, j, i, k
+    # Forbidden order    # Alpha keys
+    # ----------------------------------
+    yield 0, i, k, l, j  # i k  k l  j l
+    yield 1, i, l, k, j  # i l  k l  j k
+    yield 2, j, k, l, i  # j k  k l  i l
+    yield 3, j, l, k, i  # j l  k l  i k
+    yield 4, k, i, j, l  # i k  i j  j l
+    yield 5, k, j, i, l  # j k  i j  i l
+    yield 6, l, i, j, k  # i l  i j  j k
+    yield 7, l, j, i, k  # j l  i j  i k
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/invf_sets.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/invf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_circuit.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_circuit.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_max_dirf.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_dirf.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 )
 from khloraascaf.ilp.pulp_repeated_fragments import (
     adjacent_fragments,
     alpha_definition,
     fix_repeats_subpaths,
     forbidden_pairing_definition,
     longuest_contiguous_repeat,
-    occurences_priority,
+    occurrences_priority,
     pairs_in_path,
+    pairs_priority,
 )
 from khloraascaf.ilp.pulp_var_db import PuLPVarDirFModel
 from khloraascaf.multiplied_doubled_contig_graph import MDCGraph, OccOrCT
 from khloraascaf.result import ScaffoldingResult
 
 
 # ============================================================================ #
@@ -59,15 +60,15 @@
     # Problem
     # ------------------------------------------------------------------------ #
     prob = LpProblem(name='inters_dirf', sense=LpMaximize)
 
     # ------------------------------------------------------------------------ #
     # Variables
     # ------------------------------------------------------------------------ #
-    var = PuLPVarDirFModel(mdcg, starter_vertex, big_m)
+    var = PuLPVarDirFModel(mdcg, starter_vertex)
 
     # ------------------------------------------------------------------------ #
     # Objective function
     # ------------------------------------------------------------------------ #
     longuest_contiguous_repeat(prob, var, mdcg)
 
     # ------------------------------------------------------------------------ #
@@ -90,12 +91,16 @@
     # Fix repeats sub-paths
     #
     if fix_result is not None:
         fix_repeats_subpaths(prob, var, fix_result)
         # TODO avoid pairs for fixed sub-paths
     else:
         #
-        # Speed-up the model
+        # Speed-up
         #
-        occurences_priority(prob, var, mdcg)
+        pairs_priority(prob, var, mdcg)
+    #
+    # Speed-up
+    #
+    occurrences_priority(prob, var, mdcg)
 
     return prob, var
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_max_invf.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_invf.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 )
 from khloraascaf.ilp.pulp_repeated_fragments import (
     adjacent_fragments,
     alpha_definition,
     fix_repeats_subpaths,
     forbidden_pairing_definition,
     longuest_contiguous_repeat,
-    occurences_priority,
+    occurrences_priority,
     pairs_in_path,
+    pairs_priority,
 )
 from khloraascaf.ilp.pulp_var_db import PuLPVarInvFModel
 from khloraascaf.multiplied_doubled_contig_graph import MDCGraph, OccOrCT
 from khloraascaf.result import ScaffoldingResult
 
 
 # ============================================================================ #
@@ -59,15 +60,15 @@
     # Problem
     # ------------------------------------------------------------------------ #
     prob = LpProblem(name='nested_invf', sense=LpMaximize)
 
     # ------------------------------------------------------------------------ #
     # Variables
     # ------------------------------------------------------------------------ #
-    var = PuLPVarInvFModel(mdcg, starter_vertex, big_m)
+    var = PuLPVarInvFModel(mdcg, starter_vertex)
 
     # ------------------------------------------------------------------------ #
     # Objective function
     # ------------------------------------------------------------------------ #
     longuest_contiguous_repeat(prob, var, mdcg)
 
     # ------------------------------------------------------------------------ #
@@ -90,12 +91,16 @@
     # Fix repeats sub-paths
     #
     if fix_result is not None:
         fix_repeats_subpaths(prob, var, fix_result)
         # TODO avoid pairs for fixed sub-paths
     else:
         #
-        # Speed-up the model
+        # Speed-up
         #
-        occurences_priority(prob, var, mdcg)
+        pairs_priority(prob, var, mdcg)
+    #
+    # Speed-up
+    #
+    occurrences_priority(prob, var, mdcg)
 
     return prob, var
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_max_presscore.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_presscore.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from pulp import LpMaximize, LpProblem, lpSum
 
 from khloraascaf.ilp.pulp_circuit import (
     circuit_from_the_starter_forward,
     flow_definition,
     intermediate_in_circuit,
 )
-from khloraascaf.ilp.pulp_repeated_fragments import fix_repeats_subpaths
+from khloraascaf.ilp.pulp_repeated_fragments import (
+    fix_repeats_subpaths,
+    occurrences_priority,
+)
 from khloraascaf.ilp.pulp_var_db import PuLPVarPresScoreModel
 from khloraascaf.multiplied_doubled_contig_graph import (
     CIND_IND,
     PRESSCORE_ATTR,
     MDCGraph,
     OccOrCT,
 )
@@ -55,15 +58,15 @@
     # Problem
     # ------------------------------------------------------------------------ #
     prob = LpProblem(name='best_presscore', sense=LpMaximize)
 
     # ------------------------------------------------------------------------ #
     # Variables
     # ------------------------------------------------------------------------ #
-    var = PuLPVarPresScoreModel(mdcg, starter_vertex, big_m)
+    var = PuLPVarPresScoreModel(mdcg, starter_vertex)
 
     # ------------------------------------------------------------------------ #
     # Objective function
     # ------------------------------------------------------------------------ #
     __presscore_objective(prob, var, mdcg)
 
     # ------------------------------------------------------------------------ #
@@ -76,16 +79,18 @@
     circuit_from_the_starter_forward(prob, var, mdcg, starter_vertex)
     intermediate_in_circuit(prob, var, mdcg, starter_vertex)
     #
     # Fix repeats sub-paths
     #
     if fix_result is not None:
         fix_repeats_subpaths(prob, var, fix_result)
-    # OPTIMIZE occurrence priority?
-    #   * can it be generalisable for pairs?
+    #
+    # Speed-up
+    #
+    occurrences_priority(prob, var, mdcg)
     return prob, var
 
 
 # ============================================================================ #
 #                              OBJECTIVE FUNCTION                              #
 # ============================================================================ #
 def __presscore_objective(prob: LpProblem, var: PuLPVarPresScoreModel,
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_repeated_fragments.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_repeated_fragments.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 
 from pulp import LpAffineExpression, LpProblem, lpSum
 from revsymg.index_lib import FORWARD_INT, REVERSE_INT
 
 from khloraascaf.ilp.dirf_sets import dirf_other
 from khloraascaf.ilp.invf_sets import invf_other
-from khloraascaf.ilp.pulp_var_db import PuLPVarPath, PuLPVarRepFModelT
+from khloraascaf.ilp.pulp_var_db import (
+    PuLPVarModelT,
+    PuLPVarPath,
+    PuLPVarRepFModelT,
+)
 from khloraascaf.multiplied_doubled_contig_graph import (
     MULT_ATTR,
     MDCGraph,
     OccOrCT,
 )
 from khloraascaf.result import ScaffoldingResult
 
@@ -212,59 +216,76 @@
         #
         prob += var.isadj[u, v] <= var.m[q]
 
 
 # ---------------------------------------------------------------------------- #
 #                              Speed-up The Model                              #
 # ---------------------------------------------------------------------------- #
-def occurences_priority(prob: LpProblem,
-                        var: PuLPVarRepFModelT,
-                        mdcg: MDCGraph):
-    """Constraint for occurences priority.
+def occurrences_priority(prob: LpProblem,
+                         var: PuLPVarModelT,
+                         mdcg: MDCGraph):
+    """Constraint for occurrences priority.
 
     Parameters
     ----------
     prob : LpProblem
         PuLP problem
     var : PuLPVarInvFModel or PuLPVarDirFModel
         PuLP variables
     mdcg : MDCGraph
         Multiplied doubled contig graph
     """
     vertices = mdcg.vertices()
     for u_ind in mdcg.repeated_contigs():
         #
-        # Consecutive pairs of inverted fragments priority
-        #
-        for p, q in type(var).pair_repeat_consecutive_fn(mdcg, u_ind):
-            prob += var.m[q] <= var.m[p]
-        #
         # Vertices occurrence priority
         #
         for u_occ in range(vertices.attr(u_ind, MULT_ATTR) - 1):
             prob += (
                 var.i[(u_ind, FORWARD_INT, u_occ + 1)]
                 + var.i[(u_ind, REVERSE_INT, u_occ + 1)]
                 <= var.i[(u_ind, FORWARD_INT, u_occ)]
                 + var.i[(u_ind, REVERSE_INT, u_occ)]
             )
 
 
+def pairs_priority(prob: LpProblem,
+                   var: PuLPVarRepFModelT,
+                   mdcg: MDCGraph):
+    """Constraint for pairs priority.
+
+    Parameters
+    ----------
+    prob : LpProblem
+        PuLP problem
+    var : PuLPVarInvFModel or PuLPVarDirFModel
+        PuLP variables
+    mdcg : MDCGraph
+        Multiplied doubled contig graph
+    """
+    for u_ind in mdcg.repeated_contigs():
+        #
+        # Consecutive pairs of inverted fragments priority
+        #
+        for p, q in type(var).pair_repeat_consecutive_fn(mdcg, u_ind):
+            prob += var.m[q] <= var.m[p]
+
+
 # ---------------------------------------------------------------------------- #
 #                               Keep Old Repeats                               #
 # ---------------------------------------------------------------------------- #
 def fix_repeats_subpaths(prob: LpProblem, var: PuLPVarPath,
                          fix_result: ScaffoldingResult):
     """Fix subpaths corresponding to repeats.
 
     Parameters
     ----------
     prob : LpProblem
         PuLP problem
-    var : PuLPVarPresScoreModel
+    var : PuLPVarPath
         PuLP variables
     fix_result : ScaffoldingResult
         Previous scaffolding result
     """
     # ------------------------------------------------------------------------ #
     # Inverted repeats
     # ------------------------------------------------------------------------ #
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_to_solver.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_to_solver.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/ilp/pulp_var_db.py` & `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_var_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The PuLPVarDB classes file."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Iterator, Union
 
-from pulp import LpBinary, LpContinuous, LpInteger, LpVariable
+from pulp import LpBinary, LpContinuous, LpVariable
 from pulp.pulp import LpAffineExpression
 from revsymg.index_lib import IndexT
 
 from khloraascaf.ilp.dirf_sets import (
     DirFT,
     adirf,
     adirf_other,
@@ -52,15 +52,14 @@
 # ============================================================================ #
 #                                     TYPES                                    #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                                Path Variables                                #
 # ---------------------------------------------------------------------------- #
 DiVarT = dict[OccOrCT, LpVariable]
-DposVarT = dict[OccOrCT, LpVariable]
 DxVarT = dict[EOccOrCT, LpVariable]
 DfVarT = dict[EOccOrCT, LpVariable]
 
 # ---------------------------------------------------------------------------- #
 #                                InvF Variables                                #
 # ---------------------------------------------------------------------------- #
 DmInvFVarT = dict[InvFT, LpVariable]
@@ -89,25 +88,21 @@
 # ---------------------------------------------------------------------------- #
 #                                 Base Classes                                 #
 # ---------------------------------------------------------------------------- #
 @dataclass
 class PuLPVarPath():
     """Data class for necessary variables to modelise a path."""
 
-    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT, big_m: int):
+    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT):
         """The Initializer."""
         self.i: DiVarT = {
             v: LpVariable(f'i_{v}', cat=LpContinuous)
             for v in mdcg.multiplied_vertices()
             if v[CIND_IND] != starter_vertex[CIND_IND]
         }
-        self.pos: DposVarT = {
-            v: LpVariable(f'pos_{v}', lowBound=0, upBound=big_m, cat=LpInteger)
-            for v in mdcg.multiplied_vertices()
-        }
         self.x: DxVarT = {
             e: LpVariable(f'x_{e}', cat=LpBinary)
             for e in mdcg.multiplied_edges()
         }
         self.f: DfVarT = {
             e: LpVariable(f'f_{e}', lowBound=0, cat=LpContinuous)
             for e in mdcg.multiplied_edges()
@@ -134,15 +129,15 @@
             for p in PuLPVarInvF.repeat_frag_fn(mdcg)
         }
         self._alpha: DalphaVarT = {
             (u, v): LpVariable(f'alpha_{u}_{v}', cat=LpBinary)
             for u, v in PuLPVarInvF.pair_repeat_alpha_fn(mdcg)
         }
         self.pairing_ban: DintersVarT = {
-            (k, p, q): LpVariable(f'inters_{k}_{p}_{q}', cat=LpBinary)
+            (k, p, q): LpVariable(f'forbid_{k}_{p}_{q}', cat=LpBinary)
             for p, q in PuLPVarInvF.pair_repeat_frag_fn(mdcg)
             for k in range(8)
         }
         self.isadj: DisadjVarT = {
             (u, v): LpVariable(f'isadj_{u}_{v}', cat=LpBinary)
             for u, v in PuLPVarInvF.adj_repeat_frag_fn(mdcg)
         }
@@ -204,15 +199,15 @@
             for p in PuLPVarDirF.repeat_frag_fn(mdcg)
         }
         self._alpha: DalphaVarT = {
             (u, v): LpVariable(f'alpha_{u}_{v}', cat=LpBinary)
             for u, v in PuLPVarDirF.pair_repeat_alpha_fn(mdcg)
         }
         self.pairing_ban: DnestedVarT = {
-            (k, p, q): LpVariable(f'nested_{k}_{p}_{q}', cat=LpBinary)
+            (k, p, q): LpVariable(f'forbid_{k}_{p}_{q}', cat=LpBinary)
             for k in range(8)
             for p, q in PuLPVarDirF.pair_repeat_frag_fn(mdcg)
         }
         self.isadj: DisadjVarT = {
             (u, v): LpVariable(f'isadj_{u}_{v}', cat=LpBinary)
             for u, v in PuLPVarDirF.adj_repeat_frag_fn(mdcg)
         }
@@ -257,34 +252,34 @@
 # ---------------------------------------------------------------------------- #
 #                                 Model Classes                                #
 # ---------------------------------------------------------------------------- #
 @dataclass
 class PuLPVarInvFModel(PuLPVarPath, PuLPVarInvF):
     """Data class for necessary variables to modelise invf model."""
 
-    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT, big_m: int):
-        PuLPVarPath.__init__(self, mdcg, starter_vertex, big_m)
+    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT):
+        PuLPVarPath.__init__(self, mdcg, starter_vertex)
         PuLPVarInvF.__init__(self, mdcg)
 
 
 @dataclass
 class PuLPVarDirFModel(PuLPVarPath, PuLPVarDirF):
     """Data class for necessary variables to modelise dirf model."""
 
-    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT, big_m: int):
-        PuLPVarPath.__init__(self, mdcg, starter_vertex, big_m)
+    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT):
+        PuLPVarPath.__init__(self, mdcg, starter_vertex)
         PuLPVarDirF.__init__(self, mdcg)
 
 
 @dataclass
 class PuLPVarPresScoreModel(PuLPVarPath):
     """Data class for necessary variables to modelise presscore model."""
 
-    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT, big_m: int):
-        PuLPVarPath.__init__(self, mdcg, starter_vertex, big_m)
+    def __init__(self, mdcg: MDCGraph, starter_vertex: OccOrCT):
+        PuLPVarPath.__init__(self, mdcg, starter_vertex)
 
 
 PuLPVarRepFModelT = Union[PuLPVarInvFModel, PuLPVarDirFModel]
 PuLPVarModelT = Union[PuLPVarRepFModelT, PuLPVarPresScoreModel]
 
 
 # ============================================================================ #
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/inputs.py` & `khloraascaf-1.4.1/src/khloraascaf/inputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/lib.py` & `khloraascaf-1.4.1/src/khloraascaf/lib.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/multiplied_doubled_contig_graph.py` & `khloraascaf-1.4.1/src/khloraascaf/multiplied_doubled_contig_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         Note
         ----
         The list is sorted
         """
         return self.__repeated_contigs
 
     def multiplied_card(self) -> int:
-        """The number of occurend oriented contig.
+        """The number of multiplied oriented contig.
 
         Returns
         -------
         int
             The number of vertices in multiplied doubled contig graph
         """
         return 2 * sum(
@@ -342,26 +342,26 @@
     -------
     OccOrCT
         Reverse of the multiplied oriented contig
     """
     return v[CIND_IND], ORIENT_REV[v[COR_IND]], v[COCC_IND]
 
 
-def first_forward_occurence(vertex_index: IndexT) -> OccOrCT:
-    """Returns the first forward occurence with given vertex index.
+def first_forward_occurrence(vertex_index: IndexT) -> OccOrCT:
+    """Returns the first forward occurrence with given vertex index.
 
     Parameters
     ----------
     vertex_index : IndexT
         Contig's index
 
     Returns
     -------
     OccOrCT
-        The first occurence, in forward orientation with the given vertex index
+        The first occurrence, in forward orientation with the given vertex index
     """
     return vertex_index, FORWARD_INT, 0
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Constructors                                 #
 # ---------------------------------------------------------------------------- #
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/outputs.py` & `khloraascaf-1.4.1/src/khloraascaf/outputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/result.py` & `khloraascaf-1.4.1/src/khloraascaf/result.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/run_metadata.py` & `khloraascaf-1.4.1/src/khloraascaf/run_metadata.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf/scaffolding_methods.py` & `khloraascaf-1.4.1/src/khloraascaf/scaffolding_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     SC_CODE,
     RegionCodeT,
 )
 from khloraascaf.multiplied_doubled_contig_graph import (
     MDCGraph,
     MDCGraphIDContainer,
     OccOrCT,
-    first_forward_occurence,
+    first_forward_occurrence,
     mdcg_with_id_from_input_files,
 )
 from khloraascaf.outputs import (
     fmt_contigs_of_regions_filename,
     fmt_map_of_regions_filename,
     generate_output_directory,
     write_contigs_of_regions,
@@ -168,15 +168,15 @@
     # ------------------------------------------------------------------------ #
     # TODO what to do if several optimal solutions?
     #   * solution should be a list of results?
     #   * how to tell which results was selected?
     #   * metadata on the outputs (human reading)?
     try:
         solutions = combine_scaffolding_problems(
-            mdcg, first_forward_occurence(
+            mdcg, first_forward_occurrence(
                 id_container.contig_to_vertex(contig_starter)),
             solver, outdir_gen, instance_name,
             debug=debug,
         )
     except CombineScaffoldingError as exc:
         # TODO logging exception
         raise ScaffoldingError(outdir_gen) from exc
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf/utils_debug.py` & `khloraascaf-1.4.1/src/khloraascaf/utils_debug.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/src/khloraascaf.egg-info/PKG-INFO` & `khloraascaf-1.4.1/src/khloraascaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.3.0
+Version: 1.4.1
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf-1.3.0/src/khloraascaf.egg-info/SOURCES.txt` & `khloraascaf-1.4.1/src/khloraascaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/tests/test_assembly_graph.py` & `khloraascaf-1.4.1/tests/test_assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/tests/test_exceptions.py` & `khloraascaf-1.4.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/tests/test_toy_examples.py` & `khloraascaf-1.4.1/tests/test_toy_examples.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.3.0/tests/test_utils_debug.py` & `khloraascaf-1.4.1/tests/test_utils_debug.py`

 * *Files identical despite different names*

