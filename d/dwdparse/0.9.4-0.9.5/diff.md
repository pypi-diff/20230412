# Comparing `tmp/dwdparse-0.9.4.tar.gz` & `tmp/dwdparse-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwdparse-0.9.4.tar", last modified: Wed Mar 29 09:24:15 2023, max compression
+gzip compressed data, was "dwdparse-0.9.5.tar", last modified: Wed Apr 12 17:51:02 2023, max compression
```

## Comparing `dwdparse-0.9.4.tar` & `dwdparse-0.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:15.165382 dwdparse-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-29 09:24:07.000000 dwdparse-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-03-29 09:24:15.161382 dwdparse-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-29 09:24:07.000000 dwdparse-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:15.161382 dwdparse-0.9.4/dwdparse/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    25948 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-29 09:24:07.000000 dwdparse-0.9.4/dwdparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:15.161382 dwdparse-0.9.4/dwdparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-03-29 09:24:15.000000 dwdparse-0.9.4/dwdparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-29 09:24:15.000000 dwdparse-0.9.4/dwdparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:24:15.000000 dwdparse-0.9.4/dwdparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-29 09:24:15.000000 dwdparse-0.9.4/dwdparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 09:24:15.000000 dwdparse-0.9.4/dwdparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 09:24:15.000000 dwdparse-0.9.4/dwdparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-29 09:24:07.000000 dwdparse-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:24:15.165382 dwdparse-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-29 09:24:07.000000 dwdparse-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:15.161382 dwdparse-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-03-29 09:24:07.000000 dwdparse-0.9.4/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-29 09:24:07.000000 dwdparse-0.9.4/tests/test_stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-29 09:24:07.000000 dwdparse-0.9.4/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 17:50:54.000000 dwdparse-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-12 17:51:02.405815 dwdparse-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-12 17:50:54.000000 dwdparse-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/dwdparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/dwdparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 17:50:54.000000 dwdparse-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:51:02.405815 dwdparse-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-12 17:50:54.000000 dwdparse-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-04-12 17:50:54.000000 dwdparse-0.9.5/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-12 17:50:54.000000 dwdparse-0.9.5/tests/test_stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 17:50:54.000000 dwdparse-0.9.5/tests/test_units.py
```

### Comparing `dwdparse-0.9.4/LICENSE` & `dwdparse-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.4/PKG-INFO` & `dwdparse-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.4
+Version: 0.9.5
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.4 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.5 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: lean License-File:
 LICENSE # dwdparse [![Build Status](https://img.shields.io/github/actions/
```

### Comparing `dwdparse-0.9.4/README.md` & `dwdparse-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.4/dwdparse/api.py` & `dwdparse-0.9.5/dwdparse/api.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.4/dwdparse/cli.py` & `dwdparse-0.9.5/dwdparse/cli.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.4/dwdparse/parsers.py` & `dwdparse-0.9.5/dwdparse/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,23 @@
     wmo_id_to_dwd,
 )
 from dwdparse.units import (
     celsius_to_kelvin,
     current_observations_weather_code_to_condition,
     eighths_to_percent,
     hpa_to_pa,
+    j_per_cm2_to_j_per_m2,
+    kj_per_m2_to_j_per_m2,
     km_to_m,
     kmh_to_ms,
     minutes_to_seconds,
     synop_current_weather_code_to_condition,
     synop_form_of_precipitation_code_to_condition,
     synop_past_weather_code_to_condition,
+    w_per_m2_to_hourly_j_per_m2,
 )
 
 
 class SkipRecord(Exception):
     pass
 
 
@@ -54,14 +57,15 @@
         'DD': 'wind_direction',
         'FF': 'wind_speed',
         'FX1': 'wind_gust_speed',
         'N': 'cloud_cover',
         'PPPP': 'pressure_msl',
         'R101': 'precipitation_probability',
         'R602': 'precipitation_probability_6h',
+        'Rad1h': 'solar',
         'RR1c': 'precipitation',
         'SunD1': 'sunshine',
         'Td': 'dew_point',
         'TTT': 'temperature',
         'VV': 'visibility',
         'ww': 'condition',
     }
@@ -160,14 +164,17 @@
         except ValueError:
             return None
 
     def parse_condition(self, value):
         code = int(value.split('.')[0])
         return synop_current_weather_code_to_condition(code)
 
+    def parse_solar(self, value):
+        return kj_per_m2_to_j_per_m2(float(value))
+
     def sanitize_records(self, records):
         for r in records:
             if r['precipitation'] and r['precipitation'] < 0:
                 self.logger.warning(
                     "Ignoring negative precipitation value: %s", r)
                 r['precipitation'] = None
             if r['wind_direction'] and r['wind_direction'] > 360:
@@ -197,14 +204,15 @@
         'airTemperature': 'temperature',
         'dewpointTemperature': 'dew_point',
         'relativeHumidity': 'relative_humidity',
     }
     time_period_field = 'timePeriod'
     time_periods = (-10, -30, -60)
     time_period_elements = {
+        'globalSolarRadiationIntegratedOverPeriodSpecified': 'solar',
         'windDirection': 'wind_direction',
         'windSpeed': 'wind_speed',
         'maximumWindGustDirection': 'wind_gust_direction',
         'maximumWindGustSpeed': 'wind_gust_speed',
         'totalPrecipitationOrTotalWaterEquivalent': 'precipitation',
         'totalSunshine': 'sunshine',
     }
@@ -249,15 +257,15 @@
                 data[key] = value
                 if field := self.elements.get(key):
                     record[field] = value
                 elif field := self.height_elements.get(key):
                     if data[self.height_field] == self.height:
                         record[field] = value
                 elif field := self.time_period_elements.get(key):
-                    time_period = data[self.time_period_field]
+                    time_period = data.get(self.time_period_field, -10)
                     if time_period in self.time_periods:
                         if field == 'sunshine' and value:
                             value *= 60
                         record[field + f'_{-time_period}'] = value
                 elif parse_method := getattr(self, f'parse_{key}', None):
                     parse_method(record, data, value)
             else:
@@ -302,14 +310,15 @@
 
 class CurrentObservationsParser(Parser):
 
     ELEMENTS = {
         'cloud_cover_total': 'cloud_cover',
         'dew_point_temperature_at_2_meter_above_ground': 'dew_point',
         'dry_bulb_temperature_at_2_meter_above_ground': 'temperature',
+        'global_radiation_last_hour': 'solar',
         'horizontal_visibility': 'visibility',
         'maximum_wind_speed_last_hour': 'wind_gust_speed',
         'mean_wind_direction_during_last_10 min_at_10_meters_above_ground': (
             'wind_direction'),
         'mean_wind_speed_during last_10_min_at_10_meters_above_ground': (
             'wind_speed'),
         'precipitation_amount_last_hour': 'precipitation',
@@ -321,14 +330,15 @@
     DATE_COLUMN = 'surface observations'
     HOUR_COLUMN = 'Parameter description'
 
     CONVERTERS = {
         'condition': current_observations_weather_code_to_condition,
         'dew_point': celsius_to_kelvin,
         'pressure_msl': hpa_to_pa,
+        'solar': w_per_m2_to_hourly_j_per_m2,
         'sunshine': minutes_to_seconds,
         'temperature': celsius_to_kelvin,
         'visibility': km_to_m,
         'wind_speed': kmh_to_ms,
         'wind_gust_speed': kmh_to_ms,
     }
 
@@ -491,14 +501,73 @@
                 elements[element] = converter(elements[element])
         return elements
 
     def skip_timestamp(self, timestamp):
         return False
 
 
+class TenMinutesObservationsParser(ObservationsParser):
+
+    META_DATA_URL = None
+    TRIGGER_MINUTE = 0
+
+    def get_extra_urls(self, path):
+        with zipfile.ZipFile(path) as zf:
+            dwd_station_id = self.parse_station_id(zf)
+        return {
+            'meta_path': self.META_DATA_URL.format(
+                dwd_station_id=dwd_station_id,
+            ),
+        }
+
+    def parse_station_id(self, zf, **extra):
+        for filename in zf.namelist():
+            if (m := re.match(r'produkt_.*_(\d+)\.txt', filename)):
+                return m.group(1)
+        raise ValueError(f"Unable to parse station ID for {self.path}")
+
+    def parse_lat_lon_history(self, zf, dwd_station_id, **extra):
+        if 'meta_path' not in extra:
+            raise ValueError(
+                f"Must supply a `meta_path` keyword argument for "
+                f"{self.__class__.__name__}",
+            )
+        with zipfile.ZipFile(extra['meta_path']) as meta_zf:
+            return super().parse_lat_lon_history(meta_zf, dwd_station_id)
+
+    def parse_reader(self, filename, reader, lat_lon_history):
+        hour_values = []
+        for row in reader:
+            timestamp = datetime.datetime.strptime(
+                row['MESS_DATUM'],
+                '%Y%m%d%H%M',
+            ).replace(
+                tzinfo=datetime.timezone.utc,
+            )
+            if self.skip_timestamp(timestamp + datetime.timedelta(minutes=50)):
+                continue
+            # XXX: Station parameters are currently not supported for
+            #      10-minute parsers
+            hour_values.append(self.parse_elements(row, None, None, None))
+            if timestamp.minute == self.TRIGGER_MINUTE:
+                if self.TRIGGER_MINUTE > 30:
+                    # Likely triggered at :50, round to next full hour
+                    timestamp += datetime.timedelta(
+                        minutes=60 - self.TRIGGER_MINUTE,
+                    )
+                elif self.TRIGGER_MINUTE:
+                    timestamp = timestamp.replace(minute=0)
+                yield self._make_record(
+                    timestamp, hour_values, filename, lat_lon_history)
+                hour_values.clear()
+
+    def _make_record(self, timestamp, hour_values, filename, lat_lon_history):
+        raise NotImplementedError
+
+
 class CloudCoverObservationsParser(ObservationsParser):
 
     elements = {
         'cloud_cover': ' V_N',
     }
     ignored_values = {
         'cloud_cover': ['-1', '9'],
@@ -594,74 +663,30 @@
         'wind_direction': int,
     }
     ignored_values = {
         'wind_direction': ['990'],
     }
 
 
-class WindGustsObservationsParser(ObservationsParser):
+class WindGustsObservationsParser(TenMinutesObservationsParser):
 
     META_DATA_URL = (
         'https://opendata.dwd.de/climate_environment/CDC/observations_germany/'
         'climate/10_minutes/extreme_wind/meta_data/'
         'Meta_Daten_zehn_min_fx_{dwd_station_id}.zip')
 
     elements = {
         'wind_gust_direction': 'DX_10',
         'wind_gust_speed': 'FX_10',
     }
 
-    def get_extra_urls(self, path):
-        with zipfile.ZipFile(path) as zf:
-            dwd_station_id = self.parse_station_id(zf)
-        return {
-            'meta_path': self.META_DATA_URL.format(
-                dwd_station_id=dwd_station_id,
-            ),
-        }
-
-    def parse_station_id(self, zf, **extra):
-        for filename in zf.namelist():
-            if (m := re.match(r'produkt_.*_(\d+)\.txt', filename)):
-                return m.group(1)
-        raise ValueError(f"Unable to parse station ID for {self.path}")
-
-    def parse_lat_lon_history(self, zf, dwd_station_id, **extra):
-        if 'meta_path' not in extra:
-            raise ValueError(
-                "Must supply a `meta_path` keyword argument for "
-                "WindGustObservationsParser",
-            )
-        with zipfile.ZipFile(extra['meta_path']) as meta_zf:
-            return super().parse_lat_lon_history(meta_zf, dwd_station_id)
-
-    def parse_reader(self, filename, reader, lat_lon_history):
-        hour_values = []
-        for row in reader:
-            timestamp = datetime.datetime.strptime(
-                row['MESS_DATUM'],
-                '%Y%m%d%H%M',
-            ).replace(
-                tzinfo=datetime.timezone.utc,
-            )
-            if self.skip_timestamp(timestamp + datetime.timedelta(hours=1)):
-                continue
-            # Should this be refactored into a base class we will need to
-            # properly parse the station parameters and pass them
-            values = self.parse_elements(row, None, None, None)
-            if values['wind_gust_speed']:
-                hour_values.append(values)
-            if timestamp.minute == 0:
-                yield self._make_record(
-                    timestamp, hour_values, filename, lat_lon_history)
-                hour_values.clear()
-
     def _make_record(self, timestamp, hour_values, filename, lat_lon_history):
         lat, lon, height, station_name = self._station_params(
             timestamp, lat_lon_history)
+        hour_values = [x for x in hour_values if x['wind_gust_speed']]
         if hour_values:
             max_value = max(hour_values, key=lambda v: v['wind_gust_speed'])
             direction = max_value['wind_gust_direction']
             speed = max_value['wind_gust_speed']
         else:
             direction = None
             speed = None
@@ -709,25 +734,63 @@
                 elements['pressure_station']
                 * (1 - .0065 * height / 288.15) ** -5.255,
                 -1))
         del elements['pressure_station']
         return elements
 
 
+class SolarRadiationObservationsParser(TenMinutesObservationsParser):
+
+    META_DATA_URL = (
+        'https://opendata.dwd.de/climate_environment/CDC/observations_germany/'
+        'climate/10_minutes/solar/meta_data/'
+        'Meta_Daten_zehn_min_sd_{dwd_station_id}.zip')
+
+    # It seems that the measurement rows contain the global irradiance for the
+    # NEXT ten minutes -- at least then the values align with
+    # "global_radiation_last_hour" from the current observations
+    TRIGGER_MINUTE = 50
+
+    elements = {
+        'solar': 'GS_10',
+    }
+    converters = {
+        'solar': j_per_cm2_to_j_per_m2,
+    }
+
+    def _make_record(self, timestamp, hour_values, filename, lat_lon_history):
+        lat, lon, height, station_name = self._station_params(
+            timestamp, lat_lon_history)
+        solar = None
+        for values in hour_values:
+            if values['solar'] is not None:
+                solar = (solar or 0) + values['solar']
+        return {
+            'source': f'Observations:Recent:{filename}',
+            'lat': lat,
+            'lon': lon,
+            'height': height,
+            'station_name': station_name,
+            'timestamp': timestamp,
+            'solar': solar,
+        }
+
+
 def get_parser(filename):
     parsers = {
         r'MOSMIX_(S|L)_LATEST(_240)?\.kmz$': MOSMIXParser,
         r'Z__C_EDZW_\d+_.*\.json\.bz2$': SYNOPParser,
         r'\w{5}-BEOB\.csv$': CurrentObservationsParser,
         'stundenwerte_FF_': WindObservationsParser,
         'stundenwerte_N_': CloudCoverObservationsParser,
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

### Comparing `dwdparse-0.9.4/dwdparse/stations.py` & `dwdparse-0.9.5/dwdparse/stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.4/dwdparse/units.py` & `dwdparse-0.9.5/dwdparse/units.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,26 @@
     return int(pressure * 100)
 
 
 def kelvin_to_celsius(temperature):
     return round(temperature - 273.15, 2)
 
 
+def j_per_cm2_to_j_per_m2(solar):
+    return solar * 10000
+
+
+def j_per_m2_to_kwh_per_m2(solar):
+    return round(solar / 3600000, 3)
+
+
+def kj_per_m2_to_j_per_m2(solar):
+    return solar * 1000
+
+
 def km_to_m(distance):
     return distance * 1000
 
 
 def kmh_to_ms(speed):
     return round(speed / 3.6, 1)
 
@@ -34,14 +46,18 @@
     return pressure / 100
 
 
 def seconds_to_minutes(duration):
     return duration / 60
 
 
+def w_per_m2_to_hourly_j_per_m2(solar):
+    return solar * 3600
+
+
 # XXX: Subsequent codes with the same mapping are left out. I.e. all codes from
 #      0 through 16 map to 'dry', etc.
 SYNOP_CURRENT_CONDITION_MAP = {
     0: 'dry',
     17: 'thunderstorm',
     18: 'dry',
     40: 'fog',
@@ -155,14 +171,18 @@
     return _find(CURRENT_OBSERVATIONS_CONDITION_MAP, code)
 
 
 CONVERTERS = {
     'dwd': {
         'dew_point': kelvin_to_celsius,
         'pressure_msl': pa_to_hpa,
+        'solar': j_per_m2_to_kwh_per_m2,
+        'solar_10': j_per_m2_to_kwh_per_m2,
+        'solar_30': j_per_m2_to_kwh_per_m2,
+        'solar_60': j_per_m2_to_kwh_per_m2,
         'sunshine': seconds_to_minutes,
         'sunshine_10': seconds_to_minutes,
         'sunshine_30': seconds_to_minutes,
         'sunshine_60': seconds_to_minutes,
         'temperature': kelvin_to_celsius,
         'wind_speed': ms_to_kmh,
         'wind_speed_10': ms_to_kmh,
```

### Comparing `dwdparse-0.9.4/dwdparse.egg-info/PKG-INFO` & `dwdparse-0.9.5/dwdparse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.4
+Version: 0.9.5
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.4 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.5 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: lean License-File:
 LICENSE # dwdparse [![Build Status](https://img.shields.io/github/actions/
```

### Comparing `dwdparse-0.9.4/setup.py` & `dwdparse-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.4/tests/test_parsers.py` & `dwdparse-0.9.5/tests/test_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,79 +3,85 @@
 from dwdparse.parsers import (
     CloudCoverObservationsParser,
     CurrentObservationsParser,
     DewPointObservationsParser,
     MOSMIXParser,
     PrecipitationObservationsParser,
     PressureObservationsParser,
+    SolarRadiationObservationsParser,
     SunshineObservationsParser,
     SYNOPParser,
     TemperatureObservationsParser,
+    TenMinutesObservationsParser,
     VisibilityObservationsParser,
     WindGustsObservationsParser,
     WindObservationsParser,
     get_parser,
 )
 
 from .utils import is_subset
 
 
 utc = datetime.timezone.utc
 
 
-def test_mosmix_s_parser(data_dir):
-    records = list(MOSMIXParser().parse(data_dir / 'MOSMIX_S.kmz'))
-    assert len(records) == 240
+def test_mosmix_parser(data_dir):
+    records = list(MOSMIXParser().parse(data_dir / 'MOSMIX_L_LATEST.kmz'))
+    assert len(records) == 247
     assert records[0] == {
         'observation_type': 'forecast',
-        'source': 'MOSMIX:2020-03-13T09:00:00.000Z',
-        'lat': 74.52,
-        'lon': 19.02,
-        'height': 16.,
+        'source': 'MOSMIX:2023-04-12T09:00:00.000Z',
+        'lat': 51.97,
+        'lon': 7.63,
+        'height': 60.,
         'dwd_station_id': 'XXX',
-        'wmo_station_id': '01028',
-        'station_name': 'BJORNOYA',
-        'timestamp': datetime.datetime(2020, 3, 13, 10, 0, tzinfo=utc),
-        'cloud_cover': 93.0,
-        'dew_point': 257.25,
-        'precipitation': 0.1,
+        'wmo_station_id': 'P0036',
+        'station_name': 'MUENSTER ZENTRUM',
+        'timestamp': datetime.datetime(2023, 4, 12, 10, 0, tzinfo=utc),
+        'cloud_cover': 100.0,
+        'dew_point': 279.05,
+        'precipitation': 1.2,
+        'precipitation_probability': 75.,
         'precipitation_probability_6h': None,
-        'pressure_msl': 99000.0,
-        'sunshine': None,
-        'temperature': 260.45,
-        'visibility': 1700.0,
-        'wind_direction': 330.0,
-        'wind_speed': 8.75,
-        'wind_gust_speed': None,
-        'condition': 'snow',
+        'pressure_msl': 99700.0,
+        'sunshine': 0.0,
+        'temperature': 282.75,
+        'visibility': 14900.0,
+        'wind_direction': 179.0,
+        'wind_speed': 5.14,
+        'wind_gust_speed': 9.26,
+        'condition': 'rain',
+        'solar': 510000.0,
     }
     assert records[-1] == {
         'observation_type': 'forecast',
-        'source': 'MOSMIX:2020-03-13T09:00:00.000Z',
-        'lat': 74.52,
-        'lon': 19.02,
-        'height': 16.,
+        'source': 'MOSMIX:2023-04-12T09:00:00.000Z',
+        'lat': 51.97,
+        'lon': 7.63,
+        'height': 60.,
         'dwd_station_id': 'XXX',
-        'wmo_station_id': '01028',
-        'station_name': 'BJORNOYA',
-        'timestamp': datetime.datetime(2020, 3, 23, 9, 0, tzinfo=utc),
-        'cloud_cover': 76.,
-        'dew_point': 265.35,
-        'precipitation': None,
+        'wmo_station_id': 'P0036',
+        'station_name': 'MUENSTER ZENTRUM',
+        'timestamp': datetime.datetime(2023, 4, 22, 16, 0, tzinfo=utc),
+        'cloud_cover': 58.,
+        'dew_point': 277.85,
+        'precipitation': 0.0,
+        'precipitation_probability': 9.0,
         'precipitation_probability_6h': None,
-        'pressure_msl': 100630.0,
-        'sunshine': None,
-        'temperature': 267.15,
-        'visibility': 11600.0,
-        'wind_direction': 49.0,
-        'wind_speed': 7.72,
-        'wind_gust_speed': None,
-        'condition': 'dry',
+        'pressure_msl': 101790.0,
+        'sunshine': 2100.0,
+        'temperature': 290.85,
+        'visibility': 24900.0,
+        'wind_direction': 35.0,
+        'wind_speed': 3.6,
+        'wind_gust_speed': 7.72,
+        'condition': None,
+        'solar': 1170000.0,
     }
-    assert records[2]['precipitation_probability_6h'] == 49
+    assert records[2]['precipitation_probability_6h'] == 85.0
 
 
 def test_synop_parser(data_dir):
     records = list(SYNOPParser().parse(data_dir / 'synop.json.bz2'))
     assert len(records) == 3
     assert records[0] == {
         'observation_type': 'synop',
@@ -121,65 +127,67 @@
     assert records[2]['wmo_station_id'] == 'M031'
     assert records[2]['dwd_station_id'] == '05484'
 
 
 def test_current_observation_parser(data_dir):
     records = list(
         CurrentObservationsParser().parse(
-            data_dir / 'observations_current.csv',
+            data_dir / '10315-BEOB.csv',
             10.1,
             20.2,
             30.3,
             'Muenster',
         )
     )
     assert len(records) == 25
     assert records[0] == {
         'observation_type': 'current',
         'lat': 10.1,
         'lon': 20.2,
         'height': 30.3,
-        'dwd_station_id': 'YYY',
-        'wmo_station_id': '01049',
+        'dwd_station_id': '01766',
+        'wmo_station_id': '10315',
         'station_name': 'Muenster',
-        'timestamp': datetime.datetime(2020, 4, 6, 8, 0, tzinfo=utc),
-        'cloud_cover': None,
-        'dew_point': 263.15,
-        'precipitation': 0,
-        'pressure_msl': 102310.,
-        'relative_humidity': 59.,
-        'sunshine': None,
-        'temperature': 270.05,
-        'visibility': None,
-        'wind_direction': 140,
-        'wind_speed': 3.9,
-        'wind_gust_speed': 5.8,
-        'condition': None,
+        'timestamp': datetime.datetime(2023, 4, 12, 11, 0, tzinfo=utc),
+        'cloud_cover': 100.0,
+        'dew_point': 281.45,
+        'precipitation': 2.1,
+        'pressure_msl': 99780,
+        'relative_humidity': 94.,
+        'sunshine': 0,
+        'temperature': 282.35,
+        'visibility': 7900.0,
+        'wind_direction': 180.0,
+        'wind_speed': 2.2,
+        'wind_gust_speed': 4.7,
+        'condition': 'rain',
+        'solar': 291600.0,
     }
     assert records[15] == {
         'observation_type': 'current',
         'lat': 10.1,
         'lon': 20.2,
         'height': 30.3,
-        'dwd_station_id': 'YYY',
-        'wmo_station_id': '01049',
+        'dwd_station_id': '01766',
+        'wmo_station_id': '10315',
         'station_name': 'Muenster',
-        'timestamp': datetime.datetime(2020, 4, 5, 17, 0, tzinfo=utc),
-        'cloud_cover': None,
-        'dew_point': 270.05,
-        'precipitation': 0.6,
-        'pressure_msl': 101910.,
-        'relative_humidity': 94.,
-        'sunshine': None,
-        'temperature': 270.95,
-        'visibility': None,
-        'wind_direction': 230,
-        'wind_speed': 3.9,
-        'wind_gust_speed': 7.2,
-        'condition': None,
+        'timestamp': datetime.datetime(2023, 4, 11, 20, 0, tzinfo=utc),
+        'cloud_cover': 63.0,
+        'dew_point': 273.65,
+        'precipitation': 0.0,
+        'pressure_msl': 101170,
+        'relative_humidity': 67.0,
+        'sunshine': 0,
+        'temperature': 279.35,
+        'visibility': 49400.0,
+        'wind_direction': 140.0,
+        'wind_speed': 1.9,
+        'wind_gust_speed': 2.2,
+        'condition': 'dry',
+        'solar': 0.0,
     }
 
 
 def test_observations_parser_parses_metadata(data_dir):
     p = WindObservationsParser()
     metadata = {
         'observation_type': 'historical',
@@ -228,14 +236,26 @@
     assert len(records) == 10
     p.skip_timestamp = lambda ts: ts.year != 2019
     records = list(p.parse(data_dir / 'observations_recent_FF_akt.zip'))
     assert len(records) == 1
     assert records[0]['timestamp'].year == 2019
 
 
+def test_ten_minutes_observations_parser_extra_urls(data_dir):
+    class TestParser(TenMinutesObservationsParser):
+        META_DATA_URL = 'test_{dwd_station_id}.zip'
+
+    parser = TestParser()
+    path = data_dir / 'observations_recent_extrema_wind_akt.zip'
+    expected_meta_url = 'test_01766.zip'
+    assert parser.get_extra_urls(path) == {
+        'meta_path': expected_meta_url,
+    }
+
+
 def _test_parser(
         cls, path, first, last, count=10, first_idx=0, last_idx=-1, **kwargs):
     p = cls()
     records = list(p.parse(path, **kwargs))
     first['timestamp'] = datetime.datetime.strptime(
         first['timestamp'], '%Y-%m-%d %H:%M').replace(tzinfo=utc)
     last['timestamp'] = datetime.datetime.strptime(
@@ -343,27 +363,14 @@
          'wind_gust_speed': 6.3, 'wind_gust_direction': 210},
         {'timestamp': '2020-06-04 23:00',
          'wind_gust_speed': 6.2, 'wind_gust_direction': 270},
         meta_path=data_dir / 'observations_recent_extrema_wind_akt_meta.zip'
     )
 
 
-def test_wind_gusts_observations_parser_extra_urls(data_dir):
-    parser = WindGustsObservationsParser()
-    path = data_dir / 'observations_recent_extrema_wind_akt.zip'
-    expected_meta_url = (
-        'https://opendata.dwd.de/climate_environment/CDC/observations_germany/'
-        'climate/10_minutes/extreme_wind/meta_data/'
-        'Meta_Daten_zehn_min_fx_01766.zip'
-    )
-    assert parser.get_extra_urls(path) == {
-        'meta_path': expected_meta_url,
-    }
-
-
 def test_sunshine_observations_parser(data_dir):
     _test_parser(
         SunshineObservationsParser,
         data_dir / 'observations_recent_SD_akt.zip',
         {'timestamp': '2018-09-15 11:00', 'sunshine': 600.},
         {'timestamp': '2020-03-17 16:00', 'sunshine': 0.},
         first_idx=2,
@@ -383,23 +390,35 @@
     p = PressureObservationsParser()
     records = list(p.parse(data_dir / 'observations_recent_P0_hist.zip'))
     # The actual reduced pressure deleted from the test observation file was
     # 1023.0 hPa
     assert records[4]['pressure_msl'] == 102260
 
 
+def test_solar_radiation_observations_parser(data_dir):
+    _test_parser(
+        SolarRadiationObservationsParser,
+        data_dir / '10minutenwerte_SOLAR_01766_now.zip',
+        {'timestamp': '2023-04-12 01:00', 'solar': 0.0},
+        {'timestamp': '2023-04-12 12:00', 'solar': 674000.},
+        meta_path=data_dir / 'Meta_Daten_zehn_min_sd_01766.zip',
+        count=12,
+    )
+
+
 def test_get_parser():
     synop_with_timestamp = (
         'Z__C_EDZW_20200617114802_bda01,synop_bufr_GER_999999_999999__MW_617'
         '.json.bz2')
     synop_latest = (
         'Z__C_EDZW_latest_bda01,synop_bufr_GER_999999_999999__MW_XXX.json.bz2')
     expected = {
         '10minutenwerte_extrema_wind_00427_akt.zip': (
             WindGustsObservationsParser),
+        '10minutenwerte_SOLAR_01766_now.zip': SolarRadiationObservationsParser,
         'stundenwerte_FF_00011_akt.zip': WindObservationsParser,
         'stundenwerte_FF_00090_akt.zip': WindObservationsParser,
         'stundenwerte_N_01766_akt.zip': CloudCoverObservationsParser,
         'stundenwerte_P0_00096_akt.zip': PressureObservationsParser,
         'stundenwerte_RR_00102_akt.zip': PrecipitationObservationsParser,
         'stundenwerte_SD_00125_akt.zip': SunshineObservationsParser,
         'stundenwerte_TD_01766.zip': DewPointObservationsParser,
```

### Comparing `dwdparse-0.9.4/tests/test_stations.py` & `dwdparse-0.9.5/tests/test_stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.4/tests/test_units.py` & `dwdparse-0.9.5/tests/test_units.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     record = {
         'source_id': 11695,
         'timestamp': '2020-08-18T13:00:00+00:00',
         'dew_point': 285.96,
         'precipitation_60': 0,
         'pressure_msl': 101050,
         'relative_humidity': 51,
+        'solar': 1965600,
         'visibility': 75000,
         'wind_direction_60': 248,
         'wind_speed_60': 5,
         'wind_gust_direction_60': 230,
         'wind_gust_speed_60': 9.1,
         'sunshine_60': 1980,
         'temperature': 296.65,
@@ -47,14 +48,15 @@
     expected = {
         'source_id': 11695,
         'timestamp': '2020-08-18T13:00:00+00:00',
         'dew_point': 12.81,
         'precipitation_60': 0,
         'pressure_msl': 1010.5,
         'relative_humidity': 51,
+        'solar': 0.546,
         'visibility': 75000,
         'wind_direction_60': 248,
         'wind_speed_60': 18,
         'wind_gust_direction_60': 230,
         'wind_gust_speed_60': 32.8,
         'sunshine_60': 33,
         'temperature': 23.5,
```

