# Comparing `tmp/aliyun-python-sdk-eventbridge-1.0.6.tar.gz` & `tmp/aliyun-python-sdk-eventbridge-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eventbridge-1.0.6.tar", last modified: Fri Apr  7 03:43:53 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eventbridge-1.0.7.tar", last modified: Wed Apr 12 14:04:43 2023, max compression
```

## Comparing `aliyun-python-sdk-eventbridge-1.0.6.tar` & `aliyun-python-sdk-eventbridge-1.0.7.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1577 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3223 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateApiDestinationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateEventBusRequest.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateEventSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateEventStreamingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateServiceLinkedRoleForProductRequest.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateTargetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteApiDestinationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteEventBusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteEventSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteEventStreamingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteTargetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DisableRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/EnableRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetApiDestinationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetEventBusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1250 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetEventStreamingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListAliyunOfficialEventSourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1878 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListApiDestinationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListConnectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListEventBusesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListEventStreamingsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListUserDefinedEventSourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/PauseEventStreamingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/PutTargetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryEventRequest.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryEventTracesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryTracedEventByEventIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryTracedEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/StartEventStreamingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateApiDestinationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateEventBusRequest.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateEventSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateEventStreamingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2492 2023-04-07 03:43:53.000000 aliyun-python-sdk-eventbridge-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      543 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateApiDestinationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateEventBusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateEventSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateEventStreamingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateServiceLinkedRoleForProductRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateTargetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteApiDestinationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteEventBusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteEventSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteEventStreamingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteTargetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DisableRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/EnableRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetApiDestinationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetEventBusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetEventStreamingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListAliyunOfficialEventSourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListApiDestinationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListConnectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListEventBusesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListEventStreamingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListUserDefinedEventSourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/PauseEventStreamingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/PutTargetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryEventRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryEventTracesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryTracedEventByEventIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryTracedEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/StartEventStreamingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/TestEventPatternRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateApiDestinationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateEventBusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateEventSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateEventStreamingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-04-12 14:04:43.000000 aliyun-python-sdk-eventbridge-1.0.7/setup.py
```

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/LICENSE` & `aliyun-python-sdk-eventbridge-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/PKG-INFO` & `aliyun-python-sdk-eventbridge-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eventbridge
-Version: 1.0.6
+Version: 1.0.7
 Summary: The eventbridge module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eventbridge
```

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/README.rst` & `aliyun-python-sdk-eventbridge-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/PKG-INFO` & `aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eventbridge
-Version: 1.0.6
+Version: 1.0.7
 Summary: The eventbridge module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eventbridge
```

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyun_python_sdk_eventbridge.egg-info/SOURCES.txt` & `aliyun-python-sdk-eventbridge-1.0.7/aliyun_python_sdk_eventbridge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 aliyunsdkeventbridge/request/v20200401/PauseEventStreamingRequest.py
 aliyunsdkeventbridge/request/v20200401/PutTargetsRequest.py
 aliyunsdkeventbridge/request/v20200401/QueryEventRequest.py
 aliyunsdkeventbridge/request/v20200401/QueryEventTracesRequest.py
 aliyunsdkeventbridge/request/v20200401/QueryTracedEventByEventIdRequest.py
 aliyunsdkeventbridge/request/v20200401/QueryTracedEventsRequest.py
 aliyunsdkeventbridge/request/v20200401/StartEventStreamingRequest.py
+aliyunsdkeventbridge/request/v20200401/TestEventPatternRequest.py
 aliyunsdkeventbridge/request/v20200401/UpdateApiDestinationRequest.py
 aliyunsdkeventbridge/request/v20200401/UpdateConnectionRequest.py
 aliyunsdkeventbridge/request/v20200401/UpdateEventBusRequest.py
 aliyunsdkeventbridge/request/v20200401/UpdateEventSourceRequest.py
 aliyunsdkeventbridge/request/v20200401/UpdateEventStreamingRequest.py
 aliyunsdkeventbridge/request/v20200401/UpdateRuleRequest.py
 aliyunsdkeventbridge/request/v20200401/__init__.py
```

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateApiDestinationRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateApiDestinationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateConnectionRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateEventBusRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateEventBusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateEventSourceRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateEventSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateEventStreamingRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateEventStreamingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateRuleRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateServiceLinkedRoleForProductRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateServiceLinkedRoleForProductRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/CreateTargetsRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/CreateTargetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteApiDestinationRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteApiDestinationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteConnectionRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteEventBusRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteEventBusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteEventSourceRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteEventSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteEventStreamingRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteEventStreamingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteRuleRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DeleteTargetsRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DeleteTargetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/DisableRuleRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/DisableRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/EnableRuleRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/EnableRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetApiDestinationRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetApiDestinationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetConnectionRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetEventBusRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetEventBusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetEventStreamingRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetEventStreamingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/GetRuleRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/GetRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListAliyunOfficialEventSourcesRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListAliyunOfficialEventSourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListApiDestinationsRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListApiDestinationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListConnectionsRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListConnectionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListEventBusesRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListEventBusesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListEventStreamingsRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListEventStreamingsRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 		self.set_method('POST')
 
 	def get_NextToken(self): # String
 		return self.get_body_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_body_params('NextToken', NextToken)
-	def get_Limit(self): # Long
+	def get_Limit(self): # Integer
 		return self.get_body_params().get('Limit')
 
-	def set_Limit(self, Limit):  # Long
+	def set_Limit(self, Limit):  # Integer
 		self.add_body_params('Limit', Limit)
 	def get_NamePrefix(self): # String
 		return self.get_body_params().get('NamePrefix')
 
 	def set_NamePrefix(self, NamePrefix):  # String
 		self.add_body_params('NamePrefix', NamePrefix)
```

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListRulesRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/ListUserDefinedEventSourcesRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/ListUserDefinedEventSourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/PauseEventStreamingRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/PauseEventStreamingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/PutTargetsRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/PutTargetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryEventRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryEventRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryEventTracesRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryEventTracesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryTracedEventByEventIdRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryTracedEventByEventIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/QueryTracedEventsRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/QueryTracedEventsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/StartEventStreamingRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/StartEventStreamingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateApiDestinationRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateApiDestinationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateConnectionRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateEventBusRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateEventBusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateEventSourceRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateEventSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateEventStreamingRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateEventStreamingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/aliyunsdkeventbridge/request/v20200401/UpdateRuleRequest.py` & `aliyun-python-sdk-eventbridge-1.0.7/aliyunsdkeventbridge/request/v20200401/UpdateRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eventbridge-1.0.6/setup.py` & `aliyun-python-sdk-eventbridge-1.0.7/setup.py`

 * *Files identical despite different names*

