# Comparing `tmp/netsuite_python-1.3.3.tar.gz` & `tmp/netsuite_python-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.3.3.tar", last modified: Wed Apr 12 18:24:45 2023, max compression
+gzip compressed data, was "netsuite_python-1.3.4.tar", last modified: Wed Apr 12 18:31:07 2023, max compression
```

## Comparing `netsuite_python-1.3.3.tar` & `netsuite_python-1.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 18:24:45.956967 netsuite_python-1.3.3/
--rw-rw-rw-   0        0        0    11966 2023-04-12 18:24:45.956967 netsuite_python-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    11635 2023-04-09 23:07:01.000000 netsuite_python-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 18:24:45.939968 netsuite_python-1.3.3/netsuite/
--rw-rw-rw-   0        0        0    10514 2023-04-09 23:00:48.000000 netsuite_python-1.3.3/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:24:45.942968 netsuite_python-1.3.3/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.3/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:24:45.945970 netsuite_python-1.3.3/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.3/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.3/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.3/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.3/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.3/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.3/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:24:45.946970 netsuite_python-1.3.3/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0     5751 2023-04-12 18:24:23.000000 netsuite_python-1.3.3/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6016 2023-04-12 18:01:10.000000 netsuite_python-1.3.3/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:24:45.950967 netsuite_python-1.3.3/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.3/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:24:45.954968 netsuite_python-1.3.3/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0    11966 2023-04-12 18:24:45.000000 netsuite_python-1.3.3/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-04-12 18:24:45.000000 netsuite_python-1.3.3/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 18:24:45.000000 netsuite_python-1.3.3/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-12 18:24:45.000000 netsuite_python-1.3.3/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-04-12 18:24:45.000000 netsuite_python-1.3.3/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 18:24:45.000000 netsuite_python-1.3.3/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 18:24:45.956967 netsuite_python-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-12 18:24:43.000000 netsuite_python-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.660480 netsuite_python-1.3.4/
+-rw-rw-rw-   0        0        0    11966 2023-04-12 18:31:07.660480 netsuite_python-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11635 2023-04-09 23:07:01.000000 netsuite_python-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.641479 netsuite_python-1.3.4/netsuite/
+-rw-rw-rw-   0        0        0    10514 2023-04-09 23:00:48.000000 netsuite_python-1.3.4/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.646479 netsuite_python-1.3.4/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.4/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.649477 netsuite_python-1.3.4/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.4/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.4/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.4/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.4/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.4/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.4/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.650478 netsuite_python-1.3.4/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0     5751 2023-04-12 18:24:23.000000 netsuite_python-1.3.4/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6016 2023-04-12 18:30:51.000000 netsuite_python-1.3.4/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.654478 netsuite_python-1.3.4/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.659480 netsuite_python-1.3.4/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0    11966 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 18:31:07.660480 netsuite_python-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-04-12 18:31:02.000000 netsuite_python-1.3.4/setup.py
```

### Comparing `netsuite_python-1.3.3/PKG-INFO` & `netsuite_python-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.3/README.md` & `netsuite_python-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/Netsuite.py` & `netsuite_python-1.3.4/netsuite/Netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.3.4/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.3.4/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/api_clients/api_client.py` & `netsuite_python-1.3.4/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/api_clients/configuration.py` & `netsuite_python-1.3.4/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/api_clients/rest.py` & `netsuite_python-1.3.4/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/module_loading.py` & `netsuite_python-1.3.4/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/scripts/cli.py` & `netsuite_python-1.3.4/netsuite/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/settings.py` & `netsuite_python-1.3.4/netsuite/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     'ALLOW_NONE': False,
     'USE_DATETIME': True,
 
 
 
     'STORAGE_CLASS': 'netsuite.storages.JSONStorage',
     'CREDENTIALS_PATH': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_credentials.json')),
-    'JSON_STORAGE_PATH': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_tokens.json')),
+    'JSON_STORAGE_PATH': str(Path.joinpath(NETSUITE_TOKENS_DIR, 'netsuite_tokens.json')),
     'NETSUITE_CERTIFICATE_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_certificate.pem')),
     'NETSUITE_KEY_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_key.pem')),
     'APP_NAME': 'default',
 }
 
 # List of settings that may be in string import notation.
 IMPORT_STRINGS = [
```

### Comparing `netsuite_python-1.3.3/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.3.4/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite/storages/JSONStorage.py` & `netsuite_python-1.3.4/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.3.4/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.3/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.3.4/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.3/setup.py` & `netsuite_python-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.3.3',
+    version='1.3.4',
     description='Python SDK for Netsuite API with Django Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

