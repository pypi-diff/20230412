# Comparing `tmp/django-common-task-system-1.1.4.tar.gz` & `tmp/django-common-task-system-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.1.4.tar", last modified: Wed Apr 12 05:26:44 2023, max compression
+gzip compressed data, was "django-common-task-system-1.1.5.tar", last modified: Wed Apr 12 09:09:54 2023, max compression
```

## Comparing `django-common-task-system-1.1.4.tar` & `django-common-task-system-1.1.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.004207 django-common-task-system-1.1.4/django_common_task_system/
--rw-rw-rw-   0        0        0     2197 2023-04-07 08:17:44.000000 django-common-task-system-1.1.4/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0     6559 2023-04-06 08:09:40.000000 django-common-task-system-1.1.4/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.4/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0      937 2023-03-17 06:16:42.000000 django-common-task-system-1.1.4/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.4/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    12396 2023-03-20 05:05:30.000000 django-common-task-system-1.1.4/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.043607 django-common-task-system-1.1.4/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0    23088 2023-04-12 05:25:23.000000 django-common-task-system-1.1.4/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     2086 2023-03-22 05:08:57.000000 django-common-task-system-1.1.4/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:43.920401 django-common-task-system-1.1.4/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:43.921714 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.056653 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.089309 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.146962 django-common-task-system-1.1.4/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     4824 2023-04-11 06:00:14.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      506 2023-04-11 05:48:06.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     3717 2023-04-11 02:36:41.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.160496 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10626 2023-04-07 08:41:18.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    14418 2023-04-11 06:26:02.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1073 2023-04-07 05:56:05.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      800 2023-04-07 05:29:32.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     7503 2023-04-11 06:26:41.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.160496 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1504 2023-04-12 05:25:23.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.173815 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-04-11 05:57:33.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.206791 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      851 2023-04-04 06:16:44.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     2412 2023-04-11 05:50:53.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      834 2023-04-11 05:50:53.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1113 2023-04-11 05:50:53.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      325 2023-04-06 02:19:24.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:43.922766 django-common-task-system-1.1.4/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.256092 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.4/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      951 2023-04-06 03:57:39.000000 django-common-task-system-1.1.4/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.280446 django-common-task-system-1.1.4/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.4/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.4/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.4/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.4/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.4/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0     6535 2023-04-06 08:05:42.000000 django-common-task-system-1.1.4/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.023604 django-common-task-system-1.1.4/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3411 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-12 05:25:43.000000 django-common-task-system-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.487565 django-common-task-system-1.1.5/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-12 09:09:54.487565 django-common-task-system-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.222424 django-common-task-system-1.1.5/django_common_task_system/
+-rw-rw-rw-   0        0        0     2608 2023-04-12 09:03:52.000000 django-common-task-system-1.1.5/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0     6559 2023-04-06 08:09:40.000000 django-common-task-system-1.1.5/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.5/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0      937 2023-03-17 06:16:42.000000 django-common-task-system-1.1.5/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.5/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    12396 2023-03-20 05:05:30.000000 django-common-task-system-1.1.5/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.270538 django-common-task-system-1.1.5/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.5/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.5/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.5/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.5/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0    23088 2023-04-12 05:25:23.000000 django-common-task-system-1.1.5/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     2086 2023-03-22 05:08:57.000000 django-common-task-system-1.1.5/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.140846 django-common-task-system-1.1.5/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.140846 django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.282211 django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.319332 django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.363484 django-common-task-system-1.1.5/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     4761 2023-04-12 07:43:43.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      506 2023-04-11 05:48:06.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     3717 2023-04-11 02:36:41.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.378675 django-common-task-system-1.1.5/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10626 2023-04-07 08:41:18.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14418 2023-04-11 06:26:02.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1073 2023-04-07 05:56:05.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      800 2023-04-07 05:29:32.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     7503 2023-04-11 06:26:41.000000 django-common-task-system-1.1.5/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.380706 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1816 2023-04-12 09:07:42.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.382219 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-04-11 05:57:33.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.401980 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      851 2023-04-04 06:16:44.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     2412 2023-04-11 05:50:53.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      834 2023-04-11 05:50:53.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1113 2023-04-11 05:50:53.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.141994 django-common-task-system-1.1.5/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.458158 django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.5/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0      951 2023-04-06 03:57:39.000000 django-common-task-system-1.1.5/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.485571 django-common-task-system-1.1.5/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.5/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.5/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.5/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.5/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.5/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0     6535 2023-04-06 08:05:42.000000 django-common-task-system-1.1.5/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.243523 django-common-task-system-1.1.5/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-12 09:09:54.000000 django-common-task-system-1.1.5/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3411 2023-04-12 09:09:54.000000 django-common-task-system-1.1.5/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:09:54.000000 django-common-task-system-1.1.5/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-12 09:09:54.000000 django-common-task-system-1.1.5/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-12 09:09:54.000000 django-common-task-system-1.1.5/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:09:54.487565 django-common-task-system-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-12 08:17:59.000000 django-common-task-system-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:09:54.486573 django-common-task-system-1.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.5/tests/__init__.py
```

### Comparing `django-common-task-system-1.1.4/LICENSE` & `django-common-task-system-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/admin.py` & `django-common-task-system-1.1.5/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/choices.py` & `django-common-task-system-1.1.5/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/fields.py` & `django-common-task-system-1.1.5/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/forms.py` & `django-common-task-system-1.1.5/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.1.5/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.1.5/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/models.py` & `django-common-task-system-1.1.5/django_common_task_system/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/serializers.py` & `django-common-task-system-1.1.5/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.1.5/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 def init_system_process():
     logs_path = os.path.join(os.getcwd(), 'logs')
     if not os.path.exists(logs_path):
         os.mkdir(logs_path)
     models.SystemProcess.objects.all().delete()
     name = 'system-process-default'
     log_file = os.path.join(logs_path, f'{name}.log')
-    if os.path.isfile(log_file):
-        os.remove(log_file)
     instance = models.SystemProcess(
         process_name=name,
         log_file=log_file
     )
     process = ProcessManager.create(start_by_server, instance.log_file)
     instance.process_id = process.pid
     instance.save()
```

#### html2text {}

```diff
@@ -2,37 +2,36 @@
 django.shortcuts import reverse from django.utils.html import format_html from
 django.db.models.signals import post_delete from . import models from . import
 forms from .. import admin as base_admin from .process import ProcessManager
 from ..system_task_execution.main import start_by_server import os def
 init_system_process(): logs_path = os.path.join(os.getcwd(), 'logs') if not
 os.path.exists(logs_path): os.mkdir(logs_path) models.SystemProcess.objects.all
 ().delete() name = 'system-process-default' log_file = os.path.join(logs_path,
-f'{name}.log') if os.path.isfile(log_file): os.remove(log_file) instance =
-models.SystemProcess( process_name=name, log_file=log_file ) process =
-ProcessManager.create(start_by_server, instance.log_file) instance.process_id =
-process.pid instance.save() def init_system_data(): from .models import
-builtins builtins.initialize() if os.environ.get('RUN_MAIN') == 'true' and
-os.environ.get('RUN_CLIENT') != 'true': init_system_process() init_system_data
-() @receiver(post_delete, sender=models.SystemProcess) def delete_process
-(sender, instance: models.SystemProcess, **kwargs): ProcessManager.kill
-(instance.process_id) if os.path.isfile(instance.log_file): os.remove
-(instance.log_file) class SystemTaskAdmin(base_admin.TaskAdmin): form =
-forms.SystemTaskForm schedule_model = models.SystemSchedule list_display =
-('id', 'admin_parent', 'name', 'category', 'admin_status', 'schedules',
-'update_time') fields = ( ("parent", 'category',), ('queue',), ("name",
-"status",), "config", 'description', ) filter_horizontal = [] list_filter =
-('category', 'parent') def has_delete_permission(self, request, obj=None): if
-obj: return obj.category != models.builtins.tasks.system_default_category
-return True class SystemScheduleCallbackAdmin
-(base_admin.TaskScheduleCallbackAdmin): pass class SystemScheduleAdmin
-(base_admin.TaskScheduleAdmin): task_model = models.SystemTask
-schedule_log_model = models.SystemScheduleLog schedule_put_name =
-'system_schedule_queue_put' list_display = ('id', 'admin_task',
-'schedule_type', 'schedule_sub_type', 'next_schedule_time', 'status', 'put',
-'logs', 'update_time') list_filter = ('task__category', ) def
+f'{name}.log') instance = models.SystemProcess( process_name=name,
+log_file=log_file ) process = ProcessManager.create(start_by_server,
+instance.log_file) instance.process_id = process.pid instance.save() def
+init_system_data(): from .models import builtins builtins.initialize() if
+os.environ.get('RUN_MAIN') == 'true' and os.environ.get('RUN_CLIENT') !=
+'true': init_system_process() init_system_data() @receiver(post_delete,
+sender=models.SystemProcess) def delete_process(sender, instance:
+models.SystemProcess, **kwargs): ProcessManager.kill(instance.process_id) if
+os.path.isfile(instance.log_file): os.remove(instance.log_file) class
+SystemTaskAdmin(base_admin.TaskAdmin): form = forms.SystemTaskForm
+schedule_model = models.SystemSchedule list_display = ('id', 'admin_parent',
+'name', 'category', 'admin_status', 'schedules', 'update_time') fields = (
+("parent", 'category',), ('queue',), ("name", "status",), "config",
+'description', ) filter_horizontal = [] list_filter = ('category', 'parent')
+def has_delete_permission(self, request, obj=None): if obj: return obj.category
+!= models.builtins.tasks.system_default_category return True class
+SystemScheduleCallbackAdmin(base_admin.TaskScheduleCallbackAdmin): pass class
+SystemScheduleAdmin(base_admin.TaskScheduleAdmin): task_model =
+models.SystemTask schedule_log_model = models.SystemScheduleLog
+schedule_put_name = 'system_schedule_queue_put' list_display = ('id',
+'admin_task', 'schedule_type', 'schedule_sub_type', 'next_schedule_time',
+'status', 'put', 'logs', 'update_time') list_filter = ('task__category', ) def
 has_delete_permission(self, request, obj=None): if obj: return
 obj.task.category != models.builtins.tasks.system_default_category return True
 class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
 schedule_retry_name = 'system_schedule_retry' class SystemScheduleQueueAdmin
 (admin.ModelAdmin): list_display = ('id', 'name', 'code', 'queue_url',
 'module', 'update_time') fields = ( ('code', 'module', 'status'), 'name', ) def
 queue_url(self, obj): url = reverse('system_schedule_queue_get', args=
```

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/models.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/process.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task/views.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task_execution/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,32 +12,38 @@
 
     from .system_task_execution.executor import start_client
     from .system_task_execution import settings
     logger = settings.logger
     logger.handlers.clear()
     if not os.path.exists(os.path.dirname(log_file)):
         os.makedirs(os.path.dirname(log_file))
-
+    if os.path.isfile(log_file):
+        os.remove(log_file)
     handler = RotatingFileHandler(log_file, maxBytes=1024 * 1024 * 10, encoding='utf-8', backupCount=5)
     formatter = logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
 
+    for k, v in os.environ.items():
+        logger.info('Env: %s -> %s' % (k, v))
+
     start_client(**kwargs)
 
 
 if __name__ == '__main__':
     import django
     parser = argparse.ArgumentParser()
-    parser.add_argument('--system-path', type=str, required=True)
+    parser.add_argument('--system-path', type=str, required=False)
     parser.add_argument('--system-setting', type=str, required=False)
     shell_args = parser.parse_args()
-    sys.path.append(shell_args.system_path)
+    if shell_args.system_path:
+        assert os.path.exists(shell_args.system_path), 'system path not found'
+        sys.path.append(shell_args.system_path)
     env = shell_args.system_setting or os.environ.get('DJANGO_SETTINGS_MODULE')
     assert env, 'django settings module not found'
     os.environ.setdefault('DJANGO_SETTINGS_MODULE', env)
     os.environ['RUN_CLIENT'] = 'true'
     django.setup()
 
-    from system_task_execution.executor import start_client
+    from django_common_task_system.system_task_execution.system_task_execution.executor import start_client
     start_client()
```

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.1.5/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.1.5/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/urls.py` & `django-common-task-system-1.1.5/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.1.5/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.1.5/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.1.5/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system/views.py` & `django-common-task-system-1.1.5/django_common_task_system/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.1.5/django_common_task_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.4/setup.py` & `django-common-task-system-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.1.4',
+    version='1.1.5',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

