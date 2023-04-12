# Comparing `tmp/khloraascaf_utils-0.5.1.tar.gz` & `tmp/khloraascaf_utils-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf_utils-0.5.1.tar", last modified: Thu Mar 30 12:16:29 2023, max compression
+gzip compressed data, was "khloraascaf_utils-0.5.2.tar", last modified: Wed Apr 12 09:43:52 2023, max compression
```

## Comparing `khloraascaf_utils-0.5.1.tar` & `khloraascaf_utils-0.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:16:29.672808 khloraascaf_utils-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)    43838 2023-03-30 12:16:29.672808 khloraascaf_utils-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 12:16:29.672808 khloraascaf_utils-0.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:16:29.664850 khloraascaf_utils-0.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:16:29.668829 khloraascaf_utils-0.5.1/src/khloraascaf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7074 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils/artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7169 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils/asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils/contigs_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13756 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils/to_networkx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:16:29.670819 khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43838 2023-03-30 12:16:29.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-03-30 12:16:29.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 12:16:29.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-30 12:16:29.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-30 12:16:29.000000 khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:16:29.671814 khloraascaf_utils-0.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3364 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/tests/test_artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/tests/test_asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-03-30 12:16:03.000000 khloraascaf_utils-0.5.1/tests/test_contigs_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:43:52.588669 khloraascaf_utils-0.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-04-12 09:43:52.588669 khloraascaf_utils-0.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 09:43:52.588669 khloraascaf_utils-0.5.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:43:52.580669 khloraascaf_utils-0.5.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:43:52.584669 khloraascaf_utils-0.5.2/src/khloraascaf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7074 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils/artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7169 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils/asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils/contigs_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13756 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils/to_networkx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:43:52.586669 khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-04-12 09:43:52.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-12 09:43:52.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:43:52.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 09:43:52.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 09:43:52.000000 khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:43:52.587669 khloraascaf_utils-0.5.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/tests/test_artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/tests/test_asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-04-12 09:43:25.000000 khloraascaf_utils-0.5.2/tests/test_contigs_attributes.py
```

### Comparing `khloraascaf_utils-0.5.1/LICENCE` & `khloraascaf_utils-0.5.2/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/PKG-INFO` & `khloraascaf_utils-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf_utils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.5.1/README.md` & `khloraascaf_utils-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/pyproject.toml` & `khloraascaf_utils-0.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf_utils"
-version = "0.5.1"
+version = "0.5.2"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "Python utilities for khloraascaf python package."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -17,15 +17,15 @@
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = { file = "LICENCE" }
 requires-python = ">=3.9"
 dependencies = [
-    "khloraascaf >=1.3.0, <1.4",
+    "khloraascaf >=1.4.1, <1.5",
     "networkx >=3.0, <3.1",
     "biopython >=1.81, <1.82",
 ]
 
 [project.urls]
 
 Homepage = "https://gitlab.com/khloraa_scaffolding/khloraascaf_utils"
```

### Comparing `khloraascaf_utils-0.5.1/src/khloraascaf_utils/artificial_data.py` & `khloraascaf_utils-0.5.2/src/khloraascaf_utils/artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/src/khloraascaf_utils/asm_graph_to_fasta.py` & `khloraascaf_utils-0.5.2/src/khloraascaf_utils/asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/src/khloraascaf_utils/contigs_attributes.py` & `khloraascaf_utils-0.5.2/src/khloraascaf_utils/contigs_attributes.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/src/khloraascaf_utils/to_networkx.py` & `khloraascaf_utils-0.5.2/src/khloraascaf_utils/to_networkx.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/PKG-INFO` & `khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf-utils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.5.1/src/khloraascaf_utils.egg-info/SOURCES.txt` & `khloraascaf_utils-0.5.2/src/khloraascaf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/tests/test_artificial_data.py` & `khloraascaf_utils-0.5.2/tests/test_artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/tests/test_asm_graph_to_fasta.py` & `khloraascaf_utils-0.5.2/tests/test_asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.1/tests/test_contigs_attributes.py` & `khloraascaf_utils-0.5.2/tests/test_contigs_attributes.py`

 * *Files identical despite different names*

