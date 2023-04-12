# Comparing `tmp/ManuscriptMonitor-0.4.8.tar.gz` & `tmp/ManuscriptMonitor-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManuscriptMonitor-0.4.8.tar", max compression
+gzip compressed data, was "ManuscriptMonitor-0.4.9.tar", max compression
```

## Comparing `ManuscriptMonitor-0.4.8.tar` & `ManuscriptMonitor-0.4.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2022-02-28 23:37:46.940250 ManuscriptMonitor-0.4.8/manuscriptmonitor/__init__.py
--rw-r--r--   0        0        0       96 2022-02-28 23:37:46.941200 ManuscriptMonitor-0.4.8/manuscriptmonitor/__main__.py
--rw-r--r--   0        0        0     4441 2023-04-12 16:25:39.514619 ManuscriptMonitor-0.4.8/manuscriptmonitor/ManuscriptMonitor.py
--rw-r--r--   0        0        0      538 2023-04-12 16:32:07.000585 ManuscriptMonitor-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      830 2023-04-12 16:32:21.971566 ManuscriptMonitor-0.4.8/setup.py
--rw-r--r--   0        0        0      653 2023-04-12 16:32:21.972564 ManuscriptMonitor-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-02-28 23:37:46.940250 ManuscriptMonitor-0.4.9/manuscriptmonitor/__init__.py
+-rw-r--r--   0        0        0       96 2022-02-28 23:37:46.941200 ManuscriptMonitor-0.4.9/manuscriptmonitor/__main__.py
+-rw-r--r--   0        0        0     4402 2023-04-12 16:56:01.048335 ManuscriptMonitor-0.4.9/manuscriptmonitor/ManuscriptMonitor.py
+-rw-r--r--   0        0        0      540 2023-04-12 16:55:35.658818 ManuscriptMonitor-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-04-12 16:56:06.161397 ManuscriptMonitor-0.4.9/setup.py
+-rw-r--r--   0        0        0      613 2023-04-12 16:56:06.162485 ManuscriptMonitor-0.4.9/PKG-INFO
```

### Comparing `ManuscriptMonitor-0.4.8/manuscriptmonitor/ManuscriptMonitor.py` & `ManuscriptMonitor-0.4.9/manuscriptmonitor/ManuscriptMonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import json
 import re
 import sys
 
-from natsort import natsorted
+# from natsort import natsorted
 from rich.table import Table
 from rich.live import Live
 import pandas as pd
 import PySimpleGUI as sg
 from watchfiles import watch, Change, DefaultFilter
 
 class CaptureOneFilter(DefaultFilter):
@@ -82,28 +82,28 @@
 
 def main():
     capture_output, excel_file = get_folders()
     guide_dict = get_spreadsheet_data(excel_file)
     with Live(generate_table({}, {}, {}), refresh_per_second=10) as live:
         sg.popup_ok(f'ManuscriptMonitor is watching for new image files in {capture_output}\nTo quit, press CTRL + C or close the terminal.')
         for changes in watch(capture_output, watch_filter=CaptureOneFilter()):
-            for change, file in natsorted(changes):
+            for change, file in changes:
                 if '~' in file:
                     continue
-                print(f'{file=}')
+                # print(f'{file=}')
                 if change.name == 'added':
                     created = Path(file).name.lower().replace('.iiq', '')
                     version = None
                     for ending in ('_1', '_2', '_3'):
                         if not created.endswith(ending):
                             continue
                         else:
                             created = created.replace(ending, '')
                             version = ending
                             break
-                    created = re.sub(r'.+_', '', created).replace('M', '').replace('P', '').lstrip('0')
-                    print(f'{created=}')
+                    created = re.sub(r'.+_', '', created).lstrip('0')
+                    # print(f'{created=}')
                     prev, now, next = get_rows(created, guide_dict, version)
                     live.update(generate_table(prev, now, next))
 
 if __name__ == '__main__':
     main()
```

### Comparing `ManuscriptMonitor-0.4.8/pyproject.toml` & `ManuscriptMonitor-0.4.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "ManuscriptMonitor"
-version = "0.4.8"
+version = "0.4.9"
 description = "a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet"
 authors = ["David Flood <davidfloodii@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 watchfiles = "^0.19.0"
-natsort = "^8.1.0"
+# natsort = "^8.1.0"
 rich = "^11.2.0"
 pandas = "^1.4.1"
 PySimpleGUI = "^4.47.0"
 openpyxl = "^3.0.9"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `ManuscriptMonitor-0.4.8/setup.py` & `ManuscriptMonitor-0.4.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 ['manuscriptmonitor']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PySimpleGUI>=4.47.0,<5.0.0',
- 'natsort>=8.1.0,<9.0.0',
  'openpyxl>=3.0.9,<4.0.0',
  'pandas>=1.4.1,<2.0.0',
  'rich>=11.2.0,<12.0.0',
  'watchfiles>=0.19.0,<0.20.0']
 
 setup_kwargs = {
     'name': 'manuscriptmonitor',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet',
     'long_description': None,
     'author': 'David Flood',
     'author_email': 'davidfloodii@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `ManuscriptMonitor-0.4.8/PKG-INFO` & `ManuscriptMonitor-0.4.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: manuscriptmonitor
-Version: 0.4.8
+Version: 0.4.9
 Summary: a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet
 License: MIT
 Author: David Flood
 Author-email: davidfloodii@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PySimpleGUI (>=4.47.0,<5.0.0)
-Requires-Dist: natsort (>=8.1.0,<9.0.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: rich (>=11.2.0,<12.0.0)
 Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
```

