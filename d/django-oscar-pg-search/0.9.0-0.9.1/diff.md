# Comparing `tmp/django-oscar-pg-search-0.9.0.tar.gz` & `tmp/django-oscar-pg-search-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-pg-search-0.9.0.tar", last modified: Tue Apr 11 20:00:08 2023, max compression
+gzip compressed data, was "django-oscar-pg-search-0.9.1.tar", last modified: Wed Apr 12 18:54:09 2023, max compression
```

## Comparing `django-oscar-pg-search-0.9.0.tar` & `django-oscar-pg-search-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.807106 django-oscar-pg-search-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-11 20:00:08.803106 django-oscar-pg-search-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 20:00:01.000000 django-oscar-pg-search-0.9.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:00:08.807106 django-oscar-pg-search-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.795106 django-oscar-pg-search-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.799106 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.799106 django-oscar-pg-search-0.9.0/src/oscar_pg_search/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.803106 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/attribute_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/base_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/filter_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/offer_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/product_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/order_by_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/postgres_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.803106 django-oscar-pg-search-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/test_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.868047 django-oscar-pg-search-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-12 18:54:09.868047 django-oscar-pg-search-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 18:54:03.000000 django-oscar-pg-search-0.9.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:54:09.868047 django-oscar-pg-search-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.860047 django-oscar-pg-search-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-12 18:54:09.000000 django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-12 18:54:09.000000 django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:54:09.000000 django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 18:54:09.000000 django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 18:54:09.000000 django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/attribute_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/base_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/filter_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/offer_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/product_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/order_by_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/postgres_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templates/oscar_pg_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templates/oscar_pg_search/catalogue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/filter_forms.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.864047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templates/oscar_pg_search/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templates/oscar_pg_search/partials/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.868047 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/templatetags/oscar_pg_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/src/oscar_pg_search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:09.868047 django-oscar-pg-search-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/tests/test_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 18:54:00.000000 django-oscar-pg-search-0.9.1/tests/urls.py
```

### Comparing `django-oscar-pg-search-0.9.0/LICENSE` & `django-oscar-pg-search-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/PKG-INFO` & `django-oscar-pg-search-0.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-pg-search
-Version: 0.9.0
+Version: 0.9.1
 Summary: Pure Postgresql search backend for Django Oscar
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -21,48 +21,51 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 [![Maintainability](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/test_coverage)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/test_coverage)
 [![image](https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q)](https://codecov.io/gh/snake-soft/django-oscar-pg-search)
 [![image](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 Postgresql search handler for Django-Oscar
 ==========================================
 This creates a search handler without the need of any search backend. It is designed for the e-commerce framework [Oscar](https://github.com/django-oscar/django-oscar).
 
 It is implemented a little bit expensive but uses 4 annotated search vectors: \* upc \* title \* meta\_description \* meta\_title
 
 This way the search can be manipulated through the meta fields. It is running productive in a heavily customized env for many months now. I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded. We use it fully lazy with endless scrolling.
 
 
 To-Do
------
+==========================================
 
 - Provide a generic way to use filter forms
 - Writing Tests
 
 
 Features
---------
+==========================================
 
 + Don't need to use some additional search backend like elastic
 + Creates filters (facets) for:
     - Data that is directly attached to the Product model
     - including foreign key choices
     - AttributeValues of the products
     - StockRecord entries
 
 
 Installation
-------------
+==========================================
 
+Basic
+----------------------------------------------
 Install using pip:
 
 ```bash
 pip install django-oscar-pg-search
 ```
 
 ```python
@@ -82,17 +85,64 @@
 
 Trigram search is our search algorithm. Enable it at your database by executing the following sql:
 
 ```
 CREATE EXTENSION pg_trgm;
 ```
 
+Optional Search box
+----------------------------------------------
+To install the included Search box that passes the previous search term.
+(eg. in 'oscar/partials/search.html')
+
+```python
+{% include 'oscar_pg_search/partials/search.html' %}
+```
+
+Optional Filter Forms
+----------------------------------------------
+To use the included filter forms, include them in the template eg. in 'oscar/layout_2_col.html' after '{% block column_left_extra %}{% endblock %}'.
+
+```python
+{% include 'oscar_pg_search/catalogue/partials/filter_forms.html' %}
+```
+
+and include the mixin into the catalogue views.
+
+```python
+# apps/catalogue/views.py
+from oscar.apps.catalogue import views
+from oscar_pg_search.mixins import SearchViewMixin
+
+
+class CatalogueView(SearchViewMixin, views.CatalogueView):
+    pass
+
+
+class ProductCategoryView(SearchViewMixin, views.ProductCategoryView):
+    pass
+
+```
+
+
+Optional Use Chosen.js
+----------------------------------------------
+To empower multiple choice fields with chosen load it eg. in 'oscar/base.html'.
+
+```python
+# At the beginning:
+{% load oscar_pg_search %}
+
+# After jQuery is loaded:
+{% oscar_pg_search_base %}
+```
+
 
 Settings
---------
+==========================================
 
 If you want to add some fields that are directly attached to the Product
 model:
 
 ```python
 # settings.py
 OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
```

### Comparing `django-oscar-pg-search-0.9.0/README.md` & `django-oscar-pg-search-0.9.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 [![Maintainability](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/test_coverage)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/test_coverage)
 [![image](https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q)](https://codecov.io/gh/snake-soft/django-oscar-pg-search)
 [![image](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 Postgresql search handler for Django-Oscar
 ==========================================
 This creates a search handler without the need of any search backend. It is designed for the e-commerce framework [Oscar](https://github.com/django-oscar/django-oscar).
 
 It is implemented a little bit expensive but uses 4 annotated search vectors: \* upc \* title \* meta\_description \* meta\_title
 
 This way the search can be manipulated through the meta fields. It is running productive in a heavily customized env for many months now. I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded. We use it fully lazy with endless scrolling.
 
 
 To-Do
------
+==========================================
 
 - Provide a generic way to use filter forms
 - Writing Tests
 
 
 Features
---------
+==========================================
 
 + Don't need to use some additional search backend like elastic
 + Creates filters (facets) for:
     - Data that is directly attached to the Product model
     - including foreign key choices
     - AttributeValues of the products
     - StockRecord entries
 
 
 Installation
-------------
+==========================================
 
+Basic
+----------------------------------------------
 Install using pip:
 
 ```bash
 pip install django-oscar-pg-search
 ```
 
 ```python
@@ -57,17 +60,64 @@
 
 Trigram search is our search algorithm. Enable it at your database by executing the following sql:
 
 ```
 CREATE EXTENSION pg_trgm;
 ```
 
+Optional Search box
+----------------------------------------------
+To install the included Search box that passes the previous search term.
+(eg. in 'oscar/partials/search.html')
+
+```python
+{% include 'oscar_pg_search/partials/search.html' %}
+```
+
+Optional Filter Forms
+----------------------------------------------
+To use the included filter forms, include them in the template eg. in 'oscar/layout_2_col.html' after '{% block column_left_extra %}{% endblock %}'.
+
+```python
+{% include 'oscar_pg_search/catalogue/partials/filter_forms.html' %}
+```
+
+and include the mixin into the catalogue views.
+
+```python
+# apps/catalogue/views.py
+from oscar.apps.catalogue import views
+from oscar_pg_search.mixins import SearchViewMixin
+
+
+class CatalogueView(SearchViewMixin, views.CatalogueView):
+    pass
+
+
+class ProductCategoryView(SearchViewMixin, views.ProductCategoryView):
+    pass
+
+```
+
+
+Optional Use Chosen.js
+----------------------------------------------
+To empower multiple choice fields with chosen load it eg. in 'oscar/base.html'.
+
+```python
+# At the beginning:
+{% load oscar_pg_search %}
+
+# After jQuery is loaded:
+{% oscar_pg_search_base %}
+```
+
 
 Settings
---------
+==========================================
 
 If you want to add some fields that are directly attached to the Product
 model:
 
 ```python
 # settings.py
 OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
```

### Comparing `django-oscar-pg-search-0.9.0/setup.py` & `django-oscar-pg-search-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/PKG-INFO` & `django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-pg-search
-Version: 0.9.0
+Version: 0.9.1
 Summary: Pure Postgresql search backend for Django Oscar
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -21,48 +21,51 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 [![Maintainability](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/test_coverage)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/test_coverage)
 [![image](https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q)](https://codecov.io/gh/snake-soft/django-oscar-pg-search)
 [![image](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 Postgresql search handler for Django-Oscar
 ==========================================
 This creates a search handler without the need of any search backend. It is designed for the e-commerce framework [Oscar](https://github.com/django-oscar/django-oscar).
 
 It is implemented a little bit expensive but uses 4 annotated search vectors: \* upc \* title \* meta\_description \* meta\_title
 
 This way the search can be manipulated through the meta fields. It is running productive in a heavily customized env for many months now. I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded. We use it fully lazy with endless scrolling.
 
 
 To-Do
------
+==========================================
 
 - Provide a generic way to use filter forms
 - Writing Tests
 
 
 Features
---------
+==========================================
 
 + Don't need to use some additional search backend like elastic
 + Creates filters (facets) for:
     - Data that is directly attached to the Product model
     - including foreign key choices
     - AttributeValues of the products
     - StockRecord entries
 
 
 Installation
-------------
+==========================================
 
+Basic
+----------------------------------------------
 Install using pip:
 
 ```bash
 pip install django-oscar-pg-search
 ```
 
 ```python
@@ -82,17 +85,64 @@
 
 Trigram search is our search algorithm. Enable it at your database by executing the following sql:
 
 ```
 CREATE EXTENSION pg_trgm;
 ```
 
+Optional Search box
+----------------------------------------------
+To install the included Search box that passes the previous search term.
+(eg. in 'oscar/partials/search.html')
+
+```python
+{% include 'oscar_pg_search/partials/search.html' %}
+```
+
+Optional Filter Forms
+----------------------------------------------
+To use the included filter forms, include them in the template eg. in 'oscar/layout_2_col.html' after '{% block column_left_extra %}{% endblock %}'.
+
+```python
+{% include 'oscar_pg_search/catalogue/partials/filter_forms.html' %}
+```
+
+and include the mixin into the catalogue views.
+
+```python
+# apps/catalogue/views.py
+from oscar.apps.catalogue import views
+from oscar_pg_search.mixins import SearchViewMixin
+
+
+class CatalogueView(SearchViewMixin, views.CatalogueView):
+    pass
+
+
+class ProductCategoryView(SearchViewMixin, views.ProductCategoryView):
+    pass
+
+```
+
+
+Optional Use Chosen.js
+----------------------------------------------
+To empower multiple choice fields with chosen load it eg. in 'oscar/base.html'.
+
+```python
+# At the beginning:
+{% load oscar_pg_search %}
+
+# After jQuery is loaded:
+{% oscar_pg_search_base %}
+```
+
 
 Settings
---------
+==========================================
 
 If you want to add some fields that are directly attached to the Product
 model:
 
 ```python
 # settings.py
 OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
```

### Comparing `django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/SOURCES.txt` & `django-oscar-pg-search-0.9.1/src/django_oscar_pg_search.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,12 +18,16 @@
 src/oscar_pg_search/filter_options/__init__.py
 src/oscar_pg_search/filter_options/attribute_fields.py
 src/oscar_pg_search/filter_options/base_fields.py
 src/oscar_pg_search/filter_options/base_form.py
 src/oscar_pg_search/filter_options/filter_forms.py
 src/oscar_pg_search/filter_options/offer_fields.py
 src/oscar_pg_search/filter_options/product_fields.py
+src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/filter_forms.html
+src/oscar_pg_search/templates/oscar_pg_search/partials/search.html
+src/oscar_pg_search/templatetags/__init__.py
+src/oscar_pg_search/templatetags/oscar_pg_search.py
 tests/__init__.py
 tests/manage.py
 tests/settings.py
 tests/test_search_handler.py
 tests/urls.py
```

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/apps.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/attribute_fields.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/attribute_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/base_fields.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/base_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/filter_forms.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/filter_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         if field.get_range_products().exists():
             return {'offer_only': field}
         return {}
 
     @property
     def enabled_attributes(self):
         qs = ProductAttribute.objects.all()
-        if ProductAttribute._meta.get_field('filter_enabled'):
+        if hasattr(ProductAttribute, 'filter_enabled'):
             qs = qs.filter(filter_enabled=True)
         codes = qs.values_list('code', flat=True)
         return {x for x in codes if x not in self.disabled_fields}
 
     def get_attribute_fields(self):
         """
         :returns: MultipleChoiceAttributeField for dynamic attribute values
```

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/offer_fields.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/offer_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/product_fields.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/filter_options/product_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/forms.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/mixins.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/mixins.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 from django.conf import settings
-from oscar.apps.search.signals import user_search
 from django.utils.module_loading import import_string
+from django.shortcuts import redirect
+from oscar.apps.search.signals import user_search
 from .forms import SearchForm, OrderForm
 
 
 class SearchViewMixin:
     """
     This should be included in all sites with sort functionality
     Most likely this would be CatalogueView and ProductCategoryView
     """
 
     template_name = 'oscar/catalogue/browse.html'
     search_signal = user_search
     form_class = SearchForm
-    http_method_names = ['get', ]
+    http_method_names = ['get', 'post']
     results_per_page = settings.OSCAR_PRODUCTS_PER_PAGE
 
+    def dispatch1(self, request, *args, **kwargs):
+        return redirect(request)
+
+    def post(self, request, *args, **kwargs):
+        request_post = request.POST.copy()
+        del request_post['csrfmiddlewaretoken']
+        if 'q' in request.GET:
+            request_post['q'] = request.GET['q']
+        return redirect(f'{request.path}?{request_post.urlencode()}')
+
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context['order_form'] = OrderForm(
             self.request.GET,
             request=self.request,
         )
         context['summary'] = 'Suchergebnisse'
```

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/order_by_options.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/order_by_options.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/postgres_search_handler.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/postgres_search_handler.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/src/oscar_pg_search/utils.py` & `django-oscar-pg-search-0.9.1/src/oscar_pg_search/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/tests/manage.py` & `django-oscar-pg-search-0.9.1/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.0/tests/settings.py` & `django-oscar-pg-search-0.9.1/tests/settings.py`

 * *Files identical despite different names*

