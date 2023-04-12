# Comparing `tmp/fipiran-0.8.1.dev0.tar.gz` & `tmp/fipiran-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fipiran-0.8.1.dev0.tar", last modified: Tue Feb  1 14:07:57 2022, max compression
+gzip compressed data, was "fipiran-0.9.0.tar", last modified: Mon Feb 14 14:26:07 2022, max compression
```

## Comparing `fipiran-0.8.1.dev0.tar` & `fipiran-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-02-01 14:07:57.807515 fipiran-0.8.1.dev0/
--rw-rw-rw-   0        0        0    35149 2020-11-06 10:40:17.000000 fipiran-0.8.1.dev0/LICENSE
--rw-rw-rw-   0        0        0       10 2022-02-01 14:07:43.000000 fipiran-0.8.1.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0      948 2022-02-01 14:07:57.807515 fipiran-0.8.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0      399 2021-11-01 22:03:13.000000 fipiran-0.8.1.dev0/README.rst
-drwxrwxrwx   0        0        0        0 2022-02-01 14:07:57.803514 fipiran-0.8.1.dev0/fipiran/
--rw-rw-rw-   0        0        0      702 2022-02-01 14:05:35.000000 fipiran-0.8.1.dev0/fipiran/__init__.py
--rw-rw-rw-   0        0        0     4455 2022-02-01 14:05:13.000000 fipiran-0.8.1.dev0/fipiran/data_service.py
--rw-rw-rw-   0        0        0     2723 2022-02-01 11:12:13.000000 fipiran-0.8.1.dev0/fipiran/funds.py
--rw-rw-rw-   0        0        0     4201 2022-02-01 10:10:43.000000 fipiran-0.8.1.dev0/fipiran/symbols.py
-drwxrwxrwx   0        0        0        0 2022-02-01 14:07:57.807515 fipiran-0.8.1.dev0/fipiran.egg-info/
--rw-rw-rw-   0        0        0      948 2022-02-01 14:07:57.000000 fipiran-0.8.1.dev0/fipiran.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2022-02-01 14:07:57.000000 fipiran-0.8.1.dev0/fipiran.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-01 14:07:57.000000 fipiran-0.8.1.dev0/fipiran.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2022-02-01 14:07:57.000000 fipiran-0.8.1.dev0/fipiran.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-02-01 14:07:57.000000 fipiran-0.8.1.dev0/fipiran.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2021-12-26 16:40:17.000000 fipiran-0.8.1.dev0/fipiran.egg-info/zip-safe
--rw-rw-rw-   0        0        0      248 2021-12-26 16:34:03.000000 fipiran-0.8.1.dev0/pyproject.toml
--rw-rw-rw-   0        0        0      732 2022-02-01 14:07:57.811514 fipiran-0.8.1.dev0/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-02-14 14:26:07.420614 fipiran-0.9.0/
+-rw-rw-rw-   0        0        0    35149 2020-11-06 10:40:17.000000 fipiran-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0       10 2022-02-01 14:07:43.000000 fipiran-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      965 2022-02-14 14:26:07.420614 fipiran-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2021-11-01 22:03:13.000000 fipiran-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2022-02-14 14:26:07.420614 fipiran-0.9.0/fipiran/
+-rw-rw-rw-   0        0        0      944 2022-02-14 14:26:04.000000 fipiran-0.9.0/fipiran/__init__.py
+-rw-rw-rw-   0        0        0     4455 2022-02-01 14:05:13.000000 fipiran-0.9.0/fipiran/data_service.py
+-rw-rw-rw-   0        0        0     2723 2022-02-01 11:12:13.000000 fipiran-0.9.0/fipiran/funds.py
+-rw-rw-rw-   0        0        0     4201 2022-02-01 10:10:43.000000 fipiran-0.9.0/fipiran/symbols.py
+drwxrwxrwx   0        0        0        0 2022-02-14 14:26:07.420614 fipiran-0.9.0/fipiran.egg-info/
+-rw-rw-rw-   0        0        0      965 2022-02-14 14:26:07.000000 fipiran-0.9.0/fipiran.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2022-02-14 14:26:07.000000 fipiran-0.9.0/fipiran.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-14 14:26:07.000000 fipiran-0.9.0/fipiran.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2022-02-14 14:26:07.000000 fipiran-0.9.0/fipiran.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-02-14 14:26:07.000000 fipiran-0.9.0/fipiran.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2021-12-26 16:40:17.000000 fipiran-0.9.0/fipiran.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      248 2021-12-26 16:34:03.000000 fipiran-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0      753 2022-02-14 14:26:07.420614 fipiran-0.9.0/setup.cfg
```

### Comparing `fipiran-0.8.1.dev0/LICENSE` & `fipiran-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fipiran-0.8.1.dev0/PKG-INFO` & `fipiran-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: fipiran
-Version: 0.8.1.dev0
+Version: 0.9.0
 Summary: a library to retrieve data from fipiran.com website
 Home-page: https://github.com/5j9/fipiran
 Author: 5j9
 Author-email: 5j9@users.noreply.github.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: fipiran,client
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 Note: This is package is incomplete and still in initial development phase. The API may change without deprecation.
 
 Requires Python 3.10+.
 
 See also:
```

### Comparing `fipiran-0.8.1.dev0/fipiran/__init__.py` & `fipiran-0.9.0/fipiran/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-__version__ = '0.8.1.dev0'
+__version__ = '0.9.0'
 
-from requests import get as _get
+from json import loads
+from functools import partial as _partial
+
+from urllib3 import PoolManager as _PoolManager, Timeout as _Timeout
 
 # noinspection PyUnresolvedReferences
 from pandas import (
     DataFrame as _DataFrame,
     read_html as _read_html,
     to_datetime as _to_datetime,
 )
@@ -12,18 +15,20 @@
 # noinspection PyUnresolvedReferences
 from jdatetime import datetime as _jdatetime
 
 
 _FIPIRAN = 'https://www.fipiran.ir/'
 _YK = ''.maketrans('يك', 'یک')
 _API = 'https://fund.fipiran.ir/api/v1/'
+_http = _PoolManager(timeout=_Timeout(total=15., connect=5., read=5.))
+_http_get: _http.request = _partial(_http.request, 'GET')
 
 
 def _api(path) -> dict | list:
-    return _get(_API + path).json()
+    return loads(_http_get(_API + path).data)
 
 
-def _fipiran(path: str, data=None, json_resp=False) -> str | dict | list:
-    resp = _get(f'{_FIPIRAN}{path}', data)
+def _fipiran(path: str, fields=None, json_resp=False) -> str | dict | list:
+    data = _http_get(f'{_FIPIRAN}{path}', fields).data
     if json_resp is True:
-        return resp.json()
-    return resp.content.decode().translate(_YK)
+        return loads(data)
+    return data.decode().translate(_YK)
```

### Comparing `fipiran-0.8.1.dev0/fipiran/data_service.py` & `fipiran-0.9.0/fipiran/data_service.py`

 * *Files identical despite different names*

### Comparing `fipiran-0.8.1.dev0/fipiran/funds.py` & `fipiran-0.9.0/fipiran/funds.py`

 * *Files identical despite different names*

### Comparing `fipiran-0.8.1.dev0/fipiran/symbols.py` & `fipiran-0.9.0/fipiran/symbols.py`

 * *Files identical despite different names*

### Comparing `fipiran-0.8.1.dev0/fipiran.egg-info/PKG-INFO` & `fipiran-0.9.0/fipiran.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: fipiran
-Version: 0.8.1.dev0
+Version: 0.9.0
 Summary: a library to retrieve data from fipiran.com website
 Home-page: https://github.com/5j9/fipiran
 Author: 5j9
 Author-email: 5j9@users.noreply.github.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: fipiran,client
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 Note: This is package is incomplete and still in initial development phase. The API may change without deprecation.
 
 Requires Python 3.10+.
 
 See also:
```

### Comparing `fipiran-0.8.1.dev0/setup.cfg` & `fipiran-0.9.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 000001d0: 4c76 3329 0d0a 0950 726f 6772 616d 6d69  Lv3)...Programmi
 000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000001f0: 7974 686f 6e20 3a3a 2033 2e31 300d 0a0d  ython :: 3.10...
 00000200: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 00000210: 6167 6573 203d 2066 6970 6972 616e 0d0a  ages = fipiran..
 00000220: 7a69 705f 7361 6665 203d 2054 7275 650d  zip_safe = True.
 00000230: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000240: 7320 3d20 0d0a 0972 6571 7565 7374 730d  s = ...requests.
-00000250: 0a09 7061 6e64 6173 0d0a 0962 6561 7574  ..pandas...beaut
-00000260: 6966 756c 736f 7570 340d 0a09 6c78 6d6c  ifulsoup4...lxml
-00000270: 0d0a 096a 6461 7465 7469 6d65 0d0a 7079  ...jdatetime..py
-00000280: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000290: 3e3d 332e 3130 0d0a 7465 7374 735f 7265  >=3.10..tests_re
-000002a0: 7175 6972 6520 3d20 7079 7465 7374 0d0a  quire = pytest..
-000002b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000002d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000240: 7320 3d20 0d0a 0975 726c 6c69 6233 0d0a  s = ...urllib3..
+00000250: 0970 616e 6461 730d 0a09 6265 6175 7469  .pandas...beauti
+00000260: 6675 6c73 6f75 7034 0d0a 096c 786d 6c0d  fulsoup4...lxml.
+00000270: 0a09 6a64 6174 6574 696d 650d 0a70 7974  ..jdatetime..pyt
+00000280: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000290: 3d33 2e31 300d 0a0d 0a5b 6f70 7469 6f6e  =3.10....[option
+000002a0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
+000002b0: 5d0d 0a74 6573 7420 3d20 0d0a 0970 7974  ]..test = ...pyt
+000002c0: 6573 740d 0a0d 0a5b 6567 675f 696e 666f  est....[egg_info
+000002d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000002e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000002f0: 0a                                       .
```

