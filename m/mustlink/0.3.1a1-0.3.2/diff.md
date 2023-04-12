# Comparing `tmp/mustlink-0.3.1a1.tar.gz` & `tmp/mustlink-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mustlink-0.3.1a1.tar", last modified: Wed Oct 21 13:40:30 2020, max compression
+gzip compressed data, was "mustlink-0.3.2.tar", last modified: Wed Apr 12 12:28:57 2023, max compression
```

## Comparing `mustlink-0.3.1a1.tar` & `mustlink-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 mbentley  (1000) mbentley  (1000)        0 2020-10-21 13:40:30.361966 mustlink-0.3.1a1/
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)     2951 2020-10-21 13:40:30.361966 mustlink-0.3.1a1/PKG-INFO
--rw-r--r--   0 mbentley  (1000) mbentley  (1000)     2046 2020-06-17 14:11:55.000000 mustlink-0.3.1a1/README.md
-drwxrwxr-x   0 mbentley  (1000) mbentley  (1000)        0 2020-10-21 13:40:30.353965 mustlink-0.3.1a1/mustlink/
--rw-r--r--   0 mbentley  (1000) mbentley  (1000)      306 2019-10-24 13:49:04.000000 mustlink-0.3.1a1/mustlink/__init__.py
--rw-r--r--   0 mbentley  (1000) mbentley  (1000)    21681 2020-10-21 13:16:58.000000 mustlink-0.3.1a1/mustlink/mustlink.py
-drwxrwxr-x   0 mbentley  (1000) mbentley  (1000)        0 2020-10-21 13:40:30.353965 mustlink-0.3.1a1/mustlink.egg-info/
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)     2951 2020-10-21 13:40:30.000000 mustlink-0.3.1a1/mustlink.egg-info/PKG-INFO
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)      250 2020-10-21 13:40:30.000000 mustlink-0.3.1a1/mustlink.egg-info/SOURCES.txt
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)        1 2020-10-21 13:40:30.000000 mustlink-0.3.1a1/mustlink.egg-info/dependency_links.txt
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)        1 2020-10-21 13:40:30.000000 mustlink-0.3.1a1/mustlink.egg-info/not-zip-safe
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)       34 2020-10-21 13:40:30.000000 mustlink-0.3.1a1/mustlink.egg-info/requires.txt
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)        9 2020-10-21 13:40:30.000000 mustlink-0.3.1a1/mustlink.egg-info/top_level.txt
--rw-rw-r--   0 mbentley  (1000) mbentley  (1000)       38 2020-10-21 13:40:30.361966 mustlink-0.3.1a1/setup.cfg
--rw-r--r--   0 mbentley  (1000) mbentley  (1000)      682 2020-10-21 13:39:24.000000 mustlink-0.3.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:28:57.272218 mustlink-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 12:28:45.000000 mustlink-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-12 12:28:57.272218 mustlink-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-12 12:28:45.000000 mustlink-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:28:57.268218 mustlink-0.3.2/mustlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-12 12:28:45.000000 mustlink-0.3.2/mustlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28386 2023-04-12 12:28:45.000000 mustlink-0.3.2/mustlink/mustlink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:28:57.268218 mustlink-0.3.2/mustlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-12 12:28:57.000000 mustlink-0.3.2/mustlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-12 12:28:57.000000 mustlink-0.3.2/mustlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:28:57.000000 mustlink-0.3.2/mustlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:28:57.000000 mustlink-0.3.2/mustlink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 12:28:57.000000 mustlink-0.3.2/mustlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 12:28:57.000000 mustlink-0.3.2/mustlink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:28:57.272218 mustlink-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 12:28:45.000000 mustlink-0.3.2/setup.py
```

### Comparing `mustlink-0.3.1a1/PKG-INFO` & `mustlink-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,81 @@
 Metadata-Version: 2.1
 Name: mustlink
-Version: 0.3.1a1
+Version: 0.3.2
 Summary: A python wrapper for the ESA mustlink API
 Home-page: https://github.com/msbentley/mustlink
+Download-URL: https://github.com/msbentley/mustlink/archive/0.3.2.tar.gz
 Author: Mark S. Bentley
 Author-email: mark@lunartech.org
-License: UNKNOWN
-Download-URL: https://github.com/msbentley/mustlink/archive/0.3.1.tar.gz
-Description: # mustlink
-        A python wrapper for the WebMUST API (mustlink)
-        
-        This is a simple wrapper in python for the [WebMUST](https://www.esa.int/Enabling_Support/Operations/WebMUST_br_A_web-based_client_for_MUST) API.
-        
-        ## Dependencies
-        
-        The following dependencies must be met:
-        - python 3
-        - matplotlib
-        - pandas
-        - pyyaml
-        - requests
-        
-        ## Installation
-        
-        First, clone this repository. If you are using conda, the dependencies can be installed in a new environment using the provided environment file:
-        
-        ```conda env create -f environment.yml```
-        
-        The newly created environment can be activated with:
-        
-        ```conda activate mustlink```
-        
-        Otherwise, please make sure the dependencies are installed with your system package manager, or a tool like `pip`. Use of a conda environment or virtualenv is recommended!
-        
-        The package can then be installed with:
-        
-        ```python setup.py install```
-        
-        
-        ## URL
-        
-        The URL for the WebMUST instance in use can be specified when instantiating the Must class. If none is given, a default URL is used. For example:
-        
-        ```python
-        must = mustlink.Must(url='https://mustinstance.com/mustlink')
-        ```
-        
-        ## Authentication
-        
-        Access to WebMUST needs authentication. This is controlled by a config file which can be pointed to by the `config_file` parameter when instantiating the Must class, for example:
-        
-        ```python
-        must = mustlink.Must(config_file='path_to/config.file')
-        ```
-        
-        If nothing is specified, a file `mustlink.yml` is looked for in paths pointed to by the environment variables `APPDATA`, `XDG_CONFIG_HOME` or in the `.config` folder in the user's home directory.
-        
-        The configuration file should be in YAML format and contain the username and password as follows:
-        
-        ```yaml
-        user:
-            login: "userone"
-            password: "blah"
-        ```
-        
-        ## Example
-        
-        The Jupyter notebook included with this repository shows an example of how to use the code. Note that not all API functions are wrapped by this library, but only those that are commonly used. To view the notebook, click [here](https://nbviewer.jupyter.org/github/msbentley/mustlink/blob/master/mustlink_example.ipynb).
-        
 Keywords: telemetry,MUST,ESA
-Platform: UNKNOWN
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mustlink
+A python wrapper for the WebMUST API (mustlink)
+
+This is a simple wrapper in python for the [WebMUST](https://www.esa.int/Enabling_Support/Operations/WebMUST_br_A_web-based_client_for_MUST) API.
+
+## Dependencies
+
+The following dependencies must be met:
+- python 3
+- matplotlib
+- pandas
+- pyyaml
+- requests
+
+## Installation
+
+### pip
+
+```pip install mustlink```
+
+should do the job, although creating a dedicated environment is recommended (see below).
+
+### conda
+
+First, clone this repository. If you are using conda, the dependencies can be installed in a new environment using the provided environment file:
+
+```conda env create -f environment.yml```
+
+The newly created environment can be activated with:
+
+```conda activate mustlink```
+
+Otherwise, please make sure the dependencies are installed with your system package manager, or a tool like `pip`. Use of a conda environment or virtualenv is recommended!
+
+The package can then be installed with:
+
+```python setup.py install```
+
+
+## URL
+
+The URL for the WebMUST instance in use can be specified when instantiating the Must class. If none is given, a default URL is used. For example:
+
+```python
+must = mustlink.Must(url='https://mustinstance.com/mustlink')
+```
+
+## Authentication
+
+Access to WebMUST needs authentication. This is controlled by a config file which can be pointed to by the `config_file` parameter when instantiating the Must class, for example:
+
+```python
+must = mustlink.Must(config_file='path_to/config.file')
+```
+
+If nothing is specified, a file `mustlink.yml` is looked for in paths pointed to by the environment variables `APPDATA`, `XDG_CONFIG_HOME` or in the `.config` folder in the user's home directory.
+
+The configuration file should be in YAML format and contain the username and password as follows:
+
+```yaml
+user:
+    login: "userone"
+    password: "blah"
+```
+
+## Example
+
+The Jupyter notebook included with this repository shows an example of how to use the code. Note that not all API functions are wrapped by this library, but only those that are commonly used. To view the notebook, click [here](https://nbviewer.jupyter.org/github/msbentley/mustlink/blob/master/mustlink_example.ipynb).
```

### Comparing `mustlink-0.3.1a1/README.md` & `mustlink-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 - matplotlib
 - pandas
 - pyyaml
 - requests
 
 ## Installation
 
+### pip
+
+```pip install mustlink```
+
+should do the job, although creating a dedicated environment is recommended (see below).
+
+### conda
+
 First, clone this repository. If you are using conda, the dependencies can be installed in a new environment using the provided environment file:
 
 ```conda env create -f environment.yml```
 
 The newly created environment can be activated with:
 
 ```conda activate mustlink```
```

### Comparing `mustlink-0.3.1a1/mustlink/mustlink.py` & `mustlink-0.3.2/mustlink/mustlink.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,22 +12,26 @@
 
 user:
     login: "userone"
     password: "blah"
 
 """
 
+# from numpy.testing._private.utils import _assert_valid_refcount
 import yaml
 import requests
 import urllib
 import os
 import functools
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.dates as md
+import matplotlib.cm as cm
+
+import numpy as np
 
 from pandas.plotting import register_matplotlib_converters
 register_matplotlib_converters()
 
 import logging
 log = logging.getLogger(__name__)
 
@@ -52,87 +56,98 @@
         try:
             return function(*args, **kwargs)
         except requests.exceptions.HTTPError as e:
             log.error(e)
         except requests.exceptions.RequestException as e: 
             log.error(e)
     return wrapper
+
 class Must:
 
 
-    def __init__(self, url=default_url, config_file=default_config):
+    def __init__(self, url=default_url, config_file=default_config, proxy_url=None):
         """The WebMUST URL instance can be specified, along with a
         YAML config file containing a user section with login and
         password entries. If neither of these are provided, the
-        default values are used"""
+        default values are used.
+        
+        A SOCKS5 proxy can be used - specify as hostname:port"""
 
         self.url = url
         self.config = None
+        self.token = None
+        self.proxy = None if proxy_url is None else dict(http='socks5h://{:s}'.format(proxy_url),https='socks5h://{:s}'.format(proxy_url))
         self.auth(config_file)
         self.get_providers()
         self.default_provider = None
         self.tables = None
 
 
     def _url(self, path):
         """Helper function to append the path to the base URL"""
         
         return self.url + path
 
-
+    @exception
     def auth(self, config_file):
         """Try to authorise with the WebMUST instance using the user
         and password specified in the config file (and loaded into
         self.config). If successful, the returned token is stored for
         use in future calls."""
 
         try:
             f = open(config_file, 'r')
             self.config = yaml.load(f, Loader=yaml.BaseLoader)
             try:
                 r = requests.post(self._url('/auth/login'), json={
                     'username': self.config['user']['login'],
                     'password': self.config['user']['password'],
-                    'maxDuration': 'false'})
+                    'maxDuration': 'false'},
+                    proxies=self.proxy)
                 r.raise_for_status()
                 self.token = r.json()['token']
+                log.debug('token retrieved: {:s}'.format(self.token))
             except (requests.exceptions.RequestException, ConnectionResetError) as err:
                 log.error(err)
         except FileNotFoundError:
             log.error('config file {:s} not found'.format(config_file))
 
+        if self.token is None:
+            log.error('error logging in, please try again')
         self.user = self.get_user()
 
         return
 
     @exception
     def get_user(self):
         """Retrieves information for the currently logged-in user"""
 
         r = requests.get(
                 self._url('/usermanagement/userinfo'),
-                headers={'Authorization': self.token})
+                headers={'Authorization': self.token},
+                proxies=self.proxy)
         r.raise_for_status()
         user = r.json()
         log.info('user {:s} currently logged in'.format(user['login']))
 
         return user
 
 
     @exception
     def get_providers(self):
         """Obtains a list of so-called providers, e.g. BEPICRUISE in
         the case of BepiColombo"""
         
         r = requests.get(
                 self._url('/dataproviders'),
-                headers={'Authorization': self.token})
+                headers={'Authorization': self.token},
+                proxies=self.proxy)
         r.raise_for_status()
         providers = r.json()
-        self.providers = [p['name'] for p in providers if p['user']=='webmust']
+        self.providers = [p['name'] for p in providers if (p['user'] is not None and p['user']!='SCRIPTING ENGINE')]
         log.info('{:d} providers found'.format(len(self.providers)))
 
         return
 
 
     def check_provider(self, provider):
         """Checks that the requested provider is in the list returned
@@ -183,15 +198,16 @@
 
         provider = self.get_provider(provider)
         if provider is None:
             return None
 
         r = requests.get(
             self._url('/dataproviders/{:s}/tables'.format(provider)), 
-            headers={'Authorization': self.token})
+            headers={'Authorization': self.token},
+            proxies=self.proxy)
         r.raise_for_status()
         self.tables[provider] = r.json()
         log.info('provider {:s} has {:d} table(s)'.format(provider, len(r.json())))
 
         return
 
 
@@ -209,15 +225,16 @@
         tables = [table['dataType'] for table in self.tables[provider]]
         if table not in tables:
             log.error('table {:s} invalid for provider {:s}'.format(table, provider))
             return None
 
         r = requests.get(
             self._url('/dataproviders/{:s}/table/{:s}/metadata'.format(provider, table)), 
-            headers={'Authorization': self.token})
+            headers={'Authorization': self.token},
+            proxies=self.proxy)
         r.raise_for_status()
         table_meta = r.json()
         
         return table_meta
 
 
     @exception
@@ -266,15 +283,16 @@
                 'dateFormat': 'fromTo',
                 'from': start_time.strftime(date_format),
                 'to': stop_time.strftime(date_format),
                 'filterKeys': search_key,
                 'filterValues': search_text,
                 'mode': mode.upper(),
                 'representation': fmt.upper(),
-                'maxRows': max_rows})
+                'maxRows': max_rows},
+                proxies=self.proxy)
         log.debug('request URL: {:s}'.format(r.url))
         log.debug('data retrieval done')
 
         r.raise_for_status()
         data = r.json()
         
         if len(data['data']) == 0:
@@ -284,22 +302,27 @@
         cols = data['headers']
 
         table_data = pd.DataFrame([], columns=cols)
         if fmt=='complex':
             datacells = [row['dataCells'] for row in data['data']]
             
             for idx, col in enumerate(cols):
+                if 'cellValue' not in pd.DataFrame(datacells)[idx].iloc[0].keys():
+                    continue
                 col_vals = pd.DataFrame(datacells)[idx].apply( lambda row: row['cellValue'] )
                 table_data[col] = col_vals
         else:
             table_data = pd.DataFrame(data['data'])
 
+        # try to determine any time columns - this doesn't always work!
         time_cols = [col for col in table_data.columns if 'time' in col.lower()]
+        if 'Time Quality' in time_cols:
+            time_cols.remove('Time Quality')
         for col in time_cols:
-            table_data[col] = pd.to_datetime(table_data[col])
+            table_data[col] = pd.to_datetime(table_data[col], errors='coerce')
         
         if not quiet:
             log.info('{:d} table entries retrieved'.format(len(table_data)))
         if len(table_data) == max_rows:
             log.warn('number of rows returned equal to maximum - increase max_rows for more data')
 
         return table_data
@@ -331,27 +354,27 @@
             'elementId': param_name,
             'ssc': 'null',
             'timestamp': start_time.strftime(date_format_ms)[:-3]}
 
         
         params = urllib.parse.urlencode(params, quote_via=urllib.parse.quote)
         r = requests.get(self._url('/web/tables/params/{:s}/{:s}'.format(provider, table)),
-            headers={'Authorization': self.token}, params=params)
+            headers={'Authorization': self.token}, params=params, proxies=self.proxy)
 
         r.raise_for_status()
         data = r.json()
 
         if len(data['data']) == 0:
             log.warn('no data found for the given parameter and time')
             return None
 
         cols = data['headers']
         datacells = [row['dataCells'] for row in data['data']][0]
         table_data = pd.DataFrame(datacells)
-        drop_cols = ['cellValue', 'altText', 'bgColor', 'detail', 'webpagelink', 'rowParams']
+        drop_cols = ['cellValue', 'altText', 'bgColor', 'detail', 'webpagelink', 'rowParams', 'metadata']
         table_data.drop(drop_cols, inplace=True, axis=1)
         table_data.columns = cols
 
         if not quiet:
             log.info('{:d} table entries retrieved'.format(len(table_data)))
 
         return table_data
@@ -369,25 +392,30 @@
                 'key': 'id',
                 'value': id }
         else:
             params = {}
 
         r = requests.get(self._url('/dataproviders/{:s}/aggregations'.format(provider)),
             params = params,
-            headers={'Authorization': self.token})
+            headers={'Authorization': self.token},
+            proxies=self.proxy)
         r.raise_for_status()
 
         return r.json()
 
 
     @exception
     def get_data(self, param_name, start_time=None, stop_time=None, provider=None, calib=False, max_pts=None):
-        """Requests data for a given parameter and time-range. Minimal checking is 
+        """Requests data for given parameter(s) and time-range. Minimal checking is 
         currently performed on the times and return codes. Data are formatted into
-        a Pandas DataFrame with time conversion to UTC performed"""
+        a Pandas DataFrame with time conversion to UTC performed.
+        
+        If a list of parameters is provided these are retrieves individually and
+        the series merged into a DataFrame merging the timestamps if they are
+        identical to the nearest millisecond"""
 
         provider = self.get_provider(provider)
         if provider is None:
             return None
 
         if start_time is None:
             start_time = pd.Timestamp.now() - pd.Timedelta(days=1)
@@ -395,40 +423,62 @@
             start_time = pd.Timestamp(start_time)
 
         if stop_time is None:
             stop_time = pd.Timestamp.now()
         elif type(stop_time) == str:
             stop_time = pd.Timestamp(stop_time)
 
-        r = requests.get(self._url('/dataproviders/{:s}/parameters/data'.format(provider)),
-            headers={'Authorization': self.token},
-            params={
-                'key': 'name',
-                'values': param_name,
-                'from': start_time.strftime(date_format),
-                'to': stop_time.strftime(date_format),
-                'calibrate': 'true' if calib else 'false',
-                'chunkCount': '' if max_pts is None else max_pts})
-        r.raise_for_status()
+        if type(param_name)==str:
+            param_name = [param_name]
 
-        meta = {val['key']: val['value'] for val in r.json()[0]['metadata']}
-        data = pd.DataFrame.from_dict(r.json()[0]['data'])
-        if len(data) == 0:
-            log.warn('no data available for parameter {:s} in this time range'.format(param_name))
-            return None
-        data.date = pd.to_datetime(data.date, unit='ms')
-        data.set_index('date', drop=True, inplace=True)
-        data.rename(columns={'value': meta['name']}, inplace=True)
+        data_list = []
 
-        if not calib:
+        for param in param_name:
+
+            r = requests.get(self._url('/dataproviders/{:s}/parameters/data'.format(provider)),
+                headers={'Authorization': self.token},
+                params={
+                    'key': 'name',
+                    'values': param,
+                    'from': start_time.strftime(date_format),
+                    'to': stop_time.strftime(date_format),
+                    'calibrate': 'true' if calib else 'false',
+                    'chunkCount': '' if max_pts is None else max_pts},
+                    proxies=self.proxy)
+            r.raise_for_status()
+
+            meta = {val['key']: val['value'] for val in r.json()[0]['metadata']}
+            data = pd.DataFrame.from_dict(r.json()[0]['data'])
+            if len(data) == 0:
+                log.warn('no data available for parameter {:s} in this time range'.format(param))
+                continue
+            data.date = pd.to_datetime(data.date, unit='ms')
+            data.set_index('date', drop=True, inplace=True)
+            data.rename(columns={'value': meta['name']}, inplace=True)
+            data_list.append(data)
+
+            if calib:
+                data[param] = data['calibratedValue']
             data.drop('calibratedValue', axis=1, inplace=True)
 
-        log.info('{:d} values retrieved'.format(len(data)))
+            log.info('{:d} values retrieved for parameter {:s}'.format(len(data), param))
 
-        return data
+        if len(data_list)==0:
+            log.warning('no data found for any parameter')
+            return None
+
+        # merged = data_list[0]
+        # for data in data_list[1:]:
+        #     merged = pd.merge_asof(merged, data, left_index=True, right_index=True, tolerance=pd.Timedelta("1ms"))
+
+        merged = pd.concat(data_list, join='outer', axis=1)
+
+        merged.sort_index(inplace=True)
+
+        return merged
 
 
     @exception
     def get_latest_val(self, param_name, provider=None, calib=False):
         """Retrieves the timestamp and value of the last sample for the
         specified parameter"""
 
@@ -442,15 +492,16 @@
         r = requests.get(self._url('/dataproviders/{:s}/parameters/data'.format(provider)),
             headers={'Authorization': self.token},
             params={
                 'key': 'name',
                 'values': param_name,
                 'from': last_t.strftime(date_format),
                 'to': (last_t+pd.Timedelta(seconds=1)).strftime(date_format),
-                'calibrate': 'true' if calib else 'false'})
+                'calibrate': 'true' if calib else 'false'},
+            proxies=self.proxy)
         r.raise_for_status()
 
         data = pd.DataFrame.from_dict(r.json()[0]['data'])
         if len(data) == 0:
             log.warn('no data available for parameter {:s} in this time range'.format(param_name))
             return None
         data.date = pd.to_datetime(data.date, unit='ms')
@@ -461,41 +512,122 @@
             data.drop('calibratedValue', axis=1, inplace=True)
 
         log.info('value retrieved at time {:s}'.format(last_t.strftime(date_format)))
 
         return data
 
 
-    def plot_data(self, param_name, start_time=None, stop_time=None, provider=None, calib=False, max_pts=None):
+    def plot_data(self, param_name, start_time=None, stop_time=None, 
+        provider=None, calib=False, max_pts=None, limits=False):
         """Accepts the same parameters as get_data() and retrieves and plots the data as a
         time series.  Returns a matplotlib axis object."""
 
-        meta = self.get_param_info(param_name)
+        if limits:
+            meta = self.get_param_info(param_name, mode='complex')
+        else:
+            meta = self.get_param_info(param_name, mode='simple')
+
         data = self.get_data(param_name, start_time, stop_time, provider, calib, max_pts)
         if data is None:
             return None
 
         fig, ax = plt.subplots()
         ax.scatter(data.index, data[param_name], marker='.')
+
+        if limits:
+            ax.axhline(meta['hard_high'], linestyle='-', color='r')
+            ax.axhline(meta['hard_low'], linestyle='-', color='r')
+            ax.axhline(meta['soft_high'], linestyle='--', color='y')
+            ax.axhline(meta['soft_low'], linestyle='--', color='y')
+
         ax.set_title(meta['Description'])
         ax.set_xlabel('Date (UTC)')
         if 'Unit' in meta.index:
             ax.set_ylabel(meta['Unit'])
         else:
-            ax.set_ylabel('Raw')
+            ax.set_ylabel('Calibrated') if calib else ax.set_ylabel('Raw')
         ax.grid(True)
         fig.autofmt_xdate()
         xfmt = md.DateFormatter('%Y-%m-%d %H:%M:%S')
         ax.xaxis.set_major_formatter(xfmt)
 
         plt.show()
 
         return ax
 
 
+
+    def plot_timeline(self, param_name, start_time=None, stop_time=None, 
+        provider=None, calib=False, max_pts=None):
+        """Accepts the same parameters as get_data() and retrieves and plots the data as a
+        timeline (broken bar) plot.  Returns a matplotlib axis object."""
+
+        meta = self.get_param_info(param_name, mode='simple')
+        data = self.get_data(param_name, start_time, stop_time, provider, calib, max_pts)
+        data = data.squeeze()
+
+        if data is None:
+            return None
+
+        fig, ax = plt.subplots()
+        
+        # get a list of changes in the data
+        # changes = data[data.diff()!=0].index.tolist() # <-- does not work with strings
+        # changes = data[1:][data[1:].ne(data[1:].shift())].index.tolist()
+        changes = data[data.ne(data.shift())].index.tolist()
+
+        # add the end of the last period
+        changes.append(data.index.max())
+
+        # trying to do gap detection here to NOT fully shade areas where we have no data
+        # first finding the mean periodicity of the data
+        mean = data.index.to_series().diff().mean()
+
+        # now flag periods where the gaps are 2x this
+        gap_ends = data[data.index.to_series().diff()>2*mean].index.tolist()
+
+        # get the durations
+        durations = np.diff(changes)
+
+
+
+        # make a colour index with the correct number of colors, spanning the colourmap
+        colours = cm.get_cmap('viridis')
+
+        # get the list of unique values and create a colour list with this many entries
+        num_unique = len(data.unique())
+        colour_list = [colours(1.*i/num_unique) for i in range(num_unique)]
+        
+        # make a dictionary mapping unique values to colours
+        unique = data.unique().tolist()
+        colors = data[changes].map(dict(zip(unique, colour_list)))
+
+ 
+
+        # now define the x and y ranges 
+        xranges = [(stop, end) for stop, end in zip(changes, durations)]
+        yranges = (1, 0.5)
+
+        # plot it using the broken horizontal bar function
+        ax.broken_barh(xranges, yranges, facecolors=colors, zorder=2)
+        
+        ax.set_title(meta['Description'])
+        ax.set_xlabel('Date (UTC)')
+        # if 'Unit' in meta.index:
+        #     ax.set_ylabel(meta['Unit'])
+        # else:
+        #     ax.set_ylabel('Calibrated') if calib else ax.set_ylabel('Raw')
+        fig.autofmt_xdate()
+        xfmt = md.DateFormatter('%Y-%m-%d %H:%M:%S')
+        ax.xaxis.set_major_formatter(xfmt)
+
+        return ax
+
+
+
     @exception
     def get_param_info(self, param_name, provider=None, mode='simple'):
         """Return meta-data for a single parameter of interest.
         
         Setting mode='complex' will provide additional information such 
         as monitoring checks etc. but this is currently not unpacked."""
 
@@ -510,28 +642,61 @@
         r = requests.get(self._url('/dataproviders/{:s}/parameters'.format(provider)),
         headers={'Authorization': self.token},
         params={
             'key': 'name',
             'value': param_name,
             'search': 'false',
             'mode': mode.upper(),
-            'parameterType': 'TM'})
+            'parameterType': 'TM'},
+        proxies=self.proxy)
         r.raise_for_status()
 
         matches = r.json()
         if len(matches) == 0:
             log.warning('no matches found for parameter {:s}'.format(param_name))
             return None
 
         if mode=='simple':
             param = pd.Series(r.json())
-            param['First Sample'] = pd.NaT if param['First Sample']=='N/A' else pd.to_datetime(param['First Sample'])
-            param['Last Sample'] = pd.NaT if param['Last Sample']=='N/A' else pd.to_datetime(param['Last Sample'])
         else:
-            param = r.json()
+            param = pd.DataFrame.from_dict(r.json()['metadata'])
+            param.set_index('key', inplace=True, drop=True)
+            param = param.squeeze()
+
+            checks = pd.DataFrame.from_dict(r.json()['monitoringChecks'])
+
+            if len(checks.useCalibrated.unique())>1:
+                log.warning('mixed calibration type in checks, ignoring')
+                param['check_cal'] = None
+            else:
+                param['check_cal'] = checks.useCalibrated.unique()[0]
+
+            if len(checks.checkInterpretation.unique())>1:
+                log.warning('mixed interpretation type in checks, ignoring')
+                param['check_type'] = None
+            else:
+                param['check_type'] = checks.checkInterpretation.unique()[0]
+
+            if len(checks)>2:
+                log.warn('extracting limits for parameters with >2 checks no supported')
+            else:
+                for idx, check in checks.iterrows():
+                    details = check.checkDefinitions
+                    if details['type']=='SOFT':
+                        param['soft_low'] = float(details['lowValue'])
+                        param['soft_high'] = float(details['highValue'])
+                    elif details['type']=='HARD':
+                        param['hard_low'] = float(details['lowValue'])
+                        param['hard_high'] = float(details['highValue'])
+                    else:
+                        log.warn('unsupported check type')
+            
+        param['First Sample'] = pd.NaT if param['First Sample']=='N/A' else pd.to_datetime(param['First Sample'])
+        param['Last Sample'] = pd.NaT if param['Last Sample']=='N/A' else pd.to_datetime(param['Last Sample'])
+
 
         log.info('parameter info for {:s} extracted'.format(param.Description))
 
         return param
 
 
     @exception
@@ -553,15 +718,16 @@
 
         r = requests.get(self._url('/dataproviders/{:s}/parameters/statistics'.format(provider)),
             headers={'Authorization': self.token},
             params={
                 'key': 'name',
                 'values': param_name,
                 'from': start_time.strftime(date_format),
-                'to': stop_time.strftime(date_format) })
+                'to': stop_time.strftime(date_format) },
+            proxies=self.proxy)
         r.raise_for_status()
 
         stats = pd.Series(r.json())
         stats['from'] = pd.to_datetime(stats['from'])
         stats['to'] = pd.to_datetime(stats['to'])
         
         log.info('parameter statistics for {:s} extracted'.format(stats.parameter))
@@ -595,15 +761,16 @@
         r = requests.get(self._url('/dataproviders/{:s}/parameters'.format(provider)),
         headers={'Authorization': self.token},
         params={
             'key': search_by_dict[search_by],
             'value': search_text,
             'search': 'true',
             'mode': 'SIMPLE',
-            'parameterType': 'TM'})
+            'parameterType': 'TM'},
+        proxies=self.proxy)
         r.raise_for_status()
 
         matches = r.json()
         if len(matches) == 0:
             log.warning('no matches found for {:s}'.format(search_text))
             return None
 
@@ -629,15 +796,16 @@
 
         r = requests.get(self._url('/metadata/treesearch'),
         headers={'Authorization': self.token},
         params={
             'field': fields,
             'text': text,
             'dataproviders': provider
-        })
+        },
+        proxies=self.proxy)
 
         r.raise_for_status()
 
         data = None
         for d in r.json():
             if d['type'].startswith(provider):
                 data = d
```

### Comparing `mustlink-0.3.1a1/mustlink.egg-info/PKG-INFO` & `mustlink-0.3.2/mustlink.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,81 @@
 Metadata-Version: 2.1
 Name: mustlink
-Version: 0.3.1a1
+Version: 0.3.2
 Summary: A python wrapper for the ESA mustlink API
 Home-page: https://github.com/msbentley/mustlink
+Download-URL: https://github.com/msbentley/mustlink/archive/0.3.2.tar.gz
 Author: Mark S. Bentley
 Author-email: mark@lunartech.org
-License: UNKNOWN
-Download-URL: https://github.com/msbentley/mustlink/archive/0.3.1.tar.gz
-Description: # mustlink
-        A python wrapper for the WebMUST API (mustlink)
-        
-        This is a simple wrapper in python for the [WebMUST](https://www.esa.int/Enabling_Support/Operations/WebMUST_br_A_web-based_client_for_MUST) API.
-        
-        ## Dependencies
-        
-        The following dependencies must be met:
-        - python 3
-        - matplotlib
-        - pandas
-        - pyyaml
-        - requests
-        
-        ## Installation
-        
-        First, clone this repository. If you are using conda, the dependencies can be installed in a new environment using the provided environment file:
-        
-        ```conda env create -f environment.yml```
-        
-        The newly created environment can be activated with:
-        
-        ```conda activate mustlink```
-        
-        Otherwise, please make sure the dependencies are installed with your system package manager, or a tool like `pip`. Use of a conda environment or virtualenv is recommended!
-        
-        The package can then be installed with:
-        
-        ```python setup.py install```
-        
-        
-        ## URL
-        
-        The URL for the WebMUST instance in use can be specified when instantiating the Must class. If none is given, a default URL is used. For example:
-        
-        ```python
-        must = mustlink.Must(url='https://mustinstance.com/mustlink')
-        ```
-        
-        ## Authentication
-        
-        Access to WebMUST needs authentication. This is controlled by a config file which can be pointed to by the `config_file` parameter when instantiating the Must class, for example:
-        
-        ```python
-        must = mustlink.Must(config_file='path_to/config.file')
-        ```
-        
-        If nothing is specified, a file `mustlink.yml` is looked for in paths pointed to by the environment variables `APPDATA`, `XDG_CONFIG_HOME` or in the `.config` folder in the user's home directory.
-        
-        The configuration file should be in YAML format and contain the username and password as follows:
-        
-        ```yaml
-        user:
-            login: "userone"
-            password: "blah"
-        ```
-        
-        ## Example
-        
-        The Jupyter notebook included with this repository shows an example of how to use the code. Note that not all API functions are wrapped by this library, but only those that are commonly used. To view the notebook, click [here](https://nbviewer.jupyter.org/github/msbentley/mustlink/blob/master/mustlink_example.ipynb).
-        
 Keywords: telemetry,MUST,ESA
-Platform: UNKNOWN
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mustlink
+A python wrapper for the WebMUST API (mustlink)
+
+This is a simple wrapper in python for the [WebMUST](https://www.esa.int/Enabling_Support/Operations/WebMUST_br_A_web-based_client_for_MUST) API.
+
+## Dependencies
+
+The following dependencies must be met:
+- python 3
+- matplotlib
+- pandas
+- pyyaml
+- requests
+
+## Installation
+
+### pip
+
+```pip install mustlink```
+
+should do the job, although creating a dedicated environment is recommended (see below).
+
+### conda
+
+First, clone this repository. If you are using conda, the dependencies can be installed in a new environment using the provided environment file:
+
+```conda env create -f environment.yml```
+
+The newly created environment can be activated with:
+
+```conda activate mustlink```
+
+Otherwise, please make sure the dependencies are installed with your system package manager, or a tool like `pip`. Use of a conda environment or virtualenv is recommended!
+
+The package can then be installed with:
+
+```python setup.py install```
+
+
+## URL
+
+The URL for the WebMUST instance in use can be specified when instantiating the Must class. If none is given, a default URL is used. For example:
+
+```python
+must = mustlink.Must(url='https://mustinstance.com/mustlink')
+```
+
+## Authentication
+
+Access to WebMUST needs authentication. This is controlled by a config file which can be pointed to by the `config_file` parameter when instantiating the Must class, for example:
+
+```python
+must = mustlink.Must(config_file='path_to/config.file')
+```
+
+If nothing is specified, a file `mustlink.yml` is looked for in paths pointed to by the environment variables `APPDATA`, `XDG_CONFIG_HOME` or in the `.config` folder in the user's home directory.
+
+The configuration file should be in YAML format and contain the username and password as follows:
+
+```yaml
+user:
+    login: "userone"
+    password: "blah"
+```
+
+## Example
+
+The Jupyter notebook included with this repository shows an example of how to use the code. Note that not all API functions are wrapped by this library, but only those that are commonly used. To view the notebook, click [here](https://nbviewer.jupyter.org/github/msbentley/mustlink/blob/master/mustlink_example.ipynb).
```

### Comparing `mustlink-0.3.1a1/setup.py` & `mustlink-0.3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='mustlink',
-    version='0.3.1a1',
+    version='0.3.2',
     author='Mark S. Bentley',
     author_email='mark@lunartech.org',
     description='A python wrapper for the ESA mustlink API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/msbentley/mustlink",
-    download_url = 'https://github.com/msbentley/mustlink/archive/0.3.1.tar.gz',
-    install_requires=['matplotlib','pandas','pyyaml','requests'],
+    download_url = 'https://github.com/msbentley/mustlink/archive/0.3.2.tar.gz',
+    install_requires=['matplotlib','pandas','pyyaml','requests','pysocks'],
     python_requires='>=3.0',
     keywords = ['telemetry', 'MUST', 'ESA'],
-    packages=['mustlink'],
     zip_safe=False)
```

