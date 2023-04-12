# Comparing `tmp/test-polyspace-report2excel-1.0.2.tar.gz` & `tmp/test-polyspace-report2excel-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-polyspace-report2excel-1.0.2.tar", last modified: Wed Apr 12 13:42:28 2023, max compression
+gzip compressed data, was "test-polyspace-report2excel-1.0.3.tar", last modified: Wed Apr 12 13:56:13 2023, max compression
```

## Comparing `test-polyspace-report2excel-1.0.2.tar` & `test-polyspace-report2excel-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/
--rw-rw-r--   0 diego     (1003) diego     (1003)    35149 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/LICENSE
--rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/PKG-INFO
--rw-rw-r--   0 diego     (1003) diego     (1003)     1695 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/README.md
--rw-rw-r--   0 diego     (1003) diego     (1003)     1158 2023-04-12 13:42:22.000000 test-polyspace-report2excel-1.0.2/pyproject.toml
--rw-rw-r--   0 diego     (1003) diego     (1003)       38 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/setup.cfg
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.243902 test-polyspace-report2excel-1.0.2/src/
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/src/p2e/
--rw-rw-r--   0 diego     (1003) diego     (1003)     9827 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/HTMLReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     1462 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/src/p2e/RTFReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      295 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/src/p2e/__init__.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4321 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/exportcsv.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4622 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/exportxlsx.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4912 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/main.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      445 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/utils.py
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/
--rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1003) diego     (1003)      581 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)        1 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)       33 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)       30 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/requires.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)        4 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/tests/
--rw-rw-r--   0 diego     (1003) diego     (1003)       28 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/tests/test_HTMLReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      484 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/tests/test_csvexporter.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      363 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/tests/test_xlsxexporter.py
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.895838 test-polyspace-report2excel-1.0.3/
+-rw-rw-r--   0 diego     (1003) diego     (1003)    35149 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/LICENSE
+-rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:56:13.895838 test-polyspace-report2excel-1.0.3/PKG-INFO
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1695 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.3/README.md
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1158 2023-04-12 13:54:30.000000 test-polyspace-report2excel-1.0.3/pyproject.toml
+-rw-rw-r--   0 diego     (1003) diego     (1003)       38 2023-04-12 13:56:13.895838 test-polyspace-report2excel-1.0.3/setup.cfg
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/src/
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/src/p2e/
+-rw-rw-r--   0 diego     (1003) diego     (1003)     9827 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.3/src/p2e/HTMLReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1462 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/src/p2e/RTFReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      295 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/src/p2e/__init__.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4325 2023-04-12 13:55:46.000000 test-polyspace-report2excel-1.0.3/src/p2e/exportcsv.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4626 2023-04-12 13:55:41.000000 test-polyspace-report2excel-1.0.3/src/p2e/exportxlsx.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4916 2023-04-12 13:55:32.000000 test-polyspace-report2excel-1.0.3/src/p2e/main.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      445 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.3/src/p2e/utils.py
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/
+-rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1003) diego     (1003)      581 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)        1 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)       33 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)       30 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)        4 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/tests/
+-rw-rw-r--   0 diego     (1003) diego     (1003)       28 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/tests/test_HTMLReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      484 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/tests/test_csvexporter.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      363 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/tests/test_xlsxexporter.py
```

### Comparing `test-polyspace-report2excel-1.0.2/LICENSE` & `test-polyspace-report2excel-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.2/PKG-INFO` & `test-polyspace-report2excel-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-polyspace-report2excel
-Version: 1.0.2
+Version: 1.0.3
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `test-polyspace-report2excel-1.0.2/README.md` & `test-polyspace-report2excel-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.2/pyproject.toml` & `test-polyspace-report2excel-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 # https://pypi.org/project/polyspace-report2excel/
 name = "test-polyspace-report2excel"
-version = "1.0.2" 
+version = "1.0.3" 
 description = "read a polyspace report and export misra or run-time results"
 readme = "README.md"
 requires-python = ">=3"
 license = {file = "LICENSE"}
 keywords = ["polyspace", "report", "excel", "misra"]
 authors = [
   {name = "CAT Lab", email = "L-lequal@cnes.fr" }
```

### Comparing `test-polyspace-report2excel-1.0.2/src/p2e/HTMLReader.py` & `test-polyspace-report2excel-1.0.3/src/p2e/HTMLReader.py`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.2/src/p2e/RTFReader.py` & `test-polyspace-report2excel-1.0.3/src/p2e/RTFReader.py`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.2/src/p2e/exportcsv.py` & `test-polyspace-report2excel-1.0.3/src/p2e/exportcsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             add_sheet(name, data, section="None")
             create_synthese(is_misra = False)
             export()
 """
 
 # __________________________ IMPORT __________________________
 import csv,os,shutil
-from utils import normalize, stringtofilename
+from p2e.utils import normalize, stringtofilename
 
 # __________________ Definition de classes ___________________
 class Exportcsv(object):
     """ Nom de la classe: Exportcsv
      Description: Permet l'export d'un ensemble de donnees dans un fichier csv"""
 
     def __init__(self, filename):
```

### Comparing `test-polyspace-report2excel-1.0.2/src/p2e/exportxlsx.py` & `test-polyspace-report2excel-1.0.3/src/p2e/exportxlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             add_sheet(name, data, section="None")
             create_synthese(is_misra = False)
             export()
 """
 
 # __________________________ IMPORT __________________________
 import xlsxwriter as xwriter
-from utils import stringtofilename
+from p2e.utils import stringtofilename
 
 # __________________ Definition de classes ___________________
 class Exportxlsx(object):
     """ Nom de la classe: Exportxlsx
      Description: Permet l'export d'un ensemble de donnees dans un fichier excel"""
 
     def __init__(self, filename):
```

### Comparing `test-polyspace-report2excel-1.0.2/src/p2e/main.py` & `test-polyspace-report2excel-1.0.3/src/p2e/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 import os
 import argparse
 
 from p2e.exportcsv import Exportcsv
 from p2e.exportxlsx import Exportxlsx
 from p2e.HTMLReader import HTMLReader
-from utils import normalize, stringtofilename
+from p2e.utils import normalize, stringtofilename
 
 def main():
     # ________________________ VARIABLES _________________________
     reader = None
     tables = None
 
     # Assigning arguments to variables
```

### Comparing `test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/PKG-INFO` & `test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-polyspace-report2excel
-Version: 1.0.2
+Version: 1.0.3
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/SOURCES.txt` & `test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

