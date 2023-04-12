# Comparing `tmp/django-dkron-1.1.0.tar.gz` & `tmp/django-dkron-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dkron-1.1.0.tar", last modified: Thu Mar 23 17:34:33 2023, max compression
+gzip compressed data, was "django-dkron-1.1.1.tar", last modified: Wed Apr 12 07:56:42 2023, max compression
```

## Comparing `django-dkron-1.1.0.tar` & `django-dkron-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.979355 django-dkron-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-23 17:34:05.000000 django-dkron-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-23 17:34:05.000000 django-dkron-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-03-23 17:34:33.979355 django-dkron-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-03-23 17:34:05.000000 django-dkron-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.975355 django-dkron-1.1.0/django_dkron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-03-23 17:34:33.000000 django-dkron-1.1.0/django_dkron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-23 17:34:33.000000 django-dkron-1.1.0/django_dkron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:34:33.000000 django-dkron-1.1.0/django_dkron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:34:33.000000 django-dkron-1.1.0/django_dkron.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-23 17:34:33.000000 django-dkron-1.1.0/django_dkron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-23 17:34:33.000000 django-dkron-1.1.0/django_dkron.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.975355 django-dkron-1.1.0/dkron/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.975355 django-dkron-1.1.0/dkron/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.979355 django-dkron-1.1.0/dkron/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/management/commands/cleanup_dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/management/commands/resync_dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/management/commands/run_dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/management/commands/run_dkron_async_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.979355 django-dkron-1.1.0/dkron/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/migrations/0001_initial_20210729.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/migrations/0002_job_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.971355 django-dkron-1.1.0/dkron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.971355 django-dkron-1.1.0/dkron/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.971355 django-dkron-1.1.0/dkron/templates/admin/dkron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.979355 django-dkron-1.1.0/dkron/templates/admin/dkron/job/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/templates/admin/dkron/job/change_list_object_tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:33.979355 django-dkron-1.1.0/dkron/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/templatetags/dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/urls_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-03-23 17:34:05.000000 django-dkron-1.1.0/dkron/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-23 17:34:33.979355 django-dkron-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 17:34:05.000000 django-dkron-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.615077 django-dkron-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 07:56:31.000000 django-dkron-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 07:56:31.000000 django-dkron-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-12 07:56:42.615077 django-dkron-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-12 07:56:31.000000 django-dkron-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.611077 django-dkron-1.1.1/django_dkron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-12 07:56:42.000000 django-dkron-1.1.1/django_dkron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-12 07:56:42.000000 django-dkron-1.1.1/django_dkron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:56:42.000000 django-dkron-1.1.1/django_dkron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:56:42.000000 django-dkron-1.1.1/django_dkron.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 07:56:42.000000 django-dkron-1.1.1/django_dkron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 07:56:42.000000 django-dkron-1.1.1/django_dkron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.611077 django-dkron-1.1.1/dkron/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.611077 django-dkron-1.1.1/dkron/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.611077 django-dkron-1.1.1/dkron/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/management/commands/cleanup_dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/management/commands/resync_dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/management/commands/run_dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/management/commands/run_dkron_async_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.611077 django-dkron-1.1.1/dkron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/migrations/0001_initial_20210729.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/migrations/0002_job_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/migrations/0003_alter_job_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.607077 django-dkron-1.1.1/dkron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.607077 django-dkron-1.1.1/dkron/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.607077 django-dkron-1.1.1/dkron/templates/admin/dkron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.611077 django-dkron-1.1.1/dkron/templates/admin/dkron/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/templates/admin/dkron/job/change_list_object_tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:42.615077 django-dkron-1.1.1/dkron/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/templatetags/dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/urls_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-12 07:56:31.000000 django-dkron-1.1.1/dkron/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-12 07:56:42.615077 django-dkron-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:56:31.000000 django-dkron-1.1.1/setup.py
```

### Comparing `django-dkron-1.1.0/LICENSE` & `django-dkron-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/PKG-INFO` & `django-dkron-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dkron
-Version: 1.1.0
+Version: 1.1.1
 Summary: Manage and run jobs in Dkron from your django project
 Home-page: https://github.com/surface-security/django-dkron
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-dkron-1.1.0/README.md` & `django-dkron-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/django_dkron.egg-info/PKG-INFO` & `django-dkron-1.1.1/django_dkron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dkron
-Version: 1.1.0
+Version: 1.1.1
 Summary: Manage and run jobs in Dkron from your django project
 Home-page: https://github.com/surface-security/django-dkron
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-dkron-1.1.0/django_dkron.egg-info/SOURCES.txt` & `django-dkron-1.1.1/django_dkron.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 dkron/management/commands/__init__.py
 dkron/management/commands/cleanup_dkron.py
 dkron/management/commands/resync_dkron.py
 dkron/management/commands/run_dkron.py
 dkron/management/commands/run_dkron_async_command.py
 dkron/migrations/0001_initial_20210729.py
 dkron/migrations/0002_job_retries.py
+dkron/migrations/0003_alter_job_schedule.py
 dkron/migrations/__init__.py
 dkron/templates/admin/dkron/job/change_list_object_tools.html
 dkron/templatetags/__init__.py
 dkron/templatetags/dkron.py
```

### Comparing `django-dkron-1.1.0/dkron/admin.py` & `django-dkron-1.1.1/dkron/admin.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/apps.py` & `django-dkron-1.1.1/dkron/apps.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/management/commands/cleanup_dkron.py` & `django-dkron-1.1.1/dkron/management/commands/cleanup_dkron.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/management/commands/resync_dkron.py` & `django-dkron-1.1.1/dkron/management/commands/resync_dkron.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/management/commands/run_dkron.py` & `django-dkron-1.1.1/dkron/management/commands/run_dkron.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/management/commands/run_dkron_async_command.py` & `django-dkron-1.1.1/dkron/management/commands/run_dkron_async_command.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/migrations/0001_initial_20210729.py` & `django-dkron-1.1.1/dkron/migrations/0001_initial_20210729.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/models.py` & `django-dkron-1.1.1/dkron/models.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/templates/admin/dkron/job/change_list_object_tools.html` & `django-dkron-1.1.1/dkron/templates/admin/dkron/job/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/utils.py` & `django-dkron-1.1.1/dkron/utils.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/dkron/views.py` & `django-dkron-1.1.1/dkron/views.py`

 * *Files identical despite different names*

### Comparing `django-dkron-1.1.0/setup.cfg` & `django-dkron-1.1.1/setup.cfg`

 * *Files identical despite different names*

