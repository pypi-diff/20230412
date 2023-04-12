# Comparing `tmp/pretix_plugin_attendance_certificate-0.1.0.tar.gz` & `tmp/pretix_plugin_attendance_certificate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.0.tar", last modified: Wed Apr 12 16:06:08 2023, max compression
+gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.1.tar", last modified: Wed Apr 12 16:08:28 2023, max compression
```

## Comparing `pretix_plugin_attendance_certificate-0.1.0.tar` & `pretix_plugin_attendance_certificate-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2023-04-11 16:14:44.506145 pretix_plugin_attendance_certificate-0.1.0/LICENSE
--rw-r--r--   0        0        0     1323 2023-04-11 16:19:22.769913 pretix_plugin_attendance_certificate-0.1.0/README.rst
--rw-r--r--   0        0        0     1100 2023-04-12 15:19:32.043013 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/__init__.py
--rw-r--r--   0        0        0      313 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      313 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1960 2023-04-12 15:21:58.462668 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-11 18:53:00.088361 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/migrations/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-12 15:24:15.906589 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/models.py
--rw-r--r--   0        0        0     1516 2023-04-12 15:19:32.063013 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/render.py
--rw-r--r--   0        0        0     1997 2023-04-12 15:19:32.099012 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/signals.py
--rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      779 2023-04-11 18:09:52.325353 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
--rw-r--r--   0        0        0     2615 2023-04-12 15:19:32.135011 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/tasks.py
--rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      117 2023-04-12 11:33:19.981965 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      495 2023-04-12 15:19:32.031014 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/urls.py
--rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/views/__init__.py
--rw-r--r--   0        0        0     3611 2023-04-12 15:19:32.151010 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/views/editor.py
--rw-r--r--   0        0        0     1967 2023-04-12 15:19:32.087012 pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/views/emails.py
--rw-r--r--   0        0        0      707 2023-04-12 16:06:08.268064 pretix_plugin_attendance_certificate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 16:19:09.558301 pretix_plugin_attendance_certificate-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-11 16:14:44.506145 pretix_plugin_attendance_certificate-0.1.1/LICENSE
+-rw-r--r--   0        0        0      161 2023-04-12 16:07:59.588761 pretix_plugin_attendance_certificate-0.1.1/README.md
+-rw-r--r--   0        0        0     1100 2023-04-12 15:19:32.043013 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      313 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1960 2023-04-12 15:21:58.462668 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:53:00.088361 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/migrations/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-12 15:24:15.906589 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/models.py
+-rw-r--r--   0        0        0     1516 2023-04-12 15:19:32.063013 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/render.py
+-rw-r--r--   0        0        0     1997 2023-04-12 15:19:32.099012 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/signals.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0      779 2023-04-11 18:09:52.325353 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
+-rw-r--r--   0        0        0     2615 2023-04-12 15:19:32.135011 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0      117 2023-04-12 11:33:19.981965 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      495 2023-04-12 15:19:32.031014 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/urls.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:14:44.510145 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/views/__init__.py
+-rw-r--r--   0        0        0     3611 2023-04-12 15:19:32.151010 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/views/editor.py
+-rw-r--r--   0        0        0     1967 2023-04-12 15:19:32.087012 pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/views/emails.py
+-rw-r--r--   0        0        0      706 2023-04-12 16:08:28.527902 pretix_plugin_attendance_certificate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 16:19:09.558301 pretix_plugin_attendance_certificate-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.1/PKG-INFO
```

### Comparing `pretix_plugin_attendance_certificate-0.1.0/LICENSE` & `pretix_plugin_attendance_certificate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/__init__.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/migrations/0001_initial.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/models.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/models.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/render.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/render.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/signals.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/signals.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/tasks.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/tasks.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/views/editor.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/views/editor.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pretix_attendance_certificate/views/emails.py` & `pretix_plugin_attendance_certificate-0.1.1/pretix_attendance_certificate/views/emails.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.0/pyproject.toml` & `pretix_plugin_attendance_certificate-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pretix-plugin-attendance-certificate"
-version = "0.1.0"
+version = "0.1.1"
 description = "Create attendance certificates"
 authors = [
     { name = "Python Italia" },
 ]
 dependencies = []
 requires-python = ">=3.9,<4.0"
-readme = "README.rst"
+readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 
 [project.entry-points."pretix.plugin"]
```

