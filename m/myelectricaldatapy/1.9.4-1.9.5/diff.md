# Comparing `tmp/myelectricaldatapy-1.9.4.tar.gz` & `tmp/myelectricaldatapy-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-1.9.4.tar", last modified: Sat Apr  8 13:48:21 2023, max compression
+gzip compressed data, was "myelectricaldatapy-1.9.5.tar", last modified: Wed Apr 12 06:09:54 2023, max compression
```

## Comparing `myelectricaldatapy-1.9.4.tar` & `myelectricaldatapy-1.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:48:21.571488 myelectricaldatapy-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-08 13:48:21.571488 myelectricaldatapy-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:48:21.567488 myelectricaldatapy-1.9.4/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/myelectricaldatapy/mypdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:48:21.567488 myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-08 13:48:21.000000 myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-08 13:48:21.000000 myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 13:48:21.000000 myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 13:48:21.000000 myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 13:48:21.000000 myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 13:48:21.571488 myelectricaldatapy-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-08 13:48:20.000000 myelectricaldatapy-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:48:21.571488 myelectricaldatapy-1.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-08 13:48:12.000000 myelectricaldatapy-1.9.4/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/mypdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-12 06:09:53.000000 myelectricaldatapy-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-1.9.4/LICENSE` & `myelectricaldatapy-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.4/PKG-INFO` & `myelectricaldatapy-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.4
+Version: 1.9.5
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.4/README.md` & `myelectricaldatapy-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.4/myelectricaldatapy/analytics.py` & `myelectricaldatapy-1.9.5/myelectricaldatapy/analytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import re
 from datetime import datetime as dt
 from datetime import timedelta
 from typing import Any, Collection, Tuple
 
 import pandas as pd
 
+from .const import ATTR_OFFPEAK, ATTR_STANDARD
+
 _LOGGER = logging.getLogger(__name__)
 
 
 class EnedisAnalytics:
     """Data analaytics."""
 
     local_timezone = dt.now().astimezone().tzinfo
@@ -63,15 +65,15 @@
                 dt_start_date = pd.to_datetime(start_date, format="%Y-%m-%d %H:%M:%S")
                 dt_start_date = dt_start_date.tz_localize(self.local_timezone)
                 self.df = self.df[(self.df.date > dt_start_date)]
 
             self.df.index = self.df.date
 
             # Add mark
-            self.df["notes"] = "standard"
+            self.df["notes"] = ATTR_STANDARD
 
         if self.df.empty:
             return self.df.to_dict(orient="records")
 
         self.df.interval_length = (
             self.df.interval_length.transform(self._weighted_interval)
             if step_hour
@@ -142,15 +144,15 @@
             # Convert str to datetime
             start = pd.to_datetime(intervall[0], format="%H:%M:%S").time()
             end = pd.to_datetime(intervall[1], format="%H:%M:%S").time()
             # Mark
             self.df.loc[
                 (self.df.date.dt.time > start) & (self.df.date.dt.time <= end),
                 "notes",
-            ] = "offpeak"
+            ] = ATTR_OFFPEAK
 
         return self.df
 
     def _set_tempo_days(self, tempo: dict[str, str]) -> pd.DataFrame:
         """Add columns with tempo day."""
         for str_date, value in tempo.items():
             dt_date = pd.to_datetime(str_date, format="%Y-%m-%d")
```

### Comparing `myelectricaldatapy-1.9.4/myelectricaldatapy/auth.py` & `myelectricaldatapy-1.9.5/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.4/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-1.9.5/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.4/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-1.9.5/myelectricaldatapy/mypdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,17 @@
             }
         }
         If the update succeeds, the next one can only be done on the next day
         at least that force_refresh is true
         """
         self.access = await self._api.async_valid_access(self.pdl)
         if (
-            self._last_access is not None
-            and self._last_access > dt.now().date()
-            and force_refresh is False
+            force_refresh is False
+            and self._last_access is not None
+            and self._last_access == dt.now().date()
         ):
             return
 
         start = dt.now() - timedelta(days=730)
         end = dt.now()
         funcs: dict[str, Callable[..., Any]] = {
             DAILY_PROD: self._api.async_get_daily_production,
```

### Comparing `myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.4
+Version: 1.9.5
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.4/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.4/pyproject.toml` & `myelectricaldatapy-1.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.4/setup.py` & `myelectricaldatapy-1.9.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="myelectricaldatapy",
-    version="1.9.4",
+    version="1.9.5",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Fetch Linky data from myelectricaldata.fr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "pandas==1.4.3", "voluptuous>=0.13.1"],
```

### Comparing `myelectricaldatapy-1.9.4/tests/consts.py` & `myelectricaldatapy-1.9.5/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.4/tests/test_analytics.py` & `myelectricaldatapy-1.9.5/tests/test_analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     assert resultat[0]["value"] == 1.296
 
     dataset = DS_DAILY
     modes = {"consumption": {"service": "daily_consumption"}}
     with patch.object(
         myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
     ):
-        await api.async_update(modes=modes)
+        await api.async_update(modes=modes, force_refresh=True)
         resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert resultat[0]["value"] == 42.045
 
 
 @freeze_time("2023-03-01")
@@ -69,15 +69,15 @@
     assert round(resultat[0]["price"], 2) == 0.22
 
     dataset = DS_DAILY
     modes = {"consumption": {"service": "daily_consumption"}}
     with patch.object(
         myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
     ):
-        await api.async_update(modes=modes)
+        await api.async_update(modes=modes, force_refresh=True)
         resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert round(resultat[0]["price"], 2) == 7.15
 
 
 @freeze_time("2023-03-01")
@@ -202,15 +202,15 @@
 
     sum_value_1 = resultat1[26]["sum_value"] + resultat1[77]["sum_value"]
     assert round(sum_value, 3) == round(sum_value_1, 3)
     dataset = DS_COMPARE
     with patch.object(
         myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
     ):
-        await api.async_update(modes=modes)
+        await api.async_update(modes=modes, force_refresh=True)
         resultat2 = api.stats["consumption"]
     assert round(sum_value, 3) == resultat2[2]["sum_value"]
     print(resultat2)
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
```

### Comparing `myelectricaldatapy-1.9.4/tests/test_load_data.py` & `myelectricaldatapy-1.9.5/tests/test_load_data.py`

 * *Files identical despite different names*

