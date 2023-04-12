# Comparing `tmp/netsuite_python-1.3.4.tar.gz` & `tmp/netsuite_python-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.3.4.tar", last modified: Wed Apr 12 18:31:07 2023, max compression
+gzip compressed data, was "netsuite_python-1.3.5.tar", last modified: Wed Apr 12 21:39:22 2023, max compression
```

## Comparing `netsuite_python-1.3.4.tar` & `netsuite_python-1.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.660480 netsuite_python-1.3.4/
--rw-rw-rw-   0        0        0    11966 2023-04-12 18:31:07.660480 netsuite_python-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    11635 2023-04-09 23:07:01.000000 netsuite_python-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.641479 netsuite_python-1.3.4/netsuite/
--rw-rw-rw-   0        0        0    10514 2023-04-09 23:00:48.000000 netsuite_python-1.3.4/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.646479 netsuite_python-1.3.4/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.4/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.649477 netsuite_python-1.3.4/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.4/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.4/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.4/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.4/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.4/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.4/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.650478 netsuite_python-1.3.4/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0     5751 2023-04-12 18:24:23.000000 netsuite_python-1.3.4/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6016 2023-04-12 18:30:51.000000 netsuite_python-1.3.4/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.654478 netsuite_python-1.3.4/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.4/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:31:07.659480 netsuite_python-1.3.4/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0    11966 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 18:31:07.000000 netsuite_python-1.3.4/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 18:31:07.660480 netsuite_python-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-12 18:31:02.000000 netsuite_python-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:39:22.685121 netsuite_python-1.3.5/
+-rw-rw-rw-   0        0        0    12699 2023-04-12 21:39:22.684119 netsuite_python-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12368 2023-04-12 21:14:15.000000 netsuite_python-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 21:39:22.657120 netsuite_python-1.3.5/netsuite/
+-rw-rw-rw-   0        0        0    11858 2023-04-12 21:38:42.000000 netsuite_python-1.3.5/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:39:22.664118 netsuite_python-1.3.5/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.5/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:39:22.669119 netsuite_python-1.3.5/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.5/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.5/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.5/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.5/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.5/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.5/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:39:22.672119 netsuite_python-1.3.5/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0     8446 2023-04-12 21:38:54.000000 netsuite_python-1.3.5/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6306 2023-04-12 21:38:42.000000 netsuite_python-1.3.5/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:39:22.678119 netsuite_python-1.3.5/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.5/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:39:22.683119 netsuite_python-1.3.5/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0    12699 2023-04-12 21:39:22.000000 netsuite_python-1.3.5/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-12 21:39:22.000000 netsuite_python-1.3.5/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 21:39:22.000000 netsuite_python-1.3.5/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-12 21:39:22.000000 netsuite_python-1.3.5/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       94 2023-04-12 21:39:22.000000 netsuite_python-1.3.5/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 21:39:22.000000 netsuite_python-1.3.5/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 21:39:22.685121 netsuite_python-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      998 2023-04-12 21:39:19.000000 netsuite_python-1.3.5/setup.py
```

### Comparing `netsuite_python-1.3.4/PKG-INFO` & `netsuite_python-1.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -19,15 +19,39 @@
 ## What do I need to get set up? ##
 * Run `pip install netsuite-python`
 * Activate your python VENV
 * If using virtual environment 
   * Activate your virtual environment
   * `netsuite = python venv/bin/keap`
 
-* #### Notes ####
+## QUICK START ##
+
+### Prerequisite  Setup ###
+    1. Enable Services
+        * Rest Web Services
+        * Rest Web Services
+        * Rest Web Services
+        * Rest Web Services
+    2. Create a role for the integration with the following permissions:
+        * Access Token Management
+        * Log in using Access Tokens	
+        * Log in using OAuth 2.0 Access Tokens	
+        * OAuth 2.0 Authorized Applications Management	
+        * REST Web Services	
+        * SuiteApp Deployment	
+        * SuiteScript
+        * User Access Tokens	
+    3. Create an integration record 
+        * Check Client Credentials ( MAchine to Machine Grant) 
+        * STORE THE CLIENT ID 
+
+
+run ``` netsuite initialize ```
+
+ #### Notes ####
   * Requirements
     * Sandbox requires the same setup as Prod, it DOES NOT copy over
     * An administrator for the Netsuite app to follow the steps [here](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157771281570.html)
       * A user with the correct role
       * A role with the correct permissions
       * An Integration Record with the correct permissions (ensure default form is set correctly)
         * Client ID and Secret comes from this step, ensure they provide these
```

### Comparing `netsuite_python-1.3.4/README.md` & `netsuite_python-1.3.5/netsuite_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,57 @@
+Metadata-Version: 2.1
+Name: netsuite-python
+Version: 1.3.5
+Summary: Python SDK for Netsuite API with Django Integration
+Home-page: https://bitbucket.org/theapiguys/netsuite_python
+Author: Will @ TheAPIGuys
+Author-email: will@theapiguys.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # README #
 
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
 
 ## What do I need to get set up? ##
 * Run `pip install netsuite-python`
 * Activate your python VENV
 * If using virtual environment 
   * Activate your virtual environment
   * `netsuite = python venv/bin/keap`
 
-* #### Notes ####
+## QUICK START ##
+
+### Prerequisite  Setup ###
+    1. Enable Services
+        * Rest Web Services
+        * Rest Web Services
+        * Rest Web Services
+        * Rest Web Services
+    2. Create a role for the integration with the following permissions:
+        * Access Token Management
+        * Log in using Access Tokens	
+        * Log in using OAuth 2.0 Access Tokens	
+        * OAuth 2.0 Authorized Applications Management	
+        * REST Web Services	
+        * SuiteApp Deployment	
+        * SuiteScript
+        * User Access Tokens	
+    3. Create an integration record 
+        * Check Client Credentials ( MAchine to Machine Grant) 
+        * STORE THE CLIENT ID 
+
+
+run ``` netsuite initialize ```
+
+ #### Notes ####
   * Requirements
     * Sandbox requires the same setup as Prod, it DOES NOT copy over
     * An administrator for the Netsuite app to follow the steps [here](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157771281570.html)
       * A user with the correct role
       * A role with the correct permissions
       * An Integration Record with the correct permissions (ensure default form is set correctly)
         * Client ID and Secret comes from this step, ensure they provide these
@@ -169,8 +204,9 @@
  - [OneOfcustomerCustentityEnergyEffAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityEnergyEffAttended.md)
  - [OneOfcustomerCustentityHitachiCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHitachiCourseAttended.md)
  - [OneOfcustomerCustentityHpCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHpCourseAttended.md)
  - [OneOfcustomerCustentityPvCourseAtteneded](netsuite/swagger_client/docs/OneOfcustomerCustentityPvCourseAtteneded.md)
  - [OneOfcustomerCustentitySolCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentitySolCourseAttended.md)
  - [OneOfcustomerCustentityUnventHotWaterG3](netsuite/swagger_client/docs/OneOfcustomerCustentityUnventHotWaterG3.md)
  - [OneOfcustomerCustentityWaterRegulations1999](netsuite/swagger_client/docs/OneOfcustomerCustentityWaterRegulations1999.md)
- - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
+ - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
+
```

### Comparing `netsuite_python-1.3.4/netsuite/Netsuite.py` & `netsuite_python-1.3.5/netsuite/Netsuite.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from netsuite.settings import APISettings
 from netsuite.storages import BaseStorage, JSONStorage
 from netsuite import api_clients
 
 
 client_exists = False
 try:
-    import netsuite_client
-    from netsuite_client.api import *
+    import netsuite_rest_client
+    from netsuite_rest_client.api import *
     client_exists = True
 except ModuleNotFoundError or ImportError as err:
     print('Rest Client needs to be generated')
 
 
 class Netsuite:
     app_name: str = None
@@ -72,14 +72,15 @@
 
     @property
     def REST_CLIENT(self):
         try:
             if not self.rest_client:
                 if client_exists:
                     self.rest_client = self.get_rest_client()
+
                     return self.rest_client
             else:
                 print('Client needs to be generated.')
         except Exception as e:
             print(e)
 
 
@@ -144,17 +145,22 @@
         token = NetsuiteToken(**response.json())
         self.save_token(token)
         # if token.access_token is not None:
         #     self.get_customer_categories()
         #     self.get_status_dict()
         return self.token
 
-    def generate_swagger_client(self):
+    def generate_rest_client(self):
+        # from urllib.request import urlopen
+        # from tempfile import NamedTemporaryFile
+        # from shutil import unpack_archive
+        import zipfile, shutil
+        from io import BytesIO
         token = self.storage.get_token(self.app_name)
-        url = f"https://{self.app_name}.suitetalk.api.netsuite.com/services/rest/record/v1/metadata-catalog"
+        url = f"https://{self.netsuite_app_name}.suitetalk.api.netsuite.com/services/rest/record/v1/metadata-catalog"
         params = {
             'select': 'customer'
         }
         headers = {
             'Accept': 'application/swagger+json',
             'Authorization': f'Bearer {token.access_token}'
         }
@@ -169,32 +175,57 @@
             'spec': response.json()
         }
         headers2 = {
             'Content-Type': 'application/json'
         }
         result = requests.post('https://api-latest-master.openapi-generator.tech/api/gen/clients/python',headers=headers2, json=data)
         print(result.json())
+
+        # Defining the zip file URL
+        url = result.json().get('link')
+
+        # Split URL to get the file name
+        filename = url.split('/')[-1]
+
+        # Downloading the file by sending the request to the URL
+        req = requests.get(url)
+        print('Downloading Completed')
+
+        # extracting the zip file contents
+        file = zipfile.ZipFile(BytesIO(req.content))
+        file.extractall(path=self.api_settings.NETSUITE_CLIENT_PATH)
+
+        src = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client/netsuite_client')
+        dst = Path(self.api_settings.NETSUITE_CLIENT_PATH)
+        shutil.copytree(src, dst, symlinks=False, ignore=None, ignore_dangling_symlinks=False,
+                        dirs_exist_ok=True)
+        print('Netsuite Rest Client Created')
+        # shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
+        # print('temp folder removed.')
+
         # with open("./client_schema.json", "w") as outfile:
         #     outfile.write(json.dumps(response.json()))
 
     def get_token(self):
         if not self.token.is_expired:
             return self.token
         else:
             return self.request_access_token()
 
 
     def get_rest_client(self):
-        configuration = netsuite_client.configuration.Configuration(
-            host="https://472052.suitetalk.api.netsuite.com/services/rest/record/v1"
+        configuration = netsuite_rest_client.configuration.Configuration(
+            host=f"https://{self.netsuite_app_name}.suitetalk.api.netsuite.com/services/rest/record/v1"
         )
+
         configuration.api_key['OAuth_1.0_authorization'] = self.get_token().access_token
         configuration.api_key_prefix['OAuth_1.0_authorization'] = 'Bearer'
-        api_client = netsuite_client.api_client.ApiClient(configuration=configuration)
-        return api_client
+        rest_client.api_client = netsuite_rest_client.api_client.ApiClient(configuration=configuration)
+        rest_client.customer_api = netsuite_rest_client.api.customer_api.CustomerApi(api_client)
+        return rest_client
 
 
     class QueryClient:
         def __init__(self, netsuite):
             self.netsuite = netsuite
             self.configuration = api_clients.Configuration()
             self.configuration.token = netsuite.storage.get_token(netsuite.app_name)
```

### Comparing `netsuite_python-1.3.4/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.3.5/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.3.5/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite/api_clients/api_client.py` & `netsuite_python-1.3.5/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite/api_clients/configuration.py` & `netsuite_python-1.3.5/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite/api_clients/rest.py` & `netsuite_python-1.3.5/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite/module_loading.py` & `netsuite_python-1.3.5/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite/scripts/cli.py` & `netsuite_python-1.3.5/netsuite/scripts/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,22 +5,85 @@
 from click import prompt
 from pathlib import Path
 
 from netsuite.Netsuite import Netsuite
 from netsuite.settings import api_settings, IN_MEMORY_STORAGE, JSON_STORAGE
 from OpenSSL.SSL import FILETYPE_PEM
 from OpenSSL.crypto import (dump_certificate, X509, X509Name, PKey, TYPE_RSA, X509Req, dump_privatekey, X509Extension)
+from rich import print
+
+def link(uri, label=None):
+    if label is None:
+        label = uri
+    parameters = ''
+
+    # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
+    escape_mask = '\033]8;{};{}\033\\{}\033]8;;\033\\'
+
+    return escape_mask.format(parameters, uri, label)
 
 @click.group()
 def cli():
     """
     Simple CLI for managing Netsuite API Access
     """
     pass
 
+@cli.command()
+def initialize():
+    steps_completed = False
+    while not steps_completed:
+        steps_completed = prompt(f"Have you created the integration record by following the steps in the README?", default='y', type=click.BOOL, show_choices=True)
+        if steps_completed:
+            client_id = prompt("Client Id", hide_input=False)
+        else:
+            print('Read it and do the steps hoe https://bitbucket.org/theapiguys/netsuite_python/src/master/')
+
+    print("Generate Certificate", )
+    certificate_uploaded = False
+    while not certificate_uploaded:
+        certificate_uploaded = prompt(f"Have you generated a certificate?", default='y', type=click.BOOL, show_choices=True)
+        if certificate_uploaded:
+            certificate_id = prompt("Certificate ID: ", hide_input=False)
+        else:
+            generate_certificate()
+
+    netsuite_app_name = prompt("What is the netsuite application name? (Portion before app.netsuite.com)", hide_input=False)
+
+    app_name = prompt("App Name", default=api_settings.APP_NAME)
+    allow_none = prompt("Allow None", default=api_settings.ALLOW_NONE)
+    use_datetime = prompt("Use Datetime", default=api_settings.USE_DATETIME)
+    storage_class = prompt("Storage Class", default=api_settings.defaults.get('STORAGE_CLASS'),
+                           type=click.Choice(api_settings.defaults.get('DEFAULT_STORAGE_CLASSES')),
+                           show_choices=True)
+
+    creds = {
+        'CLIENT_ID': client_id,
+        'CERT_ID': cert_id,
+        # 'CLIENT_SECRET': client_secret,
+        # 'REDIRECT_URL': redirect_url,
+        'NETSUITE_APP_NAME': netsuite_app_name,
+        'APP_NAME': app_name,
+        'ALLOW_NONE': allow_none,
+        'USE_DATETIME': use_datetime,
+        'STORAGE_CLASS': storage_class,
+    }
+
+    if storage_class == JSON_STORAGE:
+        creds['JSON_STORAGE_PATH'] = prompt("Token Storage File", default=api_settings.JSON_STORAGE_PATH,
+                                            type=click.Path(readable=True, writable=True))
+
+    with open(api_settings.CREDENTIALS_PATH, 'w') as f:
+        creds_json = json.dumps(creds, indent=4)
+        f.write(creds_json)
+        print(f"Netsuite Credentials written to: {api_settings.CREDENTIALS_PATH}")
+
+
+
+
 
 @cli.command()
 def generate_certificate():
 
     print(f"BASE DIR: {api_settings.BASE_DIR}")
 
     CN = prompt("Domain", hide_input=False)
@@ -109,14 +172,18 @@
             f.write(creds_json)
             print(f"Netsuite Credentials written to: {api_settings.CREDENTIALS_PATH}")
     else:
         click.echo(creds)
 
     return creds
 
+@cli.command()
+def generate_rest_client():
+    netsuite = Netsuite()
+    netsuite.generate_rest_client()
 
 @cli.command()
 @click.option('--credentials-file', '--f', type=click.File('r'), default=api_settings.CREDENTIALS_PATH,
               prompt="Path to Credentials File")
 @click.pass_context
 def get_access_token(ctx, credentials_file):
     """OAuth flow for Netsuite to obtain an access and refresh token"""
```

### Comparing `netsuite_python-1.3.4/netsuite/settings.py` & `netsuite_python-1.3.5/netsuite/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,23 @@
 except ImportError as e:
     settings = None
 
 BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
 BASE_CONFIG_DIR = Path.joinpath(BASE_DIR, 'config')
 NETSUITE_CONFIG_DIR = Path.joinpath(BASE_CONFIG_DIR, 'netsuite')
 NETSUITE_TOKENS_DIR = Path.joinpath(BASE_CONFIG_DIR, 'tokens')
+PACKAGE_DIR = Path(__file__).parent.resolve()
+NETSUITE_CLIENT_DIR = Path.joinpath(PACKAGE_DIR, 'netsuite_rest_client')
 
 if not os.path.exists(NETSUITE_CONFIG_DIR):
     os.makedirs(NETSUITE_CONFIG_DIR)
 if not os.path.exists(NETSUITE_TOKENS_DIR):
     os.makedirs(NETSUITE_TOKENS_DIR)
+if not os.path.exists(NETSUITE_CLIENT_DIR):
+    os.makedirs(NETSUITE_CLIENT_DIR)
 
 
 JSON_STORAGE = 'netsuite.storages.JSONStorage'
 IN_MEMORY_STORAGE = 'netsuite.storages.InMemoryStorage'
 DEFAULTS = {
     # Base API policies
     'DEFAULT_STORAGE_CLASSES': [
@@ -65,14 +69,15 @@
 
 
     'STORAGE_CLASS': 'netsuite.storages.JSONStorage',
     'CREDENTIALS_PATH': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_credentials.json')),
     'JSON_STORAGE_PATH': str(Path.joinpath(NETSUITE_TOKENS_DIR, 'netsuite_tokens.json')),
     'NETSUITE_CERTIFICATE_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_certificate.pem')),
     'NETSUITE_KEY_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_key.pem')),
+    'NETSUITE_CLIENT_PATH': str(Path.joinpath(PACKAGE_DIR, 'netsuite_rest_client')),
     'APP_NAME': 'default',
 }
 
 # List of settings that may be in string import notation.
 IMPORT_STRINGS = [
     'DEFAULT_STORAGE_CLASSES',
     'STORAGE_CLASS',
```

### Comparing `netsuite_python-1.3.4/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.3.5/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite/storages/JSONStorage.py` & `netsuite_python-1.3.5/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-Metadata-Version: 2.1
-Name: netsuite-python
-Version: 1.3.4
-Summary: Python SDK for Netsuite API with Django Integration
-Home-page: https://bitbucket.org/theapiguys/netsuite_python
-Author: Will @ TheAPIGuys
-Author-email: will@theapiguys.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # README #
 
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
 
 ## What do I need to get set up? ##
 * Run `pip install netsuite-python`
 * Activate your python VENV
 * If using virtual environment 
   * Activate your virtual environment
   * `netsuite = python venv/bin/keap`
 
-* #### Notes ####
+## QUICK START ##
+
+### Prerequisite  Setup ###
+    1. Enable Services
+        * Rest Web Services
+        * Rest Web Services
+        * Rest Web Services
+        * Rest Web Services
+    2. Create a role for the integration with the following permissions:
+        * Access Token Management
+        * Log in using Access Tokens	
+        * Log in using OAuth 2.0 Access Tokens	
+        * OAuth 2.0 Authorized Applications Management	
+        * REST Web Services	
+        * SuiteApp Deployment	
+        * SuiteScript
+        * User Access Tokens	
+    3. Create an integration record 
+        * Check Client Credentials ( MAchine to Machine Grant) 
+        * STORE THE CLIENT ID 
+
+
+run ``` netsuite initialize ```
+
+ #### Notes ####
   * Requirements
     * Sandbox requires the same setup as Prod, it DOES NOT copy over
     * An administrator for the Netsuite app to follow the steps [here](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157771281570.html)
       * A user with the correct role
       * A role with the correct permissions
       * An Integration Record with the correct permissions (ensure default form is set correctly)
         * Client ID and Secret comes from this step, ensure they provide these
@@ -180,9 +193,8 @@
  - [OneOfcustomerCustentityEnergyEffAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityEnergyEffAttended.md)
  - [OneOfcustomerCustentityHitachiCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHitachiCourseAttended.md)
  - [OneOfcustomerCustentityHpCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHpCourseAttended.md)
  - [OneOfcustomerCustentityPvCourseAtteneded](netsuite/swagger_client/docs/OneOfcustomerCustentityPvCourseAtteneded.md)
  - [OneOfcustomerCustentitySolCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentitySolCourseAttended.md)
  - [OneOfcustomerCustentityUnventHotWaterG3](netsuite/swagger_client/docs/OneOfcustomerCustentityUnventHotWaterG3.md)
  - [OneOfcustomerCustentityWaterRegulations1999](netsuite/swagger_client/docs/OneOfcustomerCustentityWaterRegulations1999.md)
- - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
-
+ - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
```

### Comparing `netsuite_python-1.3.4/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.3.5/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.4/setup.py` & `netsuite_python-1.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.3.4',
+    version='1.3.5',
     description='Python SDK for Netsuite API with Django Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'Click',
         'requests',
+        'zipfile',
         'PyJWT',
         "urllib3 >= 1.15",
         "six >= 1.10",
         "certifi",
         "python-dateutil",
-        "pyOpenSSL"
+        "pyOpenSSL",
+        "shutil"
     ],
     entry_points={
         'console_scripts': [
             'netsuite = netsuite.scripts.cli:cli',
         ],
 
     },
```

