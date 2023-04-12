# Comparing `tmp/netsuite_python-1.3.1.tar.gz` & `tmp/netsuite_python-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.3.1.tar", last modified: Wed Apr 12 17:12:53 2023, max compression
+gzip compressed data, was "netsuite_python-1.3.2.tar", last modified: Wed Apr 12 18:13:04 2023, max compression
```

## Comparing `netsuite_python-1.3.1.tar` & `netsuite_python-1.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 17:12:53.401551 netsuite_python-1.3.1/
--rw-rw-rw-   0        0        0    11966 2023-04-12 17:12:53.401551 netsuite_python-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    11635 2023-04-09 23:07:01.000000 netsuite_python-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 17:12:53.373315 netsuite_python-1.3.1/netsuite/
--rw-rw-rw-   0        0        0    10514 2023-04-09 23:00:48.000000 netsuite_python-1.3.1/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:12:53.380551 netsuite_python-1.3.1/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.1/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:12:53.386551 netsuite_python-1.3.1/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.1/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.1/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.1/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.1/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.1/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.1/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:12:53.388553 netsuite_python-1.3.1/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0     5515 2023-04-12 17:12:31.000000 netsuite_python-1.3.1/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     5387 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:12:53.395552 netsuite_python-1.3.1/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.1/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:12:53.400551 netsuite_python-1.3.1/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0    11966 2023-04-12 17:12:53.000000 netsuite_python-1.3.1/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-04-12 17:12:53.000000 netsuite_python-1.3.1/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 17:12:53.000000 netsuite_python-1.3.1/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-12 17:12:53.000000 netsuite_python-1.3.1/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-04-12 17:12:53.000000 netsuite_python-1.3.1/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 17:12:53.000000 netsuite_python-1.3.1/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 17:12:53.401551 netsuite_python-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-12 17:12:48.000000 netsuite_python-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:13:04.453204 netsuite_python-1.3.2/
+-rw-rw-rw-   0        0        0    11966 2023-04-12 18:13:04.452204 netsuite_python-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11635 2023-04-09 23:07:01.000000 netsuite_python-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 18:13:04.436204 netsuite_python-1.3.2/netsuite/
+-rw-rw-rw-   0        0        0    10514 2023-04-09 23:00:48.000000 netsuite_python-1.3.2/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:13:04.440204 netsuite_python-1.3.2/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.2/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:13:04.442204 netsuite_python-1.3.2/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.2/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.2/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.2/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.2/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.2/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.2/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:13:04.443204 netsuite_python-1.3.2/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0     5734 2023-04-12 18:11:26.000000 netsuite_python-1.3.2/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6016 2023-04-12 18:01:10.000000 netsuite_python-1.3.2/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:13:04.447204 netsuite_python-1.3.2/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.2/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:13:04.451204 netsuite_python-1.3.2/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0    11966 2023-04-12 18:13:04.000000 netsuite_python-1.3.2/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-12 18:13:04.000000 netsuite_python-1.3.2/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 18:13:04.000000 netsuite_python-1.3.2/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-12 18:13:04.000000 netsuite_python-1.3.2/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-04-12 18:13:04.000000 netsuite_python-1.3.2/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 18:13:04.000000 netsuite_python-1.3.2/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 18:13:04.453204 netsuite_python-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-04-12 18:12:59.000000 netsuite_python-1.3.2/setup.py
```

### Comparing `netsuite_python-1.3.1/PKG-INFO` & `netsuite_python-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.1/README.md` & `netsuite_python-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/Netsuite.py` & `netsuite_python-1.3.2/netsuite/Netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.3.2/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.3.2/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/api_clients/api_client.py` & `netsuite_python-1.3.2/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/api_clients/configuration.py` & `netsuite_python-1.3.2/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/api_clients/rest.py` & `netsuite_python-1.3.2/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/module_loading.py` & `netsuite_python-1.3.2/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/scripts/cli.py` & `netsuite_python-1.3.2/netsuite/scripts/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,42 +5,36 @@
 from click import prompt
 from pathlib import Path
 
 from netsuite.Netsuite import Netsuite
 from netsuite.settings import api_settings, IN_MEMORY_STORAGE, JSON_STORAGE
 from OpenSSL.SSL import FILETYPE_PEM
 from OpenSSL.crypto import (dump_certificate, X509, X509Name, PKey, TYPE_RSA, X509Req, dump_privatekey, X509Extension)
-BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.parent.resolve()
-base_config_dir = Path.joinpath(BASE_DIR, 'config')
-netsuite_config_dir = Path.joinpath(base_config_dir, 'netsuite')
+
 @click.group()
 def cli():
     """
     Simple CLI for managing Netsuite API Access
     """
     pass
 
 
 @cli.command()
 def generate_certificate():
 
-    print(BASE_DIR)
+    print(f"BASE DIR: {api_settings.BASE_DIR}")
 
-    if not os.path.exists(netsuite_config_dir):
-        os.makedirs(netsuite_config_dir)
     CN = prompt("Domain", hide_input=False)
     ORG = prompt("Organization", hide_input=False)
     ORG_UNIT = prompt("Department", hide_input=False)
     L = prompt("City", hide_input=False)
     ST = prompt("State", hide_input=False)
     C = prompt("Country", hide_input=False)
     EMAIL = prompt("Email", hide_input=False)
 
-    private_key_file = Path.joinpath(netsuite_config_dir, 'netsuite_key.pem')
-    public_cert_file = Path.joinpath(netsuite_config_dir, 'netsuite_certificate.pem')
 
     key = PKey()
     key.generate_key(TYPE_RSA, 4096)
 
     cert = X509()
 
     subject = cert.get_subject()
@@ -58,19 +52,28 @@
     cert.set_serial_number(int.from_bytes(os.urandom(16), byteorder="big"))
     # cert.set_serial_number(int(rand.bytes(16).encode('hex'), 16))
     cert.gmtime_adj_notBefore(0)
     cert.gmtime_adj_notAfter(31536000)
     cert.set_pubkey(key)
     cert.sign(key, 'sha256')
 
-    with open(public_cert_file, 'wb+') as f:
-        f.write(dump_certificate(FILETYPE_PEM, cert))
-    with open(private_key_file, 'wb+') as f:
+
+    with open(api_settings.NETSUITE_KEY_FILE, 'wb+') as f:
         f.write(dump_privatekey(FILETYPE_PEM, key))
+        print(f"Netsuite Key File Created: {api_settings.NETSUITE_KEY_FILE} \n")
 
+    with open(api_settings.NETSUITE_CERTIFICATE_FILE, 'wb+') as f:
+        f.write(dump_certificate(FILETYPE_PEM, cert))
+        print(f"Netsuite Certificate Created: {api_settings.NETSUITE_CERTIFICATE_FILE} \n")
+        print(f"Steps to upload the certificate")
+        print(f"  1. Login to Netsuite")
+        print(f"  2. On top ribbon, go to Setup -> Integration -> Manage OAuth 2.0 Client Credentials Setup")
+        print(f"  3. Click New")
+        print(f"  4. Associate with your user, the integration record, and upload the netsuite_certificate.pem file from the path above.")
+        print(f"  5. Copy the Certificate ID for when you generate the client config")
 
 @cli.command()
 def generate_client_config():
     client_id = prompt("What is your client id?", hide_input=False)
     cert_id = prompt("What is your Netsuite certificate id?", hide_input=False)
     # client_secret = prompt("What is your client secret?", hide_input=True)
     # redirect_url = prompt("Redirect URL", default=api_settings.REDIRECT_URL)
@@ -88,26 +91,26 @@
         # 'CLIENT_SECRET': client_secret,
         # 'REDIRECT_URL': redirect_url,
         'NETSUITE_APP_NAME': netsuite_app_name,
         'APP_NAME': app_name,
         'ALLOW_NONE': allow_none,
         'USE_DATETIME': use_datetime,
         'STORAGE_CLASS': storage_class,
-        'NETSUITE_KEY_FILE': Path.joinpath(netsuite_config_dir, 'netsuite_key.pem'),
     }
 
     if storage_class == JSON_STORAGE:
         creds['JSON_STORAGE_PATH'] = prompt("Token Storage File", default=api_settings.JSON_STORAGE_PATH,
                                             type=click.Path(readable=True, writable=True))
 
     save_to_file = prompt("Save settings to file?", default='y', type=click.BOOL, show_choices=True)
 
     if save_to_file:
-        file = prompt("Save settings to file?", default=api_settings.CREDENTIALS_PATH, type=click.File("w", ))
-        file.write(json.dumps(creds, indent=4))
+        with open(api_settings.NETSUITE_CREDENTIALS_PATH, 'wb+') as f:
+            f.write(json.dumps(creds, indent=4))
+            print(f"Netsuite Credentials written to: {api_settings.NETSUITE_CREDENTIALS_PATH}")
     else:
         click.echo(creds)
 
     return creds
 
 
 @cli.command()
```

### Comparing `netsuite_python-1.3.1/netsuite/settings.py` & `netsuite_python-1.3.2/netsuite/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 }
 
 This module provides the `api_setting` object, that is used to access
 NETSUITE settings, checking for user settings first, then falling
 back to the defaults.
 """
 from .module_loading import import_string
+from pathlib import Path
+import os
 
 django_imported = False
 try:
     from django.conf import settings
     from django.test.signals import setting_changed
     # from django.utils.module_loading import import_string
     from django.core.exceptions import ImproperlyConfigured
@@ -25,40 +27,52 @@
         getattr(settings, 'NETSUITE', {})
         django_imported = True
     except ImproperlyConfigured as e:
         settings = None
 except ImportError as e:
     settings = None
 
+BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
+BASE_CONFIG_DIR = Path.joinpath(BASE_DIR, 'config')
+NETSUITE_CONFIG_DIR = Path.joinpath(BASE_CONFIG_DIR, 'netsuite')
+NETSUITE_TOKENS_DIR = Path.joinpath(BASE_CONFIG_DIR, 'tokens')
+
+if not os.path.exists(NETSUITE_CONFIG_DIR):
+    os.makedirs(NETSUITE_CONFIG_DIR)
+if not os.path.exists(NETSUITE_TOKENS_DIR):
+    os.makedirs(NETSUITE_TOKENS_DIR)
+
 
 JSON_STORAGE = 'netsuite.storages.JSONStorage'
 IN_MEMORY_STORAGE = 'netsuite.storages.InMemoryStorage'
 DEFAULTS = {
     # Base API policies
     'DEFAULT_STORAGE_CLASSES': [
         JSON_STORAGE,
         IN_MEMORY_STORAGE,
     ],
 
     # API Configuration
     'NETSUITE_APP_NAME': None,
     'CLIENT_ID': None,
-    'NETSUITE_KEY_FILE': './netsuite-key.pem',
+
     'CERT_ID': None,
     # 'CLIENT_SECRET': None,
     # 'REDIRECT_URL': 'https://theapiguys.com',
 
     'ALLOW_NONE': False,
     'USE_DATETIME': True,
 
-    'STORAGE_CLASS': 'netsuite.storages.JSONStorage',
-    'CREDENTIALS_PATH': './netsuite-credentials.json',
-    'JSON_STORAGE_PATH': './netsuite-tokens.json',
-    'NETSUITE_CERTIFICATE_PATH': './netsuite-certificate.pem',
 
+
+    'STORAGE_CLASS': 'netsuite.storages.JSONStorage',
+    'CREDENTIALS_PATH': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_credentials.json')),
+    'JSON_STORAGE_PATH': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_tokens.json')),
+    'NETSUITE_CERTIFICATE_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_certificate.pem')),
+    'NETSUITE_KEY_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_key.pem')),
     'APP_NAME': 'default',
 }
 
 # List of settings that may be in string import notation.
 IMPORT_STRINGS = [
     'DEFAULT_STORAGE_CLASSES',
     'STORAGE_CLASS',
```

### Comparing `netsuite_python-1.3.1/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.3.2/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite/storages/JSONStorage.py` & `netsuite_python-1.3.2/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.3.2/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.1/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.3.2/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.1/setup.py` & `netsuite_python-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.3.1',
+    version='1.3.2',
     description='Python SDK for Netsuite API with Django Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

