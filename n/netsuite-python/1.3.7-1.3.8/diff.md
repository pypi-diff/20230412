# Comparing `tmp/netsuite_python-1.3.7.tar.gz` & `tmp/netsuite_python-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.3.7.tar", last modified: Wed Apr 12 21:46:54 2023, max compression
+gzip compressed data, was "netsuite_python-1.3.8.tar", last modified: Wed Apr 12 21:53:31 2023, max compression
```

## Comparing `netsuite_python-1.3.7.tar` & `netsuite_python-1.3.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:46:54.791679 netsuite_python-1.3.7/
--rw-rw-rw-   0        0        0    12699 2023-04-12 21:46:54.791679 netsuite_python-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    12368 2023-04-12 21:14:15.000000 netsuite_python-1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 21:46:54.775680 netsuite_python-1.3.7/netsuite/
--rw-rw-rw-   0        0        0    11858 2023-04-12 21:38:42.000000 netsuite_python-1.3.7/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:46:54.778680 netsuite_python-1.3.7/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.7/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:46:54.780680 netsuite_python-1.3.7/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.7/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.7/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.7/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.7/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.7/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.7/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:46:54.782679 netsuite_python-1.3.7/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0     8446 2023-04-12 21:38:54.000000 netsuite_python-1.3.7/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6306 2023-04-12 21:38:42.000000 netsuite_python-1.3.7/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:46:54.785680 netsuite_python-1.3.7/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.7/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:46:54.790679 netsuite_python-1.3.7/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0    12699 2023-04-12 21:46:54.000000 netsuite_python-1.3.7/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-04-12 21:46:54.000000 netsuite_python-1.3.7/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:46:54.000000 netsuite_python-1.3.7/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-12 21:46:54.000000 netsuite_python-1.3.7/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-04-12 21:46:54.000000 netsuite_python-1.3.7/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 21:46:54.000000 netsuite_python-1.3.7/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 21:46:54.791679 netsuite_python-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-04-12 21:46:48.000000 netsuite_python-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.836536 netsuite_python-1.3.8/
+-rw-rw-rw-   0        0        0    12699 2023-04-12 21:53:31.836536 netsuite_python-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12368 2023-04-12 21:14:15.000000 netsuite_python-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.821083 netsuite_python-1.3.8/netsuite/
+-rw-rw-rw-   0        0        0    11858 2023-04-12 21:38:42.000000 netsuite_python-1.3.8/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.823526 netsuite_python-1.3.8/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.8/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.826535 netsuite_python-1.3.8/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.8/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.8/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.8/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.8/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.8/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.8/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.827535 netsuite_python-1.3.8/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0     8422 2023-04-12 21:53:28.000000 netsuite_python-1.3.8/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6306 2023-04-12 21:38:42.000000 netsuite_python-1.3.8/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.830535 netsuite_python-1.3.8/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.835536 netsuite_python-1.3.8/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0    12699 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 21:53:31.836536 netsuite_python-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-04-12 21:53:28.000000 netsuite_python-1.3.8/setup.py
```

### Comparing `netsuite_python-1.3.7/PKG-INFO` & `netsuite_python-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.3.7
+Version: 1.3.8
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.7/README.md` & `netsuite_python-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/Netsuite.py` & `netsuite_python-1.3.8/netsuite/Netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.3.8/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.3.8/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/api_clients/api_client.py` & `netsuite_python-1.3.8/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/api_clients/configuration.py` & `netsuite_python-1.3.8/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/api_clients/rest.py` & `netsuite_python-1.3.8/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/module_loading.py` & `netsuite_python-1.3.8/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/scripts/cli.py` & `netsuite_python-1.3.8/netsuite/scripts/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from click import prompt
 from pathlib import Path
 
 from netsuite.Netsuite import Netsuite
 from netsuite.settings import api_settings, IN_MEMORY_STORAGE, JSON_STORAGE
 from OpenSSL.SSL import FILETYPE_PEM
 from OpenSSL.crypto import (dump_certificate, X509, X509Name, PKey, TYPE_RSA, X509Req, dump_privatekey, X509Extension)
-from rich import print
 
 def link(uri, label=None):
     if label is None:
         label = uri
     parameters = ''
 
     # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
```

### Comparing `netsuite_python-1.3.7/netsuite/settings.py` & `netsuite_python-1.3.8/netsuite/settings.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.3.8/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite/storages/JSONStorage.py` & `netsuite_python-1.3.8/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.3.8/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.3.7
+Version: 1.3.8
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.7/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.3.8/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.7/setup.py` & `netsuite_python-1.3.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.3.7',
+    version='1.3.8',
     description='Python SDK for Netsuite API with Django Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

