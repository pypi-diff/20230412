# Comparing `tmp/awattar-0.2.0.tar.gz` & `tmp/awattar-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awattar-0.2.0.tar", last modified: Wed Apr 12 15:04:18 2023, max compression
+gzip compressed data, was "awattar-0.2.1.tar", last modified: Wed Apr 12 15:27:08 2023, max compression
```

## Comparing `awattar-0.2.0.tar` & `awattar-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:04:18.537473 awattar-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 15:04:03.000000 awattar-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-12 15:04:18.537473 awattar-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-12 15:04:03.000000 awattar-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:04:18.537473 awattar-0.2.0/awattar/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/marketitem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:04:18.537473 awattar-0.2.0/awattar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:04:18.541474 awattar-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 15:04:03.000000 awattar-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:27:08.347677 awattar-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 15:27:00.000000 awattar-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-12 15:27:08.347677 awattar-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-12 15:27:00.000000 awattar-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:27:08.343676 awattar-0.2.1/awattar/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 15:27:00.000000 awattar-0.2.1/awattar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-12 15:27:00.000000 awattar-0.2.1/awattar/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-12 15:27:00.000000 awattar-0.2.1/awattar/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-12 15:27:00.000000 awattar-0.2.1/awattar/marketitem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:27:08.347677 awattar-0.2.1/awattar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-12 15:27:08.000000 awattar-0.2.1/awattar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 15:27:08.000000 awattar-0.2.1/awattar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:27:08.000000 awattar-0.2.1/awattar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 15:27:08.000000 awattar-0.2.1/awattar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 15:27:08.000000 awattar-0.2.1/awattar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 15:27:08.000000 awattar-0.2.1/awattar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:27:08.347677 awattar-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 15:27:00.000000 awattar-0.2.1/setup.py
```

### Comparing `awattar-0.2.0/LICENSE` & `awattar-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `awattar-0.2.0/PKG-INFO` & `awattar-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awattar
-Version: 0.2.0
+Version: 0.2.1
 Summary: aWATTar Client to analyse the energy market data
 Home-page: https://github.com/Gransi/awattar
 Author: Peter Gransdorfer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -15,27 +15,63 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awattar
 
-
-
-###  Installation
+##  Installation
 
 ```sh
 $ pip install awattar
 ```
 
-This package is tested with Python 3.8.1 
+This package is tested with Python 3.10 
+
+## Command line
+
+Use the command `awattar --help` and `awattar fetch-prices --help` to get more information.
+
+```shell
+$ awattar --help
+Usage: awattar [OPTIONS] COMMAND [ARGS]...
+
+  Access aWATTar's energy prices API.
+
+Options:
+  --country [DE|AT]  the API's target country (either Germany or Austria),
+                     default: AT
+  --help             Show this message and exit.
+
+Commands:
+  fetch-prices  Fetch hourly energy prices
+```
+
+### Command line example
+
+```shell
+$  awattar --country AT fetch-prices --day 2023-02-20
+[
+    {
+        "start": "2023-02-20T00:00:00+01:00",
+        "end": "2023-02-20T01:00:00+01:00",
+        "price": 85.96,
+        "unit": "Eur/MWh",
+        "currency": "Eur",
+        "energy_unit": "MWh",
+        "price_per_kWh": 0.08596
+    },
+    ...
+]
+```
 
-###  Examples
+##  Examples
 
 ```python
+    from awattar.client import AwattarClient
 
     print ('Connect to aWATTar')
     client = AwattarClient('AT') # or DE for Germany
 
     print ('Get marketdata from API')
     data =  client.request()
     
@@ -57,25 +93,25 @@
 2020-08-11 19:00:00 - 2020-08-11 20:00:00 - 0.0465 EUR/kWh
 2020-08-11 20:00:00 - 2020-08-11 21:00:00 - 0.0413 EUR/kWh
 2020-08-11 21:00:00 - 2020-08-11 22:00:00 - 0.0400 EUR/kWh
 2020-08-11 22:00:00 - 2020-08-11 23:00:00 - 0.0369 EUR/kWh
 2020-08-11 23:00:00 - 2020-08-12 00:00:00 - 0.0309 EUR/kWh
 ```
 
-###  Usage
+##  Usage
 
-#### Initialize Awattar Client
+### Initialize Awattar Client
 
 Currently only Austria and Germany are supported
 
 ```python
     client = AwattarClient('AT') # or DE for Germany
 ```
 
-#### Get Market data
+### Get Market data
 
 Get current Market data
 ```python
     data = client.request()
 ```
 
 Get Market data from 2020-05-17
@@ -84,15 +120,15 @@
 ```
 
 Get Market data between 2020-05-18 and 2020-05-19
 ```python
     data = client.request(datetime.datetime(2020, 5, 18), datetime.datetime(2020, 5, 19))
 ```
 
-#### Analyse Market data
+### Analyse Market data
 
 ```python
     print ('Connect to aWATTar')
     client = AwattarClient('AT')
 
     print ('Get Market data from API')
     client.request()
```

### Comparing `awattar-0.2.0/README.md` & `awattar-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,58 @@
 # awattar
 
-
-
-###  Installation
+##  Installation
 
 ```sh
 $ pip install awattar
 ```
 
-This package is tested with Python 3.8.1 
+This package is tested with Python 3.10 
+
+## Command line
+
+Use the command `awattar --help` and `awattar fetch-prices --help` to get more information.
+
+```shell
+$ awattar --help
+Usage: awattar [OPTIONS] COMMAND [ARGS]...
+
+  Access aWATTar's energy prices API.
+
+Options:
+  --country [DE|AT]  the API's target country (either Germany or Austria),
+                     default: AT
+  --help             Show this message and exit.
+
+Commands:
+  fetch-prices  Fetch hourly energy prices
+```
+
+### Command line example
+
+```shell
+$  awattar --country AT fetch-prices --day 2023-02-20
+[
+    {
+        "start": "2023-02-20T00:00:00+01:00",
+        "end": "2023-02-20T01:00:00+01:00",
+        "price": 85.96,
+        "unit": "Eur/MWh",
+        "currency": "Eur",
+        "energy_unit": "MWh",
+        "price_per_kWh": 0.08596
+    },
+    ...
+]
+```
 
-###  Examples
+##  Examples
 
 ```python
+    from awattar.client import AwattarClient
 
     print ('Connect to aWATTar')
     client = AwattarClient('AT') # or DE for Germany
 
     print ('Get marketdata from API')
     data =  client.request()
     
@@ -38,25 +74,25 @@
 2020-08-11 19:00:00 - 2020-08-11 20:00:00 - 0.0465 EUR/kWh
 2020-08-11 20:00:00 - 2020-08-11 21:00:00 - 0.0413 EUR/kWh
 2020-08-11 21:00:00 - 2020-08-11 22:00:00 - 0.0400 EUR/kWh
 2020-08-11 22:00:00 - 2020-08-11 23:00:00 - 0.0369 EUR/kWh
 2020-08-11 23:00:00 - 2020-08-12 00:00:00 - 0.0309 EUR/kWh
 ```
 
-###  Usage
+##  Usage
 
-#### Initialize Awattar Client
+### Initialize Awattar Client
 
 Currently only Austria and Germany are supported
 
 ```python
     client = AwattarClient('AT') # or DE for Germany
 ```
 
-#### Get Market data
+### Get Market data
 
 Get current Market data
 ```python
     data = client.request()
 ```
 
 Get Market data from 2020-05-17
@@ -65,15 +101,15 @@
 ```
 
 Get Market data between 2020-05-18 and 2020-05-19
 ```python
     data = client.request(datetime.datetime(2020, 5, 18), datetime.datetime(2020, 5, 19))
 ```
 
-#### Analyse Market data
+### Analyse Market data
 
 ```python
     print ('Connect to aWATTar')
     client = AwattarClient('AT')
 
     print ('Get Market data from API')
     client.request()
```

### Comparing `awattar-0.2.0/awattar/cli.py` & `awattar-0.2.1/awattar/cli.py`

 * *Files identical despite different names*

### Comparing `awattar-0.2.0/awattar/client.py` & `awattar-0.2.1/awattar/client.py`

 * *Files identical despite different names*

### Comparing `awattar-0.2.0/awattar/marketitem.py` & `awattar-0.2.1/awattar/marketitem.py`

 * *Files identical despite different names*

### Comparing `awattar-0.2.0/awattar.egg-info/PKG-INFO` & `awattar-0.2.1/awattar.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awattar
-Version: 0.2.0
+Version: 0.2.1
 Summary: aWATTar Client to analyse the energy market data
 Home-page: https://github.com/Gransi/awattar
 Author: Peter Gransdorfer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -15,27 +15,63 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # awattar
 
-
-
-###  Installation
+##  Installation
 
 ```sh
 $ pip install awattar
 ```
 
-This package is tested with Python 3.8.1 
+This package is tested with Python 3.10 
+
+## Command line
+
+Use the command `awattar --help` and `awattar fetch-prices --help` to get more information.
+
+```shell
+$ awattar --help
+Usage: awattar [OPTIONS] COMMAND [ARGS]...
+
+  Access aWATTar's energy prices API.
+
+Options:
+  --country [DE|AT]  the API's target country (either Germany or Austria),
+                     default: AT
+  --help             Show this message and exit.
+
+Commands:
+  fetch-prices  Fetch hourly energy prices
+```
+
+### Command line example
+
+```shell
+$  awattar --country AT fetch-prices --day 2023-02-20
+[
+    {
+        "start": "2023-02-20T00:00:00+01:00",
+        "end": "2023-02-20T01:00:00+01:00",
+        "price": 85.96,
+        "unit": "Eur/MWh",
+        "currency": "Eur",
+        "energy_unit": "MWh",
+        "price_per_kWh": 0.08596
+    },
+    ...
+]
+```
 
-###  Examples
+##  Examples
 
 ```python
+    from awattar.client import AwattarClient
 
     print ('Connect to aWATTar')
     client = AwattarClient('AT') # or DE for Germany
 
     print ('Get marketdata from API')
     data =  client.request()
     
@@ -57,25 +93,25 @@
 2020-08-11 19:00:00 - 2020-08-11 20:00:00 - 0.0465 EUR/kWh
 2020-08-11 20:00:00 - 2020-08-11 21:00:00 - 0.0413 EUR/kWh
 2020-08-11 21:00:00 - 2020-08-11 22:00:00 - 0.0400 EUR/kWh
 2020-08-11 22:00:00 - 2020-08-11 23:00:00 - 0.0369 EUR/kWh
 2020-08-11 23:00:00 - 2020-08-12 00:00:00 - 0.0309 EUR/kWh
 ```
 
-###  Usage
+##  Usage
 
-#### Initialize Awattar Client
+### Initialize Awattar Client
 
 Currently only Austria and Germany are supported
 
 ```python
     client = AwattarClient('AT') # or DE for Germany
 ```
 
-#### Get Market data
+### Get Market data
 
 Get current Market data
 ```python
     data = client.request()
 ```
 
 Get Market data from 2020-05-17
@@ -84,15 +120,15 @@
 ```
 
 Get Market data between 2020-05-18 and 2020-05-19
 ```python
     data = client.request(datetime.datetime(2020, 5, 18), datetime.datetime(2020, 5, 19))
 ```
 
-#### Analyse Market data
+### Analyse Market data
 
 ```python
     print ('Connect to aWATTar')
     client = AwattarClient('AT')
 
     print ('Get Market data from API')
     client.request()
```

### Comparing `awattar-0.2.0/setup.py` & `awattar-0.2.1/setup.py`

 * *Files identical despite different names*

