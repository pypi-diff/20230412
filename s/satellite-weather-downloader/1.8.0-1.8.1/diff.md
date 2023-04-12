# Comparing `tmp/satellite_weather_downloader-1.8.0.tar.gz` & `tmp/satellite_weather_downloader-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellite_weather_downloader-1.8.0.tar", max compression
+gzip compressed data, was "satellite_weather_downloader-1.8.1.tar", max compression
```

## Comparing `satellite_weather_downloader-1.8.0.tar` & `satellite_weather_downloader-1.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-04-04 20:05:42.894708 satellite_weather_downloader-1.8.0/LICENSE
--rw-r--r--   0        0        0     3072 2023-04-04 20:05:42.894708 satellite_weather_downloader-1.8.0/README.md
--rw-r--r--   0        0        0     1862 2023-04-04 20:07:49.872539 satellite_weather_downloader-1.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/__init__.py
--rw-r--r--   0        0        0      190 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/downloader/__init__.py
--rw-r--r--   0        0        0     9479 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/downloader/extract_reanalysis.py
--rw-r--r--   0        0        0       52 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/downloader/reanalysis/__init__.py
--rw-r--r--   0        0        0    12112 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/downloader/reanalysis/api_vars.py
--rw-r--r--   0        0        0    16153 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/downloader/reanalysis/prompt.py
--rw-r--r--   0        0        0     2924 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/downloader/request.py
--rw-r--r--   0        0        0      296 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/weather/__init__.py
--rw-r--r--   0        0        0       20 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/__init__.py
--rw-r--r--   0        0        0     1360 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas.py
--rw-r--r--   0        0        0       11 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas_dsei.cst
--rw-r--r--   0        0        0     9413 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas_dsei.dbf
--rw-r--r--   0        0        0      417 2023-04-04 20:05:42.898708 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas_dsei.prj
--rw-r--r--   0        0        0 11174984 2023-04-04 20:05:42.970709 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas_dsei.shp
--rw-r--r--   0        0        0      372 2023-04-04 20:05:42.970709 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas_dsei.shx
--rw-r--r--   0        0        0       77 2023-04-04 20:05:42.970709 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/__init__.py
--rw-r--r--   0        0        0     4119 2023-04-04 20:05:42.970709 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/extract_coordinates.py
--rw-r--r--   0        0        0     1351 2023-04-04 20:05:42.970709 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/extract_latlons.py
--rw-r--r--   0        0        0  1175429 2023-04-04 20:05:42.974709 satellite_weather_downloader-1.8.0/satellite/weather/_brazil/municipios.json
--rw-r--r--   0        0        0       40 2023-04-04 20:05:42.974709 satellite_weather_downloader-1.8.0/satellite/weather/utils/__init__.py
--rw-r--r--   0        0        0     4871 2023-04-04 20:05:42.974709 satellite_weather_downloader-1.8.0/satellite/weather/utils/episem.py
--rw-r--r--   0        0        0    11908 2023-04-04 20:05:42.974709 satellite_weather_downloader-1.8.0/satellite/weather/xr_extensions.py
--rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 17:48:08.413393 satellite_weather_downloader-1.8.1/LICENSE
+-rw-r--r--   0        0        0     3072 2023-04-12 17:48:08.413393 satellite_weather_downloader-1.8.1/README.md
+-rw-r--r--   0        0        0     1862 2023-04-12 17:50:24.654929 satellite_weather_downloader-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/__init__.py
+-rw-r--r--   0        0        0     9715 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/extract_reanalysis.py
+-rw-r--r--   0        0        0       52 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/__init__.py
+-rw-r--r--   0        0        0    12112 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/api_vars.py
+-rw-r--r--   0        0        0    16153 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/prompt.py
+-rw-r--r--   0        0        0     2924 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/request.py
+-rw-r--r--   0        0        0      296 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/__init__.py
+-rw-r--r--   0        0        0     1360 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas.py
+-rw-r--r--   0        0        0       11 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.cst
+-rw-r--r--   0        0        0     9413 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.dbf
+-rw-r--r--   0        0        0      417 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.prj
+-rw-r--r--   0        0        0 11174984 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.shp
+-rw-r--r--   0        0        0      372 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.shx
+-rw-r--r--   0        0        0       77 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/__init__.py
+-rw-r--r--   0        0        0     4119 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_coordinates.py
+-rw-r--r--   0        0        0     1351 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_latlons.py
+-rw-r--r--   0        0        0  1175429 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/municipios.json
+-rw-r--r--   0        0        0       40 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/utils/__init__.py
+-rw-r--r--   0        0        0     4871 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/utils/episem.py
+-rw-r--r--   0        0        0    11908 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/xr_extensions.py
+-rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.1/PKG-INFO
```

### Comparing `satellite_weather_downloader-1.8.0/LICENSE` & `satellite_weather_downloader-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/README.md` & `satellite_weather_downloader-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/pyproject.toml` & `satellite_weather_downloader-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "satellite-weather-downloader"
-version = "1.8.0"  # changed by semantic-release
+version = "1.8.1"  # changed by semantic-release
 description = "The modules available in this package are designed to capture and proccess satellite data from Copernicus"
 readme = "README.md"
 authors = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 maintainers = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/osl-incubator/satellite-weather-downloader"
 homepage = "https://github.com/osl-incubator/satellite-weather-downloader"
```

### Comparing `satellite_weather_downloader-1.8.0/satellite/downloader/extract_reanalysis.py` & `satellite_weather_downloader-1.8.1/satellite/downloader/extract_reanalysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 _MAX_DELAY_F = datetime.strftime(_MAX_DELAY, _DATE_FORMAT)
 
 # TODO: make download_br_netcdf accepts date and datetime types.
 def download_br_netcdf(
     date: Optional[str] = None,
     date_end: Optional[str] = None,
     data_dir: Optional[str] = _DATA_DIR,
+    user_key: Optional[str] = None,
 ):
     """
     Creates the request for Copernicus API. Extracts the latitude and
     longitude for a given geocode of a brazilian city, calculates the
     area in which the data will be retrieved and send the request via
     `cdsapi.Client()`. Data can be retrieved for a specific date or a
     date range, usage:
@@ -82,23 +83,29 @@
 
     Attrs:
         date (opt(str)): Format 'YYYY-MM-DD'. Date of data to be retrieved.
         date_end (opt(str)): Format 'YYYY-MM-DD'. Used along with `date`
                               to define a date range.
         data_dir (opt(str)): Path in which the NetCDF file will be downloaded.
                              Default dir is `$HOME/copernicus_data/`.
+        user_key (opt(str)): Credentials for retrieving Copernicus data. Format:
+                             "<MY_UID>:<MY_API_KEY>"
 
     Returns:
         String corresponding to path: `data_dir/filename`, that can later be used
         to transform into a `xarray.Dataset` with the CopeBRDatasetExtension located
         in `satellite_weather` module.
     """
     Path(data_dir).mkdir(parents=True, exist_ok=True)
 
-    cdsapi_key = os.getenv('CDSAPI_KEY')
+    if not user_key:
+        cdsapi_key = os.getenv('CDSAPI_KEY')
+    else:
+        cdsapi_key = user_key
+
     if not cdsapi_key:
         raise EnvironmentError(
             'Environment variable CDSAPI_KEY not found in the system.\n'
             'Execute `$ export CDSAPI_KEY="<MY_UID>:<MY_API_KEY>" to fix.\n'
             'These credentials are found in your Copernicus User Page: \n'
             'https://cds.climate.copernicus.eu/user/<MY_USER>'
         )
```

### Comparing `satellite_weather_downloader-1.8.0/satellite/downloader/reanalysis/api_vars.py` & `satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/api_vars.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/downloader/reanalysis/prompt.py` & `satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/prompt.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/downloader/request.py` & `satellite_weather_downloader-1.8.1/satellite/downloader/request.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas.py` & `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas_dsei.dbf` & `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.dbf`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/_brazil/DSEI/areas_dsei.shp` & `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.shp`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/_brazil/extract_coordinates.py` & `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/_brazil/extract_latlons.py` & `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_latlons.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/_brazil/municipios.json` & `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/municipios.json`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/utils/episem.py` & `satellite_weather_downloader-1.8.1/satellite/weather/utils/episem.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/satellite/weather/xr_extensions.py` & `satellite_weather_downloader-1.8.1/satellite/weather/xr_extensions.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.0/PKG-INFO` & `satellite_weather_downloader-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellite-weather-downloader
-Version: 1.8.0
+Version: 1.8.1
 Summary: The modules available in this package are designed to capture and proccess satellite data from Copernicus
 Home-page: https://github.com/osl-incubator/satellite-weather-downloader
 License: GNU GPL v3.0
 Author: Luã Bida Vacaro
 Author-email: luabidaa@gmail.com
 Maintainer: Luã Bida Vacaro
 Maintainer-email: luabidaa@gmail.com
```

