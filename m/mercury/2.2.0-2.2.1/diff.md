# Comparing `tmp/mercury-2.2.0.tar.gz` & `tmp/mercury-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-2.2.0.tar", last modified: Fri Apr  7 10:49:44 2023, max compression
+gzip compressed data, was "mercury-2.2.1.tar", last modified: Wed Apr 12 08:54:34 2023, max compression
```

## Comparing `mercury-2.2.0.tar` & `mercury-2.2.1.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.263627 mercury-2.2.0/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.2.0/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-07 10:49:44.263627 mercury-2.2.0/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4214 2023-02-15 10:26:45.000000 mercury-2.2.0/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-04-07 10:48:43.000000 mercury-2.2.0/mercury/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/accounts/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.0/mercury/apps/accounts/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.2.0/mercury/apps/accounts/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.2.0/mercury/apps/accounts/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.2.0/mercury/apps/accounts/fields.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/accounts/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/accounts/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.0/mercury/apps/accounts/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.2.0/mercury/apps/accounts/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.2.0/mercury/apps/accounts/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.2.0/mercury/apps/accounts/tasks.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/accounts/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.2.0/mercury/apps/accounts/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/accounts/tests/test_accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.2.0/mercury/apps/accounts/tests/test_invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/accounts/tests/test_secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.2.0/mercury/apps/accounts/tests/test_sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/accounts/tests/test_subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2650 2023-03-24 11:47:32.000000 mercury-2.2.0/mercury/apps/accounts/urls.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/accounts/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.2.0/mercury/apps/accounts/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.2.0/mercury/apps/accounts/views/accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.2.0/mercury/apps/accounts/views/invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.2.0/mercury/apps/accounts/views/permissions.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.2.0/mercury/apps/accounts/views/secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6372 2023-03-31 10:52:58.000000 mercury-2.2.0/mercury/apps/accounts/views/sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/accounts/views/subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.2.0/mercury/apps/accounts/views/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/nb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/nb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/nb/exporter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/nb/nbrun.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/nb/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.2.0/mercury/apps/nb/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/nb/tests/test_nbrun.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.2.0/mercury/apps/nb/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/nb/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/apps/nbworker/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/nbworker/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1719 2023-04-05 10:59:50.000000 mercury-2.2.0/mercury/apps/nbworker/__main__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17398 2023-04-06 14:49:56.000000 mercury-2.2.0/mercury/apps/nbworker/nb.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.2.0/mercury/apps/nbworker/rest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.2.0/mercury/apps/nbworker/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/nbworker/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2976 2023-03-31 09:54:03.000000 mercury-2.2.0/mercury/apps/nbworker/ws.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/notebooks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/notebooks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/notebooks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/notebooks/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/notebooks/management/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/notebooks/management/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/notebooks/management/commands/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/notebooks/management/commands/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.2.0/mercury/apps/notebooks/management/commands/add.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.2.0/mercury/apps/notebooks/management/commands/delete.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.2.0/mercury/apps/notebooks/management/commands/list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/notebooks/management/commands/watch.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/notebooks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/notebooks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/notebooks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.2.0/mercury/apps/notebooks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.2.0/mercury/apps/notebooks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.2.0/mercury/apps/notebooks/slides_themes.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11689 2023-04-03 14:44:43.000000 mercury-2.2.0/mercury/apps/notebooks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.2.0/mercury/apps/notebooks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      567 2023-03-17 12:41:34.000000 mercury-2.2.0/mercury/apps/notebooks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3755 2023-03-17 08:55:41.000000 mercury-2.2.0/mercury/apps/notebooks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/storage/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/storage/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/storage/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/storage/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/storage/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/storage/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.2.0/mercury/apps/storage/migrations/0002_useruploadedfile.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/storage/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/storage/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.2.0/mercury/apps/storage/s3utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.2.0/mercury/apps/storage/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-03-31 09:54:03.000000 mercury-2.2.0/mercury/apps/storage/storage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.2.0/mercury/apps/storage/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.2.0/mercury/apps/storage/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.2.0/mercury/apps/storage/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/storage/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.2.0/mercury/apps/storage/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.2.0/mercury/apps/storage/views/dashboardfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.2.0/mercury/apps/storage/views/notebookfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.2.0/mercury/apps/storage/views/workerfiles.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/tasks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/tasks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/tasks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/tasks/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.2.0/mercury/apps/tasks/clean_service.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3840 2023-04-03 14:18:32.000000 mercury-2.2.0/mercury/apps/tasks/export_pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/tasks/export_png.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/tasks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/tasks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/apps/tasks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.2.0/mercury/apps/tasks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/tasks/notify.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.2.0/mercury/apps/tasks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.2.0/mercury/apps/tasks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/tasks/tasks_export.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/tasks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1401 2023-03-17 12:41:34.000000 mercury-2.2.0/mercury/apps/tasks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8619 2023-03-17 08:55:41.000000 mercury-2.2.0/mercury/apps/tasks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/workers/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/workers/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/workers/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/workers/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/workers/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/workers/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/workers/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.2.0/mercury/apps/workers/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/workers/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/workers/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1053 2023-03-17 12:41:34.000000 mercury-2.2.0/mercury/apps/workers/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.2.0/mercury/apps/workers/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/ws/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/ws/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/ws/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/ws/client.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/ws/middleware.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.255627 mercury-2.2.0/mercury/apps/ws/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/apps/ws/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.2.0/mercury/apps/ws/routing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/ws/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.2.0/mercury/apps/ws/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.2.0/mercury/apps/ws/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/apps/ws/worker.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.2.0/mercury/demo.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.259627 mercury-2.2.0/mercury/frontend-dist/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/asset-manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/favicon-old.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/favicon.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/index.html
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/jupyter-additional.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/jupyter-syntax.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   580386 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/jupyter-theme-light.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/mercury_black_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/mercury_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-04-07 10:49:28.000000 mercury-2.2.0/mercury/frontend-dist/robots.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury/frontend-dist/static/
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.259627 mercury-2.2.0/mercury/frontend-dist/static/css/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2831 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/css/main.26f96620.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5260 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.263627 mercury-2.2.0/mercury/frontend-dist/static/js/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/js/2.20950ecb.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  4973512 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    83606 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/js/main.717ee96a.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   258957 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/js/main.717ee96a.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.263627 mercury-2.2.0/mercury/frontend-dist/static/media/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-04-07 10:49:43.000000 mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/manage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8376 2023-04-07 10:38:38.000000 mercury-2.2.0/mercury/mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      543 2023-03-30 08:36:26.000000 mercury-2.2.0/mercury/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.263627 mercury-2.2.0/mercury/server/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.2.0/mercury/server/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/server/asgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.2.0/mercury/server/celery.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.2.0/mercury/server/settings.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1572 2023-03-14 07:49:44.000000 mercury-2.2.0/mercury/server/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.2.0/mercury/server/views.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.2.0/mercury/server/wsgi.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.263627 mercury-2.2.0/mercury/widgets/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.0/mercury/widgets/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-03-17 11:39:55.000000 mercury-2.2.0/mercury/widgets/app.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/button.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.2.0/mercury/widgets/chat.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2127 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/checkbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.2.0/mercury/widgets/confetti.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/file.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.2.0/mercury/widgets/json.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/manager.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.2.0/mercury/widgets/md.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2690 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/multiselect.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.2.0/mercury/widgets/note.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3016 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/numeric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.2.0/mercury/widgets/outputdir.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3025 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/range.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2403 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/select.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/slider.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.2.0/mercury/widgets/stop.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2039 2023-04-07 10:30:37.000000 mercury-2.2.0/mercury/widgets/text.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-07 10:49:44.251627 mercury-2.2.0/mercury.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-07 10:49:44.000000 mercury-2.2.0/mercury.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6285 2023-04-07 10:49:44.000000 mercury-2.2.0/mercury.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-04-07 10:49:44.000000 mercury-2.2.0/mercury.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-04-07 10:49:44.000000 mercury-2.2.0/mercury.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      491 2023-04-07 10:49:44.000000 mercury-2.2.0/mercury.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-04-07 10:49:44.000000 mercury-2.2.0/mercury.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.2.0/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-04-07 10:49:44.263627 mercury-2.2.0/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1163 2023-04-07 10:49:15.000000 mercury-2.2.0/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.2.1/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-12 08:54:34.924365 mercury-2.2.1/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4214 2023-02-15 10:26:45.000000 mercury-2.2.1/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-04-12 08:53:52.000000 mercury-2.2.1/mercury/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.2.1/mercury/apps/accounts/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/fields.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.2.1/mercury/apps/accounts/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.2.1/mercury/apps/accounts/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.2.1/mercury/apps/accounts/tasks.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.2.1/mercury/apps/accounts/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2650 2023-03-24 11:47:32.000000 mercury-2.2.1/mercury/apps/accounts/urls.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.2.1/mercury/apps/accounts/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.2.1/mercury/apps/accounts/views/accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.2.1/mercury/apps/accounts/views/invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.2.1/mercury/apps/accounts/views/permissions.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.2.1/mercury/apps/accounts/views/secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6372 2023-03-31 10:52:58.000000 mercury-2.2.1/mercury/apps/accounts/views/sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/views/subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.2.1/mercury/apps/accounts/views/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/nb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/nb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/nb/exporter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/nb/nbrun.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/nb/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.2.1/mercury/apps/nb/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/nb/tests/test_nbrun.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/nb/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/nb/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/nbworker/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/nbworker/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1719 2023-04-05 10:59:50.000000 mercury-2.2.1/mercury/apps/nbworker/__main__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.2.1/mercury/apps/nbworker/nb.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.2.1/mercury/apps/nbworker/rest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/nbworker/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/nbworker/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2976 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/nbworker/ws.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/management/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/management/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/management/commands/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/add.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/delete.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/watch.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/notebooks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.2.1/mercury/apps/notebooks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.2.1/mercury/apps/notebooks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.2.1/mercury/apps/notebooks/slides_themes.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11689 2023-04-03 14:44:43.000000 mercury-2.2.1/mercury/apps/notebooks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/notebooks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      567 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/notebooks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3755 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/notebooks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/storage/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/storage/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/storage/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/migrations/0002_useruploadedfile.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/storage/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/s3utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.2.1/mercury/apps/storage/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/storage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/storage/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.2.1/mercury/apps/storage/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/storage/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.2.1/mercury/apps/storage/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.2.1/mercury/apps/storage/views/dashboardfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.2.1/mercury/apps/storage/views/notebookfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.2.1/mercury/apps/storage/views/workerfiles.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/tasks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/tasks/clean_service.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3840 2023-04-03 14:18:32.000000 mercury-2.2.1/mercury/apps/tasks/export_pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/tasks/export_png.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/tasks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.2.1/mercury/apps/tasks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/tasks/notify.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/tasks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.2.1/mercury/apps/tasks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/tasks/tasks_export.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/tasks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1401 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/tasks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8619 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/tasks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/workers/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/workers/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/workers/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/workers/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1053 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/workers/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/workers/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/ws/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/ws/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/ws/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/ws/client.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/ws/middleware.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/ws/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/ws/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.2.1/mercury/apps/ws/routing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/ws/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.2.1/mercury/apps/ws/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/ws/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/ws/worker.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.2.1/mercury/demo.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.920365 mercury-2.2.1/mercury/frontend-dist/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/asset-manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/favicon-old.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/favicon.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/index.html
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/jupyter-additional.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/jupyter-syntax.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   580386 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/jupyter-theme-light.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/mercury_black_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/mercury_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/robots.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/frontend-dist/static/
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.920365 mercury-2.2.1/mercury/frontend-dist/static/css/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2831 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5260 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/frontend-dist/static/js/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  4973512 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    83606 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   258957 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/frontend-dist/static/media/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/manage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8376 2023-04-07 10:38:38.000000 mercury-2.2.1/mercury/mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      543 2023-03-30 08:36:26.000000 mercury-2.2.1/mercury/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/server/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/server/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/server/asgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.2.1/mercury/server/celery.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.2.1/mercury/server/settings.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1572 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/server/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.2.1/mercury/server/views.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.2.1/mercury/server/wsgi.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/widgets/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/widgets/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-03-17 11:39:55.000000 mercury-2.2.1/mercury/widgets/app.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/button.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.2.1/mercury/widgets/chat.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2127 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/checkbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.2.1/mercury/widgets/confetti.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/file.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.2.1/mercury/widgets/json.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/manager.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.2.1/mercury/widgets/md.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2690 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/multiselect.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.2.1/mercury/widgets/note.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3016 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/numeric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.2.1/mercury/widgets/outputdir.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3025 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/range.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2403 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/select.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/slider.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.2.1/mercury/widgets/stop.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2039 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/text.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6285 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      491 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.2.1/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-04-12 08:54:34.924365 mercury-2.2.1/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1163 2023-04-12 08:54:01.000000 mercury-2.2.1/setup.py
```

### Comparing `mercury-2.2.0/PKG-INFO` & `mercury-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.2.0
+Version: 2.2.1
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 License: UNKNOWN
 Description:
```

### Comparing `mercury-2.2.0/README.md` & `mercury-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/fields.py` & `mercury-2.2.1/mercury/apps/accounts/fields.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/migrations/0001_initial.py` & `mercury-2.2.1/mercury/apps/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/models.py` & `mercury-2.2.1/mercury/apps/accounts/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/serializers.py` & `mercury-2.2.1/mercury/apps/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/tasks.py` & `mercury-2.2.1/mercury/apps/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/tests/test_accounts.py` & `mercury-2.2.1/mercury/apps/accounts/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/tests/test_invitations.py` & `mercury-2.2.1/mercury/apps/accounts/tests/test_invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/tests/test_secrets.py` & `mercury-2.2.1/mercury/apps/accounts/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/tests/test_sites.py` & `mercury-2.2.1/mercury/apps/accounts/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/tests/test_subscription.py` & `mercury-2.2.1/mercury/apps/accounts/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/urls.py` & `mercury-2.2.1/mercury/apps/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/views/accounts.py` & `mercury-2.2.1/mercury/apps/accounts/views/accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/views/invitations.py` & `mercury-2.2.1/mercury/apps/accounts/views/invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/views/permissions.py` & `mercury-2.2.1/mercury/apps/accounts/views/permissions.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/views/secrets.py` & `mercury-2.2.1/mercury/apps/accounts/views/secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/views/sites.py` & `mercury-2.2.1/mercury/apps/accounts/views/sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/accounts/views/subscription.py` & `mercury-2.2.1/mercury/apps/accounts/views/subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nb/exporter.py` & `mercury-2.2.1/mercury/apps/nb/exporter.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nb/nbrun.py` & `mercury-2.2.1/mercury/apps/nb/nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nb/tests/test_nbrun.py` & `mercury-2.2.1/mercury/apps/nb/tests/test_nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nb/tests.py` & `mercury-2.2.1/mercury/apps/nb/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nbworker/__main__.py` & `mercury-2.2.1/mercury/apps/nbworker/__main__.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nbworker/nb.py` & `mercury-2.2.1/mercury/apps/nbworker/nb.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         self.ws.send(json.dumps({"purpose": Purpose.ExecutedNotebook, "body": body}))
         self.update_worker_state(WorkerState.Running)
         self.prev_body = copy.deepcopy(body)
 
     def update_nb(self, widgets):
         log.debug(f"Update nb {widgets}")
 
-        index_execute_from = 1
+        index_execute_from = None
         # fill notebook with widgets values
         self.prev_widgets = copy.deepcopy(widgets)
         for widget_key in widgets.keys():
             value = widgets[widget_key]
 
             widget_type = WidgetsManager.parse_widget_type(widget_key)
             log.debug(
@@ -187,20 +187,20 @@
             updated = "True" in str(r)
             log.debug(f"Update reponse {r}, updated={updated}")
 
             if updated:
                 cell_index = WidgetsManager.parse_cell_index(widget_key)
                 log.debug(f"Widget updated, update nb from {cell_index}")
 
-                if index_execute_from == 1:
+                if index_execute_from is None:
                     index_execute_from = cell_index
                 else:
                     index_execute_from = min(index_execute_from, cell_index)
 
-        if index_execute_from != 1:
+        if index_execute_from is not None:
             if self.prev_nb is not None:
                 self.nb = copy.deepcopy(self.prev_nb)
             else:
                 self.nb = copy.deepcopy(self.nb_original)
 
             self.nbrun.run_notebook(self.nb, start=index_execute_from - 1)
```

### Comparing `mercury-2.2.0/mercury/apps/nbworker/rest.py` & `mercury-2.2.1/mercury/apps/nbworker/rest.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nbworker/tests.py` & `mercury-2.2.1/mercury/apps/nbworker/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nbworker/utils.py` & `mercury-2.2.1/mercury/apps/nbworker/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/nbworker/ws.py` & `mercury-2.2.1/mercury/apps/nbworker/ws.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/management/commands/add.py` & `mercury-2.2.1/mercury/apps/notebooks/management/commands/add.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/management/commands/delete.py` & `mercury-2.2.1/mercury/apps/notebooks/management/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/management/commands/list.py` & `mercury-2.2.1/mercury/apps/notebooks/management/commands/list.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/management/commands/watch.py` & `mercury-2.2.1/mercury/apps/notebooks/management/commands/watch.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/migrations/0001_initial.py` & `mercury-2.2.1/mercury/apps/notebooks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/models.py` & `mercury-2.2.1/mercury/apps/notebooks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/serializers.py` & `mercury-2.2.1/mercury/apps/notebooks/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/slides_themes.py` & `mercury-2.2.1/mercury/apps/notebooks/slides_themes.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/tasks.py` & `mercury-2.2.1/mercury/apps/notebooks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/urls.py` & `mercury-2.2.1/mercury/apps/notebooks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/notebooks/views.py` & `mercury-2.2.1/mercury/apps/notebooks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/migrations/0001_initial.py` & `mercury-2.2.1/mercury/apps/storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/migrations/0002_useruploadedfile.py` & `mercury-2.2.1/mercury/apps/storage/migrations/0002_useruploadedfile.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/models.py` & `mercury-2.2.1/mercury/apps/storage/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/s3utils.py` & `mercury-2.2.1/mercury/apps/storage/s3utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/storage.py` & `mercury-2.2.1/mercury/apps/storage/storage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/tests.py` & `mercury-2.2.1/mercury/apps/storage/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/urls.py` & `mercury-2.2.1/mercury/apps/storage/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/views/dashboardfiles.py` & `mercury-2.2.1/mercury/apps/storage/views/dashboardfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/views/notebookfiles.py` & `mercury-2.2.1/mercury/apps/storage/views/notebookfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/storage/views/workerfiles.py` & `mercury-2.2.1/mercury/apps/storage/views/workerfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/export_pdf.py` & `mercury-2.2.1/mercury/apps/tasks/export_pdf.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/export_png.py` & `mercury-2.2.1/mercury/apps/tasks/export_png.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/migrations/0001_initial.py` & `mercury-2.2.1/mercury/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/models.py` & `mercury-2.2.1/mercury/apps/tasks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/notify.py` & `mercury-2.2.1/mercury/apps/tasks/notify.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/tasks.py` & `mercury-2.2.1/mercury/apps/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/tasks_export.py` & `mercury-2.2.1/mercury/apps/tasks/tasks_export.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/tests.py` & `mercury-2.2.1/mercury/apps/tasks/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/urls.py` & `mercury-2.2.1/mercury/apps/tasks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/tasks/views.py` & `mercury-2.2.1/mercury/apps/tasks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/workers/migrations/0001_initial.py` & `mercury-2.2.1/mercury/apps/workers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/workers/models.py` & `mercury-2.2.1/mercury/apps/workers/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/workers/urls.py` & `mercury-2.2.1/mercury/apps/workers/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/workers/views.py` & `mercury-2.2.1/mercury/apps/workers/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/ws/client.py` & `mercury-2.2.1/mercury/apps/ws/client.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/ws/middleware.py` & `mercury-2.2.1/mercury/apps/ws/middleware.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/ws/tasks.py` & `mercury-2.2.1/mercury/apps/ws/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/ws/utils.py` & `mercury-2.2.1/mercury/apps/ws/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/apps/ws/worker.py` & `mercury-2.2.1/mercury/apps/ws/worker.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/demo.py` & `mercury-2.2.1/mercury/demo.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/asset-manifest.json` & `mercury-2.2.1/mercury/frontend-dist/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/favicon-old.ico` & `mercury-2.2.1/mercury/frontend-dist/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/favicon.ico` & `mercury-2.2.1/mercury/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/index.html` & `mercury-2.2.1/mercury/frontend-dist/index.html`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/jupyter-additional.css` & `mercury-2.2.1/mercury/frontend-dist/jupyter-additional.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/jupyter-syntax.css` & `mercury-2.2.1/mercury/frontend-dist/jupyter-syntax.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/jupyter-theme-light.css` & `mercury-2.2.1/mercury/frontend-dist/jupyter-theme-light.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/mercury_black_logo.svg` & `mercury-2.2.1/mercury/frontend-dist/mercury_black_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/mercury_logo.svg` & `mercury-2.2.1/mercury/frontend-dist/mercury_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css` & `mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map` & `mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/css/main.26f96620.chunk.css` & `mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map` & `mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/js/2.20950ecb.chunk.js` & `mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.LICENSE.txt` & `mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.map` & `mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/js/main.717ee96a.chunk.js` & `mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/js/main.717ee96a.chunk.js.map` & `mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js` & `mercury-2.2.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map` & `mercury-2.2.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf` & `mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2` & `mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot` & `mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg` & `mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff` & `mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/manage.py` & `mercury-2.2.1/mercury/manage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/mercury.py` & `mercury-2.2.1/mercury/mercury.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/requirements.txt` & `mercury-2.2.1/mercury/requirements.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/server/asgi.py` & `mercury-2.2.1/mercury/server/asgi.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/server/celery.py` & `mercury-2.2.1/mercury/server/celery.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/server/settings.py` & `mercury-2.2.1/mercury/server/settings.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/server/urls.py` & `mercury-2.2.1/mercury/server/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/server/views.py` & `mercury-2.2.1/mercury/server/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/app.py` & `mercury-2.2.1/mercury/widgets/app.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/button.py` & `mercury-2.2.1/mercury/widgets/button.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/chat.py` & `mercury-2.2.1/mercury/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/checkbox.py` & `mercury-2.2.1/mercury/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/file.py` & `mercury-2.2.1/mercury/widgets/file.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/json.py` & `mercury-2.2.1/mercury/widgets/json.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/manager.py` & `mercury-2.2.1/mercury/widgets/manager.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/multiselect.py` & `mercury-2.2.1/mercury/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/note.py` & `mercury-2.2.1/mercury/widgets/note.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/numeric.py` & `mercury-2.2.1/mercury/widgets/numeric.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/outputdir.py` & `mercury-2.2.1/mercury/widgets/outputdir.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/range.py` & `mercury-2.2.1/mercury/widgets/range.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/select.py` & `mercury-2.2.1/mercury/widgets/select.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/slider.py` & `mercury-2.2.1/mercury/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury/widgets/text.py` & `mercury-2.2.1/mercury/widgets/text.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/mercury.egg-info/PKG-INFO` & `mercury-2.2.1/mercury.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.2.0
+Version: 2.2.1
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 License: UNKNOWN
 Description:
```

### Comparing `mercury-2.2.0/mercury.egg-info/SOURCES.txt` & `mercury-2.2.1/mercury.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.2.0/setup.py` & `mercury-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join(path, filename))
     return paths
 
 setup(
     name="mercury",
-    version="2.2.0",
+    version="2.2.1",
     maintainer="MLJAR Sp. z o.o.",
     maintainer_email="contact@mljar.com",
     description="Turn Jupyter Notebook to Web App and share with non-technical users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=open("mercury/requirements.txt").readlines(),
     url="https://github.com/mljar/mercury",
```

