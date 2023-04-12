# Comparing `tmp/peek-core-docdb-3.3.3.tar.gz` & `tmp/peek-core-docdb-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-docdb-3.3.3.tar", last modified: Mon Nov 14 05:35:28 2022, max compression
+gzip compressed data, was "peek-core-docdb-3.4.0.tar", last modified: Wed Apr 12 11:04:14 2023, max compression
```

## Comparing `peek-core-docdb-3.3.3.tar` & `peek-core-docdb-3.4.0.tar`

### file list

```diff
@@ -1,187 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.676470 peek-core-docdb-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      368 2022-11-14 05:35:28.676470 peek-core-docdb-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.661470 peek-core-docdb-3.3.3/peek_core_docdb/
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1155 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/peek_core_docdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.662470 peek-core-docdb-3.3.3/peek_core_docdb/_private/
--rw-r--r--   0 root         (0) root         (0)      214 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.662470 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)     3281 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/docDb.component.html
--rw-r--r--   0 root         (0) root         (0)      456 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/docDb.component.ts
--rw-r--r--   0 root         (0) root         (0)     2675 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/docDb.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.662470 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-object-type-table/
--rw-r--r--   0 root         (0) root         (0)     1127 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     3114 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.663470 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-property-table/
--rw-r--r--   0 root         (0) root         (0)     1999 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2314 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.663470 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1459 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.663470 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/status/
--rw-r--r--   0 root         (0) root         (0)      890 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      987 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/status/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.663470 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/view-document/
--rw-r--r--   0 root         (0) root         (0)     1515 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/view-document/view-document.html
--rw-r--r--   0 root         (0) root         (0)     1899 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/view-document/view-document.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.663470 peek-core-docdb-3.3.3/peek_core_docdb/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      556 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.664470 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      317 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.664470 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2969 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py
--rw-r--r--   0 root         (0) root         (0)     1063 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py
--rw-r--r--   0 root         (0) root         (0)     2030 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2625 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py
--rw-r--r--   0 root         (0) root         (0)     8149 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.664470 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.664470 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.665470 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/
--rw-r--r--   0 root         (0) root         (0)       35 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/index.ts
--rw-r--r--   0 root         (0) root         (0)     3488 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/popup.component.html
--rw-r--r--   0 root         (0) root         (0)      520 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/popup.component.scss
--rw-r--r--   0 root         (0) root         (0)     6434 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/popup.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.665470 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/debug-page/
--rw-r--r--   0 root         (0) root         (0)      726 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html
--rw-r--r--   0 root         (0) root         (0)     2338 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts
--rw-r--r--   0 root         (0) root         (0)     1056 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts
--rw-r--r--   0 root         (0) root         (0)     1024 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/docdb-popup.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.665470 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    12054 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.666470 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-cfg/
--rw-r--r--   0 root         (0) root         (0)      999 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-cfg/docdb-cfg.component.ts
--rw-r--r--   0 root         (0) root         (0)      383 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-cfg/docdb-cfg.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1132 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/both-cfg/docdb-cfg.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.666470 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/
--rw-r--r--   0 root         (0) root         (0)     5938 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      501 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)     1292 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.666470 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/controller/
--rw-r--r--   0 root         (0) root         (0)     1194 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/controller/DocumentCacheController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.666470 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     1052 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)      176 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.667470 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     3508 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1002 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.667470 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/
--rw-r--r--   0 root         (0) root         (0)     9607 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      526 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     2632 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.668470 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1612 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)     1638 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py
--rw-r--r--   0 root         (0) root         (0)      971 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      895 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py
--rw-r--r--   0 root         (0) root         (0)      811 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.668470 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)      660 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/api/DocDbApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.668470 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     1821 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)      752 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.669470 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     3991 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)      454 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/ImportController.py
--rw-r--r--   0 root         (0) root         (0)      820 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/StatusController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.669470 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      904 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1115 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1237 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1031 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)      991 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.670470 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      710 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1105 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     1822 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbDocument.py
--rw-r--r--   0 root         (0) root         (0)     1089 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py
--rw-r--r--   0 root         (0) root         (0)     2283 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbEncodedChunk.py
--rw-r--r--   0 root         (0) root         (0)      610 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbModelSet.py
--rw-r--r--   0 root         (0) root         (0)     1441 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbPropertyTuple.py
--rw-r--r--   0 root         (0) root         (0)     7642 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.670470 peek-core-docdb-3.3.3/peek_core_docdb/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      454 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/tuples/AdminStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)     1263 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.671470 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/
--rw-r--r--   0 root         (0) root         (0)      874 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.671470 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     6109 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)    11202 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/ImportTask.py
--rw-r--r--   0 root         (0) root         (0)      704 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.671470 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.672470 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)    38648 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png
--rw-r--r--   0 root         (0) root         (0)    54690 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png
--rw-r--r--   0 root         (0) root         (0)     2340 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)   104337 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/view_document.png
--rw-r--r--   0 root         (0) root         (0)      341 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1511 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.672470 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/status/
--rw-r--r--   0 root         (0) root         (0)    37793 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/status/status.png
--rw-r--r--   0 root         (0) root         (0)      437 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/status/status.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.673470 peek-core-docdb-3.3.3/peek_core_docdb/both-doc/
--rw-r--r--   0 root         (0) root         (0)      113 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      171 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/both-doc/offline_support.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.673470 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      574 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts
--rw-r--r--   0 root         (0) root         (0)      502 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbModelSetTuple.ts
--rw-r--r--   0 root         (0) root         (0)     4381 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbPopupService.ts
--rw-r--r--   0 root         (0) root         (0)      871 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2851 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbService.ts
--rw-r--r--   0 root         (0) root         (0)      758 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocumentTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.674470 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)     2663 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts
--rw-r--r--   0 root         (0) root         (0)      382 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/PluginNames.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.674470 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/admin/
--rw-r--r--   0 root         (0) root         (0)      494 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/admin/AdminStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      567 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.674470 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/
--rw-r--r--   0 root         (0) root         (0)      584 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      426 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/EncodedDocumentChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    21294 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      541 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      334 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/index.ts
--rw-r--r--   0 root         (0) root         (0)      302 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.674470 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)    11450 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.675470 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/constants/
--rw-r--r--   0 root         (0) root         (0)       52 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/constants/docdb.constants.ts
--rw-r--r--   0 root         (0) root         (0)       35 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/constants/index.ts
--rw-r--r--   0 root         (0) root         (0)      627 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)     4042 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/peek_core_docdb/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.675470 peek-core-docdb-3.3.3/peek_core_docdb/server/
--rw-r--r--   0 root         (0) root         (0)      915 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/server/DocDbApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.675470 peek-core-docdb-3.3.3/peek_core_docdb/tuples/
--rw-r--r--   0 root         (0) root         (0)      797 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/tuples/DocumentTuple.py
--rw-r--r--   0 root         (0) root         (0)     1070 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/tuples/ImportDocumentTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2022-11-14 05:34:26.000000 peek-core-docdb-3.3.3/peek_core_docdb/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:28.662470 peek-core-docdb-3.3.3/peek_core_docdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      368 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/peek_core_docdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8001 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/peek_core_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/peek_core_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/peek_core_docdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/peek_core_docdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:35:28.676470 peek-core-docdb-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2481 2022-11-14 05:35:28.000000 peek-core-docdb-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.871215 peek-core-docdb-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-12 11:04:14.871215 peek-core-docdb-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.864215 peek-core-docdb-3.4.0/peek_core_docdb/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/peek_core_docdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb/_private/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/docDb.component.html
+-rw-r--r--   0 root         (0) root         (0)      456 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/docDb.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/docDb.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-object-type-table/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-property-table/
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/status/
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/status/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/view-document/
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/view-document/view-document.html
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/view-document/view-document.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py
+-rw-r--r--   0 root         (0) root         (0)     8149 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/index.ts
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/popup.component.html
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/popup.component.scss
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/popup.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/debug-page/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/docdb-popup.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.866215 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.867215 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     5938 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      489 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.867215 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/controller/DocumentCacheController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.867215 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.867215 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.867215 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     9607 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.867215 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py
+-rw-r--r--   0 root         (0) root         (0)      811 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.868215 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/api/DocDbApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.868215 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.868215 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     3991 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/ImportController.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/StatusController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.868215 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.869215 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      710 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbDocument.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbEncodedChunk.py
+-rw-r--r--   0 root         (0) root         (0)      610 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbModelSet.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbPropertyTuple.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.869215 peek-core-docdb-3.4.0/peek_core_docdb/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/tuples/AdminStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.869215 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)      874 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.869215 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     6536 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)    11202 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/ImportTask.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.869215 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.869215 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)    38648 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png
+-rw-r--r--   0 root         (0) root         (0)    54690 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)   104337 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/view_document.png
+-rw-r--r--   0 root         (0) root         (0)      341 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.870215 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/status/
+-rw-r--r--   0 root         (0) root         (0)    37793 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/status/status.png
+-rw-r--r--   0 root         (0) root         (0)      437 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/status/status.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.870215 peek-core-docdb-3.4.0/peek_core_docdb/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/both-doc/offline_support.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.870215 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      502 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbModelSetTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     4381 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbPopupService.ts
+-rw-r--r--   0 root         (0) root         (0)      871 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbService.ts
+-rw-r--r--   0 root         (0) root         (0)      758 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocumentTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.870215 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts
+-rw-r--r--   0 root         (0) root         (0)      382 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/PluginNames.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.870215 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/admin/
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/admin/AdminStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      567 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.871215 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/document-loader/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/document-loader/EncodedDocumentChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    21264 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/document-loader/index.ts
+-rw-r--r--   0 root         (0) root         (0)      302 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.871215 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)    11450 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.871215 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/constants/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/constants/docdb.constants.ts
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/constants/index.ts
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/peek_core_docdb/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.871215 peek-core-docdb-3.4.0/peek_core_docdb/server/
+-rw-r--r--   0 root         (0) root         (0)      915 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/server/DocDbApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.871215 peek-core-docdb-3.4.0/peek_core_docdb/tuples/
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/tuples/DocumentTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/tuples/ImportDocumentTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-12 11:03:17.000000 peek-core-docdb-3.4.0/peek_core_docdb/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:14.865215 peek-core-docdb-3.4.0/peek_core_docdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/peek_core_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/peek_core_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/peek_core_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/peek_core_docdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/peek_core_docdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:04:14.872215 peek-core-docdb-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-04-12 11:04:14.000000 peek-core-docdb-3.4.0/setup.py
```

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/__init__.py` & `peek-core-docdb-3.4.0/peek_core_docdb/__init__.py`

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

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/docDb.component.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/docDb.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/docDb.module.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/docDb.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/status/status.component.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/status/status.component.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/view-document/view-document.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/view-document/view-document.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/admin-app/view-document/view-document.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/admin-app/view-document/view-document.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/agent/AgentEntryHook.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/script.py.mako` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/popup.component.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/popup.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/popup.component.scss` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/popup.component.scss`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/components/popup/popup.component.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/components/popup/popup.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-app/docdb-popup.module.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-app/docdb-popup.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/both-assets/icon.png` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/client/ClientEntryHook.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/client/TupleDataObservable.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/client/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/client/controller/DocumentCacheController.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/client/controller/DocumentCacheController.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 
     """
 
     _ChunkedTuple = DocDbEncodedChunk
     _UpdateDateTupleABC = DocumentUpdateDateTuple
     _chunkLoadRpcMethod = ClientChunkLoadRpc.loadDocumentChunks
     _chunkIndexDeltaRpcMethod = ClientChunkLoadRpc.loadDocumentIndexDelta
-    _updateFromServerFilt = clientDocumentUpdateFromServerFilt
+    _updateFromLogicFilt = clientDocumentUpdateFromServerFilt
     _logger = logger
```

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/LogicEntryHook.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/TupleActionProcessor.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/TupleDataObservable.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/admin_backend/__init__.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/admin_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/api/DocDbApi.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/api/DocDbApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,28 +31,28 @@
         yield self.loadDocumentIndexDelta.start(funcSelf=self)
         logger.debug("RPCs started")
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=docDbFilt,
         deferToThread=True,
     )
     def loadDocumentIndexDelta(self, indexEncodedPayload: bytes) -> bytes:
         return self.ckiChunkIndexDeltaBlocking(
             indexEncodedPayload, DocDbEncodedChunk, DocumentUpdateDateTuple
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=docDbFilt,
         deferToThread=True,
     )
     def loadDocumentChunks(self, chunkKeys: list[str]) -> list[Tuple]:
         return self.ckiInitialLoadChunksPayloadBlocking(
             chunkKeys, DocDbEncodedChunk
         )
```

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/controller/MainController.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DeclarativeBase.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbCompilerQueue.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbDocument.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbDocument.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbEncodedChunk.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbEncodedChunk.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbModelSet.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbModelSet.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/DocDbPropertyTuple.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/DocDbPropertyTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/storage/Setting.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/WorkerEntryHook.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/WorkerEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import pytz
 from sqlalchemy import select
 from txcelery.defer import DeferrableTask
 from vortex.Payload import Payload
 
 from peek_plugin_base.worker import CeleryDbConn
 from peek_plugin_base.worker.CeleryApp import celeryApp
-from peek_core_docdb._private.storage.DocDbCompilerQueue import DocDbCompilerQueue
+from peek_core_docdb._private.storage.DocDbCompilerQueue import (
+    DocDbCompilerQueue,
+)
 from peek_core_docdb._private.storage.DocDbDocument import DocDbDocument
 from peek_core_docdb._private.storage.DocDbEncodedChunk import DocDbEncodedChunk
 
 logger = logging.getLogger(__name__)
 
 """ DocDb Index Compiler
 
@@ -27,15 +29,15 @@
 2) Process queue
 3) Delete from queue
 """
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileDocumentChunk(self, payloadEncodedArgs: bytes) -> List[int]:
+def compileDocumentChunk(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile DocDb Index Task
 
     :param self: The reference to this celery task
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
@@ -47,16 +49,21 @@
     transaction = conn.begin()
     try:
         queueItemsByModelSetId = defaultdict(list)
 
         for queueItem in queueItems:
             queueItemsByModelSetId[queueItem.modelSetId].append(queueItem)
 
+        lastUpdateByChunkKey = {}
         for modelSetId, modelSetQueueItems in queueItemsByModelSetId.items():
-            _compileDocumentChunk(conn, transaction, modelSetId, modelSetQueueItems)
+            lastUpdateByChunkKey.update(
+                _compileDocumentChunk(
+                    conn, transaction, modelSetId, modelSetQueueItems
+                )
+            )
 
         queueTable = DocDbCompilerQueue.__table__
 
         transaction = conn.begin()
         conn.execute(queueTable.delete(queueTable.c.id.in_(queueItemIds)))
         transaction.commit()
 
@@ -64,20 +71,20 @@
         transaction.rollback()
         logger.debug("RETRYING task - %s", e)
         raise self.retry(exc=e, countdown=10)
 
     finally:
         conn.close()
 
-    return list(set([i.chunkKey for i in queueItems]))
+    return lastUpdateByChunkKey
 
 
 def _compileDocumentChunk(
     conn, transaction, modelSetId: int, queueItems: List[DocDbCompilerQueue]
-) -> None:
+) -> dict[str, str]:
     chunkKeys = list(set([i.chunkKey for i in queueItems]))
 
     compiledTable = DocDbEncodedChunk.__table__
     lastUpdate = datetime.now(pytz.utc).isoformat()
 
     startTime = datetime.now(pytz.utc)
 
@@ -90,27 +97,34 @@
     # Get Model Sets
 
     total = 0
     existingHashes = _loadExistingHashes(conn, chunkKeys)
     encKwPayloadByChunkKey = _buildIndex(chunkKeys)
     chunksToDelete = []
 
+    lastUpdateByChunkKey = {}
+
     inserts = []
-    for chunkKey, docDbIndexChunkEncodedPayload in encKwPayloadByChunkKey.items():
+    for (
+        chunkKey,
+        docDbIndexChunkEncodedPayload,
+    ) in encKwPayloadByChunkKey.items():
         m = hashlib.sha256()
         m.update(docDbIndexChunkEncodedPayload)
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
                 encodedData=docDbIndexChunkEncodedPayload,
                 encodedHash=encodedHash,
@@ -119,18 +133,22 @@
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
-        newIdGen = CeleryDbConn.prefetchDeclarativeIds(DocDbDocument, len(inserts))
+        newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+            DocDbDocument, len(inserts)
+        )
         for insert in inserts:
             insert["id"] = next(newIdGen)
 
     transaction.commit()
     transaction = conn.begin()
 
     if inserts:
@@ -148,14 +166,16 @@
     transaction.commit()
     logger.info(
         "Compiled and Committed %s EncodedDocumentChunks in %s",
         total,
         (datetime.now(pytz.utc) - startTime),
     )
 
+    return lastUpdateByChunkKey
+
 
 def _loadExistingHashes(conn, chunkKeys: List[str]) -> Dict[str, str]:
     compiledTable = DocDbEncodedChunk.__table__
 
     results = conn.execute(
         select(
             columns=[compiledTable.c.chunkKey, compiledTable.c.encodedHash],
@@ -168,35 +188,41 @@
 
 def _buildIndex(chunkKeys) -> Dict[str, bytes]:
     session = CeleryDbConn.getDbSession()
 
     try:
         indexQry = (
             session.query(
-                DocDbDocument.chunkKey, DocDbDocument.key, DocDbDocument.documentJson
+                DocDbDocument.chunkKey,
+                DocDbDocument.key,
+                DocDbDocument.documentJson,
             )
             .filter(DocDbDocument.chunkKey.in_(chunkKeys))
             .order_by(DocDbDocument.key)
             .yield_per(1000)
             .all()
         )
 
         # Create the ChunkKey -> {id -> packedJson, id -> packedJson, ....]
         packagedJsonByObjIdByChunkKey = defaultdict(dict)
 
         for item in indexQry:
-            packagedJsonByObjIdByChunkKey[item.chunkKey][item.key] = item.documentJson
+            packagedJsonByObjIdByChunkKey[item.chunkKey][
+                item.key
+            ] = item.documentJson
 
         encPayloadByChunkKey = {}
 
         # Sort each bucket by the key
         for chunkKey, packedJsonByKey in packagedJsonByObjIdByChunkKey.items():
             tuples = json.dumps(packedJsonByKey, sort_keys=True)
 
             # Create the blob data for this index.
             # It will be docDbed by a binary sort
-            encPayloadByChunkKey[chunkKey] = Payload(tuples=tuples).toEncodedPayload()
+            encPayloadByChunkKey[chunkKey] = (
+                Payload(tuples=tuples).toEncodedPayload().encode()
+            )
 
         return encPayloadByChunkKey
 
     finally:
         session.close()
```

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/ImportTask.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/ImportTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py` & `peek-core-docdb-3.4.0/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png` & `peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png` & `peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst` & `peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/admin_tasks/view_document.png` & `peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/admin_tasks/view_document.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/overview.rst` & `peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/admin-doc/status/status.png` & `peek-core-docdb-3.4.0/peek_core_docdb/admin-doc/status/status.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbPopupService.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbPopupService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocDbService.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocDbService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/DocumentTuple.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/DocumentTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,18 @@
     docDbTuplePrefix,
 } from "../PluginNames";
 import { EncodedDocumentChunkTuple } from "./EncodedDocumentChunkTuple";
 import { DocumentUpdateDateTuple } from "./DocumentUpdateDateTuple";
 import { DocumentTuple } from "../../DocumentTuple";
 import { DocDbTupleService } from "../DocDbTupleService";
 import { DocDbDocumentTypeTuple } from "../../DocDbDocumentTypeTuple";
-import { PrivateDocumentLoaderStatusTuple } from "./PrivateDocumentLoaderStatusTuple";
 import { DocDbModelSetTuple } from "../../DocDbModelSetTuple";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 
 // ----------------------------------------------------------------------------
 
 export interface DocumentResultI {
     [key: string]: DocumentTuple;
 }
@@ -125,24 +124,24 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new DocumentUpdateDateTuple();
+    private index: DocumentUpdateDateTuple | null;
     private askServerChunks: DocumentUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
     private _hasLoadedSubject = new Subject<void>();
 
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject = new Subject<PrivateDocumentLoaderStatusTuple>();
-    private _status = new PrivateDocumentLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     private objectTypesByIds: { [id: number]: DocDbDocumentTypeTuple } = {};
     private _hasDocTypeLoaded = false;
 
     private modelSetByIds: { [id: number]: DocDbModelSetTuple } = {};
     private _hasModelSetLoaded = false;
 
@@ -151,14 +150,17 @@
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         private tupleService: DocDbTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
 
+        this._status.pluginName = "peek_core_docdb";
+        this._status.indexName = "Document Index";
+
         let objTypeTs = new TupleSelector(DocDbDocumentTypeTuple.tupleName, {});
         this.tupleService.offlineObserver
             .subscribeToTupleSelector(objTypeTs)
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((tuples: DocDbDocumentTypeTuple[]) => {
                 this.objectTypesByIds = {};
                 for (let item of tuples) {
@@ -183,38 +185,52 @@
 
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(docDbCacheStorageName)
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
 
-    statusObservable(): Observable<PrivateDocumentLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): PrivateDocumentLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     get offlineEnabled(): boolean {
         return this.index.initialLoadComplete;
     }
 
@@ -282,81 +298,67 @@
             this._hasDocTypeLoaded &&
             this._hasModelSetLoaded &&
             this._hasLoaded
         )
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
-        status.pluginName = "peek_core_docdb";
-        status.indexName = "Document Index";
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
                 let tuples: DocumentUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new DocumentUpdateDateTuple();
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
                 clientDocumentWatchUpdateFromDeviceFilt
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
@@ -380,15 +382,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: DocumentUpdateDateTuple = tuplesAny[0];
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
@@ -430,35 +432,37 @@
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
-                let indexChunk: DocumentUpdateDateTuple =
-                    this.askServerChunks.pop();
-                let filt = extend({}, clientDocumentWatchUpdateFromDeviceFilt);
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
+        let indexChunk: DocumentUpdateDateTuple = this.askServerChunks.pop();
+        let filt = extend({}, clientDocumentWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let pl = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(pl);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process Documentes From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(payloadEnvelope: PayloadEnvelope) {
@@ -520,14 +524,16 @@
 
     /** Store Chunk Cache Index
      *
      * Updates our running tab of the update dates of the cached chunks
      *
      */
     private async saveChunkCacheIndex(force = false): Promise<void> {
+        if (this.index == null) return;
+
         if (
             this.chunksSavedSinceLastIndexSave <= this.SAVE_POINT_ITERATIONS &&
             !force
         ) {
             return;
         }
```

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin-module/index.ts` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin-module/index.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/plugin_package.json` & `peek-core-docdb-3.4.0/peek_core_docdb/plugin_package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9775132275132274%*

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
         "appModule": "debug-page/debug-page.module#DocDbPopupDebugModule",
         "assetDir": "_private/both-assets",
-        "cfgDir": "_private/both-cfg",
-        "cfgModule": "docdb-cfg.module#DocDBCfgModule",
         "icon": "",
         "moduleDir": "plugin-module",
         "rootComponents": [
             {
                 "selector": "popup-component"
             }
         ],
@@ -59,16 +57,14 @@
         "subprocessGroup": "docdb"
     },
     "logic": {},
     "office": {
         "appDir": "_private/both-app",
         "appModule": "debug-page/debug-page.module#DocDbPopupDebugModule",
         "assetDir": "_private/both-assets",
-        "cfgDir": "_private/both-cfg",
-        "cfgModule": "docdb-cfg.module#DocDBCfgModule",
         "icon": "",
         "moduleDir": "plugin-module",
         "rootComponents": [
             {
                 "selector": "popup-component"
             }
         ],
@@ -113,15 +109,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_docdb",
         "title": "Document DB",
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

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/server/DocDbApiABC.py` & `peek-core-docdb-3.4.0/peek_core_docdb/server/DocDbApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/tuples/DocumentTuple.py` & `peek-core-docdb-3.4.0/peek_core_docdb/tuples/DocumentTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb/tuples/ImportDocumentTuple.py` & `peek-core-docdb-3.4.0/peek_core_docdb/tuples/ImportDocumentTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.3.3/peek_core_docdb.egg-info/SOURCES.txt` & `peek-core-docdb-3.4.0/peek_core_docdb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,14 @@
 peek_core_docdb/_private/both-app/components/popup/popup.component.html
 peek_core_docdb/_private/both-app/components/popup/popup.component.scss
 peek_core_docdb/_private/both-app/components/popup/popup.component.ts
 peek_core_docdb/_private/both-app/debug-page/debug-page.component.html
 peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts
 peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts
 peek_core_docdb/_private/both-assets/icon.png
-peek_core_docdb/_private/both-cfg/docdb-cfg.component.ts
-peek_core_docdb/_private/both-cfg/docdb-cfg.component.web.html
-peek_core_docdb/_private/both-cfg/docdb-cfg.module.ts
 peek_core_docdb/_private/client/ClientEntryHook.py
 peek_core_docdb/_private/client/DeviceTupleDataObservableProxy.py
 peek_core_docdb/_private/client/DeviceTupleProcessorActionProxy.py
 peek_core_docdb/_private/client/TupleDataObservable.py
 peek_core_docdb/_private/client/__init__.py
 peek_core_docdb/_private/client/controller/DocumentCacheController.py
 peek_core_docdb/_private/client/controller/__init__.py
@@ -124,15 +121,14 @@
 peek_core_docdb/plugin-module/_private/PluginNames.ts
 peek_core_docdb/plugin-module/_private/index.ts
 peek_core_docdb/plugin-module/_private/admin/AdminStatusTuple.ts
 peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts
 peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts
 peek_core_docdb/plugin-module/_private/document-loader/EncodedDocumentChunkTuple.ts
 peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts
-peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderStatusTuple.ts
 peek_core_docdb/plugin-module/_private/document-loader/index.ts
 peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts
 peek_core_docdb/plugin-module/constants/docdb.constants.ts
 peek_core_docdb/plugin-module/constants/index.ts
 peek_core_docdb/server/DocDbApiABC.py
 peek_core_docdb/server/__init__.py
 peek_core_docdb/tuples/DocumentTuple.py
```

### Comparing `peek-core-docdb-3.3.3/setup.py` & `peek-core-docdb-3.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_docdb"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Core Plugin DocDB."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

