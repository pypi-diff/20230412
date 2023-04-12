# Comparing `tmp/ManuscriptMonitor-0.4.4.tar.gz` & `tmp/ManuscriptMonitor-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManuscriptMonitor-0.4.4.tar", max compression
+gzip compressed data, was "ManuscriptMonitor-0.4.5.tar", max compression
```

## Comparing `ManuscriptMonitor-0.4.4.tar` & `ManuscriptMonitor-0.4.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2022-02-28 23:37:46.940250 ManuscriptMonitor-0.4.4/manuscriptmonitor/__init__.py
--rw-r--r--   0        0        0       96 2022-02-28 23:37:46.941200 ManuscriptMonitor-0.4.4/manuscriptmonitor/__main__.py
--rw-r--r--   0        0        0     4294 2023-04-12 15:16:23.303676 ManuscriptMonitor-0.4.4/manuscriptmonitor/ManuscriptMonitor.py
--rw-r--r--   0        0        0      538 2023-04-12 15:26:59.812499 ManuscriptMonitor-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      830 2023-04-12 15:27:04.144622 ManuscriptMonitor-0.4.4/setup.py
--rw-r--r--   0        0        0      653 2023-04-12 15:27:04.144622 ManuscriptMonitor-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-02-28 23:37:46.940250 ManuscriptMonitor-0.4.5/manuscriptmonitor/__init__.py
+-rw-r--r--   0        0        0       96 2022-02-28 23:37:46.941200 ManuscriptMonitor-0.4.5/manuscriptmonitor/__main__.py
+-rw-r--r--   0        0        0     4301 2023-04-12 15:44:47.998766 ManuscriptMonitor-0.4.5/manuscriptmonitor/ManuscriptMonitor.py
+-rw-r--r--   0        0        0      538 2023-04-12 15:45:08.040376 ManuscriptMonitor-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-04-12 15:48:31.413673 ManuscriptMonitor-0.4.5/setup.py
+-rw-r--r--   0        0        0      653 2023-04-12 15:48:31.414665 ManuscriptMonitor-0.4.5/PKG-INFO
```

### Comparing `ManuscriptMonitor-0.4.4/manuscriptmonitor/ManuscriptMonitor.py` & `ManuscriptMonitor-0.4.5/manuscriptmonitor/ManuscriptMonitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,22 +84,22 @@
     capture_output, excel_file = get_folders()
     guide_dict = get_spreadsheet_data(excel_file)
     with Live(generate_table({}, {}, {}), refresh_per_second=10) as live:
         sg.popup_ok(f'ManuscriptMonitor is watching for new image files in {capture_output}\nTo quit, press CTRL + C or close the terminal.')
         for changes in watch(capture_output, watch_filter=CaptureOneFilter()):
             for change, file in natsorted(changes):
                 if change.name == 'added':
-                    created = Path(file).name.replace('.iiq', '')
+                    created = Path(file).name.lower().replace('.iiq', '')
                     version = None
                     for ending in ('_1', '_2', '_3'):
                         if not created.endswith(ending):
                             continue
                         else:
                             created = created.replace(ending, '')
                             version = ending
                             break
-                    created = re.sub(r'_.+_', '', created).replace('M', '').replace('P', '').lstrip('0')
+                    created = re.sub(r'.+_', '', created).replace('M', '').replace('P', '').lstrip('0')
                     prev, now, next = get_rows(created, guide_dict, version)
                     live.update(generate_table(prev, now, next))
 
 if __name__ == '__main__':
     main()
```

### Comparing `ManuscriptMonitor-0.4.4/pyproject.toml` & `ManuscriptMonitor-0.4.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ManuscriptMonitor"
-version = "0.4.4"
+version = "0.4.5"
 description = "a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet"
 authors = ["David Flood <davidfloodii@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 watchfiles = "^0.19.0"
```

### Comparing `ManuscriptMonitor-0.4.4/setup.py` & `ManuscriptMonitor-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'openpyxl>=3.0.9,<4.0.0',
  'pandas>=1.4.1,<2.0.0',
  'rich>=11.2.0,<12.0.0',
  'watchfiles>=0.19.0,<0.20.0']
 
 setup_kwargs = {
     'name': 'manuscriptmonitor',
-    'version': '0.4.4',
+    'version': '0.4.5',
     'description': 'a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet',
     'long_description': None,
     'author': 'David Flood',
     'author_email': 'davidfloodii@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `ManuscriptMonitor-0.4.4/PKG-INFO` & `ManuscriptMonitor-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manuscriptmonitor
-Version: 0.4.4
+Version: 0.4.5
 Summary: a tool for keeping a ongoing CaptureOne tethered workflow in sync with a guide sheet
 License: MIT
 Author: David Flood
 Author-email: davidfloodii@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

