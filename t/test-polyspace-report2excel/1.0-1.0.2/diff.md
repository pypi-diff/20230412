# Comparing `tmp/test-polyspace-report2excel-1.0.tar.gz` & `tmp/test-polyspace-report2excel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-polyspace-report2excel-1.0.tar", last modified: Wed Apr 12 07:20:03 2023, max compression
+gzip compressed data, was "test-polyspace-report2excel-1.0.2.tar", last modified: Wed Apr 12 13:42:28 2023, max compression
```

## Comparing `test-polyspace-report2excel-1.0.tar` & `test-polyspace-report2excel-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 07:20:03.734907 test-polyspace-report2excel-1.0/
--rw-rw-r--   0 diego     (1003) diego     (1003)    35149 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/LICENSE
--rw-rw-r--   0 diego     (1003) diego     (1003)    43028 2023-04-12 07:20:03.730907 test-polyspace-report2excel-1.0/PKG-INFO
--rw-rw-r--   0 diego     (1003) diego     (1003)     1679 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/README.md
--rw-rw-r--   0 diego     (1003) diego     (1003)     1156 2023-04-12 07:19:58.000000 test-polyspace-report2excel-1.0/pyproject.toml
--rw-rw-r--   0 diego     (1003) diego     (1003)       38 2023-04-12 07:20:03.734907 test-polyspace-report2excel-1.0/setup.cfg
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 07:20:03.730907 test-polyspace-report2excel-1.0/src/
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 07:20:03.730907 test-polyspace-report2excel-1.0/src/p2e/
--rw-rw-r--   0 diego     (1003) diego     (1003)     9862 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/src/p2e/HTMLReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     1462 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/src/p2e/RTFReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      295 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/src/p2e/__init__.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4851 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/src/p2e/exportcsv.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     5207 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/src/p2e/exportxlsx.py
--rw-rw-r--   0 diego     (1003) diego     (1003)     4122 2023-04-12 07:11:51.000000 test-polyspace-report2excel-1.0/src/p2e/main.py
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 07:20:03.730907 test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/
--rw-rw-r--   0 diego     (1003) diego     (1003)    43028 2023-04-12 07:20:03.000000 test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1003) diego     (1003)      564 2023-04-12 07:20:03.000000 test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)        1 2023-04-12 07:20:03.000000 test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)       33 2023-04-12 07:20:03.000000 test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)       30 2023-04-12 07:20:03.000000 test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/requires.txt
--rw-rw-r--   0 diego     (1003) diego     (1003)        4 2023-04-12 07:20:03.000000 test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 07:20:03.730907 test-polyspace-report2excel-1.0/tests/
--rw-rw-r--   0 diego     (1003) diego     (1003)       28 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/tests/test_HTMLReader.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      484 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/tests/test_csvexporter.py
--rw-rw-r--   0 diego     (1003) diego     (1003)      363 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0/tests/test_xlsxexporter.py
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/
+-rw-rw-r--   0 diego     (1003) diego     (1003)    35149 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/LICENSE
+-rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/PKG-INFO
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1695 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/README.md
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1158 2023-04-12 13:42:22.000000 test-polyspace-report2excel-1.0.2/pyproject.toml
+-rw-rw-r--   0 diego     (1003) diego     (1003)       38 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/setup.cfg
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.243902 test-polyspace-report2excel-1.0.2/src/
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/src/p2e/
+-rw-rw-r--   0 diego     (1003) diego     (1003)     9827 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/HTMLReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     1462 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/src/p2e/RTFReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      295 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/src/p2e/__init__.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4321 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/exportcsv.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4622 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/exportxlsx.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)     4912 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/main.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      445 2023-04-12 13:40:09.000000 test-polyspace-report2excel-1.0.2/src/p2e/utils.py
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/
+-rw-rw-r--   0 diego     (1003) diego     (1003)    43046 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1003) diego     (1003)      581 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)        1 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)       33 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)       30 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1003) diego     (1003)        4 2023-04-12 13:42:28.000000 test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1003) diego     (1003)        0 2023-04-12 13:42:28.247904 test-polyspace-report2excel-1.0.2/tests/
+-rw-rw-r--   0 diego     (1003) diego     (1003)       28 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/tests/test_HTMLReader.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      484 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/tests/test_csvexporter.py
+-rw-rw-r--   0 diego     (1003) diego     (1003)      363 2023-03-22 13:00:12.000000 test-polyspace-report2excel-1.0.2/tests/test_xlsxexporter.py
```

### Comparing `test-polyspace-report2excel-1.0/LICENSE` & `test-polyspace-report2excel-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0/PKG-INFO` & `test-polyspace-report2excel-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-polyspace-report2excel
-Version: 1.0
+Version: 1.0.2
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -723,17 +723,17 @@
 ### Usage example by cloning the repository
 If you don't want to install the package `polyspace-report2excel`, first install the dependencies.
 
 `pip install .`
 
 Then, you can run:
 ``` 
-python main.py input.html ouput-folder/
+python src/p2e/main.py input.html ouput-folder/
 
-python main.py input.rtf ouput-folder/ --runtime
+python src/p2e/main.py input.rtf ouput-folder/ --runtime
 ```
 ## Arguments
 - `--misra` will export misra report only.
 - `--runtime` will export run-time report only (ignored if `--misra`).
 - `-y` will force overwrite if output files already exist.
 - `--poly14` will read report from polyspace 2014
 - `--csv` will export data in CSV instead of xlsx
```

### Comparing `test-polyspace-report2excel-1.0/README.md` & `test-polyspace-report2excel-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 ### Usage example by cloning the repository
 If you don't want to install the package `polyspace-report2excel`, first install the dependencies.
 
 `pip install .`
 
 Then, you can run:
 ``` 
-python main.py input.html ouput-folder/
+python src/p2e/main.py input.html ouput-folder/
 
-python main.py input.rtf ouput-folder/ --runtime
+python src/p2e/main.py input.rtf ouput-folder/ --runtime
 ```
 ## Arguments
 - `--misra` will export misra report only.
 - `--runtime` will export run-time report only (ignored if `--misra`).
 - `-y` will force overwrite if output files already exist.
 - `--poly14` will read report from polyspace 2014
 - `--csv` will export data in CSV instead of xlsx
```

### Comparing `test-polyspace-report2excel-1.0/pyproject.toml` & `test-polyspace-report2excel-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 # https://pypi.org/project/polyspace-report2excel/
 name = "test-polyspace-report2excel"
-version = "1.0" 
+version = "1.0.2" 
 description = "read a polyspace report and export misra or run-time results"
 readme = "README.md"
 requires-python = ">=3"
 license = {file = "LICENSE"}
 keywords = ["polyspace", "report", "excel", "misra"]
 authors = [
   {name = "CAT Lab", email = "L-lequal@cnes.fr" }
```

### Comparing `test-polyspace-report2excel-1.0/src/p2e/HTMLReader.py` & `test-polyspace-report2excel-1.0.2/src/p2e/HTMLReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 class HTMLReader(object):
 
     """ Nom de la classe: HTMLReader
         Description: Cette classe lit un fichier HTML et permet
         l'extraction des tableaux qu'il contient """
 
     def __init__(self, filename, version=18):
-        self.__filename = filename
         self._file = open(filename, "r")
         self.__version = version
         self._lines = None
         # Structure de cette variable definie dans la doctstring de get_all_tables
         self.__tables = dict()
         print("Reading report for polyspace 20" + str(version))
```

### Comparing `test-polyspace-report2excel-1.0/src/p2e/RTFReader.py` & `test-polyspace-report2excel-1.0.2/src/p2e/RTFReader.py`

 * *Files identical despite different names*

### Comparing `test-polyspace-report2excel-1.0/src/p2e/exportcsv.py` & `test-polyspace-report2excel-1.0.2/src/p2e/exportcsv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 """ Nom du module: exportcsv
  Description: Ce module permet l'ecriture vers un fichier csv.
  Methodes et classes publiques:
         - exportxlsx
             __init__(filename)
-            normalize(value)
-            stringtofilename(value)
             add_sheet(name, data, section="None")
             create_synthese(is_misra = False)
             export()
 """
 
 # __________________________ IMPORT __________________________
 import csv,os,shutil
+from utils import normalize, stringtofilename
 
 # __________________ Definition de classes ___________________
 class Exportcsv(object):
-    """ Nom de la classe: Exportxlsx
-     Description: Permet l'export d'un ensemble de donnees dans un fichier excel"""
-
-    @staticmethod
-    def normalize(value):
-        """ Enleve tout les caracteres speciaux de la chaine value """
-        value = value.strip()
-        value = "".join(x for x in value if x.isalnum() or x == " ")
-        return value
-
-    @staticmethod
-    def stringtofilename(value):
-        """ Recupere le nom d'un fichier. On suppose que ce nom ne contient pas d'espace. """
-        value = "".join(x for x in value if x not in "[]:*?/")
-        value = value.replace(" ", "\\")
-        return value.split("\\")[-1]
+    """ Nom de la classe: Exportcsv
+     Description: Permet l'export d'un ensemble de donnees dans un fichier csv"""
 
     def __init__(self, filename):
         self.sheets = dict()
         self.filename = filename
         if os.path.exists(self.filename):
             shutil.rmtree(self.filename)
         os.mkdir(self.filename)
         self.output = os.path.abspath(self.filename)
         
     @staticmethod
-    def __getWriter(path):
+    def get_writer(path):
         return csv.writer(path,delimiter=';', quotechar='"', quoting=csv.QUOTE_MINIMAL)
 
     def add_sheet(self, name, data, section=None):
         """
                 add_sheet
                 Permet d'ajouter un feuille au fichier excel de sortie
 
@@ -57,66 +42,65 @@
                     de cette colonne est remplie avec  le contenu de "section", cela est utile
                     lorsque l'on ecrit plusieurs fois dans la meme feuille (pour distinguer "qui"
                     a ecrit).
             """
         # Si on a aucune donnee ou que le fichier est fermee, on stoppe l'execution
         if not data:
             return
-        if self.output is None:
-            raise Exception("Output file is closed")
-
-
 
         # On ajoute une colonne si besoin.
         if section is not None:
             data = [["#"] + data[0]] + [[section] + d for d in data[1:]]
 
-        csvPath = os.path.join(self.output, self.normalize(name)+".csv")
+        try:
+            csv_path = os.path.join(self.output, normalize(name)+".csv")
+        except FileNotFoundError:
+            print("The specified output directory does not exist.")
 
         # On essaye de creer la feuille, si celle-ci existe deja l'exception DuplicateWorksheetName sera levee
-        if not os.path.exists(csvPath):
-            sheet = open(csvPath, "w", newline = "")
+        if not os.path.exists(csv_path):
+            sheet = open(csv_path, "w", newline = "")
             # On garde les donnees en memoire, utile si on cherche a faire une synthese plus tard
 
-            self.sheets[self.stringtofilename(name)] = [None, len(data), data, name]
+            self.sheets[stringtofilename(name)] = [None, len(data), data, name]
             firstline = 0
         else:
-            sheet = open(csvPath, "a", newline = "")
-            firstline = self.sheets[self.stringtofilename(name)][1]
+            sheet = open(csv_path, "a", newline = "")
+            firstline = self.sheets[stringtofilename(name)][1]
             data = data[1:]
-            self.sheets[self.stringtofilename(name)][2] += data
+            self.sheets[stringtofilename(name)][2] += data
 
-        csvWriter = self.__getWriter(sheet)
+        csv_writer = self.get_writer(sheet)
 
         # Ajout des donnees
         for line in range(firstline, firstline + len(data)):
             i = line - firstline
             data[i] = [d.strip() for d in data[i]]
             if data[i][-1] == '\n':
                 del(data[i][-1])
 
-            csvWriter.writerow(data[i])
+            csv_writer.writerow(data[i])
         sheet.close()
 
     def create_synthese(self, is_misra=False):
         """ Permet la creation d'une feuille de synthese
         regroupant les donnees des autres feuilles """
-        csvPath = os.path.join(self.output, "Synthese.csv")
-        synth_sheet = open(csvPath, "w", newline = "")
-        csvWriter = self.__getWriter(synth_sheet)
+        csv_path = os.path.join(self.output, "Synthese.csv")
+        synth_sheet = open(csv_path, "w", newline = "")
+        csv_writer = self.get_writer(synth_sheet)
         line = 0
 
         for sheet in self.sheets.values():
             if is_misra and "by file" not in sheet[3].lower() and sheet[3].strip() or not is_misra:
                 if line == 0:
-                    csvWriter.writerow(['file'] + sheet[2][0])
+                    csv_writer.writerow(['file'] + sheet[2][0])
                     line = 1
                 for row in sheet[2][1:]:
                     row = [d.strip() for d in row]
-                    csvWriter.writerow([self.stringtofilename(sheet[3])] + row)
+                    csv_writer.writerow([stringtofilename(sheet[3])] + row)
         synth_sheet.close()
 
 
 
     def export(self):
         """
             export
```

### Comparing `test-polyspace-report2excel-1.0/src/p2e/exportxlsx.py` & `test-polyspace-report2excel-1.0.2/src/p2e/exportxlsx.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,31 @@
 """ Nom du module: exportxlsx
  Description: Ce module permet l'ecriture vers un fichier excel.
  Methodes et classes publiques:
         - exportxlsx
             __init__(filename)
-            normalize(value)
-            stringtofilename(value)
             add_sheet(name, data, section="None")
             create_synthese(is_misra = False)
             export()
 """
 
 # __________________________ IMPORT __________________________
 import xlsxwriter as xwriter
-
+from utils import stringtofilename
 
 # __________________ Definition de classes ___________________
 class Exportxlsx(object):
     """ Nom de la classe: Exportxlsx
      Description: Permet l'export d'un ensemble de donnees dans un fichier excel"""
 
-    @staticmethod
-    def normalize(value):
-        """ Enleve tout les caracteres speciaux de la chaine value """
-        value = value.strip()
-        value = "".join(x for x in value if x.isalnum() or x == " ")
-        return value
-
-    @staticmethod
-    def stringtofilename(value):
-        """ Recupere le nom d'un fichier. On suppose que ce nom ne contient pas d'espace. """
-        value = "".join(x for x in value if x not in "[]:*?/")
-        value = value.replace(" ", "\\")
-        return value.split("\\")[-1]
-
     def __init__(self, filename):
         self.sheets = dict()
         self.filename = filename
         self.output = xwriter.Workbook(self.filename + ".xlsx")
 
-
-
     def add_sheet(self, name, data, section=None):
         """
                 add_sheet
                 Permet d'ajouter un feuille au fichier excel de sortie
 
                 :param name: Nom que l'on souhaite donner a la feuille,
                     => si deja utilise, les donnees sont ajoutees a la fin
@@ -54,35 +36,35 @@
                     lorsque l'on ecrit plusieurs fois dans la meme feuille (pour distinguer "qui"
                     a ecrit).
             """
         # Si on a aucune donnee ou que le fichier est fermee, on stoppe l'execution
         if not data:
             return
         if self.output is None:
-            raise Exception("Output file is closed")
+            raise FileNotFoundError("File not found")
 
         # On ajoute une colonne si besoin.
         if section is not None:
             data = [["#"] + data[0]] + [[section] + d for d in data[1:]]
 
         # On essaye de creer la feuille, si celle-ci existe deja l'exception DuplicateWorksheetName sera levee
         try:
-            sheet = self.output.add_worksheet(self.stringtofilename(name))
+            sheet = self.output.add_worksheet(stringtofilename(name))
             # On garde les donnees en memoire, utile si on cherche a faire une synthese plus tard
-            self.sheets[self.stringtofilename(name)] = [sheet, len(data), data, name]
+            self.sheets[stringtofilename(name)] = [sheet, len(data), data, name]
             firstline = 0
         except xwriter.exceptions.DuplicateWorksheetName:
-            sheet = self.sheets[self.stringtofilename(name)][0]
-            firstline = self.sheets[self.stringtofilename(name)][1]
+            sheet = self.sheets[stringtofilename(name)][0]
+            firstline = self.sheets[stringtofilename(name)][1]
             data = data[1:]
-            self.sheets[self.stringtofilename(name)][2] += data
+            self.sheets[stringtofilename(name)][2] += data
 
         # Cette variable determine la longueur maximale d'une case, cela est utilise pour mettre en forme les cellules
         # dans excel
-        col_width = [0 for i in range(len(data[0]))]
+        col_width = [0 for _ in range(len(data[0]))]
         bold = self.output.add_format({'bold': True})
 
         # Ajout des donnees
         for line in range(firstline, firstline + len(data)):
             i = line - firstline
             data[i] = [d.strip() for d in data[i]]
 
@@ -109,15 +91,15 @@
         for sheet in self.sheets.values():
             if is_misra and "by file" not in sheet[3].lower() and sheet[3].strip() or not is_misra:
                 if line == 0:
                     synth_sheet.write_row(line, 0, ['file'] + sheet[2][0], cell_format=bold)
                     line = 1
                 for row in sheet[2][1:]:
                     row = [d.strip() for d in row]
-                    synth_sheet.write_row(line, 0, [self.stringtofilename(sheet[3])] + row)
+                    synth_sheet.write_row(line, 0, [stringtofilename(sheet[3])] + row)
                     line += 1
 
 
 
     def export(self):
         """
             export
```

### Comparing `test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/PKG-INFO` & `test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-polyspace-report2excel
-Version: 1.0
+Version: 1.0.2
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -723,17 +723,17 @@
 ### Usage example by cloning the repository
 If you don't want to install the package `polyspace-report2excel`, first install the dependencies.
 
 `pip install .`
 
 Then, you can run:
 ``` 
-python main.py input.html ouput-folder/
+python src/p2e/main.py input.html ouput-folder/
 
-python main.py input.rtf ouput-folder/ --runtime
+python src/p2e/main.py input.rtf ouput-folder/ --runtime
 ```
 ## Arguments
 - `--misra` will export misra report only.
 - `--runtime` will export run-time report only (ignored if `--misra`).
 - `-y` will force overwrite if output files already exist.
 - `--poly14` will read report from polyspace 2014
 - `--csv` will export data in CSV instead of xlsx
```

### Comparing `test-polyspace-report2excel-1.0/src/test_polyspace_report2excel.egg-info/SOURCES.txt` & `test-polyspace-report2excel-1.0.2/src/test_polyspace_report2excel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 src/p2e/HTMLReader.py
 src/p2e/RTFReader.py
 src/p2e/__init__.py
 src/p2e/exportcsv.py
 src/p2e/exportxlsx.py
 src/p2e/main.py
+src/p2e/utils.py
 src/test_polyspace_report2excel.egg-info/PKG-INFO
 src/test_polyspace_report2excel.egg-info/SOURCES.txt
 src/test_polyspace_report2excel.egg-info/dependency_links.txt
 src/test_polyspace_report2excel.egg-info/entry_points.txt
 src/test_polyspace_report2excel.egg-info/requires.txt
 src/test_polyspace_report2excel.egg-info/top_level.txt
 tests/test_HTMLReader.py
```

