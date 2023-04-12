# Comparing `tmp/omnikdatalogger-1.9.0b5.tar.gz` & `tmp/omnikdatalogger-1.9.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnikdatalogger-1.9.0b5.tar", last modified: Sun Nov  7 17:50:57 2021, max compression
+gzip compressed data, was "omnikdatalogger-1.9.0b6.tar", last modified: Mon Nov  8 07:25:37 2021, max compression
```

## Comparing `omnikdatalogger-1.9.0b5.tar` & `omnikdatalogger-1.9.0b6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.689188 omnikdatalogger-1.9.0b5/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    77919 2021-11-07 17:50:57.689188 omnikdatalogger-1.9.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    77358 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.681188 omnikdatalogger-1.9.0b5/apps/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.685188 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/
--rw-r--r--   0 runner    (1001) docker     (121)    23841 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/data_fields.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.685188 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/
--rw-r--r--   0 runner    (1001) docker     (121)     6222 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/InverterMsg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4981 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    54513 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/datalogger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/daylight.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.685188 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/dsmr/
--rw-r--r--   0 runner    (1001) docker     (121)    14972 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/dsmr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7302 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/dsmr/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/ha_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plant.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.685188 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6102 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/localproxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7804 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/solarmanpv.py
--rw-r--r--   0 runner    (1001) docker     (121)     9885 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/tcpclient.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.685188 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/hassapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/mqtt_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/tcp_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.685188 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6077 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    18111 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     6307 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/pvoutput.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.689188 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    77919 2021-11-07 17:50:57.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-11-07 17:50:57.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-07 17:50:57.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-11-07 17:50:57.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-07 17:50:57.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    13024 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omniklogger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.681188 omnikdatalogger-1.9.0b5/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:50:57.689188 omnikdatalogger-1.9.0b5/scripts/systemd/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/scripts/systemd/omnikdatalogger.service
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-11-07 17:50:57.689188 omnikdatalogger-1.9.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2021-11-07 17:50:45.000000 omnikdatalogger-1.9.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.126068 omnikdatalogger-1.9.0b6/
+-rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    77919 2021-11-08 07:25:37.126068 omnikdatalogger-1.9.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    77358 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.118068 omnikdatalogger-1.9.0b6/apps/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/
+-rw-r--r--   0 runner    (1001) docker     (121)    23841 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/data_fields.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/
+-rw-r--r--   0 runner    (1001) docker     (121)     6222 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/InverterMsg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4981 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54513 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/datalogger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3490 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/daylight.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/dsmr/
+-rw-r--r--   0 runner    (1001) docker     (121)    14972 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/dsmr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7302 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/dsmr/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/ha_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plant.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6102 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/localproxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7804 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/solarmanpv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9996 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/tcpclient.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3706 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/hassapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/mqtt_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3034 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/tcp_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6077 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18111 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6307 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/pvoutput.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    77919 2021-11-08 07:25:36.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-11-08 07:25:36.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-08 07:25:36.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-11-08 07:25:36.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-08 07:25:36.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13024 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omniklogger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.122069 omnikdatalogger-1.9.0b6/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 07:25:37.126068 omnikdatalogger-1.9.0b6/scripts/systemd/
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/scripts/systemd/omnikdatalogger.service
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-11-08 07:25:37.126068 omnikdatalogger-1.9.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1717 2021-11-08 07:25:25.000000 omnikdatalogger-1.9.0b6/setup.py
```

### Comparing `omnikdatalogger-1.9.0b5/LICENSE.txt` & `omnikdatalogger-1.9.0b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/PKG-INFO` & `omnikdatalogger-1.9.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnikdatalogger
-Version: 1.9.0b5
+Version: 1.9.0b6
 Summary: Omnik Data Logger
 Home-page: https://github.com/jbouwh/omnikdatalogger
 Author: Jan Bouwhuis
 Author-email: jan@jbsoft.nl
 License: gpl-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `omnikdatalogger-1.9.0b5/README.md` & `omnikdatalogger-1.9.0b6/README.md`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/data_fields.json` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/data_fields.json`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/InverterMsg.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/InverterMsg.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/__init__.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from omnik.ha_logger import hybridlogger
 
 from datetime import datetime, timedelta, timezone
 import threading
 
 logging.basicConfig(stream=sys.stdout, level=os.environ.get("LOGLEVEL", logging.INFO))
 
-__version__ = "1.9.0-beta-5"
+__version__ = "1.9.0-beta-6"
 
 logger = logging.getLogger(__name__)
 
 
 class RepeatedJob(object):
     def __init__(self, c, datalogger, hass_api, *args, **kwargs):
         if c.get("default", "debug", fallback=False):
```

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/datalogger.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/datalogger.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/daylight.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/daylight.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/dsmr/__init__.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/dsmr/__init__.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/dsmr/terminal.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/dsmr/terminal.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/ha_logger.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/ha_logger.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plant.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plant.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/__init__.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/__init__.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/localproxy.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/localproxy.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/solarmanpv.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/solarmanpv.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_client/tcpclient.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_client/tcpclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.inverters = {}
         self.session = {}
 
         # self._mode indicates the access mode that will be used
         # 0: Not initialized
         # 1: Running in native mode (port 8899)
         # 2: Running in fallback mode (port 80) fetching http://{inverter_ip}:80/js/status.js
-        self._mode = 0
+        self._mode = {}
 
     def getPlants(self):
         data = []
         inverterdata = {}
         for plant in self.plant_id_list:
             inverter_address = self.config.get(
                 f"plant.{plant}", "inverter_address", fallback=None
@@ -92,51 +92,52 @@
                 "inverter_port": inverter_port,
                 "logger_sn": int(logger_sn),
                 "inverter_sn": inverter_sn,
                 "inverter_connection": inverter_connection,
                 "http_only": http_only,
             }
             self.inverters[plant] = inverterdata
+            self._mode[plant] = 0
             data.append({"plant_id": plant})
 
         hybridlogger.ha_log(
             self.logger, self.hass_api, "DEBUG", f"plant list from config {data}"
         )
 
         return data
 
     def getPlantData(self, plant_id):
         data = None
         http_only = self.inverters[plant_id].get("http_only")
-        if not self._mode and not http_only:
+        if not self._mode.get(plant_id) and not http_only:
             # native mode
             hybridlogger.ha_log(
                 self.logger,
                 self.hass_api,
                 "INFO",
                 f"Initializing: Trying to reach the inverter for plant {plant_id} over port 8899.",
             )
         if (
-            self._mode <= 1
+            self._mode.get(plant_id) <= 1
             and self.inverters[plant_id].get("inverter_sn")
             and self.inverters[plant_id].get("logger_sn")
             and not http_only
         ):
             data = self._getPlantData_native(plant_id)
         if data:
             # set mode to native
-            self._mode = 1
+            self._mode[plant_id] = 1
         if not self._mode:
             hybridlogger.ha_log(
                 self.logger,
                 self.hass_api,
                 "INFO",
                 f"Initializing: Trying to reach the inverter for plant {plant_id} over port http (fallback).",
             )
-        if self._mode == 0 or self._mode == 2:
+        if self._mode.get(plant_id) == 0 or self._mode.get(plant_id) == 2:
             # fall back mode
             data = self._getPlantData_fallback(plant_id)
 
         return data
 
     def _getPlantData_native(self, plant_id):
         # Create a TCP/IP socket
@@ -251,9 +252,9 @@
                 ),
                 "inverter": inverter_data[0],
                 "current_power": Decimal(inverter_data[5]),
                 "today_energy": Decimal(inverter_data[6]) / 100,
                 "total_energy": Decimal(inverter_data[7]) / 10,
             }
             # set mode to http
-            self._mode = 2
+            self._mode[plant_id] = 2
         return data
```

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/__init__.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/__init__.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/hassapi.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/hassapi.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/mqtt_proxy.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/mqtt_proxy.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_localproxy/tcp_proxy.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_localproxy/tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/__init__.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/__init__.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/influxdb.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/influxdb.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/mqtt.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/mqtt.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnik/plugin_output/pvoutput.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnik/plugin_output/pvoutput.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/PKG-INFO` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnikdatalogger
-Version: 1.9.0b5
+Version: 1.9.0b6
 Summary: Omnik Data Logger
 Home-page: https://github.com/jbouwh/omnikdatalogger
 Author: Jan Bouwhuis
 Author-email: jan@jbsoft.nl
 License: gpl-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omnikdatalogger.egg-info/SOURCES.txt` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omnikdatalogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/apps/omnikdatalogger/omniklogger.py` & `omnikdatalogger-1.9.0b6/apps/omnikdatalogger/omniklogger.py`

 * *Files identical despite different names*

### Comparing `omnikdatalogger-1.9.0b5/setup.py` & `omnikdatalogger-1.9.0b6/setup.py`

 * *Files identical despite different names*

