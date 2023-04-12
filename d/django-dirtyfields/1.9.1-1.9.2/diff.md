# Comparing `tmp/django-dirtyfields-1.9.1.tar.gz` & `tmp/django-dirtyfields-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dirtyfields-1.9.1.tar", last modified: Sat Jan 14 06:13:41 2023, max compression
+gzip compressed data, was "django-dirtyfields-1.9.2.tar", last modified: Wed Apr 12 10:18:52 2023, max compression
```

## Comparing `django-dirtyfields-1.9.1.tar` & `django-dirtyfields-1.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 06:13:41.507292 django-dirtyfields-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/ChangeLog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-01-14 06:13:41.507292 django-dirtyfields-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-01-14 06:13:41.507292 django-dirtyfields-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 06:13:41.503292 django-dirtyfields-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 06:13:41.503292 django-dirtyfields-1.9.1/src/dirtyfields/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/src/dirtyfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/src/dirtyfields/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-01-14 06:13:30.000000 django-dirtyfields-1.9.1/src/dirtyfields/dirtyfields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 06:13:41.507292 django-dirtyfields-1.9.1/src/django_dirtyfields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-01-14 06:13:41.000000 django-dirtyfields-1.9.1/src/django_dirtyfields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-01-14 06:13:41.000000 django-dirtyfields-1.9.1/src/django_dirtyfields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 06:13:41.000000 django-dirtyfields-1.9.1/src/django_dirtyfields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-14 06:13:41.000000 django-dirtyfields-1.9.1/src/django_dirtyfields.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-14 06:13:41.000000 django-dirtyfields-1.9.1/src/django_dirtyfields.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/ChangeLog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/src/dirtyfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/src/dirtyfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/src/dirtyfields/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/src/dirtyfields/dirtyfields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/top_level.txt
```

### Comparing `django-dirtyfields-1.9.1/ChangeLog.rst` & `django-dirtyfields-1.9.2/ChangeLog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. _unreleased:
 
 unreleased
 ----------
 
 
 
+.. _v1.9.2:
+
+1.9.2 (2023-04-12)
+------------------
+
+*New:*
+    - Confirm support for Django 4.2
+
+
 .. _v1.9.1:
 
 1.9.1 (2023-01-14)
 ------------------
 
 *Bugfix:*
     - Fixed a :code:`KeyError` that would occur when updating a field two times in a row when
```

### Comparing `django-dirtyfields-1.9.1/LICENSE` & `django-dirtyfields-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dirtyfields-1.9.1/PKG-INFO` & `django-dirtyfields-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dirtyfields
-Version: 1.9.1
+Version: 1.9.2
 Summary: Tracking dirty fields on a Django model instance.
 Home-page: https://github.com/romgar/django-dirtyfields
 Author: Romain Garrigues
 Maintainer: Lincoln Puzey
 License: BSD
 Project-URL: Documentation, https://django-dirtyfields.readthedocs.io/
 Project-URL: Changelog, https://github.com/romgar/django-dirtyfields/blob/develop/ChangeLog.rst
@@ -27,14 +27,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 Django Dirty Fields
 ===================
@@ -68,15 +69,15 @@
 +------------------------+-----------------------------------+
 | 2.2, 3.0, 3.1          | 3.7, 3.8, 3.9                     |
 +------------------------+-----------------------------------+
 | 3.2                    | 3.7, 3.8, 3.9, 3.10               |
 +------------------------+-----------------------------------+
 | 4.0                    | 3.8, 3.9, 3.10                    |
 +------------------------+-----------------------------------+
-| 4.1                    | 3.8, 3.9, 3.10, 3.11              |
+| 4.1, 4.2               | 3.8, 3.9, 3.10, 3.11              |
 +------------------------+-----------------------------------+
 
 
 
 Install
 =======
```

### Comparing `django-dirtyfields-1.9.1/README.rst` & `django-dirtyfields-1.9.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 +------------------------+-----------------------------------+
 | 2.2, 3.0, 3.1          | 3.7, 3.8, 3.9                     |
 +------------------------+-----------------------------------+
 | 3.2                    | 3.7, 3.8, 3.9, 3.10               |
 +------------------------+-----------------------------------+
 | 4.0                    | 3.8, 3.9, 3.10                    |
 +------------------------+-----------------------------------+
-| 4.1                    | 3.8, 3.9, 3.10, 3.11              |
+| 4.1, 4.2               | 3.8, 3.9, 3.10, 3.11              |
 +------------------------+-----------------------------------+
 
 
 
 Install
 =======
```

### Comparing `django-dirtyfields-1.9.1/setup.cfg` & `django-dirtyfields-1.9.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 license = BSD
 license_files = LICENSE
 description = Tracking dirty fields on a Django model instance.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 
 [options]
```

### Comparing `django-dirtyfields-1.9.1/src/dirtyfields/compare.py` & `django-dirtyfields-1.9.2/src/dirtyfields/compare.py`

 * *Files identical despite different names*

### Comparing `django-dirtyfields-1.9.1/src/dirtyfields/dirtyfields.py` & `django-dirtyfields-1.9.2/src/dirtyfields/dirtyfields.py`

 * *Files identical despite different names*

### Comparing `django-dirtyfields-1.9.1/src/django_dirtyfields.egg-info/PKG-INFO` & `django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dirtyfields
-Version: 1.9.1
+Version: 1.9.2
 Summary: Tracking dirty fields on a Django model instance.
 Home-page: https://github.com/romgar/django-dirtyfields
 Author: Romain Garrigues
 Maintainer: Lincoln Puzey
 License: BSD
 Project-URL: Documentation, https://django-dirtyfields.readthedocs.io/
 Project-URL: Changelog, https://github.com/romgar/django-dirtyfields/blob/develop/ChangeLog.rst
@@ -27,14 +27,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 Django Dirty Fields
 ===================
@@ -68,15 +69,15 @@
 +------------------------+-----------------------------------+
 | 2.2, 3.0, 3.1          | 3.7, 3.8, 3.9                     |
 +------------------------+-----------------------------------+
 | 3.2                    | 3.7, 3.8, 3.9, 3.10               |
 +------------------------+-----------------------------------+
 | 4.0                    | 3.8, 3.9, 3.10                    |
 +------------------------+-----------------------------------+
-| 4.1                    | 3.8, 3.9, 3.10, 3.11              |
+| 4.1, 4.2               | 3.8, 3.9, 3.10, 3.11              |
 +------------------------+-----------------------------------+
 
 
 
 Install
 =======
```

