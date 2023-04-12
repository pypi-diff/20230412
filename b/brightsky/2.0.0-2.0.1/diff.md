# Comparing `tmp/brightsky-2.0.0.tar.gz` & `tmp/brightsky-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.0.tar", last modified: Wed Mar 29 09:36:14 2023, max compression
+gzip compressed data, was "brightsky-2.0.1.tar", last modified: Wed Apr 12 18:00:52 2023, max compression
```

## Comparing `brightsky-2.0.0.tar` & `brightsky-2.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:36:14.993481 brightsky-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-29 09:36:09.000000 brightsky-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-03-29 09:36:14.993481 brightsky-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-03-29 09:36:09.000000 brightsky-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:36:14.989481 brightsky-2.0.0/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-29 09:36:09.000000 brightsky-2.0.0/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:36:14.993481 brightsky-2.0.0/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-03-29 09:36:14.000000 brightsky-2.0.0/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-29 09:36:14.000000 brightsky-2.0.0/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:36:14.000000 brightsky-2.0.0/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-29 09:36:14.000000 brightsky-2.0.0/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 09:36:14.000000 brightsky-2.0.0/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-29 09:36:09.000000 brightsky-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:36:14.993481 brightsky-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-29 09:36:09.000000 brightsky-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:36:14.993481 brightsky-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-03-29 09:36:09.000000 brightsky-2.0.0/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.467195 brightsky-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 18:00:48.000000 brightsky-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-12 18:00:52.467195 brightsky-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-12 18:00:48.000000 brightsky-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.463195 brightsky-2.0.1/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.463195 brightsky-2.0.1/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 18:00:48.000000 brightsky-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:00:52.467195 brightsky-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 18:00:48.000000 brightsky-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.467195 brightsky-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_web.py
```

### Comparing `brightsky-2.0.0/LICENSE` & `brightsky-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/PKG-INFO` & `brightsky-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.0
+Version: 2.0.1
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.0/README.md` & `brightsky-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/cli.py` & `brightsky-2.0.1/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/db.py` & `brightsky-2.0.1/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/export.py` & `brightsky-2.0.1/brightsky/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         'condition',
         'dew_point',
         'precipitation',
         'precipitation_probability',
         'precipitation_probability_6h',
         'pressure_msl',
         'relative_humidity',
+        'solar',
         'sunshine',
         'temperature',
         'visibility',
         'wind_direction',
         'wind_speed',
         'wind_gust_direction',
         'wind_gust_speed',
@@ -190,22 +191,43 @@
     WEATHER_TABLE = 'synop'
     UPDATE_WEATHER_CONFLICT_UPDATE = (
         '{field} = COALESCE(EXCLUDED.{field}, {weather_table}.{field})')
     UPDATE_WEATHER_CLEANUP = (
         'REFRESH MATERIALIZED VIEW CONCURRENTLY current_weather')
 
     ELEMENT_FIELDS = [
-        'cloud_cover', 'condition', 'dew_point', 'precipitation_10',
-        'precipitation_30', 'precipitation_60', 'pressure_msl',
-        'relative_humidity', 'sunshine_10', 'sunshine_30', 'sunshine_60',
-        'temperature', 'visibility', 'wind_direction_10', 'wind_direction_30',
-        'wind_direction_60', 'wind_speed_10', 'wind_speed_30', 'wind_speed_60',
-        'wind_gust_direction_10', 'wind_gust_direction_30',
-        'wind_gust_direction_60', 'wind_gust_speed_10', 'wind_gust_speed_30',
-        'wind_gust_speed_60']
+        'cloud_cover',
+        'condition',
+        'dew_point',
+        'precipitation_10',
+        'precipitation_30',
+        'precipitation_60',
+        'pressure_msl',
+        'relative_humidity',
+        'solar_10',
+        'solar_30',
+        'solar_60',
+        'sunshine_10',
+        'sunshine_30',
+        'sunshine_60',
+        'temperature',
+        'visibility',
+        'wind_direction_10',
+        'wind_direction_30',
+        'wind_direction_60',
+        'wind_speed_10',
+        'wind_speed_30',
+        'wind_speed_60',
+        'wind_gust_direction_10',
+        'wind_gust_direction_30',
+        'wind_gust_direction_60',
+        'wind_gust_speed_10',
+        'wind_gust_speed_30',
+        'wind_gust_speed_60',
+    ]
 
     synop_update_lock = Lock()
 
     def prepare_records(self, records):
         # Merge records for same source and timestamp (otherwise we will run
         # into trouble with our ON CONFLICT DO UPDATE as we cannot touch the
         # same row twice in the same command).
```

### Comparing `brightsky-2.0.0/brightsky/parsers.py` & `brightsky-2.0.1/brightsky/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,14 +124,21 @@
 class PrecipitationObservationsParser(
     ObservationsBrightSkyMixin,
     dwdparse.parsers.PrecipitationObservationsParser,
 ):
     pass
 
 
+class SolarRadiationObservationsParser(
+    ObservationsBrightSkyMixin,
+    dwdparse.parsers.SolarRadiationObservationsParser,
+):
+    pass
+
+
 class VisibilityObservationsParser(
     ObservationsBrightSkyMixin,
     dwdparse.parsers.VisibilityObservationsParser,
 ):
     pass
 
 
@@ -173,11 +180,12 @@
         'stundenwerte_P0_': PressureObservationsParser,
         'stundenwerte_RR_': PrecipitationObservationsParser,
         'stundenwerte_SD_': SunshineObservationsParser,
         'stundenwerte_TD_': DewPointObservationsParser,
         'stundenwerte_TU_': TemperatureObservationsParser,
         'stundenwerte_VV_': VisibilityObservationsParser,
         '10minutenwerte_extrema_wind_': WindGustsObservationsParser,
+        '10minutenwerte_SOLAR_': SolarRadiationObservationsParser,
     }
     for pattern, parser in parsers.items():
         if re.match(pattern, filename):
             return parser
```

### Comparing `brightsky-2.0.0/brightsky/polling.py` & `brightsky-2.0.1/brightsky/polling.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         'https://opendata.dwd.de/climate_environment/CDC/observations_germany/'
         f'climate/hourly/{subfolder}/'
         for subfolder in [
             'air_temperature', 'cloudiness', 'dew_point', 'visibility',
             'precipitation', 'pressure', 'sun', 'wind']
     ] + [
         'https://opendata.dwd.de/climate_environment/CDC/observations_germany/'
-        f'climate/10_minutes/extreme_wind/{subfolder}/'
+        f'climate/10_minutes/{param}/{subfolder}/'
+        for param in ['extreme_wind', 'solar']
         for subfolder in ['recent', 'historical']
     ]
 
     @property
     def logger(self):
         if not hasattr(self, '_logger'):
             self._logger = logging.getLogger(self.__class__.__name__)
```

### Comparing `brightsky-2.0.0/brightsky/query.py` & `brightsky-2.0.1/brightsky/query.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/settings.py` & `brightsky-2.0.1/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/tasks.py` & `brightsky-2.0.1/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/utils.py` & `brightsky-2.0.1/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/web.py` & `brightsky-2.0.1/brightsky/web.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky/worker.py` & `brightsky-2.0.1/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/brightsky.egg-info/PKG-INFO` & `brightsky-2.0.1/brightsky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.0
+Version: 2.0.1
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.0/brightsky.egg-info/SOURCES.txt` & `brightsky-2.0.1/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/setup.py` & `brightsky-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/tests/test_export.py` & `brightsky-2.0.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/tests/test_parsers.py` & `brightsky-2.0.1/tests/test_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         'sunshine': None,
         'temperature': 260.45,
         'visibility': 1700.0,
         'wind_direction': 330.0,
         'wind_speed': 8.75,
         'wind_gust_speed': None,
         'condition': 'snow',
+        'solar': None,
     }
     assert records[-1] == {
         'observation_type': 'forecast',
         'source': 'MOSMIX:2020-03-13T09:00:00.000Z',
         'lat': 74.52,
         'lon': 19.02,
         'height': 16.,
@@ -58,14 +59,15 @@
         'sunshine': None,
         'temperature': 267.15,
         'visibility': 11600.0,
         'wind_direction': 49.0,
         'wind_speed': 7.72,
         'wind_gust_speed': None,
         'condition': 'dry',
+        'solar': None,
     }
     assert records[2]['precipitation_probability_6h'] == 49
 
 
 def test_synop_parser(data_dir):
     p = SYNOPParser()
     records = list(p.parse(data_dir / 'synop.json.bz2'))
@@ -137,14 +139,15 @@
         'sunshine': None,
         'temperature': 270.05,
         'visibility': None,
         'wind_direction': 140,
         'wind_speed': 3.9,
         'wind_gust_speed': 5.8,
         'condition': None,
+        'solar': None,
     }
     assert records[15] == {
         'observation_type': 'current',
         'lat': 10.1,
         'lon': 20.2,
         'height': 30.3,
         'dwd_station_id': 'YYY',
@@ -159,14 +162,15 @@
         'sunshine': None,
         'temperature': 270.95,
         'visibility': None,
         'wind_direction': 230,
         'wind_speed': 3.9,
         'wind_gust_speed': 7.2,
         'condition': None,
+        'solar': None,
     }
 
 
 def test_current_observation_parser_loads_station_data_from_db(db, data_dir):
     source = {
         'observation_type': 'forecast',
         'lat': 52.12,
```

### Comparing `brightsky-2.0.0/tests/test_polling.py` & `brightsky-2.0.1/tests/test_polling.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
             'CurrentObservationsParser', '2020-04-06 10:38', 7343),
         '/dir/10minutenwerte_extrema_wind_01766_now.zip': (
             'WindGustsObservationsParser', '2020-06-08 09:12', 701),
         '/dir/10minutenwerte_extrema_wind_01766_akt.zip': (
             'WindGustsObservationsParser', '2020-06-08 04:27', 519692),
         '/dir/10minutenwerte_extrema_wind_01766_20100101_20191231_hist.zip': (
             'WindGustsObservationsParser', '2020-04-09 09:16', 3661729),
+        '/dir/10minutenwerte_SOLAR_01766_akt.zip': (
+            'SolarRadiationObservationsParser', '2023-04-12 00:50', 367557),
     }
     assert list(DWDPoller().parse('/dir/', resp_text)) == [
         {
             'url': k,
             'parser': v[0],
             'last_modified': datetime.datetime.strptime(
                 v[1], '%Y-%m-%d %H:%M').replace(tzinfo=tzutc()),
```

### Comparing `brightsky-2.0.0/tests/test_settings.py` & `brightsky-2.0.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/tests/test_tasks.py` & `brightsky-2.0.1/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/tests/test_utils.py` & `brightsky-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.0/tests/test_web.py` & `brightsky-2.0.1/tests/test_web.py`

 * *Files identical despite different names*

