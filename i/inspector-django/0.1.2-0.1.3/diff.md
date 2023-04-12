# Comparing `tmp/inspector-django-0.1.2.tar.gz` & `tmp/inspector-django-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspector-django-0.1.2.tar", last modified: Wed Apr 12 08:19:45 2023, max compression
+gzip compressed data, was "inspector-django-0.1.3.tar", last modified: Wed Apr 12 08:30:37 2023, max compression
```

## Comparing `inspector-django-0.1.2.tar` & `inspector-django-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 08:19:35.000000 inspector-django-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 08:19:45.629798 inspector-django-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 08:19:35.000000 inspector-django-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:19:45.629798 inspector-django-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 08:19:35.000000 inspector-django-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/enums/settings_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/lib/app_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/lib/inspector_django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/tracking/guard_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-12 08:19:35.000000 inspector-django-0.1.2/src/inspector_django/tracking/sql_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:19:45.629798 inspector-django-0.1.2/src/inspector_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 08:19:45.000000 inspector-django-0.1.2/src/inspector_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:30:37.890040 inspector-django-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 08:30:28.000000 inspector-django-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 08:30:37.890040 inspector-django-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 08:30:28.000000 inspector-django-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:30:37.890040 inspector-django-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 08:30:28.000000 inspector-django-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:30:37.886040 inspector-django-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:30:37.886040 inspector-django-0.1.3/src/inspector_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:30:37.890040 inspector-django-0.1.3/src/inspector_django/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/enums/settings_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:30:37.890040 inspector-django-0.1.3/src/inspector_django/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/lib/app_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/lib/inspector_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:30:37.890040 inspector-django-0.1.3/src/inspector_django/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/tracking/guard_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-12 08:30:28.000000 inspector-django-0.1.3/src/inspector_django/tracking/sql_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:30:37.886040 inspector-django-0.1.3/src/inspector_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 08:30:37.000000 inspector-django-0.1.3/src/inspector_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-12 08:30:37.000000 inspector-django-0.1.3/src/inspector_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:30:37.000000 inspector-django-0.1.3/src/inspector_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:30:37.000000 inspector-django-0.1.3/src/inspector_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 08:30:37.000000 inspector-django-0.1.3/src/inspector_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 08:30:37.000000 inspector-django-0.1.3/src/inspector_django.egg-info/top_level.txt
```

### Comparing `inspector-django-0.1.2/LICENSE` & `inspector-django-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.2/PKG-INFO` & `inspector-django-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspector-django
-Version: 0.1.2
+Version: 0.1.3
 Summary: Real-time Code Execution Monitoring of your Django applications.
 Home-page: https://inspector.dev/
 Author: Inspector
 Author-email: support@inspector.dev
 License: MIT
 Project-URL: Documentation, https://docs.inspector.dev/guides/django/
 Project-URL: Source Code, https://github.com/inspector-apm/inspector-django
```

### Comparing `inspector-django-0.1.2/README.md` & `inspector-django-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.2/setup.py` & `inspector-django-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='inspector-django',
-    version='0.1.2',
+    version='0.1.3',
     description='Real-time Code Execution Monitoring of your Django applications.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Inspector',
     author_email='support@inspector.dev',
     url='https://inspector.dev/',
     install_requires=[
```

### Comparing `inspector-django-0.1.2/src/inspector_django/__init__.py` & `inspector-django-0.1.3/src/inspector_django/__init__.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.2/src/inspector_django/lib/app_configurations.py` & `inspector-django-0.1.3/src/inspector_django/lib/app_configurations.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.2/src/inspector_django/lib/inspector_django.py` & `inspector-django-0.1.3/src/inspector_django/lib/inspector_django.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,13 @@
             "headers": request_data.headers
         }
         return request_transaction
 
     def add_context_response(self, response_data):
         status_code = getattr(response_data, 'status_code', None)
         context_data = {
-            'response': {
-                'status_code': status_code,
-                'template_name': response_data['template_name'] if 'template_name' in response_data else None,
-                'headers': response_data.headers,
-                'cookies': response_data.cookies
-            }
+            'status_code': status_code,
+            'template_name': response_data['template_name'] if 'template_name' in response_data else None,
+            'headers': response_data.headers,
+            'cookies': response_data.cookies
         }
         self.transaction().add_context(self.NAME_RESPONSE_CONTEXT, context_data)
```

### Comparing `inspector-django-0.1.2/src/inspector_django/middleware.py` & `inspector-django-0.1.3/src/inspector_django/middleware.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.2/src/inspector_django/tracking/guard_transaction.py` & `inspector-django-0.1.3/src/inspector_django/tracking/guard_transaction.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.2/src/inspector_django/tracking/sql_hook.py` & `inspector-django-0.1.3/src/inspector_django/tracking/sql_hook.py`

 * *Files identical despite different names*

### Comparing `inspector-django-0.1.2/src/inspector_django.egg-info/PKG-INFO` & `inspector-django-0.1.3/src/inspector_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspector-django
-Version: 0.1.2
+Version: 0.1.3
 Summary: Real-time Code Execution Monitoring of your Django applications.
 Home-page: https://inspector.dev/
 Author: Inspector
 Author-email: support@inspector.dev
 License: MIT
 Project-URL: Documentation, https://docs.inspector.dev/guides/django/
 Project-URL: Source Code, https://github.com/inspector-apm/inspector-django
```

### Comparing `inspector-django-0.1.2/src/inspector_django.egg-info/SOURCES.txt` & `inspector-django-0.1.3/src/inspector_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

