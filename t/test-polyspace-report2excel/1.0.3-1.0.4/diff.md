# Comparing `tmp/test-polyspace-report2excel-1.0.3.tar.gz` & `tmp/test-polyspace-report2excel-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-polyspace-report2excel-1.0.3.tar", last modified: Wed Apr 12 13:56:13 2023, max compression
+gzip compressed data, was "test-polyspace-report2excel-1.0.4.tar", last modified: Wed Apr 12 14:19:07 2023, max compression
```

## Comparing `test-polyspace-report2excel-1.0.3.tar` & `test-polyspace-report2excel-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.895838 test-polyspace-report2excel-1.0.3/
--rw-rw-r--   0 diego     (1003) diego     (1003)    35149 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/LICENSE
--rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:56:13.895838 test-polyspace-report2excel-1.0.3/PKG-INFO
--rw-rw-r--   0 diego     (1003) diego     (1003)     1695 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.3/README.md
--rw-rw-r--   0 diego     (1003) diego     (1003)     1158 2023-04-12 13:54:30.000000 test-polyspace-report2excel-1.0.3/pyproject.toml
--rw-rw-r--   0 diego     (1003) diego     (1003)       38 2023-04-12 13:56:13.895838 test-polyspace-report2excel-1.0.3/setup.cfg
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/src/
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/src/p2e/
--rw-rw-r--   0 diego     (1003) diego     (1003)     9827 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.3/src/p2e/HTMLReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     1462 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/src/p2e/RTFReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      295 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/src/p2e/__init__.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4325 2023-04-12 13:55:46.000000 test-polyspace-report2excel-1.0.3/src/p2e/exportcsv.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4626 2023-04-12 13:55:41.000000 test-polyspace-report2excel-1.0.3/src/p2e/exportxlsx.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4916 2023-04-12 13:55:32.000000 test-polyspace-report2excel-1.0.3/src/p2e/main.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      445 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.3/src/p2e/utils.py
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/
--rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1003) diego     (1003)      581 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)        1 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)       33 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)       30 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/requires.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)        4 2023-04-12 13:56:13.000000 test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:56:13.891838 test-polyspace-report2excel-1.0.3/tests/
--rw-rw-r--   0 diego     (1003) diego     (1003)       28 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/tests/test_HTMLReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      484 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/tests/test_csvexporter.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      363 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.3/tests/test_xlsxexporter.py
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 14:19:07.832697 test-polyspace-report2excel-1.0.4/
+-rw-rw-r--   0 diego     (1003) diego     (1003)    35149 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.4/LICENSE
+-rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 14:19:07.832697 test-polyspace-report2excel-1.0.4/PKG-INFO
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1695 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.4/README.md
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1158 2023-04-12 14:08:55.000000 test-polyspace-report2excel-1.0.4/pyproject.toml
+-rw-rw-r--   0 diego     (1003) diego     (1003)       38 2023-04-12 14:19:07.832697 test-polyspace-report2excel-1.0.4/setup.cfg
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 14:19:07.828696 test-polyspace-report2excel-1.0.4/src/
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 14:19:07.832697 test-polyspace-report2excel-1.0.4/src/p2e/
+-rw-rw-r--   0 diego     (1003) diego     (1003)     9827 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.4/src/p2e/HTMLReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1462 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.4/src/p2e/RTFReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      324 2023-04-12 14:13:53.000000 test-polyspace-report2excel-1.0.4/src/p2e/__init__.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4333 2023-04-12 14:14:34.000000 test-polyspace-report2excel-1.0.4/src/p2e/exportcsv.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4651 2023-04-12 14:14:32.000000 test-polyspace-report2excel-1.0.4/src/p2e/exportxlsx.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4912 2023-04-12 14:17:42.000000 test-polyspace-report2excel-1.0.4/src/p2e/main.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      535 2023-04-12 14:05:20.000000 test-polyspace-report2excel-1.0.4/src/p2e/utils.py
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 14:19:07.832697 test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/
+-rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 14:19:07.000000 test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1003) diego     (1003)      581 2023-04-12 14:19:07.000000 test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)        1 2023-04-12 14:19:07.000000 test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)       33 2023-04-12 14:19:07.000000 test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)       30 2023-04-12 14:19:07.000000 test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)        4 2023-04-12 14:19:07.000000 test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 14:19:07.832697 test-polyspace-report2excel-1.0.4/tests/
+-rw-rw-r--   0 diego     (1003) diego     (1003)       28 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.4/tests/test_HTMLReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      484 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.4/tests/test_csvexporter.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      363 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.4/tests/test_xlsxexporter.py
```

### Comparing `test-polyspace-report2excel-1.0.3/LICENSE` & `test-polyspace-report2excel-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.3/PKG-INFO` & `test-polyspace-report2excel-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-polyspace-report2excel
-Version: 1.0.3
+Version: 1.0.4
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `test-polyspace-report2excel-1.0.3/README.md` & `test-polyspace-report2excel-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.3/pyproject.toml` & `test-polyspace-report2excel-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 # https://pypi.org/project/polyspace-report2excel/
 name = "test-polyspace-report2excel"
-version = "1.0.3" 
+version = "1.0.4" 
 description = "read a polyspace report and export misra or run-time results"
 readme = "README.md"
 requires-python = ">=3"
 license = {file = "LICENSE"}
 keywords = ["polyspace", "report", "excel", "misra"]
 authors = [
   {name = "CAT Lab", email = "L-lequal@cnes.fr" }
```

### Comparing `test-polyspace-report2excel-1.0.3/src/p2e/HTMLReader.py` & `test-polyspace-report2excel-1.0.4/src/p2e/HTMLReader.py`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.3/src/p2e/RTFReader.py` & `test-polyspace-report2excel-1.0.4/src/p2e/RTFReader.py`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0.3/src/p2e/exportcsv.py` & `test-polyspace-report2excel-1.0.4/src/p2e/exportcsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             add_sheet(name, data, section="None")
             create_synthese(is_misra = False)
             export()
 """
 
 # __________________________ IMPORT __________________________
 import csv,os,shutil
-from p2e.utils import normalize, stringtofilename
+from p2e.utils import Utils
 
 # __________________ Definition de classes ___________________
 class Exportcsv(object):
     """ Nom de la classe: Exportcsv
      Description: Permet l'export d'un ensemble de donnees dans un fichier csv"""
 
     def __init__(self, filename):
@@ -48,30 +48,30 @@
             return
 
         # On ajoute une colonne si besoin.
         if section is not None:
             data = [["#"] + data[0]] + [[section] + d for d in data[1:]]
 
         try:
-            csv_path = os.path.join(self.output, normalize(name)+".csv")
+            csv_path = os.path.join(self.output, Utils.normalize(name)+".csv")
         except FileNotFoundError:
             print("The specified output directory does not exist.")
 
         # On essaye de creer la feuille, si celle-ci existe deja l'exception DuplicateWorksheetName sera levee
         if not os.path.exists(csv_path):
             sheet = open(csv_path, "w", newline = "")
             # On garde les donnees en memoire, utile si on cherche a faire une synthese plus tard
 
-            self.sheets[stringtofilename(name)] = [None, len(data), data, name]
+            self.sheets[Utils.stringtofilename(name)] = [None, len(data), data, name]
             firstline = 0
         else:
             sheet = open(csv_path, "a", newline = "")
-            firstline = self.sheets[stringtofilename(name)][1]
+            firstline = self.sheets[Utils.stringtofilename(name)][1]
             data = data[1:]
-            self.sheets[stringtofilename(name)][2] += data
+            self.sheets[Utils.stringtofilename(name)][2] += data
 
         csv_writer = self.get_writer(sheet)
 
         # Ajout des donnees
         for line in range(firstline, firstline + len(data)):
             i = line - firstline
             data[i] = [d.strip() for d in data[i]]
@@ -92,15 +92,15 @@
         for sheet in self.sheets.values():
             if is_misra and "by file" not in sheet[3].lower() and sheet[3].strip() or not is_misra:
                 if line == 0:
                     csv_writer.writerow(['file'] + sheet[2][0])
                     line = 1
                 for row in sheet[2][1:]:
                     row = [d.strip() for d in row]
-                    csv_writer.writerow([stringtofilename(sheet[3])] + row)
+                    csv_writer.writerow([Utils.stringtofilename(sheet[3])] + row)
         synth_sheet.close()
 
 
 
     def export(self):
         """
             export
```

### Comparing `test-polyspace-report2excel-1.0.3/src/p2e/exportxlsx.py` & `test-polyspace-report2excel-1.0.4/src/p2e/exportxlsx.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             add_sheet(name, data, section="None")
             create_synthese(is_misra = False)
             export()
 """
 
 # __________________________ IMPORT __________________________
 import xlsxwriter as xwriter
-from p2e.utils import stringtofilename
+from p2e.utils import Utils
 
 # __________________ Definition de classes ___________________
 class Exportxlsx(object):
     """ Nom de la classe: Exportxlsx
      Description: Permet l'export d'un ensemble de donnees dans un fichier excel"""
 
     def __init__(self, filename):
@@ -44,23 +44,23 @@
 
         # On ajoute une colonne si besoin.
         if section is not None:
             data = [["#"] + data[0]] + [[section] + d for d in data[1:]]
 
         # On essaye de creer la feuille, si celle-ci existe deja l'exception DuplicateWorksheetName sera levee
         try:
-            sheet = self.output.add_worksheet(stringtofilename(name))
+            sheet = self.output.add_worksheet(Utils.stringtofilename(name))
             # On garde les donnees en memoire, utile si on cherche a faire une synthese plus tard
-            self.sheets[stringtofilename(name)] = [sheet, len(data), data, name]
+            self.sheets[Utils.stringtofilename(name)] = [sheet, len(data), data, name]
             firstline = 0
         except xwriter.exceptions.DuplicateWorksheetName:
-            sheet = self.sheets[stringtofilename(name)][0]
-            firstline = self.sheets[stringtofilename(name)][1]
+            sheet = self.sheets[Utils.stringtofilename(name)][0]
+            firstline = self.sheets[Utils.stringtofilename(name)][1]
             data = data[1:]
-            self.sheets[stringtofilename(name)][2] += data
+            self.sheets[Utils.stringtofilename(name)][2] += data
 
         # Cette variable determine la longueur maximale d'une case, cela est utilise pour mettre en forme les cellules
         # dans excel
         col_width = [0 for _ in range(len(data[0]))]
         bold = self.output.add_format({'bold': True})
 
         # Ajout des donnees
@@ -91,15 +91,15 @@
         for sheet in self.sheets.values():
             if is_misra and "by file" not in sheet[3].lower() and sheet[3].strip() or not is_misra:
                 if line == 0:
                     synth_sheet.write_row(line, 0, ['file'] + sheet[2][0], cell_format=bold)
                     line = 1
                 for row in sheet[2][1:]:
                     row = [d.strip() for d in row]
-                    synth_sheet.write_row(line, 0, [stringtofilename(sheet[3])] + row)
+                    synth_sheet.write_row(line, 0, [Utils.stringtofilename(sheet[3])] + row)
                     line += 1
 
 
 
     def export(self):
         """
             export
```

### Comparing `test-polyspace-report2excel-1.0.3/src/p2e/main.py` & `test-polyspace-report2excel-1.0.4/src/p2e/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 import os
 import argparse
 
 from p2e.exportcsv import Exportcsv
 from p2e.exportxlsx import Exportxlsx
 from p2e.HTMLReader import HTMLReader
-from p2e.utils import normalize, stringtofilename
+from p2e.utils import Utils
 
 def main():
     # ________________________ VARIABLES _________________________
     reader = None
     tables = None
 
     # Assigning arguments to variables
@@ -53,22 +53,22 @@
 
     export_tables_to_output(tables, output_folder, misra, runtime, csv)
 
 def export_tables_to_output(tables, output_folder, misra, runtime, csv):
     for chapter in tables.keys():
         # ouverture du fichier de sortie (un fichier par chapitre)
         if not csv:
-            output = Exportxlsx(os.path.join(output_folder, normalize(chapter)))
+            output = Exportxlsx(os.path.join(output_folder, Utils.normalize(chapter)))
         else:
-            output = Exportcsv(os.path.join(output_folder, normalize(chapter)))
+            output = Exportcsv(os.path.join(output_folder, Utils.normalize(chapter)))
 
         # Export de toute les tables dans les excel
         for table in tables[chapter]:
             output.add_sheet(
-                stringtofilename(table['name'])[-31:],
+                Utils.stringtofilename(table['name'])[-31:],
                 table['table'],
                 table["section"]
             )
 
         # If runtime or misra, we create a summary sheet
         summary_sheet(misra, runtime, output)
         output.export()
```

### Comparing `test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/PKG-INFO` & `test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-polyspace-report2excel
-Version: 1.0.3
+Version: 1.0.4
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `test-polyspace-report2excel-1.0.3/src/test_polyspace_report2excel.egg-info/SOURCES.txt` & `test-polyspace-report2excel-1.0.4/src/test_polyspace_report2excel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

