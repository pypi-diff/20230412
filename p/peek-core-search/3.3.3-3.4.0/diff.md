# Comparing `tmp/peek-core-search-3.3.3.tar.gz` & `tmp/peek-core-search-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-search-3.3.3.tar", last modified: Mon Nov 14 05:35:39 2022, max compression
+gzip compressed data, was "peek-core-search-3.4.0.tar", last modified: Wed Apr 12 11:04:24 2023, max compression
```

## Comparing `peek-core-search-3.3.3.tar` & `peek-core-search-3.4.0.tar`

### file list

```diff
@@ -1,217 +1,227 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.193401 peek-core-search-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-14 05:35:39.193401 peek-core-search-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.181401 peek-core-search-3.3.3/peek_core_search/
--rw-r--r--   0 root         (0) root         (0)      555 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-11-14 05:35:38.000000 peek-core-search-3.3.3/peek_core_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.181401 peek-core-search-3.3.3/peek_core_search/_private/
--rw-r--r--   0 root         (0) root         (0)      224 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.182401 peek-core-search-3.3.3/peek_core_search/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.182401 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-object-type-table/
--rw-r--r--   0 root         (0) root         (0)     1259 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1503 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.182401 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-property-table/
--rw-r--r--   0 root         (0) root         (0)     1572 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-property-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1458 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.182401 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1462 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.182401 peek-core-search-3.3.3/peek_core_search/_private/admin-app/search-component/
--rw-r--r--   0 root         (0) root         (0)     3289 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/search-component/search.component.html
--rw-r--r--   0 root         (0) root         (0)      164 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/search-component/search.component.ts
--rw-r--r--   0 root         (0) root         (0)     2607 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/search.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.182401 peek-core-search-3.3.3/peek_core_search/_private/admin-app/status-component/
--rw-r--r--   0 root         (0) root         (0)     1405 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/status-component/status.component.html
--rw-r--r--   0 root         (0) root         (0)      989 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/admin-app/status-component/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.183401 peek-core-search-3.3.3/peek_core_search/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      557 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.183401 peek-core-search-3.3.3/peek_core_search/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      319 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.184401 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3066 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py
--rw-r--r--   0 root         (0) root         (0)      871 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py
--rw-r--r--   0 root         (0) root         (0)    10042 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)     1497 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py
--rw-r--r--   0 root         (0) root         (0)     1065 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py
--rw-r--r--   0 root         (0) root         (0)      794 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py
--rw-r--r--   0 root         (0) root         (0)     1023 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3215 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.184401 peek-core-search-3.3.3/peek_core_search/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.184401 peek-core-search-3.3.3/peek_core_search/_private/both-app/find-component/
--rw-r--r--   0 root         (0) root         (0)     2810 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/find-component/find.component.html
--rw-r--r--   0 root         (0) root         (0)      633 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/find-component/find.component.scss
--rw-r--r--   0 root         (0) root         (0)     8069 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/find-component/find.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.184401 peek-core-search-3.3.3/peek_core_search/_private/both-app/result-component/
--rw-r--r--   0 root         (0) root         (0)     1261 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/result-component/result.component.html
--rw-r--r--   0 root         (0) root         (0)      214 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/result-component/result.component.scss
--rw-r--r--   0 root         (0) root         (0)     3433 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/result-component/result.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.184401 peek-core-search-3.3.3/peek_core_search/_private/both-app/search-component/
--rw-r--r--   0 root         (0) root         (0)      550 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/search-component/search.component.html
--rw-r--r--   0 root         (0) root         (0)      138 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/search-component/search.component.scss
--rw-r--r--   0 root         (0) root         (0)     1049 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/search-component/search.component.ts
--rw-r--r--   0 root         (0) root         (0)     1464 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-app/search.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.184401 peek-core-search-3.3.3/peek_core_search/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    12730 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.185401 peek-core-search-3.3.3/peek_core_search/_private/both-cfg/
--rw-r--r--   0 root         (0) root         (0)      957 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-cfg/search-cfg.component.html
--rw-r--r--   0 root         (0) root         (0)     1605 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-cfg/search-cfg.component.ts
--rw-r--r--   0 root         (0) root         (0)     1139 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/both-cfg/search-cfg.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.185401 peek-core-search-3.3.3/peek_core_search/_private/client/
--rw-r--r--   0 root         (0) root         (0)     7257 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      507 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      873 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)     1867 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.186401 peek-core-search-3.3.3/peek_core_search/_private/client/controller/
--rw-r--r--   0 root         (0) root         (0)    12295 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/controller/FastKeywordController.py
--rw-r--r--   0 root         (0) root         (0)     3405 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/controller/FastKeywordControllerTest.py
--rw-r--r--   0 root         (0) root         (0)     2025 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/controller/SearchIndexCacheController.py
--rw-r--r--   0 root         (0) root         (0)     4721 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/controller/SearchObjectCacheController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.186401 peek-core-search-3.3.3/peek_core_search/_private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     1103 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/handlers/SearchIndexCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)     1115 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/handlers/SearchObjectCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)      176 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.186401 peek-core-search-3.3.3/peek_core_search/_private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1015 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1019 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.186401 peek-core-search-3.3.3/peek_core_search/_private/server/
--rw-r--r--   0 root         (0) root         (0)    12183 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      532 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     2050 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.187401 peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1640 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py
--rw-r--r--   0 root         (0) root         (0)     1617 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      975 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      579 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.187401 peek-core-search-3.3.3/peek_core_search/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)      774 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/api/SearchApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.187401 peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     3120 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)      801 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)      808 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.188401 peek-core-search-3.3.3/peek_core_search/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)      821 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     4363 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)     4135 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)      691 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/controller/SearchObjectImportController.py
--rw-r--r--   0 root         (0) root         (0)      391 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/controller/StatusController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.188401 peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      914 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1166 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1118 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.189401 peek-core-search-3.3.3/peek_core_search/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      711 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     2081 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/EncodedSearchIndexChunk.py
--rw-r--r--   0 root         (0) root         (0)     1947 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/EncodedSearchObjectChunk.py
--rw-r--r--   0 root         (0) root         (0)     1169 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/SearchIndex.py
--rw-r--r--   0 root         (0) root         (0)      966 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/SearchIndexCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     1207 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObject.py
--rw-r--r--   0 root         (0) root         (0)      971 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObjectCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObjectRoute.py
--rw-r--r--   0 root         (0) root         (0)      793 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObjectTypeTuple.py
--rw-r--r--   0 root         (0) root         (0)      945 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/SearchPropertyTuple.py
--rw-r--r--   0 root         (0) root         (0)     7759 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.189401 peek-core-search-3.3.3/peek_core_search/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      711 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/AdminStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      694 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py
--rw-r--r--   0 root         (0) root         (0)      471 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/SearchResultDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)      563 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py
--rw-r--r--   0 root         (0) root         (0)      692 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/SearchResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.189401 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_index/
--rw-r--r--   0 root         (0) root         (0)     1273 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.190401 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/
--rw-r--r--   0 root         (0) root         (0)     1276 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)      539 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py
--rw-r--r--   0 root         (0) root         (0)     1190 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.190401 peek-core-search-3.3.3/peek_core_search/_private/worker/
--rw-r--r--   0 root         (0) root         (0)     1059 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.190401 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     4453 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py
--rw-r--r--   0 root         (0) root         (0)    19206 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py
--rw-r--r--   0 root         (0) root         (0)     2002 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/KeywordSplitter.py
--rw-r--r--   0 root         (0) root         (0)     3257 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/KeywordSplitterTest.py
--rw-r--r--   0 root         (0) root         (0)     6834 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)     5947 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)      851 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/_CalcChunkKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.190401 peek-core-search-3.3.3/peek_core_search/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.191401 peek-core-search-3.3.3/peek_core_search/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)    69265 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png
--rw-r--r--   0 root         (0) root         (0)    65374 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png
--rw-r--r--   0 root         (0) root         (0)     2677 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)      528 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.191401 peek-core-search-3.3.3/peek_core_search/admin-doc/status/
--rw-r--r--   0 root         (0) root         (0)    37092 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/admin-doc/status/status.png
--rw-r--r--   0 root         (0) root         (0)      724 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/admin-doc/status/status.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.191401 peek-core-search-3.3.3/peek_core_search/both-doc/
--rw-r--r--   0 root         (0) root         (0)      381 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      966 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/both-doc/search_button.png
--rw-r--r--   0 root         (0) root         (0)    31589 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/both-doc/search_filtered.png
--rw-r--r--   0 root         (0) root         (0)    28759 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/both-doc/search_popup.png
--rw-r--r--   0 root         (0) root         (0)     1142 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/both-doc/searching.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.191401 peek-core-search-3.3.3/peek_core_search/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      559 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/SearchObjectTypeTuple.ts
--rw-r--r--   0 root         (0) root         (0)      988 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts
--rw-r--r--   0 root         (0) root         (0)      981 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/SearchResultObjectTuple.ts
--rw-r--r--   0 root         (0) root         (0)     6553 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/SearchService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.192401 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)     1944 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/KeywordSplitter.ts
--rw-r--r--   0 root         (0) root         (0)      534 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)     2697 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/SearchTupleService.ts
--rw-r--r--   0 root         (0) root         (0)     9484 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/fast-keyword-controller.ts
--rw-r--r--   0 root         (0) root         (0)      381 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.192401 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/
--rw-r--r--   0 root         (0) root         (0)      437 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/EncodedSearchIndexChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    17250 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      552 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      595 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      332 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.192401 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/
--rw-r--r--   0 root         (0) root         (0)      440 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/EncodedSearchObjectChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    19188 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      555 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      598 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      340 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.192401 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      652 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)      743 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.192401 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/admin/
--rw-r--r--   0 root         (0) root         (0)      702 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      572 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      310 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)     3086 2022-11-14 05:35:38.000000 peek-core-search-3.3.3/peek_core_search/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.193401 peek-core-search-3.3.3/peek_core_search/server/
--rw-r--r--   0 root         (0) root         (0)     1235 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/server/SearchApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.193401 peek-core-search-3.3.3/peek_core_search/tuples/
--rw-r--r--   0 root         (0) root         (0)      695 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/tuples/ImportSearchObjectRouteTuple.py
--rw-r--r--   0 root         (0) root         (0)     1263 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/tuples/ImportSearchObjectTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2022-11-14 05:34:27.000000 peek-core-search-3.3.3/peek_core_search/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:39.181401 peek-core-search-3.3.3/peek_core_search.egg-info/
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-14 05:35:39.000000 peek-core-search-3.3.3/peek_core_search.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10425 2022-11-14 05:35:39.000000 peek-core-search-3.3.3/peek_core_search.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:39.000000 peek-core-search-3.3.3/peek_core_search.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:39.000000 peek-core-search-3.3.3/peek_core_search.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       75 2022-11-14 05:35:39.000000 peek-core-search-3.3.3/peek_core_search.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-14 05:35:39.000000 peek-core-search-3.3.3/peek_core_search.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:35:39.193401 peek-core-search-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2727 2022-11-14 05:35:38.000000 peek-core-search-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.893213 peek-core-search-3.4.0/peek_core_search/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.893213 peek-core-search-3.4.0/peek_core_search/_private/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.893213 peek-core-search-3.4.0/peek_core_search/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-exclude-search-term-table/
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-object-type-table/
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-property-table/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-property-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/admin-app/search-component/
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/search-component/search.component.html
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/search-component/search.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/search.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/admin-app/status-component/
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/status-component/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/status-component/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/admin-app/tuples/ExcludeSearchStringTable.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.894214 peek-core-search-3.4.0/peek_core_search/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.895213 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py
+-rw-r--r--   0 root         (0) root         (0)      819 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/3dba609610b6_fix_exclude_comment.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/79609b0e25a5_add_full_exclude_terms.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/e51cdf9b7d4c_add_exclude_terms.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.895213 peek-core-search-3.4.0/peek_core_search/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.895213 peek-core-search-3.4.0/peek_core_search/_private/both-app/find-component/
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/find-component/find.component.html
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/find-component/find.component.scss
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/find-component/find.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.895213 peek-core-search-3.4.0/peek_core_search/_private/both-app/result-component/
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/result-component/result.component.html
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/result-component/result.component.scss
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/result-component/result.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.896213 peek-core-search-3.4.0/peek_core_search/_private/both-app/search-component/
+-rw-r--r--   0 root         (0) root         (0)      550 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/search-component/search.component.html
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/search-component/search.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/search-component/search.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-app/search.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.896213 peek-core-search-3.4.0/peek_core_search/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    12730 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.896213 peek-core-search-3.4.0/peek_core_search/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     7303 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.896213 peek-core-search-3.4.0/peek_core_search/_private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)    15042 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/controller/FastKeywordController.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/controller/FastKeywordControllerTest.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/controller/SearchIndexCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/controller/SearchObjectCacheController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-search-3.4.0/peek_core_search/_private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.896213 peek-core-search-3.4.0/peek_core_search/_private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/client/handlers/SearchIndexCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/client/handlers/SearchObjectCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.896213 peek-core-search-3.4.0/peek_core_search/_private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.897214 peek-core-search-3.4.0/peek_core_search/_private/server/
+-rw-r--r--   0 root         (0) root         (0)    12183 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.897214 peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/ExcludeSearchStringTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      741 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.897214 peek-core-search-3.4.0/peek_core_search/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)      774 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/api/SearchApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.897214 peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.898213 peek-core-search-3.4.0/peek_core_search/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)      821 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/controller/SearchObjectImportController.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/controller/StatusController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.898213 peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/ExcludeSearchStringsTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.898213 peek-core-search-3.4.0/peek_core_search/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/EncodedSearchIndexChunk.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/EncodedSearchObjectChunk.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/ExcludeSearchStringTable.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/SearchIndex.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/SearchIndexCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObject.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObjectCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObjectRoute.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObjectTypeTuple.py
+-rw-r--r--   0 root         (0) root         (0)      945 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/SearchPropertyTuple.py
+-rw-r--r--   0 root         (0) root         (0)     7759 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.899213 peek-core-search-3.4.0/peek_core_search/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/AdminStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/ExcludeSearchStringsTuple.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/SearchResultDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/SearchResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.899213 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_index/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.899213 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      539 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.899213 peek-core-search-3.4.0/peek_core_search/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.900213 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     5006 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py
+-rw-r--r--   0 root         (0) root         (0)    20585 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/KeywordSplitter.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/KeywordSplitterTest.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)      851 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/_CalcChunkKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.900213 peek-core-search-3.4.0/peek_core_search/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.900213 peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)    69265 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png
+-rw-r--r--   0 root         (0) root         (0)    65374 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    59417 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/exclude_keyword.png
+-rw-r--r--   0 root         (0) root         (0)    49895 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/general_settings.png
+-rw-r--r--   0 root         (0) root         (0)    45973 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/remove_exclude.png
+-rw-r--r--   0 root         (0) root         (0)      528 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.900213 peek-core-search-3.4.0/peek_core_search/admin-doc/status/
+-rw-r--r--   0 root         (0) root         (0)    37092 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/status/status.png
+-rw-r--r--   0 root         (0) root         (0)      724 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/admin-doc/status/status.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.901214 peek-core-search-3.4.0/peek_core_search/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      966 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/both-doc/search_button.png
+-rw-r--r--   0 root         (0) root         (0)    31589 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/both-doc/search_filtered.png
+-rw-r--r--   0 root         (0) root         (0)    28759 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/both-doc/search_popup.png
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/both-doc/searching.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.901214 peek-core-search-3.4.0/peek_core_search/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/SearchObjectTypeTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      988 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      981 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/SearchResultObjectTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     7550 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/SearchService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.901214 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/KeywordSplitter.ts
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/SearchTupleService.ts
+-rw-r--r--   0 root         (0) root         (0)    11554 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/fast-keyword-controller.ts
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.901214 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-index-loader/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-index-loader/EncodedSearchIndexChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    17206 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-index-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-object-loader/
+-rw-r--r--   0 root         (0) root         (0)      440 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-object-loader/EncodedSearchObjectChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    19221 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-object-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/ExcludeSearchStringsTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      652 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/admin/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      310 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/peek_core_search/server/
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/server/SearchApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/peek_core_search/tuples/
+-rw-r--r--   0 root         (0) root         (0)      695 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/tuples/ImportSearchObjectRouteTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/tuples/ImportSearchObjectTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-12 11:03:18.000000 peek-core-search-3.4.0/peek_core_search/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:24.893213 peek-core-search-3.4.0/peek_core_search.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11075 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/peek_core_search.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:04:24.902213 peek-core-search-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-04-12 11:04:24.000000 peek-core-search-3.4.0/setup.py
```

### Comparing `peek-core-search-3.3.3/peek_core_search/PlatformDependencyTest.py` & `peek-core-search-3.4.0/peek_core_search/PlatformDependencyTest.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/__init__.py` & `peek-core-search-3.4.0/peek_core_search/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 from typing import Type
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-property-table/edit.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-property-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/search-component/search.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/search-component/search.component.html`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,24 @@
                 aria-controls="editSearchObjectType"
                 data-toggle="tab"
                 href="#editSearchObjectType"
                 role="tab"
                 >Edit Search Object Types
             </a>
         </li>
+        <!-- Edit Exclude Search Terms -->
+        <li role="presentation">
+            <a
+                aria-controls="editExcludeString"
+                data-toggle="tab"
+                href="#editExcludeString"
+                role="tab"
+                >Edit Exclude Search Terms
+            </a>
+        </li>
     </ul>
 
     <!-- Tab panes -->
     <div class="tab-content">
         <!-- Home Tab -->
         <div class="tab-pane active" id="home" role="tabpanel">
             <div class="panel panel-default">
@@ -87,9 +97,13 @@
         <div class="tab-pane" id="editSearchProperty" role="tabpanel">
             <pl-search-edit-property></pl-search-edit-property>
         </div>
         <!-- Edit Object Type Tab -->
         <div class="tab-pane" id="editSearchObjectType" role="tabpanel">
             <pl-search-edit-object-type></pl-search-edit-object-type>
         </div>
+        <!-- Edit Object Type Tab -->
+        <div class="tab-pane" id="editExcludeString" role="tabpanel">
+            <pl-search-edit-exclude-search-term></pl-search-edit-exclude-search-term>
+        </div>
     </div>
 </div>
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/search.module.ts` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/search.module.ts`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import {
     searchActionProcessorName,
     searchFilt,
     searchObservableName,
     searchTupleOfflineServiceName,
 } from "@peek/peek_core_search/_private";
 import { NzSwitchModule } from "ng-zorro-antd/switch";
+import { EditExcludeSearchTermComponent } from "./edit-exclude-search-term-table/edit.component";
 
 export function tupleActionPushNameServiceFactory() {
     return new TupleActionPushNameService(
         searchActionProcessorName,
         searchFilt
     );
 }
@@ -76,10 +77,11 @@
     ],
     declarations: [
         SearchComponent,
         EditPropertyComponent,
         EditSettingComponent,
         EditObjectTypeComponent,
         StatusComponent,
+        EditExcludeSearchTermComponent,
     ],
 })
 export class SearchModule {}
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/status-component/status.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/status-component/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/admin-app/status-component/status.component.ts` & `peek-core-search-3.4.0/peek_core_search/_private/admin-app/status-component/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/agent/AgentEntryHook.py` & `peek-core-search-3.4.0/peek_core_search/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/script.py.mako` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/script.py.mako`

 * *Files 4% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
 from alembic import op
 import sqlalchemy as sa
 import geoalchemy2
 ${imports if imports else ""}
 
 def upgrade():
-${upgrades if upgrades else "pass"}
+    ${upgrades if upgrades else "pass"}
 
 
 def downgrade():
-${downgrades if downgrades else "pass"}
+    ${downgrades if downgrades else "pass"}
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py` & `peek-core-search-3.4.0/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/find-component/find.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/find-component/find.component.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,10 @@
-<nz-alert
-    *ngIf="searchNotAvailable$ | async"
-    [nzMessage]="offlineAlertContent"
-    nzType="warning"
->
-    <ng-template #offlineAlertContent>
-        You are offline and offline mode is not enabled.
-        Search is unavailable at this time.
-    </ng-template>
-</nz-alert>
-
 <div class="search-input">
     <nz-input-group [nzSuffix]="suffixTemplate">
         <input
-            (ngModelChange)="searchKeywordOnChange($event)"
             [(ngModel)]="searchString"
             autofocus
             nz-input
             placeholder="Search..."
             type="text"
         />
         <ng-template #suffixTemplate>
@@ -35,15 +23,14 @@
 </div>
 
 <div *ngIf="optionsShown$ | async" class="search-filter">
     <nz-form-item>
         <nz-form-label nzFor="searchPropertyId">Property</nz-form-label>
         <nz-form-control>
             <nz-select
-                (ngModelChange)="searchPropertyOnChange($event)"
                 [(ngModel)]="searchProperty"
                 id="searchPropertyId"
                 name="searchPropertyId"
             >
                 <nz-option
                     *ngFor="let option of searchProperties"
                     [nzLabel]="option.title"
@@ -53,37 +40,58 @@
         </nz-form-control>
     </nz-form-item>
 
     <nz-form-item>
         <nz-form-label nzFor="searchObjectTypesId">Object Type</nz-form-label>
         <nz-form-control>
             <nz-select
-                (ngModelChange)="searchObjectTypesOnChange($event)"
                 [(ngModel)]="searchObjectType"
                 id="searchObjectTypesId"
                 name="searchObjectTypesId"
             >
                 <nz-option
                     *ngFor="let option of searchObjectTypes"
                     [nzLabel]="option.title"
                     [nzValue]="option"
                 ></nz-option>
             </nz-select>
         </nz-form-control>
     </nz-form-item>
 </div>
 
-<div
-    *ngIf="!(resultObjects$ | async)?.length && (firstSearchHasRun$ | async)"
-    class="result-alert"
->
+<div class="result-alert">
     <nz-alert
         nzDescription="Peek could not find any results, please refine your search"
         nzMessage="No Results"
         nzType="info"
+        *ngIf="
+            !(notEnoughTokens$ | async) &&
+            !(resultObjects$ | async)?.length &&
+            (firstSearchHasRun$ | async)
+        "
+    >
+    </nz-alert>
+
+    <nz-alert
+        *ngIf="searchNotAvailable$ | async"
+        [nzMessage]="offlineAlertContent"
+        nzType="warning"
+    >
+        <ng-template #offlineAlertContent>
+            <p>
+                You are offline and offline mode is not enabled. Search is
+                unavailable at this time.
+            </p>
+        </ng-template>
+    </nz-alert>
+
+    <nz-alert
+        *ngIf="notEnoughTokens$ | async"
+        nzMessage="Please enter more text to find what you're looking for."
+        nzType="info"
     >
     </nz-alert>
 </div>
 
 <nz-spin *ngIf="searchInProgress$ | async"></nz-spin>
 
 <result-component
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/find-component/find.component.scss` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/find-component/find.component.scss`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/find-component/find.component.ts` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/find-component/find.component.ts`

 * *Files 7% similar despite different names*

```diff
@@ -29,102 +29,52 @@
 @Component({
     selector: "find-component",
     templateUrl: "find.component.html",
     styleUrls: ["find.component.scss"],
     changeDetection: ChangeDetectionStrategy.OnPush,
 })
 export class FindComponent extends NgLifeCycleEvents implements OnInit {
-    searchString: string = "";
+    _searchString: string = "";
     resultObjects$ = new BehaviorSubject<SearchResultObjectTuple[]>([]);
     searchInProgress$ = new BehaviorSubject<boolean>(false);
     searchProperties: SearchPropertyTuple[] = [];
     searchPropertyStrings: string[] = [];
-    searchProperty: SearchPropertyTuple = new SearchPropertyTuple();
+    _searchProperty: SearchPropertyTuple = new SearchPropertyTuple();
     searchObjectTypes: SearchObjectTypeTuple[] = [];
     searchObjectTypeStrings: string[] = [];
-    searchObjectType: SearchObjectTypeTuple = new SearchObjectTypeTuple();
+    _searchObjectType: SearchObjectTypeTuple = new SearchObjectTypeTuple();
     optionsShown$ = new BehaviorSubject<boolean>(false);
     firstSearchHasRun$ = new BehaviorSubject<boolean>(false);
 
     searchNotAvailable$ = new BehaviorSubject<boolean>(false);
+    notEnoughTokens$ = new BehaviorSubject<boolean>(false);
+
+    private searchNeeded: boolean = false;
 
     private readonly ALL = "All";
     private performAutoCompleteSubject: Subject<string> = new Subject<string>();
 
     constructor(
         private vortexStatusService: VortexStatusService,
         private searchService: SearchService,
         private balloonMsg: BalloonMsgService,
-        private tupleService: SearchTupleService,
-        private deviceCacheControllerService: DeviceOfflineCacheService
+        private tupleService: SearchTupleService
     ) {
         super();
-        this.searchProperty.title = this.ALL;
-        this.searchObjectType.title = this.ALL;
+        this._searchProperty.title = this.ALL;
+        this._searchObjectType.title = this.ALL;
 
         zip(
             this.vortexStatusService.isOnline,
-            this.deviceCacheControllerService.offlineModeEnabled$
+            this.searchService.canSearchOffline$
         )
             .pipe(map((values) => !values[0] && !values[1]))
             .subscribe((state) => this.searchNotAvailable$.next(state));
     }
 
-    get resultObjects() {
-        return this.resultObjects$.getValue();
-    }
-
-    set resultObjects(value) {
-        this.resultObjects$.next(value);
-    }
-
-    get searchInProgress() {
-        return this.searchInProgress$.getValue();
-    }
-
-    set searchInProgress(value) {
-        this.searchInProgress$.next(value);
-    }
-
-    get optionsShown() {
-        return this.optionsShown$.getValue();
-    }
-
-    set optionsShown(value) {
-        this.optionsShown$.next(value);
-    }
-
-    get firstSearchHasRun() {
-        return this.firstSearchHasRun$.getValue();
-    }
-
-    set firstSearchHasRun(value) {
-        this.firstSearchHasRun$.next(value);
-    }
-
-    get getSearchPropertyName(): string | null {
-        const prop = this.searchProperty;
-        if (prop.title != this.ALL && prop.name != null && prop.name.length) {
-            return prop.name;
-        }
-        return null;
-    }
-
-    get getSearchObjectTypeId(): number | null {
-        const objProp = this.searchObjectType;
-        if (
-            objProp.title != this.ALL &&
-            objProp.name != null &&
-            objProp.name.length
-        ) {
-            return objProp.id;
-        }
-        return null;
-    }
-
     ngOnInit() {
         const propTs = new TupleSelector(SearchPropertyTuple.tupleName, {});
         this.tupleService.offlineObserver
             .subscribeToTupleSelector(propTs)
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((v: SearchPropertyTuple[]) => {
                 this.updateSearchProperties(v);
@@ -150,53 +100,129 @@
         // Only emit if value is different from previous value
         this.performAutoCompleteSubject
             .pipe(
                 debounceTime(500),
                 distinctUntilChanged(),
                 takeUntil(this.onDestroyEvent)
             )
-            .subscribe(() => this.performAutoComplete());
+            .subscribe((value) => this.debouncedSetSearchString(value));
 
         this.vortexStatusService.isOnline
             .pipe(
                 takeUntil(this.onDestroyEvent),
                 filter((online) => online)
             )
             .subscribe(() => this.performAutoComplete());
     }
 
     resetSearch(): void {
-        this.searchString = "";
+        this._searchString = "";
         this.resultObjects = [];
         this.firstSearchHasRun = false;
         this.searchInProgress = false;
     }
 
-    searchKeywordOnChange($event): void {
-        this.searchString = $event;
-        this.performAutoCompleteSubject.next($event);
+    get searchString() {
+        return this._searchString;
+    }
+
+    set searchString(value: string) {
+        this.performAutoCompleteSubject.next(value);
     }
 
-    searchPropertyOnChange($event): void {
-        this.searchProperty = $event;
+    private debouncedSetSearchString(value: string) {
+        this._searchString = value;
         this.performAutoComplete();
     }
 
-    searchObjectTypesOnChange($event): void {
-        this.searchObjectType = $event;
+    get searchProperty() {
+        return this._searchProperty;
+    }
+
+    set searchProperty(value: SearchPropertyTuple) {
+        this._searchProperty = value;
+        this.performAutoComplete();
+    }
+
+    get searchObjectType() {
+        return this._searchObjectType;
+    }
+
+    set searchObjectType(value: SearchObjectTypeTuple) {
+        this._searchObjectType = value;
         this.performAutoComplete();
     }
 
+    get resultObjects() {
+        return this.resultObjects$.getValue();
+    }
+
+    set resultObjects(value: SearchResultObjectTuple[]) {
+        this.resultObjects$.next(value);
+    }
+
+    get notEnoughTokens() {
+        return this.notEnoughTokens$.getValue();
+    }
+
+    set notEnoughTokens(value: boolean) {
+        this.notEnoughTokens$.next(value);
+    }
+
+    get searchInProgress() {
+        return this.searchInProgress$.getValue();
+    }
+
+    set searchInProgress(value) {
+        this.searchInProgress$.next(value);
+    }
+
+    get optionsShown() {
+        return this.optionsShown$.getValue();
+    }
+
+    set optionsShown(value) {
+        this.optionsShown$.next(value);
+    }
+
+    get firstSearchHasRun() {
+        return this.firstSearchHasRun$.getValue();
+    }
+
+    set firstSearchHasRun(value) {
+        this.firstSearchHasRun$.next(value);
+    }
+
+    get getSearchPropertyName(): string | null {
+        const prop = this._searchProperty;
+        if (prop.title != this.ALL && prop.name != null && prop.name.length) {
+            return prop.name;
+        }
+        return null;
+    }
+
+    get getSearchObjectTypeId(): number | null {
+        const objProp = this._searchObjectType;
+        if (
+            objProp.title != this.ALL &&
+            objProp.name != null &&
+            objProp.name.length
+        ) {
+            return objProp.id;
+        }
+        return null;
+    }
+
     private updateSearchProperties(v: SearchPropertyTuple[]): void {
         // Create the empty item
         const all = new SearchPropertyTuple();
         all.title = "All";
 
-        if (this.searchProperty.title === all.title) {
-            this.searchProperty = all;
+        if (this._searchProperty.title === all.title) {
+            this._searchProperty = all;
         }
 
         // Update the search objects
         this.searchProperties = [...v];
         this.searchProperties.splice(0, 0, all);
 
         // Set the string array and lookup by id
@@ -208,16 +234,16 @@
     }
 
     private updateSearchObjectTypes(v: SearchObjectTypeTuple[]): void {
         // Create the empty item
         const all = new SearchObjectTypeTuple();
         all.title = "All";
 
-        if (this.searchObjectType.title === all.title) {
-            this.searchObjectType = all;
+        if (this._searchObjectType.title === all.title) {
+            this._searchObjectType = all;
         }
 
         // Update the search objects
         this.searchObjectTypes = [...v];
         this.searchObjectTypes.splice(0, 0, all);
 
         // Set the string array, and object type lookup
@@ -225,43 +251,49 @@
 
         for (const item of this.searchObjectTypes) {
             this.searchObjectTypeStrings.push(item.title);
         }
     }
 
     private performAutoComplete(): void {
-        const check = () => {
-            if (this.searchString == null || this.searchString.length === 0) {
-                return false;
-            }
-
-            if (this.searchString.length < 3) {
-                return false;
-            }
+        if (this.searchInProgress) {
+            this.searchNeeded = true;
+            return;
+        }
+        this.searchNeeded = false;
 
-            return true;
-        };
+        // Have they typed enough for a string
+        this.notEnoughTokens = !this.searchService.haveEnoughSearchKeywords(
+            this._searchString
+        );
 
-        if (!check()) {
+        if (this.notEnoughTokens) {
             this.resultObjects = [];
             return;
         }
 
+        const thisSearchesSearchString = this._searchString;
+
         this.searchInProgress = true;
         this.searchService
             .getObjects(
                 this.getSearchPropertyName,
                 this.getSearchObjectTypeId,
-                this.searchString
+                thisSearchesSearchString
             )
             .then((results: SearchResultObjectTuple[]) => {
-                this.resultObjects = results;
+                if (this._searchString === thisSearchesSearchString) {
+                    this.resultObjects = results;
+                } else {
+                    this.resultObjects = [];
+                }
             })
             .catch((e: string) => {
                 this.balloonMsg.showError(`Find Failed:${e}`);
             })
             .then(() => {
                 this.searchInProgress = false;
                 this.firstSearchHasRun = true;
+                if (this.searchNeeded) this.performAutoComplete();
             });
     }
 }
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/result-component/result.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/result-component/result.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/result-component/result.component.ts` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/result-component/result.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/search-component/search.component.html` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/search-component/search.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/search-component/search.component.ts` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/search-component/search.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-app/search.module.ts` & `peek-core-search-3.4.0/peek_core_search/_private/both-app/search.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/both-assets/icon.png` & `peek-core-search-3.4.0/peek_core_search/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/ClientEntryHook.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/ClientEntryHook.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,17 @@
 
         searchObjectCacheController.setCacheHandler(searchObjectCacheHandler)
 
         # ----------------
         # Fast Keyword Controller
 
         fastKeywordController = FastKeywordController(
-            searchObjectCacheController, searchIndexCacheController
+            searchObjectCacheController,
+            searchIndexCacheController,
+            serverTupleObserver,
         )
         self._loadedObjects.append(fastKeywordController)
 
         searchIndexCacheController.setFastKeywordController(
             fastKeywordController
         )
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/TupleDataObservable.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/controller/FastKeywordController.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/controller/FastKeywordController.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,32 +10,46 @@
 
 import pytz
 import json
 from twisted.internet.defer import inlineCallbacks, Deferred
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 from vortex.TupleAction import TupleActionABC
+from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleActionProcessor import TupleActionProcessorDelegateABC
+from vortex.handler.TupleDataObserverClient import TupleDataObserverClient
 
 from peek_core_search._private.client.controller.SearchIndexCacheController import (
     SearchIndexCacheController,
 )
 from peek_core_search._private.client.controller.SearchObjectCacheController import (
     SearchObjectCacheController,
 )
 from peek_core_search._private.storage.EncodedSearchIndexChunk import (
     EncodedSearchIndexChunk,
 )
+from peek_core_search._private.tuples.ExcludeSearchStringsTuple import (
+    ExcludeSearchStringsTuple,
+)
 from peek_core_search._private.tuples.KeywordAutoCompleteTupleAction import (
     KeywordAutoCompleteTupleAction,
 )
 from peek_core_search._private.tuples.search_object.SearchResultObjectTuple import (
     SearchResultObjectTuple,
 )
 from peek_core_search._private.worker.tasks.KeywordSplitter import (
+    filterExcludedFullTerms,
+)
+from peek_core_search._private.worker.tasks.KeywordSplitter import (
+    filterExcludedPartialTerms,
+)
+from peek_core_search._private.worker.tasks.KeywordSplitter import (
+    prepareExcludedPartialTermsForFind,
+)
+from peek_core_search._private.worker.tasks.KeywordSplitter import (
     splitPartialKeywords,
     splitFullKeywords,
     _splitFullTokens,
 )
 from peek_core_search._private.worker.tasks._CalcChunkKey import (
     makeSearchIndexChunkKey,
 )
@@ -44,32 +58,80 @@
 
 
 class FastKeywordController(TupleActionProcessorDelegateABC):
     def __init__(
         self,
         objectCacheController: SearchObjectCacheController,
         indexCacheController: SearchIndexCacheController,
+        serverTupleObserver: TupleDataObserverClient,
     ):
         self._objectCacheController = objectCacheController
         self._indexCacheController = indexCacheController
         self._objectIdsByKeywordByPropertyKeyByChunkKey: Dict[
             str, Dict[str, Dict[str, List[int]]]
         ] = {}
 
+        self.excludedPartialSearchTerms: list[str] = []
+        self.excludedFullSearchTerms: set[str] = set()
+
+        excludeStringsTs = TupleSelector(
+            ExcludeSearchStringsTuple.tupleName(), {}
+        )
+
+        def excludeCallback(tuples):
+            if tuples:
+                self.excludedPartialSearchTerms = (
+                    prepareExcludedPartialTermsForFind(
+                        tuples[0].excludedPartialSearchTerms
+                    )
+                )
+
+                self.excludedFullSearchTerms = set(
+                    tuples[0].excludedFullSearchTerms
+                )
+
+        self._excludedSubscription = (
+            serverTupleObserver.subscribeToTupleSelector(
+                excludeStringsTs
+            ).subscribe(excludeCallback)
+        )
+
     def shutdown(self):
         self._objectCacheController = None
         self._indexCacheController = None
         self._objectIdsByKeywordByPropertyKeyByChunkKey = {}
+        self.excludedPartialSearchTerms = []
+        self.excludedFullSearchTerms = set()
+
+        # Ok, we won't unsubscribe...
+        # AttributeError: 'AnonymousDisposable' object has no attribute 'unsubscribe'
+        # self._excludedSubscription.unsubscribe()
+
+    def haveEnoughSearchKeywords(self, keywordsString: str) -> bool:
+        keywordsString = filterExcludedFullTerms(
+            self.excludedFullSearchTerms, keywordsString
+        )
+        kw = filterExcludedPartialTerms(
+            self.excludedPartialSearchTerms, keywordsString
+        )
+        return kw and 3 <= len(kw)
 
     @inlineCallbacks
     def processTupleAction(self, tupleAction: TupleActionABC) -> Deferred:
         assert isinstance(
             tupleAction, KeywordAutoCompleteTupleAction
         ), "Tuple is not a KeywordAutoCompleteTupleAction"
 
+        if not self.haveEnoughSearchKeywords(tupleAction.searchString):
+            logger.debug(
+                f"Skipping search for '${tupleAction.searchString}'"
+                f" as it's too short after excluding keywords"
+            )
+            return []
+
         startTime = datetime.now(pytz.utc)
 
         objectIds = yield self._getObjectIdsForSearchString(
             tupleAction.searchString, tupleAction.propertyName
         )
 
         results = yield self._objectCacheController.getObjects(
@@ -160,29 +222,33 @@
         :rtype List[int]
 
         """
         logger.debug("Started search with string |%s|", searchString)
 
         # ---------------
         # Search for fulls
-        fullTokens = splitFullKeywords(searchString)
+        fullTokens = splitFullKeywords(
+            self.excludedFullSearchTerms, searchString
+        )
 
         logger.debug("Searching for full tokens |%s|", fullTokens)
 
         # Now lookup any remaining keywords, if any
         resultsByFullKw = self._getObjectIdsForTokensBlocking(
             fullTokens, propertyName
         )
         resultsByFullKw = {k: v for k, v in resultsByFullKw.items() if v}
 
         logger.debug("Found results for full tokens |%s|", set(resultsByFullKw))
 
         # ---------------
         # Search for partials
-        partialTokens = splitPartialKeywords(searchString)
+        partialTokens = splitPartialKeywords(
+            self.excludedPartialSearchTerms, searchString
+        )
         logger.debug("Searching for partial tokens |%s|", partialTokens)
 
         # Now lookup any remaining keywords, if any
         resultsByPartialKw = self._getObjectIdsForTokensBlocking(
             partialTokens, propertyName
         )
         resultsByPartialKw = {k: v for k, v in resultsByPartialKw.items() if v}
@@ -230,34 +296,41 @@
 
             mergedResultsByKw[fullKw] = existing
 
         tokens = _splitFullTokens(searchString)
         for token in tokens:
             token = token.strip("^$")
             existing = mergedResultsByKw.get(token, list())
-            partialKws = splitPartialKeywords(token)
+            partialKws = splitPartialKeywords(
+                self.excludedPartialSearchTerms, token
+            )
 
             if not len(partialKws) <= len(resultsByPartialKwSet):
                 continue
 
             # Union all
-            objectIdsForToken = set(resultsByPartialKw[partialKws.pop()])
+            objectIdsForToken = (
+                set(resultsByPartialKw.get(partialKws.pop(), []))
+                if partialKws
+                else set()
+            )
             while partialKws:
-                objectIdsForToken &= set(resultsByPartialKw[partialKws.pop()])
+                objectIdsForToken &= set(
+                    resultsByPartialKw.get(partialKws.pop(), [])
+                )
 
             existing.extend(list(objectIdsForToken))
 
             mergedResultsByKw[token] = existing
 
         return mergedResultsByKw
 
     def _setIntersectFilterIndexResults(
         self, objectIdsByKw: Dict[str, List[int]]
     ) -> List[int]:
-
         if not objectIdsByKw:
             return []
 
         keys = set(objectIdsByKw)
         twoCharTokens_ = set([t for t in keys if len(t) == 2])
         keys -= twoCharTokens_
 
@@ -335,19 +408,23 @@
          updates from the server.
 
         """
         for chunkKey in chunkKeys:
             encodedChunkTuple = self._indexCacheController.encodedChunk(
                 chunkKey
             )
-            yield self._unpackKeywordsFromChunk(encodedChunkTuple)
+            if encodedChunkTuple:
+                yield self._unpackKeywordsFromChunk(encodedChunkTuple)
+            else:
+                self._objectIdsByKeywordByPropertyKeyByChunkKey.pop(
+                    chunkKey, None
+                )
 
     @deferToThreadWrapWithLogger(logger)
     def _unpackKeywordsFromChunk(self, chunk: EncodedSearchIndexChunk) -> None:
-
         chunkDataTuples = Payload().fromEncodedPayload(chunk.encodedData).tuples
 
         chunkData: Dict[str, Dict[str, List[int]]] = defaultdict(dict)
 
         for data in chunkDataTuples:
             keyword = data[EncodedSearchIndexChunk.ENCODED_DATA_KEYWORD_NUM]
             propertyName = data[
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/controller/FastKeywordControllerTest.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/controller/FastKeywordControllerTest.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/controller/SearchIndexCacheController.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/controller/SearchIndexCacheController.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,25 +33,24 @@
 
     """
 
     _ChunkedTuple = EncodedSearchIndexChunk
     _UpdateDateTupleABC = SearchIndexUpdateDateTuple
     _chunkLoadRpcMethod = ClientChunkLoadRpc.loadSearchIndexChunks
     _chunkIndexDeltaRpcMethod = ClientChunkLoadRpc.loadSearchIndexDelta
-    _updateFromServerFilt = clientSearchIndexUpdateFromServerFilt
+    _updateFromLogicFilt = clientSearchIndexUpdateFromServerFilt
     _logger = logger
 
     def __init__(self, clientId: str, pluginDataDir: Path):
         ACICacheControllerABC.__init__(self, clientId, pluginDataDir)
         self._fastKeywordController = None
 
     def setFastKeywordController(self, fastKeywordController):
         self._fastKeywordController = fastKeywordController
 
     def shutdown(self):
         ACICacheControllerABC.shutdown(self)
         self._fastKeywordController = None
 
     @inlineCallbacks
-    def _notifyOfChunkKeysUpdated(self, chunkKeys: List[Any]):
-        yield ACICacheControllerABC._notifyOfChunkKeysUpdated(self, chunkKeys)
+    def notifyFastIndexOfChunkKeysUpdated(self, chunkKeys: List[Any]):
         yield self._fastKeywordController.notifyOfUpdate(chunkKeys)
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/controller/SearchObjectCacheController.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/controller/SearchObjectCacheController.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     """
 
     _ChunkedTuple = EncodedSearchObjectChunk
     _UpdateDateTupleABC = SearchObjectUpdateDateTuple
     _chunkLoadRpcMethod = ClientChunkLoadRpc.loadSearchObjectChunks
     _chunkIndexDeltaRpcMethod = ClientChunkLoadRpc.loadSearchObjectDelta
-    _updateFromServerFilt = clientSearchObjectUpdateFromServerFilt
+    _updateFromLogicFilt = clientSearchObjectUpdateFromServerFilt
     _logger = logger
 
     @deferToThreadWrapWithLogger(logger)
     def getObjects(
         self, objectTypeId: Optional[int], objectIds: List[int]
     ) -> List[SearchResultObjectTuple]:
         return self.getObjectsBlocking(objectTypeId, objectIds)
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/handlers/SearchIndexCacheHandler.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/handlers/SearchObjectCacheHandler.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from peek_abstract_chunked_index.private.client.handlers.ACICacheHandlerABC import (
     ACICacheHandlerABC,
 )
 from peek_abstract_chunked_index.private.tuples.ACIUpdateDateTupleABC import (
     ACIUpdateDateTupleABC,
 )
 from peek_core_search._private.PluginNames import searchFilt
-from peek_core_search._private.client.controller.SearchIndexCacheController import (
-    clientSearchIndexUpdateFromServerFilt,
+from peek_core_search._private.client.controller.SearchObjectCacheController import (
+    clientSearchObjectUpdateFromServerFilt,
 )
-from peek_core_search._private.tuples.search_index.SearchIndexUpdateDateTuple import (
-    SearchIndexUpdateDateTuple,
+from peek_core_search._private.tuples.search_object.SearchObjectUpdateDateTuple import (
+    SearchObjectUpdateDateTuple,
 )
 
 logger = logging.getLogger(__name__)
 
-clientSearchIndexWatchUpdateFromDeviceFilt = {
-    "key": "clientSearchIndexWatchUpdateFromDevice"
+clientSearchObjectWatchUpdateFromDeviceFilt = {
+    "key": "clientSearchObjectWatchUpdateFromDevice"
 }
-clientSearchIndexWatchUpdateFromDeviceFilt.update(searchFilt)
+clientSearchObjectWatchUpdateFromDeviceFilt.update(searchFilt)
 
 
 # ModelSet HANDLER
-class SearchIndexCacheHandler(ACICacheHandlerABC):
-    _UpdateDateTuple: ACIUpdateDateTupleABC = SearchIndexUpdateDateTuple
-    _updateFromDeviceFilt: Dict = clientSearchIndexWatchUpdateFromDeviceFilt
-    _updateFromLogicFilt: Dict = clientSearchIndexUpdateFromServerFilt
+class SearchObjectCacheHandler(ACICacheHandlerABC):
+    _UpdateDateTuple: ACIUpdateDateTupleABC = SearchObjectUpdateDateTuple
+    _updateFromDeviceFilt: Dict = clientSearchObjectWatchUpdateFromDeviceFilt
+    _updateFromLogicFilt: Dict = clientSearchObjectUpdateFromServerFilt
     _logger: logging.Logger = logger
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py` & `peek-core-search-3.4.0/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/LogicEntryHook.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/TupleActionProcessor.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/TupleDataObservable.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/TupleDataObservable.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,27 @@
 )
 from peek_core_search._private.server.tuple_providers.SearchObjectTypeTupleProvider import (
     SearchObjectTypeTupleProvider,
 )
 from peek_core_search._private.storage.SearchObjectTypeTuple import (
     SearchObjectTypeTuple,
 )
-from peek_core_search._private.storage.SearchPropertyTuple import SearchPropertyTuple
+from peek_core_search._private.storage.SearchPropertyTuple import (
+    SearchPropertyTuple,
+)
 from peek_core_search._private.tuples.AdminStatusTuple import AdminStatusTuple
 from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
 from .controller.StatusController import StatusController
-from .tuple_providers.SearchPropertyTupleProvider import SearchPropertyTupleProvider
+from .tuple_providers.ExcludeSearchStringsTupleProvider import (
+    ExcludeSearchStringsTupleProvider,
+)
+from .tuple_providers.SearchPropertyTupleProvider import (
+    SearchPropertyTupleProvider,
+)
+from ..tuples.ExcludeSearchStringsTuple import ExcludeSearchStringsTuple
 
 
 def makeTupleDataObservableHandler(
     dbSessionCreator: DbSessionCreator, statusController: StatusController
 ):
     """ " Make Tuple Data Observable Handler
 
@@ -33,22 +41,29 @@
     """
     tupleObservable = TupleDataObservableHandler(
         observableName=searchObservableName, additionalFilt=searchFilt
     )
 
     # Search Property
     tupleObservable.addTupleProvider(
-        SearchPropertyTuple.tupleName(), SearchPropertyTupleProvider(dbSessionCreator)
+        SearchPropertyTuple.tupleName(),
+        SearchPropertyTupleProvider(dbSessionCreator),
     )
 
     # Search Object Type
     tupleObservable.addTupleProvider(
         SearchObjectTypeTuple.tupleName(),
         SearchObjectTypeTupleProvider(dbSessionCreator),
     )
 
+    # Exclude Terms Tuple
+    tupleObservable.addTupleProvider(
+        ExcludeSearchStringsTuple.tupleName(),
+        ExcludeSearchStringsTupleProvider(dbSessionCreator),
+    )
+
     # Admin status tuple
     tupleObservable.addTupleProvider(
         AdminStatusTuple.tupleName(), AdminStatusTupleProvider(statusController)
     )
 
     return tupleObservable
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/admin_backend/__init__.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/admin_backend/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
 from .EditSearchObjectTypeHandler import makeSearchObjectTypeHandler
 from .EditSearchPropertyHandler import makeSearchPropertyHandler
+from .ExcludeSearchStringTableHandler import makeExcludeSearchStringTableHandler
 from .SettingPropertyHandler import makeSettingPropertyHandler
 
 
 def makeAdminBackendHandlers(
     tupleObservable: TupleDataObservableHandler, dbSessionCreator
 ):
+    yield makeExcludeSearchStringTableHandler(tupleObservable, dbSessionCreator)
     yield makeSearchPropertyHandler(tupleObservable, dbSessionCreator)
     yield makeSearchObjectTypeHandler(tupleObservable, dbSessionCreator)
 
     yield makeSettingPropertyHandler(dbSessionCreator)
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/api/SearchApi.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/api/SearchApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,58 +41,58 @@
         yield self.loadSearchObjectDelta.start(funcSelf=self)
         logger.debug("RPCs started")
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=searchFilt,
         deferToThread=True,
     )
     def loadSearchIndexDelta(self, indexEncodedPayload: bytes) -> bytes:
         return self.ckiChunkIndexDeltaBlocking(
             indexEncodedPayload,
             EncodedSearchIndexChunk,
             SearchIndexUpdateDateTuple,
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=searchFilt,
         deferToThread=True,
     )
     def loadSearchIndexChunks(self, chunkKeys: list[str]) -> list[Tuple]:
         return self.ckiInitialLoadChunksPayloadBlocking(
             chunkKeys, EncodedSearchIndexChunk
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=searchFilt,
         deferToThread=True,
     )
     def loadSearchObjectDelta(self, indexEncodedPayload: bytes) -> bytes:
         return self.ckiChunkIndexDeltaBlocking(
             indexEncodedPayload,
             EncodedSearchObjectChunk,
             SearchObjectUpdateDateTuple,
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=searchFilt,
         deferToThread=True,
     )
     def loadSearchObjectChunks(self, chunkKeys: list[str]) -> list[Tuple]:
         return self.ckiInitialLoadChunksPayloadBlocking(
             chunkKeys, EncodedSearchObjectChunk
         )
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/controller/MainController.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,32 @@
 
 
 class _Notifier(ACIProcessorStatusNotifierABC):
     def __init__(self, adminStatusController: StatusController):
         self._adminStatusController = adminStatusController
 
     def setProcessorStatus(self, state: bool, queueSize: int):
-        self._adminStatusController.status.searchIndexCompilerQueueStatus = state
-        self._adminStatusController.status.searchIndexCompilerQueueSize = queueSize
+        self._adminStatusController.status.searchIndexCompilerQueueStatus = (
+            state
+        )
+        self._adminStatusController.status.searchIndexCompilerQueueSize = (
+            queueSize
+        )
         self._adminStatusController.notify()
 
     def addToProcessorTotal(self, delta: int):
         self._adminStatusController.status.searchIndexCompilerQueueProcessedTotal += (
             delta
         )
         self._adminStatusController.notify()
 
     def setProcessorError(self, error: str):
-        self._adminStatusController.status.searchIndexCompilerQueueLastError = error
+        self._adminStatusController.status.searchIndexCompilerQueueLastError = (
+            error
+        )
         self._adminStatusController.notify()
 
 
 class SearchIndexChunkCompilerQueueController(ACIProcessorQueueControllerABC):
     QUEUE_ITEMS_PER_TASK = 10
     POLL_PERIOD_SECONDS = 1.000
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/controller/SearchObjectImportController.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/controller/SearchObjectImportController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py` & `peek-core-search-3.4.0/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/DeclarativeBase.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/EncodedSearchIndexChunk.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/EncodedSearchIndexChunk.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/EncodedSearchObjectChunk.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/EncodedSearchObjectChunk.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/SearchIndex.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/SearchIndex.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/SearchIndexCompilerQueue.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/SearchIndexCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObject.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObject.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObjectCompilerQueue.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObjectCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObjectRoute.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObjectRoute.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/SearchObjectTypeTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/SearchObjectTypeTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/SearchPropertyTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/SearchPropertyTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/storage/Setting.py` & `peek-core-search-3.4.0/peek_core_search/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/AdminStatusTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/AdminStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/SearchResultTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/SearchResultTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py` & `peek-core-search-3.4.0/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/worker/WorkerEntryHook.py` & `peek-core-search-3.4.0/peek_core_search/_private/worker/WorkerEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py` & `peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,32 +10,41 @@
 from peek_core_search._private.storage.SearchIndexCompilerQueue import (
     SearchIndexCompilerQueue,
 )
 from peek_core_search._private.worker.tasks.KeywordSplitter import (
     splitFullKeywords,
     splitPartialKeywords,
 )
-from peek_core_search._private.worker.tasks._CalcChunkKey import makeSearchIndexChunkKey
+from peek_core_search._private.worker.tasks._CalcChunkKey import (
+    makeSearchIndexChunkKey,
+)
 from peek_plugin_base.worker import CeleryDbConn
 
 logger = logging.getLogger(__name__)
 
 ObjectToIndexTuple = namedtuple(
     "ObjectToIndexTuple", ["id", "fullKwProps", "partialKwProps"]
 )
 
 
 def removeObjectIdsFromSearchIndex(deletedObjectIds: List[int]) -> None:
     pass
 
 
-def reindexSearchObject(conn, objectsToIndex: List[ObjectToIndexTuple]) -> None:
+def reindexSearchObject(
+    conn,
+    objectsToIndex: List[ObjectToIndexTuple],
+    excludedPartialSearchTerms: list[str],
+    excludedFullSearchTerms: set[str],
+) -> None:
     """Reindex Search Object
 
-    :param conn:
+    :param excludedFullSearchTerms:
+    :param excludedPartialSearchTerms: A list of strings to exclude from tokenizing
+    :param conn: The database connection
     :param objectsToIndex: Object To Index
     :returns:
     """
 
     logger.debug("Starting to index %s SearchIndex", len(objectsToIndex))
 
     searchIndexTable = SearchIndex.__table__
@@ -44,18 +53,26 @@
     startTime = datetime.now(pytz.utc)
 
     newSearchIndexes = []
     objectIds = []
     searchIndexChunksToQueue = set()
 
     for objectToIndex in objectsToIndex:
-        newSearchIndexes.extend(_indexObject(objectToIndex))
+        newSearchIndexes.extend(
+            _indexObject(
+                objectToIndex,
+                excludedPartialSearchTerms,
+                excludedFullSearchTerms,
+            )
+        )
         objectIds.append(objectToIndex.id)
 
-    newIdGen = CeleryDbConn.prefetchDeclarativeIds(SearchIndex, len(newSearchIndexes))
+    newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+        SearchIndex, len(newSearchIndexes)
+    )
     for newSearchIndex in newSearchIndexes:
         newSearchIndex.id = next(newIdGen)
         searchIndexChunksToQueue.add(newSearchIndex.chunkKey)
 
     results = conn.execute(
         select(
             columns=[searchIndexTable.c.chunkKey],
@@ -74,15 +91,16 @@
     if newSearchIndexes:
         logger.debug("Inserting %s SearchIndex", len(newSearchIndexes))
         inserts = [o.tupleToSqlaBulkInsertDict() for o in newSearchIndexes]
         conn.execute(searchIndexTable.insert(), inserts)
 
     if searchIndexChunksToQueue:
         conn.execute(
-            queueTable.insert(), [dict(chunkKey=k) for k in searchIndexChunksToQueue]
+            queueTable.insert(),
+            [dict(chunkKey=k) for k in searchIndexChunksToQueue],
         )
 
     logger.info(
         "Inserted %s SearchIndex keywords in %s",
         len(newSearchIndexes),
         (datetime.now(pytz.utc) - startTime),
     )
@@ -97,41 +115,45 @@
 
 
 # from nltk.stem import WordNetLemmatizer
 #
 # lemmatizer = WordNetLemmatizer()
 
 
-def _indexObject(objectToIndex: ObjectToIndexTuple) -> List[SearchIndex]:
+def _indexObject(
+    objectToIndex: ObjectToIndexTuple,
+    excludedPartialSearchTerms: list[str],
+    excludedFullSearchTerms: set[str],
+) -> List[SearchIndex]:
     """Index Object
 
     This method creates  the "SearchIndex" objects to insert into the DB.
 
     Because our data is not news articles, we can skip some of the advanced
     natural language processing (NLP)
 
     We're going to be indexing things like unique IDs, job titles, and equipment names.
     We may add exclusions for nuisance words later on.
 
     """
     searchIndexes = []
 
     for propKey, text in objectToIndex.fullKwProps.items():
-        for token in splitFullKeywords(text):
+        for token in splitFullKeywords(excludedFullSearchTerms, text):
             searchIndexes.append(
                 SearchIndex(
                     chunkKey=makeSearchIndexChunkKey(token),
                     keyword=token,
                     propertyName=propKey,
                     objectId=objectToIndex.id,
                 )
             )
 
     for propKey, text in objectToIndex.partialKwProps.items():
-        for token in splitPartialKeywords(text):
+        for token in splitPartialKeywords(excludedPartialSearchTerms, text):
             searchIndexes.append(
                 SearchIndex(
                     chunkKey=makeSearchIndexChunkKey(token),
                     keyword=token,
                     propertyName=propKey,
                     objectId=objectToIndex.id,
                 )
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py` & `peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 import json
 import logging
 from collections import defaultdict
 from datetime import datetime
 from typing import List, Dict, Tuple, Set
 
 import pytz
+
+from peek_core_search._private.storage.ExcludeSearchStringTable import (
+    ExcludeSearchStringTable,
+)
 from peek_core_search._private.storage.SearchObject import SearchObject
 from peek_core_search._private.storage.SearchObjectCompilerQueue import (
     SearchObjectCompilerQueue,
 )
-from peek_core_search._private.storage.SearchObjectRoute import SearchObjectRoute
+from peek_core_search._private.storage.SearchObjectRoute import (
+    SearchObjectRoute,
+)
 from peek_core_search._private.storage.SearchObjectTypeTuple import (
     SearchObjectTypeTuple,
 )
-from peek_core_search._private.storage.SearchPropertyTuple import SearchPropertyTuple
+from peek_core_search._private.storage.SearchPropertyTuple import (
+    SearchPropertyTuple,
+)
 from peek_core_search._private.worker.tasks.ImportSearchIndexTask import (
     ObjectToIndexTuple,
     reindexSearchObject,
 )
 from peek_core_search._private.worker.tasks._CalcChunkKey import (
     makeSearchObjectChunkKey,
 )
-from peek_core_search.tuples.ImportSearchObjectTuple import ImportSearchObjectTuple
+from peek_core_search.tuples.ImportSearchObjectTuple import (
+    ImportSearchObjectTuple,
+)
 from peek_plugin_base.worker import CeleryDbConn
 from peek_plugin_base.worker.CeleryApp import celeryApp
 from sqlalchemy import select, bindparam, and_, or_
 from txcelery.defer import DeferrableTask
 from vortex.Payload import Payload
 
 logger = logging.getLogger(__name__)
@@ -61,15 +71,17 @@
 
         o.objectType = o.objectType.lower()
 
         if o.fullKeywords:
             o.fullKeywords = {k.lower(): v for k, v in o.fullKeywords.items()}
 
         if o.partialKeywords:
-            o.partialKeywords = {k.lower(): v for k, v in o.partialKeywords.items()}
+            o.partialKeywords = {
+                k.lower(): v for k, v in o.partialKeywords.items()
+            }
 
     try:
         objectTypeIdsByName = _prepareLookups(newSearchObjects)
 
         objectIdByKey, chunkKeysForQueue = _insertOrUpdateObjects(
             newSearchObjects, objectTypeIdsByName
         )
@@ -85,27 +97,28 @@
         )
 
     except Exception as e:
         logger.debug("Retrying import search objects, %s", e)
         raise self.retry(exc=e, countdown=3)
 
 
-def _prepareLookups(newSearchObjects: List[ImportSearchObjectTuple]) -> Dict[str, int]:
+def _prepareLookups(
+    newSearchObjects: List[ImportSearchObjectTuple],
+) -> Dict[str, int]:
     """Check Or Insert Search Properties
 
     Make sure the search properties exist.
 
     """
 
     dbSession = CeleryDbConn.getDbSession()
 
     startTime = datetime.now(pytz.utc)
 
     try:
-
         objectTypeNames = {"none"}
         propertyNames = {"key"}
 
         for o in newSearchObjects:
             objectTypeNames.add(o.objectType)
 
             if o.fullKeywords:
@@ -116,15 +129,17 @@
 
         # Prepare Properties
         dbProps = dbSession.query(SearchPropertyTuple).all()
         propertyNames -= set([o.name for o in dbProps])
 
         if propertyNames:
             for newPropName in propertyNames:
-                dbSession.add(SearchPropertyTuple(name=newPropName, title=newPropName))
+                dbSession.add(
+                    SearchPropertyTuple(name=newPropName, title=newPropName)
+                )
 
             dbSession.commit()
 
         del dbProps
         del propertyNames
 
         # Prepare Object Types
@@ -141,28 +156,31 @@
                 )
 
             dbSession.commit()
 
             dbObjectTypes = dbSession.query(SearchObjectTypeTuple).all()
             objectTypeIdsByName = {o.name: o.id for o in dbObjectTypes}
 
-        logger.debug("Prepared lookups in %s", (datetime.now(pytz.utc) - startTime))
+        logger.debug(
+            "Prepared lookups in %s", (datetime.now(pytz.utc) - startTime)
+        )
 
         return objectTypeIdsByName
 
     except Exception as e:
         dbSession.rollback()
         raise
 
     finally:
         dbSession.close()
 
 
 def _insertOrUpdateObjects(
-    newSearchObjects: List[ImportSearchObjectTuple], objectTypeIdsByName: Dict[str, int]
+    newSearchObjects: List[ImportSearchObjectTuple],
+    objectTypeIdsByName: Dict[str, int],
 ) -> Tuple[Dict[str, int], Set[int]]:
     """Insert or Update Objects
 
     1) Find objects and update them
     2) Insert object if the are missing
 
     """
@@ -175,22 +193,26 @@
         newSearchObjects, searchObjectTable
     )
 
     conn = engine.connect()
     transaction = conn.begin()
 
     try:
-
         # Create state arrays
         objectsToIndex: Dict[int, ObjectToIndexTuple] = {}
         objectIdByKey: Dict[str, int] = {}
         inserts = []
         propUpdates = []
         objectTypeUpdates = []
-        chunkKeysForQueue: Set[int] = set()
+        chunkKeysForQueue: set[int] = set()
+
+        (
+            excludedFullSearchTerms,
+            excludedPartialSearchTerms,
+        ) = queryExcludedTerms(conn)
 
         # Work out which objects have been updated or need inserting
         for importObject in newSearchObjects:
             originalImportObjectKey = importObject.key
             importObject.key = importObject.key.lower()
             loweredObjectKey = importObject.key
 
@@ -205,15 +227,17 @@
                     fullKwPropsWithKey.update(
                         json.loads(existingObject.fullKwPropertiesJson)
                     )
 
                 # Add the data we're importing second
                 # Remove null values
                 fullKwPropsWithKey.update(importObject.fullKeywords)
-                fullKwPropsWithKey = {k: v for k, v in fullKwPropsWithKey.items() if v}
+                fullKwPropsWithKey = {
+                    k: v for k, v in fullKwPropsWithKey.items() if v
+                }
 
             if importObject.partialKeywords:
                 if existingObject and existingObject.partialKwPropertiesJson:
                     partialKwProps.update(
                         json.loads(existingObject.partialKwPropertiesJson)
                     )
 
@@ -239,15 +263,16 @@
                     fullKwPropsStr
                     and existingObject.fullKwPropertiesJson != fullKwPropsStr
                 )
 
                 searchIndexUpdateNeeded = (
                     searchIndexUpdateNeeded
                     or partialKwPropsStr
-                    and existingObject.partialKwPropertiesJson != partialKwPropsStr
+                    and existingObject.partialKwPropertiesJson
+                    != partialKwPropsStr
                 )
 
                 if searchIndexUpdateNeeded:
                     propUpdates.append(
                         dict(
                             b_id=existingObject.id,
                             b_fullPropsKwStr=fullKwPropsStr,
@@ -302,15 +327,20 @@
                 searchObjectTable.update()
                 .where(searchObjectTable.c.id == bindparam("b_id"))
                 .values(objectTypeId=bindparam("b_typeId"))
             )
             conn.execute(stmt, objectTypeUpdates)
 
         # Reindex the keywords
-        reindexSearchObject(conn, list(objectsToIndex.values()))
+        reindexSearchObject(
+            conn,
+            list(objectsToIndex.values()),
+            excludedPartialSearchTerms,
+            excludedFullSearchTerms,
+        )
 
         if objectsToIndex or inserts or propUpdates or objectTypeUpdates:
             transaction.commit()
         else:
             transaction.rollback()
 
         logger.debug(
@@ -328,14 +358,40 @@
         transaction.rollback()
         raise
 
     finally:
         conn.close()
 
 
+def queryExcludedTerms(conn):
+    excludeSearchStringTable = ExcludeSearchStringTable.__table__
+
+    sql = select(
+        columns=[
+            excludeSearchStringTable.c.term,
+            excludeSearchStringTable.c.partial,
+            excludeSearchStringTable.c.full,
+        ]
+    )
+
+    excludedPartialSearchTerms = []
+    excludedFullSearchTerms = []
+
+    for result in conn.execute(sql):
+        if result.partial:
+            excludedPartialSearchTerms.append(result.term.lower())
+        if result.full:
+            excludedFullSearchTerms.append(result.term.lower())
+
+    excludedPartialSearchTerms.sort(key=lambda t: -len(t))
+    excludedFullSearchTerms = set(excludedFullSearchTerms)
+
+    return excludedFullSearchTerms, excludedPartialSearchTerms
+
+
 def _loadExistingObjects(newSearchObjects, searchObjectTable):
     engine = CeleryDbConn.getDbEngine()
     conn = engine.connect()
     try:
         objectKeys = set(
             [o.key for o in newSearchObjects]
             + [o.key.lower() for o in newSearchObjects]
@@ -360,24 +416,27 @@
         createdObjectByKey = {o.key.lower(): o for o in results}
         del results
         del objectKeys
 
     finally:
         conn.close()
     # Get the IDs that we need
-    newSearchObjectUniqueCount = len(set([o.key.lower() for o in newSearchObjects]))
+    newSearchObjectUniqueCount = len(
+        set([o.key.lower() for o in newSearchObjects])
+    )
     newIdGen = CeleryDbConn.prefetchDeclarativeIds(
         SearchObject, newSearchObjectUniqueCount - len(createdObjectByKey)
     )
     del newSearchObjectUniqueCount
     return createdObjectByKey, engine, newIdGen
 
 
 def _insertObjectRoutes(
-    newSearchObjects: List[ImportSearchObjectTuple], objectIdByKey: Dict[str, int]
+    newSearchObjects: List[ImportSearchObjectTuple],
+    objectIdByKey: Dict[str, int],
 ):
     """Insert Object Routes
 
     1) Drop all routes with matching importGroupHash
 
     2) Insert the new routes
 
@@ -439,15 +498,16 @@
                     routePath=impRoute.routePath,
                 )
 
                 uniqueRouteStr = "%s.%s" % (objectId, impRoute.routeTitle)
 
                 if uniqueRouteStr in existingRoutes:
                     logger.debug(
-                        "A duplicate route exists in another" " import group\n%s\n%s",
+                        "A duplicate route exists in another"
+                        " import group\n%s\n%s",
                         existingRoutes[uniqueRouteStr],
                         routeInsert,
                     )
 
                 elif uniqueRouteStr in newRoutes:
                     logger.debug(
                         "Duplicate route titles defined in this"
@@ -505,25 +565,26 @@
     searchObjectTable = SearchObject.__table__
     objectQueueTable = SearchObjectCompilerQueue.__table__
     dbSession = CeleryDbConn.getDbSession()
 
     startTime = datetime.now(pytz.utc)
 
     try:
-
         indexQry = (
             dbSession.query(
                 SearchObject.id,
                 SearchObject.fullKwPropertiesJson,
                 SearchObject.partialKwPropertiesJson,
                 SearchObject.objectTypeId,
                 SearchObjectRoute.routeTitle,
                 SearchObjectRoute.routePath,
             )
-            .outerjoin(SearchObjectRoute, SearchObject.id == SearchObjectRoute.objectId)
+            .outerjoin(
+                SearchObjectRoute, SearchObject.id == SearchObjectRoute.objectId
+            )
             .filter(SearchObject.id.in_(updatedIds))
             .filter(
                 or_(
                     SearchObject.fullKwPropertiesJson != None,
                     SearchObject.partialKwPropertiesJson != None,
                 )
             )
@@ -569,15 +630,16 @@
                 .where(searchObjectTable.c.id == bindparam("b_id"))
                 .values(packedJson=bindparam("b_packedJson"))
             )
             dbSession.execute(stmt, packedJsonUpdates)
 
         if chunkKeysForQueue:
             dbSession.execute(
-                objectQueueTable.insert(), [dict(chunkKey=v) for v in chunkKeysForQueue]
+                objectQueueTable.insert(),
+                [dict(chunkKey=v) for v in chunkKeysForQueue],
             )
 
         if packedJsonUpdates or chunkKeysForQueue:
             dbSession.commit()
         else:
             dbSession.rollback()
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/KeywordSplitter.py` & `peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/KeywordSplitter.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,44 +9,78 @@
     # Remove punctuation
     tokens = keywordStr.lower().split(" ")
 
     # Strip and Split words, filter out words less than three letters
     return set([w.strip() for w in tokens if 2 <= len(w)])
 
 
-def splitFullKeywords(keywordStr: str) -> Set[str]:
+def filterExcludedFullTerms(excludeStrings: set[str], keywordStr: str):
+    return " ".join(
+        filter(lambda t: t not in excludeStrings, _splitFullTokens(keywordStr))
+    )
+
+
+def splitFullKeywords(excludeStrings: set[str], keywordStr: str) -> Set[str]:
     """Split Full Keywords
 
     This tokenizer function is used for search strings loaded into
     the fullKwPropertiesJson field of the SearchObject.
 
     This exists, because not all data is suitable for partial keywork search
     for example IDs like J00001223COMP
 
     """
     tokens = _splitFullTokens(keywordStr)
-    tokens = ["^%s$" % t for t in tokens]
+    tokens = ["^%s$" % t for t in tokens if t not in excludeStrings]
 
     return set(tokens)
 
 
-def splitPartialKeywords(keywordStr: str) -> Set[str]:
+def filterExcludedPartialTerms(excludeStrings, keywordStr):
+    keywordStr = keywordStr.lower()
+    for excludeString in excludeStrings:
+        keywordStr = keywordStr.replace(excludeString, "")
+    return keywordStr
+
+
+def prepareExcludedPartialTermsForFind(excludeStrings: list[str]) -> list[str]:
+    # Add terms so we have `conn` and `con`
+
+    uniqueExcludes = set()
+
+    for term in excludeStrings:
+        uniqueExcludes.add(term)
+        while 3 < len(term):
+            term = term[:-1]
+            uniqueExcludes.add(term)
+
+    # Sort terms so we replace larger matches first
+    return list(sorted(uniqueExcludes, key=lambda s: -len(s)))
+
+
+def splitPartialKeywords(
+    excludeStrings: list[str], keywordStr: str
+) -> Set[str]:
     """Split Partial Keywords
 
     This tokenizer function is used for search strings loaded into the
     partialKwPropertiesJson field of the SearchObject.
 
     This will tokenize
     * all the smaller keywords as a full keyword,
     * all numbers as full keywords
     * all remaining items will be tokenized in a rolling three char method.
 
+    :param excludeStrings: An array of lowercase strings that are not worth
+        tokenizing
     :param keywordStr: The string to tokenize
 
     """
+    keywordStr = filterExcludedPartialTerms(excludeStrings, keywordStr)
+
     # Strip and Split words, filter out words less than three letters
     tokens = _splitFullTokens(keywordStr)
 
     # Split the words up into tokens, this creates partial keyword search support
     tempTokens, tokens = tokens, []
     for token in tempTokens:
         # Partial tokenize the other words.
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py` & `peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 2) Process queue
 3) Delete from queue
 """
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileSearchIndexChunk(self, payloadEncodedArgs: bytes) -> List[str]:
+def compileSearchIndexChunk(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile Search Index Task
 
     :param self: A celery reference to this task
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
@@ -69,27 +69,34 @@
         # Get Model Sets
 
         total = 0
         existingHashes = _loadExistingHashes(conn, chunkKeys)
         encKwPayloadByChunkKey = _buildIndex(conn, chunkKeys)
         chunksToDelete = []
 
+        lastUpdateByChunkKey = {}
+
         inserts = []
-        for chunkKey, searchIndexChunkEncodedPayload in encKwPayloadByChunkKey.items():
+        for (
+            chunkKey,
+            searchIndexChunkEncodedPayload,
+        ) in encKwPayloadByChunkKey.items():
             m = hashlib.sha256()
             m.update(searchIndexChunkEncodedPayload)
             encodedHash = b64encode(m.digest()).decode()
 
             # Compare the hash, AND delete the chunk key
             if chunkKey in existingHashes:
                 # At this point we could decide to do an update instead,
                 # but inserts are quicker
                 if encodedHash == existingHashes.pop(chunkKey):
                     continue
 
+            lastUpdateByChunkKey[str(chunkKey)] = lastUpdate
+
             chunksToDelete.append(chunkKey)
             inserts.append(
                 dict(
                     chunkKey=chunkKey,
                     encodedData=searchIndexChunkEncodedPayload,
                     encodedHash=encodedHash,
                     lastUpdate=lastUpdate,
@@ -98,19 +105,23 @@
 
         # Add any chnuks that we need to delete that we don't have new data for, here
         chunksToDelete.extend(list(existingHashes))
 
         if chunksToDelete:
             # Delete the old chunks
             conn.execute(
-                compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete))
+                compiledTable.delete(
+                    compiledTable.c.chunkKey.in_(chunksToDelete)
+                )
             )
 
         if inserts:
-            newIdGen = CeleryDbConn.prefetchDeclarativeIds(SearchIndex, len(inserts))
+            newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+                SearchIndex, len(inserts)
+            )
             for insert in inserts:
                 insert["id"] = next(newIdGen)
 
         transaction.commit()
         transaction = conn.begin()
 
         if inserts:
@@ -130,15 +141,15 @@
         transaction.commit()
         logger.info(
             "Compiled and Committed %s EncodedSearchIndexChunks in %s",
             total,
             (datetime.now(pytz.utc) - startTime),
         )
 
-        return chunkKeys
+        return lastUpdateByChunkKey
 
     except Exception as e:
         transaction.rollback()
         # logger.warning(e)  # Just a warning, it will retry
         logger.exception(e)
         raise self.retry(exc=e, countdown=10)
 
@@ -216,12 +227,12 @@
                     [keyword, propertyName, json.dumps(list(sorted(objectIds)))]
                 )
 
         compileSearchIndexChunks.sort(key=cmp_to_key(_sortSearchIndex))
 
         # Create the blob data for this index.
         # It will be searched by a binary sort
-        encKwPayloadByChunkKey[chunkKey] = Payload(
-            tuples=compileSearchIndexChunks
-        ).toEncodedPayload()
+        encKwPayloadByChunkKey[chunkKey] = (
+            Payload(tuples=compileSearchIndexChunks).toEncodedPayload().encode()
+        )
 
     return encKwPayloadByChunkKey
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py` & `peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 2) Process queue
 3) Delete from queue
 """
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileSearchObjectChunk(self, payloadEncodedArgs: bytes) -> List[str]:
+def compileSearchObjectChunk(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile Search Index Task
 
     :param self: A celery reference to this task
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
@@ -68,27 +68,34 @@
         # Get Model Sets
 
         total = 0
         existingHashes = _loadExistingHashes(conn, chunkKeys)
         encKwPayloadByChunkKey = _buildIndex(chunkKeys)
         chunksToDelete = []
 
+        lastUpdateByChunkKey = {}
+
         inserts = []
-        for chunkKey, searchIndexChunkEncodedPayload in encKwPayloadByChunkKey.items():
+        for (
+            chunkKey,
+            searchIndexChunkEncodedPayload,
+        ) in encKwPayloadByChunkKey.items():
             m = hashlib.sha256()
             m.update(searchIndexChunkEncodedPayload)
             encodedHash = b64encode(m.digest()).decode()
 
             # Compare the hash, AND delete the chunk key
             if chunkKey in existingHashes:
                 # At this point we could decide to do an update instead,
                 # but inserts are quicker
                 if encodedHash == existingHashes.pop(chunkKey):
                     continue
 
+            lastUpdateByChunkKey[str(chunkKey)] = lastUpdate
+
             chunksToDelete.append(chunkKey)
             inserts.append(
                 dict(
                     chunkKey=chunkKey,
                     encodedData=searchIndexChunkEncodedPayload,
                     encodedHash=encodedHash,
                     lastUpdate=lastUpdate,
@@ -97,19 +104,23 @@
 
         # Add any chnuks that we need to delete that we don't have new data for, here
         chunksToDelete.extend(list(existingHashes))
 
         if chunksToDelete:
             # Delete the old chunks
             conn.execute(
-                compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete))
+                compiledTable.delete(
+                    compiledTable.c.chunkKey.in_(chunksToDelete)
+                )
             )
 
         if inserts:
-            newIdGen = CeleryDbConn.prefetchDeclarativeIds(SearchObject, len(inserts))
+            newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+                SearchObject, len(inserts)
+            )
             for insert in inserts:
                 insert["id"] = next(newIdGen)
 
         transaction.commit()
         transaction = conn.begin()
 
         if inserts:
@@ -129,15 +140,15 @@
         transaction.commit()
         logger.info(
             "Compiled and Committed %s EncodedSearchObjectChunks in %s",
             total,
             (datetime.now(pytz.utc) - startTime),
         )
 
-        return chunkKeys
+        return lastUpdateByChunkKey
 
     except Exception as e:
         transaction.rollback()
         # logger.warning(e)  # Just a warning, it will retry
         logger.exception(e)
         raise self.retry(exc=e, countdown=10)
 
@@ -173,23 +184,27 @@
             .all()
         )
 
         # Create the ChunkKey -> {id -> packedJson, id -> packedJson, ....]
         packagedJsonByObjIdByChunkKey = defaultdict(dict)
 
         for item in indexQry:
-            packagedJsonByObjIdByChunkKey[item.chunkKey][item.id] = item.packedJson
+            packagedJsonByObjIdByChunkKey[item.chunkKey][
+                item.id
+            ] = item.packedJson
 
         encPayloadByChunkKey = {}
 
         # Sort each bucket by the key
         for chunkKey, packedJsonById in packagedJsonByObjIdByChunkKey.items():
             tuples = json.dumps(packedJsonById, sort_keys=True)
 
             # Create the blob data for this index.
             # It will be searched by a binary sort
-            encPayloadByChunkKey[chunkKey] = Payload(tuples=tuples).toEncodedPayload()
+            encPayloadByChunkKey[chunkKey] = (
+                Payload(tuples=tuples).toEncodedPayload().encode()
+            )
 
         return encPayloadByChunkKey
 
     finally:
         session.close()
```

### Comparing `peek-core-search-3.3.3/peek_core_search/_private/worker/tasks/_CalcChunkKey.py` & `peek-core-search-3.4.0/peek_core_search/_private/worker/tasks/_CalcChunkKey.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png` & `peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png` & `peek-core-search-3.4.0/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/admin-doc/index.rst` & `peek-core-search-3.4.0/peek_core_search/admin-doc/index.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/admin-doc/overview.rst` & `peek-core-search-3.4.0/peek_core_search/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/admin-doc/status/status.png` & `peek-core-search-3.4.0/peek_core_search/admin-doc/status/status.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/admin-doc/status/status.rst` & `peek-core-search-3.4.0/peek_core_search/admin-doc/status/status.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/both-doc/search_button.png` & `peek-core-search-3.4.0/peek_core_search/both-doc/search_button.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/both-doc/search_filtered.png` & `peek-core-search-3.4.0/peek_core_search/both-doc/search_filtered.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/both-doc/search_popup.png` & `peek-core-search-3.4.0/peek_core_search/both-doc/search_popup.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/both-doc/searching.rst` & `peek-core-search-3.4.0/peek_core_search/both-doc/searching.rst`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 Overview
 --------
 
 This screen is used to search the Peek database.
 
 Searches can be performed with the following criteria :
 
-- Whole keywords (partial is on the roadmap)
-- An object type, or all object types
+- Whole or Parial Keywords
+- An object type, or all object types.
 - The property name that contains the keyword, or all property names.
 
 Peeks Search functionality can be used to find:
 
 - Jobs
 - Operations
 - Incidents
```

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/SearchObjectTypeTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/SearchObjectTypeTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/SearchResultObjectTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/SearchResultObjectTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/SearchService.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/SearchService.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import { filter, first, takeUntil } from "rxjs/operators";
+import { filter, first, map, takeUntil } from "rxjs/operators";
 import { Injectable } from "@angular/core";
 import {
     NgLifeCycleEvents,
     TupleSelector,
     VortexStatusService,
 } from "@synerty/vortexjs";
 import { PrivateSearchIndexLoaderService } from "./_private/search-index-loader";
 import { PrivateSearchObjectLoaderService } from "./_private/search-object-loader";
 import { SearchResultObjectTuple } from "./SearchResultObjectTuple";
 import { SearchObjectTypeTuple } from "./SearchObjectTypeTuple";
 import { SearchPropertyTuple, SearchTupleService } from "./_private";
 import { KeywordAutoCompleteTupleAction } from "./_private/tuples/KeywordAutoCompleteTupleAction";
 import { DeviceOfflineCacheService } from "@peek/peek_core_device";
 import { FastKeywordController } from "./_private/fast-keyword-controller";
+import { Observable, zip } from "rxjs";
 
 export interface SearchPropT {
     title: string;
     value: string;
     order: number;
 
     // Should this property be shown as the name in the search result
@@ -54,29 +55,60 @@
         private searchIndexLoader: PrivateSearchIndexLoaderService,
         private searchObjectLoader: PrivateSearchObjectLoaderService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
         this.fastIndexController = new FastKeywordController(
             searchIndexLoader,
-            searchObjectLoader
+            searchObjectLoader,
+            tupleService,
+            this
         );
         this._loadPropsAndObjs();
     }
 
+    get canSearchOffline$(): Observable<boolean> {
+        return zip(
+            this.searchIndexLoader.isReadyObservable(),
+            this.searchObjectLoader.isReadyObservable()
+        )
+            .pipe(
+                filter(
+                    () =>
+                        this.searchObjectLoader.offlineEnabled &&
+                        this.searchIndexLoader.offlineEnabled
+                )
+            )
+            .pipe(map((values) => true));
+    }
+
+    haveEnoughSearchKeywords(keywordsString: string): boolean {
+        return this.fastIndexController.haveEnoughSearchKeywords(
+            keywordsString
+        );
+    }
+
     /** Get Locations
      *
      * Get the objects with matching keywords from the index..
      *
      */
     async getObjects(
         propertyName: string | null,
         objectTypeId: number | null,
         keywordsString: string
     ): Promise<SearchResultObjectTuple[]> {
+        if (!this.haveEnoughSearchKeywords(keywordsString)) {
+            console.log(
+                `Skipping search for '${keywordsString}'` +
+                    ` as it's too short after excluding keywords`
+            );
+            return [];
+        }
+
         // If we're online
         if (this.vortexStatusService.snapshot.isOnline) {
             return this.getObjectsOnline(
                 propertyName,
                 objectTypeId,
                 keywordsString
             );
```

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/PluginNames.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/PluginNames.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/SearchTupleService.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/SearchTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,18 @@
     searchIndexCacheStorageName,
     searchTuplePrefix,
 } from "../PluginNames";
 
 import { EncodedSearchIndexChunkTuple } from "./EncodedSearchIndexChunkTuple";
 import { SearchIndexUpdateDateTuple } from "./SearchIndexUpdateDateTuple";
 import { SearchTupleService } from "../SearchTupleService";
-import { PrivateSearchIndexLoaderStatusTuple } from "./PrivateSearchIndexLoaderStatusTuple";
 
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 
 // ----------------------------------------------------------------------------
 
 let clientSearchIndexWatchUpdateFromDeviceFilt = extend(
     { key: "clientSearchIndexWatchUpdateFromDevice" },
     searchFilt
@@ -115,64 +114,82 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new SearchIndexUpdateDateTuple();
+    private index: SearchIndexUpdateDateTuple | null = null;
     private askServerChunks: SearchIndexUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
 
     private _hasLoadedSubject = new Subject<void>();
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject = new Subject<PrivateSearchIndexLoaderStatusTuple>();
-    private _status = new PrivateSearchIndexLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         private tupleService: SearchTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
 
+        this._status.pluginName = "peek_core_search";
+        this._status.indexName = "Keyword Index";
+
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(searchIndexCacheStorageName)
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
 
-    statusObservable(): Observable<PrivateSearchIndexLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): PrivateSearchIndexLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     get offlineEnabled(): boolean {
         return this.index.initialLoadComplete;
     }
 
@@ -190,81 +207,71 @@
 
         return this.isReadyObservable()
             .pipe(first())
             .toPromise()
             .then(() => this._getObjectIdsForTokens(tokens, propertyName));
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
+    private _notifyReady(): void {
+        if (this._hasLoaded) this._hasLoadedSubject.next();
+    }
+
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
-        status.pluginName = "peek_core_search";
-        status.indexName = "Keyword Index";
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
                 let tuples: SearchIndexUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new SearchIndexUpdateDateTuple();
+                } else {
                     this.index = tuples[0];
 
                     if (this.index.initialLoadComplete) {
                         this._hasLoaded = true;
-                        this._hasLoadedSubject.next();
+                        this._notifyReady();
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
                 clientSearchIndexWatchUpdateFromDeviceFilt
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
@@ -288,15 +295,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: SearchIndexUpdateDateTuple = tuplesAny[0];
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
@@ -337,39 +344,38 @@
             }
         }
 
         if (count) this.askServerChunks.push(indexChunk);
 
         this.askServerForNextUpdateChunk();
 
-        this._status.lastCheck = new Date();
+        this._status.lastCheckDate = new Date();
         this._notifyStatus();
     }
 
     private askServerForNextUpdateChunk() {
         if (!this.areWeTalkingToTheServer()) return;
 
         if (this.askServerChunks.length == 0) return;
 
-        this.deviceCacheControllerService //
-            .waitForGarbageCollector()
-            .then(() => {
-                let indexChunk: SearchIndexUpdateDateTuple =
-                    this.askServerChunks.pop();
-                let filt = extend(
-                    {},
-                    clientSearchIndexWatchUpdateFromDeviceFilt
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
+        let indexChunk: SearchIndexUpdateDateTuple = this.askServerChunks.pop();
+        let filt = extend({}, clientSearchIndexWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let pl = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(pl);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process SearchIndexes From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(
```

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     searchTuplePrefix,
 } from "../PluginNames";
 import { EncodedSearchObjectChunkTuple } from "./EncodedSearchObjectChunkTuple";
 import { SearchObjectUpdateDateTuple } from "./SearchObjectUpdateDateTuple";
 import { SearchResultObjectTuple } from "../../SearchResultObjectTuple";
 import { SearchResultObjectRouteTuple } from "../../SearchResultObjectRouteTuple";
 import { SearchTupleService } from "../SearchTupleService";
-import { PrivateSearchObjectLoaderStatusTuple } from "./PrivateSearchObjectLoaderStatusTuple";
 import { SearchObjectTypeTuple } from "../../SearchObjectTypeTuple";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
+import { SearchIndexUpdateDateTuple } from "@peek/peek_core_search/_private";
 
 // ----------------------------------------------------------------------------
 
 let clientSearchObjectWatchUpdateFromDeviceFilt = extend(
     { key: "clientSearchObjectWatchUpdateFromDevice" },
     searchFilt
 );
@@ -107,65 +107,82 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new SearchObjectUpdateDateTuple();
+    private index: SearchObjectUpdateDateTuple | null = null;
     private askServerChunks: SearchObjectUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
 
     private _hasLoadedSubject = new Subject<void>();
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject =
-        new Subject<PrivateSearchObjectLoaderStatusTuple>();
-    private _status = new PrivateSearchObjectLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         private tupleService: SearchTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
 
+        this._status.pluginName = "peek_core_search";
+        this._status.indexName = "Object Index";
+
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(searchObjectCacheStorageName)
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
 
-    statusObservable(): Observable<PrivateSearchObjectLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): PrivateSearchObjectLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     get offlineEnabled(): boolean {
         return this.index.initialLoadComplete;
     }
 
@@ -187,81 +204,71 @@
 
         return this.isReadyObservable()
             .pipe(first())
             .toPromise()
             .then(() => this.getObjectsWhenReady(objectTypeId, objectIds));
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
+    private _notifyReady(): void {
+        if (this._hasLoaded) this._hasLoadedSubject.next();
+    }
+
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
-        status.pluginName = "peek_core_search";
-        status.indexName = "Object Index";
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
                 let tuples: SearchObjectUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new SearchObjectUpdateDateTuple();
+                } else {
                     this.index = tuples[0];
 
                     if (this.index.initialLoadComplete) {
                         this._hasLoaded = true;
-                        this._hasLoadedSubject.next();
+                        this._notifyReady();
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
                 clientSearchObjectWatchUpdateFromDeviceFilt
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
@@ -285,15 +292,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: SearchObjectUpdateDateTuple = tuplesAny[0];
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
@@ -334,38 +341,38 @@
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
-                let indexChunk: SearchObjectUpdateDateTuple =
-                    this.askServerChunks.pop();
-                let filt = extend(
-                    {},
-                    clientSearchObjectWatchUpdateFromDeviceFilt
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
+        let indexChunk: SearchObjectUpdateDateTuple =
+            this.askServerChunks.pop();
+        let filt = extend({}, clientSearchObjectWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let pl = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(pl);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process SearchObjects From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(
```

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts` & `peek-core-search-3.4.0/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/plugin_package.json` & `peek-core-search-3.4.0/peek_core_search/plugin_package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9864285714285714%*

 * *Differences: {"'field'": "{delete: ['cfgDir', 'cfgModule']}", "'plugin'": "{'version': '3.4.0'}"}*

```diff
@@ -11,16 +11,14 @@
         "hasApi": true
     },
     "agent": {},
     "field": {
         "appDir": "_private/both-app",
         "appModule": "search.module#SearchModule",
         "assetDir": "_private/both-assets",
-        "cfgDir": "_private/both-cfg",
-        "cfgModule": "search-cfg.module#SearchCfgModule",
         "icon": "/assets/peek_core_search/icon.png",
         "moduleDir": "plugin-module",
         "rootServices": [
             {
                 "class": "SearchTupleService",
                 "file": "_private/SearchTupleService"
             },
@@ -78,15 +76,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_search",
         "title": "Search",
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

### Comparing `peek-core-search-3.3.3/peek_core_search/server/SearchApiABC.py` & `peek-core-search-3.4.0/peek_core_search/server/SearchApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/tuples/ImportSearchObjectRouteTuple.py` & `peek-core-search-3.4.0/peek_core_search/tuples/ImportSearchObjectRouteTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.3.3/peek_core_search/tuples/ImportSearchObjectTuple.py` & `peek-core-search-3.4.0/peek_core_search/tuples/ImportSearchObjectTuple.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,7 +32,27 @@
     #:  Partial Keywords
     # The keywords to index that allows the user to search by partial keywords
     # The key of the property will match of create a new "SearchProperty"
     partialKeywords: Dict[str, str] = TupleField({})
 
     #:  The color
     routes: List[ImportSearchObjectRouteTuple] = TupleField([])
+
+    def __repr__(self):
+        s = ""
+        s += f"key={self.key}\n"
+        s += f"objectType={self.objectType}\n"
+
+        for key, value in sorted(self.fullKeywords.items(), key=lambda i: i[0]):
+            s += f"fullKw.{key}={value}\n"
+
+        for key, value in sorted(
+            self.partialKeywords.items(), key=lambda i: i[0]
+        ):
+            s += f"partialKw.{key}={value}\n"
+
+        for route in sorted(
+            self.routes, key=lambda i: i.routeTitle + i.routePath
+        ):
+            s += f"route.{route.routeTitle}={route.routePath}\n"
+
+        return s
```

### Comparing `peek-core-search-3.3.3/peek_core_search.egg-info/SOURCES.txt` & `peek-core-search-3.4.0/peek_core_search.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,52 +9,55 @@
 peek_core_search.egg-info/not-zip-safe
 peek_core_search.egg-info/requires.txt
 peek_core_search.egg-info/top_level.txt
 peek_core_search/_private/PluginNames.py
 peek_core_search/_private/__init__.py
 peek_core_search/_private/alembic.ini
 peek_core_search/_private/admin-app/search.module.ts
+peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.html
+peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.ts
 peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html
 peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts
 peek_core_search/_private/admin-app/edit-property-table/edit.component.html
 peek_core_search/_private/admin-app/edit-property-table/edit.component.ts
 peek_core_search/_private/admin-app/edit-setting-table/edit.component.html
 peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts
 peek_core_search/_private/admin-app/search-component/search.component.html
 peek_core_search/_private/admin-app/search-component/search.component.ts
 peek_core_search/_private/admin-app/status-component/status.component.html
 peek_core_search/_private/admin-app/status-component/status.component.ts
+peek_core_search/_private/admin-app/tuples/ExcludeSearchStringTable.ts
 peek_core_search/_private/agent/AgentEntryHook.py
 peek_core_search/_private/agent/__init__.py
 peek_core_search/_private/alembic/__init__.py
 peek_core_search/_private/alembic/env.py
 peek_core_search/_private/alembic/script.py.mako
 peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py
 peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py
 peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py
 peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py
+peek_core_search/_private/alembic/versions/3dba609610b6_fix_exclude_comment.py
 peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py
 peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py
 peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py
+peek_core_search/_private/alembic/versions/79609b0e25a5_add_full_exclude_terms.py
 peek_core_search/_private/alembic/versions/__init__.py
 peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py
+peek_core_search/_private/alembic/versions/e51cdf9b7d4c_add_exclude_terms.py
 peek_core_search/_private/both-app/search.module.ts
 peek_core_search/_private/both-app/find-component/find.component.html
 peek_core_search/_private/both-app/find-component/find.component.scss
 peek_core_search/_private/both-app/find-component/find.component.ts
 peek_core_search/_private/both-app/result-component/result.component.html
 peek_core_search/_private/both-app/result-component/result.component.scss
 peek_core_search/_private/both-app/result-component/result.component.ts
 peek_core_search/_private/both-app/search-component/search.component.html
 peek_core_search/_private/both-app/search-component/search.component.scss
 peek_core_search/_private/both-app/search-component/search.component.ts
 peek_core_search/_private/both-assets/icon.png
-peek_core_search/_private/both-cfg/search-cfg.component.html
-peek_core_search/_private/both-cfg/search-cfg.component.ts
-peek_core_search/_private/both-cfg/search-cfg.module.ts
 peek_core_search/_private/client/ClientEntryHook.py
 peek_core_search/_private/client/DeviceTupleDataObservableProxy.py
 peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py
 peek_core_search/_private/client/TupleDataObservable.py
 peek_core_search/_private/client/__init__.py
 peek_core_search/_private/client/controller/FastKeywordController.py
 peek_core_search/_private/client/controller/FastKeywordControllerTest.py
@@ -69,14 +72,15 @@
 peek_core_search/_private/client/tuple_providers/__init__.py
 peek_core_search/_private/server/LogicEntryHook.py
 peek_core_search/_private/server/TupleActionProcessor.py
 peek_core_search/_private/server/TupleDataObservable.py
 peek_core_search/_private/server/__init__.py
 peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py
 peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py
+peek_core_search/_private/server/admin_backend/ExcludeSearchStringTableHandler.py
 peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py
 peek_core_search/_private/server/admin_backend/__init__.py
 peek_core_search/_private/server/api/SearchApi.py
 peek_core_search/_private/server/api/__init__.py
 peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py
 peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py
 peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py
@@ -84,30 +88,33 @@
 peek_core_search/_private/server/controller/MainController.py
 peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py
 peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py
 peek_core_search/_private/server/controller/SearchObjectImportController.py
 peek_core_search/_private/server/controller/StatusController.py
 peek_core_search/_private/server/controller/__init__.py
 peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py
+peek_core_search/_private/server/tuple_providers/ExcludeSearchStringsTupleProvider.py
 peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py
 peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py
 peek_core_search/_private/server/tuple_providers/__init__.py
 peek_core_search/_private/storage/DeclarativeBase.py
 peek_core_search/_private/storage/EncodedSearchIndexChunk.py
 peek_core_search/_private/storage/EncodedSearchObjectChunk.py
+peek_core_search/_private/storage/ExcludeSearchStringTable.py
 peek_core_search/_private/storage/SearchIndex.py
 peek_core_search/_private/storage/SearchIndexCompilerQueue.py
 peek_core_search/_private/storage/SearchObject.py
 peek_core_search/_private/storage/SearchObjectCompilerQueue.py
 peek_core_search/_private/storage/SearchObjectRoute.py
 peek_core_search/_private/storage/SearchObjectTypeTuple.py
 peek_core_search/_private/storage/SearchPropertyTuple.py
 peek_core_search/_private/storage/Setting.py
 peek_core_search/_private/storage/__init__.py
 peek_core_search/_private/tuples/AdminStatusTuple.py
+peek_core_search/_private/tuples/ExcludeSearchStringsTuple.py
 peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py
 peek_core_search/_private/tuples/SearchResultDetailTuple.py
 peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py
 peek_core_search/_private/tuples/SearchResultTuple.py
 peek_core_search/_private/tuples/__init__.py
 peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py
 peek_core_search/_private/tuples/search_index/__init__.py
@@ -126,14 +133,17 @@
 peek_core_search/_private/worker/tasks/_CalcChunkKey.py
 peek_core_search/_private/worker/tasks/__init__.py
 peek_core_search/admin-doc/index.rst
 peek_core_search/admin-doc/overview.rst
 peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png
 peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png
 peek_core_search/admin-doc/admin_tasks/admin_tasks.rst
+peek_core_search/admin-doc/admin_tasks/exclude_keyword.png
+peek_core_search/admin-doc/admin_tasks/general_settings.png
+peek_core_search/admin-doc/admin_tasks/remove_exclude.png
 peek_core_search/admin-doc/status/status.png
 peek_core_search/admin-doc/status/status.rst
 peek_core_search/both-doc/index.rst
 peek_core_search/both-doc/search_button.png
 peek_core_search/both-doc/search_filtered.png
 peek_core_search/both-doc/search_popup.png
 peek_core_search/both-doc/searching.rst
@@ -145,22 +155,21 @@
 peek_core_search/plugin-module/_private/KeywordSplitter.ts
 peek_core_search/plugin-module/_private/PluginNames.ts
 peek_core_search/plugin-module/_private/SearchTupleService.ts
 peek_core_search/plugin-module/_private/fast-keyword-controller.ts
 peek_core_search/plugin-module/_private/index.ts
 peek_core_search/plugin-module/_private/search-index-loader/EncodedSearchIndexChunkTuple.ts
 peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts
-peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderStatusTuple.ts
 peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts
 peek_core_search/plugin-module/_private/search-index-loader/index.ts
 peek_core_search/plugin-module/_private/search-object-loader/EncodedSearchObjectChunkTuple.ts
 peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts
-peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderStatusTuple.ts
 peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts
 peek_core_search/plugin-module/_private/search-object-loader/index.ts
+peek_core_search/plugin-module/_private/tuples/ExcludeSearchStringsTuple.ts
 peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts
 peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts
 peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts
 peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
 peek_core_search/server/SearchApiABC.py
 peek_core_search/server/__init__.py
 peek_core_search/tuples/ImportSearchObjectRouteTuple.py
```

### Comparing `peek-core-search-3.3.3/setup.py` & `peek-core-search-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_search"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin Search - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

