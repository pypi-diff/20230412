# Comparing `tmp/django-common-task-system-1.1.3.tar.gz` & `tmp/django-common-task-system-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.1.3.tar", last modified: Tue Apr 11 06:32:32 2023, max compression
+gzip compressed data, was "django-common-task-system-1.1.4.tar", last modified: Wed Apr 12 05:26:44 2023, max compression
```

## Comparing `django-common-task-system-1.1.3.tar` & `django-common-task-system-1.1.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.105694 django-common-task-system-1.1.3/django_common_task_system/
--rw-rw-rw-   0        0        0     2197 2023-04-07 08:17:44.000000 django-common-task-system-1.1.3/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0     6559 2023-04-06 08:09:40.000000 django-common-task-system-1.1.3/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.3/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0      937 2023-03-17 06:16:42.000000 django-common-task-system-1.1.3/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.3/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    12396 2023-03-20 05:05:30.000000 django-common-task-system-1.1.3/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.134439 django-common-task-system-1.1.3/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.3/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0    23017 2023-04-07 08:40:33.000000 django-common-task-system-1.1.3/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     2086 2023-03-22 05:08:57.000000 django-common-task-system-1.1.3/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.032055 django-common-task-system-1.1.3/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.033052 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.145617 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.173028 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.192031 django-common-task-system-1.1.3/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     4824 2023-04-11 06:00:14.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      506 2023-04-11 05:48:06.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     3717 2023-04-11 02:36:41.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.200622 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10626 2023-04-07 08:41:18.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    14418 2023-04-11 06:26:02.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1073 2023-04-07 05:56:05.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      800 2023-04-07 05:29:32.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     7503 2023-04-11 06:26:41.000000 django-common-task-system-1.1.3/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.202622 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1401 2023-04-07 08:04:08.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.205622 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-04-11 05:57:33.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.213622 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      851 2023-04-04 06:16:44.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     2412 2023-04-11 05:50:53.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      834 2023-04-11 05:50:53.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1113 2023-04-11 05:50:53.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      325 2023-04-06 02:19:24.000000 django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.034057 django-common-task-system-1.1.3/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.269538 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.3/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      951 2023-04-06 03:57:39.000000 django-common-task-system-1.1.3/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.288649 django-common-task-system-1.1.3/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.3/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.3/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.3/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.3/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.3/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0     6535 2023-04-06 08:05:42.000000 django-common-task-system-1.1.3/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.124438 django-common-task-system-1.1.3/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3411 2023-04-11 06:32:32.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-11 06:32:31.000000 django-common-task-system-1.1.3/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-07 09:00:10.000000 django-common-task-system-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:32:32.289649 django-common-task-system-1.1.3/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.004207 django-common-task-system-1.1.4/django_common_task_system/
+-rw-rw-rw-   0        0        0     2197 2023-04-07 08:17:44.000000 django-common-task-system-1.1.4/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0     6559 2023-04-06 08:09:40.000000 django-common-task-system-1.1.4/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.4/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0      937 2023-03-17 06:16:42.000000 django-common-task-system-1.1.4/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.4/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    12396 2023-03-20 05:05:30.000000 django-common-task-system-1.1.4/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.043607 django-common-task-system-1.1.4/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.4/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0    23088 2023-04-12 05:25:23.000000 django-common-task-system-1.1.4/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     2086 2023-03-22 05:08:57.000000 django-common-task-system-1.1.4/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:43.920401 django-common-task-system-1.1.4/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:43.921714 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.056653 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.089309 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.146962 django-common-task-system-1.1.4/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     4824 2023-04-11 06:00:14.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      506 2023-04-11 05:48:06.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     3717 2023-04-11 02:36:41.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.160496 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10626 2023-04-07 08:41:18.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14418 2023-04-11 06:26:02.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1073 2023-04-07 05:56:05.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      800 2023-04-07 05:29:32.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     7503 2023-04-11 06:26:41.000000 django-common-task-system-1.1.4/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.160496 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1504 2023-04-12 05:25:23.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.173815 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-04-11 05:57:33.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.206791 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      851 2023-04-04 06:16:44.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     2412 2023-04-11 05:50:53.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      834 2023-04-11 05:50:53.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1113 2023-04-11 05:50:53.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      325 2023-04-06 02:19:24.000000 django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:43.922766 django-common-task-system-1.1.4/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.256092 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.4/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0      951 2023-04-06 03:57:39.000000 django-common-task-system-1.1.4/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.280446 django-common-task-system-1.1.4/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.4/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.4/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.4/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.4/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.4/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0     6535 2023-04-06 08:05:42.000000 django-common-task-system-1.1.4/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.023604 django-common-task-system-1.1.4/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3411 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-12 05:26:43.000000 django-common-task-system-1.1.4/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-12 05:25:43.000000 django-common-task-system-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:26:44.281447 django-common-task-system-1.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.4/tests/__init__.py
```

### Comparing `django-common-task-system-1.1.3/LICENSE` & `django-common-task-system-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/__init__.py` & `django-common-task-system-1.1.4/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/admin.py` & `django-common-task-system-1.1.4/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/choices.py` & `django-common-task-system-1.1.4/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/fields.py` & `django-common-task-system-1.1.4/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/forms.py` & `django-common-task-system-1.1.4/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.1.4/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.1.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/models.py` & `django-common-task-system-1.1.4/django_common_task_system/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,14 +361,16 @@
                     elif day == 32:
                         day = mdays[last_time.month]
                     next_time = datetime(last_time.year, last_time.month, day, hour, minute, second)
                     if next_time > last_time:
                         break
                 else:
                     month = (last_time.month + timing_period) % 12
+                    if month == 0:
+                        month = 1
                     year = last_time.year + (last_time.month + timing_period) // 12
                     next_time = datetime(year, month, day, hour, minute, second)
             elif timing_type == ScheduleTimingType.YEAR:
                 month_days = timing_config['year']
                 if not month_days:
                     raise ValidationError("year month day is required while type is timing-datetime")
                 month, day = 1, 1
```

### Comparing `django-common-task-system-1.1.3/django_common_task_system/serializers.py` & `django-common-task-system-1.1.4/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.1.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/models.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/process.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task/views.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     import django
     django.setup()
 
     from .system_task_execution.executor import start_client
     from .system_task_execution import settings
     logger = settings.logger
     logger.handlers.clear()
+    if not os.path.exists(os.path.dirname(log_file)):
+        os.makedirs(os.path.dirname(log_file))
 
     handler = RotatingFileHandler(log_file, maxBytes=1024 * 1024 * 10, encoding='utf-8', backupCount=5)
     formatter = logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
```

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.1.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.1.4/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/urls.py` & `django-common-task-system-1.1.4/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.1.4/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.1.4/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.1.4/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system/views.py` & `django-common-task-system-1.1.4/django_common_task_system/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.1.4/django_common_task_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.3/setup.py` & `django-common-task-system-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.1.3',
+    version='1.1.4',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

