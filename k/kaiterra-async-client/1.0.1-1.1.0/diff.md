# Comparing `tmp/kaiterra-async-client-1.0.1.tar.gz` & `tmp/kaiterra-async-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaiterra-async-client-1.0.1.tar", last modified: Tue Apr 11 17:29:35 2023, max compression
+gzip compressed data, was "kaiterra-async-client-1.1.0.tar", last modified: Wed Apr 12 12:33:49 2023, max compression
```

## Comparing `kaiterra-async-client-1.0.1.tar` & `kaiterra-async-client-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/
--rw-r--r--   0 michal    (1000) michal    (1000)     1065 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/LICENSE
--rw-r--r--   0 michal    (1000) michal    (1000)       73 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/MANIFEST.in
--rw-r--r--   0 michal    (1000) michal    (1000)      517 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/Makefile
--rw-r--r--   0 michal    (1000) michal    (1000)     1803 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/PKG-INFO
--rw-r--r--   0 michal    (1000) michal    (1000)     1153 2023-04-11 16:33:21.000000 kaiterra-async-client-1.0.1/README.rst
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/kaiterra_async_client/
--rw-r--r--   0 michal    (1000) michal    (1000)      183 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/kaiterra_async_client/__init__.py
--rw-r--r--   0 michal    (1000) michal    (1000)     8088 2023-04-11 16:34:31.000000 kaiterra-async-client-1.0.1/kaiterra_async_client/client.py
--rw-r--r--   0 michal    (1000) michal    (1000)      484 2023-04-11 16:18:08.000000 kaiterra-async-client-1.0.1/kaiterra_async_client/dateutil.py
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/
--rw-r--r--   0 michal    (1000) michal    (1000)     1803 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/PKG-INFO
--rw-r--r--   0 michal    (1000) michal    (1000)      372 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/SOURCES.txt
--rw-r--r--   0 michal    (1000) michal    (1000)        1 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/dependency_links.txt
--rw-r--r--   0 michal    (1000) michal    (1000)       15 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/requires.txt
--rw-r--r--   0 michal    (1000) michal    (1000)       22 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/top_level.txt
--rw-r--r--   0 michal    (1000) michal    (1000)       38 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/setup.cfg
--rw-r--r--   0 michal    (1000) michal    (1000)     1118 2023-04-11 17:04:37.000000 kaiterra-async-client-1.0.1/setup.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-12 12:33:49.442341 kaiterra-async-client-1.1.0/
+-rw-r--r--   0 michal    (1000) michal    (1000)     1065 2022-07-07 20:59:04.000000 kaiterra-async-client-1.1.0/LICENSE
+-rw-r--r--   0 michal    (1000) michal    (1000)       73 2022-07-07 20:59:04.000000 kaiterra-async-client-1.1.0/MANIFEST.in
+-rw-r--r--   0 michal    (1000) michal    (1000)      517 2022-07-07 20:59:04.000000 kaiterra-async-client-1.1.0/Makefile
+-rw-r--r--   0 michal    (1000) michal    (1000)     1807 2023-04-12 12:33:49.442341 kaiterra-async-client-1.1.0/PKG-INFO
+-rw-r--r--   0 michal    (1000) michal    (1000)     1157 2023-04-12 12:33:03.000000 kaiterra-async-client-1.1.0/README.rst
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-12 12:33:49.441341 kaiterra-async-client-1.1.0/kaiterra_async_client/
+-rw-r--r--   0 michal    (1000) michal    (1000)      183 2023-04-12 12:29:12.000000 kaiterra-async-client-1.1.0/kaiterra_async_client/__init__.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     8340 2023-04-12 12:27:59.000000 kaiterra-async-client-1.1.0/kaiterra_async_client/client.py
+-rw-r--r--   0 michal    (1000) michal    (1000)      507 2023-04-12 12:29:10.000000 kaiterra-async-client-1.1.0/kaiterra_async_client/dateutil.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-12 12:33:49.442341 kaiterra-async-client-1.1.0/kaiterra_async_client.egg-info/
+-rw-r--r--   0 michal    (1000) michal    (1000)     1807 2023-04-12 12:33:49.000000 kaiterra-async-client-1.1.0/kaiterra_async_client.egg-info/PKG-INFO
+-rw-r--r--   0 michal    (1000) michal    (1000)      372 2023-04-12 12:33:49.000000 kaiterra-async-client-1.1.0/kaiterra_async_client.egg-info/SOURCES.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)        1 2023-04-12 12:33:49.000000 kaiterra-async-client-1.1.0/kaiterra_async_client.egg-info/dependency_links.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       15 2023-04-12 12:33:49.000000 kaiterra-async-client-1.1.0/kaiterra_async_client.egg-info/requires.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       22 2023-04-12 12:33:49.000000 kaiterra-async-client-1.1.0/kaiterra_async_client.egg-info/top_level.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       38 2023-04-12 12:33:49.442341 kaiterra-async-client-1.1.0/setup.cfg
+-rw-r--r--   0 michal    (1000) michal    (1000)     1096 2023-04-12 12:28:45.000000 kaiterra-async-client-1.1.0/setup.py
```

### Comparing `kaiterra-async-client-1.0.1/LICENSE` & `kaiterra-async-client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaiterra-async-client-1.0.1/Makefile` & `kaiterra-async-client-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `kaiterra-async-client-1.0.1/PKG-INFO` & `kaiterra-async-client-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiterra-async-client
-Version: 1.0.1
+Version: 1.1.0
 Summary: Kaiterra API Async Client
 Home-page: https://github.com/Michsior14/python-kaiterra-async-client
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,16 +41,16 @@
 
 	import aiohttp
 	from kaiterra_async_client import KaiterraAPIClient
 
 	async with aiohttp.ClientSession() as session:
 		client = KaiterraAPIClient(session, api_key='YOUR_API_KEY_HERE')
 		r = await client.get_latest_sensor_readings([
-			'/lasereggs/00000000-0001-0001-0000-00007e57c0de',
-			'/sensedges/00000000-0031-0001-0000-00007e57c0de',
+			'/devices/00000000-0001-0001-0000-00007e57c0de/top',
+			'/devices/00000000-0031-0001-0000-00007e57c0de/top',
 		])
 		print(r)
 
 Development
 -------------
 
 Source code, issues, and pull requests are managed using `Github <https://github.com/Michsior14/python-kaiterra-async-client>`__.
```

### Comparing `kaiterra-async-client-1.0.1/README.rst` & `kaiterra-async-client-1.1.0/kaiterra_async_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: kaiterra-async-client
+Version: 1.1.0
+Summary: Kaiterra API Async Client
+Home-page: https://github.com/Michsior14/python-kaiterra-async-client
+License: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 python-kaiterra-async-client
 ============================
 
 Python 3 client for retrieving readings from your Laser Egg or Sensedge using the `Kaiterra REST API <https://dashboard.kaiterra.com>`__.
 
 To use it, you'll first need to create an account at the `Kaiterra Dashboard <https://dashboard.kaiterra.com>`__, then create an API key under Settings -> Profile -> Developer.
 
@@ -24,16 +41,16 @@
 
 	import aiohttp
 	from kaiterra_async_client import KaiterraAPIClient
 
 	async with aiohttp.ClientSession() as session:
 		client = KaiterraAPIClient(session, api_key='YOUR_API_KEY_HERE')
 		r = await client.get_latest_sensor_readings([
-			'/lasereggs/00000000-0001-0001-0000-00007e57c0de',
-			'/sensedges/00000000-0031-0001-0000-00007e57c0de',
+			'/devices/00000000-0001-0001-0000-00007e57c0de/top',
+			'/devices/00000000-0031-0001-0000-00007e57c0de/top',
 		])
 		print(r)
 
 Development
 -------------
 
 Source code, issues, and pull requests are managed using `Github <https://github.com/Michsior14/python-kaiterra-async-client>`__.
```

### Comparing `kaiterra-async-client-1.0.1/kaiterra_async_client/client.py` & `kaiterra-async-client-1.1.0/kaiterra_async_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 """
 Python client for the Kaiterra REST API.
 """
 
 import json
-import aiohttp
 from typing import List
 from enum import Enum
 from kaiterra_async_client import dateutil
 
 
 class AQIStandard(Enum):
     """
     Denotes a scale according to which air quality index should be calculated
     from pollutant readings.
     """
-    USA = 'us'
-    China = 'cn'
-    India = 'in'
+
+    USA = "us"
+    China = "cn"
+    India = "in"
 
     @staticmethod
     def from_str(s: str):
         for v in AQIStandard.__members__.values():
             if v.value == s:
                 return v
         raise ValueError("'{}' isn't a known value for AQIStandard".format(s))
 
 
 class Units(Enum):
     """
     Lists units in which sensor-reported values may be reported.  Use .value
     to return the short string representation of these enums.
     """
-    Unknown = '?'
-    Count = 'x'
-    Percent = '%'
-    DegreesCelsius = 'C'
-    DegreesFahrenheit = 'F'
-    MilligramsPerCubicMeter = 'mg/m³'
-    MicrogramsPerCubicMeter = 'µg/m³'
-    PartsPerMillion = 'ppm'
-    PartsPerBillion = 'ppb'
+
+    Unknown = "?"
+    Count = "x"
+    Percent = "%"
+    DegreesCelsius = "C"
+    DegreesFahrenheit = "F"
+    MilligramsPerCubicMeter = "mg/m³"
+    MicrogramsPerCubicMeter = "µg/m³"
+    PartsPerMillion = "ppm"
+    PartsPerBillion = "ppb"
 
     @staticmethod
     def from_str(s: str):
         for v in Units.__members__.values():
             if v.value == s:
                 return v
         raise ValueError("'{}' isn't a known value for Units".format(s))
@@ -64,24 +65,25 @@
     US EPA, Chinese MEP, or other given governing body.  The index returned is the Kaiterra
     Overall Index described at https://support.kaiterra.com/hc/en-us/articles/360016529993-What-is-the-Overall-Index-
     :param preferred_units: List of Units preferred by the client.  For instance,
     passing [Units.DegreesFahrenheit] will cause all temperature quantities to be reported
     in degrees Fahrenheit instead of the default, which is degrees Celsius.
     """
 
-    def __init__(self,
-                 session,
-                 base_url='https://api.kaiterra.com',
-                 api_key=None,
-                 hmac_secret=None,
-                 aqi_standard=None,
-                 preferred_units=None
-                 ):
+    def __init__(
+        self,
+        session,
+        base_url="https://api.kaiterra.com",
+        api_key=None,
+        hmac_secret=None,
+        aqi_standard=None,
+        preferred_units=None,
+    ):
         """Constructs a new KaiterraAPIClient object."""
-        self._base_url = base_url.rstrip('/')
+        self._base_url = base_url.rstrip("/")
         self._api_key = api_key
         self._hmac_secret = hmac_secret
         self._preferred_units = []
         self._aqi_standard = aqi_standard
         self._session = session
 
         if preferred_units is not None:
@@ -95,118 +97,133 @@
             raise ValueError("Must specify only one of api_key or hmac_secret")
 
     async def get_latest_sensor_readings(self, sensor_ids: List[str]) -> List[dict]:
         """
         Retrieves the latest sensor readings for the given sensors.
 
         :param sensor_ids: A list of sensor IDs whose data to return.  IDs must look like
+        /devices/993c6bda-ddc5-4187-a7ab-253f1c0df6eb/top for all types of devices, or
         /lasereggs/00000000-0001-0001-0000-00007e57c0de for Laser Eggs, or
-        /sensedges/00000000-0031-0001-0000-00007e57c0de for Sensedges.  The maximum
-        length of this list is 100.
+        /sensedges/00000000-0031-0001-0000-00007e57c0de for Sensedges. The maximum length
+        of this list is 100.
         :returns: a list of dictionaries containing sensor data, where the list has
         one element corresponding to each ID passed in sensor_ids.  Sensors that don't exist
         or have never reported any data will have values of None.  Otherwise, each dictionary's
         keys are the names of the measurement parameters ('pm25', 'pm10', 'humidity', etc.)
         and the values are themselves dictionaries with the following keys:
 
         - units: a Units enum showing the units in which the quantity is being reported
         - source: (optional) for Sensedges, this is the model of the sensor that captured
         the reading; e.g. 'km100', 'km102'
         - points: a list of one or more data points -- dictionaries -- with the following keys:
             - ts: a datetime object that is the time at which the quantity was measured
             - value: the numeric value of the reading
             - aqi: (optional) the air quality index of the reading, if applicable
         """
-        from urllib.parse import urlencode
-
         if isinstance(sensor_ids, str):
             raise ValueError("sensor_ids must be a list of strings")
 
         if len(sensor_ids) > 100:
             raise ValueError("sensor_ids is too long; max length is 100")
 
         requests = []
 
-        get_params = ['format=series_major']
+        get_params = ["format=series_major"]
         if self._aqi_standard is not None:
-            get_params.append('aqi=' + self._aqi_standard.value)
+            get_params.append("aqi=" + self._aqi_standard.value)
         for u in self._preferred_units:
-            get_params.append('units=' + u.value)
+            get_params.append("units=" + u.value)
 
         for sid in sensor_ids:
             if not self._is_valid_sensor_id(sid):
-                raise ValueError('sensor ID ' + sid + ' is invalid')
+                raise ValueError("sensor ID " + sid + " is invalid")
             req = {
-                'method': 'GET',
-                'relative_url': sid + "?" + '&'.join(get_params),
+                "method": "GET",
+                "relative_url": sid + "?" + "&".join(get_params),
             }
             requests.append(req)
 
         r = await self._do_request(
-            '/v1/batch',
-            headers={'Content-Type': 'application/json'},
-            json=requests)
+            "/v1/batch", headers={"Content-Type": "application/json"}, json=requests
+        )
 
         # Do some slight reformatting and parse dates
         return [self._parse_series_major_single_points(x) for x in r]
 
     def _parse_series_major_single_points(self, response: dict) -> dict:
         from collections.abc import Mapping
+
         if not isinstance(response, Mapping):
             return None
-        if response.get('code', 0) < 200 or response.get('code', 0) >= 400:
+        if response.get("code", 0) < 200 or response.get("code", 0) >= 400:
             return None
 
-        body = json.loads(response['body'])
-        params = body.get('latest', None)
+        body = json.loads(response["body"])
+
+        # New 'devices' endpoint returns 'data'
+        params = body.get("data", None)
+
+        # Old 'lasereggs/sensedges' endpoints returns 'latest'
         if not params:
-            params = body.get('info.aqi', None)
-            if not params:
-                return None
+            params = body.get("latest", None)
+
+        # or 'info.aqi'
+        if not params:
+            params = body.get("info.aqi", None)
+
+        if not params:
+            return None
 
         parsed = {}
         for param in params:
-            if len(param['points']) == 0:
+            if len(param["points"]) == 0:
                 continue
 
-            points = param['points']
+            points = param["points"]
             point = points[0]
-            point['ts'] = dateutil.parse_rfc3339(point['ts'])
+            point["ts"] = dateutil.parse_rfc3339(point["ts"])
             new_pt = {
-                'units': Units.from_str(param['units']),
+                "units": Units.from_str(param["units"]),
             }
-            if 'source' in param:
-                new_pt['source'] = param['source']
-            new_pt['points'] = [point]
+            if "source" in param:
+                new_pt["source"] = param["source"]
+            new_pt["points"] = [point]
 
-            parsed[param['param']] = new_pt
+            parsed[param["param"]] = new_pt
 
         return parsed
 
     async def _do_request(self, relative_url, *, params=None, headers=None, json=None):
         """
         Executes an HTTP GET/POST against the given resource.  The request is authorized
         using the credentials given to __init__.
         """
         params = params or {}
         headers = headers or {}
-        if 'key' in params:
-            raise ValueError("don't pass the 'key' parameter to individual requests; authorization is already handled by KaiterraAPIClient")
+        if "key" in params:
+            raise ValueError(
+                "don't pass the 'key' parameter to individual requests; authorization is already handled by KaiterraAPIClient"
+            )
 
         if self._api_key:
-            params['key'] = self._api_key
+            params["key"] = self._api_key
 
-        url = self._base_url + '/' + relative_url.lstrip('/')
-        async with self._session.post(url, params=params, headers=headers, json=json, raise_for_status=True) as r:
+        url = self._base_url + "/" + relative_url.lstrip("/")
+        async with self._session.post(
+            url, params=params, headers=headers, json=json, raise_for_status=True
+        ) as r:
             return await r.json()
 
     def _is_valid_sensor_id(self, sid: str) -> bool:
         """
         Ensures the given ID is a valid sensor ID.
         """
         import re
 
-        m = re.match(r'/?(lasereggs?|sensedges?)/([0-9a-f]{32}|[0-9a-f]{8}-?[0-9a-f]{4}-?[0-9a-f]{4}-?[0-9a-f]{4}-?[0-9a-f]{12})', sid.lower())
+        m = re.match(
+            r"/?(lasereggs?|sensedges?|devices?)/([0-9a-f]{32}|[0-9a-f]{8}-?[0-9a-f]{4}-?[0-9a-f]{4}-?[0-9a-f]{4}-?[0-9a-f]{12})",
+            sid.lower(),
+        )
         if not m:
             return False
 
         return True
```

### Comparing `kaiterra-async-client-1.0.1/setup.py` & `kaiterra-async-client-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 #!/usr/bin/env python3
 """Define the setup options."""
 import os
 import re
 import setuptools
 
-with open('README.rst', 'r') as f:
+with open("README.rst", "r") as f:
     readme = f.read()
 
 
 setuptools.setup(
-    name='kaiterra-async-client',
-    version='1.0.1',
+    name="kaiterra-async-client",
+    version="1.1.0",
     description="Kaiterra API Async Client",
     long_description=readme,
     long_description_content_type="text/x-rst",
-    url='https://github.com/Michsior14/python-kaiterra-async-client',
-    license='MIT License',
-    packages=setuptools.find_packages(exclude=['*.tests', '*.tests.*']),
-    test_suite='kaiterra_async_client.tests',
-    tests_require=[
-        'aioresponses',
-        'aiounittest'
-    ],
+    url="https://github.com/Michsior14/python-kaiterra-async-client",
+    license="MIT License",
+    packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*"]),
+    test_suite="kaiterra_async_client.tests",
+    tests_require=["aioresponses", "aiounittest"],
     install_requires=[
-        'aiohttp>=3.8.1',
+        "aiohttp>=3.8.1",
     ],
-    python_requires='>=3.5',
+    python_requires=">=3.5",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.5',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.5",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

