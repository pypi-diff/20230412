# Comparing `tmp/peek-plugin-diagram-trace-3.3.3.tar.gz` & `tmp/peek-plugin-diagram-trace-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-diagram-trace-3.3.3.tar", last modified: Mon Nov 14 05:37:18 2022, max compression
+gzip compressed data, was "peek-plugin-diagram-trace-3.4.0.tar", last modified: Wed Apr 12 11:06:05 2023, max compression
```

## Comparing `peek-plugin-diagram-trace-3.3.3.tar` & `peek-plugin-diagram-trace-3.4.0.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.594747 peek-plugin-diagram-trace-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      423 2022-11-14 05:37:18.593747 peek-plugin-diagram-trace-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.590747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/
--rw-r--r--   0 root         (0) root         (0)      679 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.591747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/
--rw-r--r--   0 root         (0) root         (0)      299 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.591747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)     1099 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html
--rw-r--r--   0 root         (0) root         (0)      227 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.ts
--rw-r--r--   0 root         (0) root         (0)      772 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.591747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1490 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.591747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      337 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.591747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1952 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.591747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/
--rw-r--r--   0 root         (0) root         (0)     2043 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      549 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      546 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/
--rw-r--r--   0 root         (0) root         (0)     3065 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      583 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1871 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      318 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)      720 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1006 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      716 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     7799 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      197 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.592747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)      606 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)    45670 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png
--rw-r--r--   0 root         (0) root         (0)      226 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.593747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/
--rw-r--r--   0 root         (0) root         (0)     8724 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/clear_trace_button.png
--rw-r--r--   0 root         (0) root         (0)      167 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)    10636 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/trace_button.png
--rw-r--r--   0 root         (0) root         (0)    16807 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/trace_popup.png
--rw-r--r--   0 root         (0) root         (0)      480 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/tracing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.590747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.593747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      423 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      101 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.593747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)    10675 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts
--rw-r--r--   0 root         (0) root         (0)     2016 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.593747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      707 2022-11-14 05:34:29.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1879 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:18.590747 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace.egg-info/
--rw-r--r--   0 root         (0) root         (0)      423 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3173 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:37:18.594747 peek-plugin-diagram-trace-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2507 2022-11-14 05:37:18.000000 peek-plugin-diagram-trace-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.255200 peek-plugin-diagram-trace-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-04-12 11:06:05.255200 peek-plugin-diagram-trace-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.252200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.252200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/
+-rw-r--r--   0 root         (0) root         (0)      299 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.253200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.ts
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.253200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.253200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.253200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.253200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      546 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.253200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      716 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     7799 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)      606 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    45670 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/
+-rw-r--r--   0 root         (0) root         (0)     8724 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/clear_trace_button.png
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)    10636 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/trace_button.png
+-rw-r--r--   0 root         (0) root         (0)    16807 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/trace_popup.png
+-rw-r--r--   0 root         (0) root         (0)      480 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/tracing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.254200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/DiagramTraceService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.255200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.255200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)    11217 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.255200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      707 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)       91 2023-04-12 11:03:20.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:05.252200 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:06:05.255200 peek-plugin-diagram-trace-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-04-12 11:06:05.000000 peek-plugin-diagram-trace-3.4.0/setup.py
```

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/__init__.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from typing import Type
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/script.py.mako` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/controller/MainController.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/_private/storage/Setting.py` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/clear_trace_button.png` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/clear_trace_button.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/trace_button.png` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/trace_button.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/both-doc/trace_popup.png` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/both-doc/trace_popup.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts`

 * *Files 4% similar despite different names*

```diff
@@ -12,46 +12,54 @@
 import {
     DocDbPopupActionI,
     DocDbPopupContextI,
     DocDbPopupService,
     DocDbPopupTypeE,
 } from "@peek/peek_core_docdb";
 import { DiagramOverrideColor } from "@peek/peek_plugin_diagram/override";
-import { DispColor } from "@peek/peek_plugin_diagram/lookups";
+import { ShapeColorTuple } from "@peek/peek_plugin_diagram/lookup_tuples";
 import { NgLifeCycleEvents, TupleSelector } from "@synerty/vortexjs";
 import { BalloonMsgService } from "@synerty/peek-plugin-base-js";
 import {
     GraphDbService,
     GraphDbTraceResultTuple,
     TraceConfigListItemI,
 } from "@peek/peek_plugin_graphdb";
 import { diagramTraceTuplePrefix } from "../PluginNames";
 import { PrivateDiagramTraceTupleService } from "./PrivateDiagramTraceTupleService";
 import {
     MaxTraceVertexesPropertyName,
     SettingPropertyTuple,
     TraceColorsPropertyName,
 } from "../tuples/SettingPropertyTuple";
+import {
+    DiagramTraceI,
+    DiagramTraceService,
+} from "@peek/peek_plugin_diagram_trace/DiagramTraceService";
 
 /** DMS Diagram Item Popup Service
  *
  * This service allows other plugins to add information to the item select popups.
  *
  * This is a helper service to simplify integrations with the diagram.
  *
  */
 @Injectable()
-export class PrivateDiagramTraceService extends NgLifeCycleEvents {
+export class PrivateDiagramTraceService
+    extends NgLifeCycleEvents
+    implements DiagramTraceService
+{
     private traceConfigsByModelSetKey: {
         [modelSetKey: string]: TraceConfigListItemI[];
     } = {};
     private appliedOverrides: DiagramOverrideColor[] = [];
+    private _activeTraces: DiagramTraceI[] = [];
     private readonly clearTracesButtonKey: string;
-    private originalColorsByModelSet: { [key: string]: DispColor[] } = {};
-    private colorsByModelSet: { [key: string]: DispColor[] } = {};
+    private originalColorsByModelSet: { [key: string]: ShapeColorTuple[] } = {};
+    private colorsByModelSet: { [key: string]: ShapeColorTuple[] } = {};
     private maxVertexes: number | null = null;
 
     constructor(
         private diagramCoordSetService: DiagramCoordSetService,
         private tupleService: PrivateDiagramTraceTupleService,
         private balloonMsg: BalloonMsgService,
         private diagramBranchService: DiagramBranchService,
@@ -74,14 +82,18 @@
                 .pipe(filter((ready) => ready))
                 .pipe(first())
                 .pipe(takeUntil(this.onDestroyEvent))
                 .subscribe(() => this.setup());
         }
     }
 
+    get activeTraces(): DiagramTraceI[] {
+        return this._activeTraces;
+    }
+
     private setup(): void {
         this.objectPopupService
             .popupObservable(DocDbPopupTypeE.summaryPopup)
             .pipe(
                 filter(
                     (c: DocDbPopupContextI) =>
                         c.triggeredByPlugin == diagramPluginName
@@ -269,14 +281,21 @@
         for (let vertex of traceResult.edges) {
             override.addDispKeys([vertex.key]);
         }
 
         this.diagramOverrideService.applyOverride(override);
         this.appliedOverrides.push(override);
 
+        this._activeTraces.push({
+            modelSetKey: context.modelSetKey,
+            startKey: context.key,
+            traceKey: traceKey,
+            traceModel: traceResult,
+        });
+
         this.addClearTracesButton(context.modelSetKey);
     }
 
     private addClearTracesButton(modelSetKey: string) {
         if (this.appliedOverrides.length != 1) return;
 
         this.diagramToolbar.addToolButton(
@@ -307,10 +326,12 @@
         }
 
         while (this.appliedOverrides.length != 0) {
             const override = this.appliedOverrides.pop();
             this.diagramOverrideService.removeOverride(override);
         }
 
+        this._activeTraces = [];
+
         this.removeClearTracesButton();
     }
 }
```

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace/plugin_package.json` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace/plugin_package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9876984126984127%*

 * *Differences: {"'field'": "{'rootServices': {1: {'file': 'DiagramTraceService', 'class': 'DiagramTraceService', "*

 * *            "'useClassFile': '_private/services/PrivateDiagramTraceService', 'useClassClass': "*

 * *            "'PrivateDiagramTraceService'}}}",*

 * * "'office'": "{'rootServices': {1: {'file': 'DiagramTraceService', 'class': 'DiagramTraceService', "*

 * *             "'useClassFile': '_private/services/PrivateDiagramTraceService', 'useClassClass': "*

 * *             "'PrivateDiagramTraceService'}}}",*

 * * "'plugin'": "{'version […]*

```diff
@@ -14,47 +14,51 @@
         "rootServices": [
             {
                 "class": "PrivateDiagramTraceTupleService",
                 "file": "_private/services/PrivateDiagramTraceTupleService",
                 "persistent": true
             },
             {
-                "class": "PrivateDiagramTraceService",
-                "file": "_private/services/PrivateDiagramTraceService",
-                "persistent": true
+                "class": "DiagramTraceService",
+                "file": "DiagramTraceService",
+                "persistent": true,
+                "useClassClass": "PrivateDiagramTraceService",
+                "useClassFile": "_private/services/PrivateDiagramTraceService"
             }
         ]
     },
     "logic": {},
     "office": {
         "moduleDir": "plugin-module",
         "rootServices": [
             {
                 "class": "PrivateDiagramTraceTupleService",
                 "file": "_private/services/PrivateDiagramTraceTupleService",
                 "persistent": true
             },
             {
-                "class": "PrivateDiagramTraceService",
-                "file": "_private/services/PrivateDiagramTraceService",
-                "persistent": true
+                "class": "DiagramTraceService",
+                "file": "DiagramTraceService",
+                "persistent": true,
+                "useClassClass": "PrivateDiagramTraceService",
+                "useClassFile": "_private/services/PrivateDiagramTraceService"
             }
         ]
     },
     "office-doc": {
         "docDir": "both-doc",
         "docRst": "index.rst"
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_diagram_trace",
         "title": "Diagram Trace",
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

### Comparing `peek-plugin-diagram-trace-3.3.3/peek_plugin_diagram_trace.egg-info/SOURCES.txt` & `peek-plugin-diagram-trace-3.4.0/peek_plugin_diagram_trace.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,14 @@
 peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst
 peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png
 peek_plugin_diagram_trace/both-doc/clear_trace_button.png
 peek_plugin_diagram_trace/both-doc/index.rst
 peek_plugin_diagram_trace/both-doc/trace_button.png
 peek_plugin_diagram_trace/both-doc/trace_popup.png
 peek_plugin_diagram_trace/both-doc/tracing.rst
+peek_plugin_diagram_trace/plugin-module/DiagramTraceService.ts
+peek_plugin_diagram_trace/plugin-module/index.ts
 peek_plugin_diagram_trace/plugin-module/_private/PluginNames.ts
 peek_plugin_diagram_trace/plugin-module/_private/index.ts
 peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts
 peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts
 peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts
```

### Comparing `peek-plugin-diagram-trace-3.3.3/setup.py` & `peek-plugin-diagram-trace-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_diagram_trace"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin DiagramTrace - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

