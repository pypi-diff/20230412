# Comparing `tmp/oekofen_api-0.0.6.tar.gz` & `tmp/oekofen_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oekofen_api-0.0.6.tar", last modified: Sun Jan 22 22:29:02 2023, max compression
+gzip compressed data, was "oekofen_api-0.0.7.tar", last modified: Mon Jan 23 09:01:58 2023, max compression
```

## Comparing `oekofen_api-0.0.6.tar` & `oekofen_api-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-01-22 22:29:02.848104 oekofen_api-0.0.6/
--rw-r--r--   0 christian  (1000) christian  (1000)     1074 2023-01-21 15:27:10.000000 oekofen_api-0.0.6/LICENSE
--rw-r--r--   0 christian  (1000) christian  (1000)     1359 2023-01-22 22:29:02.848104 oekofen_api-0.0.6/PKG-INFO
--rw-r--r--   0 christian  (1000) christian  (1000)      822 2023-01-22 22:26:28.000000 oekofen_api-0.0.6/README.md
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-01-22 22:29:02.848104 oekofen_api-0.0.6/oekofen_api/
--rw-r--r--   0 christian  (1000) christian  (1000)     9099 2023-01-22 22:22:51.000000 oekofen_api-0.0.6/oekofen_api/__init__.py
--rw-r--r--   0 christian  (1000) christian  (1000)     2996 2023-01-21 18:08:58.000000 oekofen_api-0.0.6/oekofen_api/const.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-01-22 22:29:02.848104 oekofen_api-0.0.6/oekofen_api.egg-info/
--rw-r--r--   0 christian  (1000) christian  (1000)     1359 2023-01-22 22:29:02.000000 oekofen_api-0.0.6/oekofen_api.egg-info/PKG-INFO
--rw-r--r--   0 christian  (1000) christian  (1000)      255 2023-01-22 22:29:02.000000 oekofen_api-0.0.6/oekofen_api.egg-info/SOURCES.txt
--rw-r--r--   0 christian  (1000) christian  (1000)        1 2023-01-22 22:29:02.000000 oekofen_api-0.0.6/oekofen_api.egg-info/dependency_links.txt
--rw-r--r--   0 christian  (1000) christian  (1000)       34 2023-01-22 22:29:02.000000 oekofen_api-0.0.6/oekofen_api.egg-info/requires.txt
--rw-r--r--   0 christian  (1000) christian  (1000)       12 2023-01-22 22:29:02.000000 oekofen_api-0.0.6/oekofen_api.egg-info/top_level.txt
--rw-r--r--   0 christian  (1000) christian  (1000)       79 2023-01-22 22:29:02.848104 oekofen_api-0.0.6/setup.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)      862 2023-01-22 22:27:02.000000 oekofen_api-0.0.6/setup.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-01-23 09:01:58.643036 oekofen_api-0.0.7/
+-rw-r--r--   0 christian  (1000) christian  (1000)     1074 2023-01-21 15:27:10.000000 oekofen_api-0.0.7/LICENSE
+-rw-r--r--   0 christian  (1000) christian  (1000)     1603 2023-01-23 09:01:58.643036 oekofen_api-0.0.7/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)     1066 2023-01-22 22:45:58.000000 oekofen_api-0.0.7/README.md
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-01-23 09:01:58.643036 oekofen_api-0.0.7/oekofen_api/
+-rw-r--r--   0 christian  (1000) christian  (1000)    10039 2023-01-23 08:53:55.000000 oekofen_api-0.0.7/oekofen_api/__init__.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     2996 2023-01-21 18:08:58.000000 oekofen_api-0.0.7/oekofen_api/const.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-01-23 09:01:58.643036 oekofen_api-0.0.7/oekofen_api.egg-info/
+-rw-r--r--   0 christian  (1000) christian  (1000)     1603 2023-01-23 09:01:58.000000 oekofen_api-0.0.7/oekofen_api.egg-info/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)      255 2023-01-23 09:01:58.000000 oekofen_api-0.0.7/oekofen_api.egg-info/SOURCES.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)        1 2023-01-23 09:01:58.000000 oekofen_api-0.0.7/oekofen_api.egg-info/dependency_links.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)       34 2023-01-23 09:01:58.000000 oekofen_api-0.0.7/oekofen_api.egg-info/requires.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)       12 2023-01-23 09:01:58.000000 oekofen_api-0.0.7/oekofen_api.egg-info/top_level.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)       79 2023-01-23 09:01:58.643036 oekofen_api-0.0.7/setup.cfg
+-rw-r--r--   0 christian  (1000) christian  (1000)      862 2023-01-23 08:33:16.000000 oekofen_api-0.0.7/setup.py
```

### Comparing `oekofen_api-0.0.6/LICENSE` & `oekofen_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oekofen_api-0.0.6/PKG-INFO` & `oekofen_api-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: oekofen_api
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library to retrieve statistics from your Oekofen Pelletronic
 Home-page: https://github.com/ckarrie/oekofen-api
-Download-URL: https://github.com/ckarrie/oekofen-api/archive/refs/tags/v0.0.6.tar.gz
+Download-URL: https://github.com/ckarrie/oekofen-api/archive/refs/tags/v0.0.7.tar.gz
 Author: Christian Karrié
 Author-email: ckarrie@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,7 +44,18 @@
         print(old_value, new_value)
         old_value = new_value
 
 #asyncio.run(client.set_heating_circuit_temp(celsius=23))
 
 
 ```
+
+
+## Todo
+
+- dont use `domains` and `attributes`- make it less complicate and pass dict to homeassistant, then use data scheme like netgear integration
+
+
+## References
+
+- https://github.com/JbPasquier/pyokofen/blob/master/pyokofen/okofen.py
+-
```

### Comparing `oekofen_api-0.0.6/oekofen_api/__init__.py` & `oekofen_api-0.0.7/oekofen_api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 logger = logging.getLogger(__name__)
 
 
 class Oekofen(object):
     def __init__(self, host: str, json_password: str, port: int = const.DEFAULT_PORT, update_interval: int = const.UPDATE_INTERVAL_SECONDS):
         self.host = host
         self.update_interval = update_interval
-        self._data = {}
+        self._raw_data = {}
+        self.data = {}
         self._last_fetch = datetime.now()
         self._status = None
         self.domains = OrderedDict()
         self.base_url = const.BASE_URL_TMPL.format(
             host=host,
             port=port,
             json_password=json_password
@@ -30,35 +31,57 @@
 
     def __repr__(self):
         cls_name = self.__class__.__name__
         return f"{cls_name}({self.host})"
 
     async def update_data(self):
         if not self._has_valid_data():
-            self._data = await self._fetch_data(path=const.URL_PATH_ALL_WITH_FORMATS)
+            self._raw_data = await self._fetch_data(path=const.URL_PATH_ALL_WITH_FORMATS)
             self._last_fetch = datetime.now()
             self.domains = OrderedDict()
 
+            self.data = {
+                'hk_indexes': [],
+                'pu_indexes': [],
+                'ww_indexes': [],
+                'circ_indexes': [],
+                'pe_indexes': [],
+            }
+
             # Domain part
-            for domain_with_index, attributes_dict in self._data.items():
+            for domain_with_index, attributes_dict in self._raw_data.items():
                 index_nrs = re.findall(const.RE_FIND_NUMBERS, domain_with_index)
                 if index_nrs:
-                    index_nr = index_nrs[0]
+                    index_nr = int(index_nrs[0])
                 else:
-                    index_nr = 0
+                    index_nr = None
                 domain_name = domain_with_index.replace(str(index_nr), '')
                 domain = Domain(oekofen=self, name=domain_name, index=index_nr)
                 if domain_name in self.domains:
                     self.domains[domain_name].append(domain)
                 else:
                     self.domains[domain_name] = [domain]
 
+                if index_nr is not None:
+                    self.data.setdefault(f'{domain_name}_indexes', [])
+                    self.data[f'{domain_name}_indexes'].append(index_nr)
+
                 # Attribute part
                 domain.update_attributes(data=attributes_dict)
 
+                # data-Part
+                for att_key, att_value in attributes_dict.items():
+                    if index_nr is None:
+                        index_nr = 1
+                    att_rendered_value = self._get_value(domain=domain_name, attribute=att_key, domain_index=index_nr)
+                    self.data[f'{domain_with_index}.{att_key}'] = att_rendered_value
+
+            if isinstance(self.data, dict) and 'system.system_info' in self.data:
+                return self.data
+
     async def _fetch_data(self, path, is_json=True) -> Optional(dict):
         raw_url = f'{self.base_url}{path}'
         print("_fetch_data", raw_url)
         async with aiohttp.ClientSession(raise_for_status=True) as session:
             try:
                 resp = await session.get(raw_url)
                 if resp.status == 200:
@@ -73,15 +96,15 @@
 
             except Exception as e:
                 logger.error(e)
                 raise
 
     def _has_valid_data(self):
         data_is_old = (datetime.now() - self._last_fetch).total_seconds() >= self.update_interval
-        if (not self._data) or data_is_old:
+        if (not self._raw_data) or data_is_old:
             return False
         return True
 
     def _get_value(self, domain: str, attribute: str, domain_index: int = 1, return_attribute=False):
         if domain_index < 1:
             return None
         if not self.domains:
```

### Comparing `oekofen_api-0.0.6/oekofen_api/const.py` & `oekofen_api-0.0.7/oekofen_api/const.py`

 * *Files identical despite different names*

### Comparing `oekofen_api-0.0.6/oekofen_api.egg-info/PKG-INFO` & `oekofen_api-0.0.7/oekofen_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: oekofen-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library to retrieve statistics from your Oekofen Pelletronic
 Home-page: https://github.com/ckarrie/oekofen-api
-Download-URL: https://github.com/ckarrie/oekofen-api/archive/refs/tags/v0.0.6.tar.gz
+Download-URL: https://github.com/ckarrie/oekofen-api/archive/refs/tags/v0.0.7.tar.gz
 Author: Christian Karrié
 Author-email: ckarrie@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,7 +44,18 @@
         print(old_value, new_value)
         old_value = new_value
 
 #asyncio.run(client.set_heating_circuit_temp(celsius=23))
 
 
 ```
+
+
+## Todo
+
+- dont use `domains` and `attributes`- make it less complicate and pass dict to homeassistant, then use data scheme like netgear integration
+
+
+## References
+
+- https://github.com/JbPasquier/pyokofen/blob/master/pyokofen/okofen.py
+-
```

### Comparing `oekofen_api-0.0.6/setup.py` & `oekofen_api-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 setup(
     name="oekofen_api",
     version=VERSION,
     author="Christian Karrié",
     author_email="ckarrie@gmail.com",
     description="A python library to retrieve statistics from your Oekofen Pelletronic",
```

