# Comparing `tmp/taegis-sdk-python-1.0.0a6.tar.gz` & `tmp/taegis-sdk-python-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.0a6.tar", last modified: Fri Mar 24 21:06:08 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.0a7.tar", last modified: Wed Apr 12 20:03:55 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.0a6.tar` & `taegis-sdk-python-1.0.0a7.tar`

### file list

```diff
@@ -1,168 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.474009 taegis-sdk-python-1.0.0a6/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5757 2023-03-24 21:06:08.474009 taegis-sdk-python-1.0.0a6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5320 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 21:06:08.474009 taegis-sdk-python-1.0.0a6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.451009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-24 21:06:08.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8552 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.452009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    11112 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.453009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2370 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.454009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.455009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3803 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6644 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78000 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.456009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14905 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.457009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8642 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12087 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22552 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.457009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.458009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.459009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15763 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    22552 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    30927 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.460009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6219 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.461009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8037 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.462009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.463009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3897 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.464009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8988 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.464009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12950 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24248 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.466009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22054 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    27703 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39075 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.467009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9242 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.467009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.468009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.469009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16048 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.470009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.471009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10847 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31216 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.472009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13732 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.473009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3856 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7910 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.474009 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11509 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25197 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-03-24 21:05:21.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:06:08.452009 taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5757 2023-03-24 21:06:08.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6552 2023-03-24 21:06:08.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 21:06:08.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-03-24 21:06:08.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-24 21:06:08.000000 taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.653665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8552 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.654665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    11461 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.654665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.655665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.656665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6644 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78106 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.657665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.658665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9259 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12852 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24754 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.658665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.659665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.660665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15763 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    22552 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    30927 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.661665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.662665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8037 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.662665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.663665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4109 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.664665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.665665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12950 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24248 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.666665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22054 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    27703 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39186 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.666665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6558 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    36501 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.667665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9242 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.668665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.669665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.670665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16048 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.670665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.671665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10847 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31499 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.672665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13732 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.673665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3856 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6309 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25285 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.653665 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6829 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.0a6/LICENSE` & `taegis-sdk-python-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/PKG-INFO` & `taegis-sdk-python-1.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0a6/README.md` & `taegis-sdk-python-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/setup.py` & `taegis-sdk-python-1.0.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/service_core.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from taegis_sdk_python.services.endpoint_management_service import (
     EndpointManagementServiceService,
 )
 from taegis_sdk_python.services.event_search import EventSearchService
 from taegis_sdk_python.services.events import EventsService
 from taegis_sdk_python.services.exports import ExportsService
 from taegis_sdk_python.services.investigations import InvestigationsService
+from taegis_sdk_python.services.investigations2 import Investigations2Service
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 from taegis_sdk_python.services.notebooks import NotebooksService
 from taegis_sdk_python.services.notifications import NotificationsService
 from taegis_sdk_python.services.rules import RulesService
 from taegis_sdk_python.services.sharelinks import SharelinksService
 from taegis_sdk_python.services.tenants import TenantsService
 from taegis_sdk_python.services.threat import ThreatService
@@ -91,14 +92,15 @@
         self._comments = None
         self._endpoint_command_manager = None
         self._endpoint_management_service = None
         self._event_search = None
         self._events = None
         self._exports = None
         self._investigations = None
+        self._investigations2 = None
         self._mitre_attack_info = None
         self._notebooks = None
         self._notifications = None
         self._rules = None
         self._core = None
         self._sharelinks = None
         self._tenants = None
@@ -277,14 +279,21 @@
     def investigations(self):
         """Investigations Service Endpoint."""
         if not self._investigations:
             self._investigations = InvestigationsService(self)
         return self._investigations
 
     @property
+    def investigations2(self):
+        """Investigations2 Service Endpoint."""
+        if not self._investigations2:
+            self._investigations2 = Investigations2Service(self)
+        return self._investigations2
+
+    @property
     def mitre_attack_info(self):
         """MitreAttackInfo Service Endpoint."""
         if not self._mitre_attack_info:
             self._mitre_attack_info = MitreAttackInfoService(self)
         return self._mitre_attack_info
 
     @property
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     """AgentChannel."""
 
     BETA = "BETA"
     PREVIEW = "PREVIEW"
     STABLE = "STABLE"
     DEV = "DEV"
     CANARY = "CANARY"
+    QE_PREV = "QE_PREV"
+    QE_NEXT = "QE_NEXT"
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class MetaData:
     """MetaData."""
 
@@ -81,14 +83,17 @@
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class PackageDownloadInput:
     """PackageDownloadInput."""
 
     version: Optional[str] = field(default=None, metadata=config(field_name="version"))
+    language: Optional[str] = field(
+        default=None, metadata=config(field_name="language")
+    )
     platform: Optional[AgentPlatform] = field(
         default=None, metadata=config(field_name="platform")
     )
     architecture: Optional[AgentArch] = field(
         default=None, metadata=config(field_name="architecture")
     )
     pkg_type: Optional[AgentPkgType] = field(
@@ -107,14 +112,17 @@
     modified_time: Optional[str] = field(
         default=None, metadata=config(field_name="modifiedTime")
     )
     checksum: Optional[str] = field(
         default=None, metadata=config(field_name="checksum")
     )
     size: Optional[int] = field(default=None, metadata=config(field_name="size"))
+    supported_languages: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="supportedLanguages")
+    )
     platform: Optional[AgentPlatform] = field(
         default=None, metadata=config(field_name="platform")
     )
     pkg_type: Optional[AgentPkgType] = field(
         default=None, metadata=config(field_name="pkgType")
     )
     architecture: Optional[AgentArch] = field(
@@ -130,14 +138,17 @@
 class PackageSearchInput:
     """PackageSearchInput."""
 
     num_recent_versions: Optional[int] = field(
         default=None, metadata=config(field_name="numRecentVersions")
     )
     version: Optional[str] = field(default=None, metadata=config(field_name="version"))
+    language: Optional[str] = field(
+        default=None, metadata=config(field_name="language")
+    )
     platform: Optional[AgentPlatform] = field(
         default=None, metadata=config(field_name="platform")
     )
     architecture: Optional[AgentArch] = field(
         default=None, metadata=config(field_name="architecture")
     )
     pkg_type: Optional[AgentPkgType] = field(
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/mutations.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         raise GraphQLNoRowsInResultSetError(
             "for mutation alertsServiceBulkInvestigationsProcessor"
         )
 
     def alerts_service_evict(
         self, in_: Optional[EvictRequestInput] = None
     ) -> EvictResponse:
-        """Evict a search request by search ID."""
+        """DEPRECATED: Does not do anything other than to return OK. No replacement necessary.."""
         endpoint = "alertsServiceEvict"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "in": prepare_input(in_),
             },
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,17 @@
     """SearchRequestInput."""
 
     cql_query: Optional[str] = field(
         default=None, metadata=config(field_name="cql_query")
     )
     offset: Optional[int] = field(default=None, metadata=config(field_name="offset"))
     limit: Optional[int] = field(default=None, metadata=config(field_name="limit"))
+    search_id: Optional[str] = field(
+        default=None, metadata=config(field_name="search_id")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class TimestampInput:
     """TimestampInput."""
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/mutations.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,7 +204,24 @@
                 "input": prepare_input(input_),
             },
             output=build_output_string(BulkOpPayloadV2),
         )
         if result.get(endpoint) is not None:
             return BulkOpPayloadV2.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation bulkReconnectNativeAssets")
+
+    def bulk_uninstall_native_assets(
+        self, input_: BulkUninstallNativeAssetsInput
+    ) -> BulkOpPayloadV2:
+        """None."""
+        endpoint = "bulkUninstallNativeAssets"
+
+        result = self.service.execute_mutation(
+            endpoint=endpoint,
+            variables={
+                "input": prepare_input(input_),
+            },
+            output=build_output_string(BulkOpPayloadV2),
+        )
+        if result.get(endpoint) is not None:
+            return BulkOpPayloadV2.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation bulkUninstallNativeAssets")
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,26 +292,45 @@
             },
             output=build_output_string(TaskInfoPayload),
         )
         if result.get(endpoint) is not None:
             return TaskInfoPayload.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query bulkReconnectNativeAssetsStatus")
 
+    def bulk_uninstall_native_assets_status(self, id_: str) -> TaskInfoPayload:
+        """Return the status of the bulkUninstallNativeAssets operation.."""
+        endpoint = "bulkUninstallNativeAssetsStatus"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "id": prepare_input(id_),
+            },
+            output=build_output_string(TaskInfoPayload),
+        )
+        if result.get(endpoint) is not None:
+            return TaskInfoPayload.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for query bulkUninstallNativeAssetsStatus")
+
     def asset_dead_period(self) -> str:
         """Return the tenant's asset dead period threshold used by the api. The value
         from the tenants preference api is used if present, otherwise the default of
         720h (30 days) is used.."""
         endpoint = "assetDeadPeriod"
 
         result = self.service.execute_query(endpoint=endpoint, variables={}, output="")
         if result.get(endpoint) is not None:
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for query assetDeadPeriod")
 
-    def subject_can_isolate(self) -> bool:
+    def subject_can_isolate(self) -> CanIsolateResponse:
         """Returns whether a subject can isolate an asset for the current tenant context."""
         endpoint = "subjectCanIsolate"
 
-        result = self.service.execute_query(endpoint=endpoint, variables={}, output="")
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={},
+            output=build_output_string(CanIsolateResponse),
+        )
         if result.get(endpoint) is not None:
-            return result.get(endpoint)
+            return CanIsolateResponse.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query subjectCanIsolate")
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,22 @@
     TAG_KEY_DESC = "tag_key_desc"
     TAG_VALUE_ASC = "tag_value_asc"
     TAG_VALUE_DESC = "tag_value_desc"
     TAG_ASC = "tag_asc"
     TAG_DESC = "tag_desc"
 
 
+class CanIsolateResponse(str, Enum):
+    """CanIsolateResponse."""
+
+    UNAUTHORIZED = "unauthorized"
+    AUTHORIZED = "authorized"
+    ALWAYS = "always"
+
+
 class BulkOpStatusV2(str, Enum):
     """BulkOpStatusV2."""
 
     TASK_STATE_PENDING = "TASK_STATE_PENDING"
     TASK_STATE_FAILED = "TASK_STATE_FAILED"
     TASK_STATE_COMPLETED = "TASK_STATE_COMPLETED"
     TASK_STATE_IN_PROGRESS = "TASK_STATE_IN_PROGRESS"
@@ -370,14 +378,29 @@
 class AssetWhereInputV2:
     """AssetWhereInputV2."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     connection_status: Optional[str] = field(
         default=None, metadata=config(field_name="connectionStatus")
     )
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt")
+    )
+    created_at_lt: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt_lt")
+    )
+    created_at_lte: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt_lte")
+    )
+    created_at_gt: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt_gt")
+    )
+    created_at_gte: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt_gte")
+    )
     group_name: Optional[str] = field(
         default=None, metadata=config(field_name="groupName")
     )
     group_name_contains: Optional[str] = field(
         default=None, metadata=config(field_name="groupName_contains")
     )
     host_id: Optional[str] = field(default=None, metadata=config(field_name="hostId"))
@@ -401,14 +424,29 @@
     )
     ip_address_contains: Optional[str] = field(
         default=None, metadata=config(field_name="ipAddress_contains")
     )
     isolation_status: Optional[str] = field(
         default=None, metadata=config(field_name="isolationStatus")
     )
+    last_seen_at: Optional[str] = field(
+        default=None, metadata=config(field_name="lastSeenAt")
+    )
+    last_seen_at_lt: Optional[str] = field(
+        default=None, metadata=config(field_name="lastSeenAt_lt")
+    )
+    last_seen_at_lte: Optional[str] = field(
+        default=None, metadata=config(field_name="lastSeenAt_lte")
+    )
+    last_seen_at_gt: Optional[str] = field(
+        default=None, metadata=config(field_name="lastSeenAt_gt")
+    )
+    last_seen_at_gte: Optional[str] = field(
+        default=None, metadata=config(field_name="lastSeenAt_gte")
+    )
     mac_address: Optional[str] = field(
         default=None, metadata=config(field_name="macAddress")
     )
     mac_address_contains: Optional[str] = field(
         default=None, metadata=config(field_name="macAddress_contains")
     )
     os_distributor: Optional[str] = field(
@@ -422,14 +460,29 @@
     )
     sensor_version: Optional[str] = field(
         default=None, metadata=config(field_name="sensorVersion")
     )
     system_type: Optional[str] = field(
         default=None, metadata=config(field_name="systemType")
     )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt")
+    )
+    updated_at_lt: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt_lt")
+    )
+    updated_at_lte: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt_lte")
+    )
+    updated_at_gt: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt_gt")
+    )
+    updated_at_gte: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt_gte")
+    )
     username: Optional[str] = field(
         default=None, metadata=config(field_name="username")
     )
     username_contains: Optional[str] = field(
         default=None, metadata=config(field_name="username_contains")
     )
     and_: Optional[List["AssetWhereInputV2"]] = field(
@@ -570,14 +623,25 @@
 
     reason: Optional[str] = field(default=None, metadata=config(field_name="reason"))
     where: Optional[AssetWhereInputV2] = field(
         default=None, metadata=config(field_name="where")
     )
 
 
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class BulkUninstallNativeAssetsInput:
+    """BulkUninstallNativeAssetsInput."""
+
+    reason: Optional[str] = field(default=None, metadata=config(field_name="reason"))
+    where: Optional[AssetWhereInputV2] = field(
+        default=None, metadata=config(field_name="where")
+    )
+
+
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AssetsV2:
     """AssetsV2."""
 
     total_count: Optional[int] = field(
         default=None, metadata=config(field_name="totalCount")
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 @dataclass(order=True, eq=True, frozen=True)
 class AuxiliaryEventsSearchInput:
     """AuxiliaryEventsSearchInput."""
 
     query: Optional[str] = field(default=None, metadata=config(field_name="query"))
     limit: Optional[int] = field(default=None, metadata=config(field_name="limit"))
     offset: Optional[int] = field(default=None, metadata=config(field_name="offset"))
+    search_id: Optional[str] = field(
+        default=None, metadata=config(field_name="search_id")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AsynchronousEventsSearchPrepInput:
     """AsynchronousEventsSearchPrepInput."""
 
@@ -115,10 +118,13 @@
 @dataclass(order=True, eq=True, frozen=True)
 class AuxiliaryEventsSearchResponse:
     """AuxiliaryEventsSearchResponse."""
 
     total_hits: Optional[int] = field(
         default=None, metadata=config(field_name="total_hits")
     )
+    search_id: Optional[str] = field(
+        default=None, metadata=config(field_name="search_id")
+    )
     events: Optional[List[AuxiliaryEvent]] = field(
         default=None, metadata=config(field_name="events")
     )
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1001,14 +1001,17 @@
         default=None, metadata=config(field_name="assets_count")
     )
     files_count: Optional[int] = field(
         default=None, metadata=config(field_name="files_count")
     )
     rn: Optional[str] = field(default=None, metadata=config(field_name="rn"))
     short_id: Optional[str] = field(default=None, metadata=config(field_name="shortId"))
+    close_reason: Optional[str] = field(
+        default=None, metadata=config(field_name="closeReason")
+    )
     genesis_alerts: Optional[List[Alert]] = field(
         default=None, metadata=config(field_name="genesis_alerts")
     )
     genesis_alerts2: Optional[List[Alert2]] = field(
         default=None, metadata=config(field_name="genesis_alerts2")
     )
     genesis_events: Optional[List[Event]] = field(
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -723,14 +723,17 @@
     )
     enabled_in_production: Optional[bool] = field(
         default=None, metadata=config(field_name="enabled_in_production")
     )
     enabled_in_pilot: Optional[bool] = field(
         default=None, metadata=config(field_name="enabled_in_pilot")
     )
+    post_disablement_complete: Optional[bool] = field(
+        default=None, metadata=config(field_name="post_disablement_complete")
+    )
     labels: Optional[List[TenantLabel]] = field(
         default=None, metadata=config(field_name="labels")
     )
     environments: Optional[List[Environment]] = field(
         default=None, metadata=config(field_name="environments")
     )
     services: Optional[List[Service]] = field(
@@ -828,14 +831,17 @@
     )
     is_partner: Optional[bool] = field(
         default=None, metadata=config(field_name="isPartner")
     )
     with_support: Optional[bool] = field(
         default=None, metadata=config(field_name="withSupport")
     )
+    with_pending_post_disablement: Optional[bool] = field(
+        default=None, metadata=config(field_name="withPendingPostDisablement")
+    )
     enabled_in_production: Optional[bool] = field(
         default=None, metadata=config(field_name="enabledInProduction")
     )
     enabled_in_pilot: Optional[bool] = field(
         default=None, metadata=config(field_name="enabledInPilot")
     )
     environment_filter: Optional[TenantEnvironmentFilter] = field(
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     LEGACY = "Legacy"
     API_ONLY = "ApiOnly"
 
 
 class ApiIntegrationStatus(str, Enum):
     """ApiIntegrationStatus."""
 
-    NEW = "New"
+    PROVISIONING = "Provisioning"
     ACTIVE = "Active"
     DISABLED = "Disabled"
     PAUSED = "Paused"
 
 
 class ApiIntegrationHealthStatus(str, Enum):
     """ApiIntegrationHealthStatus."""
@@ -64,14 +64,15 @@
     OPTION = "Option"
 
 
 class ApiFormItemValidatorType(str, Enum):
     """ApiFormItemValidatorType."""
 
     PATTERN = "Pattern"
+    JSON = "Json"
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class ApiIntegrationParameterInput:
     """ApiIntegrationParameterInput."""
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,14 +584,15 @@
     )
     updated_by: Optional[str] = field(
         default=None, metadata=config(field_name="updated_by")
     )
     last_login: Optional[str] = field(
         default=None, metadata=config(field_name="last_login")
     )
+    last_ip: Optional[str] = field(default=None, metadata=config(field_name="last_ip"))
     invited_date: Optional[str] = field(
         default=None, metadata=config(field_name="invited_date")
     )
     registered_date: Optional[str] = field(
         default=None, metadata=config(field_name="registered_date")
     )
     deactivated_date: Optional[str] = field(
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0a6/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,19 @@
 taegis_sdk_python/services/exports/subscriptions.py
 taegis_sdk_python/services/exports/types.py
 taegis_sdk_python/services/investigations/__init__.py
 taegis_sdk_python/services/investigations/mutations.py
 taegis_sdk_python/services/investigations/queries.py
 taegis_sdk_python/services/investigations/subscriptions.py
 taegis_sdk_python/services/investigations/types.py
+taegis_sdk_python/services/investigations2/__init__.py
+taegis_sdk_python/services/investigations2/mutations.py
+taegis_sdk_python/services/investigations2/queries.py
+taegis_sdk_python/services/investigations2/subscriptions.py
+taegis_sdk_python/services/investigations2/types.py
 taegis_sdk_python/services/mitre_attack_info/__init__.py
 taegis_sdk_python/services/mitre_attack_info/mutations.py
 taegis_sdk_python/services/mitre_attack_info/queries.py
 taegis_sdk_python/services/mitre_attack_info/subscriptions.py
 taegis_sdk_python/services/mitre_attack_info/types.py
 taegis_sdk_python/services/notebooks/__init__.py
 taegis_sdk_python/services/notebooks/mutations.py
```

