# Comparing `tmp/django-advanced-pages-0.8.3.tar.gz` & `tmp/django-advanced-pages-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-pages-0.8.3.tar", last modified: Wed Mar 23 11:44:29 2022, max compression
+gzip compressed data, was "django-advanced-pages-0.8.4.tar", last modified: Wed Apr 12 19:41:20 2023, max compression
```

## Comparing `django-advanced-pages-0.8.3.tar` & `django-advanced-pages-0.8.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:29.659907 django-advanced-pages-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-03-23 11:44:29.655907 django-advanced-pages-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-23 11:44:21.000000 django-advanced-pages-0.8.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 11:44:29.659907 django-advanced-pages-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:29.655907 django-advanced-pages-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:29.655907 django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-03-23 11:44:29.000000 django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-03-23 11:44:29.000000 django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 11:44:29.000000 django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-03-23 11:44:29.000000 django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-23 11:44:29.000000 django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:29.655907 django-advanced-pages-0.8.3/src/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:29.655907 django-advanced-pages-0.8.3/src/pages/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/fixtures/initial_pages.json
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:29.655907 django-advanced-pages-0.8.3/src/pages/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/migrations/0002_auto_20210609_2039.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/migrations/0003_auto_20210621_0847.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/src/pages/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:29.655907 django-advanced-pages-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      655 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-03-23 11:44:16.000000 django-advanced-pages-0.8.3/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 19:41:12.000000 django-advanced-pages-0.8.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.082033 django-advanced-pages-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 19:41:20.000000 django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/pages/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/fixtures/initial_pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/src/pages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/0002_auto_20210609_2039.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/0003_auto_20210621_0847.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/src/pages/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:20.086033 django-advanced-pages-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 19:41:09.000000 django-advanced-pages-0.8.4/tests/urls.py
```

### Comparing `django-advanced-pages-0.8.3/PKG-INFO` & `django-advanced-pages-0.8.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: django-advanced-pages
-Version: 0.8.3
+Version: 0.8.4
 Summary: Django flatpages with advanced features
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -19,23 +18,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: test
+License-File: LICENSE
 
 .. image:: https://github.com/snake-soft/django-advanced-pages/workflows/Django%20CI/badge.svg
    :target: https://github.com/snake-soft/django-advanced-pages/actions
    :alt: Build
 
 .. image:: https://api.codeclimate.com/v1/badges/cfd2071c8e13d1eab244/maintainability
    :target: https://codeclimate.com/github/snake-soft/django-advanced-pages/maintainability
    :alt: Maintainability
 
+.. image:: https://api.codeclimate.com/v1/badges/cfd2071c8e13d1eab244/test_coverage
+   :target: https://codeclimate.com/github/snake-soft/django-advanced-pages/test_coverage
+   :alt: Test Coverage
+
 .. image:: https://codecov.io/gh/snake-soft/django-advanced-pages/branch/main/graph/badge.svg?token=X9MJQJBAEH
    :target: https://codecov.io/gh/snake-soft/django-advanced-pages
 
 .. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
     
 =====================
@@ -83,9 +87,7 @@
 .. code-block:: python
 
    from pages.models import Page, Category
    'pages': {
       'company': Page.objects.filter(category=Category.COMPANY),
       'legal': Page.objects.filter(category=Category.LEGAL),
    },
-
-
```

### Comparing `django-advanced-pages-0.8.3/README.rst` & `django-advanced-pages-0.8.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,18 @@
    :target: https://github.com/snake-soft/django-advanced-pages/actions
    :alt: Build
 
 .. image:: https://api.codeclimate.com/v1/badges/cfd2071c8e13d1eab244/maintainability
    :target: https://codeclimate.com/github/snake-soft/django-advanced-pages/maintainability
    :alt: Maintainability
 
+.. image:: https://api.codeclimate.com/v1/badges/cfd2071c8e13d1eab244/test_coverage
+   :target: https://codeclimate.com/github/snake-soft/django-advanced-pages/test_coverage
+   :alt: Test Coverage
+
 .. image:: https://codecov.io/gh/snake-soft/django-advanced-pages/branch/main/graph/badge.svg?token=X9MJQJBAEH
    :target: https://codecov.io/gh/snake-soft/django-advanced-pages
 
 .. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
     
 =====================
```

### Comparing `django-advanced-pages-0.8.3/setup.py` & `django-advanced-pages-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/PKG-INFO` & `django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: django-advanced-pages
-Version: 0.8.3
+Version: 0.8.4
 Summary: Django flatpages with advanced features
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -19,23 +18,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: test
+License-File: LICENSE
 
 .. image:: https://github.com/snake-soft/django-advanced-pages/workflows/Django%20CI/badge.svg
    :target: https://github.com/snake-soft/django-advanced-pages/actions
    :alt: Build
 
 .. image:: https://api.codeclimate.com/v1/badges/cfd2071c8e13d1eab244/maintainability
    :target: https://codeclimate.com/github/snake-soft/django-advanced-pages/maintainability
    :alt: Maintainability
 
+.. image:: https://api.codeclimate.com/v1/badges/cfd2071c8e13d1eab244/test_coverage
+   :target: https://codeclimate.com/github/snake-soft/django-advanced-pages/test_coverage
+   :alt: Test Coverage
+
 .. image:: https://codecov.io/gh/snake-soft/django-advanced-pages/branch/main/graph/badge.svg?token=X9MJQJBAEH
    :target: https://codecov.io/gh/snake-soft/django-advanced-pages
 
 .. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
     
 =====================
@@ -83,9 +87,7 @@
 .. code-block:: python
 
    from pages.models import Page, Category
    'pages': {
       'company': Page.objects.filter(category=Category.COMPANY),
       'legal': Page.objects.filter(category=Category.LEGAL),
    },
-
-
```

### Comparing `django-advanced-pages-0.8.3/src/django_advanced_pages.egg-info/SOURCES.txt` & `django-advanced-pages-0.8.4/src/django_advanced_pages.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 VERSION
 setup.py
 src/django_advanced_pages.egg-info/PKG-INFO
 src/django_advanced_pages.egg-info/SOURCES.txt
 src/django_advanced_pages.egg-info/dependency_links.txt
```

### Comparing `django-advanced-pages-0.8.3/src/pages/admin.py` & `django-advanced-pages-0.8.4/src/pages/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/src/pages/fixtures/initial_pages.json` & `django-advanced-pages-0.8.4/src/pages/fixtures/initial_pages.json`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/src/pages/migrations/0001_initial.py` & `django-advanced-pages-0.8.4/src/pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/src/pages/migrations/0003_auto_20210621_0847.py` & `django-advanced-pages-0.8.4/src/pages/migrations/0003_auto_20210621_0847.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/src/pages/models.py` & `django-advanced-pages-0.8.4/src/pages/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/tests/manage.py` & `django-advanced-pages-0.8.4/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/tests/settings.py` & `django-advanced-pages-0.8.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.3/tests/test_models.py` & `django-advanced-pages-0.8.4/tests/test_models.py`

 * *Files identical despite different names*

