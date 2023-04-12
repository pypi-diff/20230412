# Comparing `tmp/Datev-Splitter-0.4.0.tar.gz` & `tmp/Datev-Splitter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Datev-Splitter-0.4.0.tar", last modified: Wed Jan 11 10:50:36 2023, max compression
+gzip compressed data, was "Datev-Splitter-0.5.0.tar", last modified: Wed Apr 12 14:53:17 2023, max compression
```

## Comparing `Datev-Splitter-0.4.0.tar` & `Datev-Splitter-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-01-11 10:50:33.871048 Datev-Splitter-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-01-11 10:50:18.747139 Datev-Splitter-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-01-11 10:50:18.747139 Datev-Splitter-0.4.0/datev_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-11 10:50:33.879048 Datev-Splitter-0.4.0/datev_splitter/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-01-11 10:50:18.747139 Datev-Splitter-0.4.0/datev_splitter/pdf_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-11 10:50:18.747139 Datev-Splitter-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-11 10:50:18.747139 Datev-Splitter-0.4.0/tests/test_pdf_extract.py
--rw-------   0 runner    (1001) docker     (123)     2466 2023-01-11 10:50:36.915031 Datev-Splitter-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-04-12 14:53:13.656500 Datev-Splitter-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2200 2023-04-12 14:52:55.476135 Datev-Splitter-0.5.0/README.md
+-rw-r--r--   0        0        0     1614 2023-04-12 14:52:55.476135 Datev-Splitter-0.5.0/datev_splitter/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-12 14:53:13.668501 Datev-Splitter-0.5.0/datev_splitter/__version__.py
+-rw-r--r--   0        0        0     5001 2023-04-12 14:52:55.476135 Datev-Splitter-0.5.0/datev_splitter/pdf_extract.py
+-rw-r--r--   0        0        0     1106 2023-04-12 14:52:55.480135 Datev-Splitter-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3161 2023-04-12 14:52:55.480135 Datev-Splitter-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1636 2023-04-12 14:52:55.480135 Datev-Splitter-0.5.0/tests/test_pdf_extract.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 Datev-Splitter-0.5.0/PKG-INFO
```

### Comparing `Datev-Splitter-0.4.0/CHANGELOG.md` & `Datev-Splitter-0.5.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.5.0 (2023-04-12)
+### Feature
+* Add date to Meldebescheinigungen ([`dd555ea`](https://github.com/tuergeist/datev-splitter/commit/dd555ea25194cd1d96c89cb32cac50ca7342e0a3))
+
+### Fix
+* Tests respect module dir ([`1cca1e2`](https://github.com/tuergeist/datev-splitter/commit/1cca1e2f2665998ec70211224183d9ec46edabf4))
+* Rm .pdm.toml ([`48206bc`](https://github.com/tuergeist/datev-splitter/commit/48206bc86a1b70434f679a3ea3a507632157c479))
+
 ## v0.4.0 (2023-01-11)
 ### Feature
 * Return list of skipped pdf pages ([`1ca02d3`](https://github.com/tuergeist/datev-splitter/commit/1ca02d3e6f058c309caba6802e2a1eee531f8a47))
 
 ## v0.3.2 (2023-01-03)
 ### Fix
 * Repo env upper case ([`371301f`](https://github.com/tuergeist/datev-splitter/commit/371301f2b2cf3a9057df2c9f9a12b32aadaeef44))
```

### Comparing `Datev-Splitter-0.4.0/README.md` & `Datev-Splitter-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `Datev-Splitter-0.4.0/datev_splitter/__init__.py` & `Datev-Splitter-0.5.0/datev_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `Datev-Splitter-0.4.0/datev_splitter/pdf_extract.py` & `Datev-Splitter-0.5.0/datev_splitter/pdf_extract.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os.path
 import re
+from enum import Enum
 from typing import Optional
 
 import fitz  # pip install PyMuPDF
 from loguru import logger
 
 PERSONAL_NR_PATTERN = r'Pers\.-Nr\. ([0-9]{5})'
 
@@ -16,25 +17,54 @@
         logger.trace(text)
         pn = INVALID_PN
     else:
         pn = r[0]
     return pn
 
 
-def get_name(prefix: str, old_pn: str, text: str) -> str:
-    suffix = ""
-    lst = re.findall('(Lohnsteuerbescheinigung) für ([0-9]{4})', text)
-    title = re.findall('für ([A-Z]{1}[a-z]+) (20[0-9]{2})', text)
-    mb = re.findall('Meldebescheinigung', text)
-    if len(title) > 0:
-        suffix = "-".join(list(reversed(title[0])))
-    elif len(lst) > 0:
-        suffix = "-".join(list(reversed(lst[0])))
-    elif len(mb) > 0:
-        suffix = mb[0]
+class FormNr(Enum):
+    Abrechnung = 'LOGN15'
+    AbrechnungswertePruefung = 'LOAP10'
+    Begleitdaten = 'LOA104'  # Begleitzettel, Mandatendaten etc
+    Lohnsteuerbescheinigung = 'LO4723'
+    Meldebescheinigung = 'LOMS04'
+    SVJahresarbeitsentgelt = 'LOJE11'
+    Ueberweisungsprotokoll = 'LOA203'
+
+    Unkown = 'UKNOWN'
+
+
+def get_form_nr(text: str) -> FormNr:
+    form = re.findall(r'AFP Form.-Nr. ([A-Z]{2}\w{4})', text)
+    try:
+        return FormNr(form[0])
+    except IndexError:
+        logger.error(f"No Form Nr found in text >>> '{text}' <<<")
+    except ValueError:
+        logger.error(f"Unknown Form Nr. '{form}'")
+    return FormNr.Unkown
+
+
+def get_name(prefix: str, old_pn: str, _text: str) -> str | None:
+    text = _text.replace('ä', 'ae')
+    form: FormNr = get_form_nr(text)
+
+    match form:
+        case FormNr.Abrechnung:
+            title = re.findall('für ([A-Z]{1}[a-z]+) (20[0-9]{2})', text)
+            suffix = "-".join(list(reversed(title[0])))
+        case FormNr.Lohnsteuerbescheinigung:
+            lst = re.findall('(Lohnsteuerbescheinigung) für ([0-9]{4})', text)
+            suffix = "-".join(list(reversed(lst[0])))
+        case FormNr.Meldebescheinigung:
+            mb = re.findall('Meldebescheinigung', text)
+            datum = re.findall(r'((0[1-9]|[12][0-9]|3[01])\.(0[1-9]|1[012])\.(20[0-9]{2}))', text)
+            suffix = mb[0] + "-" + datum[0][0]
+        case _:
+            return None
     return f'{prefix}{old_pn}-{suffix}.pdf'
 
 
 def save(infile: str, name: str, start_page: int, end_page: int):
     pages = list(range(start_page - 1, end_page))
     with fitz.open(infile) as pdf:
         pdf.select(pages)
@@ -94,15 +124,16 @@
                 start_page = page
                 file_name = get_name(prefix, pn, text)
 
             old_pn = pn
 
         logger.debug('%s from %s to %s' % (file_name, start_page, page))
         mark_used(start_page, page + 1)
-        result.add((file_name, start_page, page))
+        if file_name:
+            result.add((file_name, start_page, page))
 
         if export_pns:
             sorted_pns = sorted(pn_set)
             import csv
             with open(export_pns, 'w', newline='') as f:
                 writer = csv.writer(f)
                 writer.writerows(sorted_pns)
@@ -111,13 +142,16 @@
 
 
 def extract_pages(infile: str, dst_path: str, identify_set: set):
     skipped = []
     for entry in identify_set:
         name, start, end = entry
         logger.debug(f"Saving {name}")
-        if f"{INVALID_PN}-" in name:  # thats what the datev splitter adds for unknon PNs
+        if name is None:
+            logger.info(f"Skipping page {start} to {end} for a nameless file")
+            skipped.append(entry)
+        elif f"{INVALID_PN}-" in name:  # thats what the datev splitter adds for unknon PNs
             logger.info(f"Skip saving {name} from page {start} to {end} ")
             skipped.append(entry)
         else:
             save(infile, os.path.join(dst_path, name), start, end)
     return skipped
```

### Comparing `Datev-Splitter-0.4.0/pyproject.toml` & `Datev-Splitter-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "loguru>=0.6.0",
     "flake8>=6.0.0",
     "pytest>=7.2.0",
 ]
 requires-python = ">=3.10"
 dynamic = []
 readme = "README.md"
-version = "0.4.0"
+version = "0.5.0"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 datev_splitr = "datev_splitter:datev_split"
```

### Comparing `Datev-Splitter-0.4.0/PKG-INFO` & `Datev-Splitter-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Datev-Splitter
-Version: 0.4.0
+Version: 0.5.0
 Summary: Splits Datev-Reports into single pdf files per Personalnummer.
 License: MIT
 Author-email: Christoph Becker <christoph.becker@exb.de>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Datev Lohnbescheinigung Splitter
```

