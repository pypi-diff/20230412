# Comparing `tmp/peek-core-device-3.3.3.tar.gz` & `tmp/peek-core-device-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-device-3.3.3.tar", last modified: Mon Nov 14 05:35:23 2022, max compression
+gzip compressed data, was "peek-core-device-3.4.0.tar", last modified: Wed Apr 12 11:04:09 2023, max compression
```

## Comparing `peek-core-device-3.3.3.tar` & `peek-core-device-3.4.0.tar`

### file list

```diff
@@ -1,215 +1,231 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.016507 peek-core-device-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      407 2022-11-14 05:35:23.016507 peek-core-device-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      138 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.006507 peek-core-device-3.3.3/peek_core_device/
--rw-r--r--   0 root         (0) root         (0)      466 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      692 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/peek_core_device/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.007507 peek-core-device-3.3.3/peek_core_device/_private/
--rw-r--r--   0 root         (0) root         (0)      224 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.007507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.007507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-cache-status/
--rw-r--r--   0 root         (0) root         (0)      578 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.html
--rw-r--r--   0 root         (0) root         (0)       33 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.scss
--rw-r--r--   0 root         (0) root         (0)     2057 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.007507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-info-table/
--rw-r--r--   0 root         (0) root         (0)     4088 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-info-table/device-info.component.html
--rw-r--r--   0 root         (0) root         (0)     4891 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.007507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-update-table/
--rw-r--r--   0 root         (0) root         (0)     1741 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-update-table/device-update.component.html
--rw-r--r--   0 root         (0) root         (0)     2504 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts
--rw-r--r--   0 root         (0) root         (0)     2986 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device.component.html
--rw-r--r--   0 root         (0) root         (0)      209 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device.component.ts
--rw-r--r--   0 root         (0) root         (0)     3125 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/device.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.008507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1502 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.008507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/loading/
--rw-r--r--   0 root         (0) root         (0)      302 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/loading/loading.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.008507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      510 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/tuples/DeviceCacheStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)     3219 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts
--rw-r--r--   0 root         (0) root         (0)      469 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/tuples/UpdateOfflineCacheSettingAction.ts
--rw-r--r--   0 root         (0) root         (0)       53 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/tuples/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.008507 peek-core-device-3.3.3/peek_core_device/_private/admin-app/upload-device-update/
--rw-r--r--   0 root         (0) root         (0)     3134 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html
--rw-r--r--   0 root         (0) root         (0)     4085 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.008507 peek-core-device-3.3.3/peek_core_device/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      318 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      524 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.009507 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1916 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py
--rw-r--r--   0 root         (0) root         (0)     1681 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py
--rw-r--r--   0 root         (0) root         (0)      895 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py
--rw-r--r--   0 root         (0) root         (0)      800 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1313 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)     1129 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4139 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.009507 peek-core-device-3.3.3/peek_core_device/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.009507 peek-core-device-3.3.3/peek_core_device/_private/both-app/connect/
--rw-r--r--   0 root         (0) root         (0)     3096 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/connect/connect.component.ts
--rw-r--r--   0 root         (0) root         (0)     2405 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/connect/connect.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.009507 peek-core-device-3.3.3/peek_core_device/_private/both-app/connecting/
--rw-r--r--   0 root         (0) root         (0)     1448 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/connecting/connecting.component.ts
--rw-r--r--   0 root         (0) root         (0)     1098 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/connecting/connecting.component.web.html
--rw-r--r--   0 root         (0) root         (0)      285 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/device.component.ts
--rw-r--r--   0 root         (0) root         (0)      471 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/device.component.web.html
--rw-r--r--   0 root         (0) root         (0)     2988 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/device.module.ts
--rw-r--r--   0 root         (0) root         (0)     1006 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/device.routes.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.009507 peek-core-device-3.3.3/peek_core_device/_private/both-app/enroll/
--rw-r--r--   0 root         (0) root         (0)     3897 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/enroll/enroll.component.ts
--rw-r--r--   0 root         (0) root         (0)     1295 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/enroll/enroll.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.009507 peek-core-device-3.3.3/peek_core_device/_private/both-app/enrolling/
--rw-r--r--   0 root         (0) root         (0)     1536 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/enrolling/enrolling.component.ts
--rw-r--r--   0 root         (0) root         (0)      582 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.009507 peek-core-device-3.3.3/peek_core_device/_private/both-app/loading/
--rw-r--r--   0 root         (0) root         (0)      537 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/loading/loading.component.ts
--rw-r--r--   0 root         (0) root         (0)      489 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-app/loading/loading.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.010507 peek-core-device-3.3.3/peek_core_device/_private/both-cfg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.010507 peek-core-device-3.3.3/peek_core_device/_private/both-cfg/connect/
--rw-r--r--   0 root         (0) root         (0)     2423 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-cfg/connect/connect.component.ts
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-cfg/connect/connect.component.web.html
--rw-r--r--   0 root         (0) root         (0)      930 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-cfg/core-device-cfg.component.ts
--rw-r--r--   0 root         (0) root         (0)      712 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-cfg/core-device-cfg.component.web.html
--rw-r--r--   0 root         (0) root         (0)     2798 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/both-cfg/core-device-cfg.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.010507 peek-core-device-3.3.3/peek_core_device/_private/client/
--rw-r--r--   0 root         (0) root         (0)     3296 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)     3946 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/client/DeviceOnlineHandler.py
--rw-r--r--   0 root         (0) root         (0)      527 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      496 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)     2175 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/client/UpdateDownloadHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.010507 peek-core-device-3.3.3/peek_core_device/_private/server/
--rw-r--r--   0 root         (0) root         (0)     4271 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/DeviceApi.py
--rw-r--r--   0 root         (0) root         (0)     5308 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      532 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     3520 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.010507 peek-core-device-3.3.3/peek_core_device/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     2170 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      318 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.011507 peek-core-device-3.3.3/peek_core_device/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     4101 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/DeviceStatusController.py
--rw-r--r--   0 root         (0) root         (0)     4352 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/EnrollmentController.py
--rw-r--r--   0 root         (0) root         (0)     4363 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/GpsController.py
--rw-r--r--   0 root         (0) root         (0)     3228 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     2999 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/NotifierController.py
--rw-r--r--   0 root         (0) root         (0)     3364 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/OfflineCacheController.py
--rw-r--r--   0 root         (0) root         (0)     5731 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/UpdateController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.011507 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1595 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1390 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceCacheStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1240 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1648 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2049 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2556 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2106 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.012507 peek-core-device-3.3.3/peek_core_device/_private/server/update_resources/
--rw-r--r--   0 root         (0) root         (0)     2350 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/server/update_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.012507 peek-core-device-3.3.3/peek_core_device/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      711 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     3324 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/storage/DeviceInfoTable.py
--rw-r--r--   0 root         (0) root         (0)     1431 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/storage/DeviceUpdateTuple.py
--rw-r--r--   0 root         (0) root         (0)     1005 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/storage/GpsLocationHistoryTable.py
--rw-r--r--   0 root         (0) root         (0)     1242 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/storage/GpsLocationTable.py
--rw-r--r--   0 root         (0) root         (0)     9027 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.013507 peek-core-device-3.3.3/peek_core_device/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      777 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py
--rw-r--r--   0 root         (0) root         (0)      506 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/ClientSettingsTuple.py
--rw-r--r--   0 root         (0) root         (0)      602 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py
--rw-r--r--   0 root         (0) root         (0)      414 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/DeviceBackgroundStateTupleAction.py
--rw-r--r--   0 root         (0) root         (0)      527 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/DeviceCacheStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      446 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/EnrolDeviceAction.py
--rw-r--r--   0 root         (0) root         (0)      515 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/OfflineCacheSettingTuple.py
--rw-r--r--   0 root         (0) root         (0)      673 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/OfflineCacheStatusAction.py
--rw-r--r--   0 root         (0) root         (0)      678 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/OfflineCacheStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      506 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateAppliedAction.py
--rw-r--r--   0 root         (0) root         (0)      590 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py
--rw-r--r--   0 root         (0) root         (0)      620 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py
--rw-r--r--   0 root         (0) root         (0)      587 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateEnrollmentAction.py
--rw-r--r--   0 root         (0) root         (0)      588 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py
--rw-r--r--   0 root         (0) root         (0)      637 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.013507 peek-core-device-3.3.3/peek_core_device/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.013507 peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)    64585 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png
--rw-r--r--   0 root         (0) root         (0)     1475 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)    62597 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/device_search.png
--rw-r--r--   0 root         (0) root         (0)    25072 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.013507 peek-core-device-3.3.3/peek_core_device/admin-doc/general_settings/
--rw-r--r--   0 root         (0) root         (0)    77281 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/general_settings/general_settings.png
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/general_settings/general_settings.rst
--rw-r--r--   0 root         (0) root         (0)      433 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      515 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.013507 peek-core-device-3.3.3/peek_core_device/both-doc/
--rw-r--r--   0 root         (0) root         (0)      848 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.014507 peek-core-device-3.3.3/peek_core_device/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      552 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2952 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/DeviceInfoTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.014507 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      333 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      852 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-background.service.ts
--rw-r--r--   0 root         (0) root         (0)     1180 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-nav.service.ts
--rw-r--r--   0 root         (0) root         (0)     1024 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-online.service.ts
--rw-r--r--   0 root         (0) root         (0)     7574 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-server.service.ts
--rw-r--r--   0 root         (0) root         (0)     2937 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-tuple.service.ts
--rw-r--r--   0 root         (0) root         (0)     5938 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-update.service.ts
--rw-r--r--   0 root         (0) root         (0)      592 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-update.service.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.015507 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/gps/
--rw-r--r--   0 root         (0) root         (0)      711 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)     6038 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.015507 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/hardware-info/
--rw-r--r--   0 root         (0) root         (0)     2318 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts
--rw-r--r--   0 root         (0) root         (0)       30 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/hardware-info/is-field.dweb.ts
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/hardware-info/is-field.mweb.ts
--rw-r--r--   0 root         (0) root         (0)     1180 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.015507 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      504 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/ClientSettingsTuple.ts
--rw-r--r--   0 root         (0) root         (0)      451 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/DeviceBackgroundStateTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)      662 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts
--rw-r--r--   0 root         (0) root         (0)      551 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      438 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/EnrolDeviceAction.ts
--rw-r--r--   0 root         (0) root         (0)      432 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/OfflineCacheSettingTuple.ts
--rw-r--r--   0 root         (0) root         (0)      530 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusAction.ts
--rw-r--r--   0 root         (0) root         (0)      470 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/UpdateAppliedAction.ts
--rw-r--r--   0 root         (0) root         (0)      641 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.016507 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/admin/
--rw-r--r--   0 root         (0) root         (0)      523 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts
--rw-r--r--   0 root         (0) root         (0)      467 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/admin/CreateDeviceUpdateAction.ts
--rw-r--r--   0 root         (0) root         (0)      572 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      455 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/admin/UpdateEnrollmentAction.ts
--rw-r--r--   0 root         (0) root         (0)     2337 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/device-enrolled.guard.ts
--rw-r--r--   0 root         (0) root         (0)     3687 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/device-enrolment.service.ts
--rw-r--r--   0 root         (0) root         (0)      767 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/device-loading.module.ts
--rw-r--r--   0 root         (0) root         (0)     8373 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/device-offline-cache.service.ts
--rw-r--r--   0 root         (0) root         (0)      904 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/device-status.service.ts
--rw-r--r--   0 root         (0) root         (0)      275 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/gps-location.service.ts
--rw-r--r--   0 root         (0) root         (0)      534 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)      301 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.016507 peek-core-device-3.3.3/peek_core_device/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)      605 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/plugin-module/tuples/OfflineCacheStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)     6026 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/peek_core_device/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.016507 peek-core-device-3.3.3/peek_core_device/server/
--rw-r--r--   0 root         (0) root         (0)     2404 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/server/DeviceApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.016507 peek-core-device-3.3.3/peek_core_device/tuples/
--rw-r--r--   0 root         (0) root         (0)     1312 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/tuples/DeviceDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)      494 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/tuples/DeviceGpsLocationTuple.py
--rw-r--r--   0 root         (0) root         (0)     1321 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/tuples/DeviceInfoTuple.py
--rw-r--r--   0 root         (0) root         (0)      814 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/tuples/DeviceStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-11-14 05:34:26.000000 peek-core-device-3.3.3/peek_core_device/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:23.007507 peek-core-device-3.3.3/peek_core_device.egg-info/
--rw-r--r--   0 root         (0) root         (0)      407 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/peek_core_device.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10517 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/peek_core_device.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/peek_core_device.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/peek_core_device.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/peek_core_device.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:35:23.017507 peek-core-device-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2547 2022-11-14 05:35:22.000000 peek-core-device-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.686215 peek-core-device-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-12 11:04:09.686215 peek-core-device-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.676216 peek-core-device-3.4.0/peek_core_device/
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/peek_core_device/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.676216 peek-core-device-3.4.0/peek_core_device/_private/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.676216 peek-core-device-3.4.0/peek_core_device/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-cache-status/
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.html
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-info-table/
+-rw-r--r--   0 root         (0) root         (0)     5597 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-info-table/device-info.component.html
+-rw-r--r--   0 root         (0) root         (0)     5442 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-update-table/
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-update-table/device-update.component.html
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device.component.html
+-rw-r--r--   0 root         (0) root         (0)      209 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device.component.ts
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/device.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/admin-app/loading/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/loading/loading.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      528 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/tuples/DeviceCacheStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts
+-rw-r--r--   0 root         (0) root         (0)      469 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/tuples/UpdateOfflineCacheSettingAction.ts
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/tuples/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/admin-app/upload-device-update/
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.677215 peek-core-device-3.4.0/peek_core_device/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.678215 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py
+-rw-r--r--   0 root         (0) root         (0)      810 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/97d44e5aeb18_add_lastbandwidthmetric.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.678215 peek-core-device-3.4.0/peek_core_device/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.678215 peek-core-device-3.4.0/peek_core_device/_private/both-app/connect/
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/connect/connect.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2405 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/connect/connect.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.678215 peek-core-device-3.4.0/peek_core_device/_private/both-app/connecting/
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/connecting/connecting.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/connecting/connecting.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/device.component.ts
+-rw-r--r--   0 root         (0) root         (0)      471 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/device.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/device.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/device.routes.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.679216 peek-core-device-3.4.0/peek_core_device/_private/both-app/enroll/
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/enroll/enroll.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/enroll/enroll.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.679216 peek-core-device-3.4.0/peek_core_device/_private/both-app/enrolling/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/enrolling/enrolling.component.ts
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.679216 peek-core-device-3.4.0/peek_core_device/_private/both-app/loading/
+-rw-r--r--   0 root         (0) root         (0)      537 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/loading/loading.component.ts
+-rw-r--r--   0 root         (0) root         (0)      489 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-app/loading/loading.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.679216 peek-core-device-3.4.0/peek_core_device/_private/both-cfg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.679216 peek-core-device-3.4.0/peek_core_device/_private/both-cfg/connect/
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-cfg/connect/connect.component.ts
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-cfg/connect/connect.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-cfg/core-device-cfg.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-cfg/core-device-cfg.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/both-cfg/core-device-cfg.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.679216 peek-core-device-3.4.0/peek_core_device/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     3629 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/UpdateDownloadHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.679216 peek-core-device-3.4.0/peek_core_device/_private/client/controllers/
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/controllers/BandwidthTestController.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/controllers/DeviceOnlineController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/client/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.680215 peek-core-device-3.4.0/peek_core_device/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/DeviceApi.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.680215 peek-core-device-3.4.0/peek_core_device/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.680215 peek-core-device-3.4.0/peek_core_device/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/BandwidthResultController.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/DeviceStatusController.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/EnrollmentController.py
+-rw-r--r--   0 root         (0) root         (0)     5391 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/GpsController.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/NotifierController.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/OfflineCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     5731 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/UpdateController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.681215 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     3001 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/OfflineCacheCombinedStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.681215 peek-core-device-3.4.0/peek_core_device/_private/server/update_resources/
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/server/update_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.681215 peek-core-device-3.4.0/peek_core_device/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/storage/DeviceInfoTable.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/storage/DeviceUpdateTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/storage/GpsLocationHistoryTable.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/storage/GpsLocationTable.py
+-rw-r--r--   0 root         (0) root         (0)     8668 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.682215 peek-core-device-3.4.0/peek_core_device/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py
+-rw-r--r--   0 root         (0) root         (0)      509 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/BandwidthTestResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      342 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/BandwidthTestTuple.py
+-rw-r--r--   0 root         (0) root         (0)      686 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/ClientSettingsTuple.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/DeviceBackgroundStateTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/DeviceCacheStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/EnrolDeviceAction.py
+-rw-r--r--   0 root         (0) root         (0)      847 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/OfflineCacheLoaderStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/OfflineCacheSettingTuple.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/OfflineCacheStatusAction.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/OfflineCacheStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      506 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateAppliedAction.py
+-rw-r--r--   0 root         (0) root         (0)      590 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py
+-rw-r--r--   0 root         (0) root         (0)      587 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateEnrollmentAction.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.682215 peek-core-device-3.4.0/peek_core_device/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.683215 peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)    64585 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    62597 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/device_search.png
+-rw-r--r--   0 root         (0) root         (0)    25072 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.683215 peek-core-device-3.4.0/peek_core_device/admin-doc/general_settings/
+-rw-r--r--   0 root         (0) root         (0)    41296 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/general_settings/general_settings.png
+-rw-r--r--   0 root         (0) root         (0)      875 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/general_settings/general_settings.rst
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.683215 peek-core-device-3.4.0/peek_core_device/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.683215 peek-core-device-3.4.0/peek_core_device/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/DeviceInfoTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.684215 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      333 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-background.service.ts
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-bandwidth-test.service.ts
+-rw-r--r--   0 root         (0) root         (0)      767 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-loading.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-nav.service.ts
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-online.service.ts
+-rw-r--r--   0 root         (0) root         (0)     7051 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-server.service.ts
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-tuple.service.ts
+-rw-r--r--   0 root         (0) root         (0)     5938 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-update.service.ts
+-rw-r--r--   0 root         (0) root         (0)      592 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-update.service.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.684215 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/gps/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.684215 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/hardware-info/
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/hardware-info/is-field.dweb.ts
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/hardware-info/is-field.mweb.ts
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.685215 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/BandwidthTestResultTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/BandwidthTestTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/ClientSettingsTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/DeviceBackgroundStateTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)      662 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      551 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/EnrolDeviceAction.ts
+-rw-r--r--   0 root         (0) root         (0)      670 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/OfflineCacheCombinedStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/OfflineCacheSettingTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      477 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusAction.ts
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/UpdateAppliedAction.ts
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.685215 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/admin/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts
+-rw-r--r--   0 root         (0) root         (0)      467 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/admin/CreateDeviceUpdateAction.ts
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/admin/UpdateEnrollmentAction.ts
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/server-info-tuple-defaults.ts
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/server-info-tuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/device-enrolled.guard.ts
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/device-enrolment.service.ts
+-rw-r--r--   0 root         (0) root         (0)    23425 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/device-offline-cache.service.ts
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/device-status.service.ts
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/gps-location.service.ts
+-rw-r--r--   0 root         (0) root         (0)      546 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)      301 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.685215 peek-core-device-3.4.0/peek_core_device/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/plugin-module/tuples/OfflineCacheLoaderStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     6342 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/peek_core_device/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.685215 peek-core-device-3.4.0/peek_core_device/server/
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/server/DeviceApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.686215 peek-core-device-3.4.0/peek_core_device/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/tuples/DeviceDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/tuples/DeviceGpsLocationTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/tuples/DeviceInfoTuple.py
+-rw-r--r--   0 root         (0) root         (0)      814 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/tuples/DeviceStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-04-12 11:03:17.000000 peek-core-device-3.4.0/peek_core_device/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:09.676216 peek-core-device-3.4.0/peek_core_device.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/peek_core_device.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11609 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/peek_core_device.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/peek_core_device.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/peek_core_device.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/peek_core_device.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:04:09.686215 peek-core-device-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2547 2023-04-12 11:04:09.000000 peek-core-device-3.4.0/setup.py
```

### Comparing `peek-core-device-3.3.3/peek_core_device/__init__.py` & `peek-core-device-3.4.0/peek_core_device/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import \
     PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import \
     PluginLogicEntryHookABC
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts`

 * *Files 23% similar despite different names*

```diff
@@ -6,27 +6,29 @@
     TupleActionPushService,
     TupleDataObserverService,
     TupleSelector,
 } from "@synerty/vortexjs";
 import { takeUntil } from "rxjs/operators";
 import { DatePipe } from "@angular/common";
 import { DeviceCacheStatusTuple } from "../tuples/DeviceCacheStatusTuple";
-import { OfflineCacheStatusTuple } from "@peek/peek_core_device/tuples/OfflineCacheStatusTuple";
+import { OfflineCacheLoaderStatusTuple } from "@peek/peek_core_device/tuples/OfflineCacheLoaderStatusTuple";
+import { OfflineCacheCombinedStatusTuple } from "@peek/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple";
 
 @Component({
     selector: "core-device-device-cache-status",
     styleUrls: ["./device-cache-status.component.scss"],
     templateUrl: "./device-cache-status.component.html",
     providers: [DatePipe],
 })
 export class DeviceCacheStatusComponent
     extends NgLifeCycleEvents
     implements OnInit
 {
-    readonly statusList$ = new BehaviorSubject<OfflineCacheStatusTuple[]>([]);
+    readonly combinedStatus$ =
+        new BehaviorSubject<OfflineCacheCombinedStatusTuple | null>(null);
 
     @Input()
     deviceToken$: BehaviorSubject<string>;
 
     private unsub = new Subject<void>();
 
     constructor(
@@ -38,22 +40,28 @@
     }
 
     ngOnInit() {
         this.deviceToken$
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((deviceToken: string) => {
                 this.unsub.next();
+                this.combinedStatus$.next(null);
 
                 this.tupleDataObserver // Setup a subscription for the device info data
                     .subscribeToTupleSelector(
-                        new TupleSelector(DeviceCacheStatusTuple.tupleName, {
-                            deviceToken: deviceToken,
-                        })
+                        new TupleSelector(
+                            OfflineCacheCombinedStatusTuple.tupleName,
+                            {
+                                deviceToken: deviceToken,
+                            }
+                        )
                     )
                     .pipe(takeUntil(this.onDestroyEvent))
                     .pipe(takeUntil(this.unsub))
-                    .subscribe((tuples: DeviceCacheStatusTuple[]) => {
-                        this.statusList$.next(tuples[0].statusList || []);
+                    .subscribe((tuples: OfflineCacheCombinedStatusTuple[]) => {
+                        if (tuples.length !== 0) {
+                            this.combinedStatus$.next(tuples[0]);
+                        }
                     });
             });
     }
 }
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-info-table/device-info.component.html` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-info-table/device-info.component.html`

 * *Files 20% similar despite different names*

```diff
@@ -3,37 +3,57 @@
         <nz-table #basicTable [nzData]="items$ | async">
             <thead>
                 <tr>
                     <th>Type</th>
                     <th>
                         Description
                         <nz-filter-trigger
-                            [(nzVisible)]="searchVisible"
-                            [nzActive]="searchValue.length > 0"
-                            [nzDropdownMenu]="menu"
+                            [(nzVisible)]="deviceSearchVisible"
+                            [nzActive]="deviceSearchValue.length > 0"
+                            [nzDropdownMenu]="deviceSearchMenu"
+                        >
+                            <i nz-icon nzType="search"></i>
+                        </nz-filter-trigger>
+                    </th>
+                    <th>
+                        Logged In User
+                        <nz-filter-trigger
+                            [(nzVisible)]="userSearchVisible"
+                            [nzActive]="userSearchValue.length > 0"
+                            [nzDropdownMenu]="userSearchMenu"
                         >
                             <i nz-icon nzType="search"></i>
                         </nz-filter-trigger>
                     </th>
                     <th>Last Online</th>
                     <th>Enrollment</th>
                     <th>Offline Cache</th>
+                    <th>Last Cache Check</th>
+                    <th
+                        nz-tooltip
+                        nzTooltipTitle="The round trip time in milliseconds for the device to request and download 100kb from Peek services."
+                    >
+                        Bandwidth Metric
+                    </th>
                     <th>Current Location</th>
                     <th></th>
                 </tr>
             </thead>
             <tbody>
                 <tr *ngFor="let item of basicTable.data">
                     <td>
                         {{ item.deviceType }}
                     </td>
                     <td>
                         {{ item.description }}
                     </td>
                     <td>
+                        {{ item.loggedInUser }}
+                    </td>
+                    <td>
                         <p>{{ deviceStatus(item) }}</p>
                     </td>
                     <td>
                         <nz-switch
                             [ngModel]="item.isEnrolled"
                             (ngModelChange)="toggleEnrollClicked(item)"
                         ></nz-switch>
@@ -53,15 +73,20 @@
                             nzTooltipTitle="Show Cache Status"
                             nz-button
                             (click)="handleShowOfflineCacheStatus(item)"
                         ></i>
                     </td>
                     <td>
                         <div *ngIf="item.lastCacheCheck != null">
-                            {{ item.lastCacheCheck | date: "medium" }}
+                            {{ item.lastCacheCheck | date : "medium" }}
+                        </div>
+                    </td>
+                    <td>
+                        <div *ngIf="item.lastBandwidthMetric != null">
+                            {{ item.lastBandwidthMetric }}
                         </div>
                     </td>
                     <td>
                         <div *ngIf="item.hasCurrentLocation()">
                             {{ item.currentLocation.latitude }},
                             {{ item.currentLocation.longitude }}
                             <br />
@@ -83,22 +108,35 @@
                     </td>
                 </tr>
             </tbody>
         </nz-table>
     </div>
 </div>
 
-<nz-dropdown-menu #menu="nzDropdownMenu">
+<nz-dropdown-menu #deviceSearchMenu="nzDropdownMenu">
+    <div class="ant-table-filter-dropdown">
+        <div class="search-box">
+            <input
+                type="text"
+                nz-input
+                placeholder="Search device name"
+                [(ngModel)]="deviceSearchValue"
+            />
+        </div>
+    </div>
+</nz-dropdown-menu>
+
+<nz-dropdown-menu #userSearchMenu="nzDropdownMenu">
     <div class="ant-table-filter-dropdown">
         <div class="search-box">
             <input
                 type="text"
                 nz-input
-                placeholder="Search name"
-                [(ngModel)]="searchValue"
+                placeholder="Search user name"
+                [(ngModel)]="userSearchValue"
             />
         </div>
     </div>
 </nz-dropdown-menu>
 
 <nz-modal
     [(nzVisible)]="isOfflineCacheModalShown"
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts`

 * *Files 24% similar despite different names*

```diff
@@ -26,16 +26,19 @@
 export class DeviceInfoComponent extends NgLifeCycleEvents {
     private items: DeviceInfoTable[] = [];
     readonly items$ = new BehaviorSubject<DeviceInfoTable[]>([]);
 
     readonly deviceToken$ = new BehaviorSubject<string | null>(null);
     isOfflineCacheModalShown: boolean = false;
 
-    private _searchValue: string = "";
-    searchVisible: boolean = false;
+    private _deviceSearchValue: string = "";
+    deviceSearchVisible: boolean = false;
+
+    private _userSearchValue: string = "";
+    userSearchVisible: boolean = false;
 
     constructor(
         private balloonMsg: BalloonMsgService,
         private actionService: TupleActionPushService,
         private tupleDataObserver: TupleDataObserverService,
         private datePipe: DatePipe
     ) {
@@ -49,35 +52,45 @@
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((tuples: DeviceInfoTable[]) => {
                 this.items = tuples;
                 this.refilter();
             });
     }
 
-    get searchValue(): string {
-        return this._searchValue;
+    get deviceSearchValue(): string {
+        return this._deviceSearchValue;
+    }
+
+    set deviceSearchValue(value: string) {
+        this._deviceSearchValue = (value || "").toLocaleLowerCase();
+        this.refilter();
+    }
+
+    get userSearchValue(): string {
+        return this._userSearchValue;
     }
 
-    set searchValue(value: string) {
-        this._searchValue = (value || "").toLocaleLowerCase();
+    set userSearchValue(value: string) {
+        this._userSearchValue = (value || "").toLocaleLowerCase();
         this.refilter();
     }
 
     private refilter(): void {
-        if (!this._searchValue) {
-            this.searchVisible = false;
-            this.items$.next(this.items);
-            return;
-        }
-        const items = this.items.filter(
-            (item: DeviceInfoTable) =>
-                item.description
-                    .toLocaleLowerCase()
-                    .indexOf(this._searchValue) !== -1
-        );
+        const filter = (item: DeviceInfoTable) => {
+            if (this.deviceSearchValue.length !== 0) {
+                const val = (item.description || "").toLocaleLowerCase();
+                if (val.indexOf(this.deviceSearchValue) === -1) return false;
+            }
+            if (this.userSearchValue.length !== 0) {
+                const val = (item.loggedInUser || "").toLocaleLowerCase();
+                if (val.indexOf(this.userSearchValue) === -1) return false;
+            }
+            return true;
+        };
+        const items = this.items.filter(filter);
         this.items$.next(items);
     }
 
     deviceStatus(device: DeviceInfoTable): string {
         if (
             device.deviceStatus & DeviceInfoTable.DEVICE_ONLINE &&
             !(device.deviceStatus & DeviceInfoTable.DEVICE_BACKGROUND)
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-update-table/device-update.component.html` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-update-table/device-update.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/device.component.html` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/device.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/device.module.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/device.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     lastUpdateCheck: Date;
     createdDate: Date;
     deviceStatus: number;
     isEnrolled: boolean;
     isOfflineCacheEnabled: boolean;
     currentLocation: DeviceGpsLocationTuple;
     lastCacheUpdate: Date;
+    lastBandwidthMetric: number;
+    loggedInUser: string;
 
     constructor() {
         super(DeviceInfoTable.tupleName);
     }
 
     get isWeb(): boolean {
         return !Capacitor.isNativePlatform();
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/script.py.mako` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py` & `peek-core-device-3.4.0/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/connect/connect.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/connect/connect.component.ts`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,25 @@
     DeviceNavService,
     DeviceServerService,
     DeviceTupleService,
     ServerInfoTuple,
 } from "@peek/peek_core_device/_private";
 import { DeviceTypeEnum } from "@peek/peek_core_device/_private/hardware-info/hardware-info";
 import { Capacitor } from "@capacitor/core";
+import { SERVER_INFO_TUPLE_DEFAULTS } from "@peek/peek_core_device/_private/tuples/server-info-tuple-defaults";
 
 @Component({
     selector: "core-device-enroll",
     templateUrl: "connect.component.web.html",
 })
 export class ConnectComponent extends NgLifeCycleEvents implements OnInit {
     server: ServerInfoTuple = new ServerInfoTuple();
-    httpPortStr: string = ServerInfoTuple.DEFAULT_HTTP_PORT.toString();
+    httpPortStr: string = SERVER_INFO_TUPLE_DEFAULTS.httpPort.toString();
     websocketPortStr: string =
-        ServerInfoTuple.DEFAULT_WEBSOCKET_PORT.toString();
+        SERVER_INFO_TUPLE_DEFAULTS.websocketPort.toString();
     deviceType: DeviceTypeEnum;
     isWeb: boolean;
     platform: string;
 
     constructor(
         private balloonMsg: BalloonMsgService,
         private headerService: HeaderService,
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/connect/connect.component.web.html` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/connect/connect.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/connecting/connecting.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/connecting/connecting.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/connecting/connecting.component.web.html` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/connecting/connecting.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/device.module.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/device.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/device.routes.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/device.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/enroll/enroll.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/enroll/enroll.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/enroll/enroll.component.web.html` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/enroll/enroll.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/enrolling/enrolling.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/enrolling/enrolling.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-app/loading/loading.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-app/loading/loading.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-cfg/connect/connect.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-cfg/connect/connect.component.ts`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 import { NgLifeCycleEvents } from "@synerty/vortexjs";
 import {
     DeviceServerService,
     DeviceTupleService,
     ServerInfoTuple,
 } from "@peek/peek_core_device/_private";
 import { DeviceTypeEnum } from "@peek/peek_core_device/_private/hardware-info/hardware-info";
+import { SERVER_INFO_TUPLE_DEFAULTS } from "@peek/peek_core_device/_private/tuples/server-info-tuple-defaults";
 
 @Component({
     selector: "peek-core-device-cfg-connect",
     templateUrl: "connect.component.web.html",
 })
 export class ConnectComponent extends NgLifeCycleEvents implements OnInit {
     server: ServerInfoTuple = new ServerInfoTuple();
-    httpPortStr: string = ServerInfoTuple.DEFAULT_HTTP_PORT.toString();
+    httpPortStr: string = SERVER_INFO_TUPLE_DEFAULTS.httpPort.toString();
     websocketPortStr: string =
-        ServerInfoTuple.DEFAULT_WEBSOCKET_PORT.toString();
+        SERVER_INFO_TUPLE_DEFAULTS.websocketPort.toString();
     deviceType: DeviceTypeEnum;
     isWeb: boolean;
 
     constructor(
         private balloonMsg: BalloonMsgService,
         private headerService: HeaderService,
         private tupleService: DeviceTupleService,
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-cfg/core-device-cfg.component.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-cfg/core-device-cfg.component.ts`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 import { Component } from "@angular/core";
 import { HeaderService } from "@synerty/peek-plugin-base-js";
 import { NgLifeCycleEvents } from "@synerty/vortexjs";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 import { DeviceTupleService } from "@peek/peek_core_device/_private";
 import { BehaviorSubject } from "rxjs";
+import { DatePipe } from "@angular/common";
+import { OfflineCacheStatusTuple } from "@peek/peek_core_device/_private/tuples/OfflineCacheStatusTuple";
+import {
+    BandwidthStatusI,
+    DeviceBandwidthTestService,
+} from "@peek/peek_core_device/_private/device-bandwidth-test.service";
 
 @Component({
     selector: "peek-core-device-cfg",
     templateUrl: "core-device-cfg.component.web.html",
+    providers: [DatePipe],
 })
 export class CoreDeviceCfgComponent extends NgLifeCycleEvents {
-    statusList$: BehaviorSubject<OfflineCacheStatusTuple[]>;
+    offlineLoaderList$: BehaviorSubject<OfflineCacheLoaderStatusTuple[]>;
+    offlineCacheStatus$: BehaviorSubject<OfflineCacheStatusTuple | null[]>;
+
+    bandwidthStatus$: BehaviorSubject<BandwidthStatusI>;
 
     constructor(
         private headerService: HeaderService,
         private tupleService: DeviceTupleService,
-        private cacheController: DeviceOfflineCacheService
+        private cacheController: DeviceOfflineCacheService,
+        public deviceBandwidthTestService: DeviceBandwidthTestService
     ) {
         super();
-        this.statusList$ = cacheController.cacheStatus$;
+        this.offlineLoaderList$ = cacheController.loaderStatus$;
+        this.offlineCacheStatus$ = cacheController.status$;
+        this.bandwidthStatus$ = deviceBandwidthTestService.status$;
 
         this.headerService.setTitle("Core Device Config");
     }
 }
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/both-cfg/core-device-cfg.module.ts` & `peek-core-device-3.4.0/peek_core_device/_private/both-cfg/core-device-cfg.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/client/ClientEntryHook.py` & `peek-core-device-3.4.0/peek_core_device/_private/client/ClientEntryHook.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 
 from twisted.internet.defer import inlineCallbacks
 
-from peek_core_device._private.client.DeviceOnlineHandler import (
-    DeviceOnlineHandler,
+from peek_core_device._private.client.controllers.DeviceOnlineController import (
+    DeviceOnlineController,
 )
 from peek_core_device._private.storage.DeclarativeBase import loadStorageTuples
 from peek_core_device._private.tuples import loadPrivateTuples
 from peek_core_device.tuples import loadPublicTuples
 from peek_plugin_base.client.PluginClientEntryHookABC import (
     PluginClientEntryHookABC,
 )
 from .DeviceTupleDataObservableProxy import makeDeviceTupleDataObservableProxy
 from .DeviceTupleProcessorActionProxy import makeTupleActionProcessorProxy
+from .controllers.BandwidthTestController import BandwidthTestController
 
 logger = logging.getLogger(__name__)
 
 
 class ClientEntryHook(PluginClientEntryHookABC):
     def __init__(self, *args, **kwargs):
         """ " Constructor"""
@@ -37,14 +38,15 @@
         loadStorageTuples()
 
         loadPrivateTuples()
         loadPublicTuples()
 
         logger.debug("Loaded")
 
+    @inlineCallbacks
     def start(self):
         """Load
 
         This will be called when the plugin is loaded, just after the db is migrated.
         Place any custom initialiastion steps here.
 
         """
@@ -67,15 +69,21 @@
 
         # ----------------
         # Data Observable Proxy
         self._loadedObjects.append(makeDeviceTupleDataObservableProxy())
 
         # ----------------
         # Online Handler
-        self._loadedObjects.append(DeviceOnlineHandler())
+        self._loadedObjects.append(DeviceOnlineController())
+
+        # ----------------
+        # Bandwidth Test Controller
+        bandwidthController = BandwidthTestController()
+        self._loadedObjects.append(bandwidthController)
+        yield bandwidthController.start()
 
         # # ----------------
         # # Update Download Handler
         # self._loadedObjects.append(
         #     UpdateDownloadHandler(self.platform.fileStorageDirectory,
         #                           self.platform.peekServerHost,
         #                           self.platform.peekServerHttpPort)
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/client/DeviceOnlineHandler.py` & `peek-core-device-3.4.0/peek_core_device/_private/client/controllers/DeviceOnlineController.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 deviceOnlineFilt.update(deviceFilt)
 
 
 # The sender is located at:
 # peek_core_device/plugin-module/_private/device-server.service.ts
 
 
-class DeviceOnlineHandler:
+class DeviceOnlineController:
     CHECK_TIME = 5.0
 
     def __init__(self):
         self._ep = PayloadEndpoint(deviceOnlineFilt, self._process)
         self._onlineDeviceIdsByUuid = {}
 
         self._loopingCall = LoopingCall(self._poll)
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py` & `peek-core-device-3.4.0/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/client/UpdateDownloadHandler.py` & `peek-core-device-3.4.0/peek_core_device/_private/client/UpdateDownloadHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/DeviceApi.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/DeviceApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/LogicEntryHook.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/LogicEntryHook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 
+from twisted.internet.defer import inlineCallbacks
 from txhttputil.site.FileUnderlayResource import FileUnderlayResource
 
 from peek_core_device._private.server.controller.NotifierController import (
     NotifierController,
 )
 from peek_core_device._private.server.update_resources.DeviceUpdateUploadResource import (
     DeviceUpdateUploadResource,
@@ -57,28 +58,31 @@
         self._deviceUpdatesPath.mkdir(parents=True, exist_ok=True)
 
         loadStorageTuples()
         loadPrivateTuples()
         loadPublicTuples()
         logger.debug("Loaded")
 
+    @inlineCallbacks
     def start(self):
         """Start
 
         This will be called when the plugin is loaded, just after the db is migrated.
         Place any custom initialiastion steps here.
 
         """
+        userApi = self.platform.getOtherPluginApi("peek_core_user")
+
         offlineCacheController = OfflineCacheController(
-            dbSessionCreator=self.dbSessionCreator,
+            dbSessionCreator=self.dbSessionCreator
         )
         self._loadedObjects.append(offlineCacheController)
 
         tupleObservable = makeTupleDataObservableHandler(
-            self.dbSessionCreator, offlineCacheController
+            self.dbSessionCreator, offlineCacheController, userApi
         )
         self._loadedObjects.append(tupleObservable)
 
         notifierController = NotifierController(tupleObservable=tupleObservable)
         self._loadedObjects.append(notifierController)
 
         offlineCacheController.setNotificationController(notifierController)
@@ -118,14 +122,16 @@
 
         # Initialise the API object that will be shared with other plugins
         self._api = DeviceApi(mainController, self.dbSessionCreator)
         self._loadedObjects.append(self._api)
 
         notifierController.setApi(self._api)
 
+        yield mainController.start()
+
         logger.debug("Started")
 
     def stop(self):
         """Stop
 
         This method is called by the platform to tell the peek app to shutdown and stop
         everything it's doing
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/TupleActionProcessor.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/TupleDataObservable.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/TupleDataObservable.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,59 +4,63 @@
 from peek_core_device._private.PluginNames import deviceObservableName
 from peek_core_device._private.server.controller.OfflineCacheController import (
     OfflineCacheController,
 )
 from peek_core_device._private.server.tuple_providers.ClientSettingsTupleProvider import (
     ClientSettingsTupleProvider,
 )
-from peek_core_device._private.server.tuple_providers.DeviceCacheStatusTupleProvider import (
-    DeviceCacheStatusTupleProvider,
-)
 from peek_core_device._private.server.tuple_providers.DeviceGpsLocationTupleProvider import (
     DeviceGpsLocationTupleProvider,
 )
 from peek_core_device._private.server.tuple_providers.DeviceInfoTableTupleProvider import (
     DeviceInfoTableTupleProvider,
 )
 from peek_core_device._private.server.tuple_providers.DeviceInfoTupleProvider import (
     DeviceInfoTupleProvider,
 )
 from peek_core_device._private.server.tuple_providers.DeviceUpdateTupleProvider import (
     DeviceUpdateTupleProvider,
 )
+from peek_core_device._private.server.tuple_providers.OfflineCacheCombinedStatusTupleProvider import (
+    OfflineCacheCombinedStatusTupleProvider,
+)
 from peek_core_device._private.server.tuple_providers.OfflineCacheSettingTupleProvider import (
     OfflineCacheSettingTupleProvider,
 )
 from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
 from peek_core_device._private.storage.DeviceUpdateTuple import (
     DeviceUpdateTuple,
 )
 from peek_core_device._private.tuples.ClientSettingsTuple import (
     ClientSettingsTuple,
 )
 from peek_core_device._private.tuples.DeviceCacheStatusTuple import (
     DeviceCacheStatusTuple,
 )
+from peek_core_device._private.tuples.OfflineCacheCombinedStatusTuple import (
+    OfflineCacheCombinedStatusTuple,
+)
 from peek_core_device._private.tuples.OfflineCacheSettingTuple import (
     OfflineCacheSettingTuple,
 )
 from peek_core_device.tuples.DeviceGpsLocationTuple import (
     DeviceGpsLocationTuple,
 )
 from peek_core_device.tuples.DeviceInfoTuple import DeviceInfoTuple
 
 
 def makeTupleDataObservableHandler(
-    ormSessionCreator, offlineCacheController: OfflineCacheController
+    ormSessionCreator, offlineCacheController: OfflineCacheController, userApi
 ):
     """ " Make Tuple Data Observable Handler
 
     This method creates the observable object, registers the tuple providers and then
     returns it.
 
+    :param userApi:
     :param ormSessionCreator: A function that returns a SQLAlchemy session when called
     :param offlineCacheController:
 
     :return: An instance of :code:`TupleDataObservableHandler`
 
     """
     tupleObservable = TupleDataObservableHandler(
@@ -67,25 +71,29 @@
     tupleObservable.addTupleProvider(
         DeviceUpdateTuple.tupleName(),
         DeviceUpdateTupleProvider(ormSessionCreator),
     )
 
     tupleObservable.addTupleProvider(
         DeviceInfoTuple.tupleName(),
-        DeviceInfoTupleProvider(ormSessionCreator, offlineCacheController),
+        DeviceInfoTupleProvider(
+            ormSessionCreator, offlineCacheController, userApi
+        ),
     )
 
     tupleObservable.addTupleProvider(
-        DeviceCacheStatusTuple.tupleName(),
-        DeviceCacheStatusTupleProvider(offlineCacheController),
+        OfflineCacheCombinedStatusTuple.tupleName(),
+        OfflineCacheCombinedStatusTupleProvider(offlineCacheController),
     )
 
     tupleObservable.addTupleProvider(
         DeviceInfoTable.tupleName(),
-        DeviceInfoTableTupleProvider(ormSessionCreator),
+        DeviceInfoTableTupleProvider(
+            ormSessionCreator, offlineCacheController, userApi
+        ),
     )
 
     tupleObservable.addTupleProvider(
         ClientSettingsTuple.tupleName(),
         ClientSettingsTupleProvider(ormSessionCreator),
     )
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/controller/DeviceStatusController.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/controller/DeviceStatusController.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import List
 
 from sqlalchemy.orm.exc import NoResultFound
 from twisted.internet.defer import Deferred
+from twisted.internet.defer import inlineCallbacks
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Tuple import Tuple
 from vortex.TupleAction import TupleActionABC
 
 from peek_core_device._private.server.controller.NotifierController import (
     NotifierController,
 )
@@ -19,19 +20,23 @@
 )
 from peek_core_device.tuples.DeviceInfoTuple import DeviceInfoTuple
 
 logger = logging.getLogger(__name__)
 
 
 class DeviceStatusController:
-    def __init__(self, dbSessionCreator, notifierController: NotifierController):
+    def __init__(
+        self, dbSessionCreator, notifierController: NotifierController
+    ):
         self._dbSessionCreator = dbSessionCreator
         self._notifierController = notifierController
 
-        self._setAllDevicesOfflineBlocking()
+    @inlineCallbacks
+    def start(self):
+        yield self._setAllDevicesOffline()
 
     def shutdown(self):
         pass
 
     def processTupleAction(self, tupleAction: TupleActionABC) -> List[Tuple]:
         if isinstance(tupleAction, UpdateDeviceOnlineAction):
             return self._processUpdateOnline(tupleAction)
@@ -67,27 +72,31 @@
             if action.deviceBackgrounded:
                 deviceInfo.deviceStatus |= DeviceInfoTuple.DEVICE_BACKGROUND
 
             session.commit()
 
             self._notifierController.notifyDeviceInfo(deviceId=deviceId)
             self._notifierController.notifyDeviceOnline(
-                deviceInfo.deviceId, deviceInfo.deviceToken, deviceInfo.deviceStatus
+                deviceInfo.deviceId,
+                deviceInfo.deviceToken,
+                deviceInfo.deviceStatus,
             )
 
             return []
 
         except NoResultFound:
             return []
 
         finally:
             session.close()
 
     @deferToThreadWrapWithLogger(logger)
-    def _processUpdateOnline(self, action: UpdateDeviceOnlineAction) -> List[Tuple]:
+    def _processUpdateOnline(
+        self, action: UpdateDeviceOnlineAction
+    ) -> List[Tuple]:
         """Process Online Status Update
 
         :rtype: Deferred
         """
         session = self._dbSessionCreator()
         try:
             deviceInfo = (
@@ -101,26 +110,29 @@
             deviceInfo.lastOnline = action.dateTime
             deviceInfo.deviceStatus = action.deviceStatus
 
             session.commit()
 
             self._notifierController.notifyDeviceInfo(deviceId=deviceId)
             self._notifierController.notifyDeviceOnline(
-                deviceInfo.deviceId, deviceInfo.deviceToken, deviceInfo.deviceStatus
+                deviceInfo.deviceId,
+                deviceInfo.deviceToken,
+                deviceInfo.deviceStatus,
             )
 
             return []
 
         except NoResultFound:
             return []
 
         finally:
             session.close()
 
-    def _setAllDevicesOfflineBlocking(self):
+    @deferToThreadWrapWithLogger(logger)
+    def _setAllDevicesOffline(self):
         """Set All Devices to Offline"""
         session = self._dbSessionCreator()
         try:
             session.execute(
                 DeviceInfoTable.__table__.update().values(
                     deviceStatus=DeviceInfoTuple.DEVICE_OFFLINE
                 )
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/controller/EnrollmentController.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/controller/EnrollmentController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/controller/MainController.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/controller/MainController.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 from twisted.internet.defer import Deferred
 from twisted.internet.defer import inlineCallbacks
 from vortex.TupleAction import TupleActionABC
 from vortex.handler.TupleActionProcessor import TupleActionProcessorDelegateABC
 from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
 
+from peek_core_device._private.server.controller.BandwidthResultController import (
+    BandwidthResultController,
+)
 from peek_core_device._private.server.controller.EnrollmentController import (
     EnrollmentController,
 )
 from peek_core_device._private.server.controller.GpsController import (
     GpsController,
 )
 from peek_core_device._private.server.controller.NotifierController import (
@@ -49,31 +52,42 @@
             dbSessionCreator, notifierController
         )
 
         self._updateController = UpdateController(
             dbSessionCreator, notifierController, deviceUpdateFilePath
         )
 
+        self._bandwidthResultController = BandwidthResultController(
+            dbSessionCreator, notifierController
+        )
+
         self._gpsController = GpsController(
             dbSessionCreator=dbSessionCreator,
             tupleObservable=tupleObservable,
             notifierController=notifierController,
         )
 
         self._offlineCacheController = offlineCacheController
 
     @property
     def deviceUpdateController(self):
         return self._updateController
 
+    @inlineCallbacks
+    def start(self):
+        yield self._onlineController.start()
+        yield self._bandwidthResultController.start()
+        yield self._gpsController.start()
+
     def shutdown(self):
         self._enrollmentController.shutdown()
         self._onlineController.shutdown()
         self._updateController.shutdown()
         self._gpsController.shutdown()
+        self._bandwidthResultController.shutdown()
 
     @inlineCallbacks
     def processTupleAction(self, tupleAction: TupleActionABC) -> Deferred:
         result = yield self._enrollmentController.processTupleAction(
             tupleAction
         )
         if result is not None:
@@ -93,8 +107,16 @@
 
         result = yield self._offlineCacheController.processTupleAction(
             tupleAction
         )
         if result is not None:
             return result
 
+        # At this point, someone needs to create an array and iterate over
+        # the controllers.
+        result = yield self._bandwidthResultController.processTupleAction(
+            tupleAction
+        )
+        if result is not None:
+            return result
+
         raise NotImplementedError(tupleAction.tupleName())
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/controller/NotifierController.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/controller/NotifierController.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from datetime import datetime
 
 from vortex.DeferUtil import callMethodLater
 from vortex.TupleSelector import TupleSelector
+from vortex.VortexUtil import debounceCall
 from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
 
 from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
 from peek_core_device._private.storage.DeviceUpdateTuple import (
     DeviceUpdateTuple,
 )
 from peek_core_device._private.tuples.OfflineCacheSettingTuple import (
@@ -34,14 +35,18 @@
 
     @callMethodLater
     def notifyDeviceInfo(self, deviceId: str):
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(DeviceInfoTuple.tupleName(), dict(deviceId=deviceId))
         )
 
+        self.notifyAllDeviceInfos()
+
+    @debounceCall(55)
+    def notifyAllDeviceInfos(self):
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(DeviceInfoTuple.tupleName(), dict())
         )
 
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(DeviceInfoTable.tupleName(), dict())
         )
@@ -50,14 +55,18 @@
     def notifyDeviceUpdate(self, deviceType: str):
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(
                 DeviceUpdateTuple.tupleName(), dict(deviceType=deviceType)
             )
         )
 
+        self.notifyAllDeviceUpdate()
+
+    @debounceCall(30)
+    def notifyAllDeviceUpdate(self):
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(DeviceUpdateTuple.tupleName(), dict())
         )
 
     @callMethodLater
     def notifyDeviceOnline(self, deviceId: str, deviceToken: str, online: bool):
         """Notify Device Online
@@ -71,34 +80,29 @@
     def notifyDeviceGpsLocation(
         self,
         deviceToken: str,
         latitude: float,
         longitude: float,
         updatedDate: datetime,
     ):
+        self._api.notifyCurrentGpsLocation(
+            deviceToken, latitude, longitude, updatedDate
+        )
 
+    @debounceCall(120)
+    def notifyAllDeviceGpsLocation(self):
         from peek_core_device._private.storage.GpsLocationTable import (
             GpsLocationTable,
         )
 
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(GpsLocationTable.tupleName(), dict())
         )
 
-        self._api.notifyCurrentGpsLocation(
-            deviceToken,
-            latitude,
-            longitude,
-            updatedDate,
-        )
-
     @callMethodLater
-    def notifyDeviceOfflineCacheSetting(
-        self,
-        deviceToken: str,
-    ):
+    def notifyDeviceOfflineCacheSetting(self, deviceToken: str):
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(
                 OfflineCacheSettingTuple.tupleName(),
                 dict(deviceToken=deviceToken),
             )
         )
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/controller/OfflineCacheController.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/controller/OfflineCacheController.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,63 +2,69 @@
 from collections import defaultdict
 from datetime import datetime
 from typing import List
 from typing import Optional
 
 from twisted.internet.defer import Deferred
 from vortex.DeferUtil import deferToThreadWrapWithLogger
+from vortex.DeferUtil import vortexLogFailure
 from vortex.Tuple import Tuple
 from vortex.TupleAction import TupleActionABC
 
 from peek_core_device._private.server.controller.NotifierController import (
     NotifierController,
 )
 from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
+from peek_core_device._private.tuples.OfflineCacheCombinedStatusTuple import (
+    OfflineCacheCombinedStatusTuple,
+)
 from peek_core_device._private.tuples.OfflineCacheStatusAction import (
     OfflineCacheStatusAction,
 )
-from peek_core_device._private.tuples.OfflineCacheStatusTuple import (
-    OfflineCacheStatusTuple,
+from peek_core_device._private.tuples.OfflineCacheLoaderStatusTuple import (
+    OfflineCacheLoaderStatusTuple,
 )
 from peek_core_device._private.tuples.UpdateOfflineCacheSettingAction import (
     UpdateOfflineCacheSettingAction,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class OfflineCacheController:
     def __init__(self, dbSessionCreator):
         self._dbSessionCreator = dbSessionCreator
         self._notifierController = None
 
         self._lastUpdateByDeviceToken = {}
-        self._lastStatusByDeviceToken = defaultdict(list)
+        self._lastStatusEncodedPayloadByDeviceToken: dict[str, str] = {}
 
     def setNotificationController(self, notifierController: NotifierController):
         self._notifierController = notifierController
 
     def lastCacheUpdate(self, deviceToken: str) -> Optional[datetime]:
         return self._lastUpdateByDeviceToken.get(deviceToken)
 
-    def lastCacheStatus(
-        self, deviceToken: str
-    ) -> dict[str : list[OfflineCacheStatusTuple]]:
-        return self._lastStatusByDeviceToken.get(deviceToken)
+    def lastCacheStatusEncodedPayload(self, deviceToken: str) -> str:
+        return self._lastStatusEncodedPayloadByDeviceToken.get(deviceToken)
 
     def shutdown(self):
         self._lastUpdateByDeviceToken = {}
 
     def processTupleAction(self, tupleAction: TupleActionABC) -> List[Tuple]:
 
         if isinstance(tupleAction, UpdateOfflineCacheSettingAction):
-            return self._processOfflineCacheSettingUpdate(tupleAction)
+            d = self._processOfflineCacheSettingUpdate(tupleAction)
+            d.addErrback(vortexLogFailure, logger)
+            return []
 
         if isinstance(tupleAction, OfflineCacheStatusAction):
-            return self._processOfflineCacheStatusUpdate(tupleAction)
+            d = self._processOfflineCacheStatusUpdate(tupleAction)
+            d.addErrback(vortexLogFailure, logger)
+            return []
 
     @deferToThreadWrapWithLogger(logger)
     def _processOfflineCacheSettingUpdate(
         self, action: UpdateOfflineCacheSettingAction
     ) -> List[Tuple]:
         """Process Offline Cache Update
 
@@ -78,23 +84,23 @@
 
             ormSession.commit()
 
             self._notifierController.notifyDeviceOfflineCacheSetting(
                 deviceToken=deviceInfo.deviceToken
             )
 
-            return []
-
         finally:
             # Always close the session after we create it
             ormSession.close()
 
     @deferToThreadWrapWithLogger(logger)
     def _processOfflineCacheStatusUpdate(
         self, action: OfflineCacheStatusAction
     ) -> List[Tuple]:
-        lastDate = min([s.lastCheckDate for s in action.cacheStatusList])
-        self._lastUpdateByDeviceToken[action.deviceToken] = lastDate
-        self._lastStatusByDeviceToken[
+        # lastDate = min([s.lastCheckDate for s in action.loaderStatusList])
+        self._lastUpdateByDeviceToken[
+            action.deviceToken
+        ] = action.lastCachingStartDate
+
+        self._lastStatusEncodedPayloadByDeviceToken[
             action.deviceToken
-        ] = action.cacheStatusList
-        return []
+        ] = action.encodedCombinedTuplePayload
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/controller/UpdateController.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/controller/UpdateController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,27 @@
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
 from peek_core_device._private.storage.Setting import FIELD_ENROLLMENT_ENABLED
 from peek_core_device._private.storage.Setting import OFFICE_ENROLLMENT_ENABLED
+from peek_core_device._private.storage.Setting import (
+    OFFLINE_CACHE_REFRESH_SECONDS,
+)
+from peek_core_device._private.storage.Setting import (
+    OFFLINE_MASTER_SWITCH_ENABLED,
+)
+from peek_core_device._private.storage.Setting import (
+    SLOW_NETWORK_BANDWIDTH_METRIC_THRESHOLD,
+)
 from peek_core_device._private.storage.Setting import globalSetting
-from peek_core_device._private.tuples.ClientSettingsTuple import \
-    ClientSettingsTuple
+from peek_core_device._private.tuples.ClientSettingsTuple import (
+    ClientSettingsTuple,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class ClientSettingsTupleProvider(TuplesProviderABC):
     def __init__(self, ormSessionCreator):
         self._ormSessionCreator = ormSessionCreator
@@ -33,16 +43,28 @@
                 ormSession, FIELD_ENROLLMENT_ENABLED
             )
 
             clientSetting.officeEnrollmentEnabled = globalSetting(
                 ormSession, OFFICE_ENROLLMENT_ENABLED
             )
 
+            clientSetting.slowNetworkBandwidthMetricThreshold = globalSetting(
+                ormSession, SLOW_NETWORK_BANDWIDTH_METRIC_THRESHOLD
+            )
+
+            clientSetting.offlineCacheSyncSeconds = globalSetting(
+                ormSession, OFFLINE_CACHE_REFRESH_SECONDS
+            )
+
+            clientSetting.offlineMasterSwitchEnabled = globalSetting(
+                ormSession, OFFLINE_MASTER_SWITCH_ENABLED
+            )
+
             # Create the vortex message
             return (
                 Payload(filt, tuples=[clientSetting])
-                    .makePayloadEnvelope()
-                    .toVortexMsg()
+                .makePayloadEnvelope()
+                .toVortexMsg()
             )
 
         finally:
             ormSession.close()
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceCacheStatusTupleProvider.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/OfflineCacheCombinedStatusTupleProvider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import logging
 from typing import Union
 
-from peek_core_device._private.server.controller.OfflineCacheController import (
-    OfflineCacheController,
-)
-from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
-from peek_core_device._private.storage.GpsLocationTable import GpsLocationTable
 from twisted.internet.defer import Deferred
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
+from vortex.PayloadEnvelope import PayloadEnvelope
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
+from peek_core_device._private.server.controller.OfflineCacheController import (
+    OfflineCacheController,
+)
 from peek_core_device._private.tuples.DeviceCacheStatusTuple import (
     DeviceCacheStatusTuple,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class DeviceCacheStatusTupleProvider(TuplesProviderABC):
+class OfflineCacheCombinedStatusTupleProvider(TuplesProviderABC):
     def __init__(self, offlineCacheController: OfflineCacheController):
         self._offlineCacheController = offlineCacheController
 
     @deferToThreadWrapWithLogger(logger)
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
 
         deviceToken = tupleSelector.selector.get("deviceToken")
 
-        tuple_ = DeviceCacheStatusTuple(
-            statusList=self._offlineCacheController.lastCacheStatus(deviceToken)
+        encodedPayload = DeviceCacheStatusTuple(
+            statusList=self._offlineCacheController.lastCacheStatusEncodedPayload(
+                deviceToken
+            )
         )
+
         # Create the vortex message
-        return (
-            Payload(filt, tuples=[tuple_]).makePayloadEnvelope().toVortexMsg()
-        )
+        return PayloadEnvelope(
+            filt=filt, encodedPayload=encodedPayload
+        ).toVortexMsg()
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,88 @@
 import logging
 from typing import Union
 
+from twisted.internet.defer import inlineCallbacks
+
+from peek_core_device._private.server.controller.OfflineCacheController import (
+    OfflineCacheController,
+)
 from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
 from peek_core_device._private.storage.GpsLocationTable import GpsLocationTable
 from twisted.internet.defer import Deferred
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
+
 logger = logging.getLogger(__name__)
 
 
-class DeviceInfoTableTupleProvider(TuplesProviderABC):
-    def __init__(self, ormSessionCreator):
+class DeviceInfoTupleProvider(TuplesProviderABC):
+    def __init__(
+        self,
+        ormSessionCreator,
+        offlineCacheController: OfflineCacheController,
+        userApi,
+    ):
+
+        from peek_core_user.server.UserApiABC import UserApiABC
+
         self._ormSessionCreator = ormSessionCreator
+        self._offlineCacheController = offlineCacheController
+        self._userApi: UserApiABC = userApi
 
-    @deferToThreadWrapWithLogger(logger)
+    @inlineCallbacks
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
+        from peek_core_user.tuples.UserLoggedInInfoTuple import (
+            UserLoggedInInfoTuple,
+        )
+
+        loggedInUsers: list[
+            UserLoggedInInfoTuple
+        ] = yield self._userApi.infoApi.userLoggedInInfo()
+
+        return (
+            yield self._makeVortexMsgDeferred(
+                filt, tupleSelector, loggedInUsers
+            )
+        )
 
+    @deferToThreadWrapWithLogger(logger)
+    def _makeVortexMsgDeferred(
+        self, filt: dict, tupleSelector: TupleSelector, loggedInUsers
+    ) -> Union[Deferred, bytes]:
         deviceId = tupleSelector.selector.get("deviceId")
+        userByDeviceToken = {o.deviceToken: o.userName for o in loggedInUsers}
 
         ormSession = self._ormSessionCreator()
         try:
             query = ormSession.query(
                 DeviceInfoTable, GpsLocationTable
             ).outerjoin(GpsLocationTable)
 
             if deviceId is not None:
                 query = query.filter(DeviceInfoTable.deviceId == deviceId)
 
-            # Add the current location to each DeviceInfo row
             tuples = []
             for deviceInfoTableRow, gpsLocationTableRow in query.all():
-                deviceInfoTableRow.currentLocation = gpsLocationTableRow
-                tuples.append(deviceInfoTableRow)
+                tuples.append(
+                    deviceInfoTableRow.toTuple(
+                        currentLocationTuple=gpsLocationTableRow,
+                        lastCacheCheck=self._offlineCacheController.lastCacheUpdate(
+                            deviceInfoTableRow.deviceToken
+                        ),
+                        loggedInUser=userByDeviceToken.get(
+                            deviceInfoTableRow.deviceToken
+                        ),
+                    )
+                )
 
             # Create the vortex message
             return (
                 Payload(filt, tuples=tuples).makePayloadEnvelope().toVortexMsg()
             )
 
         finally:
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 import logging
 from typing import Union
 
-from peek_core_device._private.server.controller.OfflineCacheController import (
-    OfflineCacheController,
-)
-from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
-from peek_core_device._private.storage.GpsLocationTable import GpsLocationTable
+import sqlalchemy
 from twisted.internet.defer import Deferred
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
+from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
+from peek_core_device._private.tuples.OfflineCacheSettingTuple import (
+    OfflineCacheSettingTuple,
+)
+
 logger = logging.getLogger(__name__)
 
 
-class DeviceInfoTupleProvider(TuplesProviderABC):
-    def __init__(
-        self, ormSessionCreator, offlineCacheController: OfflineCacheController
-    ):
+class OfflineCacheSettingTupleProvider(TuplesProviderABC):
+    def __init__(self, ormSessionCreator):
         self._ormSessionCreator = ormSessionCreator
-        self._offlineCacheController = offlineCacheController
 
     @deferToThreadWrapWithLogger(logger)
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
 
-        deviceId = tupleSelector.selector.get("deviceId")
+        deviceToken = tupleSelector.selector.get("deviceToken")
 
         ormSession = self._ormSessionCreator()
         try:
-            query = ormSession.query(
-                DeviceInfoTable, GpsLocationTable
-            ).outerjoin(GpsLocationTable)
-
-            if deviceId is not None:
-                query = query.filter(DeviceInfoTable.deviceId == deviceId)
-
-            tuples = []
-            for deviceInfoTableRow, gpsLocationTableRow in query.all():
-                tuples.append(
-                    deviceInfoTableRow.toTuple(
-                        currentLocationTuple=gpsLocationTableRow,
-                        lastCacheCheck=self._offlineCacheController.lastCacheUpdate(
-                            deviceInfoTableRow.deviceToken
-                        ),
-                    )
+            try:
+                deviceTuple = (
+                    ormSession.query(DeviceInfoTable)
+                    .filter(DeviceInfoTable.deviceToken == deviceToken)
+                    .one()
+                )
+
+            except sqlalchemy.orm.exc.NoResultFound:
+                deviceTuple = DeviceInfoTable(isOfflineCacheEnabled=False)
+
+            tuples = [
+                OfflineCacheSettingTuple(
+                    offlineEnabled=deviceTuple.isOfflineCacheEnabled
                 )
+            ]
 
             # Create the vortex message
             return (
                 Payload(filt, tuples=tuples).makePayloadEnvelope().toVortexMsg()
             )
 
         finally:
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,89 @@
 import logging
 from typing import Union
 
-import sqlalchemy
+from sqlalchemy import desc
+from twisted.internet.defer import inlineCallbacks
 
+from peek_core_device._private.server.controller.OfflineCacheController import (
+    OfflineCacheController,
+)
 from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
 from peek_core_device._private.storage.GpsLocationTable import GpsLocationTable
 from twisted.internet.defer import Deferred
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
-from peek_core_device._private.storage.Setting import (
-    OFFLINE_CACHE_REFRESH_SECONDS,
-)
-from peek_core_device._private.storage.Setting import globalSetting
-from peek_core_device._private.tuples.OfflineCacheSettingTuple import (
-    OfflineCacheSettingTuple,
-)
-
 logger = logging.getLogger(__name__)
 
 
-class OfflineCacheSettingTupleProvider(TuplesProviderABC):
-    def __init__(self, ormSessionCreator):
+class DeviceInfoTableTupleProvider(TuplesProviderABC):
+    def __init__(
+        self,
+        ormSessionCreator,
+        offlineCacheController: OfflineCacheController,
+        userApi,
+    ):
+        from peek_core_user.server.UserApiABC import UserApiABC
+
         self._ormSessionCreator = ormSessionCreator
+        self._offlineCacheController = offlineCacheController
+        self._userApi: UserApiABC = userApi
 
-    @deferToThreadWrapWithLogger(logger)
+    @inlineCallbacks
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
+        from peek_core_user.tuples.UserLoggedInInfoTuple import (
+            UserLoggedInInfoTuple,
+        )
+
+        loggedInUsers: list[
+            UserLoggedInInfoTuple
+        ] = yield self._userApi.infoApi.userLoggedInInfo()
+
+        return (
+            yield self._makeVortexMsgDeferred(
+                filt, tupleSelector, loggedInUsers
+            )
+        )
 
-        deviceToken = tupleSelector.selector.get("deviceToken")
+    @deferToThreadWrapWithLogger(logger)
+    def _makeVortexMsgDeferred(
+        self, filt: dict, tupleSelector: TupleSelector, loggedInUsers
+    ) -> Union[Deferred, bytes]:
+        deviceId = tupleSelector.selector.get("deviceId")
+        userByDeviceToken = {o.deviceToken: o.userName for o in loggedInUsers}
 
         ormSession = self._ormSessionCreator()
         try:
-            try:
-                deviceTuple = (
-                    ormSession.query(DeviceInfoTable)
-                    .filter(DeviceInfoTable.deviceToken == deviceToken)
-                    .one()
-                )
-
-            except sqlalchemy.orm.exc.NoResultFound:
-                deviceTuple = DeviceInfoTable(isOfflineCacheEnabled=False)
-
-            syncSeconds = globalSetting(
-                ormSession, OFFLINE_CACHE_REFRESH_SECONDS
+            query = (
+                ormSession.query(DeviceInfoTable, GpsLocationTable)
+                .outerjoin(GpsLocationTable)
+                .order_by(desc(DeviceInfoTable.lastOnline))
             )
 
-            tuples = [
-                OfflineCacheSettingTuple(
-                    offlineEnabled=deviceTuple.isOfflineCacheEnabled,
-                    offlineCacheSyncSeconds=syncSeconds,
+            if deviceId is not None:
+                query = query.filter(DeviceInfoTable.deviceId == deviceId)
+
+            # Add the current location to each DeviceInfo row
+            tuples = []
+            for deviceInfoTableRow, gpsLocationTableRow in query.all():
+                deviceInfoTableRow.currentLocation = gpsLocationTableRow
+                deviceInfoTableRow.lastCacheCheck = (
+                    self._offlineCacheController.lastCacheUpdate(
+                        deviceInfoTableRow.deviceToken
+                    ),
+                )
+                deviceInfoTableRow.loggedInUser = userByDeviceToken.get(
+                    deviceInfoTableRow.deviceToken
                 )
-            ]
+                tuples.append(deviceInfoTableRow)
 
             # Create the vortex message
             return (
                 Payload(filt, tuples=tuples).makePayloadEnvelope().toVortexMsg()
             )
 
         finally:
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py` & `peek-core-device-3.4.0/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/storage/DeclarativeBase.py` & `peek-core-device-3.4.0/peek_core_device/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/storage/DeviceInfoTable.py` & `peek-core-device-3.4.0/peek_core_device/_private/storage/DeviceInfoTable.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,38 +51,47 @@
     updateVersion = Column(String(15))  # Null means it hasn't updated
     lastOnline = Column(DateTime(True))
     lastUpdateCheck = Column(DateTime(True))
     createdDate = Column(DateTime(True), nullable=False)
     deviceStatus = Column(Integer, nullable=False, server_default="0")
     isEnrolled = Column(Boolean, nullable=False, server_default="0")
     isOfflineCacheEnabled = Column(Boolean, nullable=False, server_default="0")
+    lastBandwidthMetric = Column(Integer, nullable=True)
     currentLocation: DeviceGpsLocationTuple = TupleField()
     lastCacheUpdate: Optional[datetime] = TupleField()
+    loggedInUser: Optional[str] = TupleField()
 
     def toTuple(
         self,
         currentLocationTuple: DeviceGpsLocationTuple = None,
         lastCacheCheck: Optional[datetime] = None,
+        loggedInUser: Optional[str] = None,
     ):
-        return self.toTupleStatic(self, currentLocationTuple, lastCacheCheck)
+        return self.toTupleStatic(
+            self, currentLocationTuple, lastCacheCheck, loggedInUser
+        )
 
     @staticmethod
     def toTupleStatic(
         table: "DeviceInfoTable",
         currentLocationTuple: Optional[DeviceGpsLocationTuple] = None,
         lastCacheCheck: Optional[datetime] = None,
+        loggedInUser: Optional[str] = None,
     ):
         return DeviceInfoTuple(
             description=table.description,
             deviceId=table.deviceId,
             deviceType=table.deviceType,
             deviceToken=table.deviceToken,
             appVersion=table.appVersion,
             updateVersion=table.updateVersion,
             lastOnline=table.lastOnline,
             lastUpdateCheck=table.lastUpdateCheck,
             createdDate=table.createdDate,
             deviceStatus=table.deviceStatus,
             isEnrolled=table.isEnrolled,
+            isOfflineCacheEnabled=table.isOfflineCacheEnabled,
+            lastBandwidthMetric=table.lastBandwidthMetric,
             currentLocation=currentLocationTuple,
             lastCacheCheck=lastCacheCheck,
+            loggedInUser=loggedInUser,
         )
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/storage/DeviceUpdateTuple.py` & `peek-core-device-3.4.0/peek_core_device/_private/storage/DeviceUpdateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/storage/GpsLocationHistoryTable.py` & `peek-core-device-3.4.0/peek_core_device/_private/storage/GpsLocationHistoryTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/storage/GpsLocationTable.py` & `peek-core-device-3.4.0/peek_core_device/_private/storage/GpsLocationTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/storage/Setting.py` & `peek-core-device-3.4.0/peek_core_device/_private/storage/Setting.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,134 +41,93 @@
     called ``_proxied``.  The class which inherits this class
     should have an attribute called ``_proxied`` which points to a dictionary.
 
     """
 
     _proxied = None
 
-    def __len__(
-        self
-        ):
+    def __len__(self):
         return len(self._proxied)
 
-    def __iter__(
-        self
-        ):
+    def __iter__(self):
         return iter(self._proxied)
 
-    def __getitem__(
-        self,
-        key
-        ):
+    def __getitem__(self, key):
         return self._proxied[str(key)]
 
-    def __contains__(
-        self,
-        key
-        ):
+    def __contains__(self, key):
         return str(key) in self._proxied
 
-    def __setitem__(
-        self,
-        key,
-        value
-        ):
+    def __setitem__(self, key, value):
         self._proxied[str(key)] = value
 
-    def __delitem__(
-        self,
-        key
-        ):
+    def __delitem__(self, key):
         del self._proxied[str(key)]
 
 
 class PolymorphicVerticalProperty(object):
     """A key/value pair with polymorphic value storage.
 
     The class which is mapped should indicate typing information
     within the "info" dictionary of mapped Column objects; see
     the AnimalFact mapping below for an example.
 
     """
 
-    def __init__(
-        self,
-        key,
-        value=None
-        ):
+    def __init__(self, key, value=None):
         self.key = key
         self.value = value
 
     @hybrid_property
-    def value(
-        self
-        ):
+    def value(self):
         fieldname, discriminator = self.type_map[self.type]
         if fieldname is None:
             return None
         else:
             return getattr(self, fieldname)
 
     @value.setter
-    def value(
-        self,
-        value
-        ):
+    def value(self, value):
         py_type = type(value)
         fieldname, discriminator = self.type_map[py_type]
 
         self.type = discriminator
         if fieldname is not None:
             setattr(self, fieldname, value)
 
     @value.deleter
-    def value(
-        self
-        ):
+    def value(self):
         self._set_value(None)
 
     @value.comparator
     class value(PropComparator):
         """A comparator for .value, builds a polymorphic comparison via CASE."""
 
-        def __init__(
-            self,
-            cls
-            ):
+        def __init__(self, cls):
             self.cls = cls
 
-        def _case(
-            self
-            ):
+        def _case(self):
             pairs = set(self.cls.type_map.values())
             whens = [
                 (
                     literal_column("'%s'" % discriminator),
                     cast(getattr(self.cls, attribute), String),
                 )
                 for attribute, discriminator in pairs
                 if attribute is not None
             ]
             return case(whens, self.cls.type, null())
 
-        def __eq__(
-            self,
-            other
-            ):
+        def __eq__(self, other):
             return self._case() == cast(other, String)
 
-        def __ne__(
-            self,
-            other
-            ):
+        def __ne__(self, other):
             return self._case() != cast(other, String)
 
-    def __repr__(
-        self
-        ):
+    def __repr__(self):
         return "<%s %r=%r>" % (self.__class__.__name__, self.key, self.value)
 
 
 @addTupleType
 class SettingProperty(PolymorphicVerticalProperty, Tuple, DeclarativeBase):
     """A setting property."""
 
@@ -182,19 +141,15 @@
 
     # add information about storage for different types
     # in the info dictionary of Columns
     int_value = Column(Integer, info={"type": (int, "integer")})
     char_value = Column(String, info={"type": (str, "string")})
     boolean_value = Column(Boolean, info={"type": (bool, "boolean")})
 
-    def __init__(
-        self,
-        key=None,
-        value=None
-        ):
+    def __init__(self, key=None, value=None):
         PolymorphicVerticalProperty.__init__(self, key=key, value=value)
         Tuple.__init__(self)
 
     __table_args__ = (Index("idx_SettingProperty_settingId", settingId),)
 
 
 @addTupleType
@@ -212,44 +167,30 @@
     )
 
     propertyObjects = relationship("SettingProperty", viewonly=True, lazy=False)
 
     _proxied = association_proxy(
         "properties",
         "value",
-        creator=lambda
-            key,
-            value: SettingProperty(key=key, value=value),
+        creator=lambda key, value: SettingProperty(key=key, value=value),
     )
 
-    def __init__(
-        self,
-        name=None
-        ):
+    def __init__(self, name=None):
         self.name = name
 
-    def __repr__(
-        self
-        ):
+    def __repr__(self):
         return "Setting(%r)" % self.name
 
     @classmethod
-    def with_characteristic(
-        self,
-        key,
-        value
-        ):
+    def with_characteristic(self, key, value):
         return self.properties.any(key=key, value=value)
 
 
 @event.listens_for(SettingProperty, "mapper_configured", propagate=True)
-def on_new_class(
-    mapper,
-    cls_
-    ):
+def on_new_class(mapper, cls_):
     """Look for Column objects with type info in them, and work up
     a lookup table."""
 
     info_dict = {}
     info_dict[type(None)] = (None, "none")
     info_dict["none"] = (None, "none")
 
@@ -259,37 +200,24 @@
             python_type, discriminator = col.info["type"]
             info_dict[python_type] = (k, discriminator)
             info_dict[discriminator] = (k, discriminator)
     cls_.type_map = info_dict
 
 
 class PropertyKey(object):
-    def __init__(
-        self,
-        name,
-        defaultValue,
-        propertyDict
-        ):
+    def __init__(self, name, defaultValue, propertyDict):
         self.name = name
         self.defaultValue = defaultValue
         propertyDict[name] = self
 
-    def __repr__(
-        self
-        ):
+    def __repr__(self):
         return self.name
 
 
-def _getSetting(
-    ormSession,
-    name,
-    propertyDict,
-    key=None,
-    value=None
-    ):
+def _getSetting(ormSession, name, propertyDict, key=None, value=None):
     all = ormSession.query(Setting).filter(Setting.name == name).all()
 
     if all:
         setting = all[0]
         ormSession.expire(setting)
     else:
         setting = Setting(name)
@@ -307,15 +235,17 @@
         ormSession.commit()
 
     if not key:
         return setting
 
     # Make sure the propery is defined for this setting
     assert str(key) in propertyDict, "Key %s is not defined in setting %s" % (
-        key, name)
+        key,
+        name,
+    )
 
     if value is None:
         return setting[key]
 
     setting[key] = value
     ormSession.commit()
 
@@ -326,21 +256,18 @@
 # =============================================================================
 # GLOBAL PROPERTIES
 # =============================================================================
 
 globalProperties = {}
 
 
-def globalSetting(
-    ormSession,
-    key=None,
-    value=None
-    ):
-    return _getSetting(ormSession, "Global", globalProperties, key=key,
-        value=value)
+def globalSetting(ormSession, key=None, value=None):
+    return _getSetting(
+        ormSession, "Global", globalProperties, key=key, value=value
+    )
 
 
 AUTO_ENROLLMENT = PropertyKey(
     "Device Auto Enrollment", False, propertyDict=globalProperties
 )
 
 # =============================================================================
@@ -353,9 +280,20 @@
 )
 
 OFFICE_ENROLLMENT_ENABLED = PropertyKey(
     "Office Enrollment Enabled", False, propertyDict=globalProperties
 )
 
 OFFLINE_CACHE_REFRESH_SECONDS = PropertyKey(
-    "Offline Cache Refresh Seconds", 15 * 60, propertyDict=globalProperties
+    "Offline Cache Refresh Seconds", 24 * 60 * 60, propertyDict=globalProperties
+)
+
+OFFLINE_MASTER_SWITCH_ENABLED = PropertyKey(
+    "Offline Master Switch Enabled", True, propertyDict=globalProperties
+)
+
+
+SLOW_NETWORK_BANDWIDTH_METRIC_THRESHOLD = PropertyKey(
+    "Slow Network Bandwidth Metric Threshold",
+    1200,
+    propertyDict=globalProperties,
 )
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/OfflineCacheSettingTuple.py` & `peek-core-device-3.4.0/peek_core_device/tuples/DeviceStatusTuple.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from vortex.Tuple import Tuple
 from vortex.Tuple import TupleField
 from vortex.Tuple import addTupleType
 
 from peek_core_device._private.PluginNames import deviceTuplePrefix
+from peek_core_device.tuples.DeviceInfoTuple import DeviceInfoTuple
 
 
 @addTupleType
-class OfflineCacheSettingTuple(Tuple):
-    """Offline Cache Setting Tuple
+class DeviceStatusTuple(Tuple):
+    __tupleType__ = deviceTuplePrefix + "DeviceStatusTuple"
 
-    This tuple is for the client UI settings.
-
-    """
-
-    __tupleType__ = deviceTuplePrefix + "OfflineCacheSettingTuple"
-
-    offlineEnabled: bool = TupleField(defaultValue=False)
-    offlineCacheSyncSeconds: int = TupleField(defaultValue=15 * 60)
+    DEVICE_OFFLINE = DeviceInfoTuple.DEVICE_OFFLINE
+    DEVICE_ONLINE = DeviceInfoTuple.DEVICE_ONLINE
+    DEVICE_BACKGROUND = DeviceInfoTuple.DEVICE_BACKGROUND
+
+    deviceId: str = TupleField()
+    deviceToken: str = TupleField()
+    deviceStatus: int = TupleField()
+
+    @property
+    def deviceOnline(self) -> bool:
+        return bool(
+            self.deviceStatus & self.DEVICE_ONLINE and not
+            self.deviceStatus & self.DEVICE_BACKGROUND
+        )
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/OfflineCacheStatusAction.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+from vortex.Tuple import Tuple
 from vortex.Tuple import TupleField
 from vortex.Tuple import addTupleType
-from vortex.TupleAction import TupleActionABC
 
 from peek_core_device._private.PluginNames import deviceTuplePrefix
+from peek_core_device._private.tuples.OfflineCacheLoaderStatusTuple import (
+    OfflineCacheLoaderStatusTuple,
+)
 from peek_core_device._private.tuples.OfflineCacheStatusTuple import (
     OfflineCacheStatusTuple,
 )
 
 
 @addTupleType
-class OfflineCacheStatusAction(TupleActionABC):
+class OfflineCacheCombinedStatusTuple(Tuple):
     """Offline Cache Status Action
 
     This tuple is sent from the client to the server periodically when
     an update cycle finishes
 
     """
 
-    __tupleType__ = deviceTuplePrefix + "OfflineCacheStatusAction"
+    __tupleType__ = deviceTuplePrefix + "OfflineCacheCombinedStatusTuple"
 
     deviceToken: str = TupleField()
-    cacheStatusList: list[OfflineCacheStatusTuple] = TupleField([])
+    loaderStatusList: list[OfflineCacheLoaderStatusTuple] = TupleField([])
+    offlineCacheStatus: OfflineCacheStatusTuple = TupleField()
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/OfflineCacheStatusTuple.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/OfflineCacheLoaderStatusTuple.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from vortex.Tuple import TupleField
 from vortex.Tuple import addTupleType
 
 from peek_core_device._private.PluginNames import deviceTuplePrefix
 
 
 @addTupleType
-class OfflineCacheStatusTuple(Tuple):
+class OfflineCacheLoaderStatusTuple(Tuple):
     """Offline Cache Status Tuple
 
     This tuple represents the load status of the mobile device.
 
     """
 
-    __tupleType__ = deviceTuplePrefix + "OfflineCacheStatusTuple"
+    __tupleType__ = deviceTuplePrefix + "OfflineCacheLoaderStatusTuple"
 
     pluginName: str = TupleField()
     indexName: str = TupleField()
     loadingQueueCount: int = TupleField()
     totalLoadedCount: int = TupleField()
     lastCheckDate: datetime = TupleField()
-    initialFullLoadComplete:bool = TupleField()
+    initialFullLoadComplete: bool = TupleField()
```

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateEnrollmentAction.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateEnrollmentAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py` & `peek-core-device-3.4.0/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png` & `peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst` & `peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/device_search.png` & `peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/device_search.png`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png` & `peek-core-device-3.4.0/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/admin-doc/overview.rst` & `peek-core-device-3.4.0/peek_core_device/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/both-doc/index.rst` & `peek-core-device-3.4.0/peek_core_device/both-doc/index.rst`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/DeviceInfoTuple.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/DeviceInfoTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-background.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-background.service.ts`

 * *Files 12% similar despite different names*

```diff
@@ -16,11 +16,17 @@
         App.addListener("appStateChange", (state) => {
             this.deviceBackgrounded = !state.isActive;
 
             const action = new DeviceBackgroundStateTupleAction();
             action.deviceId = this.deviceId;
             action.deviceBackgrounded = this.deviceBackgrounded;
 
-            this.tupleService.tupleAction.pushAction(action);
+            this.tupleService.tupleAction
+                .pushAction(action)
+                .catch((e) =>
+                    console.log(
+                        `Failed to send device background update, Error: ${e}`
+                    )
+                );
         });
     }
 }
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-nav.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-nav.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-online.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-online.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-server.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-server.service.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,22 @@
 import { Observable, Subject } from "rxjs";
 import { filter, first } from "rxjs/operators";
 import { Injectable } from "@angular/core";
 import { BalloonMsgService } from "@synerty/peek-plugin-base-js";
 import {
-    addTupleType,
     extend,
-    Tuple,
     TupleSelector,
     VortexService,
     VortexStatusService,
 } from "@synerty/vortexjs";
-import { deviceFilt, deviceTuplePrefix } from "./PluginNames";
+import { deviceFilt } from "./PluginNames";
 import { DeviceTupleService } from "./device-tuple.service";
 import { DeviceNavService } from "./device-nav.service";
 import { Capacitor } from "@capacitor/core";
-
-@addTupleType
-export class ServerInfoTuple extends Tuple {
-    public static readonly tupleName = deviceTuplePrefix + "ServerInfoTuple";
-
-    static readonly DEFAULT_HTTP_PORT = 8000;
-    static readonly DEFAULT_WEBSOCKET_PORT = 8000;
-
-    host: string;
-    useSsl: boolean = false;
-    httpPort: number;
-    websocketPort: number;
-    hasConnected: boolean = false;
-
-    constructor() {
-        super(ServerInfoTuple.tupleName);
-        this.httpPort = ServerInfoTuple.DEFAULT_HTTP_PORT;
-        this.websocketPort = ServerInfoTuple.DEFAULT_WEBSOCKET_PORT;
-    }
-}
+import { ServerInfoTuple } from "@peek/peek_core_device/_private/tuples/server-info-tuple";
 
 @Injectable()
 export class DeviceServerService {
     private tupleSelector: TupleSelector = new TupleSelector(
         ServerInfoTuple.tupleName,
         {}
     );
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-tuple.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-tuple.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-update.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-update.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/device-update.service.web.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-update.service.web.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,84 @@
 import { Injectable } from "@angular/core";
-import { BehaviorSubject, combineLatest, Observable } from "rxjs";
+import {
+    BehaviorSubject,
+    combineLatest,
+    fromEvent,
+    interval,
+    Observable,
+    Subject,
+} from "rxjs";
+import { takeUntil, throttle } from "rxjs/operators";
 import {
     DeviceGpsLocationService,
     DeviceGpsLocationTuple,
 } from "@peek/peek_core_device";
 import { UserService } from "@peek/peek_core_user";
-import { Capacitor, Plugins } from "@capacitor/core";
+import { Capacitor, registerPlugin } from "@capacitor/core";
 import { Dialog } from "@capacitor/dialog";
 import { Geolocation } from "@capacitor/geolocation";
 import { DeviceTupleService } from "../device-tuple.service";
 import { GpsLocationUpdateTupleAction } from "./GpsLocationUpdateTupleAction";
 import { DeviceEnrolmentService } from "../../device-enrolment.service";
 import { DeviceBackgroundService } from "../device-background.service";
 import { isField } from "@peek/peek_core_device/_private/hardware-info/is-field.mweb";
-
-import { registerPlugin } from "@capacitor/core";
 import { BackgroundGeolocationPlugin } from "@capacitor-community/background-geolocation";
+
 const BackgroundGeolocation = registerPlugin<BackgroundGeolocationPlugin>(
     "BackgroundGeolocation"
 );
 
 @Injectable()
 export class PrivateDeviceGpsLocationService extends DeviceGpsLocationService {
     private _location$ = new BehaviorSubject<DeviceGpsLocationTuple | null>(
         null
     );
     private gpsWatchId: string | null;
     private lastSeenPositionTupleAction: GpsLocationUpdateTupleAction;
 
+    private readonly GPS_UPDATE_SECONDS = 120;
+
+    private readonly position$ = new Subject<any>();
+
     constructor(
         private tupleService: DeviceTupleService,
         private deviceService: DeviceEnrolmentService,
         private deviceBackgroundService: DeviceBackgroundService,
         private userService: UserService
     ) {
         super();
 
         if (isField) {
-            combineLatest([
-                this.userService.loggedInStatus,
-                this.deviceService.deviceInfoObservable(),
-            ]).subscribe(async ([isLoggedIn, deviceInfo]) => {
+            this.setupWatch();
+        }
+    }
+
+    private setupWatch(): void {
+        // Reduce the frequency of updates
+        this.position$
+            .pipe(throttle(() => interval(this.GPS_UPDATE_SECONDS * 1000)))
+            .pipe(takeUntil(this.onDestroyEvent))
+            .subscribe((position) => this.updateLocationThrottled(position));
+
+        combineLatest([
+            this.userService.loggedInStatus,
+            this.deviceService.deviceInfoObservable(),
+        ])
+            .pipe(takeUntil(this.onDestroyEvent))
+            .subscribe(async ([isLoggedIn, deviceInfo]) => {
                 if (isLoggedIn && deviceInfo.isEnrolled) {
                     if (!this.gpsWatchId) {
                         this.startLocationListener();
                     }
                 } else {
                     if (this.gpsWatchId) {
                         this.stopLocationListener();
                     }
                 }
             });
-        }
     }
 
     get location$(): Observable<DeviceGpsLocationTuple | null> {
         return this._location$.asObservable();
     }
 
     get location(): DeviceGpsLocationTuple | null {
@@ -140,17 +163,22 @@
         } else {
             Geolocation.clearWatch({ id: this.gpsWatchId }) //
                 .then(() => (this.gpsWatchId = null));
         }
     }
 
     private updateLocation(position): void {
+        this.position$.next(position);
+    }
+
+    private updateLocationThrottled(position): void {
         const now = new Date(); // In datetime with timezone
 
         // Send to Peek Logic
+        console.log("Sending GPS Location");
         const action = new GpsLocationUpdateTupleAction();
         action.latitude = position.coords.latitude;
         action.longitude = position.coords.longitude;
         action.updateType = GpsLocationUpdateTupleAction.ACCURACY_FINE;
         action.datetime = now;
         action.deviceToken = this.deviceService.enrolmentToken();
         this.lastSeenPositionTupleAction = action;
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/index.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 export { AlterDeviceUpdateAction } from "./tuples/admin/AlterDeviceUpdateAction";
 export { CreateDeviceUpdateAction } from "./tuples/admin/CreateDeviceUpdateAction";
 
 export { HardwareInfo } from "./hardware-info/hardware-info";
 export { DeviceTypeEnum } from "./hardware-info/hardware-info";
 
 export { DeviceNavService } from "./device-nav.service";
-export { DeviceServerService, ServerInfoTuple } from "./device-server.service";
+export { DeviceServerService } from "./device-server.service";
 export { DeviceTupleService } from "./device-tuple.service";
 export { DeviceOnlineService } from "./device-online.service";
+export { ServerInfoTuple } from "@peek/peek_core_device/_private/tuples/server-info-tuple";
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusAction.ts` & `peek-core-device-3.4.0/peek_core_device/_private/admin-app/tuples/DeviceCacheStatusTuple.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import { addTupleType, TupleActionABC } from "@synerty/vortexjs";
-import { deviceTuplePrefix } from "../PluginNames";
-import { OfflineCacheStatusTuple } from "../../tuples/OfflineCacheStatusTuple";
+import { addTupleType, Tuple } from "@synerty/vortexjs";
+import { deviceTuplePrefix } from "@peek/peek_core_device/_private";
+import { OfflineCacheLoaderStatusTuple } from "@peek/peek_core_device/tuples/OfflineCacheLoaderStatusTuple";
 
 @addTupleType
-export class OfflineCacheStatusAction extends TupleActionABC {
+export class DeviceCacheStatusTuple extends Tuple {
     public static readonly tupleName =
-        deviceTuplePrefix + "OfflineCacheStatusAction";
+        deviceTuplePrefix + "DeviceCacheStatusTuple";
 
-    deviceToken: string;
-    cacheStatusList: OfflineCacheStatusTuple[] = [];
+    statusList: OfflineCacheLoaderStatusTuple[] = [];
 
     constructor() {
-        super(OfflineCacheStatusAction.tupleName);
+        super(DeviceCacheStatusTuple.tupleName);
     }
 }
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/device-enrolled.guard.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/device-enrolled.guard.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/device-enrolment.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/device-enrolment.service.ts`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import { Injectable } from "@angular/core";
 import { HeaderService } from "@synerty/peek-plugin-base-js";
-import { Observable, Subject } from "rxjs";
+import { BehaviorSubject, Observable, Subject } from "rxjs";
 import { TupleSelector, VortexStatusService } from "@synerty/vortexjs";
 import { DeviceInfoTuple } from "./DeviceInfoTuple";
 import { DeviceNavService } from "./_private/device-nav.service";
 import { DeviceTupleService } from "./_private/device-tuple.service";
 import { DeviceServerService } from "./_private/device-server.service";
+import { filter } from "rxjs/operators";
 
 @Injectable()
 export class DeviceEnrolmentService {
     deviceInfo: DeviceInfoTuple = null;
 
     // There is no point having multiple services observing the same thing
     // So lets create a nice observable for the device info.
-    private deviceInfoSubject = new Subject<DeviceInfoTuple>();
+    private deviceInfoSubject = new BehaviorSubject<DeviceInfoTuple | null>(
+        null
+    );
 
     private _isLoading = true;
 
     constructor(
         private nav: DeviceNavService,
         private headerService: HeaderService,
         private vortexStatusService: VortexStatusService,
@@ -80,15 +83,17 @@
             return false;
         }
 
         return true;
     }
 
     deviceInfoObservable(): Observable<DeviceInfoTuple> {
-        return this.deviceInfoSubject;
+        return this.deviceInfoSubject.pipe(
+            filter((deviceInfo) => deviceInfo != null)
+        );
     }
 
     isFieldService(): boolean {
         return this.tupleService.hardwareInfo.isField();
     }
 
     isOfficeService(): boolean {
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/device-loading.module.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/_private/device-loading.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/device-status.service.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/device-status.service.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 import { Injectable } from "@angular/core";
 import { DeviceServerService } from "./_private/device-server.service";
 import { DeviceEnrolmentService } from "./device-enrolment.service";
 import { Router } from "@angular/router";
 import { deviceBaseUrl } from "./_private";
+import { BehaviorSubject } from "rxjs";
+import { DeviceBandwidthTestService } from "@peek/peek_core_device/_private/device-bandwidth-test.service";
+import { takeUntil } from "rxjs/operators";
+
+import { NgLifeCycleEvents } from "@synerty/vortexjs";
 
 @Injectable()
-export class DeviceStatusService {
+export class DeviceStatusService extends NgLifeCycleEvents {
+    public readonly isNetworkSlow$ = new BehaviorSubject<boolean>(false);
+
     constructor(
         private router: Router,
         private enrolmentService: DeviceEnrolmentService,
-        private deviceServerService: DeviceServerService
-    ) {}
+        private deviceServerService: DeviceServerService,
+        private deviceBandwidthTestService: DeviceBandwidthTestService
+    ) {
+        super();
+        deviceBandwidthTestService.status$
+            .pipe(takeUntil(this.onDestroyEvent))
+            .subscribe((status) =>
+                this.isNetworkSlow$.next(status.isSlowNetwork)
+            );
+    }
 
     get isLoading(): boolean {
         // If we're currently showing a peek_core_device route then, loading = false
         let index = this.router.url.indexOf(deviceBaseUrl);
         if (0 <= index && index <= 4)
             // allow for "/..." etc
             return false;
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin-module/index.ts` & `peek-core-device-3.4.0/peek_core_device/plugin-module/index.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 export { DeviceStatusService } from "./device-status.service";
 export { DeviceInfoTuple } from "./DeviceInfoTuple";
 export { DeviceEnrolmentService } from "./device-enrolment.service";
 export { DeviceEnrolledGuard } from "./device-enrolled.guard";
 export { DeviceGpsLocationService } from "./gps-location.service";
 export { DeviceGpsLocationTuple } from "./DeviceGpsLocationTuple";
 export { DeviceOfflineCacheService } from "./device-offline-cache.service";
-export { OfflineCacheStatusTuple } from "./tuples/OfflineCacheStatusTuple";
+export { OfflineCacheLoaderStatusTuple } from "./tuples/OfflineCacheLoaderStatusTuple";
```

### Comparing `peek-core-device-3.3.3/peek_core_device/plugin_package.json` & `peek-core-device-3.4.0/peek_core_device/plugin_package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940934065934066%*

 * *Differences: {"'field'": "{'rootModules': {0: {'file': '_private/device-loading.module'}}, 'rootServices': "*

 * *            "{insert: [(7, OrderedDict([('file', '_private/device-bandwidth-test.service'), "*

 * *            "('class', 'DeviceBandwidthTestService')]))]}}",*

 * * "'office'": "{'rootModules': {0: {'file': '_private/device-loading.module'}}, 'rootServices': "*

 * *             "{insert: [(7, OrderedDict([('file', '_private/device-bandwidth-test.service'), "*

 * *             "('class', 'DeviceBandwidthTestService')]))]}}",*

 * * "'plug […]*

```diff
@@ -14,15 +14,15 @@
         "appDir": "_private/both-app",
         "cfgDir": "_private/both-cfg",
         "cfgModule": "core-device-cfg.module#CoreDeviceCfgModule",
         "moduleDir": "plugin-module",
         "rootModules": [
             {
                 "class": "DeviceLoadingModule",
-                "file": "device-loading.module"
+                "file": "_private/device-loading.module"
             }
         ],
         "rootServices": [
             {
                 "class": "DeviceOfflineCacheService",
                 "file": "device-offline-cache.service",
                 "persistent": true
@@ -54,14 +54,18 @@
             },
             {
                 "class": "DeviceTupleService",
                 "file": "_private/device-tuple.service",
                 "persistent": true
             },
             {
+                "class": "DeviceBandwidthTestService",
+                "file": "_private/device-bandwidth-test.service"
+            },
+            {
                 "class": "DeviceStatusService",
                 "file": "device-status.service",
                 "persistent": true
             },
             {
                 "class": "PrivateDeviceGpsLocationService",
                 "file": "_private/gps/private-gps-location.service",
@@ -94,15 +98,15 @@
         "appDir": "_private/both-app",
         "cfgDir": "_private/both-cfg",
         "cfgModule": "core-device-cfg.module#CoreDeviceCfgModule",
         "moduleDir": "plugin-module",
         "rootModules": [
             {
                 "class": "DeviceLoadingModule",
-                "file": "device-loading.module"
+                "file": "_private/device-loading.module"
             }
         ],
         "rootServices": [
             {
                 "class": "DeviceOfflineCacheService",
                 "file": "device-offline-cache.service",
                 "persistent": true
@@ -134,14 +138,18 @@
             },
             {
                 "class": "DeviceTupleService",
                 "file": "_private/device-tuple.service",
                 "persistent": true
             },
             {
+                "class": "DeviceBandwidthTestService",
+                "file": "_private/device-bandwidth-test.service"
+            },
+            {
                 "class": "DeviceStatusService",
                 "file": "device-status.service",
                 "persistent": true
             },
             {
                 "class": "PrivateDeviceGpsLocationService",
                 "file": "_private/gps/private-gps-location.service",
@@ -171,15 +179,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_device",
         "title": "Device",
-        "version": "3.3.3",
+        "version": "3.4.0",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "admin",
         "field",
```

### Comparing `peek-core-device-3.3.3/peek_core_device/server/DeviceApiABC.py` & `peek-core-device-3.4.0/peek_core_device/server/DeviceApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/tuples/DeviceDetailTuple.py` & `peek-core-device-3.4.0/peek_core_device/tuples/DeviceDetailTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.3.3/peek_core_device/tuples/DeviceInfoTuple.py` & `peek-core-device-3.4.0/peek_core_device/tuples/DeviceInfoTuple.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,9 +43,12 @@
     appVersion = TupleField()
     updateVersion = TupleField()
     lastOnline = TupleField()
     lastUpdateCheck = TupleField()
     createdDate = TupleField()
     deviceStatus = TupleField()
     isEnrolled = TupleField()
+    lastBandwidthMetric: Optional[int] = TupleField()
+    isOfflineCacheEnabled: Optional[bool] = TupleField()
     currentLocation: DeviceGpsLocationTuple = TupleField()
     lastCacheCheck: Optional[datetime] = TupleField()
+    loggedInUser: Optional[str] = TupleField()
```

### Comparing `peek-core-device-3.3.3/peek_core_device.egg-info/SOURCES.txt` & `peek-core-device-3.4.0/peek_core_device.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 peek_core_device/_private/alembic/script.py.mako
 peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py
 peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py
 peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py
 peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py
 peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py
 peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py
+peek_core_device/_private/alembic/versions/97d44e5aeb18_add_lastbandwidthmetric.py
 peek_core_device/_private/alembic/versions/__init__.py
 peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py
 peek_core_device/_private/both-app/device.component.ts
 peek_core_device/_private/both-app/device.component.web.html
 peek_core_device/_private/both-app/device.module.ts
 peek_core_device/_private/both-app/device.routes.ts
 peek_core_device/_private/both-app/connect/connect.component.ts
@@ -57,57 +58,64 @@
 peek_core_device/_private/both-app/loading/loading.component.web.html
 peek_core_device/_private/both-cfg/core-device-cfg.component.ts
 peek_core_device/_private/both-cfg/core-device-cfg.component.web.html
 peek_core_device/_private/both-cfg/core-device-cfg.module.ts
 peek_core_device/_private/both-cfg/connect/connect.component.ts
 peek_core_device/_private/both-cfg/connect/connect.component.web.html
 peek_core_device/_private/client/ClientEntryHook.py
-peek_core_device/_private/client/DeviceOnlineHandler.py
 peek_core_device/_private/client/DeviceTupleDataObservableProxy.py
 peek_core_device/_private/client/DeviceTupleProcessorActionProxy.py
 peek_core_device/_private/client/UpdateDownloadHandler.py
 peek_core_device/_private/client/__init__.py
+peek_core_device/_private/client/controllers/BandwidthTestController.py
+peek_core_device/_private/client/controllers/DeviceOnlineController.py
+peek_core_device/_private/client/controllers/__init__.py
 peek_core_device/_private/server/DeviceApi.py
 peek_core_device/_private/server/LogicEntryHook.py
 peek_core_device/_private/server/TupleActionProcessor.py
 peek_core_device/_private/server/TupleDataObservable.py
 peek_core_device/_private/server/__init__.py
 peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py
 peek_core_device/_private/server/admin_backend/__init__.py
+peek_core_device/_private/server/controller/BandwidthResultController.py
 peek_core_device/_private/server/controller/DeviceStatusController.py
 peek_core_device/_private/server/controller/EnrollmentController.py
 peek_core_device/_private/server/controller/GpsController.py
 peek_core_device/_private/server/controller/MainController.py
 peek_core_device/_private/server/controller/NotifierController.py
 peek_core_device/_private/server/controller/OfflineCacheController.py
 peek_core_device/_private/server/controller/UpdateController.py
 peek_core_device/_private/server/controller/__init__.py
 peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py
-peek_core_device/_private/server/tuple_providers/DeviceCacheStatusTupleProvider.py
 peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py
 peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py
 peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py
 peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py
+peek_core_device/_private/server/tuple_providers/OfflineCacheCombinedStatusTupleProvider.py
 peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py
 peek_core_device/_private/server/tuple_providers/__init__.py
 peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py
 peek_core_device/_private/server/update_resources/__init__.py
 peek_core_device/_private/storage/DeclarativeBase.py
 peek_core_device/_private/storage/DeviceInfoTable.py
 peek_core_device/_private/storage/DeviceUpdateTuple.py
 peek_core_device/_private/storage/GpsLocationHistoryTable.py
 peek_core_device/_private/storage/GpsLocationTable.py
 peek_core_device/_private/storage/Setting.py
 peek_core_device/_private/storage/__init__.py
 peek_core_device/_private/tuples/AlterDeviceUpdateAction.py
+peek_core_device/_private/tuples/BandwidthTestResultTuple.py
+peek_core_device/_private/tuples/BandwidthTestTuple.py
 peek_core_device/_private/tuples/ClientSettingsTuple.py
 peek_core_device/_private/tuples/CreateDeviceUpdateAction.py
 peek_core_device/_private/tuples/DeviceBackgroundStateTupleAction.py
 peek_core_device/_private/tuples/DeviceCacheStatusTuple.py
 peek_core_device/_private/tuples/EnrolDeviceAction.py
+peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple.py
+peek_core_device/_private/tuples/OfflineCacheLoaderStatusTuple.py
 peek_core_device/_private/tuples/OfflineCacheSettingTuple.py
 peek_core_device/_private/tuples/OfflineCacheStatusAction.py
 peek_core_device/_private/tuples/OfflineCacheStatusTuple.py
 peek_core_device/_private/tuples/UpdateAppliedAction.py
 peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py
 peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py
 peek_core_device/_private/tuples/UpdateEnrollmentAction.py
@@ -123,48 +131,55 @@
 peek_core_device/admin-doc/general_settings/general_settings.png
 peek_core_device/admin-doc/general_settings/general_settings.rst
 peek_core_device/both-doc/index.rst
 peek_core_device/plugin-module/DeviceGpsLocationTuple.ts
 peek_core_device/plugin-module/DeviceInfoTuple.ts
 peek_core_device/plugin-module/device-enrolled.guard.ts
 peek_core_device/plugin-module/device-enrolment.service.ts
-peek_core_device/plugin-module/device-loading.module.ts
 peek_core_device/plugin-module/device-offline-cache.service.ts
 peek_core_device/plugin-module/device-status.service.ts
 peek_core_device/plugin-module/gps-location.service.ts
 peek_core_device/plugin-module/index.ts
 peek_core_device/plugin-module/package.json
 peek_core_device/plugin-module/_private/PluginNames.ts
 peek_core_device/plugin-module/_private/device-background.service.ts
+peek_core_device/plugin-module/_private/device-bandwidth-test.service.ts
+peek_core_device/plugin-module/_private/device-loading.module.ts
 peek_core_device/plugin-module/_private/device-nav.service.ts
 peek_core_device/plugin-module/_private/device-online.service.ts
 peek_core_device/plugin-module/_private/device-server.service.ts
 peek_core_device/plugin-module/_private/device-tuple.service.ts
 peek_core_device/plugin-module/_private/device-update.service.ts
 peek_core_device/plugin-module/_private/device-update.service.web.ts
 peek_core_device/plugin-module/_private/index.ts
 peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts
 peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts
 peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts
 peek_core_device/plugin-module/_private/hardware-info/is-field.dweb.ts
 peek_core_device/plugin-module/_private/hardware-info/is-field.mweb.ts
+peek_core_device/plugin-module/_private/tuples/BandwidthTestResultTuple.ts
+peek_core_device/plugin-module/_private/tuples/BandwidthTestTuple.ts
 peek_core_device/plugin-module/_private/tuples/ClientSettingsTuple.ts
 peek_core_device/plugin-module/_private/tuples/DeviceBackgroundStateTupleAction.ts
 peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts
 peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts
 peek_core_device/plugin-module/_private/tuples/EnrolDeviceAction.ts
+peek_core_device/plugin-module/_private/tuples/OfflineCacheCombinedStatusTuple.ts
 peek_core_device/plugin-module/_private/tuples/OfflineCacheSettingTuple.ts
 peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusAction.ts
+peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusTuple.ts
 peek_core_device/plugin-module/_private/tuples/UpdateAppliedAction.ts
 peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts
+peek_core_device/plugin-module/_private/tuples/server-info-tuple-defaults.ts
+peek_core_device/plugin-module/_private/tuples/server-info-tuple.ts
 peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts
 peek_core_device/plugin-module/_private/tuples/admin/CreateDeviceUpdateAction.ts
 peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
 peek_core_device/plugin-module/_private/tuples/admin/UpdateEnrollmentAction.ts
-peek_core_device/plugin-module/tuples/OfflineCacheStatusTuple.ts
+peek_core_device/plugin-module/tuples/OfflineCacheLoaderStatusTuple.ts
 peek_core_device/server/DeviceApiABC.py
 peek_core_device/server/__init__.py
 peek_core_device/tuples/DeviceDetailTuple.py
 peek_core_device/tuples/DeviceGpsLocationTuple.py
 peek_core_device/tuples/DeviceInfoTuple.py
 peek_core_device/tuples/DeviceStatusTuple.py
 peek_core_device/tuples/__init__.py
```

### Comparing `peek-core-device-3.3.3/setup.py` & `peek-core-device-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_device"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Core Device - Device management for the peek platform."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

