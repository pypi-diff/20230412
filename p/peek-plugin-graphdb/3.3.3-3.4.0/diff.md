# Comparing `tmp/peek-plugin-graphdb-3.3.3.tar.gz` & `tmp/peek-plugin-graphdb-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-graphdb-3.3.3.tar", last modified: Mon Nov 14 05:37:43 2022, max compression
+gzip compressed data, was "peek-plugin-graphdb-3.4.0.tar", last modified: Wed Apr 12 11:06:32 2023, max compression
```

## Comparing `peek-plugin-graphdb-3.3.3.tar` & `peek-plugin-graphdb-3.4.0.tar`

### file list

```diff
@@ -1,222 +1,216 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.258585 peek-plugin-graphdb-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      400 2022-11-14 05:37:43.258585 peek-plugin-graphdb-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      288 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.240585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/
--rw-r--r--   0 root         (0) root         (0)     1155 2022-11-14 05:37:42.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.241585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/
--rw-r--r--   0 root         (0) root         (0)      244 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.241585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.241585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1469 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.ts
--rw-r--r--   0 root         (0) root         (0)     3040 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/graphdb.component.html
--rw-r--r--   0 root         (0) root         (0)      461 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/graphdb.component.ts
--rw-r--r--   0 root         (0) root         (0)     2659 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/graphdb.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.242585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/status/
--rw-r--r--   0 root         (0) root         (0)     1260 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      998 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/status/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.242585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      560 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.242585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      325 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.243585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)      954 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/26f8d213ba06_tracerule_propname_nullable.py
--rw-r--r--   0 root         (0) root         (0)     1049 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/6dac32ecea20_added_trccfg_title.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10556 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/bdc665a4d160_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)     3196 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/d762bc44dbb3_change_to_biginteger.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.243585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/
--rw-r--r--   0 root         (0) root         (0)      192 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/graphdb.component.ts
--rw-r--r--   0 root         (0) root         (0)      711 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/graphdb.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1321 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/graphdb.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.243585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/view-trace/
--rw-r--r--   0 root         (0) root         (0)     3304 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/view-trace/view.component.ts
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/view-trace/view.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.243585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    12054 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.244585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-cfg/
--rw-r--r--   0 root         (0) root         (0)     1593 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-cfg/graphdb-cfg.component.ts
--rw-r--r--   0 root         (0) root         (0)      759 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-cfg/graphdb-cfg.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1145 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-cfg/graphdb-cfg.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.244585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/
--rw-r--r--   0 root         (0) root         (0)     8217 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)     3854 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/ClientTupleObservable.py
--rw-r--r--   0 root         (0) root         (0)      505 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/TupleActionProcessorProxy.py
--rw-r--r--   0 root         (0) root         (0)      517 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/TupleObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.245585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/
--rw-r--r--   0 root         (0) root         (0)     4120 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/FastGraphDb.py
--rw-r--r--   0 root         (0) root         (0)     3027 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/ItemKeyIndexCacheController.py
--rw-r--r--   0 root         (0) root         (0)    15818 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/PrivateRunTrace.py
--rw-r--r--   0 root         (0) root         (0)     2196 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/SegmentCacheController.py
--rw-r--r--   0 root         (0) root         (0)     5560 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/TraceConfigCacheController.py
--rw-r--r--   0 root         (0) root         (0)     2430 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/TracerController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.245585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     1112 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/handlers/ItemKeyIndexCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)     1041 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/handlers/SegmentCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)      176 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.246585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1318 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/GraphDbDoesKeyExistTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1016 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/ItemKeyIndexUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2665 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/PackedItemKeyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2656 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/PackedSegmentTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)      996 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/SegmentUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1085 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/TraceConfigTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1257 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/TraceResultTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.246585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/
--rw-r--r--   0 root         (0) root         (0)    10072 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      542 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1652 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.247585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)      983 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)     1741 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/admin_backend/ViewSegmentHandler.py
--rw-r--r--   0 root         (0) root         (0)      426 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.247585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)     1304 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/api/GraphDbApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.248585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     1940 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)      808 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)     1479 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/SegmentChunkIndexUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)     2824 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/SegmentIndexChunkLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)     1913 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)     5156 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.248585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     1746 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/ImportController.py
--rw-r--r--   0 root         (0) root         (0)     4039 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/ItemKeyIndexCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)      919 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     3920 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/SegmentIndexCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)      397 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/StatusController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.248585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/graph/
--rw-r--r--   0 root         (0) root         (0)     1474 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/graph/GrpahModelController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/graph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.249585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1027 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/tuple_providers/ModelSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)      925 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/tuple_providers/ServerStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.250585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      710 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1123 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     2246 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbEncodedChunk.py
--rw-r--r--   0 root         (0) root         (0)     1242 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbModelSet.py
--rw-r--r--   0 root         (0) root         (0)     1446 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbSegment.py
--rw-r--r--   0 root         (0) root         (0)     2770 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbTraceConfig.py
--rw-r--r--   0 root         (0) root         (0)     2914 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbTraceConfigRule.py
--rw-r--r--   0 root         (0) root         (0)     1702 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/ItemKeyIndex.py
--rw-r--r--   0 root         (0) root         (0)     1194 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/ItemKeyIndexCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     2385 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/ItemKeyIndexEncodedChunk.py
--rw-r--r--   0 root         (0) root         (0)     7777 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.251585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      942 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/GraphDbEncodedChunkTuple.py
--rw-r--r--   0 root         (0) root         (0)      598 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/GraphDbPackedItemKeyTuple.py
--rw-r--r--   0 root         (0) root         (0)      591 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/GraphDbPackedSegmentTuple.py
--rw-r--r--   0 root         (0) root         (0)     1286 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/ItemKeyIndexUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)     1167 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/ItemKeyTuple.py
--rw-r--r--   0 root         (0) root         (0)     1281 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/SegmentIndexUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)      702 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/ServerStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.251585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/
--rw-r--r--   0 root         (0) root         (0)     1169 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.252585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     6769 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexCompiler.py
--rw-r--r--   0 root         (0) root         (0)     3724 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexImporter.py
--rw-r--r--   0 root         (0) root         (0)     6161 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexCompiler.py
--rw-r--r--   0 root         (0) root         (0)     8174 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexImporter.py
--rw-r--r--   0 root         (0) root         (0)     5237 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/TraceConfigImporter.py
--rw-r--r--   0 root         (0) root         (0)      692 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/_ItemKeyIndexCalcChunkKey.py
--rw-r--r--   0 root         (0) root         (0)      717 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/_SegmentIndexCalcChunkKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.252585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/
--rw-r--r--   0 root         (0) root         (0)     2743 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)      437 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1850 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.252585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/status/
--rw-r--r--   0 root         (0) root         (0)    29513 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/status/status.png
--rw-r--r--   0 root         (0) root         (0)      678 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/status/status.rst
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/trace_logic.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.252585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/both-doc/
--rw-r--r--   0 root         (0) root         (0)      113 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      156 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/both-doc/offline_support.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.254585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      424 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbDoesKeyExistTuple.ts
--rw-r--r--   0 root         (0) root         (0)      717 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbLinkedEdge.ts
--rw-r--r--   0 root         (0) root         (0)     1547 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbLinkedModel.ts
--rw-r--r--   0 root         (0) root         (0)     2240 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbLinkedSegment.ts
--rw-r--r--   0 root         (0) root         (0)      312 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbLinkedVertex.ts
--rw-r--r--   0 root         (0) root         (0)      552 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbModelSetTuple.ts
--rw-r--r--   0 root         (0) root         (0)     3587 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbService.ts
--rw-r--r--   0 root         (0) root         (0)     1144 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbTraceResultEdgeTuple.ts
--rw-r--r--   0 root         (0) root         (0)      973 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbTraceResultTuple.ts
--rw-r--r--   0 root         (0) root         (0)      481 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbTraceResultVertexTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.254585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)     2842 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/GraphDbOfflineTupleCacherService.ts
--rw-r--r--   0 root         (0) root         (0)     2733 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/GraphDbTupleService.ts
--rw-r--r--   0 root         (0) root         (0)      424 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/PluginNames.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.254585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/admin/
--rw-r--r--   0 root         (0) root         (0)      688 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/admin/ServerStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      571 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/admin/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.255585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/
--rw-r--r--   0 root         (0) root         (0)      568 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/GraphDbPackedItemKeyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      442 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexEncodedChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    20202 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1053 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      360 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.255585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/
--rw-r--r--   0 root         (0) root         (0)      427 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/EncodedSegmentChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)      568 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/GraphDbPackedSegmentTuple.ts
--rw-r--r--   0 root         (0) root         (0)    19952 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/PrivateSegmentLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      542 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/PrivateSegmentLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/SegmentIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      335 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.256585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tracer-service/
--rw-r--r--   0 root         (0) root         (0)    17950 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateRunTrace.ts
--rw-r--r--   0 root         (0) root         (0)     8661 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateTracerService.ts
--rw-r--r--   0 root         (0) root         (0)       63 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tracer-service/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.256585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)     2266 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigRuleTuple.ts
--rw-r--r--   0 root         (0) root         (0)      929 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigTuple.ts
--rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)     3834 2022-11-14 05:37:42.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.256585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/server/
--rw-r--r--   0 root         (0) root         (0)     1738 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/server/GraphDbApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.258585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/
--rw-r--r--   0 root         (0) root         (0)      358 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbDoesKeyExistTuple.py
--rw-r--r--   0 root         (0) root         (0)     2168 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportEdgeTuple.py
--rw-r--r--   0 root         (0) root         (0)      664 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportSegmentLinkTuple.py
--rw-r--r--   0 root         (0) root         (0)     3548 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportSegmentTuple.py
--rw-r--r--   0 root         (0) root         (0)      916 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportVertexTuple.py
--rw-r--r--   0 root         (0) root         (0)     1231 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbLinkedEdge.py
--rw-r--r--   0 root         (0) root         (0)      487 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbLinkedModel.py
--rw-r--r--   0 root         (0) root         (0)     1983 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbLinkedSegment.py
--rw-r--r--   0 root         (0) root         (0)      914 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbLinkedVertex.py
--rw-r--r--   0 root         (0) root         (0)      539 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbModelSetTuple.py
--rw-r--r--   0 root         (0) root         (0)     3644 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceConfigRuleTuple.py
--rw-r--r--   0 root         (0) root         (0)     1364 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceConfigTuple.py
--rw-r--r--   0 root         (0) root         (0)      753 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceResultEdgeTuple.py
--rw-r--r--   0 root         (0) root         (0)     1297 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      581 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceResultVertexTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2022-11-14 05:34:29.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:43.240585 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      400 2022-11-14 05:37:43.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11234 2022-11-14 05:37:43.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:37:43.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:37:43.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-14 05:37:43.000000 peek-plugin-graphdb-3.3.3/peek_plugin_graphdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:37:43.259585 peek-plugin-graphdb-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2496 2022-11-14 05:37:42.000000 peek-plugin-graphdb-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.141197 peek-plugin-graphdb-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      400 2023-04-12 11:06:32.140197 peek-plugin-graphdb-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      288 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.130197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-04-12 11:06:31.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.131197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.131197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.131197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.ts
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/graphdb.component.html
+-rw-r--r--   0 root         (0) root         (0)      461 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/graphdb.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/graphdb.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.131197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/status/
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/status/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.131197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      560 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.132197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.132197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      954 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/26f8d213ba06_tracerule_propname_nullable.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/6dac32ecea20_added_trccfg_title.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10556 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/bdc665a4d160_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/d762bc44dbb3_change_to_biginteger.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.132197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/graphdb.component.ts
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/graphdb.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/graphdb.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.132197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/view-trace/
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/view-trace/view.component.ts
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/view-trace/view.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.132197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.133197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     8217 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/ClientTupleObservable.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/TupleActionProcessorProxy.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/TupleObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.133197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)     4120 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/FastGraphDb.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/ItemKeyIndexCacheController.py
+-rw-r--r--   0 root         (0) root         (0)    15818 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/PrivateRunTrace.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/SegmentCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/TraceConfigCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/TracerController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.133197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/handlers/ItemKeyIndexCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/handlers/SegmentCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.134197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/GraphDbDoesKeyExistTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/ItemKeyIndexUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/PackedItemKeyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/PackedSegmentTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/SegmentUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/TraceConfigTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/TraceResultTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.134197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/
+-rw-r--r--   0 root         (0) root         (0)    10072 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.134197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)      983 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/admin_backend/ViewSegmentHandler.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.134197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/api/GraphDbApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.135197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/SegmentChunkIndexUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/SegmentIndexChunkLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.135197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/ImportController.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/ItemKeyIndexCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     3988 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/SegmentIndexCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/StatusController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.135197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/graph/
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/graph/GrpahModelController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/graph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.135197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/tuple_providers/ModelSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/tuple_providers/ServerStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.136197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      710 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbEncodedChunk.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbModelSet.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbSegment.py
+-rw-r--r--   0 root         (0) root         (0)     2770 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbTraceConfig.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbTraceConfigRule.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/ItemKeyIndex.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/ItemKeyIndexCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/ItemKeyIndexEncodedChunk.py
+-rw-r--r--   0 root         (0) root         (0)     7777 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.136197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      942 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/GraphDbEncodedChunkTuple.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/GraphDbPackedItemKeyTuple.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/GraphDbPackedSegmentTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/ItemKeyIndexUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/ItemKeyTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/SegmentIndexUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/ServerStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.136197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.137197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     7174 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexImporterTask.py
+-rw-r--r--   0 root         (0) root         (0)     6588 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     8253 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexImporterTask.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/TraceConfigImporterTask.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/_ItemKeyIndexCalcChunkKey.py
+-rw-r--r--   0 root         (0) root         (0)      717 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/_SegmentIndexCalcChunkKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.137197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)      437 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.137197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/status/
+-rw-r--r--   0 root         (0) root         (0)    29513 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/status/status.png
+-rw-r--r--   0 root         (0) root         (0)      678 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/status/status.rst
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/trace_logic.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.137197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/both-doc/offline_support.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.138197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      424 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbDoesKeyExistTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      717 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbLinkedEdge.ts
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbLinkedModel.ts
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbLinkedSegment.ts
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbLinkedVertex.ts
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbModelSetTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbService.ts
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbTraceResultEdgeTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      973 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbTraceResultTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      481 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbTraceResultVertexTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.138197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/GraphDbOfflineTupleCacherService.ts
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/GraphDbTupleService.ts
+-rw-r--r--   0 root         (0) root         (0)      424 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/PluginNames.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.138197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/admin/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/admin/ServerStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      571 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/admin/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.139197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/
+-rw-r--r--   0 root         (0) root         (0)      568 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/GraphDbPackedItemKeyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      442 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexEncodedChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    20114 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      279 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.139197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/EncodedSegmentChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      568 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/GraphDbPackedSegmentTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    19910 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/PrivateSegmentLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/SegmentIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      250 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.139197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tracer-service/
+-rw-r--r--   0 root         (0) root         (0)    17950 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateRunTrace.ts
+-rw-r--r--   0 root         (0) root         (0)     8437 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateTracerService.ts
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tracer-service/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.139197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigRuleTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      929 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     3636 2023-04-12 11:06:31.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.139197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/server/
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/server/GraphDbApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.140197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbDoesKeyExistTuple.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportEdgeTuple.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportSegmentLinkTuple.py
+-rw-r--r--   0 root         (0) root         (0)     3548 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportSegmentTuple.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportVertexTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbLinkedEdge.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbLinkedModel.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbLinkedSegment.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbLinkedVertex.py
+-rw-r--r--   0 root         (0) root         (0)      539 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbModelSetTuple.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceConfigRuleTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceConfigTuple.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceResultEdgeTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      581 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceResultVertexTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-12 11:03:20.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:32.131197 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      400 2023-04-12 11:06:32.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10871 2023-04-12 11:06:32.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:06:32.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:06:32.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-12 11:06:32.000000 peek-plugin-graphdb-3.4.0/peek_plugin_graphdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:06:32.141197 peek-plugin-graphdb-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-04-12 11:06:31.000000 peek-plugin-graphdb-3.4.0/setup.py
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/__init__.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/graphdb.component.html` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/graphdb.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/graphdb.module.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/graphdb.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/status/status.component.html` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/admin-app/status/status.component.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/admin-app/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/agent/AgentEntryHook.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/script.py.mako` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/26f8d213ba06_tracerule_propname_nullable.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/26f8d213ba06_tracerule_propname_nullable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/6dac32ecea20_added_trccfg_title.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/6dac32ecea20_added_trccfg_title.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/bdc665a4d160_initial_tables.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/bdc665a4d160_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/alembic/versions/d762bc44dbb3_change_to_biginteger.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/alembic/versions/d762bc44dbb3_change_to_biginteger.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/graphdb.component.web.html` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/graphdb.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/graphdb.module.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/graphdb.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-app/view-trace/view.component.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-app/view-trace/view.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/both-assets/icon.png` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/ClientEntryHook.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/ClientTupleObservable.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/ClientTupleObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/TupleObservableProxy.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/TupleObservableProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/FastGraphDb.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/FastGraphDb.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/ItemKeyIndexCacheController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/ItemKeyIndexCacheController.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     """
 
     _ChunkedTuple = ItemKeyIndexEncodedChunk
     _UpdateDateTupleABC = ItemKeyIndexUpdateDateTuple
     _chunkLoadRpcMethod = ItemKeyIndexChunkLoadRpc.loadItemKeyIndexChunks
     _chunkIndexDeltaRpcMethod = ItemKeyIndexChunkLoadRpc.loadItemKeyIndexDelta
-    _updateFromServerFilt = clientItemKeyIndexUpdateFromServerFilt
+    _updateFromLogicFilt = clientItemKeyIndexUpdateFromServerFilt
     _logger = logger
 
     def getSegmentKeys(self, modelSetKey: str, vertexKey: str) -> List[str]:
 
         chunkKey = makeChunkKeyForItemKey(modelSetKey, vertexKey)
         # noinspection PyTypeChecker
         chunk: ItemKeyIndexEncodedChunk = self.encodedChunk(chunkKey)
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/PrivateRunTrace.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/PrivateRunTrace.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/SegmentCacheController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/SegmentCacheController.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,26 @@
 
     """
 
     _ChunkedTuple = GraphDbEncodedChunkTuple
     _UpdateDateTupleABC = SegmentIndexUpdateDateTuple
     _chunkLoadRpcMethod = SegmentIndexChunkLoadRpc.loadSegmentChunks
     _chunkIndexDeltaRpcMethod = SegmentIndexChunkLoadRpc.loadSegmentIndexDelta
-    _updateFromServerFilt = clientSegmentUpdateFromServerFilt
+    _updateFromLogicFilt = clientSegmentUpdateFromServerFilt
     _logger = logger
 
     def setFastGraphDb(self, fastGraphDb):
         self._fastGraphDb = fastGraphDb
 
     def shutdown(self):
         ACICacheControllerABC.shutdown(self)
         self._fastGraphDb = None
 
     @inlineCallbacks
-    def _notifyOfChunkKeysUpdated(self, chunkKeys: List[Any]):
-        yield ACICacheControllerABC._notifyOfChunkKeysUpdated(self, chunkKeys)
-
+    def notifyFastGraphDbModelChunkKeysUpdated(self, chunkKeys: List[Any]):
         chunkKeysUpdatedByModelSet: Dict[str, List[str]] = defaultdict(list)
         for chunkKey in chunkKeys:
             modelSetKey = chunkKey.split(".")[0]
             chunkKeysUpdatedByModelSet[modelSetKey].append(chunkKey)
 
         for modelSetKey, updatedChunkKeys in chunkKeysUpdatedByModelSet.items():
             fastGraphDbModel = self._fastGraphDb.graphForModelSet(modelSetKey)
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/TraceConfigCacheController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/TraceConfigCacheController.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,117 @@
 import logging
 from collections import defaultdict
 from typing import Dict, List, Set, Optional
 
+from vortex.Payload import Payload
+
 from peek_plugin_graphdb._private.PluginNames import graphDbFilt
 from peek_plugin_graphdb._private.server.client_handlers.TraceConfigLoadRpc import (
     TraceConfigLoadRpc,
 )
-from peek_plugin_graphdb.tuples.GraphDbTraceConfigTuple import GraphDbTraceConfigTuple
+from peek_plugin_graphdb.tuples.GraphDbTraceConfigTuple import (
+    GraphDbTraceConfigTuple,
+)
 from twisted.internet.defer import inlineCallbacks
 from vortex.PayloadEndpoint import PayloadEndpoint
 from vortex.PayloadEnvelope import PayloadEnvelope
 from vortex.PayloadFilterKeys import plDeleteKey
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableProxyHandler import (
     TupleDataObservableProxyHandler,
 )
 
 logger = logging.getLogger(__name__)
 
-clientTraceConfigUpdateFromServerFilt = dict(key="clientTraceConfigUpdateFromServer")
+clientTraceConfigUpdateFromServerFilt = dict(
+    key="clientTraceConfigUpdateFromServer"
+)
 clientTraceConfigUpdateFromServerFilt.update(graphDbFilt)
 
 
 class TraceConfigCacheController:
     """TraceConfig Cache Controller
 
     The TraceConfig cache controller stores all the chunks in memory,
     allowing fast access from the mobile and desktop devices.
 
     """
 
     LOAD_CHUNK = 32
 
-    def __init__(self, clientId: str, tupleObservable: TupleDataObservableProxyHandler):
+    def __init__(
+        self, clientId: str, tupleObservable: TupleDataObservableProxyHandler
+    ):
         self._clientId = clientId
         self._tupleObservable = tupleObservable
 
         #: This stores the cache of segment data for the clients
-        self._cache: Dict[str, Dict[str, GraphDbTraceConfigTuple]] = defaultdict(dict)
+        self._cache: Dict[
+            str, Dict[str, GraphDbTraceConfigTuple]
+        ] = defaultdict(dict)
+
+        self._vortexMsgCache: Dict[str, bytes] = {}
 
         self._endpoint = PayloadEndpoint(
-            clientTraceConfigUpdateFromServerFilt, self._processTraceConfigPayload
+            clientTraceConfigUpdateFromServerFilt,
+            self._processTraceConfigPayload,
         )
 
     @inlineCallbacks
     def start(self):
         yield self.reloadCache()
 
     def shutdown(self):
         self._tupleObservable = None
 
         self._endpoint.shutdown()
         self._endpoint = None
 
         self._cache = defaultdict(dict)
 
+        self._vortexMsgCache = {}
+
     @inlineCallbacks
     def reloadCache(self):
         self._cache = defaultdict(dict)
+        self._vortexMsgCache = {}
 
         offset = 0
         while True:
             logger.info(
-                "Loading TraceConfig %s to %s" % (offset, offset + self.LOAD_CHUNK)
+                "Loading TraceConfig %s to %s"
+                % (offset, offset + self.LOAD_CHUNK)
             )
             traceConfigTuples: List[GraphDbTraceConfigTuple] = (
-                yield TraceConfigLoadRpc.loadTraceConfigs(offset, self.LOAD_CHUNK)
+                yield TraceConfigLoadRpc.loadTraceConfigs(
+                    offset, self.LOAD_CHUNK
+                )
             )
 
             if not traceConfigTuples:
                 break
 
             traceConfigsByModelSetKey = defaultdict(list)
             for trace in traceConfigTuples:
                 traceConfigsByModelSetKey[trace.modelSetKey].append(trace)
 
             del traceConfigTuples
 
-            for modelSetKey, traceConfigTuples in traceConfigsByModelSetKey.items():
+            for (
+                modelSetKey,
+                traceConfigTuples,
+            ) in traceConfigsByModelSetKey.items():
                 self._loadTraceConfigIntoCache(modelSetKey, traceConfigTuples)
 
             offset += self.LOAD_CHUNK
 
     @inlineCallbacks
-    def _processTraceConfigPayload(self, payloadEnvelope: PayloadEnvelope, **kwargs):
+    def _processTraceConfigPayload(
+        self, payloadEnvelope: PayloadEnvelope, **kwargs
+    ):
         payload = yield payloadEnvelope.decodePayloadDefer()
 
         dataDict = payload.tuples[0]
 
         if payload.filt.get(plDeleteKey):
             modelSetKey = dataDict["modelSetKey"]
             traceConfigKeys = dataDict["traceConfigKeys"]
@@ -95,30 +119,35 @@
             return
 
         modelSetKey = dataDict["modelSetKey"]
 
         traceConfigTuples: List[GraphDbTraceConfigTuple] = dataDict["tuples"]
         self._loadTraceConfigIntoCache(modelSetKey, traceConfigTuples)
 
-    def _removeTraceConfigFromCache(self, modelSetKey: str, traceConfigKeys: List[str]):
+    def _removeTraceConfigFromCache(
+        self, modelSetKey: str, traceConfigKeys: List[str]
+    ):
+        self._vortexMsgCache.pop(modelSetKey, None)
+
         subCache = self._cache[modelSetKey]
 
         logger.debug(
             "Received TraceConfig deletes from server, %s %s removed",
             modelSetKey,
             len(traceConfigKeys),
         )
 
         for traceConfigKey in traceConfigKeys:
             if traceConfigKey in subCache:
                 subCache.pop(traceConfigKey)
 
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(
-                GraphDbTraceConfigTuple.tupleType(), dict(modelSetKey=modelSetKey)
+                GraphDbTraceConfigTuple.tupleType(),
+                dict(modelSetKey=modelSetKey),
             )
         )
 
     def _loadTraceConfigIntoCache(
         self,
         modelSetKey: str,
         traceConfigTuples: List[GraphDbTraceConfigTuple],
@@ -145,15 +174,16 @@
             modelSetKey,
             len(deletedTraceConfigKeys),
             len(traceKeysUpdated),
         )
 
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(
-                GraphDbTraceConfigTuple.tupleType(), dict(modelSetKey=modelSetKey)
+                GraphDbTraceConfigTuple.tupleType(),
+                dict(modelSetKey=modelSetKey),
             )
         )
 
     def traceConfigTuple(
         self, modelSetKey: str, traceConfigKey: str
     ) -> GraphDbTraceConfigTuple:
         return self._cache[modelSetKey][traceConfigKey]
@@ -164,7 +194,20 @@
         if modelSetKey:
             return list(self._cache[modelSetKey].values())
 
         configs = []
         for configsByKey in self._cache.values():
             configs += configsByKey.values()
         return configs
+
+    def cachedVortexMsgBlocking(self, modelSetKey: str, filt: dict) -> bytes:
+        if modelSetKey in self._vortexMsgCache:
+            return self._vortexMsgCache[modelSetKey]
+
+        data = self.traceConfigTuples(modelSetKey=modelSetKey)
+
+        # Create the vortex message
+        vortexMsg = (
+            Payload(filt, tuples=data).makePayloadEnvelope().toVortexMsg()
+        )
+        self._vortexMsgCache[modelSetKey] = vortexMsg
+        return vortexMsg
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/controller/TracerController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/controller/TracerController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/handlers/ItemKeyIndexCacheHandler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/handlers/ItemKeyIndexCacheHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/GraphDbDoesKeyExistTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/GraphDbDoesKeyExistTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/ItemKeyIndexUpdateDateTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/ItemKeyIndexUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/PackedItemKeyTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/PackedItemKeyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/PackedSegmentTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/PackedSegmentTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/SegmentUpdateDateTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/SegmentUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/TraceConfigTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/TraceConfigTupleProvider.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,10 @@
     @deferToThreadWrapWithLogger(logger)
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
         # the UI doesn't supply the model set at present.
         modelSetKey = tupleSelector.selector.get("modelSetKey")
 
-        data = self._cacheHandler.traceConfigTuples(modelSetKey=modelSetKey)
-
-        # Create the vortex message
-        return Payload(filt, tuples=data).makePayloadEnvelope().toVortexMsg()
+        return self._cacheHandler.cachedVortexMsgBlocking(
+            modelSetKey=modelSetKey, filt=filt
+        )
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/client/tuple_providers/TraceResultTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/client/tuple_providers/TraceResultTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/LogicEntryHook.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/TupleActionProcessor.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/TupleDataObservable.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/admin_backend/ViewSegmentHandler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/admin_backend/ViewSegmentHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/api/GraphDbApi.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/api/GraphDbApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkLoadRpc.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkLoadRpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,30 @@
         yield self.loadItemKeyIndexDelta.start(funcSelf=self)
         logger.debug("RPCs started")
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=graphDbFilt,
         deferToThread=True,
     )
     def loadItemKeyIndexDelta(self, indexEncodedPayload: bytes) -> bytes:
         return self.ckiChunkIndexDeltaBlocking(
             indexEncodedPayload,
             ItemKeyIndexEncodedChunk,
             ItemKeyIndexUpdateDateTuple,
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=graphDbFilt,
         deferToThread=True,
     )
     def loadItemKeyIndexChunks(self, chunkKeys: list[str]) -> list[Tuple]:
         return self.ckiInitialLoadChunksPayloadBlocking(
             chunkKeys, ItemKeyIndexEncodedChunk
         )
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkUpdateHandler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/ItemKeyIndexChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/SegmentChunkIndexUpdateHandler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/SegmentChunkIndexUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/SegmentIndexChunkLoadRpc.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/SegmentIndexChunkLoadRpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,30 +39,30 @@
         yield self.loadSegmentIndexDelta.start(funcSelf=self)
         logger.debug("RPCs started")
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=graphDbFilt,
         deferToThread=True,
     )
     def loadSegmentIndexDelta(self, indexEncodedPayload: bytes) -> bytes:
         return self.ckiChunkIndexDeltaBlocking(
             indexEncodedPayload,
             GraphDbEncodedChunk,
             SegmentIndexUpdateDateTuple,
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=graphDbFilt,
         deferToThread=True,
     )
     def loadSegmentChunks(self, chunkKeys: list[str]) -> list[Tuple]:
         """Load Segment Chunks
 
         Allow the client to incrementally load the chunks.
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigLoadRpc.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigLoadRpc.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigUpdateHandler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/client_handlers/TraceConfigUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/ImportController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/ImportController.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,48 +2,54 @@
 from typing import List
 
 from twisted.internet.defer import inlineCallbacks, Deferred
 
 from peek_plugin_graphdb._private.server.client_handlers.TraceConfigUpdateHandler import (
     TraceConfigUpdateHandler,
 )
-from peek_plugin_graphdb._private.worker.tasks import SegmentIndexImporter
-from peek_plugin_graphdb._private.worker.tasks import TraceConfigImporter
+from peek_plugin_graphdb._private.worker.tasks import SegmentIndexImporterTask
+from peek_plugin_graphdb._private.worker.tasks import TraceConfigImporterTask
 
 logger = logging.getLogger(__name__)
 
 
 class ImportController:
     def __init__(self, traceConfigUpdateHandler: TraceConfigUpdateHandler):
         self._traceConfigUpdateHandler = traceConfigUpdateHandler
 
     def shutdown(self):
         pass
 
     @inlineCallbacks
     def createOrUpdateSegments(self, graphSegmentEncodedPayload: bytes):
-        yield SegmentIndexImporter.createOrUpdateSegments.delay(
+        yield SegmentIndexImporterTask.createOrUpdateSegments.delay(
             graphSegmentEncodedPayload
         )
 
     @inlineCallbacks
     def deleteSegment(self, modelSetKey: str, importGroupHashes: List[str]):
-        yield SegmentIndexImporter.deleteSegment.delay(modelSetKey, importGroupHashes)
+        yield SegmentIndexImporterTask.deleteSegment.delay(
+            modelSetKey, importGroupHashes
+        )
 
     @inlineCallbacks
     def createOrUpdateTraceConfig(self, traceEncodedPayload: bytes) -> Deferred:
-        insertedOrCreated = yield TraceConfigImporter.createOrUpdateTraceConfigs.delay(
-            traceEncodedPayload
+        insertedOrCreated = (
+            yield TraceConfigImporterTask.createOrUpdateTraceConfigs.delay(
+                traceEncodedPayload
+            )
         )
 
         for modelSetKey, traceConfigKeys in insertedOrCreated.items():
             self._traceConfigUpdateHandler.sendCreatedOrUpdatedUpdates(
                 modelSetKey, traceConfigKeys
             )
 
     @inlineCallbacks
     def deleteTraceConfig(
         self, modelSetKey: str, traceConfigKeys: List[str]
     ) -> Deferred:
-        yield TraceConfigImporter.deleteTraceConfig.delay(modelSetKey, traceConfigKeys)
+        yield TraceConfigImporterTask.deleteTraceConfig.delay(
+            modelSetKey, traceConfigKeys
+        )
 
         self._traceConfigUpdateHandler.sendDeleted(modelSetKey, traceConfigKeys)
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/ItemKeyIndexCompilerQueueController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/ItemKeyIndexCompilerQueueController.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,32 @@
 
 
 class _Notifier(ACIProcessorStatusNotifierABC):
     def __init__(self, adminStatusController: StatusController):
         self._adminStatusController = adminStatusController
 
     def setProcessorStatus(self, state: bool, queueSize: int):
-        self._adminStatusController.status.itemKeyIndexCompilerQueueStatus = state
-        self._adminStatusController.status.itemKeyIndexCompilerQueueSize = queueSize
+        self._adminStatusController.status.itemKeyIndexCompilerQueueStatus = (
+            state
+        )
+        self._adminStatusController.status.itemKeyIndexCompilerQueueSize = (
+            queueSize
+        )
         self._adminStatusController.notify()
 
     def addToProcessorTotal(self, delta: int):
         self._adminStatusController.status.itemKeyIndexCompilerQueueProcessedTotal += (
             delta
         )
         self._adminStatusController.notify()
 
     def setProcessorError(self, error: str):
-        self._adminStatusController.status.itemKeyIndexCompilerQueueLastError = error
+        self._adminStatusController.status.itemKeyIndexCompilerQueueLastError = (
+            error
+        )
         self._adminStatusController.notify()
 
 
 class ItemKeyIndexCompilerQueueController(ACIProcessorQueueControllerABC):
     QUEUE_ITEMS_PER_TASK = 10
     POLL_PERIOD_SECONDS = 1.000
 
@@ -70,18 +76,20 @@
         statusController: StatusController,
         clientUpdateHandler: ItemKeyIndexChunkUpdateHandler,
     ):
         ACIProcessorQueueControllerABC.__init__(
             self, dbSessionCreator, _Notifier(statusController)
         )
 
-        self._clientUpdateHandler: ItemKeyIndexChunkUpdateHandler = clientUpdateHandler
+        self._clientUpdateHandler: ItemKeyIndexChunkUpdateHandler = (
+            clientUpdateHandler
+        )
 
     def _sendToWorker(self, block: ACIProcessorQueueBlockItem):
-        from peek_plugin_graphdb._private.worker.tasks.ItemKeyIndexCompiler import (
+        from peek_plugin_graphdb._private.worker.tasks.ItemKeyIndexCompilerTask import (
             compileItemKeyIndexChunk,
         )
 
         return compileItemKeyIndexChunk.delay(block.itemsEncodedPayload)
 
     def _processWorkerResults(self, results):
         self._clientUpdateHandler.sendChunks(results)
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/MainController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/controller/SegmentIndexCompilerQueueController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/controller/SegmentIndexCompilerQueueController.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 )
 from peek_plugin_graphdb._private.server.controller.StatusController import (
     StatusController,
 )
 from peek_plugin_graphdb._private.storage.GraphDbCompilerQueue import (
     GraphDbCompilerQueue,
 )
-from peek_plugin_graphdb._private.storage.GraphDbEncodedChunk import GraphDbEncodedChunk
+from peek_plugin_graphdb._private.storage.GraphDbEncodedChunk import (
+    GraphDbEncodedChunk,
+)
 from peek_plugin_graphdb._private.storage.GraphDbSegment import GraphDbSegment
 
 logger = logging.getLogger(__name__)
 
 
 class _Notifier(ACIProcessorStatusNotifierABC):
     def __init__(self, adminStatusController: StatusController):
@@ -31,15 +33,17 @@
 
     def setProcessorStatus(self, state: bool, queueSize: int):
         self._adminStatusController.status.segmentCompilerQueueStatus = state
         self._adminStatusController.status.segmentCompilerQueueSize = queueSize
         self._adminStatusController.notify()
 
     def addToProcessorTotal(self, delta: int):
-        self._adminStatusController.status.segmentCompilerQueueProcessedTotal += delta
+        self._adminStatusController.status.segmentCompilerQueueProcessedTotal += (
+            delta
+        )
         self._adminStatusController.notify()
 
     def setProcessorError(self, error: str):
         self._adminStatusController.status.segmentCompilerQueueLastError = error
         self._adminStatusController.notify()
 
 
@@ -50,15 +54,19 @@
     QUEUE_BLOCKS_MAX = 20
     QUEUE_BLOCKS_MIN = 4
 
     WORKER_TASK_TIMEOUT = 60.0
 
     _logger = logger
     _QueueDeclarative: ACIProcessorQueueTupleABC = GraphDbCompilerQueue
-    _VacuumDeclaratives = (GraphDbCompilerQueue, GraphDbEncodedChunk, GraphDbSegment)
+    _VacuumDeclaratives = (
+        GraphDbCompilerQueue,
+        GraphDbEncodedChunk,
+        GraphDbSegment,
+    )
 
     def __init__(
         self,
         dbSessionCreator,
         statusController: StatusController,
         clientChunkUpdateHandler: SegmentChunkIndexUpdateHandler,
     ):
@@ -67,15 +75,15 @@
         )
 
         self._clientChunkUpdateHandler: SegmentChunkIndexUpdateHandler = (
             clientChunkUpdateHandler
         )
 
     def _sendToWorker(self, block: ACIProcessorQueueBlockItem):
-        from peek_plugin_graphdb._private.worker.tasks.SegmentIndexCompiler import (
+        from peek_plugin_graphdb._private.worker.tasks.SegmentIndexCompilerTask import (
             compileSegmentChunk,
         )
 
         return compileSegmentChunk.delay(block.itemsEncodedPayload)
 
     def _processWorkerResults(self, results):
         self._clientChunkUpdateHandler.sendChunks(results)
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/graph/GrpahModelController.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/graph/GrpahModelController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/tuple_providers/ModelSetTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/tuple_providers/ModelSetTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/server/tuple_providers/ServerStatusTupleProvider.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/server/tuple_providers/ServerStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/DeclarativeBase.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbCompilerQueue.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbEncodedChunk.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbEncodedChunk.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbModelSet.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbModelSet.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbSegment.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbSegment.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbTraceConfig.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbTraceConfig.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/GraphDbTraceConfigRule.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/GraphDbTraceConfigRule.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/ItemKeyIndex.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/ItemKeyIndex.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/ItemKeyIndexCompilerQueue.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/ItemKeyIndexCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/ItemKeyIndexEncodedChunk.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/ItemKeyIndexEncodedChunk.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/storage/Setting.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/GraphDbEncodedChunkTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/GraphDbEncodedChunkTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/GraphDbPackedItemKeyTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/GraphDbPackedItemKeyTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/GraphDbPackedSegmentTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/GraphDbPackedSegmentTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/ItemKeyIndexUpdateDateTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/ItemKeyIndexUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/ItemKeyTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/ItemKeyTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/SegmentIndexUpdateDateTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/SegmentIndexUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/tuples/ServerStatusTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/tuples/ServerStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/WorkerEntryHook.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/WorkerEntryHook.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 from peek_plugin_graphdb._private.storage.DeclarativeBase import loadStorageTuples
 from peek_plugin_graphdb._private.tuples import loadPrivateTuples
 from peek_plugin_graphdb._private.worker.tasks import (
-    SegmentIndexCompiler,
-    SegmentIndexImporter,
-    TraceConfigImporter,
-    ItemKeyIndexCompiler,
-    ItemKeyIndexImporter,
+    SegmentIndexCompilerTask,
+    SegmentIndexImporterTask,
+    TraceConfigImporterTask,
+    ItemKeyIndexCompilerTask,
+    ItemKeyIndexImporterTask,
 )
 from peek_plugin_graphdb.tuples import loadPublicTuples
 
 logger = logging.getLogger(__name__)
 
 
 class WorkerEntryHook(PluginWorkerEntryHookABC):
@@ -30,13 +30,13 @@
 
     def unload(self):
         logger.debug("unloaded")
 
     @property
     def celeryAppIncludes(self):
         return [
-            TraceConfigImporter.__name__,
-            SegmentIndexImporter.__name__,
-            SegmentIndexCompiler.__name__,
-            ItemKeyIndexImporter.__name__,
-            ItemKeyIndexCompiler.__name__,
+            TraceConfigImporterTask.__name__,
+            SegmentIndexImporterTask.__name__,
+            SegmentIndexCompilerTask.__name__,
+            ItemKeyIndexImporterTask.__name__,
+            ItemKeyIndexCompilerTask.__name__,
         ]
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexCompiler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexCompilerTask.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 2) Process queue
 3) Delete from queue
 """
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileItemKeyIndexChunk(self, payloadEncodedArgs: bytes) -> List[int]:
+def compileItemKeyIndexChunk(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile ItemKeyIndex Index Task
 
     :param self: A celery reference to this task
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
@@ -51,16 +51,21 @@
     transaction = conn.begin()
     try:
         queueItemsByModelSetId = defaultdict(list)
 
         for queueItem in queueItems:
             queueItemsByModelSetId[queueItem.modelSetId].append(queueItem)
 
+        lastUpdateByChunkKey = {}
         for modelSetId, modelSetQueueItems in queueItemsByModelSetId.items():
-            _compileItemKeyIndexChunk(conn, transaction, modelSetId, modelSetQueueItems)
+            lastUpdateByChunkKey.update(
+                _compileItemKeyIndexChunk(
+                    conn, transaction, modelSetId, modelSetQueueItems
+                )
+            )
 
         queueTable = ItemKeyIndexCompilerQueue.__table__
 
         transaction = conn.begin()
         conn.execute(queueTable.delete(queueTable.c.id.in_(queueItemIds)))
         transaction.commit()
 
@@ -68,20 +73,23 @@
         transaction.rollback()
         logger.debug("RETRYING task - %s", e)
         raise self.retry(exc=e, countdown=10)
 
     finally:
         conn.close()
 
-    return list(set([i.chunkKey for i in queueItems]))
+    return lastUpdateByChunkKey
 
 
 def _compileItemKeyIndexChunk(
-    conn, transaction, modelSetId: int, queueItems: List[ItemKeyIndexCompilerQueue]
-) -> None:
+    conn,
+    transaction,
+    modelSetId: int,
+    queueItems: List[ItemKeyIndexCompilerQueue],
+) -> dict[str, str]:
     chunkKeys = list(set([i.chunkKey for i in queueItems]))
 
     compiledTable = ItemKeyIndexEncodedChunk.__table__
     lastUpdate = datetime.now(pytz.utc).isoformat()
 
     startTime = datetime.now(pytz.utc)
 
@@ -94,27 +102,34 @@
     # Get Model Sets
 
     total = 0
     existingHashes = _loadExistingHashes(conn, chunkKeys)
     encKwPayloadByChunkKey = _buildIndex(chunkKeys)
     chunksToDelete = []
 
+    lastUpdateByChunkKey = {}
+
     inserts = []
-    for chunkKey, graphDbIndexChunkEncodedPayload in encKwPayloadByChunkKey.items():
+    for (
+        chunkKey,
+        graphDbIndexChunkEncodedPayload,
+    ) in encKwPayloadByChunkKey.items():
         m = hashlib.sha256()
         m.update(graphDbIndexChunkEncodedPayload)
         encodedHash = b64encode(m.digest()).decode()
 
         # Compare the hash, AND delete the chunk key
         if chunkKey in existingHashes:
             # At this point we could decide to do an update instead,
             # but inserts are quicker
             if encodedHash == existingHashes.pop(chunkKey):
                 continue
 
+        lastUpdateByChunkKey[str(chunkKey)] = lastUpdate
+
         chunksToDelete.append(chunkKey)
         inserts.append(
             dict(
                 modelSetId=modelSetId,
                 chunkKey=chunkKey,
                 encodedData=graphDbIndexChunkEncodedPayload,
                 encodedHash=encodedHash,
@@ -123,18 +138,22 @@
         )
 
     # Add any chnuks that we need to delete that we don't have new data for, here
     chunksToDelete.extend(list(existingHashes))
 
     if chunksToDelete:
         # Delete the old chunks
-        conn.execute(compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete)))
+        conn.execute(
+            compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete))
+        )
 
     if inserts:
-        newIdGen = CeleryDbConn.prefetchDeclarativeIds(ItemKeyIndex, len(inserts))
+        newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+            ItemKeyIndex, len(inserts)
+        )
         for insert in inserts:
             insert["id"] = next(newIdGen)
 
     transaction.commit()
     transaction = conn.begin()
 
     if inserts:
@@ -152,14 +171,16 @@
     transaction.commit()
     logger.info(
         "Compiled and Committed %s EncodedItemKeyIndexChunks in %s",
         total,
         (datetime.now(pytz.utc) - startTime),
     )
 
+    return lastUpdateByChunkKey
+
 
 def _loadExistingHashes(conn, chunkKeys: List[str]) -> Dict[str, str]:
     compiledTable = ItemKeyIndexEncodedChunk.__table__
 
     results = conn.execute(
         select(
             columns=[compiledTable.c.chunkKey, compiledTable.c.encodedHash],
@@ -189,33 +210,38 @@
         )
 
         # Create the ChunkKey -> {id -> packedJson, id -> packedJson, ....]
         packagedJsonByObjIdByChunkKey = defaultdict(lambda: defaultdict(list))
 
         for item in indexQry:
             (
-                packagedJsonByObjIdByChunkKey[item.chunkKey][item.itemKey].append(
-                    item.segmentKey
-                )
+                packagedJsonByObjIdByChunkKey[item.chunkKey][
+                    item.itemKey
+                ].append(item.segmentKey)
             )
 
         encPayloadByChunkKey = {}
 
         # Sort each bucket by the key
-        for chunkKey, segmentKeysByItemKey in packagedJsonByObjIdByChunkKey.items():
+        for (
+            chunkKey,
+            segmentKeysByItemKey,
+        ) in packagedJsonByObjIdByChunkKey.items():
             # Convert the list to a json string, this reduces the memory footprint when
             # searching the index.
             packedJsonByKey = {
                 itemKey: json.dumps(segmentKeys)
                 for itemKey, segmentKeys in segmentKeysByItemKey.items()
             }
 
             tuples = json.dumps(packedJsonByKey, sort_keys=True)
 
             # Create the blob data for this index.
             # It could/will be found by a binary sort
-            encPayloadByChunkKey[chunkKey] = Payload(tuples=tuples).toEncodedPayload()
+            encPayloadByChunkKey[chunkKey] = (
+                Payload(tuples=tuples).toEncodedPayload().encode()
+            )
 
         return encPayloadByChunkKey
 
     finally:
         session.close()
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexImporter.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexImporterTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexCompiler.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexCompilerTask.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from vortex.Payload import Payload
 
 from peek_plugin_base.worker import CeleryDbConn
 from peek_plugin_base.worker.CeleryApp import celeryApp
 from peek_plugin_graphdb._private.storage.GraphDbCompilerQueue import (
     GraphDbCompilerQueue,
 )
-from peek_plugin_graphdb._private.storage.GraphDbEncodedChunk import GraphDbEncodedChunk
+from peek_plugin_graphdb._private.storage.GraphDbEncodedChunk import (
+    GraphDbEncodedChunk,
+)
 from peek_plugin_graphdb._private.storage.GraphDbSegment import GraphDbSegment
 
 logger = logging.getLogger(__name__)
 
 """ GraphDb Index Compiler
 
 Compile the graphDb indexes
@@ -29,15 +31,15 @@
 2) Process queue
 3) Delete from queue
 """
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileSegmentChunk(self, payloadEncodedArgs: bytes) -> List[int]:
+def compileSegmentChunk(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile GraphDb Index Task
 
     :param self: The reference to this celery task
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
@@ -49,16 +51,21 @@
     transaction = conn.begin()
     try:
         queueItemsByModelSetId = defaultdict(list)
 
         for queueItem in queueItems:
             queueItemsByModelSetId[queueItem.modelSetId].append(queueItem)
 
+        lastUpdateByChunkKey = {}
         for modelSetId, modelSetQueueItems in queueItemsByModelSetId.items():
-            _compileSegmentChunk(conn, transaction, modelSetId, modelSetQueueItems)
+            lastUpdateByChunkKey.update(
+                _compileSegmentChunk(
+                    conn, transaction, modelSetId, modelSetQueueItems
+                )
+            )
 
         queueTable = GraphDbCompilerQueue.__table__
 
         transaction = conn.begin()
         conn.execute(queueTable.delete(queueTable.c.id.in_(queueItemIds)))
         transaction.commit()
 
@@ -66,20 +73,20 @@
         transaction.rollback()
         logger.debug("RETRYING task - %s", e)
         raise self.retry(exc=e, countdown=10)
 
     finally:
         conn.close()
 
-    return list(set([i.chunkKey for i in queueItems]))
+    return lastUpdateByChunkKey
 
 
 def _compileSegmentChunk(
     conn, transaction, modelSetId: int, queueItems: List[GraphDbCompilerQueue]
-) -> None:
+) -> dict[str, str]:
     chunkKeys = list(set([i.chunkKey for i in queueItems]))
 
     compiledTable = GraphDbEncodedChunk.__table__
     lastUpdate = datetime.now(pytz.utc).isoformat()
 
     startTime = datetime.now(pytz.utc)
 
@@ -92,27 +99,34 @@
     # Get Model Sets
 
     total = 0
     existingHashes = _loadExistingHashes(conn, chunkKeys)
     encKwPayloadByChunkKey = _buildIndex(chunkKeys)
     chunksToDelete = []
 
+    lastUpdateByChunkKey = {}
+
     inserts = []
-    for chunkKey, graphDbIndexChunkEncodedPayload in encKwPayloadByChunkKey.items():
+    for (
+        chunkKey,
+        graphDbIndexChunkEncodedPayload,
+    ) in encKwPayloadByChunkKey.items():
         m = hashlib.sha256()
         m.update(graphDbIndexChunkEncodedPayload)
         encodedHash = b64encode(m.digest()).decode()
 
         # Compare the hash, AND delete the chunk key
         if chunkKey in existingHashes:
             # At this point we could decide to do an update instead,
             # but inserts are quicker
             if encodedHash == existingHashes.pop(chunkKey):
                 continue
 
+        lastUpdateByChunkKey[str(chunkKey)] = lastUpdate
+
         chunksToDelete.append(chunkKey)
         inserts.append(
             dict(
                 modelSetId=modelSetId,
                 chunkKey=chunkKey,
                 encodedData=graphDbIndexChunkEncodedPayload,
                 encodedHash=encodedHash,
@@ -121,18 +135,22 @@
         )
 
     # Add any chnuks that we need to delete that we don't have new data for, here
     chunksToDelete.extend(list(existingHashes))
 
     if chunksToDelete:
         # Delete the old chunks
-        conn.execute(compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete)))
+        conn.execute(
+            compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete))
+        )
 
     if inserts:
-        newIdGen = CeleryDbConn.prefetchDeclarativeIds(GraphDbSegment, len(inserts))
+        newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+            GraphDbSegment, len(inserts)
+        )
         for insert in inserts:
             insert["id"] = next(newIdGen)
 
     transaction.commit()
     transaction = conn.begin()
 
     if inserts:
@@ -150,14 +168,16 @@
     transaction.commit()
     logger.info(
         "Compiled and Committed %s EncodedSegmentChunks in %s",
         total,
         (datetime.now(pytz.utc) - startTime),
     )
 
+    return lastUpdateByChunkKey
+
 
 def _loadExistingHashes(conn, chunkKeys: List[str]) -> Dict[str, str]:
     compiledTable = GraphDbEncodedChunk.__table__
 
     results = conn.execute(
         select(
             columns=[compiledTable.c.chunkKey, compiledTable.c.encodedHash],
@@ -170,35 +190,41 @@
 
 def _buildIndex(chunkKeys) -> Dict[str, bytes]:
     session = CeleryDbConn.getDbSession()
 
     try:
         indexQry = (
             session.query(
-                GraphDbSegment.chunkKey, GraphDbSegment.key, GraphDbSegment.segmentJson
+                GraphDbSegment.chunkKey,
+                GraphDbSegment.key,
+                GraphDbSegment.segmentJson,
             )
             .filter(GraphDbSegment.chunkKey.in_(chunkKeys))
             .order_by(GraphDbSegment.key)
             .yield_per(1000)
             .all()
         )
 
         # Create the ChunkKey -> {id -> packedJson, id -> packedJson, ....]
         packagedJsonByObjIdByChunkKey = defaultdict(dict)
 
         for item in indexQry:
-            packagedJsonByObjIdByChunkKey[item.chunkKey][item.key] = item.segmentJson
+            packagedJsonByObjIdByChunkKey[item.chunkKey][
+                item.key
+            ] = item.segmentJson
 
         encPayloadByChunkKey = {}
 
         # Sort each bucket by the key
         for chunkKey, packedJsonByKey in packagedJsonByObjIdByChunkKey.items():
             tuples = json.dumps(packedJsonByKey, sort_keys=True)
 
             # Create the blob data for this index.
             # It will be graphDbed by a binary sort
-            encPayloadByChunkKey[chunkKey] = Payload(tuples=tuples).toEncodedPayload()
+            encPayloadByChunkKey[chunkKey] = (
+                Payload(tuples=tuples).toEncodedPayload().encode()
+            )
 
         return encPayloadByChunkKey
 
     finally:
         session.close()
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexImporter.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/SegmentIndexImporterTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from peek_plugin_graphdb._private.storage.GraphDbCompilerQueue import (
     GraphDbCompilerQueue,
 )
 from peek_plugin_graphdb._private.storage.GraphDbModelSet import GraphDbModelSet
 from peek_plugin_graphdb._private.storage.GraphDbSegment import GraphDbSegment
 from peek_plugin_graphdb._private.tuples.ItemKeyTuple import ItemKeyTuple
 from peek_plugin_base.worker.CeleryApp import celeryApp
-from peek_plugin_graphdb._private.worker.tasks.ItemKeyIndexImporter import (
+from peek_plugin_graphdb._private.worker.tasks.ItemKeyIndexImporterTask import (
     ItemKeyImportTuple,
     loadItemKeys,
     deleteItemKeys,
 )
 from peek_plugin_graphdb._private.worker.tasks._SegmentIndexCalcChunkKey import (
     makeChunkKeyForSegmentKey,
 )
@@ -133,15 +133,17 @@
 def _loadModelSets() -> Dict[str, int]:
     # Get the model set
     engine = CeleryDbConn.getDbEngine()
     conn = engine.connect()
     try:
         modelSetTable = GraphDbModelSet.__table__
         results = list(
-            conn.execute(select(columns=[modelSetTable.c.id, modelSetTable.c.key]))
+            conn.execute(
+                select(columns=[modelSetTable.c.id, modelSetTable.c.key])
+            )
         )
         modelSetIdByKey = {o.key: o.id for o in results}
         del results
 
     finally:
         conn.close()
     return modelSetIdByKey
@@ -157,15 +159,17 @@
         return newItem.id
 
     finally:
         dbSession.close()
 
 
 def _insertOrUpdateObjects(
-    newSegments: List[GraphDbImportSegmentTuple], modelSetId: int, modelSetKey: str
+    newSegments: List[GraphDbImportSegmentTuple],
+    modelSetId: int,
+    modelSetKey: str,
 ) -> None:
     """Insert or Update Objects
 
     1) Find objects and update them
     2) Insert object if the are missing
 
     """
@@ -175,15 +179,17 @@
 
     startTime = datetime.now(pytz.utc)
     importHashSet = set()
 
     chunkKeysForQueue: Set[Tuple[int, str]] = set()
 
     # Get the IDs that we need
-    newIdGen = CeleryDbConn.prefetchDeclarativeIds(GraphDbSegment, len(newSegments))
+    newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+        GraphDbSegment, len(newSegments)
+    )
 
     # Create state arrays
     inserts = []
 
     newItemKeys = []
 
     # Work out which objects have been updated or need inserting
@@ -228,15 +234,17 @@
 
     # TODO: If this fails, we could potentially delete by segment key.
     # But that seems a bit hackish, the agents should delete the old first.
     # Or should they. That might leave a temporary gap in the network.
 
     # Delete old stuff
     if importHashSet:
-        deleteSegment(modelSetKey=modelSetKey, importGroupHashes=list(importHashSet))
+        deleteSegment(
+            modelSetKey=modelSetKey, importGroupHashes=list(importHashSet)
+        )
 
     engine = CeleryDbConn.getDbEngine()
     conn = engine.connect()
     transaction = conn.begin()
 
     try:
         # Insert the GraphDb Objects
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/TraceConfigImporter.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/TraceConfigImporterTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/_ItemKeyIndexCalcChunkKey.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/_ItemKeyIndexCalcChunkKey.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/_private/worker/tasks/_SegmentIndexCalcChunkKey.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/_private/worker/tasks/_SegmentIndexCalcChunkKey.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/admin_tasks.rst` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/overview.rst` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/status/status.png` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/status/status.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/admin-doc/status/status.rst` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/admin-doc/status/status.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbLinkedEdge.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbLinkedEdge.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbLinkedModel.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbLinkedModel.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbLinkedSegment.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbLinkedSegment.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbModelSetTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbModelSetTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbService.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbTraceResultEdgeTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbTraceResultEdgeTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/GraphDbTraceResultTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/GraphDbTraceResultTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/GraphDbOfflineTupleCacherService.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/GraphDbOfflineTupleCacherService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/GraphDbTupleService.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/GraphDbTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/admin/ServerStatusTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/admin/ServerStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/admin/SettingPropertyTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/GraphDbPackedItemKeyTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/GraphDbPackedItemKeyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderService.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderService.ts`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,20 @@
     graphDbCacheStorageName,
     graphDbFilt,
     graphDbTuplePrefix,
 } from "../PluginNames";
 import { ItemKeyIndexEncodedChunkTuple } from "./ItemKeyIndexEncodedChunkTuple";
 import { ItemKeyIndexUpdateDateTuple } from "./ItemKeyIndexUpdateDateTuple";
 import { ItemKeyTuple } from "./ItemKeyTuple";
-import { ItemKeyIndexLoaderStatusTuple } from "./ItemKeyIndexLoaderStatusTuple";
 import { GraphDbModelSetTuple } from "../../GraphDbModelSetTuple";
 import { GraphDbTupleService } from "../GraphDbTupleService";
 import { GraphDbPackedItemKeyTuple } from "./GraphDbPackedItemKeyTuple";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 
 // ----------------------------------------------------------------------------
 
 let clientItemKeyIndexWatchUpdateFromDeviceFilt = extend(
     { key: "clientItemKeyIndexWatchUpdateFromDevice" },
     graphDbFilt
@@ -118,69 +117,86 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new ItemKeyIndexUpdateDateTuple();
+    private index: ItemKeyIndexUpdateDateTuple | null = null;
     private askServerChunks: ItemKeyIndexUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
 
     private _hasLoadedSubject = new Subject<void>();
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject = new Subject<ItemKeyIndexLoaderStatusTuple>();
-    private _status = new ItemKeyIndexLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     private modelSetByIds: { [id: number]: GraphDbModelSetTuple } = {};
     private _hasModelSetLoaded = false;
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         private tupleService: GraphDbTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
+        this._status.pluginName = "peek_plugin_graphdb";
+        this._status.indexName = "Key Index";
 
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(
                 graphDbCacheStorageName + ".item_key"
             )
         );
 
         this.setupVortexSubscriptions();
-        this._notifyStatus();
 
-        this.deviceCacheControllerService.triggerCachingObservable
+        this.deviceCacheControllerService.offlineModeEnabled$
             .pipe(takeUntil(this.onDestroyEvent))
             .pipe(filter((v) => v))
+            .pipe(first())
             .subscribe(() => {
                 this.initialLoad();
+            });
+
+        this.deviceCacheControllerService.triggerCachingStartObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+            .pipe(filter((v) => v))
+            .subscribe(() => {
+                this.askServerForUpdates();
                 this._notifyStatus();
             });
+
+        this.deviceCacheControllerService.triggerCachingResumeObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+
+            .subscribe(() => {
+                this._notifyStatus();
+                this.askServerForNextUpdateChunk();
+            });
     }
 
     isReady(): boolean {
         return this._hasLoaded;
     }
 
     isReadyObservable(): Observable<void> {
         return this._hasLoadedSubject;
     }
 
-    statusObservable(): Observable<ItemKeyIndexLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): ItemKeyIndexLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     get offlineEnabled(): boolean {
         return this.index.initialLoadComplete;
     }
 
@@ -210,81 +226,67 @@
     }
 
     private _notifyReady(): void {
         if (this._hasModelSetLoaded && this._hasLoaded)
             this._hasLoadedSubject.next();
     }
 
-    private _notifyStatus(): void {
-        this._status.cacheForOfflineEnabled =
-            this.deviceCacheControllerService.cachingEnabled;
-        this._status.initialLoadComplete = this.index.initialLoadComplete;
-
-        this._status.loadProgress = Object.keys(
-            this.index.updateDateByChunkKey
-        ).length;
-        for (let chunk of this.askServerChunks)
-            this._status.loadProgress -= Object.keys(
+    private _notifyStatus(paused: boolean = false): void {
+        this._status.lastCheckDate = new Date();
+        this._status.paused = paused;
+        this._status.initialFullLoadComplete = this.index.initialLoadComplete;
+
+        this._status.loadingQueueCount = 0;
+        for (let chunk of this.askServerChunks) {
+            this._status.loadingQueueCount += Object.keys(
                 chunk.updateDateByChunkKey
             ).length;
+        }
 
         this._statusSubject.next(this._status);
-
-        const status = new OfflineCacheStatusTuple();
-        status.pluginName = "peek_plugin_graphdb";
-        status.indexName = "Key Index";
-        status.loadingQueueCount = this._status.loadProgress;
-        status.totalLoadedCount = this._status.loadTotal;
-        status.lastCheckDate = new Date();
-        status.initialFullLoadComplete = this._status.initialLoadComplete;
-        this.deviceCacheControllerService.updateCachingStatus(status);
+        this.deviceCacheControllerService.updateLoaderCachingStatus(
+            this._status
+        );
     }
 
     /** Initial load
      *
      * Load the dates of the index buckets and ask the server if it has any updates.
      */
     private initialLoad(): void {
         this.storage
             .loadTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any[]) => {
                 let tuples: ItemKeyIndexUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new ItemKeyIndexUpdateDateTuple();
+                } else {
                     this.index = tuples[0];
 
                     if (this.index.initialLoadComplete) {
                         this._hasLoaded = true;
                         this._notifyReady();
                     }
                 }
 
-                this.askServerForUpdates();
                 this._notifyStatus();
             });
-
-        this._notifyStatus();
     }
 
     private setupVortexSubscriptions(): void {
         // Services don't have destructors, I'm not sure how to unsubscribe.
         this.vortexService
             .createEndpointObservable(
                 this,
                 clientItemKeyIndexWatchUpdateFromDeviceFilt
             )
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((payloadEnvelope: PayloadEnvelope) => {
                 this.processChunksFromServer(payloadEnvelope);
             });
-
-        // If the vortex service comes back online, update the watch grids.
-        this.vortexStatusService.isOnline
-            .pipe(filter((isOnline) => isOnline == true))
-            .pipe(takeUntil(this.onDestroyEvent))
-            .subscribe(() => this.askServerForUpdates());
     }
 
     private areWeTalkingToTheServer(): boolean {
         return (
             this.deviceCacheControllerService.offlineModeEnabled &&
             this.vortexStatusService.snapshot.isOnline
         );
@@ -308,15 +310,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: ItemKeyIndexUpdateDateTuple = tuplesAny[0];
                 let keys = Object.keys(serverIndex.updateDateByChunkKey);
                 let keysNeedingUpdate: string[] = [];
 
-                this._status.loadTotal = keys.length;
+                this._status.totalLoadedCount = keys.length;
 
                 // Tuples is an array of strings
                 for (let chunkKey of keys) {
                     if (
                         !this.index.updateDateByChunkKey.hasOwnProperty(
                             chunkKey
                         )
@@ -357,38 +359,38 @@
             }
         }
 
         if (count) this.askServerChunks.push(indexChunk);
 
         this.askServerForNextUpdateChunk();
 
-        this._status.lastCheck = new Date();
+        this._status.lastCheckDate = new Date();
     }
 
     private askServerForNextUpdateChunk() {
         if (!this.areWeTalkingToTheServer()) return;
 
         if (this.askServerChunks.length == 0) return;
 
-        this.deviceCacheControllerService //
-            .waitForGarbageCollector()
-            .then(() => {
-                let indexChunk: ItemKeyIndexUpdateDateTuple =
-                    this.askServerChunks.pop();
-                let filt = extend(
-                    {},
-                    clientItemKeyIndexWatchUpdateFromDeviceFilt
-                );
-                filt[cacheAll] = true;
-                let pl = new Payload(filt, [indexChunk]);
-                this.vortexService.sendPayload(pl);
+        if (this.deviceCacheControllerService.isOfflineCachingPaused) {
+            this.saveChunkCacheIndex(true) //
+                .catch((e) => console.log(`ERROR saveChunkCacheIndex: ${e}`));
+            this._notifyStatus(true);
+            return;
+        }
 
-                this._status.lastCheck = new Date();
-                this._notifyStatus();
-            });
+        let indexChunk: ItemKeyIndexUpdateDateTuple =
+            this.askServerChunks.pop();
+        let filt = extend({}, clientItemKeyIndexWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let pl = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(pl);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process ItemKeyIndexes From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderStatusTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/SegmentIndexUpdateDateTuple.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import { addTupleType, Tuple } from "@synerty/vortexjs";
 import { graphDbTuplePrefix } from "../PluginNames";
 
 @addTupleType
-export class ItemKeyIndexLoaderStatusTuple extends Tuple {
+export class SegmentIndexUpdateDateTuple extends Tuple {
     public static readonly tupleName =
-        graphDbTuplePrefix + "ItemKeyIndexLoaderStatusTuple";
-
-    cacheForOfflineEnabled: boolean = false;
+        graphDbTuplePrefix + "SegmentIndexUpdateDateTuple";
     initialLoadComplete: boolean = false;
-    loadProgress: number = 0;
-    loadTotal: number = 0;
-    lastCheck: Date;
+    updateDateByChunkKey: {} = {};
+    // Improve performance of the JSON serialisation
+    protected _rawJonableFields = [
+        "initialLoadComplete",
+        "updateDateByChunkKey",
+    ];
 
     constructor() {
-        super(ItemKeyIndexLoaderStatusTuple.tupleName);
+        super(SegmentIndexUpdateDateTuple.tupleName);
     }
 }
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexUpdateDateTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/GraphDbPackedSegmentTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/GraphDbPackedSegmentTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/segment-loader/PrivateSegmentLoaderService.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/segment-loader/PrivateSegmentLoaderService.ts`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,19 @@
     graphDbFilt,
     graphDbTuplePrefix,
 } from "../PluginNames";
 import { EncodedSegmentChunkTuple } from "./EncodedSegmentChunkTuple";
 import { SegmentIndexUpdateDateTuple } from "./SegmentIndexUpdateDateTuple";
 import { GraphDbLinkedSegment } from "../../GraphDbLinkedSegment";
 import { GraphDbTupleService } from "../GraphDbTupleService";
-import { PrivateSegmentLoaderStatusTuple } from "./PrivateSegmentLoaderStatusTuple";
 
 import { GraphDbPackedSegmentTuple } from "./GraphDbPackedSegmentTuple";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 
 // ----------------------------------------------------------------------------
 
 export interface SegmentResultI {
     [key: string]: GraphDbLinkedSegment;
 }
@@ -124,66 +123,83 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new SegmentIndexUpdateDateTuple();
+    private index: SegmentIndexUpdateDateTuple | null = null;
     private askServerChunks: SegmentIndexUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
 
     private _hasLoadedSubject = new Subject<void>();
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject = new Subject<PrivateSegmentLoaderStatusTuple>();
-    private _status = new PrivateSegmentLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         private tupleService: GraphDbTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
+        this._status.pluginName = "peek_plugin_graphdb";
+        this._status.indexName = "Segment Index";
 
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(
                 graphDbCacheStorageName + ".segment"
             )
         );
 
         this.setupVortexSubscriptions();
-        this._notifyStatus();
 
-        this.deviceCacheControllerService.triggerCachingObservable
+        this.deviceCacheControllerService.offlineModeEnabled$
             .pipe(takeUntil(this.onDestroyEvent))
             .pipe(filter((v) => v))
+            .pipe(first())
             .subscribe(() => {
                 this.initialLoad();
+            });
+
+        this.deviceCacheControllerService.triggerCachingStartObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+            .pipe(filter((v) => v))
+            .subscribe(() => {
+                this.askServerForUpdates();
+                this._notifyStatus();
+            });
+
+        this.deviceCacheControllerService.triggerCachingResumeObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+
+            .subscribe(() => {
                 this._notifyStatus();
+                this.askServerForNextUpdateChunk();
             });
     }
 
     isReady(): boolean {
         return this._hasLoaded;
     }
 
     isReadyObservable(): Observable<void> {
         return this._hasLoadedSubject;
     }
 
-    statusObservable(): Observable<PrivateSegmentLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): PrivateSegmentLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     get offlineEnabled(): boolean {
         return this.index.initialLoadComplete;
     }
 
@@ -265,81 +281,67 @@
             .then((segments) => this._makeDictFromSegments(segments));
     }
 
     private _notifyReady(): void {
         if (this._hasLoaded) this._hasLoadedSubject.next();
     }
 
-    private _notifyStatus(): void {
-        this._status.cacheForOfflineEnabled =
-            this.deviceCacheControllerService.cachingEnabled;
-        this._status.initialLoadComplete = this.index.initialLoadComplete;
-
-        this._status.loadProgress = Object.keys(
-            this.index.updateDateByChunkKey
-        ).length;
-        for (let chunk of this.askServerChunks)
-            this._status.loadProgress -= Object.keys(
+    private _notifyStatus(paused: boolean = false): void {
+        this._status.lastCheckDate = new Date();
+        this._status.paused = paused;
+        this._status.initialFullLoadComplete = this.index.initialLoadComplete;
+
+        this._status.loadingQueueCount = 0;
+        for (let chunk of this.askServerChunks) {
+            this._status.loadingQueueCount += Object.keys(
                 chunk.updateDateByChunkKey
             ).length;
+        }
 
         this._statusSubject.next(this._status);
-
-        const status = new OfflineCacheStatusTuple();
-        status.pluginName = "peek_plugin_graphdb";
-        status.indexName = "Segment Index";
-        status.loadingQueueCount = this._status.loadProgress;
-        status.totalLoadedCount = this._status.loadTotal;
-        status.lastCheckDate = new Date();
-        status.initialFullLoadComplete = this._status.initialLoadComplete;
-        this.deviceCacheControllerService.updateCachingStatus(status);
+        this.deviceCacheControllerService.updateLoaderCachingStatus(
+            this._status
+        );
     }
 
     /** Initial load
      *
      * Load the dates of the index buckets and ask the server if it has any updates.
      */
     private initialLoad(): void {
         this.storage
             .loadTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any[]) => {
                 let tuples: SegmentIndexUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new SegmentIndexUpdateDateTuple();
+                } else {
                     this.index = tuples[0];
 
                     if (this.index.initialLoadComplete) {
                         this._hasLoaded = true;
                         this._notifyReady();
                     }
                 }
 
-                this.askServerForUpdates();
                 this._notifyStatus();
             });
-
-        this._notifyStatus();
     }
 
     private setupVortexSubscriptions(): void {
         // Services don't have destructors, I'm not sure how to unsubscribe.
         this.vortexService
             .createEndpointObservable(
                 this,
                 clientSegmentWatchUpdateFromDeviceFilt
             )
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((payloadEnvelope: PayloadEnvelope) => {
                 this.processChunksFromServer(payloadEnvelope);
             });
-
-        // If the vortex service comes back online, update the watch grids.
-        this.vortexStatusService.isOnline
-            .pipe(filter((isOnline) => isOnline == true))
-            .pipe(takeUntil(this.onDestroyEvent))
-            .subscribe(() => this.askServerForUpdates());
     }
 
     private areWeTalkingToTheServer(): boolean {
         return (
             this.deviceCacheControllerService.offlineModeEnabled &&
             this.vortexStatusService.snapshot.isOnline
         );
@@ -363,15 +365,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: SegmentIndexUpdateDateTuple = tuplesAny[0];
                 let keys = Object.keys(serverIndex.updateDateByChunkKey);
                 let keysNeedingUpdate: string[] = [];
 
-                this._status.loadTotal = keys.length;
+                this._status.totalLoadedCount = keys.length;
 
                 // Tuples is an array of strings
                 for (let chunkKey of keys) {
                     if (
                         !this.index.updateDateByChunkKey.hasOwnProperty(
                             chunkKey
                         )
@@ -412,35 +414,38 @@
             }
         }
 
         if (count) this.askServerChunks.push(indexChunk);
 
         this.askServerForNextUpdateChunk();
 
-        this._status.lastCheck = new Date();
+        this._status.lastCheckDate = new Date();
     }
 
     private askServerForNextUpdateChunk() {
         if (!this.areWeTalkingToTheServer()) return;
 
         if (this.askServerChunks.length == 0) return;
 
-        this.deviceCacheControllerService //
-            .waitForGarbageCollector()
-            .then(() => {
-                let indexChunk: SegmentIndexUpdateDateTuple =
-                    this.askServerChunks.pop();
-                let filt = extend({}, clientSegmentWatchUpdateFromDeviceFilt);
-                filt[cacheAll] = true;
-                let pl = new Payload(filt, [indexChunk]);
-                this.vortexService.sendPayload(pl);
+        if (this.deviceCacheControllerService.isOfflineCachingPaused) {
+            this.saveChunkCacheIndex(true) //
+                .catch((e) => console.log(`ERROR saveChunkCacheIndex: ${e}`));
+            this._notifyStatus(true);
+            return;
+        }
 
-                this._status.lastCheck = new Date();
-                this._notifyStatus();
-            });
+        let indexChunk: SegmentIndexUpdateDateTuple =
+            this.askServerChunks.pop();
+        let filt = extend({}, clientSegmentWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let pl = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(pl);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process Segmentes From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateRunTrace.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateRunTrace.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateTracerService.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateTracerService.ts`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,14 @@
         private vortexStatusService: VortexStatusService,
         private segmentLoader: PrivateSegmentLoaderService,
         private itemKeyLoader: ItemKeyIndexLoaderService,
         private tupleService: GraphDbTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
-
-        this.deviceCacheControllerService.triggerCachingObservable
-            .pipe(takeUntil(this.onDestroyEvent))
-            .pipe(filter((v) => v))
-            .subscribe(() => {
-                // ???
-            });
     }
 
     doesKeyExist(
         modelSetKey: string,
         vertexOrEdgeKey: string
     ): Promise<boolean> {
         if (modelSetKey == null || modelSetKey.length == 0) {
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigRuleTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigRuleTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigTuple.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin-module/index.ts` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin-module/index.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/plugin_package.json` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/plugin_package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9738095238095238%*

 * *Differences: {"'field'": "{delete: ['cfgDir', 'cfgModule']}",*

 * * "'office'": "{delete: ['cfgDir', 'cfgModule']}",*

 * * "'plugin'": "{'version': '3.4.0'}"}*

```diff
@@ -10,16 +10,14 @@
         "docRst": "index.rst",
         "hasApi": true
     },
     "field": {
         "appDir": "_private/both-app",
         "appModule": "graphdb.module#GraphDbModule",
         "assetDir": "_private/both-assets",
-        "cfgDir": "_private/both-cfg",
-        "cfgModule": "graphdb-cfg.module#GraphDbCfgModule",
         "icon": "/assets/peek_plugin_graphdb/icon.png",
         "moduleDir": "plugin-module",
         "rootServices": [
             {
                 "class": "GraphDbTupleService",
                 "file": "_private/GraphDbTupleService"
             },
@@ -51,16 +49,14 @@
         "subprocessGroup": "graphdb"
     },
     "logic": {},
     "office": {
         "appDir": "_private/both-app",
         "appModule": "graphdb.module#GraphDbModule",
         "assetDir": "_private/both-assets",
-        "cfgDir": "_private/both-cfg",
-        "cfgModule": "graphdb-cfg.module#GraphDbCfgModule",
         "icon": "/assets/peek_plugin_graphdb/icon.png",
         "moduleDir": "plugin-module",
         "rootServices": [
             {
                 "class": "GraphDbTupleService",
                 "file": "_private/GraphDbTupleService"
             },
@@ -97,15 +93,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty HQ Pty Ltd",
         "packageName": "peek_plugin_graphdb",
         "title": "Graph DB",
-        "version": "3.3.3",
+        "version": "3.4.0",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "worker",
         "agent",
         "storage",
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/server/GraphDbApiABC.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/server/GraphDbApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportEdgeTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportEdgeTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportSegmentLinkTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportSegmentLinkTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportSegmentTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportSegmentTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbImportVertexTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbImportVertexTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbLinkedEdge.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbLinkedEdge.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbLinkedSegment.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbLinkedSegment.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbLinkedVertex.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbLinkedVertex.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbModelSetTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbModelSetTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceConfigRuleTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceConfigRuleTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceConfigTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceConfigTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceResultEdgeTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceResultEdgeTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceResultTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceResultTuple.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from itertools import chain
 from typing import List, Optional
 
 from vortex.Tuple import Tuple, addTupleType, TupleField
 
 from peek_plugin_graphdb._private.PluginNames import graphDbTuplePrefix
 from peek_plugin_graphdb.tuples.GraphDbTraceResultEdgeTuple import (
     GraphDbTraceResultEdgeTuple,
@@ -40,7 +41,13 @@
     edges: List[GraphDbTraceResultEdgeTuple] = TupleField([])
 
     #:  The vertexes
     vertexes: List[GraphDbTraceResultVertexTuple] = TupleField([])
 
     #:  The message if the trace was aborted
     traceAbortedMessage: Optional[str] = TupleField()
+
+    def allUniqueTracedShapeKeys(self) -> list[str]:
+        edgeKeys = [edge.key for edge in self.edges]
+        vertexes = [vertex.key for vertex in self.vertexes]
+
+        return list(set(chain(edgeKeys, vertexes)))
```

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb/tuples/GraphDbTraceResultVertexTuple.py` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb/tuples/GraphDbTraceResultVertexTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-graphdb-3.3.3/peek_plugin_graphdb.egg-info/SOURCES.txt` & `peek-plugin-graphdb-3.4.0/peek_plugin_graphdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,14 @@
 peek_plugin_graphdb/_private/alembic/versions/d762bc44dbb3_change_to_biginteger.py
 peek_plugin_graphdb/_private/both-app/graphdb.component.ts
 peek_plugin_graphdb/_private/both-app/graphdb.component.web.html
 peek_plugin_graphdb/_private/both-app/graphdb.module.ts
 peek_plugin_graphdb/_private/both-app/view-trace/view.component.ts
 peek_plugin_graphdb/_private/both-app/view-trace/view.component.web.html
 peek_plugin_graphdb/_private/both-assets/icon.png
-peek_plugin_graphdb/_private/both-cfg/graphdb-cfg.component.ts
-peek_plugin_graphdb/_private/both-cfg/graphdb-cfg.component.web.html
-peek_plugin_graphdb/_private/both-cfg/graphdb-cfg.module.ts
 peek_plugin_graphdb/_private/client/ClientEntryHook.py
 peek_plugin_graphdb/_private/client/ClientTupleObservable.py
 peek_plugin_graphdb/_private/client/TupleActionProcessorProxy.py
 peek_plugin_graphdb/_private/client/TupleObservableProxy.py
 peek_plugin_graphdb/_private/client/__init__.py
 peek_plugin_graphdb/_private/client/controller/FastGraphDb.py
 peek_plugin_graphdb/_private/client/controller/ItemKeyIndexCacheController.py
@@ -104,19 +101,19 @@
 peek_plugin_graphdb/_private/tuples/ItemKeyIndexUpdateDateTuple.py
 peek_plugin_graphdb/_private/tuples/ItemKeyTuple.py
 peek_plugin_graphdb/_private/tuples/SegmentIndexUpdateDateTuple.py
 peek_plugin_graphdb/_private/tuples/ServerStatusTuple.py
 peek_plugin_graphdb/_private/tuples/__init__.py
 peek_plugin_graphdb/_private/worker/WorkerEntryHook.py
 peek_plugin_graphdb/_private/worker/__init__.py
-peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexCompiler.py
-peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexImporter.py
-peek_plugin_graphdb/_private/worker/tasks/SegmentIndexCompiler.py
-peek_plugin_graphdb/_private/worker/tasks/SegmentIndexImporter.py
-peek_plugin_graphdb/_private/worker/tasks/TraceConfigImporter.py
+peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexCompilerTask.py
+peek_plugin_graphdb/_private/worker/tasks/ItemKeyIndexImporterTask.py
+peek_plugin_graphdb/_private/worker/tasks/SegmentIndexCompilerTask.py
+peek_plugin_graphdb/_private/worker/tasks/SegmentIndexImporterTask.py
+peek_plugin_graphdb/_private/worker/tasks/TraceConfigImporterTask.py
 peek_plugin_graphdb/_private/worker/tasks/_ItemKeyIndexCalcChunkKey.py
 peek_plugin_graphdb/_private/worker/tasks/_SegmentIndexCalcChunkKey.py
 peek_plugin_graphdb/_private/worker/tasks/__init__.py
 peek_plugin_graphdb/admin-doc/admin_tasks.rst
 peek_plugin_graphdb/admin-doc/index.rst
 peek_plugin_graphdb/admin-doc/overview.rst
 peek_plugin_graphdb/admin-doc/trace_logic.rst
@@ -140,22 +137,20 @@
 peek_plugin_graphdb/plugin-module/_private/PluginNames.ts
 peek_plugin_graphdb/plugin-module/_private/index.ts
 peek_plugin_graphdb/plugin-module/_private/admin/ServerStatusTuple.ts
 peek_plugin_graphdb/plugin-module/_private/admin/SettingPropertyTuple.ts
 peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/GraphDbPackedItemKeyTuple.ts
 peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexEncodedChunkTuple.ts
 peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderService.ts
-peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexLoaderStatusTuple.ts
 peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyIndexUpdateDateTuple.ts
 peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/ItemKeyTuple.ts
 peek_plugin_graphdb/plugin-module/_private/item-key-index-loader/index.ts
 peek_plugin_graphdb/plugin-module/_private/segment-loader/EncodedSegmentChunkTuple.ts
 peek_plugin_graphdb/plugin-module/_private/segment-loader/GraphDbPackedSegmentTuple.ts
 peek_plugin_graphdb/plugin-module/_private/segment-loader/PrivateSegmentLoaderService.ts
-peek_plugin_graphdb/plugin-module/_private/segment-loader/PrivateSegmentLoaderStatusTuple.ts
 peek_plugin_graphdb/plugin-module/_private/segment-loader/SegmentIndexUpdateDateTuple.ts
 peek_plugin_graphdb/plugin-module/_private/segment-loader/index.ts
 peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateRunTrace.ts
 peek_plugin_graphdb/plugin-module/_private/tracer-service/PrivateTracerService.ts
 peek_plugin_graphdb/plugin-module/_private/tracer-service/index.ts
 peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigRuleTuple.ts
 peek_plugin_graphdb/plugin-module/_private/tuples/GraphDbTraceConfigTuple.ts
```

### Comparing `peek-plugin-graphdb-3.3.3/setup.py` & `peek-plugin-graphdb-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_graphdb"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin GraphDB - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

