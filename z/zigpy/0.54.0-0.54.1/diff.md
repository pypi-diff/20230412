# Comparing `tmp/zigpy-0.54.0.tar.gz` & `tmp/zigpy-0.54.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-0.54.0.tar", last modified: Wed Mar 29 23:50:42 2023, max compression
+gzip compressed data, was "zigpy-0.54.1.tar", last modified: Tue Apr 11 23:16:42 2023, max compression
```

## Comparing `zigpy-0.54.0.tar` & `zigpy-0.54.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-29 23:50:38.000000 zigpy-0.54.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-29 23:50:38.000000 zigpy-0.54.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-03-29 23:50:42.685885 zigpy-0.54.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-03-29 23:50:38.000000 zigpy-0.54.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-29 23:50:42.685885 zigpy-0.54.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-29 23:50:38.000000 zigpy-0.54.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.681885 zigpy-0.54.0/zigpy/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43034 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.681885 zigpy-0.54.0/zigpy/appdb_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v0.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v1.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v2.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v4.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v5.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v6.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v8.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/appdb_schemas/schema_v9.sql
--rw-r--r--   0 runner    (1001) docker     (123)    40169 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/backups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.681885 zigpy-0.54.0/zigpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/zigpy/ota/
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/ota/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/ota/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/ota/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/zigpy/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/profiles/zha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/profiles/zll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/zigpy/quirks/
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/quirks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/quirks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/zigpy/types/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/zigpy/zcl/
--rw-r--r--   0 runner    (1001) docker     (123)    33225 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/zigpy/zcl/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25260 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/closures.py
--rw-r--r--   0 runner    (1001) docker     (123)    82633 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/hvac.py
--rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/manufacturer_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/clusters/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (123)    31472 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zcl/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.685885 zigpy-0.54.0/zigpy/zdo/
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-03-29 23:50:38.000000 zigpy-0.54.0/zigpy/zdo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:50:42.681885 zigpy-0.54.0/zigpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-03-29 23:50:42.000000 zigpy-0.54.0/zigpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-29 23:50:42.000000 zigpy-0.54.0/zigpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 23:50:42.000000 zigpy-0.54.0/zigpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-29 23:50:42.000000 zigpy-0.54.0/zigpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-29 23:50:42.000000 zigpy-0.54.0/zigpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 23:16:39.000000 zigpy-0.54.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-11 23:16:39.000000 zigpy-0.54.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-11 23:16:42.214049 zigpy-0.54.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 23:16:39.000000 zigpy-0.54.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-11 23:16:42.214049 zigpy-0.54.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 23:16:39.000000 zigpy-0.54.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.206049 zigpy-0.54.1/zigpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43034 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/appdb_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v0.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v4.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v5.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v6.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v8.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v9.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    41314 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/backups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/ota/
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/profiles/zha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/profiles/zll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/quirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/quirks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/quirks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/zcl/
+-rw-r--r--   0 runner    (1001) docker     (123)    33225 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/zcl/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25260 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82633 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/manufacturer_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31472 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/zdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zdo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.206049 zigpy-0.54.1/zigpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/top_level.txt
```

### Comparing `zigpy-0.54.0/COPYING` & `zigpy-0.54.1/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/LICENSE` & `zigpy-0.54.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/PKG-INFO` & `zigpy-0.54.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.54.0
+Version: 0.54.1
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.54.0/README.md` & `zigpy-0.54.1/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/setup.cfg` & `zigpy-0.54.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/setup.py` & `zigpy-0.54.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "attrs",
     "aiohttp",
     "aiosqlite>=0.16.0",
     "async_timeout",
     "crccheck",
     "cryptography",
     'importlib_resources; python_version<"3.9"',
+    'async-timeout; python_version<"3.11"',
     "voluptuous",
     'pyserial-asyncio; platform_system!="Windows"',
     'pyserial-asyncio!=0.5; platform_system=="Windows"',
 ]
 
 setup(
     name="zigpy",
```

### Comparing `zigpy-0.54.0/zigpy/appdb.py` & `zigpy-0.54.1/zigpy/appdb.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v0.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v0.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v1.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v1.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v10.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v10.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v11.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v11.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v2.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v2.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v3.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v3.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v4.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v4.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v5.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v5.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v6.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v6.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v7.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v7.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v8.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v8.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/appdb_schemas/schema_v9.sql` & `zigpy-0.54.1/zigpy/appdb_schemas/schema_v9.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/application.py` & `zigpy-0.54.1/zigpy/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,28 @@
 import asyncio
 import collections
 import contextlib
 import errno
 import logging
 import os
 import random
+import sys
 import time
 import typing
-from typing import Any
+from typing import Any, Coroutine, TypeVar
+
+if sys.version_info[:2] < (3, 11):
+    from async_timeout import timeout as asyncio_timeout  # pragma: no cover
+else:
+    from asyncio import timeout as asyncio_timeout  # pragma: no cover
 
 import zigpy.appdb
 import zigpy.backups
 import zigpy.config as conf
+import zigpy.const as const
 import zigpy.device
 import zigpy.exceptions
 import zigpy.group
 import zigpy.listeners
 import zigpy.ota
 import zigpy.profiles
 import zigpy.quirks
@@ -35,14 +42,15 @@
 LOGGER = logging.getLogger(__name__)
 
 TRANSIENT_CONNECTION_ERRORS = {
     errno.ENETUNREACH,
 }
 
 ENERGY_SCAN_WARN_THRESHOLD = 0.75 * 255
+_R = TypeVar("_R")
 
 
 class ControllerApplication(zigpy.util.ListenableMixin, abc.ABC):
     SCHEMA = conf.CONFIG_SCHEMA
     SCHEMA_DEVICE = conf.SCHEMA_DEVICE
 
     def __init__(self, config: dict):
@@ -51,27 +59,40 @@
         self._listeners = {}
         self._config = self.SCHEMA(config)
         self._dblistener = None
         self._groups = zigpy.group.Groups(self)
         self._listeners = {}
         self._ota = zigpy.ota.OTA(self)
         self._send_sequence = 0
+        self._tasks: set[asyncio.Future[Any]] = set()
 
         self._concurrent_requests_semaphore = zigpy.util.DynamicBoundedSemaphore(
             self._config[conf.CONF_MAX_CONCURRENT_REQUESTS]
         )
 
         self.backups: zigpy.backups.BackupManager = zigpy.backups.BackupManager(self)
         self.topology: zigpy.topology.Topology = zigpy.topology.Topology(self)
 
         self._req_listeners: collections.defaultdict[
             zigpy.device.Device,
             collections.deque[zigpy.listeners.BaseRequestListener],
         ] = collections.defaultdict(lambda: collections.deque([]))
 
+    def create_task(
+        self, target: Coroutine[Any, Any, _R], name: str | None = None
+    ) -> asyncio.Task[_R]:
+        """Create a task and store a reference to it until the task completes.
+
+        target: target to call.
+        """
+        task = asyncio.get_running_loop().create_task(target, name=name)
+        self._tasks.add(task)
+        task.add_done_callback(self._tasks.remove)
+        return task
+
     async def _load_db(self) -> None:
         """Restore save state."""
         database_file = self.config[conf.CONF_DATABASE]
         if not database_file:
             return
 
         self._dblistener = await zigpy.appdb.PersistingListener.new(database_file, self)
@@ -119,27 +140,24 @@
                 f"Current settings: {new_state!r}\n"
                 f"Last backup: {last_backup!r}"
             )
 
         await self.start_network()
 
         # Some radios erroneously permit joins on startup
-        await self.permit(0)
-
-        if self.config[conf.CONF_NWK_BACKUP_ENABLED]:
-            self.backups.start_periodic_backups(
-                # Config specifies the period in minutes, not seconds
-                period=(60 * self.config[conf.CONF_NWK_BACKUP_PERIOD])
-            )
+        try:
+            await self.permit(0)
+        except zigpy.exceptions.DeliveryError as e:
+            if e.status != t.MACStatus.MAC_CHANNEL_ACCESS_FAILURE:
+                raise
 
-        if self.config[conf.CONF_TOPO_SCAN_ENABLED]:
-            # Config specifies the period in minutes, not seconds
-            self.topology.start_periodic_scans(
-                period=(60 * self.config[zigpy.config.CONF_TOPO_SCAN_PERIOD])
-            )
+            # Some radios (like the Conbee) can fail to deliver the startup broadcast
+            # due to interference
+            LOGGER.warning("Failed to send startup broadcast: %s", e)
+            LOGGER.warning(const.INTERFERENCE_MESSAGE)
 
         if self.config[conf.CONF_STARTUP_ENERGY_SCAN]:
             # Each scan period is 15.36ms. Scan for at least 200ms (2^4 + 1 periods) to
             # pick up WiFi beacon frames.
             results = await self.energy_scan(
                 channels=t.Channels.ALL_CHANNELS, duration_exp=4, count=1
             )
@@ -147,32 +165,39 @@
 
             if results[self.state.network_info.channel] > ENERGY_SCAN_WARN_THRESHOLD:
                 LOGGER.warning(
                     "Zigbee channel %s utilization is %0.2f%%!",
                     self.state.network_info.channel,
                     100 * results[self.state.network_info.channel] / 255,
                 )
-                LOGGER.warning(
-                    "If you are having problems joining new devices, are missing sensor"
-                    " updates, or have issues keeping devices joined, ensure your"
-                    " coordinator is away from interference sources such as USB 3.0"
-                    " devices, SSDs, WiFi routers, etc."
-                )
+                LOGGER.warning(const.INTERFERENCE_MESSAGE)
+
+        if self.config[conf.CONF_NWK_BACKUP_ENABLED]:
+            self.backups.start_periodic_backups(
+                # Config specifies the period in minutes, not seconds
+                period=(60 * self.config[conf.CONF_NWK_BACKUP_PERIOD])
+            )
+
+        if self.config[conf.CONF_TOPO_SCAN_ENABLED]:
+            # Config specifies the period in minutes, not seconds
+            self.topology.start_periodic_scans(
+                period=(60 * self.config[zigpy.config.CONF_TOPO_SCAN_PERIOD])
+            )
 
     async def startup(self, *, auto_form: bool = False):
         """Starts a network, optionally forming one with random settings if necessary."""
 
         try:
             await self.connect()
             await self.initialize(auto_form=auto_form)
         except Exception as e:
             LOGGER.error("Couldn't start application", exc_info=e)
             await self.shutdown()
 
-            if isinstance(e, ConnectionRefusedError) or (
+            if isinstance(e, ConnectionError) or (
                 isinstance(e, OSError) and e.errno in TRANSIENT_CONNECTION_ERRORS
             ):
                 raise zigpy.exceptions.TransientConnectionError() from e
 
             raise
 
     @classmethod
@@ -300,14 +325,15 @@
         await self.backups.restore_backup(
             backup=zigpy.backups.NetworkBackup(
                 network_info=network_info,
                 node_info=node_info,
             ),
             counter_increment=0,
             allow_incomplete=True,
+            create_new=(not fast),
         )
 
     async def shutdown(self) -> None:
         """Shutdown controller."""
         self.backups.stop_periodic_backups()
         self.topology.stop_periodic_scans()
 
@@ -349,16 +375,17 @@
         if not dev:
             LOGGER.debug("Device not found for removal: %s", ieee)
             return
 
         dev.cancel_initialization()
 
         LOGGER.info("Removing device 0x%04x (%s)", dev.nwk, ieee)
-        asyncio.create_task(
-            self._remove_device(dev, remove_children=remove_children, rejoin=rejoin)
+        self.create_task(
+            self._remove_device(dev, remove_children=remove_children, rejoin=rejoin),
+            f"remove_device-nwk={dev.nwk!r}-ieee={ieee!r}",
         )
         if dev.node_desc is not None and dev.node_desc.is_end_device:
             parents = []
 
             for parent in self.devices.values():
                 for zdo_neighbor in self.topology.neighbors[parent.ieee]:
                     try:
@@ -386,20 +413,20 @@
         self,
         device: zigpy.device.Device,
         remove_children: bool = True,
         rejoin: bool = False,
     ) -> None:
         """Send a remove request then pop the device."""
         try:
-            await asyncio.wait_for(
-                device.zdo.leave(remove_children=remove_children, rejoin=rejoin),
-                timeout=30
+            async with asyncio_timeout(
+                30
                 if device.node_desc is not None and device.node_desc.is_end_device
-                else 7,
-            )
+                else 7
+            ):
+                await device.zdo.leave(remove_children=remove_children, rejoin=rejoin)
         except (zigpy.exceptions.DeliveryError, asyncio.TimeoutError) as ex:
             LOGGER.debug("Sending 'zdo_leave_req' failed: %s", ex)
 
         self.devices.pop(device.ieee, None)
 
     def deserialize(
         self,
@@ -543,15 +570,18 @@
 
     def handle_relays(self, nwk: t.NWK, relays: list[t.NWK]) -> None:
         """Called when a list of relaying devices is received."""
         try:
             device = self.get_device(nwk=nwk)
         except KeyError:
             LOGGER.warning("Received relays from an unknown device: %s", nwk)
-            asyncio.create_task(self._discover_unknown_device(nwk))
+            self.create_task(
+                self._discover_unknown_device(nwk),
+                f"discover_unknown_device_from_relays-nwk={nwk!r}",
+            )
         else:
             # `relays` is a property with a setter that emits an event
             device.relays = relays
 
     @classmethod
     async def probe(cls, device_config: dict[str, Any]) -> bool | dict[str, Any]:
         """Probes the device specified by `device_config` and returns valid device settings
@@ -900,15 +930,18 @@
         try:
             device = self.get_device_with_address(packet.src)
         except KeyError:
             LOGGER.warning("Unknown device %r", packet.src)
 
             if packet.src.addr_mode == t.AddrMode.NWK:
                 # Manually send a ZDO IEEE address request to discover the device
-                asyncio.create_task(self._discover_unknown_device(packet.src.address))
+                self.create_task(
+                    self._discover_unknown_device(packet.src.address),
+                    f"discover_unknown_device_from_packet-nwk={packet.src.address!r}",
+                )
 
             return
 
         device.radio_details(lqi=packet.lqi, rssi=packet.rssi)
 
         self.handle_message(
             sender=device,
```

### Comparing `zigpy-0.54.0/zigpy/backups.py` & `zigpy-0.54.1/zigpy/backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/config/__init__.py` & `zigpy-0.54.1/zigpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/config/defaults.py` & `zigpy-0.54.1/zigpy/config/defaults.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/config/validators.py` & `zigpy-0.54.1/zigpy/config/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/device.py` & `zigpy-0.54.1/zigpy/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from __future__ import annotations
 
 import asyncio
 import binascii
 from datetime import datetime, timezone
 import enum
 import logging
+import sys
 import typing
 
+if sys.version_info[:2] < (3, 11):
+    from async_timeout import timeout as asyncio_timeout  # pragma: no cover
+else:
+    from asyncio import timeout as asyncio_timeout  # pragma: no cover
+
 from zigpy.const import (
     SIG_ENDPOINTS,
     SIG_EP_INPUT,
     SIG_EP_OUTPUT,
     SIG_EP_PROFILE,
     SIG_EP_TYPE,
     SIG_MANUFACTURER,
@@ -303,15 +309,16 @@
                 use_ieee=use_ieee,
                 extended_timeout=extended_timeout,
             )
 
             if not expect_reply:
                 return None
 
-            return await asyncio.wait_for(req.result, timeout)
+            async with asyncio_timeout(timeout):
+                return await req.result
 
     def deserialize(self, endpoint_id, cluster_id, data):
         return self.endpoints[endpoint_id].deserialize(cluster_id, data)
 
     def handle_message(
         self,
         profile: int,
```

### Comparing `zigpy-0.54.0/zigpy/endpoint.py` & `zigpy-0.54.1/zigpy/endpoint.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/exceptions.py` & `zigpy-0.54.1/zigpy/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+
 class ZigbeeException(Exception):
     """Base exception class"""
 
 
 class ControllerException(ZigbeeException):
     """Application controller failed in some way."""
 
@@ -9,15 +12,15 @@
 class APIException(ZigbeeException):
     """Radio API failed in some way."""
 
 
 class DeliveryError(ZigbeeException):
     """Message delivery failed in some way"""
 
-    def __init__(self, message: str, status=None):
+    def __init__(self, message: str, status: int | None = None):
         super().__init__(message)
         self.status = status
 
 
 class InvalidResponse(ZigbeeException):
     """A ZDO or ZCL response has an unsuccessful status code"""
```

### Comparing `zigpy-0.54.0/zigpy/group.py` & `zigpy-0.54.1/zigpy/group.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/listeners.py` & `zigpy-0.54.1/zigpy/listeners.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         command: foundation.CommandSchema,
     ) -> bool:
         try:
             result = self.callback(hdr, command)
 
             # Run coroutines in the background
             if asyncio.iscoroutine(result):
-                asyncio.create_task(result)
+                self.device.application.create_task(result)
         except Exception:
             LOGGER.warning(
                 "Caught an exception while executing callback", exc_info=True
             )
 
         # Callbacks are always resolved
         return True
```

### Comparing `zigpy-0.54.0/zigpy/ota/__init__.py` & `zigpy-0.54.1/zigpy/ota/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/ota/image.py` & `zigpy-0.54.1/zigpy/ota/image.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/ota/provider.py` & `zigpy-0.54.1/zigpy/ota/provider.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/ota/validators.py` & `zigpy-0.54.1/zigpy/ota/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/profiles/zha.py` & `zigpy-0.54.1/zigpy/profiles/zha.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/profiles/zll.py` & `zigpy-0.54.1/zigpy/profiles/zll.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/quirks/__init__.py` & `zigpy-0.54.1/zigpy/quirks/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/quirks/registry.py` & `zigpy-0.54.1/zigpy/quirks/registry.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/serial.py` & `zigpy-0.54.1/zigpy/serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/state.py` & `zigpy-0.54.1/zigpy/state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/topology.py` & `zigpy-0.54.1/zigpy/topology.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/types/basic.py` & `zigpy-0.54.1/zigpy/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/types/named.py` & `zigpy-0.54.1/zigpy/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/types/struct.py` & `zigpy-0.54.1/zigpy/types/struct.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/typing.py` & `zigpy-0.54.1/zigpy/typing.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/util.py` & `zigpy-0.54.1/zigpy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,21 +285,28 @@
             LOGGER.debug("Duplicate %s TSN", sequence)
             raise ControllerException(f"duplicate {sequence} TSN") from AssertionError
 
 
 class CatchingTaskMixin(LocalLogMixin):
     """Allow creating tasks suppressing exceptions."""
 
+    _tasks: set[asyncio.Future[typing.Any]] = set()
+
     def create_catching_task(
         self,
         target: typing.Coroutine,
         exceptions: type[Exception] | tuple | None = None,
+        name: str | None = None,
     ) -> None:
         """Create a task."""
-        asyncio.create_task(self.catching_coro(target, exceptions))
+        task = asyncio.get_running_loop().create_task(
+            self.catching_coro(target, exceptions), name=name
+        )
+        self._tasks.add(task)
+        task.add_done_callback(self._tasks.remove)
 
     async def catching_coro(
         self,
         target: typing.Coroutine,
         exceptions: type[Exception] | tuple | None = None,
     ) -> typing.Any:
         """Wrap a target coro and catch specified exceptions."""
```

### Comparing `zigpy-0.54.0/zigpy/zcl/__init__.py` & `zigpy-0.54.1/zigpy/zcl/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/__init__.py` & `zigpy-0.54.1/zigpy/zcl/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/closures.py` & `zigpy-0.54.1/zigpy/zcl/clusters/closures.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/general.py` & `zigpy-0.54.1/zigpy/zcl/clusters/general.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/homeautomation.py` & `zigpy-0.54.1/zigpy/zcl/clusters/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/hvac.py` & `zigpy-0.54.1/zigpy/zcl/clusters/hvac.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/lighting.py` & `zigpy-0.54.1/zigpy/zcl/clusters/lighting.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/lightlink.py` & `zigpy-0.54.1/zigpy/zcl/clusters/lightlink.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/measurement.py` & `zigpy-0.54.1/zigpy/zcl/clusters/measurement.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/protocol.py` & `zigpy-0.54.1/zigpy/zcl/clusters/protocol.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/security.py` & `zigpy-0.54.1/zigpy/zcl/clusters/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/clusters/smartenergy.py` & `zigpy-0.54.1/zigpy/zcl/clusters/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zcl/foundation.py` & `zigpy-0.54.1/zigpy/zcl/foundation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zdo/__init__.py` & `zigpy-0.54.1/zigpy/zdo/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy/zdo/types.py` & `zigpy-0.54.1/zigpy/zdo/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.0/zigpy.egg-info/PKG-INFO` & `zigpy-0.54.1/zigpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.54.0
+Version: 0.54.1
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.54.0/zigpy.egg-info/SOURCES.txt` & `zigpy-0.54.1/zigpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

