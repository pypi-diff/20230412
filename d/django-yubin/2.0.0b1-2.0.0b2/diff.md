# Comparing `tmp/django-yubin-2.0.0b1.tar.gz` & `tmp/django-yubin-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-yubin-2.0.0b1.tar", last modified: Thu Mar 30 10:59:11 2023, max compression
+gzip compressed data, was "django-yubin-2.0.0b2.tar", last modified: Wed Apr 12 11:10:22 2023, max compression
```

## Comparing `django-yubin-2.0.0b1.tar` & `django-yubin-2.0.0b2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.963780 django-yubin-2.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-30 10:59:11.967780 django-yubin-2.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.959780 django-yubin-2.0.0b1/django_yubin/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/mailparser_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.959780 django-yubin-2.0.0b1/django_yubin/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.959780 django-yubin-2.0.0b1/django_yubin/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/management/commands/create_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/management/commands/db2file.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/management/commands/file2db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/management/commands/sample.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/management/commands/send_test_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/message_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.963780 django-yubin-2.0.0b1/django_yubin/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0002_auto_20170405_1635.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0003_auto_20171201_1506.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0004_message_date_sent.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0005_auto_20181128_0407.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0006_auto_20200319_1120.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0007_auto_20200319_1158.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0008_auto_20200320_0407.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0009_auto_20221122_1605.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/0010_message_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/storage_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.955780 django-yubin-2.0.0b1/django_yubin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.951780 django-yubin-2.0.0b1/django_yubin/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.955780 django-yubin-2.0.0b1/django_yubin/templates/admin/django_yubin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.963780 django-yubin-2.0.0b1/django_yubin/templates/admin/django_yubin/message/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/templates/admin/django_yubin/message/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.963780 django-yubin-2.0.0b1/django_yubin/templates/django_yubin/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/templates/django_yubin/html_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/templates/django_yubin/message_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/django_yubin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.959780 django-yubin-2.0.0b1/django_yubin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-30 10:59:11.000000 django-yubin-2.0.0b1/django_yubin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-30 10:59:11.000000 django-yubin-2.0.0b1/django_yubin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:59:11.000000 django-yubin-2.0.0b1/django_yubin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 10:59:11.000000 django-yubin-2.0.0b1/django_yubin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 10:59:11.000000 django-yubin-2.0.0b1/django_yubin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:11.963780 django-yubin-2.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/mailviews.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/queue.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/docs/storages.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-30 10:59:11.967780 django-yubin-2.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-30 10:59:01.000000 django-yubin-2.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/mailparser_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/create_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/db2file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/file2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/sample.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/send_test_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/message_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0002_auto_20170405_1635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0003_auto_20171201_1506.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0004_message_date_sent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0005_auto_20181128_0407.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0006_auto_20200319_1120.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0007_auto_20200319_1158.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0008_auto_20200320_0407.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0009_auto_20221122_1605.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0010_message_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/storage_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.154146 django-yubin-2.0.0b2/django_yubin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.154146 django-yubin-2.0.0b2/django_yubin/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.154146 django-yubin-2.0.0b2/django_yubin/templates/admin/django_yubin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/templates/admin/django_yubin/message/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/templates/admin/django_yubin/message/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/templates/django_yubin/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/templates/django_yubin/html_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/templates/django_yubin/message_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/mailviews.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/queue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/storages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/setup.py
```

### Comparing `django-yubin-2.0.0b1/LICENSE` & `django-yubin-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/PKG-INFO` & `django-yubin-2.0.0b2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-yubin
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A reusable Django app for composing and queueing emails django-mailviews + Celery + others
 Home-page: http://github.com/APSL/django-yubin
 Author: Antoni Aloy
 Author-email: aaloy@apsl.net
 Maintainer: APSL
 Maintainer-email: info@apsl.net
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 django-yubin
 ============
 
 .. image:: https://github.com/APSL/django-yubin/actions/workflows/test.yml/badge.svg
   :target: https://github.com/APSL/django-yubin/actions/workflows/test.yml
```

### Comparing `django-yubin-2.0.0b1/README.rst` & `django-yubin-2.0.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/__init__.py` & `django-yubin-2.0.0b2/django_yubin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/admin.py` & `django-yubin-2.0.0b2/django_yubin/admin.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/backends.py` & `django-yubin-2.0.0b2/django_yubin/backends.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/constants.py` & `django-yubin-2.0.0b2/django_yubin/constants.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/engine.py` & `django-yubin-2.0.0b2/django_yubin/engine.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/mailparser_utils.py` & `django-yubin-2.0.0b2/django_yubin/mailparser_utils.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/management/commands/create_mail.py` & `django-yubin-2.0.0b2/django_yubin/management/commands/create_mail.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/management/commands/file2db.py` & `django-yubin-2.0.0b2/django_yubin/management/commands/file2db.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/management/commands/sample.pdf` & `django-yubin-2.0.0b2/django_yubin/management/commands/sample.pdf`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/management/commands/send_test_mail.py` & `django-yubin-2.0.0b2/django_yubin/management/commands/send_test_mail.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/message_views.py` & `django-yubin-2.0.0b2/django_yubin/message_views.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/migrations/0001_initial.py` & `django-yubin-2.0.0b2/django_yubin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/migrations/0002_auto_20170405_1635.py` & `django-yubin-2.0.0b2/django_yubin/migrations/0002_auto_20170405_1635.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/migrations/0003_auto_20171201_1506.py` & `django-yubin-2.0.0b2/django_yubin/migrations/0003_auto_20171201_1506.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/migrations/0006_auto_20200319_1120.py` & `django-yubin-2.0.0b2/django_yubin/migrations/0006_auto_20200319_1120.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/migrations/0007_auto_20200319_1158.py` & `django-yubin-2.0.0b2/django_yubin/migrations/0007_auto_20200319_1158.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/migrations/0009_auto_20221122_1605.py` & `django-yubin-2.0.0b2/django_yubin/migrations/0009_auto_20221122_1605.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/models.py` & `django-yubin-2.0.0b2/django_yubin/models.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/settings.py` & `django-yubin-2.0.0b2/django_yubin/settings.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/signals.py` & `django-yubin-2.0.0b2/django_yubin/signals.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/storage_backends.py` & `django-yubin-2.0.0b2/django_yubin/storage_backends.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/tasks.py` & `django-yubin-2.0.0b2/django_yubin/tasks.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/templates/django_yubin/message_detail.html` & `django-yubin-2.0.0b2/django_yubin/templates/django_yubin/message_detail.html`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin/views.py` & `django-yubin-2.0.0b2/django_yubin/views.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/django_yubin.egg-info/PKG-INFO` & `django-yubin-2.0.0b2/django_yubin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-yubin
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A reusable Django app for composing and queueing emails django-mailviews + Celery + others
 Home-page: http://github.com/APSL/django-yubin
 Author: Antoni Aloy
 Author-email: aaloy@apsl.net
 Maintainer: APSL
 Maintainer-email: info@apsl.net
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 django-yubin
 ============
 
 .. image:: https://github.com/APSL/django-yubin/actions/workflows/test.yml/badge.svg
   :target: https://github.com/APSL/django-yubin/actions/workflows/test.yml
```

### Comparing `django-yubin-2.0.0b1/django_yubin.egg-info/SOURCES.txt` & `django-yubin-2.0.0b2/django_yubin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/Makefile` & `django-yubin-2.0.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/changelog.rst` & `django-yubin-2.0.0b2/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 --------------------
 
 Changed
 ^^^^^^^
 * Send and queue emails with Celery instead of with Cron.
 * Drop priority headers (useless with queues).
 * Storage backends to save emails in databases, file storages, etc.
-* Supported versions: Python 3.8~3.11, Django 3.2~4.1, Celery 5.0~5.2.
+* Supported versions: Python 3.8~3.11, Django 3.2~4.2, Celery 5.0~5.2.
 * Migrate CI/CD from Travis to Github Actions.
 * Docker Compose for external dependencies in development environment.
 * Get django_yubin version programmatically.
 * Update docs.
 
 
 Older versions - 2022-01-17
```

### Comparing `django-yubin-2.0.0b1/docs/conf.py` & `django-yubin-2.0.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/contributing.rst` & `django-yubin-2.0.0b2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/index.rst` & `django-yubin-2.0.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/install.rst` & `django-yubin-2.0.0b2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/mailviews.rst` & `django-yubin-2.0.0b2/docs/mailviews.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/queue.rst` & `django-yubin-2.0.0b2/docs/queue.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/settings.rst` & `django-yubin-2.0.0b2/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/docs/storages.rst` & `django-yubin-2.0.0b2/docs/storages.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b1/setup.py` & `django-yubin-2.0.0b2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,9 +51,10 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ]
 )
```

