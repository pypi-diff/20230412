# Comparing `tmp/flet_django-0.4.3.tar.gz` & `tmp/flet_django-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_django-0.4.3.tar", max compression
+gzip compressed data, was "flet_django-0.4.4.tar", max compression
```

## Comparing `flet_django-0.4.3.tar` & `flet_django-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1062 2023-01-27 18:19:02.046982 flet_django-0.4.3/LICENSE
--rw-r--r--   0        0        0     4897 2023-03-16 22:22:44.921078 flet_django-0.4.3/README.md
--rw-r--r--   0        0        0     6148 2023-02-10 10:09:43.158866 flet_django-0.4.3/flet_django/.DS_Store
--rw-r--r--   0        0        0      218 2023-03-16 22:22:44.911109 flet_django-0.4.3/flet_django/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 12:39:40.800698 flet_django-0.4.3/flet_django/admin.py
--rw-r--r--   0        0        0      136 2023-01-27 18:31:59.730446 flet_django-0.4.3/flet_django/apps.py
--rw-r--r--   0        0        0      190 2023-01-27 12:39:40.800815 flet_django-0.4.3/flet_django/compat.py
--rw-r--r--   0        0        0       41 2023-01-18 11:02:05.354951 flet_django-0.4.3/flet_django/controls/__init__.py
--rw-r--r--   0        0        0     1065 2023-01-18 11:02:05.355098 flet_django-0.4.3/flet_django/controls/modelform.py
--rw-r--r--   0        0        0     7981 2023-01-18 11:02:05.357789 flet_django-0.4.3/flet_django/controls/modeltable.py
--rw-r--r--   0        0        0        0 2023-01-05 21:02:56.432428 flet_django-0.4.3/flet_django/management/__init__.py
--rw-r--r--   0        0        0        0 2023-01-05 21:02:56.432514 flet_django-0.4.3/flet_django/management/commands/__init__.py
--rw-r--r--   0        0        0     1286 2023-03-12 20:05:32.635368 flet_django-0.4.3/flet_django/management/commands/run_app.py
--rw-r--r--   0        0        0     1550 2023-03-16 17:15:05.276041 flet_django-0.4.3/flet_django/middlewares.py
--rw-r--r--   0        0        0        0 2023-01-27 12:39:40.800836 flet_django-0.4.3/flet_django/models.py
--rw-r--r--   0        0        0     4421 2023-03-16 17:17:47.924174 flet_django-0.4.3/flet_django/navigation.py
--rw-r--r--   0        0        0     6524 2023-03-27 18:22:33.136283 flet_django-0.4.3/flet_django/pages.py
--rw-r--r--   0        0        0      569 2023-01-30 13:39:29.209985 flet_django-0.4.3/flet_django/routes.py
--rw-r--r--   0        0        0        0 2023-01-27 12:39:40.800870 flet_django-0.4.3/flet_django/serializers.py
--rw-r--r--   0        0        0      223 2023-03-16 22:22:44.907503 flet_django-0.4.3/flet_django/types.py
--rw-r--r--   0        0        0       47 2023-03-12 20:05:32.636367 flet_django-0.4.3/flet_django/urls.py
--rw-r--r--   0        0        0     4014 2023-03-16 22:40:39.305904 flet_django-0.4.3/flet_django/views.py
--rw-r--r--   0        0        0     2063 2023-03-29 09:24:16.916991 flet_django-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 flet_django-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-01-27 18:19:02.046982 flet_django-0.4.4/LICENSE
+-rw-r--r--   0        0        0     4897 2023-03-16 22:22:44.921078 flet_django-0.4.4/README.md
+-rw-r--r--   0        0        0     6148 2023-02-10 10:09:43.158866 flet_django-0.4.4/flet_django/.DS_Store
+-rw-r--r--   0        0        0      218 2023-03-16 22:22:44.911109 flet_django-0.4.4/flet_django/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-27 12:39:40.800698 flet_django-0.4.4/flet_django/admin.py
+-rw-r--r--   0        0        0      136 2023-01-27 18:31:59.730446 flet_django-0.4.4/flet_django/apps.py
+-rw-r--r--   0        0        0      190 2023-01-27 12:39:40.800815 flet_django-0.4.4/flet_django/compat.py
+-rw-r--r--   0        0        0       41 2023-01-18 11:02:05.354951 flet_django-0.4.4/flet_django/controls/__init__.py
+-rw-r--r--   0        0        0     1065 2023-01-18 11:02:05.355098 flet_django-0.4.4/flet_django/controls/modelform.py
+-rw-r--r--   0        0        0     7981 2023-01-18 11:02:05.357789 flet_django-0.4.4/flet_django/controls/modeltable.py
+-rw-r--r--   0        0        0        0 2023-01-05 21:02:56.432428 flet_django-0.4.4/flet_django/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-05 21:02:56.432514 flet_django-0.4.4/flet_django/management/commands/__init__.py
+-rw-r--r--   0        0        0     1286 2023-03-12 20:05:32.635368 flet_django-0.4.4/flet_django/management/commands/run_app.py
+-rw-r--r--   0        0        0     1550 2023-03-16 17:15:05.276041 flet_django-0.4.4/flet_django/middlewares.py
+-rw-r--r--   0        0        0        0 2023-01-27 12:39:40.800836 flet_django-0.4.4/flet_django/models.py
+-rw-r--r--   0        0        0     4421 2023-03-16 17:17:47.924174 flet_django-0.4.4/flet_django/navigation.py
+-rw-r--r--   0        0        0     6524 2023-03-27 18:22:33.136283 flet_django-0.4.4/flet_django/pages.py
+-rw-r--r--   0        0        0      569 2023-01-30 13:39:29.209985 flet_django-0.4.4/flet_django/routes.py
+-rw-r--r--   0        0        0        0 2023-01-27 12:39:40.800870 flet_django-0.4.4/flet_django/serializers.py
+-rw-r--r--   0        0        0      223 2023-03-16 22:22:44.907503 flet_django-0.4.4/flet_django/types.py
+-rw-r--r--   0        0        0       47 2023-03-12 20:05:32.636367 flet_django-0.4.4/flet_django/urls.py
+-rw-r--r--   0        0        0     4014 2023-03-16 22:40:39.305904 flet_django-0.4.4/flet_django/views.py
+-rw-r--r--   0        0        0     2061 2023-04-12 16:16:05.868592 flet_django-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 flet_django-0.4.4/PKG-INFO
```

### Comparing `flet_django-0.4.3/LICENSE` & `flet_django-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/README.md` & `flet_django-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/.DS_Store` & `flet_django-0.4.4/flet_django/.DS_Store`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/controls/modelform.py` & `flet_django-0.4.4/flet_django/controls/modelform.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/controls/modeltable.py` & `flet_django-0.4.4/flet_django/controls/modeltable.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/management/commands/run_app.py` & `flet_django-0.4.4/flet_django/management/commands/run_app.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/middlewares.py` & `flet_django-0.4.4/flet_django/middlewares.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/navigation.py` & `flet_django-0.4.4/flet_django/navigation.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/pages.py` & `flet_django-0.4.4/flet_django/pages.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/routes.py` & `flet_django-0.4.4/flet_django/routes.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/flet_django/views.py` & `flet_django-0.4.4/flet_django/views.py`

 * *Files identical despite different names*

### Comparing `flet_django-0.4.3/pyproject.toml` & `flet_django-0.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-django"
-version = "0.4.3"
+version = "0.4.4"
 description = "Django Flutter Framework."
 license = "MIT"
 authors = ["beret <beret@hipisi.org.pl>"]  # Here is a place for You'r name, contributors welcome!
 maintainers = ["Marysia Software Limited <office@marysia.app>"]  # Here is You'r advertising site.
 readme = "README.md"
 homepage = "https://marysia.app"
 repository = "https://github.com/Marysia-Software-Limited/flet-django"
@@ -56,16 +56,16 @@
 
 django-extensions = "*"
 django-rest-framework = "*"
 werkzeug = "*"
 
 
 # for local development only
-#flet-core = {path = "../flet/sdk/python/packages/flet-core", develop = true}
-#flet = {path = "../flet/sdk/python/packages/flet", develop = true}
+flet-core = {path = "../flet/sdk/python/packages/flet-core", develop = true}
+flet = {path = "../flet/sdk/python/packages/flet", develop = true}
 #flet-routed-app = {path = "../flet-routed-app", develop = true}
 #django = {path = "../django", develop = true}
 
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `flet_django-0.4.3/PKG-INFO` & `flet_django-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-django
-Version: 0.4.3
+Version: 0.4.4
 Summary: Django Flutter Framework.
 Home-page: https://marysia.app
 License: MIT
 Author: beret
 Author-email: beret@hipisi.org.pl
 Maintainer: Marysia Software Limited
 Maintainer-email: office@marysia.app
```

