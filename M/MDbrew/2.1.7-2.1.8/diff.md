# Comparing `tmp/MDbrew-2.1.7.tar.gz` & `tmp/MDbrew-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.1.7.tar", last modified: Wed Apr 12 06:47:18 2023, max compression
+gzip compressed data, was "MDbrew-2.1.8.tar", last modified: Wed Apr 12 06:49:55 2023, max compression
```

## Comparing `MDbrew-2.1.7.tar` & `MDbrew-2.1.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/
--rw-r--r--   0 minu928   (1000) minu928   (1000)       24 2023-04-12 06:13:04.000000 MDbrew-2.1.7/MANIFEST.in
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/MDbrew/
--rw-r--r--   0 minu928   (1000) minu928   (1000)     1303 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/__init__.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)      107 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/_base.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)      129 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/_type.py
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/MDbrew/analysis/
--rw-r--r--   0 minu928   (1000) minu928   (1000)       68 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     4170 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/analysis/msd.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     5260 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/MDbrew/brew/
--rw-r--r--   0 minu928   (1000) minu928   (1000)       33 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/brew/__init__.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)    10322 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/brew/extractor.py
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/MDbrew/chemistry/
--rw-r--r--   0 minu928   (1000) minu928   (1000)       20 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/chemistry/__init__.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     1288 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/chemistry/atom.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     1742 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/chemistry/atom_info.npz
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/MDbrew/opener/
--rw-r--r--   0 minu928   (1000) minu928   (1000)      159 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/opener/__init__.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)      672 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/opener/datopener.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     2104 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/opener/lammpsopener.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     1334 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/opener/opener.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     2901 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/opener/wmiopener.py
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/MDbrew/tool/
--rw-r--r--   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/tool/__init__.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)      610 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/tool/query.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)     1533 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/tool/spacer.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)      831 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/tool/tester.py
--rw-r--r--   0 minu928   (1000) minu928   (1000)      744 2023-04-12 06:46:21.000000 MDbrew-2.1.7/MDbrew/tool/timer.py
-drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:47:18.098706 MDbrew-2.1.7/MDbrew.egg-info/
--rw-r--r--   0 minu928   (1000) minu928   (1000)      332 2023-04-12 06:47:18.000000 MDbrew-2.1.7/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu928   (1000) minu928   (1000)      698 2023-04-12 06:47:18.000000 MDbrew-2.1.7/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu928   (1000) minu928   (1000)        1 2023-04-12 06:47:18.000000 MDbrew-2.1.7/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu928   (1000) minu928   (1000)        1 2023-04-12 06:47:18.000000 MDbrew-2.1.7/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu928   (1000) minu928   (1000)        7 2023-04-12 06:47:18.000000 MDbrew-2.1.7/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu928   (1000) minu928   (1000)      332 2023-04-12 06:47:18.098706 MDbrew-2.1.7/PKG-INFO
--rw-r--r--   0 minu928   (1000) minu928   (1000)       58 2023-04-12 06:13:04.000000 MDbrew-2.1.7/requirement.txt
--rw-r--r--   0 minu928   (1000) minu928   (1000)       79 2023-04-12 06:47:18.098706 MDbrew-2.1.7/setup.cfg
--rw-r--r--   0 minu928   (1000) minu928   (1000)      631 2023-04-12 06:46:32.000000 MDbrew-2.1.7/setup.py
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.178674 MDbrew-2.1.8/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)       24 2023-04-12 06:13:04.000000 MDbrew-2.1.8/MANIFEST.in
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.168674 MDbrew-2.1.8/MDbrew/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     1303 2023-04-12 06:49:44.000000 MDbrew-2.1.8/MDbrew/__init__.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      107 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/_base.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      129 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/_type.py
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.178674 MDbrew-2.1.8/MDbrew/analysis/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)       68 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     4170 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     5260 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.178674 MDbrew-2.1.8/MDbrew/brew/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)       33 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/brew/__init__.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)    10322 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/brew/extractor.py
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.178674 MDbrew-2.1.8/MDbrew/chemistry/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)       20 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/chemistry/__init__.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     1288 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/chemistry/atom.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     1742 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/chemistry/atom_info.npz
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.178674 MDbrew-2.1.8/MDbrew/opener/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      159 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/opener/__init__.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      672 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/opener/datopener.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     2104 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/opener/lammpsopener.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     1334 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/opener/opener.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     2901 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/opener/wmiopener.py
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.178674 MDbrew-2.1.8/MDbrew/tool/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      610 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/tool/query.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)     1533 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/tool/spacer.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      828 2023-04-12 06:49:33.000000 MDbrew-2.1.8/MDbrew/tool/tester.py
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      744 2023-04-12 06:46:21.000000 MDbrew-2.1.8/MDbrew/tool/timer.py
+drwxr-xr-x   0 minu928   (1000) minu928   (1000)        0 2023-04-12 06:49:55.178674 MDbrew-2.1.8/MDbrew.egg-info/
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      332 2023-04-12 06:49:55.000000 MDbrew-2.1.8/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      698 2023-04-12 06:49:55.000000 MDbrew-2.1.8/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu928   (1000) minu928   (1000)        1 2023-04-12 06:49:55.000000 MDbrew-2.1.8/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu928   (1000) minu928   (1000)        1 2023-04-12 06:47:18.000000 MDbrew-2.1.8/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu928   (1000) minu928   (1000)        7 2023-04-12 06:49:55.000000 MDbrew-2.1.8/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      332 2023-04-12 06:49:55.178674 MDbrew-2.1.8/PKG-INFO
+-rw-r--r--   0 minu928   (1000) minu928   (1000)       58 2023-04-12 06:13:04.000000 MDbrew-2.1.8/requirement.txt
+-rw-r--r--   0 minu928   (1000) minu928   (1000)       79 2023-04-12 06:49:55.178674 MDbrew-2.1.8/setup.cfg
+-rw-r--r--   0 minu928   (1000) minu928   (1000)      631 2023-04-12 06:49:38.000000 MDbrew-2.1.8/setup.py
```

### Comparing `MDbrew-2.1.7/MDbrew/__init__.py` & `MDbrew-2.1.8/MDbrew/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .brew.extractor import Extractor
 
 from .opener.datopener import DATOpener
 from .opener.lammpsopener import LAMMPSOpener
 from .opener.wmiopener import WMIOpener
 
-__version__ = "2.1.6"
+__version__ = "2.1.8"
 __name__ = "MDbrew"
 
 
 __all__ = ["Extractor", "LAMMPSOpener", "DATOpener", "WMIOpener", "MSD", "RDF"]
 
 """ How to use
```

### Comparing `MDbrew-2.1.7/MDbrew/analysis/msd.py` & `MDbrew-2.1.8/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/analysis/rdf.py` & `MDbrew-2.1.8/MDbrew/analysis/rdf.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/brew/extractor.py` & `MDbrew-2.1.8/MDbrew/brew/extractor.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/chemistry/atom.py` & `MDbrew-2.1.8/MDbrew/chemistry/atom.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/chemistry/atom_info.npz` & `MDbrew-2.1.8/MDbrew/chemistry/atom_info.npz`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/opener/datopener.py` & `MDbrew-2.1.8/MDbrew/opener/datopener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/opener/lammpsopener.py` & `MDbrew-2.1.8/MDbrew/opener/lammpsopener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/opener/opener.py` & `MDbrew-2.1.8/MDbrew/opener/opener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/opener/wmiopener.py` & `MDbrew-2.1.8/MDbrew/opener/wmiopener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/tool/query.py` & `MDbrew-2.1.8/MDbrew/tool/query.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/tool/spacer.py` & `MDbrew-2.1.8/MDbrew/tool/spacer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew/tool/tester.py` & `MDbrew-2.1.8/MDbrew/tool/tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     extractor.atom_info
     id_list = extractor.extract_id_list()
     type_list = extractor.extract_type_list()
     type_info = extractor.extract_type_info()
     dict_type = {1: "O", 2: "N"}
     atom_list = extractor.extract_atom_list(dict_type=dict_type)
     rdf = RDF(position, position, system_size).run()
-    rdf.result
+    rdf.rdf
     rdf.cn
     msd = MSD(uw_position)
     msd.result
     print("\n\ttest Done \u2713 \t\n")
```

### Comparing `MDbrew-2.1.7/MDbrew/tool/timer.py` & `MDbrew-2.1.8/MDbrew/tool/timer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.1.8/MDbrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MDbrew-2.1.7/setup.py` & `MDbrew-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.1.7",
+    version="2.1.8",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
     download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.1.6.tar.gz",
     install_requies=[
         "numpy>=1.0.0",
         "pandas>=1.0.0",
```

