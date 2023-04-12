# Comparing `tmp/peek-plugin-inbox-3.3.3.tar.gz` & `tmp/peek-plugin-inbox-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-inbox-3.3.3.tar", last modified: Mon Nov 14 05:37:48 2022, max compression
+gzip compressed data, was "peek-plugin-inbox-3.4.0.tar", last modified: Wed Apr 12 11:06:39 2023, max compression
```

## Comparing `peek-plugin-inbox-3.3.3.tar` & `peek-plugin-inbox-3.4.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.605550 peek-plugin-inbox-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      369 2022-11-14 05:37:48.605550 peek-plugin-inbox-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      899 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.598550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/
--rw-r--r--   0 root         (0) root         (0)      271 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/TempUnitTest.py
--rw-r--r--   0 root         (0) root         (0)      836 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.599550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/
--rw-r--r--   0 root         (0) root         (0)      210 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.599550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.599550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/activity-list/
--rw-r--r--   0 root         (0) root         (0)     1112 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html
--rw-r--r--   0 root         (0) root         (0)     1259 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.css
--rw-r--r--   0 root         (0) root         (0)     2683 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html
--rw-r--r--   0 root         (0) root         (0)      290 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.ts
--rw-r--r--   0 root         (0) root         (0)     2671 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.599550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-activity/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.css
--rw-r--r--   0 root         (0) root         (0)     3060 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html
--rw-r--r--   0 root         (0) root         (0)     1581 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.599550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-task/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.css
--rw-r--r--   0 root         (0) root         (0)     8647 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html
--rw-r--r--   0 root         (0) root         (0)     2662 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.600550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/setting-list/
--rw-r--r--   0 root         (0) root         (0)     1496 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html
--rw-r--r--   0 root         (0) root         (0)     1119 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.600550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/task-list/
--rw-r--r--   0 root         (0) root         (0)     1022 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html
--rw-r--r--   0 root         (0) root         (0)     1210 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.600550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      544 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.601550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     5253 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py
--rw-r--r--   0 root         (0) root         (0)     1324 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)      813 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py
--rw-r--r--   0 root         (0) root         (0)      558 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py
--rw-r--r--   0 root         (0) root         (0)     8035 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py
--rw-r--r--   0 root         (0) root         (0)     1848 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1012 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py
--rw-r--r--   0 root         (0) root         (0)     5175 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py
--rw-r--r--   0 root         (0) root         (0)     1985 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py
--rw-r--r--   0 root         (0) root         (0)       96 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.601550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/client/
--rw-r--r--   0 root         (0) root         (0)      444 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/client/ClientFeTupleActionProcessorProxy.py
--rw-r--r--   0 root         (0) root         (0)      449 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/client/ClientFeTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)     1207 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/client/PluginClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.601550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.601550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/activity-list/
--rw-r--r--   0 root         (0) root         (0)     2074 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts
--rw-r--r--   0 root         (0) root         (0)      949 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html
--rw-r--r--   0 root         (0) root         (0)      637 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts
--rw-r--r--   0 root         (0) root         (0)      699 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1230 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.601550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/task-list/
--rw-r--r--   0 root         (0) root         (0)     2495 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts
--rw-r--r--   0 root         (0) root         (0)     2474 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.601550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-assets/
--rw-r--r--   0 root         (0) root         (0)    97846 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-assets/alert.mp3
--rw-r--r--   0 root         (0) root         (0)     1539 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.602550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/
--rw-r--r--   0 root         (0) root         (0)      566 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)      919 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)     8809 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/InboxApi.py
--rw-r--r--   0 root         (0) root         (0)     3792 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.602550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/backend/
--rw-r--r--   0 root         (0) root         (0)      976 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.602550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     2173 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/controller/AdminTestController.py
--rw-r--r--   0 root         (0) root         (0)    11069 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.602550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1079 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1663 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.603550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/
--rw-r--r--   0 root         (0) root         (0)     1747 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/Activity.py
--rw-r--r--   0 root         (0) root         (0)      446 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     7776 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)     4093 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/Task.py
--rw-r--r--   0 root         (0) root         (0)     1720 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/TaskAction.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.603550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      340 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/tuples/AdminSendTestActivityActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      331 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/tuples/AdminSendTestTaskActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      348 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.603550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/admin-doc/
--rw-r--r--   0 root         (0) root         (0)    86000 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/admin-doc/design_diagram.png
--rw-r--r--   0 root         (0) root         (0)     1653 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.603550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/both-doc/
--rw-r--r--   0 root         (0) root         (0)      234 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.603550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.604550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      180 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.604550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/notifiers/
--rw-r--r--   0 root         (0) root         (0)     2719 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/notifiers/notifier.interface.ts
--rw-r--r--   0 root         (0) root         (0)      845 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts
--rw-r--r--   0 root         (0) root         (0)     9870 2022-11-14 05:34:35.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts
--rw-r--r--   0 root         (0) root         (0)     5396 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.604550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      419 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestActivityActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      407 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestTaskActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      283 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)       66 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/package.json
--rw-r--r--   0 root         (0) root         (0)      379 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/plugin-inbox-names.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.605550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)      629 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts
--rw-r--r--   0 root         (0) root         (0)      395 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/tuples/TaskActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)     4717 2022-11-14 05:34:35.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1710 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.605550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/server/
--rw-r--r--   0 root         (0) root         (0)    13813 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/server/InboxApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.605550 peek-plugin-inbox-3.3.3/peek_plugin_inbox/tuples/
--rw-r--r--   0 root         (0) root         (0)     1079 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/tuples/ActivityTuple.py
--rw-r--r--   0 root         (0) root         (0)     1858 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/tuples/TaskTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2022-11-14 05:34:29.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:48.598550 peek-plugin-inbox-3.3.3/peek_plugin_inbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)      369 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6067 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/peek_plugin_inbox.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-14 05:37:48.606550 peek-plugin-inbox-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2655 2022-11-14 05:37:48.000000 peek-plugin-inbox-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.096196 peek-plugin-inbox-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-12 11:06:39.096196 peek-plugin-inbox-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      899 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.091196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/
+-rw-r--r--   0 root         (0) root         (0)      271 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/TempUnitTest.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-04-12 11:06:38.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.091196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/
+-rw-r--r--   0 root         (0) root         (0)      210 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.091196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.091196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/activity-list/
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.css
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html
+-rw-r--r--   0 root         (0) root         (0)      290 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.092196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-activity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.css
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.092196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-task/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.css
+-rw-r--r--   0 root         (0) root         (0)     8647 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.092196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/setting-list/
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.092196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/task-list/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.092196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      544 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.093196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     5253 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)      813 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py
+-rw-r--r--   0 root         (0) root         (0)     8035 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py
+-rw-r--r--   0 root         (0) root         (0)     5175 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.093196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/client/
+-rw-r--r--   0 root         (0) root         (0)      444 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/client/ClientFeTupleActionProcessorProxy.py
+-rw-r--r--   0 root         (0) root         (0)      449 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/client/ClientFeTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/client/PluginClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.093196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.093196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/activity-list/
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts
+-rw-r--r--   0 root         (0) root         (0)      949 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts
+-rw-r--r--   0 root         (0) root         (0)      699 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.093196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/task-list/
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.093196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-assets/
+-rw-r--r--   0 root         (0) root         (0)    97846 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-assets/alert.mp3
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.094196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)     8809 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/InboxApi.py
+-rw-r--r--   0 root         (0) root         (0)     3792 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.094196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/backend/
+-rw-r--r--   0 root         (0) root         (0)      976 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.094196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/controller/AdminTestController.py
+-rw-r--r--   0 root         (0) root         (0)    11069 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.094196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.094196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/Activity.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     7776 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/Task.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/TaskAction.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/tuples/AdminSendTestActivityActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/tuples/AdminSendTestTaskActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/admin-doc/
+-rw-r--r--   0 root         (0) root         (0)    86000 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/admin-doc/design_diagram.png
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/notifiers/
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/notifiers/notifier.interface.ts
+-rw-r--r--   0 root         (0) root         (0)      845 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts
+-rw-r--r--   0 root         (0) root         (0)    10414 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestActivityActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestTaskActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      283 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/package.json
+-rw-r--r--   0 root         (0) root         (0)      379 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/plugin-inbox-names.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.095196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/tuples/TaskActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-12 11:06:38.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.096196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/server/
+-rw-r--r--   0 root         (0) root         (0)    13813 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/server/InboxApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.096196 peek-plugin-inbox-3.4.0/peek_plugin_inbox/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/tuples/ActivityTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/tuples/TaskTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-12 11:03:21.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:06:39.091196 peek-plugin-inbox-3.4.0/peek_plugin_inbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-12 11:06:39.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-04-12 11:06:39.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:06:39.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:06:39.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 11:06:39.000000 peek-plugin-inbox-3.4.0/peek_plugin_inbox.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 11:06:39.097196 peek-plugin-inbox-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-12 11:06:38.000000 peek-plugin-inbox-3.4.0/setup.py
```

### Comparing `peek-plugin-inbox-3.3.3/README.rst` & `peek-plugin-inbox-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/__init__.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from peek_plugin_inbox._private.server.PluginLogicEntryHook import (
         PluginLogicEntryHook,
     )
```

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/script.py.mako` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/client/PluginClientEntryHook.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/client/PluginClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-assets/alert.mp3` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-assets/alert.mp3`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/InboxApi.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/InboxApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/controller/AdminTestController.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/controller/AdminTestController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/controller/MainController.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/Activity.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/Activity.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/Setting.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/Task.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/Task.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/_private/storage/TaskAction.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/_private/storage/TaskAction.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/admin-doc/design_diagram.png` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/admin-doc/design_diagram.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/admin-doc/index.rst` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/admin-doc/index.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts`

 * *Files 5% similar despite different names*

```diff
@@ -48,23 +48,22 @@
                 },
             ],
         });
     }
 
     async checkNotificationSettings(): Promise<void> {
         console.log("NATIVE NOTIFIER checking iOS permissions");
-        let permissionState: PermissionState =
-            await LocalNotifications.checkPermissions();
+        let permissionStatus = await LocalNotifications.checkPermissions();
 
-        if (permissionState === "prompt") {
-            permissionState = await LocalNotifications.requestPermission();
+        if (permissionStatus.display === "prompt") {
+            permissionStatus = await LocalNotifications.requestPermissions();
             return;
         }
 
-        if (permissionState === "denied") {
+        if (permissionStatus.display === "denied") {
             const confirmed = await Dialog.confirm({
                 title: "Notifications Required",
                 message:
                     "Peek requires notifications to be enabled.\n" +
                     "Would you like to enable them now?",
             });
```

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import { takeUntil } from "rxjs/operators";
 import { Injectable } from "@angular/core";
 import { NgLifeCycleEvents, TupleGenericAction } from "@synerty/vortexjs";
 import {
     BalloonMsgLevel,
     BalloonMsgService,
     BalloonMsgType,
+    BalloonMsgClickType,
     HeaderService,
 } from "@synerty/peek-plugin-base-js";
 import { TaskTuple } from "../tuples/TaskTuple";
 import { inboxPluginName } from "../plugin-inbox-names";
 import { PrivateInboxTupleProviderService } from "./private-inbox-tuple-provider.service";
 import { Capacitor } from "@capacitor/core";
 import { DeviceEnrolmentService } from "@peek/peek_core_device";
@@ -81,15 +82,16 @@
                 }
 
                 // Now we can set the tasks
                 this.tasks = tuples;
 
                 let notCompletedCount = 0;
                 for (let task of this.tasks) {
-                    notCompletedCount += task.isCompleted() ? 0 : 1;
+                    notCompletedCount +=
+                        task.isCompleted() || task.isSelected() ? 0 : 1;
                 }
 
                 this.headerService.updateBadgeCount(
                     inboxPluginName,
                     notCompletedCount
                 );
 
@@ -180,22 +182,30 @@
                     this.nativeNotifier.playSound();
                 } else {
                     this.webNotifier.playSound();
                 }
             }
 
             if (task.isNotifyByPopup() && !task.isNotifiedByPopup()) {
-                this.showMessage(BalloonMsgType.Fleeting, task);
+                this.showMessage(BalloonMsgType.Fleeting, task)
+                    .then((balloonMsgClickType: BalloonMsgClickType) => {
+                        this.sendStateUpdate(task, TaskTuple.STATE_SELECTED, 0);
+                    })
+                    .catch((err) => {
+                        const e = `Inbox Dialog Error\n${err}`;
+                        console.log(e);
+                        this.balloonMsg.showError(e);
+                    });
                 notificationSentFlags =
                     notificationSentFlags | TaskTuple.NOTIFY_BY_DEVICE_POPUP;
             }
 
             if (task.isNotifyByDialog() && !task.isNotifiedByDialog()) {
                 this.showMessage(BalloonMsgType.Confirm, task)
-                    .then(() => {
+                    .then((balloonMsgClickType: BalloonMsgClickType) => {
                         this.sendStateUpdate(
                             task,
                             TaskTuple.STATE_DIALOG_CONFIRMED,
                             0
                         );
                     })
                     .catch((err) => {
@@ -218,15 +228,18 @@
                 this.sendStateUpdate(task, newStateMask, notificationSentFlags);
             }
         }
 
         return updateApplied;
     }
 
-    private showMessage(type_: BalloonMsgType, task: TaskTuple): Promise<null> {
+    private showMessage(
+        type_: BalloonMsgType,
+        task: TaskTuple
+    ): Promise<BalloonMsgClickType> {
         let level: BalloonMsgLevel | null = null;
 
         switch (task.displayPriority) {
             case TaskTuple.PRIORITY_SUCCESS:
                 level = BalloonMsgLevel.Success;
                 break;
```

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         return !!(this.stateFlags & TaskTuple.STATE_ACTIONED);
     }
 
     isDelivered(): boolean {
         return !!(this.stateFlags & TaskTuple.STATE_DELIVERED);
     }
 
+    isSelected(): boolean {
+        return !!(this.stateFlags & TaskTuple.STATE_SELECTED);
+    }
+
     // ------------------------------
     // Notifications Required properties
     isNotifyBySound(): boolean {
         return !!(
             this.notificationRequiredFlags & TaskTuple.NOTIFY_BY_DEVICE_SOUND
         );
     }
```

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/plugin_package.json` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/plugin_package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960317460317462%*

 * *Differences: {"'plugin'": "{'version': '3.4.0'}"}*

```diff
@@ -42,15 +42,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_inbox",
         "title": "Inbox",
-        "version": "3.3.3",
+        "version": "3.4.0",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "field",
         "office",
         "storage",
```

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/server/InboxApiABC.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/server/InboxApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/tuples/ActivityTuple.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/tuples/ActivityTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox/tuples/TaskTuple.py` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox/tuples/TaskTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/peek_plugin_inbox.egg-info/SOURCES.txt` & `peek-plugin-inbox-3.4.0/peek_plugin_inbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.3.3/setup.py` & `peek-plugin-inbox-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_inbox"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin Inbox."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

