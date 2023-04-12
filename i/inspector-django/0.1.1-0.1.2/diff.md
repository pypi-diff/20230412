# Comparing `tmp/inspector-django-0.1.1.tar.gz` & `tmp/inspector-django-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspector-django-0.1.1.tar", last modified: Thu Mar 23 09:57:56 2023, max compression
+gzip compressed data, was "inspector-django-0.1.2.tar", last modified: Wed Apr 12 08:19:45 2023, max compression
```

## Comparing `inspector-django-0.1.1.tar` & `inspector-django-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:57:56.314945 inspector-django-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-23 09:57:45.000000 inspector-django-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-23 09:57:56.314945 inspector-django-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-23 09:57:45.000000 inspector-django-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 09:57:56.314945 inspector-django-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-23 09:57:45.000000 inspector-django-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:57:56.310945 inspector-django-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:57:56.310945 inspector-django-0.1.1/src/inspector_django/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:57:56.314945 inspector-django-0.1.1/src/inspector_django/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/enums/settings_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:57:56.314945 inspector-django-0.1.1/src/inspector_django/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/lib/app_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/lib/inspector_django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:57:56.314945 inspector-django-0.1.1/src/inspector_django/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/tracking/guard_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-23 09:57:45.000000 inspector-django-0.1.1/src/inspector_django/tracking/sql_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:57:56.314945 inspector-django-0.1.1/src/inspector_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-23 09:57:56.000000 inspector-django-0.1.1/src/inspector_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-23 09:57:56.000000 inspector-django-0.1.1/src/inspector_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 09:57:56.000000 inspector-django-0.1.1/src/inspector_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 09:57:56.000000 inspector-django-0.1.1/src/inspector_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-23 09:57:56.000000 inspector-django-0.1.1/src/inspector_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 09:57:56.000000 inspector-django-0.1.1/src/inspector_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 08:19:35.000000 inspector-django-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 08:19:45.629798 inspector-django-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 08:19:35.000000 inspector-django-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:19:45.629798 inspector-django-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 08:19:35.000000 inspector-django-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/enums/settings_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/lib/app_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/lib/inspector_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/tracking/guard_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/tracking/sql_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/top_level.txt
```

### Comparing `inspector-django-0.1.1/LICENSE` & `inspector-django-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.1/PKG-INFO` & `inspector-django-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspector-django
-Version: 0.1.1
+Version: 0.1.2
 Summary: Real-time Code Execution Monitoring of your Django applications.
 Home-page: https://inspector.dev/
 Author: Inspector
 Author-email: support@inspector.dev
 License: MIT
 Project-URL: Documentation, https://docs.inspector.dev/guides/django/
 Project-URL: Source Code, https://github.com/inspector-apm/inspector-django
@@ -19,41 +19,42 @@
 
 ## Requirements
 
 - Python >= 3.x
 - Django >= 3.x
 
 ## Install
-Install the latest version of the package from PyPI:
+Install the latest version of the package from [PyPI](https://pypi.org/project/inspector-django/):
 
 ```shell
 pip install inspector-django
 ```
 
 ## Configure the Ingestion Key
-In settings.py add the ingestion key of your project:
+In `settings.py` add the ingestion key of your project:
 
 ```python
 INSPECTOR_INGESTION_KEY = "xxxxxxxxx"
 ```
 
 ### Get a new Ingestion Key
 You can get a new key creating a new project in your [Inspector dashboard](https://app.inspector.dev).
 
 ## Activate the module
 Add `inspector_django` to installed apps:
+
 ```python
 INSTALLED_APPS = [
     ....,
  	
     'inspector_django',
 ]
 ```
 
-## Attach the middleware
+## Register the middleware
 To monitor the incoming HTTP traffic you need to register the middleware. 
 
 We suggest to add the middleware at the top of the list:
 
 ```python
 MIDDLEWARE = [
 	'inspector_django.InspectorMiddleware',
```

### Comparing `inspector-django-0.1.1/README.md` & `inspector-django-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,41 +4,42 @@
 
 ## Requirements
 
 - Python >= 3.x
 - Django >= 3.x
 
 ## Install
-Install the latest version of the package from PyPI:
+Install the latest version of the package from [PyPI](https://pypi.org/project/inspector-django/):
 
 ```shell
 pip install inspector-django
 ```
 
 ## Configure the Ingestion Key
-In settings.py add the ingestion key of your project:
+In `settings.py` add the ingestion key of your project:
 
 ```python
 INSPECTOR_INGESTION_KEY = "xxxxxxxxx"
 ```
 
 ### Get a new Ingestion Key
 You can get a new key creating a new project in your [Inspector dashboard](https://app.inspector.dev).
 
 ## Activate the module
 Add `inspector_django` to installed apps:
+
 ```python
 INSTALLED_APPS = [
     ....,
  	
     'inspector_django',
 ]
 ```
 
-## Attach the middleware
+## Register the middleware
 To monitor the incoming HTTP traffic you need to register the middleware. 
 
 We suggest to add the middleware at the top of the list:
 
 ```python
 MIDDLEWARE = [
 	'inspector_django.InspectorMiddleware',
```

### Comparing `inspector-django-0.1.1/setup.py` & `inspector-django-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='inspector-django',
-    version='0.1.1',
+    version='0.1.2',
     description='Real-time Code Execution Monitoring of your Django applications.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Inspector',
     author_email='support@inspector.dev',
     url='https://inspector.dev/',
     install_requires=[
```

### Comparing `inspector-django-0.1.1/src/inspector_django/__init__.py` & `inspector-django-0.1.2/src/inspector_django/__init__.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.1/src/inspector_django/lib/app_configurations.py` & `inspector-django-0.1.2/src/inspector_django/lib/app_configurations.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.1/src/inspector_django/lib/inspector_django.py` & `inspector-django-0.1.2/src/inspector_django/lib/inspector_django.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.1/src/inspector_django/middleware.py` & `inspector-django-0.1.2/src/inspector_django/middleware.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.1/src/inspector_django/tracking/guard_transaction.py` & `inspector-django-0.1.2/src/inspector_django/tracking/guard_transaction.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.1/src/inspector_django/tracking/sql_hook.py` & `inspector-django-0.1.2/src/inspector_django/tracking/sql_hook.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.1/src/inspector_django.egg-info/PKG-INFO` & `inspector-django-0.1.2/src/inspector_django.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspector-django
-Version: 0.1.1
+Version: 0.1.2
 Summary: Real-time Code Execution Monitoring of your Django applications.
 Home-page: https://inspector.dev/
 Author: Inspector
 Author-email: support@inspector.dev
 License: MIT
 Project-URL: Documentation, https://docs.inspector.dev/guides/django/
 Project-URL: Source Code, https://github.com/inspector-apm/inspector-django
@@ -19,41 +19,42 @@
 
 ## Requirements
 
 - Python >= 3.x
 - Django >= 3.x
 
 ## Install
-Install the latest version of the package from PyPI:
+Install the latest version of the package from [PyPI](https://pypi.org/project/inspector-django/):
 
 ```shell
 pip install inspector-django
 ```
 
 ## Configure the Ingestion Key
-In settings.py add the ingestion key of your project:
+In `settings.py` add the ingestion key of your project:
 
 ```python
 INSPECTOR_INGESTION_KEY = "xxxxxxxxx"
 ```
 
 ### Get a new Ingestion Key
 You can get a new key creating a new project in your [Inspector dashboard](https://app.inspector.dev).
 
 ## Activate the module
 Add `inspector_django` to installed apps:
+
 ```python
 INSTALLED_APPS = [
     ....,
  	
     'inspector_django',
 ]
 ```
 
-## Attach the middleware
+## Register the middleware
 To monitor the incoming HTTP traffic you need to register the middleware. 
 
 We suggest to add the middleware at the top of the list:
 
 ```python
 MIDDLEWARE = [
 	'inspector_django.InspectorMiddleware',
```

### Comparing `inspector-django-0.1.1/src/inspector_django.egg-info/SOURCES.txt` & `inspector-django-0.1.2/src/inspector_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

