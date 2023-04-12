# Comparing `tmp/peek-plugin-branch-3.3.3.tar.gz` & `tmp/peek-plugin-branch-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-branch-3.3.3.tar", last modified: Mon Nov 14 05:36:58 2022, max compression
+gzip compressed data, was "peek-plugin-branch-3.4.0.tar", last modified: Wed Apr 12 11:05:43 2023, max compression
```

## Comparing `peek-plugin-branch-3.3.3.tar` & `peek-plugin-branch-3.4.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.337880 peek-plugin-branch-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      396 2022-11-14 05:36:58.337880 peek-plugin-branch-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.328881 peek-plugin-branch-3.3.3/peek_plugin_branch/
--rw-r--r--   0 root         (0) root         (0)      680 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.329881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/
--rw-r--r--   0 root         (0) root         (0)      274 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.329881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)     1626 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/branch.component.html
--rw-r--r--   0 root         (0) root         (0)      209 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/branch.component.ts
--rw-r--r--   0 root         (0) root         (0)      887 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/branch.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.329881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/
--rw-r--r--   0 root         (0) root         (0)     1575 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2380 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.330880 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1464 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.330880 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      323 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.330880 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2659 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/versions/53e411bea4ab_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)      828 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/versions/87f770b6a183_removed_location_field.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.331881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.332881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch-detail/
--rw-r--r--   0 root         (0) root         (0)     1228 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.dweb.html
--rw-r--r--   0 root         (0) root         (0)     1228 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     1631 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.ts
--rw-r--r--   0 root         (0) root         (0)      333 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch.component.dweb.html
--rw-r--r--   0 root         (0) root         (0)      333 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)      192 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch.component.ts
--rw-r--r--   0 root         (0) root         (0)     2776 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.332881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    12054 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.333881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/client/
--rw-r--r--   0 root         (0) root         (0)     2111 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      511 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      499 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.333881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/
--rw-r--r--   0 root         (0) root         (0)      831 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/BranchApi.py
--rw-r--r--   0 root         (0) root         (0)     3353 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1057 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.334880 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1759 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/admin_backend/BranchDetailTupleHandler.py
--rw-r--r--   0 root         (0) root         (0)      979 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      451 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.334880 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     2565 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.334880 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1243 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/tuple_providers/BranchDetailTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.335881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/
--rw-r--r--   0 root         (0) root         (0)     1210 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/BranchDetailTable.py
--rw-r--r--   0 root         (0) root         (0)      709 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     7699 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.335881 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      422 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/tuples/CreateBranchActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.335881 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      999 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/BranchDetailTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1694 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/BranchService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.336881 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      345 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      235 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.336881 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)     2649 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/services/PrivateBranchTupleService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.336881 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      472 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/tuples/CreateBranchActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      569 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/tuples/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      106 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)     1943 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.336881 peek-plugin-branch-3.3.3/peek_plugin_branch/server/
--rw-r--r--   0 root         (0) root         (0)      421 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/server/BranchApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.336881 peek-plugin-branch-3.3.3/peek_plugin_branch/tuples/
--rw-r--r--   0 root         (0) root         (0)     1081 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/tuples/BranchDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2022-11-14 05:34:28.000000 peek-plugin-branch-3.3.3/peek_plugin_branch/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:58.329881 peek-plugin-branch-3.3.3/peek_plugin_branch.egg-info/
--rw-r--r--   0 root         (0) root         (0)      396 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/peek_plugin_branch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3752 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/peek_plugin_branch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/peek_plugin_branch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/peek_plugin_branch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/peek_plugin_branch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:36:58.337880 peek-plugin-branch-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2494 2022-11-14 05:36:58.000000 peek-plugin-branch-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.705203 peek-plugin-branch-3.4.0/peek_plugin_branch/
+-rw-r--r--   0 root         (0) root         (0)      680 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.705203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.705203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/branch.component.html
+-rw-r--r--   0 root         (0) root         (0)      209 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/branch.component.ts
+-rw-r--r--   0 root         (0) root         (0)      887 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/branch.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.706203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.706203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.706203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.706203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/versions/53e411bea4ab_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/versions/87f770b6a183_removed_location_field.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.706203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.706203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch-detail/
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.dweb.html
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.ts
+-rw-r--r--   0 root         (0) root         (0)      333 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch.component.dweb.html
+-rw-r--r--   0 root         (0) root         (0)      333 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.706203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.707203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      511 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.707203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/
+-rw-r--r--   0 root         (0) root         (0)      831 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/BranchApi.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.707203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/admin_backend/BranchDetailTupleHandler.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.707203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     2565 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.707203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/tuple_providers/BranchDetailTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.707203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/BranchDetailTable.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     7699 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.707203 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      422 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/tuples/CreateBranchActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/BranchDetailTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/BranchService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      235 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/services/PrivateBranchTupleService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/tuples/CreateBranchActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      569 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/tuples/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/peek_plugin_branch/server/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/server/BranchApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.708203 peek-plugin-branch-3.4.0/peek_plugin_branch/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/tuples/BranchDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-12 11:03:19.000000 peek-plugin-branch-3.4.0/peek_plugin_branch/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:43.705203 peek-plugin-branch-3.4.0/peek_plugin_branch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/peek_plugin_branch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/peek_plugin_branch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/peek_plugin_branch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/peek_plugin_branch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/peek_plugin_branch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:05:43.709203 peek-plugin-branch-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-04-12 11:05:43.000000 peek-plugin-branch-3.4.0/setup.py
```

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/__init__.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/branch.component.html` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/branch.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/branch.module.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/branch.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.html` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-branch-detail-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/script.py.mako` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/versions/53e411bea4ab_initial_tables.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/versions/53e411bea4ab_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/alembic/versions/87f770b6a183_removed_location_field.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/alembic/versions/87f770b6a183_removed_location_field.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.dweb.html` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.dweb.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.mweb.html` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.mweb.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch-detail/branch-detail.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-app/branch.module.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-app/branch.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/both-assets/icon.png` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/client/ClientEntryHook.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/BranchApi.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/BranchApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/LogicEntryHook.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/TupleActionProcessor.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/TupleDataObservable.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/admin_backend/BranchDetailTupleHandler.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/admin_backend/BranchDetailTupleHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/controller/MainController.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/server/tuple_providers/BranchDetailTupleProvider.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/server/tuple_providers/BranchDetailTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/BranchDetailTable.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/BranchDetailTable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/DeclarativeBase.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/_private/storage/Setting.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/BranchDetailTuple.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/BranchDetailTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/BranchService.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/BranchService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/services/PrivateBranchTupleService.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/services/PrivateBranchTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/plugin-module/_private/tuples/SettingPropertyTuple.ts` & `peek-plugin-branch-3.4.0/peek_plugin_branch/plugin-module/_private/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/plugin_package.json` & `peek-plugin-branch-3.4.0/peek_plugin_branch/plugin_package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'plugin'": "{'version': '3.4.0'}"}*

```diff
@@ -49,15 +49,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_branch",
         "title": "Model Branches",
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

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch/tuples/BranchDetailTuple.py` & `peek-plugin-branch-3.4.0/peek_plugin_branch/tuples/BranchDetailTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/peek_plugin_branch.egg-info/SOURCES.txt` & `peek-plugin-branch-3.4.0/peek_plugin_branch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-branch-3.3.3/setup.py` & `peek-plugin-branch-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_branch"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin Branch - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

