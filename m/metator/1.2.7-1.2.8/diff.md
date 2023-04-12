# Comparing `tmp/metator-1.2.7.tar.gz` & `tmp/metator-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metator-1.2.7.tar", last modified: Fri Apr  7 07:54:29 2023, max compression
+gzip compressed data, was "metator-1.2.8.tar", last modified: Wed Apr 12 10:36:04 2023, max compression
```

## Comparing `metator-1.2.7.tar` & `metator-1.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:54:29.843555 metator-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-04-07 07:54:18.000000 metator-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-07 07:54:18.000000 metator-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-04-07 07:54:29.843555 metator-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-04-07 07:54:18.000000 metator-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:54:29.843555 metator-1.2.7/metator/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-07 07:54:18.000000 metator-1.2.7/metator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-04-07 07:54:18.000000 metator-1.2.7/metator/align.py
--rw-r--r--   0 runner    (1001) docker     (123)    59703 2023-04-07 07:54:18.000000 metator-1.2.7/metator/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-04-07 07:54:18.000000 metator-1.2.7/metator/contact_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    24780 2023-04-07 07:54:18.000000 metator-1.2.7/metator/figures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-04-07 07:54:18.000000 metator-1.2.7/metator/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-07 07:54:18.000000 metator-1.2.7/metator/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-07 07:54:18.000000 metator-1.2.7/metator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-04-07 07:54:18.000000 metator-1.2.7/metator/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-04-07 07:54:18.000000 metator-1.2.7/metator/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-04-07 07:54:18.000000 metator-1.2.7/metator/quality_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-04-07 07:54:18.000000 metator-1.2.7/metator/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-04-07 07:54:18.000000 metator-1.2.7/metator/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)    41117 2023-04-07 07:54:18.000000 metator-1.2.7/metator/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 07:54:29.000000 metator-1.2.7/metator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:54:29.843555 metator-1.2.7/metator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-04-07 07:54:29.000000 metator-1.2.7/metator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 07:54:29.000000 metator-1.2.7/metator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 07:54:29.000000 metator-1.2.7/metator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-07 07:54:29.000000 metator-1.2.7/metator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-07 07:54:29.000000 metator-1.2.7/metator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 07:54:29.000000 metator-1.2.7/metator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-07 07:54:18.000000 metator-1.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-07 07:54:29.843555 metator-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-07 07:54:18.000000 metator-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:36:04.160029 metator-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-04-12 10:35:38.000000 metator-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 10:35:38.000000 metator-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-04-12 10:36:04.160029 metator-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-04-12 10:35:38.000000 metator-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:36:04.160029 metator-1.2.8/metator/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 10:35:38.000000 metator-1.2.8/metator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-04-12 10:35:38.000000 metator-1.2.8/metator/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59703 2023-04-12 10:35:38.000000 metator-1.2.8/metator/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-04-12 10:35:38.000000 metator-1.2.8/metator/contact_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24780 2023-04-12 10:35:38.000000 metator-1.2.8/metator/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-04-12 10:35:38.000000 metator-1.2.8/metator/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-12 10:35:38.000000 metator-1.2.8/metator/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-12 10:35:38.000000 metator-1.2.8/metator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-04-12 10:35:38.000000 metator-1.2.8/metator/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-04-12 10:35:38.000000 metator-1.2.8/metator/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-04-12 10:35:38.000000 metator-1.2.8/metator/quality_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-04-12 10:35:38.000000 metator-1.2.8/metator/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-04-12 10:35:38.000000 metator-1.2.8/metator/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41117 2023-04-12 10:35:38.000000 metator-1.2.8/metator/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 10:36:02.000000 metator-1.2.8/metator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:36:04.160029 metator-1.2.8/metator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-04-12 10:36:03.000000 metator-1.2.8/metator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 10:36:04.000000 metator-1.2.8/metator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:36:03.000000 metator-1.2.8/metator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 10:36:03.000000 metator-1.2.8/metator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 10:36:03.000000 metator-1.2.8/metator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 10:36:03.000000 metator-1.2.8/metator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 10:35:38.000000 metator-1.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 10:36:04.160029 metator-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-12 10:35:38.000000 metator-1.2.8/setup.py
```

### Comparing `metator-1.2.7/LICENSE` & `metator-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/PKG-INFO` & `metator-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metator
-Version: 1.2.7
+Version: 1.2.8
 Summary: A pipeline for binning metagenomic datasets from metaHiC data.
 Home-page: https://github.com/koszullab/metator
 Author: amaury.bignaud@pasteur.fr
 License: GPLv3
 Description: # MetaTOR
         
         [![PyPI version](https://badge.fury.io/py/metator.svg)](https://badge.fury.io/py/metator)
```

### Comparing `metator-1.2.7/README.md` & `metator-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/__init__.py` & `metator-1.2.8/metator/__init__.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/align.py` & `metator-1.2.8/metator/align.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/commands.py` & `metator-1.2.8/metator/commands.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/contact_map.py` & `metator-1.2.8/metator/contact_map.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/figures.py` & `metator-1.2.8/metator/figures.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/io.py` & `metator-1.2.8/metator/io.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/log.py` & `metator-1.2.8/metator/log.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/main.py` & `metator-1.2.8/metator/main.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/network.py` & `metator-1.2.8/metator/network.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/partition.py` & `metator-1.2.8/metator/partition.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/quality_check.py` & `metator-1.2.8/metator/quality_check.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/regions.py` & `metator-1.2.8/metator/regions.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/scaffold.py` & `metator-1.2.8/metator/scaffold.py`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/metator/validation.py` & `metator-1.2.8/metator/validation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -862,30 +862,30 @@
         else:
             src = join(recursive_fasta_dir, f"step_{step}", f"{bin_name}.fa")
         shutil.copyfile(src, dst)
 
     # Return some values of efficiency of the binning.
     give_results_info(bin_summary)
 
+    # Correct final bin value in contigs data
+    contigs_data = correct_final_bin(contigs_data, final_fasta_dir, bin_summary)
+
     # Write relevant bins/contigs information for anvio.
     binning_file = join(outdir, "binning.txt")
     contigs_data = write_bins_contigs(
         bin_summary, contigs_data, binning_file, prefix
     )
 
     # Compute the abundance of the mags.
     bin_summary = get_bin_coverage(bin_summary, contigs_data)
 
     # Save bin information in final file
     bin_summary_file = join(outdir, "bin_summary.txt")
     mio.write_bin_summary(bin_summary, bin_summary_file)
 
-    # Correct final bin value in contigs data
-    contigs_data = correct_final_bin(contigs_data, final_fasta_dir, bin_summary)
-
     # Write the new file
     contig_data_file_final = join(outdir, "contig_data_final.txt")
     contigs_data.to_csv(
         contig_data_file_final, sep="\t", header=True, index=True
     )
 
     # Plot some figures of contigs distribution inside bins:
```

### Comparing `metator-1.2.7/metator.egg-info/PKG-INFO` & `metator-1.2.8/metator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metator
-Version: 1.2.7
+Version: 1.2.8
 Summary: A pipeline for binning metagenomic datasets from metaHiC data.
 Home-page: https://github.com/koszullab/metator
 Author: amaury.bignaud@pasteur.fr
 License: GPLv3
 Description: # MetaTOR
         
         [![PyPI version](https://badge.fury.io/py/metator.svg)](https://badge.fury.io/py/metator)
```

### Comparing `metator-1.2.7/metator.egg-info/SOURCES.txt` & `metator-1.2.8/metator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metator-1.2.7/setup.py` & `metator-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Operating System :: Unix",
 ]
 
 name = "metator"
 
 MAJOR = 1
 MINOR = 2
-MAINTENANCE = 7
+MAINTENANCE = 8
 VERSION = "{}.{}.{}".format(MAJOR, MINOR, MAINTENANCE)
 
 LICENSE = "GPLv3"
 URL = "https://github.com/koszullab/metator"
 
 DESCRIPTION = __doc__.strip("\n")
```

