# Comparing `tmp/sphinxcontrib-django-2.2.tar.gz` & `tmp/sphinxcontrib-django-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-django-2.2.tar", last modified: Wed Mar  1 22:48:13 2023, max compression
+gzip compressed data, was "sphinxcontrib-django-2.3.tar", last modified: Wed Apr 12 13:50:46 2023, max compression
```

## Comparing `sphinxcontrib-django-2.2.tar` & `sphinxcontrib-django-2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:48:13.237873 sphinxcontrib-django-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-03-01 22:48:13.237873 sphinxcontrib-django-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 22:48:13.237873 sphinxcontrib-django-2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:48:13.233873 sphinxcontrib-django-2.2/sphinxcontrib_django/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:48:13.237873 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/field_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/sphinxcontrib_django/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:48:13.233873 sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-03-01 22:48:13.000000 sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-01 22:48:13.000000 sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 22:48:13.000000 sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-01 22:48:13.000000 sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-01 22:48:13.000000 sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:48:13.237873 sphinxcontrib-django-2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_attribute_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_autodoc_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_class_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_data_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_django_configured.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_django_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_method_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-01 22:48:00.000000 sphinxcontrib-django-2.2/tests/test_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.552496 sphinxcontrib-django-2.3/sphinxcontrib_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.552496 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/field_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.552496 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_attribute_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_autodoc_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_class_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_data_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_django_configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_django_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_method_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_roles.py
```

### Comparing `sphinxcontrib-django-2.2/LICENSE` & `sphinxcontrib-django-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/PKG-INFO` & `sphinxcontrib-django-2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-django
-Version: 2.2
+Version: 2.3
 Summary: Improve the Sphinx autodoc for Django classes.
 Author-email: Diederik van der Boor <opensource@edoburu.nl>, Timo Ludwig <ti.ludwig@web.de>
 License: Apache2 2.0 License
 Project-URL: Bug Tracker, https://github.com/edoburu/sphinxcontrib-django/issues
 Project-URL: Documentation, https://sphinxcontrib-django.readthedocs.io/
 Project-URL: Release Notes, https://github.com/edoburu/sphinxcontrib-django/blob/main/CHANGES.rst
 Project-URL: Source Code, https://github.com/edoburu/sphinxcontrib-django
 Keywords: django,docstrings,extension,sphinx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `sphinxcontrib-django-2.2/README.rst` & `sphinxcontrib-django-2.3/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/pyproject.toml` & `sphinxcontrib-django-2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,33 +7,33 @@
         { name = "Diederik van der Boor", email = "opensource@edoburu.nl" },
         { name = "Timo Ludwig", email = "ti.ludwig@web.de" }
     ]
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Framework :: Django",
         "Framework :: Sphinx :: Extension",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
-    dependencies = ["Django>=2.2", "Sphinx>=0.5", "pprintpp"]
+    dependencies = ["Django>=3.2", "Sphinx>=0.5", "pprintpp"]
     description = "Improve the Sphinx autodoc for Django classes."
     dynamic = ["version"]
     keywords = ["django", "docstrings", "extension", "sphinx"]
     license = { text = "Apache2 2.0 License" }
     name = "sphinxcontrib-django"
     readme = "README.rst"
     requires-python = ">=3.7"
```

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/__init__.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This is a sphinx extension which improves the documentation of Django apps.
 """
-__version__ = "2.2"
+__version__ = "2.3"
 
 from . import docstrings, roles
 
 
 def setup(app):
     """
     Allow this module to be used as sphinx extension.
```

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/__init__.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/attributes.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/attributes.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/classes.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/classes.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/config.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/config.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/data.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/data.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/field_utils.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/field_utils.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/methods.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/methods.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/docstrings/patches.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/patches.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django/roles.py` & `sphinxcontrib-django-2.3/sphinxcontrib_django/roles.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/PKG-INFO` & `sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-django
-Version: 2.2
+Version: 2.3
 Summary: Improve the Sphinx autodoc for Django classes.
 Author-email: Diederik van der Boor <opensource@edoburu.nl>, Timo Ludwig <ti.ludwig@web.de>
 License: Apache2 2.0 License
 Project-URL: Bug Tracker, https://github.com/edoburu/sphinxcontrib-django/issues
 Project-URL: Documentation, https://sphinxcontrib-django.readthedocs.io/
 Project-URL: Release Notes, https://github.com/edoburu/sphinxcontrib-django/blob/main/CHANGES.rst
 Project-URL: Source Code, https://github.com/edoburu/sphinxcontrib-django
 Keywords: django,docstrings,extension,sphinx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `sphinxcontrib-django-2.2/sphinxcontrib_django.egg-info/SOURCES.txt` & `sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/tests/test_attribute_docstrings.py` & `sphinxcontrib-django-2.3/tests/test_attribute_docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/tests/test_autodoc_skip.py` & `sphinxcontrib-django-2.3/tests/test_autodoc_skip.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/tests/test_class_docstrings.py` & `sphinxcontrib-django-2.3/tests/test_class_docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/tests/test_data_docstrings.py` & `sphinxcontrib-django-2.3/tests/test_data_docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/tests/test_django_configured.py` & `sphinxcontrib-django-2.3/tests/test_django_configured.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/tests/test_django_setup.py` & `sphinxcontrib-django-2.3/tests/test_django_setup.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.2/tests/test_method_docstrings.py` & `sphinxcontrib-django-2.3/tests/test_method_docstrings.py`

 * *Files identical despite different names*

