# Comparing `tmp/django_mongoengine_rql-0.1.3.tar.gz` & `tmp/django_mongoengine_rql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mongoengine_rql-0.1.3.tar", max compression
+gzip compressed data, was "django_mongoengine_rql-0.2.0.tar", max compression
```

## Comparing `django_mongoengine_rql-0.1.3.tar` & `django_mongoengine_rql-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    11357 2022-11-21 17:18:47.078550 django_mongoengine_rql-0.1.3/LICENSE
--rw-r--r--   0        0        0     3874 2022-11-21 17:18:47.078550 django_mongoengine_rql-0.1.3/README.md
--rw-r--r--   0        0        0        0 2022-11-21 17:18:47.078550 django_mongoengine_rql-0.1.3/dj_mongoengine_rql/__init__.py
--rw-r--r--   0        0        0      553 2022-11-21 17:18:47.078550 django_mongoengine_rql-0.1.3/dj_mongoengine_rql/constants.py
--rw-r--r--   0        0        0     1655 2022-11-21 17:18:47.078550 django_mongoengine_rql-0.1.3/dj_mongoengine_rql/filter_cls.py
--rw-r--r--   0        0        0      323 2022-11-21 17:18:47.078550 django_mongoengine_rql-0.1.3/dj_mongoengine_rql/q.py
--rw-r--r--   0        0        0     1944 2022-11-21 17:19:49.399047 django_mongoengine_rql-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 django_mongoengine_rql-0.1.3/setup.py
--rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 django_mongoengine_rql-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3874 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/constants.py
+-rw-r--r--   0        0        0     1654 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/filter_cls.py
+-rw-r--r--   0        0        0      322 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/q.py
+-rw-r--r--   0        0        0     1965 2023-04-12 09:07:32.109243 django_mongoengine_rql-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 django_mongoengine_rql-0.2.0/PKG-INFO
```

### Comparing `django_mongoengine_rql-0.1.3/LICENSE` & `django_mongoengine_rql-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.1.3/README.md` & `django_mongoengine_rql-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.1.3/dj_mongoengine_rql/constants.py` & `django_mongoengine_rql-0.2.0/dj_mongoengine_rql/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright © 2022 CloudBlue LLC. All rights reserved.
+#  Copyright © 2022 Ingram Micro. All rights reserved.
 #
 
 from dj_rql.constants import FilterTypes
 from django_mongoengine import fields
 
 
 class MongoengineFilterTypes(FilterTypes):
```

### Comparing `django_mongoengine_rql-0.1.3/dj_mongoengine_rql/filter_cls.py` & `django_mongoengine_rql-0.2.0/dj_mongoengine_rql/filter_cls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright © 2022 CloudBlue LLC. All rights reserved.
+#  Copyright © 2022 Ingram Micro. All rights reserved.
 #
 
 from dj_rql.constants import DjangoLookups
 from dj_rql.filter_cls import RQLFilterClass
 from django_mongoengine.fields.djangoflavor import DjangoField
 from py_rql.constants import FilterLookups
```

### Comparing `django_mongoengine_rql-0.1.3/pyproject.toml` & `django_mongoengine_rql-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "django-mongoengine-rql"
-version = "0.1.3"
+version = "0.2.0"
 description = "Django Mongoengine RQL Filtering"
-authors = ["CloudBlue LLC"]
+authors = ["Ingram Micro"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_mongoengine_rql" }
 ]
 readme = "./README.md"
 homepage = "https://connect.cloudblue.com/community/api/rql/"
 repository = "https://github.com/cloudblue/django-mongoengine-rql"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: Unix",
-    "Framework :: Django :: 3.0",
-    "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Text Processing :: Filters"
 ]
 keywords = [
     "rql",
@@ -34,17 +34,18 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django-rql = "^4.2.0"
 django-mongoengine = "^0.5.4"
 
 [tool.poetry.dev-dependencies]
+mongoengine = "0.26.*"
 mongomock = "^4.1"
-ipython = ">=7.10.0"
-pytest = "^6.1.2"
+ipython = "^7.10.0"
+pytest = "^7.2.0"
 pytest-cov = "^2.10.1"
 pytest-django = "^4.4"
 pytest-mock = "^3.3.1"
 coverage = {extras = ["toml"], version = "^5.3"}
 flake8 = "~3.8"
 flake8-bugbear = "~20"
 flake8-cognitive-complexity = "^0.1"
```

### Comparing `django_mongoengine_rql-0.1.3/PKG-INFO` & `django_mongoengine_rql-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-mongoengine-rql
-Version: 0.1.3
+Version: 0.2.0
 Summary: Django Mongoengine RQL Filtering
 Home-page: https://connect.cloudblue.com/community/api/rql/
 License: Apache-2.0
 Keywords: rql,filter,django,mongo,mongoengine
-Author: CloudBlue LLC
+Author: Ingram Micro
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

