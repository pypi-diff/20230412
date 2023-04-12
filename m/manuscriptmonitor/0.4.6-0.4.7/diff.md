# Comparing `tmp/ManuscriptMonitor-0.4.6.tar.gz` & `tmp/ManuscriptMonitor-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManuscriptMonitor-0.4.6.tar", max compression
+gzip compressed data, was "ManuscriptMonitor-0.4.7.tar", max compression
```

## Comparing `ManuscriptMonitor-0.4.6.tar` & `ManuscriptMonitor-0.4.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2022-02-28 23:37:46.940250 ManuscriptMonitor-0.4.6/manuscriptmonitor/__init__.py
--rw-r--r--   0        0        0       96 2022-02-28 23:37:46.941200 ManuscriptMonitor-0.4.6/manuscriptmonitor/__main__.py
--rw-r--r--   0        0        0     4380 2023-04-12 15:59:13.084420 ManuscriptMonitor-0.4.6/manuscriptmonitor/ManuscriptMonitor.py
--rw-r--r--   0        0        0      538 2023-04-12 15:58:23.351782 ManuscriptMonitor-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      830 2023-04-12 15:59:18.430132 ManuscriptMonitor-0.4.6/setup.py
--rw-r--r--   0        0        0      653 2023-04-12 15:59:18.430132 ManuscriptMonitor-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-02-28 23:37:46.940250 ManuscriptMonitor-0.4.7/manuscriptmonitor/__init__.py
+-rw-r--r--   0        0        0       96 2022-02-28 23:37:46.941200 ManuscriptMonitor-0.4.7/manuscriptmonitor/__main__.py
+-rw-r--r--   0        0        0     4378 2023-04-12 16:04:12.665647 ManuscriptMonitor-0.4.7/manuscriptmonitor/ManuscriptMonitor.py
+-rw-r--r--   0        0        0      538 2023-04-12 16:04:30.449822 ManuscriptMonitor-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-04-12 16:04:35.082609 ManuscriptMonitor-0.4.7/setup.py
+-rw-r--r--   0        0        0      653 2023-04-12 16:04:35.082609 ManuscriptMonitor-0.4.7/PKG-INFO
```

### Comparing `ManuscriptMonitor-0.4.6/manuscriptmonitor/ManuscriptMonitor.py` & `ManuscriptMonitor-0.4.7/manuscriptmonitor/ManuscriptMonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 def main():
     capture_output, excel_file = get_folders()
     guide_dict = get_spreadsheet_data(excel_file)
     with Live(generate_table({}, {}, {}), refresh_per_second=10) as live:
         sg.popup_ok(f'ManuscriptMonitor is watching for new image files in {capture_output}\nTo quit, press CTRL + C or close the terminal.')
         for changes in watch(capture_output, watch_filter=CaptureOneFilter()):
             for change, file in natsorted(changes):
-                print(f'{change=}')
+                print(f'{file=}')
                 if change.name == 'added':
                     created = Path(file).name.lower().replace('.iiq', '')
                     version = None
                     for ending in ('_1', '_2', '_3'):
                         if not created.endswith(ending):
                             continue
                         else:
```

### Comparing `ManuscriptMonitor-0.4.6/pyproject.toml` & `ManuscriptMonitor-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ManuscriptMonitor"
-version = "0.4.6"
+version = "0.4.7"
 description = "a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet"
 authors = ["David Flood <davidfloodii@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 watchfiles = "^0.19.0"
```

### Comparing `ManuscriptMonitor-0.4.6/setup.py` & `ManuscriptMonitor-0.4.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'openpyxl>=3.0.9,<4.0.0',
  'pandas>=1.4.1,<2.0.0',
  'rich>=11.2.0,<12.0.0',
  'watchfiles>=0.19.0,<0.20.0']
 
 setup_kwargs = {
     'name': 'manuscriptmonitor',
-    'version': '0.4.6',
+    'version': '0.4.7',
     'description': 'a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet',
     'long_description': None,
     'author': 'David Flood',
     'author_email': 'davidfloodii@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `ManuscriptMonitor-0.4.6/PKG-INFO` & `ManuscriptMonitor-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manuscriptmonitor
-Version: 0.4.6
+Version: 0.4.7
 Summary: a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet
 License: MIT
 Author: David Flood
 Author-email: davidfloodii@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

