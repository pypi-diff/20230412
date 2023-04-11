# Comparing `tmp/zibanu-django-1.2.0a4.tar.gz` & `tmp/zibanu-django-1.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.2.0a4.tar", last modified: Sun Apr  9 00:12:54 2023, max compression
+gzip compressed data, was "zibanu-django-1.2.0a5.tar", last modified: Tue Apr 11 22:56:50 2023, max compression
```

## Comparing `zibanu-django-1.2.0a4.tar` & `zibanu-django-1.2.0a5.tar`

### file list

```diff
@@ -1,131 +1,139 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.433503 zibanu-django-1.2.0a4/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0a4/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      207 2023-03-31 15:51:33.000000 zibanu-django-1.2.0a4/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-09 00:12:54.433503 zibanu-django-1.2.0a4/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      158 2023-01-18 12:15:22.000000 zibanu-django-1.2.0a4/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      849 2023-04-09 00:11:04.000000 zibanu-django-1.2.0a4/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-04-09 00:12:54.433503 zibanu-django-1.2.0a4/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.417503 zibanu-django-1.2.0a4/zibanu/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0a4/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.417503 zibanu-django-1.2.0a4/zibanu/django/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0a4/zibanu/django/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.418503 zibanu-django-1.2.0a4/zibanu/django/auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-1.2.0a4/zibanu/django/auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.418503 zibanu-django-1.2.0a4/zibanu/django/auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-1.2.0a4/zibanu/django/auth/api/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3471 2023-04-09 00:10:08.000000 zibanu-django-1.2.0a4/zibanu/django/auth/api/serializers.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-04-08 23:45:31.000000 zibanu-django-1.2.0a4/zibanu/django/auth/apps.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      637 2023-04-08 12:38:36.000000 zibanu-django-1.2.0a4/zibanu/django/auth/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.418503 zibanu-django-1.2.0a4/zibanu/django/db/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0a4/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.419504 zibanu-django-1.2.0a4/zibanu/django/db/backends/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a4/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.419504 zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.420503 zibanu-django-1.2.0a4/zibanu/django/db/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/dated_model.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/manager.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0a4/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.420503 zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3609 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.420503 zibanu-django-1.2.0a4/zibanu/django/logging/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0a4/zibanu/django/logging/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.421503 zibanu-django-1.2.0a4/zibanu/django/logging/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.421503 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_change_password.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_login.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_send_mail.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.421503 zibanu-django-1.2.0a4/zibanu/django/logging/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      453 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/logging/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.414504 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.422503 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.422503 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0002_maillog.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0a4/zibanu/django/logging/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/logging/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0a4/zibanu/django/repository/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0a4/zibanu/django/repository/api/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0a4/zibanu/django/repository/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.423503 zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/document.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.424503 zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6973 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/document_generator.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.415504 zibanu-django-1.2.0a4/zibanu/django/repository/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.415504 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.424503 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/0002_document_description.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0a4/zibanu/django/repository/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0a4/zibanu/django/repository/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1967 2022-12-14 09:17:28.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/api_exception.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.425503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/current_user_default.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.426503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/fields.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/model_serializer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.426503 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    10439 2023-03-31 16:50:03.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.427503 zibanu-django-1.2.0a4/zibanu/django/template/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0a4/zibanu/django/template/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0a4/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.427503 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/full_static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0a4/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.416504 zibanu-django-1.2.0a4/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.416504 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.427503 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.428503 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/string_concat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/subtotal_dict.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0a4/zibanu/django/template/templatetags/sum_dict.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.432503 zibanu-django-1.2.0a4/zibanu/django/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3059 2023-03-14 20:09:11.000000 zibanu-django-1.2.0a4/zibanu/django/utils/code_generator.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0a4/zibanu/django/utils/date_time.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a4/zibanu/django/utils/error_messages.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4325 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/utils/mail.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a4/zibanu/django/utils/request_utils.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1251 2022-12-14 09:24:38.000000 zibanu-django-1.2.0a4/zibanu/django/utils/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a4/zibanu/django/utils/validate_cache_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-09 00:12:54.432503 zibanu-django-1.2.0a4/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3621 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       32 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-04-09 00:12:54.000000 zibanu-django-1.2.0a4/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.692224 zibanu-django-1.2.0a5/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0a5/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      207 2023-03-31 15:51:33.000000 zibanu-django-1.2.0a5/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-11 22:56:50.692224 zibanu-django-1.2.0a5/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      158 2023-01-18 12:15:22.000000 zibanu-django-1.2.0a5/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      849 2023-04-11 22:55:00.000000 zibanu-django-1.2.0a5/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-04-11 22:56:50.692224 zibanu-django-1.2.0a5/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.674224 zibanu-django-1.2.0a5/zibanu/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0a5/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.675224 zibanu-django-1.2.0a5/zibanu/django/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0a5/zibanu/django/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.675224 zibanu-django-1.2.0a5/zibanu/django/auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-1.2.0a5/zibanu/django/auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.676224 zibanu-django-1.2.0a5/zibanu/django/auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-1.2.0a5/zibanu/django/auth/api/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3848 2023-04-11 22:46:44.000000 zibanu-django-1.2.0a5/zibanu/django/auth/api/serializers.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      915 2023-04-10 18:51:33.000000 zibanu-django-1.2.0a5/zibanu/django/auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.676224 zibanu-django-1.2.0a5/zibanu/django/auth/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-1.2.0a5/zibanu/django/auth/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.676224 zibanu-django-1.2.0a5/zibanu/django/auth/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-1.2.0a5/zibanu/django/auth/lib/choices/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.677224 zibanu-django-1.2.0a5/zibanu/django/auth/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-1.2.0a5/zibanu/django/auth/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-1.2.0a5/zibanu/django/auth/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-04-11 22:39:53.000000 zibanu-django-1.2.0a5/zibanu/django/auth/models.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      637 2023-04-08 12:38:36.000000 zibanu-django-1.2.0a5/zibanu/django/auth/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.677224 zibanu-django-1.2.0a5/zibanu/django/db/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0a5/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.677224 zibanu-django-1.2.0a5/zibanu/django/db/backends/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a5/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.678224 zibanu-django-1.2.0a5/zibanu/django/db/backends/oracle/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a5/zibanu/django/db/backends/oracle/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0a5/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.678224 zibanu-django-1.2.0a5/zibanu/django/db/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0a5/zibanu/django/db/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0a5/zibanu/django/db/models/dated_model.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0a5/zibanu/django/db/models/manager.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0a5/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.671224 zibanu-django-1.2.0a5/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.671224 zibanu-django-1.2.0a5/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.679224 zibanu-django-1.2.0a5/zibanu/django/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3609 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.679224 zibanu-django-1.2.0a5/zibanu/django/logging/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0a5/zibanu/django/logging/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.680224 zibanu-django-1.2.0a5/zibanu/django/logging/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0a5/zibanu/django/logging/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.680224 zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/on_change_password.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/on_login.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/on_send_mail.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.680224 zibanu-django-1.2.0a5/zibanu/django/logging/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0a5/zibanu/django/logging/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      453 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.672224 zibanu-django-1.2.0a5/zibanu/django/logging/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.672224 zibanu-django-1.2.0a5/zibanu/django/logging/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.681224 zibanu-django-1.2.0a5/zibanu/django/logging/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.682224 zibanu-django-1.2.0a5/zibanu/django/logging/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0a5/zibanu/django/logging/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/migrations/0002_maillog.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0a5/zibanu/django/logging/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/logging/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.682224 zibanu-django-1.2.0a5/zibanu/django/repository/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0a5/zibanu/django/repository/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.682224 zibanu-django-1.2.0a5/zibanu/django/repository/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0a5/zibanu/django/repository/api/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0a5/zibanu/django/repository/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.683224 zibanu-django-1.2.0a5/zibanu/django/repository/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a5/zibanu/django/repository/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.683224 zibanu-django-1.2.0a5/zibanu/django/repository/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0a5/zibanu/django/repository/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0a5/zibanu/django/repository/lib/managers/document.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.683224 zibanu-django-1.2.0a5/zibanu/django/repository/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a5/zibanu/django/repository/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6973 2023-04-11 22:50:39.000000 zibanu-django-1.2.0a5/zibanu/django/repository/lib/utils/document_generator.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.672224 zibanu-django-1.2.0a5/zibanu/django/repository/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.672224 zibanu-django-1.2.0a5/zibanu/django/repository/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.684224 zibanu-django-1.2.0a5/zibanu/django/repository/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0a5/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-04-11 22:52:31.000000 zibanu-django-1.2.0a5/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.684224 zibanu-django-1.2.0a5/zibanu/django/repository/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0a5/zibanu/django/repository/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0a5/zibanu/django/repository/migrations/0002_document_description.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0a5/zibanu/django/repository/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0a5/zibanu/django/repository/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.685224 zibanu-django-1.2.0a5/zibanu/django/rest_framework/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.685224 zibanu-django-1.2.0a5/zibanu/django/rest_framework/exceptions/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1967 2022-12-14 09:17:28.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/exceptions/api_exception.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.685224 zibanu-django-1.2.0a5/zibanu/django/rest_framework/fields/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/fields/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/fields/current_user_default.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.686224 zibanu-django-1.2.0a5/zibanu/django/rest_framework/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/serializers/fields.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/serializers/model_serializer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.687224 zibanu-django-1.2.0a5/zibanu/django/rest_framework/viewsets/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    10439 2023-03-31 16:50:03.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a5/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.687224 zibanu-django-1.2.0a5/zibanu/django/template/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0a5/zibanu/django/template/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0a5/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.688224 zibanu-django-1.2.0a5/zibanu/django/template/context_processors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a5/zibanu/django/template/context_processors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a5/zibanu/django/template/context_processors/full_static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0a5/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.673225 zibanu-django-1.2.0a5/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.673225 zibanu-django-1.2.0a5/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.688224 zibanu-django-1.2.0a5/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0a5/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.689224 zibanu-django-1.2.0a5/zibanu/django/template/templatetags/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0a5/zibanu/django/template/templatetags/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0a5/zibanu/django/template/templatetags/static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0a5/zibanu/django/template/templatetags/string_concat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0a5/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0a5/zibanu/django/template/templatetags/sum_dict.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.690224 zibanu-django-1.2.0a5/zibanu/django/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3059 2023-03-14 20:09:11.000000 zibanu-django-1.2.0a5/zibanu/django/utils/code_generator.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0a5/zibanu/django/utils/date_time.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a5/zibanu/django/utils/error_messages.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4325 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/utils/mail.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a5/zibanu/django/utils/request_utils.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1251 2022-12-14 09:24:38.000000 zibanu-django-1.2.0a5/zibanu/django/utils/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a5/zibanu/django/utils/validate_cache_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-04-11 22:56:50.691224 zibanu-django-1.2.0a5/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-04-11 22:56:50.000000 zibanu-django-1.2.0a5/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3816 2023-04-11 22:56:50.000000 zibanu-django-1.2.0a5/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-04-11 22:56:50.000000 zibanu-django-1.2.0a5/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       32 2023-04-11 22:56:50.000000 zibanu-django-1.2.0a5/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-04-11 22:56:50.000000 zibanu-django-1.2.0a5/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.2.0a4/LICENSE` & `zibanu-django-1.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/PKG-INFO` & `zibanu-django-1.2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a4
+Version: 1.2.0a5
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.2.0a4/pyproject.toml` & `zibanu-django-1.2.0a5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.2.0-alpha.4"
+version = "1.2.0-alpha.5"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Zibanu library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `zibanu-django-1.2.0a4/zibanu/__init__.py` & `zibanu-django-1.2.0a5/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/apps.py` & `zibanu-django-1.2.0a5/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/auth/api/serializers.py` & `zibanu-django-1.2.0a5/zibanu/django/auth/api/serializers.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,27 +9,75 @@
 # Description:
 # ****************************************************************
 from django.conf import settings
 from django.contrib.auth import authenticate
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import update_last_login
 from rest_framework.exceptions import AuthenticationFailed
-from rest_framework_simplejwt import serializers
+from rest_framework import serializers
+from rest_framework_simplejwt.serializers import TokenObtainSerializer, TokenRefreshSerializer
 from rest_framework_simplejwt.settings import api_settings
 from rest_framework_simplejwt.tokens import SlidingToken
 from typing import Dict, Any
+from zibanu.django.auth.models import UserProfile
 
+class ProfileSerializer(serializers.ModelSerializer):
 
-class EmailTokenObtainSerializer(serializers.TokenObtainSerializer):
+    class Meta:
+        model = UserProfile
+        fields = ("timezone", "theme", "lang", "avatar", "messages_timeout", "keep_logged_in", "app_profile")
+
+class UserSerializer(serializers.ModelSerializer):
+    full_name = serializers.SerializerMethodField(default="Guest")
+    profile = ProfileSerializer(required=True, read_only=False)
+    roles = serializers.SerializerMethodField(default=[])
+    user_permissions = serializers.SerializerMethodField(default=[])
+
+    class Meta:
+        model = get_user_model()
+        fields = ("id", "email", "full_name", "is_staff", "is_superuser", "last_login", "profile", "roles", "user_permissions")
+
+    def get_user_permissions(self, instance) -> list:
+        user_permissions = []
+        if self.context.get("load_permissions", settings.ZB_AUTH_INCLUDE_PERMISSIONS):
+            for user_permission in instance.user_permissions.all():
+                user_permissions.append(user_permission.code)
+        return user_permissions
+
+    def get_roles(self, instance) -> list:
+        roles = []
+        if self.context.get("load_roles", settings.ZB_AUTH_INCLUDE_GROUPS):
+            for group in instance.user_permissions.all():
+                roles.append(group.name)
+        return roles
+
+    def get_full_name(self, instance) -> str:
+        return instance.get_full_name()
+
+
+
+
+
+class EmailTokenObtainSerializer(TokenObtainSerializer):
     username_field = get_user_model().EMAIL_FIELD
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.user = None
 
+    @classmethod
+    def get_token(cls, user):
+        token = super().get_token(user)
+
+        # Include user data
+        user_serializer = UserSerializer(instance=user)
+        token["user"] = user_serializer.data
+
+        return token
+
     def validate(self, attrs: Dict[str, Any]) -> Dict[Any, Any]:
         user = get_user_model().objects.filter(email__iexact=attrs.get(self.username_field)).first()
 
         if user is None:
             raise AuthenticationFailed(self.error_messages["no_active_account"], "no_active_account")
 
         authenticate_kwargs = {
@@ -44,45 +92,14 @@
             )
         return {}
 
 
 class TokenObtainSlidingSerializer(EmailTokenObtainSerializer):
     token_class = SlidingToken
 
-    @classmethod
-    def get_token(cls, user):
-        b_include_groups = settings.ZB_AUTH_INCLUDE_GROUPS
-        b_include_permissions = settings.ZB_AUTH_INCLUDE_PERMISSIONS
-        lst_user_roles = list()
-        lst_user_permissions = list()
-        token = super().get_token(user)
-        # Include user data
-        # Include Groups/Roles
-        if b_include_groups:
-            for user_group in user.groups.all():
-                lst_user_roles.append(user_group.name)
-        else:
-            lst_user_roles.append("guest")
-        # Include User Permissions
-        if b_include_permissions:
-            for user_permission in user.permissions.all():
-                lst_user_permissions.append(user_permission.codename)
-
-        token["user"] = dict(full_name=user.get_full_name(), email=user.email, username=user.username,
-                             is_staff=user.is_staff, is_superuser=user.is_superuser,
-                             last_login=user.last_login.isoformat(), roles=lst_user_roles.copy(),
-                             permissiones=lst_user_permissions.copy())
-
-        # Include User Permissions
-        if b_include_permissions:
-            for user_permission in user.permissions.all():
-                lst_user_permissions.append(user_permission.codename)
-            token["permissions"] = lst_user_permissions
-        return token
-
     def validate(self, attrs: Dict[str, Any]) -> Dict[Any, Any]:
         data = super().validate(attrs)
         token = self.get_token(self.user)
         data["token"] = str(token)
 
         if api_settings.UPDATE_LAST_LOGIN:
             update_last_login(None, self.user)
```

### Comparing `zibanu-django-1.2.0a4/zibanu/django/auth/urls.py` & `zibanu-django-1.2.0a5/zibanu/django/auth/urls.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/db/backends/oracle/base.py` & `zibanu-django-1.2.0a5/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/db/models/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/db/models/dated_model.py` & `zibanu-django-1.2.0a5/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/db/models/manager.py` & `zibanu-django-1.2.0a5/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/db/models/model.py` & `zibanu-django-1.2.0a5/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a5/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a5/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/apps.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_change_password.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/on_change_password.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_login.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/on_login.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/lib/events/on_send_mail.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/lib/events/on_send_mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a5/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a5/zibanu/django/logging/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0001_initial.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/migrations/0002_maillog.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/migrations/0002_maillog.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/logging/models.py` & `zibanu-django-1.2.0a5/zibanu/django/logging/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/apps.py` & `zibanu-django-1.2.0a5/zibanu/django/repository/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/repository/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/lib/managers/document.py` & `zibanu-django-1.2.0a5/zibanu/django/repository/lib/managers/document.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/repository/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/lib/utils/document_generator.py` & `zibanu-django-1.2.0a5/zibanu/django/repository/lib/utils/document_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a5/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a5/zibanu/django/repository/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/migrations/0001_initial.py` & `zibanu-django-1.2.0a5/zibanu/django/repository/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/repository/models.py` & `zibanu-django-1.2.0a5/zibanu/django/repository/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/fields.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu-django-1.2.0a5/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/apps.py` & `zibanu-django-1.2.0a5/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/context_processors/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu-django-1.2.0a5/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/context_processors/site.py` & `zibanu-django-1.2.0a5/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a5/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a5/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/static_uri.py` & `zibanu-django-1.2.0a5/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/string_concat.py` & `zibanu-django-1.2.0a5/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu-django-1.2.0a5/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/template/templatetags/sum_dict.py` & `zibanu-django-1.2.0a5/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/__init__.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/code_generator.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/date_time.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/error_messages.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/mail.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/request_utils.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/user.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu/django/utils/validate_cache_code.py` & `zibanu-django-1.2.0a5/zibanu/django/utils/validate_cache_code.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a4/zibanu_django.egg-info/PKG-INFO` & `zibanu-django-1.2.0a5/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a4
+Version: 1.2.0a5
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.2.0a4/zibanu_django.egg-info/SOURCES.txt` & `zibanu-django-1.2.0a5/zibanu_django.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 README.md
 pyproject.toml
 zibanu/__init__.py
 zibanu/django/__init__.py
 zibanu/django/apps.py
 zibanu/django/auth/__init__.py
 zibanu/django/auth/apps.py
+zibanu/django/auth/models.py
 zibanu/django/auth/urls.py
 zibanu/django/auth/api/__init__.py
 zibanu/django/auth/api/serializers.py
+zibanu/django/auth/lib/__init__.py
+zibanu/django/auth/lib/choices/__init__.py
+zibanu/django/auth/migrations/0001_initial.py
+zibanu/django/auth/migrations/__init__.py
 zibanu/django/db/__init__.py
 zibanu/django/db/backends/__init__.py
 zibanu/django/db/backends/oracle/__init__.py
 zibanu/django/db/backends/oracle/base.py
 zibanu/django/db/models/__init__.py
 zibanu/django/db/models/dated_model.py
 zibanu/django/db/models/manager.py
```

