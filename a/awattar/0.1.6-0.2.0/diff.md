# Comparing `tmp/awattar-0.1.6.tar.gz` & `tmp/awattar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awattar-0.1.6.tar", last modified: Sat Oct 24 18:07:15 2020, max compression
+gzip compressed data, was "awattar-0.2.0.tar", last modified: Wed Apr 12 15:04:18 2023, max compression
```

## Comparing `awattar-0.1.6.tar` & `awattar-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-24 18:07:15.541600 awattar-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (116)     5236 2020-10-24 18:07:15.541600 awattar-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3577 2020-10-24 18:07:01.000000 awattar-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-24 18:07:15.541600 awattar-0.1.6/awattar/
--rw-r--r--   0 runner    (1001) docker     (116)      189 2020-10-24 18:07:01.000000 awattar-0.1.6/awattar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4835 2020-10-24 18:07:01.000000 awattar-0.1.6/awattar/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1979 2020-10-24 18:07:01.000000 awattar-0.1.6/awattar/marketitem.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-24 18:07:15.541600 awattar-0.1.6/awattar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5236 2020-10-24 18:07:14.000000 awattar-0.1.6/awattar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      242 2020-10-24 18:07:15.000000 awattar-0.1.6/awattar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-24 18:07:14.000000 awattar-0.1.6/awattar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       34 2020-10-24 18:07:14.000000 awattar-0.1.6/awattar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-10-24 18:07:14.000000 awattar-0.1.6/awattar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-24 18:07:15.541600 awattar-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1161 2020-10-24 18:07:01.000000 awattar-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:04:18.537473 awattar-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 15:04:03.000000 awattar-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-12 15:04:18.537473 awattar-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-12 15:04:03.000000 awattar-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:04:18.537473 awattar-0.2.0/awattar/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-12 15:04:03.000000 awattar-0.2.0/awattar/marketitem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:04:18.537473 awattar-0.2.0/awattar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 15:04:18.000000 awattar-0.2.0/awattar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:04:18.541474 awattar-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 15:04:03.000000 awattar-0.2.0/setup.py
```

### Comparing `awattar-0.1.6/PKG-INFO` & `awattar-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,135 +1,135 @@
 Metadata-Version: 2.1
 Name: awattar
-Version: 0.1.6
+Version: 0.2.0
 Summary: aWATTar Client to analyse the energy market data
 Home-page: https://github.com/Gransi/awattar
 Author: Peter Gransdorfer
-License: UNKNOWN
-Description: # awattar
-        
-        
-        
-        ###  Installation
-        
-        ```sh
-        $ pip install awattar
-        ```
-        
-        This package is tested with Python 3.8.1 
-        
-        ###  Examples
-        
-        ```python
-        
-            print ('Connect to aWATTar')
-            client = AwattarClient('AT') # or DE for Germany
-        
-            print ('Get marketdata from API')
-            data =  client.request()
-            
-            for item in data:
-                print(f'{item.start_datetime:%Y-%m-%d %H:%M:%S} - {item.end_datetime:%Y-%m-%d %H:%M:%S} - {(item.marketprice / 1000):.4f} EUR/kWh')
-        
-        ```
-        
-        Output
-        ```
-        Connect to aWATTar
-        Get marketdata from API
-        2020-08-11 13:00:00 - 2020-08-11 14:00:00 - 0.0350 EUR/kWh
-        2020-08-11 14:00:00 - 2020-08-11 15:00:00 - 0.0341 EUR/kWh
-        2020-08-11 15:00:00 - 2020-08-11 16:00:00 - 0.0340 EUR/kWh
-        2020-08-11 16:00:00 - 2020-08-11 17:00:00 - 0.0387 EUR/kWh
-        2020-08-11 17:00:00 - 2020-08-11 18:00:00 - 0.0417 EUR/kWh
-        2020-08-11 18:00:00 - 2020-08-11 19:00:00 - 0.0430 EUR/kWh
-        2020-08-11 19:00:00 - 2020-08-11 20:00:00 - 0.0465 EUR/kWh
-        2020-08-11 20:00:00 - 2020-08-11 21:00:00 - 0.0413 EUR/kWh
-        2020-08-11 21:00:00 - 2020-08-11 22:00:00 - 0.0400 EUR/kWh
-        2020-08-11 22:00:00 - 2020-08-11 23:00:00 - 0.0369 EUR/kWh
-        2020-08-11 23:00:00 - 2020-08-12 00:00:00 - 0.0309 EUR/kWh
-        ```
-        
-        ###  Usage
-        
-        #### Initialize Awattar Client
-        
-        Currently only Austria and Germany are supported
-        
-        ```python
-            client = AwattarClient('AT') # or DE for Germany
-        ```
-        
-        #### Get Market data
-        
-        Get current Market data
-        ```python
-            data = client.request()
-        ```
-        
-        Get Market data from 2020-05-17
-        ```python
-            data = client.request(datetime.datetime(2020, 5, 17))
-        ```
-        
-        Get Market data between 2020-05-18 and 2020-05-19
-        ```python
-            data = client.request(datetime.datetime(2020, 5, 18), datetime.datetime(2020, 5, 19))
-        ```
-        
-        #### Analyse Market data
-        
-        ```python
-            print ('Connect to aWATTar')
-            client = AwattarClient('AT')
-        
-            print ('Get Market data from API')
-            client.request()
-            
-            min_item = client.min()
-            print(f'Min: {min_item.start_datetime:%Y-%m-%d %H:%M:%S} - {min_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(min_item.marketprice / 1000):.4f} EUR/kWh')
-        
-            max_item = client.max()
-            print(f'Max: {max_item.start_datetime:%Y-%m-%d %H:%M:%S} - {max_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(max_item.marketprice / 1000):.4f} EUR/kWh')
-        
-            mean_item = client.mean()
-            print(f'Mean: {mean_item.start_datetime:%Y-%m-%d %H:%M:%S} - {mean_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(mean_item.marketprice / 1000):.4f} EUR/kWh')
-        
-        
-            best_slot = client.best_slot(3)
-            if best_slot is None:
-                print("No slot found")
-            else:        
-                print(f'Best slot 1: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
-        
-            best_slot = client.best_slot(1,datetime.datetime(2020, 10, 5, 0, 0, 0),datetime.datetime(2020, 10, 6, 3, 0, 0))
-            if best_slot is None:
-                print("No slot found")
-            else:        
-                print(f'Best slot 2: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
-        ```
-        
-        Output
-        ```
-        Connect to aWATTar
-        Get Market data from API
-        Min: 2020-10-06 03:00:00 - 2020-10-06 04:00:00 - 0.0107 EUR/kWh
-        Max: 2020-10-05 19:00:00 - 2020-10-05 20:00:00 - 0.0544 EUR/kWh
-        Mean: 2020-10-05 17:00:00 - 2020-10-06 17:00:00 - 0.0349 EUR/kWh
-        Best slot 1: 2020-10-06 02:00:00 - 2020-10-06 05:00:00 - 0.0149 EUR/kWh
-        Best slot 2: 2020-10-06 02:00:00 - 2020-10-06 03:00:00 - 0.0190 EUR/kWh
-        ```
-        
-        # Source code
-        The source code is currently available on Github: [https://github.com/Gransi/awattar](https://github.com/Gransi/awattar)
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# awattar
+
+
+
+###  Installation
+
+```sh
+$ pip install awattar
+```
+
+This package is tested with Python 3.8.1 
+
+###  Examples
+
+```python
+
+    print ('Connect to aWATTar')
+    client = AwattarClient('AT') # or DE for Germany
+
+    print ('Get marketdata from API')
+    data =  client.request()
+    
+    for item in data:
+        print(f'{item.start_datetime:%Y-%m-%d %H:%M:%S} - {item.end_datetime:%Y-%m-%d %H:%M:%S} - {(item.marketprice / 1000):.4f} EUR/kWh')
+
+```
+
+Output
+```
+Connect to aWATTar
+Get marketdata from API
+2020-08-11 13:00:00 - 2020-08-11 14:00:00 - 0.0350 EUR/kWh
+2020-08-11 14:00:00 - 2020-08-11 15:00:00 - 0.0341 EUR/kWh
+2020-08-11 15:00:00 - 2020-08-11 16:00:00 - 0.0340 EUR/kWh
+2020-08-11 16:00:00 - 2020-08-11 17:00:00 - 0.0387 EUR/kWh
+2020-08-11 17:00:00 - 2020-08-11 18:00:00 - 0.0417 EUR/kWh
+2020-08-11 18:00:00 - 2020-08-11 19:00:00 - 0.0430 EUR/kWh
+2020-08-11 19:00:00 - 2020-08-11 20:00:00 - 0.0465 EUR/kWh
+2020-08-11 20:00:00 - 2020-08-11 21:00:00 - 0.0413 EUR/kWh
+2020-08-11 21:00:00 - 2020-08-11 22:00:00 - 0.0400 EUR/kWh
+2020-08-11 22:00:00 - 2020-08-11 23:00:00 - 0.0369 EUR/kWh
+2020-08-11 23:00:00 - 2020-08-12 00:00:00 - 0.0309 EUR/kWh
+```
+
+###  Usage
+
+#### Initialize Awattar Client
+
+Currently only Austria and Germany are supported
+
+```python
+    client = AwattarClient('AT') # or DE for Germany
+```
+
+#### Get Market data
+
+Get current Market data
+```python
+    data = client.request()
+```
+
+Get Market data from 2020-05-17
+```python
+    data = client.request(datetime.datetime(2020, 5, 17))
+```
+
+Get Market data between 2020-05-18 and 2020-05-19
+```python
+    data = client.request(datetime.datetime(2020, 5, 18), datetime.datetime(2020, 5, 19))
+```
+
+#### Analyse Market data
+
+```python
+    print ('Connect to aWATTar')
+    client = AwattarClient('AT')
+
+    print ('Get Market data from API')
+    client.request()
+    
+    min_item = client.min()
+    print(f'Min: {min_item.start_datetime:%Y-%m-%d %H:%M:%S} - {min_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(min_item.marketprice / 1000):.4f} EUR/kWh')
+
+    max_item = client.max()
+    print(f'Max: {max_item.start_datetime:%Y-%m-%d %H:%M:%S} - {max_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(max_item.marketprice / 1000):.4f} EUR/kWh')
+
+    mean_item = client.mean()
+    print(f'Mean: {mean_item.start_datetime:%Y-%m-%d %H:%M:%S} - {mean_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(mean_item.marketprice / 1000):.4f} EUR/kWh')
+
+
+    best_slot = client.best_slot(3)
+    if best_slot is None:
+        print("No slot found")
+    else:        
+        print(f'Best slot 1: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
+
+    best_slot = client.best_slot(1,datetime.datetime(2020, 10, 5, 0, 0, 0),datetime.datetime(2020, 10, 6, 3, 0, 0))
+    if best_slot is None:
+        print("No slot found")
+    else:        
+        print(f'Best slot 2: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
+```
+
+Output
+```
+Connect to aWATTar
+Get Market data from API
+Min: 2020-10-06 03:00:00 - 2020-10-06 04:00:00 - 0.0107 EUR/kWh
+Max: 2020-10-05 19:00:00 - 2020-10-05 20:00:00 - 0.0544 EUR/kWh
+Mean: 2020-10-05 17:00:00 - 2020-10-06 17:00:00 - 0.0349 EUR/kWh
+Best slot 1: 2020-10-06 02:00:00 - 2020-10-06 05:00:00 - 0.0149 EUR/kWh
+Best slot 2: 2020-10-06 02:00:00 - 2020-10-06 03:00:00 - 0.0190 EUR/kWh
+```
+
+# Source code
+The source code is currently available on Github: [https://github.com/Gransi/awattar](https://github.com/Gransi/awattar)
```

### Comparing `awattar-0.1.6/README.md` & `awattar-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `awattar-0.1.6/awattar/client.py` & `awattar-0.2.0/awattar/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,17 +32,23 @@
             Returns list of MarketItem
 
         """                   
 
         #set params
         params = ''
         if start_time != None:
+            #remove microseconds
+            start_time = start_time.replace(microsecond=0)
+
             params = '?start=' + str(int(start_time.timestamp())) + '000'
 
             if end_time != None:
+                #remove microseconds
+                end_time = end_time.replace(microsecond=0)
+
                 #set end timestamp
                 params = params + '&end=' + str(int(end_time.timestamp())) + '000'
 
         #build url
         if self._country == 'AT':
             url = 'https://api.awattar.com/v1/marketdata' + params
         elif self._country == 'DE':
@@ -140,20 +146,20 @@
         best_slot = None
         start_index = None
         start_mean_market_price = None
         start_mean_datetime = None
 
         #clean up start_datetime
         if start_datetime is not None:
-            start_datetime = start_datetime.replace(minute=0, second=0,microsecond=0)
+            start_datetime = start_datetime.replace(minute=0, second=0)
             start_datetime = start_datetime.replace(tzinfo=datetime.timezone.utc)
 
         #clean up end_datetime
         if end_datetime is not None:
-            end_datetime = end_datetime.replace(minute=0, second=0,microsecond=0)
+            end_datetime = end_datetime.replace(minute=0, second=0)
             end_datetime = end_datetime.replace(tzinfo=datetime.timezone.utc)
 
         datalenght = len(self._data) - (durationround - 1)
 
         for i in range(0,datalenght):
 
             item = self._data[i]
@@ -169,8 +175,43 @@
                     sum_slot += self._data[i+x].marketprice
 
                 mean_slot_price = sum_slot / durationround
 
                 if best_slot is None or best_slot.marketprice > (mean_slot_price):
                     best_slot = MarketItem(item.start_datetime, item.start_datetime + datetime .timedelta(hours=durationround),mean_slot_price, item.unit)
 
-        return best_slot        
+        return best_slot
+
+    def today(self):
+        """
+        Get Market data for today
+
+        Returns
+        -------
+        MarketItem:
+            Returns list of MarketItem
+
+        """
+
+       	starttime = datetime.datetime.now(tz=datetime.timezone.utc)
+        starttime = starttime.replace(hour=0, minute=0, second=0)		
+        endtime = starttime.replace(hour=23, minute=0, second=0)
+
+        return self.request(starttime, endtime)
+    
+    def tomorrow(self):
+        """
+        Get Market data for tomorrow
+
+        Returns
+        -------
+        MarketItem:
+            Returns list of MarketItem
+
+        """
+
+       	starttime = datetime.datetime.now(tz=datetime.timezone.utc)
+        starttime = starttime.replace(hour=23, minute=00, second=00) 
+        endtime = starttime.replace(hour=23, minute=0, second=0) + datetime.timedelta(days=1)
+
+        return self.request(starttime, endtime)
+
```

### Comparing `awattar-0.1.6/awattar.egg-info/PKG-INFO` & `awattar-0.2.0/awattar.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,135 +1,135 @@
 Metadata-Version: 2.1
 Name: awattar
-Version: 0.1.6
+Version: 0.2.0
 Summary: aWATTar Client to analyse the energy market data
 Home-page: https://github.com/Gransi/awattar
 Author: Peter Gransdorfer
-License: UNKNOWN
-Description: # awattar
-        
-        
-        
-        ###  Installation
-        
-        ```sh
-        $ pip install awattar
-        ```
-        
-        This package is tested with Python 3.8.1 
-        
-        ###  Examples
-        
-        ```python
-        
-            print ('Connect to aWATTar')
-            client = AwattarClient('AT') # or DE for Germany
-        
-            print ('Get marketdata from API')
-            data =  client.request()
-            
-            for item in data:
-                print(f'{item.start_datetime:%Y-%m-%d %H:%M:%S} - {item.end_datetime:%Y-%m-%d %H:%M:%S} - {(item.marketprice / 1000):.4f} EUR/kWh')
-        
-        ```
-        
-        Output
-        ```
-        Connect to aWATTar
-        Get marketdata from API
-        2020-08-11 13:00:00 - 2020-08-11 14:00:00 - 0.0350 EUR/kWh
-        2020-08-11 14:00:00 - 2020-08-11 15:00:00 - 0.0341 EUR/kWh
-        2020-08-11 15:00:00 - 2020-08-11 16:00:00 - 0.0340 EUR/kWh
-        2020-08-11 16:00:00 - 2020-08-11 17:00:00 - 0.0387 EUR/kWh
-        2020-08-11 17:00:00 - 2020-08-11 18:00:00 - 0.0417 EUR/kWh
-        2020-08-11 18:00:00 - 2020-08-11 19:00:00 - 0.0430 EUR/kWh
-        2020-08-11 19:00:00 - 2020-08-11 20:00:00 - 0.0465 EUR/kWh
-        2020-08-11 20:00:00 - 2020-08-11 21:00:00 - 0.0413 EUR/kWh
-        2020-08-11 21:00:00 - 2020-08-11 22:00:00 - 0.0400 EUR/kWh
-        2020-08-11 22:00:00 - 2020-08-11 23:00:00 - 0.0369 EUR/kWh
-        2020-08-11 23:00:00 - 2020-08-12 00:00:00 - 0.0309 EUR/kWh
-        ```
-        
-        ###  Usage
-        
-        #### Initialize Awattar Client
-        
-        Currently only Austria and Germany are supported
-        
-        ```python
-            client = AwattarClient('AT') # or DE for Germany
-        ```
-        
-        #### Get Market data
-        
-        Get current Market data
-        ```python
-            data = client.request()
-        ```
-        
-        Get Market data from 2020-05-17
-        ```python
-            data = client.request(datetime.datetime(2020, 5, 17))
-        ```
-        
-        Get Market data between 2020-05-18 and 2020-05-19
-        ```python
-            data = client.request(datetime.datetime(2020, 5, 18), datetime.datetime(2020, 5, 19))
-        ```
-        
-        #### Analyse Market data
-        
-        ```python
-            print ('Connect to aWATTar')
-            client = AwattarClient('AT')
-        
-            print ('Get Market data from API')
-            client.request()
-            
-            min_item = client.min()
-            print(f'Min: {min_item.start_datetime:%Y-%m-%d %H:%M:%S} - {min_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(min_item.marketprice / 1000):.4f} EUR/kWh')
-        
-            max_item = client.max()
-            print(f'Max: {max_item.start_datetime:%Y-%m-%d %H:%M:%S} - {max_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(max_item.marketprice / 1000):.4f} EUR/kWh')
-        
-            mean_item = client.mean()
-            print(f'Mean: {mean_item.start_datetime:%Y-%m-%d %H:%M:%S} - {mean_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(mean_item.marketprice / 1000):.4f} EUR/kWh')
-        
-        
-            best_slot = client.best_slot(3)
-            if best_slot is None:
-                print("No slot found")
-            else:        
-                print(f'Best slot 1: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
-        
-            best_slot = client.best_slot(1,datetime.datetime(2020, 10, 5, 0, 0, 0),datetime.datetime(2020, 10, 6, 3, 0, 0))
-            if best_slot is None:
-                print("No slot found")
-            else:        
-                print(f'Best slot 2: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
-        ```
-        
-        Output
-        ```
-        Connect to aWATTar
-        Get Market data from API
-        Min: 2020-10-06 03:00:00 - 2020-10-06 04:00:00 - 0.0107 EUR/kWh
-        Max: 2020-10-05 19:00:00 - 2020-10-05 20:00:00 - 0.0544 EUR/kWh
-        Mean: 2020-10-05 17:00:00 - 2020-10-06 17:00:00 - 0.0349 EUR/kWh
-        Best slot 1: 2020-10-06 02:00:00 - 2020-10-06 05:00:00 - 0.0149 EUR/kWh
-        Best slot 2: 2020-10-06 02:00:00 - 2020-10-06 03:00:00 - 0.0190 EUR/kWh
-        ```
-        
-        # Source code
-        The source code is currently available on Github: [https://github.com/Gransi/awattar](https://github.com/Gransi/awattar)
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# awattar
+
+
+
+###  Installation
+
+```sh
+$ pip install awattar
+```
+
+This package is tested with Python 3.8.1 
+
+###  Examples
+
+```python
+
+    print ('Connect to aWATTar')
+    client = AwattarClient('AT') # or DE for Germany
+
+    print ('Get marketdata from API')
+    data =  client.request()
+    
+    for item in data:
+        print(f'{item.start_datetime:%Y-%m-%d %H:%M:%S} - {item.end_datetime:%Y-%m-%d %H:%M:%S} - {(item.marketprice / 1000):.4f} EUR/kWh')
+
+```
+
+Output
+```
+Connect to aWATTar
+Get marketdata from API
+2020-08-11 13:00:00 - 2020-08-11 14:00:00 - 0.0350 EUR/kWh
+2020-08-11 14:00:00 - 2020-08-11 15:00:00 - 0.0341 EUR/kWh
+2020-08-11 15:00:00 - 2020-08-11 16:00:00 - 0.0340 EUR/kWh
+2020-08-11 16:00:00 - 2020-08-11 17:00:00 - 0.0387 EUR/kWh
+2020-08-11 17:00:00 - 2020-08-11 18:00:00 - 0.0417 EUR/kWh
+2020-08-11 18:00:00 - 2020-08-11 19:00:00 - 0.0430 EUR/kWh
+2020-08-11 19:00:00 - 2020-08-11 20:00:00 - 0.0465 EUR/kWh
+2020-08-11 20:00:00 - 2020-08-11 21:00:00 - 0.0413 EUR/kWh
+2020-08-11 21:00:00 - 2020-08-11 22:00:00 - 0.0400 EUR/kWh
+2020-08-11 22:00:00 - 2020-08-11 23:00:00 - 0.0369 EUR/kWh
+2020-08-11 23:00:00 - 2020-08-12 00:00:00 - 0.0309 EUR/kWh
+```
+
+###  Usage
+
+#### Initialize Awattar Client
+
+Currently only Austria and Germany are supported
+
+```python
+    client = AwattarClient('AT') # or DE for Germany
+```
+
+#### Get Market data
+
+Get current Market data
+```python
+    data = client.request()
+```
+
+Get Market data from 2020-05-17
+```python
+    data = client.request(datetime.datetime(2020, 5, 17))
+```
+
+Get Market data between 2020-05-18 and 2020-05-19
+```python
+    data = client.request(datetime.datetime(2020, 5, 18), datetime.datetime(2020, 5, 19))
+```
+
+#### Analyse Market data
+
+```python
+    print ('Connect to aWATTar')
+    client = AwattarClient('AT')
+
+    print ('Get Market data from API')
+    client.request()
+    
+    min_item = client.min()
+    print(f'Min: {min_item.start_datetime:%Y-%m-%d %H:%M:%S} - {min_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(min_item.marketprice / 1000):.4f} EUR/kWh')
+
+    max_item = client.max()
+    print(f'Max: {max_item.start_datetime:%Y-%m-%d %H:%M:%S} - {max_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(max_item.marketprice / 1000):.4f} EUR/kWh')
+
+    mean_item = client.mean()
+    print(f'Mean: {mean_item.start_datetime:%Y-%m-%d %H:%M:%S} - {mean_item.end_datetime:%Y-%m-%d %H:%M:%S} - {(mean_item.marketprice / 1000):.4f} EUR/kWh')
+
+
+    best_slot = client.best_slot(3)
+    if best_slot is None:
+        print("No slot found")
+    else:        
+        print(f'Best slot 1: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
+
+    best_slot = client.best_slot(1,datetime.datetime(2020, 10, 5, 0, 0, 0),datetime.datetime(2020, 10, 6, 3, 0, 0))
+    if best_slot is None:
+        print("No slot found")
+    else:        
+        print(f'Best slot 2: {best_slot.start_datetime:%Y-%m-%d %H:%M:%S} - {best_slot.end_datetime:%Y-%m-%d %H:%M:%S} - {(best_slot.marketprice / 1000):.4f} EUR/kWh')
+```
+
+Output
+```
+Connect to aWATTar
+Get Market data from API
+Min: 2020-10-06 03:00:00 - 2020-10-06 04:00:00 - 0.0107 EUR/kWh
+Max: 2020-10-05 19:00:00 - 2020-10-05 20:00:00 - 0.0544 EUR/kWh
+Mean: 2020-10-05 17:00:00 - 2020-10-06 17:00:00 - 0.0349 EUR/kWh
+Best slot 1: 2020-10-06 02:00:00 - 2020-10-06 05:00:00 - 0.0149 EUR/kWh
+Best slot 2: 2020-10-06 02:00:00 - 2020-10-06 03:00:00 - 0.0190 EUR/kWh
+```
+
+# Source code
+The source code is currently available on Github: [https://github.com/Gransi/awattar](https://github.com/Gransi/awattar)
```

### Comparing `awattar-0.1.6/setup.py` & `awattar-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,25 @@
     author="Peter Gransdorfer",    
     description="aWATTar Client to analyse the energy market data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Gransi/awattar",
     packages=setuptools.find_packages(),
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',        
     ],
-    install_requires=['requests', 'datetime', 'python-dateutil'],
-    python_requires='>=3.6'
-)
+    install_requires=['requests', 'datetime', 'python-dateutil', 'click'],
+    python_requires='>=3.6',
+    entry_points={
+            'console_scripts': [
+                'awattar = awattar:_cli',
+            ]
+    },
+    )
```

