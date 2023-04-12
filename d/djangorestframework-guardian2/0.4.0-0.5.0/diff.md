# Comparing `tmp/djangorestframework-guardian2-0.4.0.tar.gz` & `tmp/djangorestframework-guardian2-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-guardian2-0.4.0.tar", last modified: Wed Dec 28 18:56:48 2022, max compression
+gzip compressed data, was "djangorestframework-guardian2-0.5.0.tar", last modified: Wed Apr 12 12:54:17 2023, max compression
```

## Comparing `djangorestframework-guardian2-0.4.0.tar` & `djangorestframework-guardian2-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-12-28 18:56:48.172165 djangorestframework-guardian2-0.4.0/
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-12-28 18:56:48.158679 djangorestframework-guardian2-0.4.0/.github/
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-12-28 18:56:48.164397 djangorestframework-guardian2-0.4.0/.github/workflows/
--rw-r--r--   0 hagenjt1   (501) staff       (20)      573 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.4.0/.github/workflows/python.yml
--rw-r--r--   0 hagenjt1   (501) staff       (20)     1220 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.4.0/.gitignore
--rw-r--r--   0 hagenjt1   (501) staff       (20)      896 2022-12-28 18:56:05.000000 djangorestframework-guardian2-0.4.0/CHANGELOG
--rw-r--r--   0 hagenjt1   (501) staff       (20)     1512 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/LICENSE
--rw-r--r--   0 hagenjt1   (501) staff       (20)       61 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/MANIFEST.in
--rw-r--r--   0 hagenjt1   (501) staff       (20)     7436 2022-12-28 18:56:48.172324 djangorestframework-guardian2-0.4.0/PKG-INFO
--rw-r--r--   0 hagenjt1   (501) staff       (20)     4621 2022-12-28 18:56:05.000000 djangorestframework-guardian2-0.4.0/README.md
--rw-r--r--   0 hagenjt1   (501) staff       (20)      544 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/manage.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)       81 2022-12-28 18:56:05.000000 djangorestframework-guardian2-0.4.0/pyproject.toml
--rw-r--r--   0 hagenjt1   (501) staff       (20)     1715 2022-12-28 18:56:48.173253 djangorestframework-guardian2-0.4.0/setup.cfg
--rw-r--r--   0 hagenjt1   (501) staff       (20)       39 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/setup.py
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-12-28 18:56:48.159359 djangorestframework-guardian2-0.4.0/src/
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-12-28 18:56:48.167457 djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/
--rw-r--r--   0 hagenjt1   (501) staff       (20)     7436 2022-12-28 18:56:48.000000 djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/PKG-INFO
--rw-r--r--   0 hagenjt1   (501) staff       (20)      712 2022-12-28 18:56:48.000000 djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/SOURCES.txt
--rw-r--r--   0 hagenjt1   (501) staff       (20)        1 2022-12-28 18:56:48.000000 djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/dependency_links.txt
--rw-r--r--   0 hagenjt1   (501) staff       (20)        1 2022-12-28 18:41:32.000000 djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/not-zip-safe
--rw-r--r--   0 hagenjt1   (501) staff       (20)       43 2022-12-28 18:56:48.000000 djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/requires.txt
--rw-r--r--   0 hagenjt1   (501) staff       (20)       24 2022-12-28 18:56:48.000000 djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/top_level.txt
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-12-28 18:56:48.169034 djangorestframework-guardian2-0.4.0/src/rest_framework_guardian/
--rw-r--r--   0 hagenjt1   (501) staff       (20)        0 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/src/rest_framework_guardian/__init__.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)     1399 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/src/rest_framework_guardian/filters.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)     2193 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/src/rest_framework_guardian/serializers.py
-drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2022-12-28 18:56:48.171774 djangorestframework-guardian2-0.4.0/tests/
--rw-r--r--   0 hagenjt1   (501) staff       (20)        0 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/tests/__init__.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)      323 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.4.0/tests/models.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)      944 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/tests/settings.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)     5631 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/tests/test_permissions.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)     3867 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.4.0/tests/test_serializers.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)      309 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.4.0/tests/utils.py
--rw-r--r--   0 hagenjt1   (501) staff       (20)     1016 2022-12-28 18:56:05.000000 djangorestframework-guardian2-0.4.0/tox.ini
+drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2023-04-12 12:54:17.511983 djangorestframework-guardian2-0.5.0/
+drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2023-04-12 12:54:17.499255 djangorestframework-guardian2-0.5.0/.github/
+drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2023-04-12 12:54:17.505186 djangorestframework-guardian2-0.5.0/.github/workflows/
+-rw-r--r--   0 hagenjt1   (501) staff       (20)      573 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.5.0/.github/workflows/python.yml
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     1220 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.5.0/.gitignore
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     1045 2023-04-12 12:49:39.000000 djangorestframework-guardian2-0.5.0/CHANGELOG
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     1512 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/LICENSE
+-rw-r--r--   0 hagenjt1   (501) staff       (20)       61 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/MANIFEST.in
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     7462 2023-04-12 12:54:17.512136 djangorestframework-guardian2-0.5.0/PKG-INFO
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     4644 2023-04-12 12:39:02.000000 djangorestframework-guardian2-0.5.0/README.md
+-rw-r--r--   0 hagenjt1   (501) staff       (20)      544 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/manage.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)       81 2022-12-28 18:56:05.000000 djangorestframework-guardian2-0.5.0/pyproject.toml
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     1736 2023-04-12 12:54:17.513274 djangorestframework-guardian2-0.5.0/setup.cfg
+-rw-r--r--   0 hagenjt1   (501) staff       (20)       39 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/setup.py
+drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2023-04-12 12:54:17.500318 djangorestframework-guardian2-0.5.0/src/
+drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2023-04-12 12:54:17.507979 djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     7462 2023-04-12 12:54:17.000000 djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/PKG-INFO
+-rw-r--r--   0 hagenjt1   (501) staff       (20)      712 2023-04-12 12:54:17.000000 djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/SOURCES.txt
+-rw-r--r--   0 hagenjt1   (501) staff       (20)        1 2023-04-12 12:54:17.000000 djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/dependency_links.txt
+-rw-r--r--   0 hagenjt1   (501) staff       (20)        1 2022-12-28 18:41:32.000000 djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/not-zip-safe
+-rw-r--r--   0 hagenjt1   (501) staff       (20)       61 2023-04-12 12:54:17.000000 djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/requires.txt
+-rw-r--r--   0 hagenjt1   (501) staff       (20)       24 2023-04-12 12:54:17.000000 djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/top_level.txt
+drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2023-04-12 12:54:17.509159 djangorestframework-guardian2-0.5.0/src/rest_framework_guardian/
+-rw-r--r--   0 hagenjt1   (501) staff       (20)        0 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/src/rest_framework_guardian/__init__.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     1399 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/src/rest_framework_guardian/filters.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     2193 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/src/rest_framework_guardian/serializers.py
+drwxr-xr-x   0 hagenjt1   (501) staff       (20)        0 2023-04-12 12:54:17.511637 djangorestframework-guardian2-0.5.0/tests/
+-rw-r--r--   0 hagenjt1   (501) staff       (20)        0 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/tests/__init__.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)      323 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.5.0/tests/models.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)      944 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/tests/settings.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     5631 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/tests/test_permissions.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     3867 2022-12-28 18:21:00.000000 djangorestframework-guardian2-0.5.0/tests/test_serializers.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)      309 2022-12-28 17:38:00.000000 djangorestframework-guardian2-0.5.0/tests/utils.py
+-rw-r--r--   0 hagenjt1   (501) staff       (20)     1021 2023-04-12 12:48:45.000000 djangorestframework-guardian2-0.5.0/tox.ini
```

### Comparing `djangorestframework-guardian2-0.4.0/.github/workflows/python.yml` & `djangorestframework-guardian2-0.5.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/.gitignore` & `djangorestframework-guardian2-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/CHANGELOG` & `djangorestframework-guardian2-0.5.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-Unreleased
-==========
+0.5.0 (2023-04-12)
+==================
+
+- Update GitHub project name.
+- Add support for Django 4.2.
+- Drop support for Django 4.0.
+- Add minimum versions for dependencies.
 
 0.4.0 (2022-12-28)
 ==================
 
 - Drop support for Python 3.5 and 3.6.
 - Add support for Python 3.9, 3.10, and 3.11.
 - Drop support for Django 2.1, 2.2, and 3.0.
```

### Comparing `djangorestframework-guardian2-0.4.0/LICENSE` & `djangorestframework-guardian2-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/PKG-INFO` & `djangorestframework-guardian2-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: djangorestframework-guardian2
-Version: 0.4.0
+Version: 0.5.0
 Summary: django-guardian support for Django REST Framework
-Home-page: https://github.com/johnthagen/django-rest-framework-guardian
+Home-page: https://github.com/johnthagen/django-rest-framework-guardian2
 Author: Ryan P Kilby
 Author-email: kilbyr@gmail.com
 License: BSD
-Project-URL: Source, https://github.com/johnthagen/django-rest-framework-guardian
-Project-URL: Tracker, https://github.com/johnthagen/django-rest-framework-guardian/issues
+Project-URL: Source, https://github.com/johnthagen/django-rest-framework-guardian2
+Project-URL: Tracker, https://github.com/johnthagen/django-rest-framework-guardian2/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,20 +27,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-rest-framework-guardian2
 
-[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/python-blueprint/actions)
+[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/django-rest-framework-guardian2/actions)
 [![License](https://img.shields.io/pypi/l/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2)
 [![Version](https://img.shields.io/pypi/v/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2)
 [![Python](https://img.shields.io/pypi/pyversions/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2/)
 
-[github-actions-badge]: https://github.com/johnthagen/django-rest-framework-guardian/workflows/python/badge.svg
+[github-actions-badge]: https://github.com/johnthagen/django-rest-framework-guardian2/workflows/python/badge.svg
 
 django-rest-framework-guardian2 provides django-guardian integrations for Django REST Framework.
 
 
 ## Installation & Setup
 
 To use django-rest-framework-guardian2, install it into your environment.
@@ -156,24 +156,24 @@
 ## Release Process
 
 - Update changelog
 - Update package version in setup.cfg
 - Create git tag for version
 - Build & upload release to PyPI
   ```bash
-  $ pip install -U build
   $ rm -rf dist/ build/
+  $ pip install -U build twine
   $ python -m build
   $ twine upload -r test dist/*
   $ twine upload dist/*
   ```
 
 ## License
 
-See: [LICENSE](https://github.com/johnthagen/django-rest-framework-guardian/blob/master/LICENSE)
+See: [LICENSE](https://github.com/johnthagen/django-rest-framework-guardian2/blob/master/LICENSE)
 
 BSD 3-Clause License
 
 Copyright (c) 2018, Ryan P Kilby
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `djangorestframework-guardian2-0.4.0/README.md` & `djangorestframework-guardian2-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # django-rest-framework-guardian2
 
-[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/python-blueprint/actions)
+[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/django-rest-framework-guardian2/actions)
 [![License](https://img.shields.io/pypi/l/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2)
 [![Version](https://img.shields.io/pypi/v/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2)
 [![Python](https://img.shields.io/pypi/pyversions/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2/)
 
-[github-actions-badge]: https://github.com/johnthagen/django-rest-framework-guardian/workflows/python/badge.svg
+[github-actions-badge]: https://github.com/johnthagen/django-rest-framework-guardian2/workflows/python/badge.svg
 
 django-rest-framework-guardian2 provides django-guardian integrations for Django REST Framework.
 
 
 ## Installation & Setup
 
 To use django-rest-framework-guardian2, install it into your environment.
@@ -125,17 +125,17 @@
 ## Release Process
 
 - Update changelog
 - Update package version in setup.cfg
 - Create git tag for version
 - Build & upload release to PyPI
   ```bash
-  $ pip install -U build
   $ rm -rf dist/ build/
+  $ pip install -U build twine
   $ python -m build
   $ twine upload -r test dist/*
   $ twine upload dist/*
   ```
 
 ## License
 
-See: [LICENSE](https://github.com/johnthagen/django-rest-framework-guardian/blob/master/LICENSE)
+See: [LICENSE](https://github.com/johnthagen/django-rest-framework-guardian2/blob/master/LICENSE)
```

### Comparing `djangorestframework-guardian2-0.4.0/manage.py` & `djangorestframework-guardian2-0.5.0/manage.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/setup.cfg` & `djangorestframework-guardian2-0.5.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 lines_after_imports = 2
 multi_line_output = 4
 known_third_party = django,rest_framework
 known_first_party = rest_framework_guardian,tests
 
 [metadata]
 name = djangorestframework-guardian2
-version = 0.4.0
+version = 0.5.0
 description = django-guardian support for Django REST Framework
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 license = BSD
 license_files = 
 	LICENSE
 author = Ryan P Kilby
 author_email = kilbyr@gmail.com
-url = https://github.com/johnthagen/django-rest-framework-guardian
+url = https://github.com/johnthagen/django-rest-framework-guardian2
 project_urls = 
-	Source=https://github.com/johnthagen/django-rest-framework-guardian
-	Tracker=https://github.com/johnthagen/django-rest-framework-guardian/issues
+	Source=https://github.com/johnthagen/django-rest-framework-guardian2
+	Tracker=https://github.com/johnthagen/django-rest-framework-guardian2/issues
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
@@ -50,17 +50,17 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 
 [options]
 python_requires = >=3.7
 install_requires = 
-	django
-	djangorestframework
-	django-guardian
+	django>=3.2
+	djangorestframework>=3.12
+	django-guardian>=2.4.0
 include_package_data = true
 package_dir = 
 	=src
 packages = find:
 zip_safe = false
 
 [options.packages.find]
```

### Comparing `djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/PKG-INFO` & `djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: djangorestframework-guardian2
-Version: 0.4.0
+Version: 0.5.0
 Summary: django-guardian support for Django REST Framework
-Home-page: https://github.com/johnthagen/django-rest-framework-guardian
+Home-page: https://github.com/johnthagen/django-rest-framework-guardian2
 Author: Ryan P Kilby
 Author-email: kilbyr@gmail.com
 License: BSD
-Project-URL: Source, https://github.com/johnthagen/django-rest-framework-guardian
-Project-URL: Tracker, https://github.com/johnthagen/django-rest-framework-guardian/issues
+Project-URL: Source, https://github.com/johnthagen/django-rest-framework-guardian2
+Project-URL: Tracker, https://github.com/johnthagen/django-rest-framework-guardian2/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,20 +27,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-rest-framework-guardian2
 
-[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/python-blueprint/actions)
+[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/django-rest-framework-guardian2/actions)
 [![License](https://img.shields.io/pypi/l/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2)
 [![Version](https://img.shields.io/pypi/v/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2)
 [![Python](https://img.shields.io/pypi/pyversions/djangorestframework-guardian2.svg)](https://pypi.org/project/djangorestframework-guardian2/)
 
-[github-actions-badge]: https://github.com/johnthagen/django-rest-framework-guardian/workflows/python/badge.svg
+[github-actions-badge]: https://github.com/johnthagen/django-rest-framework-guardian2/workflows/python/badge.svg
 
 django-rest-framework-guardian2 provides django-guardian integrations for Django REST Framework.
 
 
 ## Installation & Setup
 
 To use django-rest-framework-guardian2, install it into your environment.
@@ -156,24 +156,24 @@
 ## Release Process
 
 - Update changelog
 - Update package version in setup.cfg
 - Create git tag for version
 - Build & upload release to PyPI
   ```bash
-  $ pip install -U build
   $ rm -rf dist/ build/
+  $ pip install -U build twine
   $ python -m build
   $ twine upload -r test dist/*
   $ twine upload dist/*
   ```
 
 ## License
 
-See: [LICENSE](https://github.com/johnthagen/django-rest-framework-guardian/blob/master/LICENSE)
+See: [LICENSE](https://github.com/johnthagen/django-rest-framework-guardian2/blob/master/LICENSE)
 
 BSD 3-Clause License
 
 Copyright (c) 2018, Ryan P Kilby
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `djangorestframework-guardian2-0.4.0/src/djangorestframework_guardian2.egg-info/SOURCES.txt` & `djangorestframework-guardian2-0.5.0/src/djangorestframework_guardian2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/src/rest_framework_guardian/filters.py` & `djangorestframework-guardian2-0.5.0/src/rest_framework_guardian/filters.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/src/rest_framework_guardian/serializers.py` & `djangorestframework-guardian2-0.5.0/src/rest_framework_guardian/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/tests/settings.py` & `djangorestframework-guardian2-0.5.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/tests/test_permissions.py` & `djangorestframework-guardian2-0.5.0/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/tests/test_serializers.py` & `djangorestframework-guardian2-0.5.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-guardian2-0.4.0/tox.ini` & `djangorestframework-guardian2-0.5.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -5,31 +5,31 @@
     3.9: py39
     3.10: py310
     3.11: py311
 
 [tox]
 envlist =
         py37-django32
-        py38-django{32,40,41}
-        py39-django{32,40,41}
-        py310-django{32,40,41}
-        py311-django41
+        py38-django{32,41,42}
+        py39-django{32,41,42}
+        py310-django{32,41,42}
+        py311-django{41,42}
         dist,isort,lint,readme
 
 [testenv]
 commands = coverage run manage.py test {posargs: --no-input -v 2}
 usedevelop = True
 envdir={toxworkdir}/v/{envname}
 setenv =
     PYTHONDONTWRITEBYTECODE = 1
 deps =
     coverage
     django32: Django~=3.2
-    django40: Django~=4.0
     django41: Django~=4.1
+    django42: Django~=4.2
 
 [testenv:dist]
 commands = python manage.py test {posargs: --no-input -v 2}
 usedevelop = False
 
 [testenv:isort]
 commands = isort --check-only --recursive src tests {posargs:--diff}
```

