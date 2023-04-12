# Comparing `tmp/ms_salesforce_to_bigquery-0.0.4.tar.gz` & `tmp/ms_salesforce_to_bigquery-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_to_bigquery-0.0.4.tar", max compression
+gzip compressed data, was "ms_salesforce_to_bigquery-0.0.5.tar", max compression
```

## Comparing `ms_salesforce_to_bigquery-0.0.4.tar` & `ms_salesforce_to_bigquery-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/LICENSE
--rw-r--r--   0        0        0     3396 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2132 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2841 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2403 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     3268 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     1419 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0     6900 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     3661 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0      980 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 14:11:36.248908 ms_salesforce_to_bigquery-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3396 2023-04-12 14:11:36.248908 ms_salesforce_to_bigquery-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 14:11:36.248908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/__init__.py
+-rw-r--r--   0        0        0     1499 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2046 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2757 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2403 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     3268 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     1419 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0     6900 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     3661 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0      980 2023-04-12 14:11:36.252908 ms_salesforce_to_bigquery-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.5/PKG-INFO
```

### Comparing `ms_salesforce_to_bigquery-0.0.4/LICENSE` & `ms_salesforce_to_bigquery-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/README.md` & `ms_salesforce_to_bigquery-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/Auth.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/Auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,24 @@
         self,
         client_id,
         username,
         domain,
         private_key,
         audience,
         session_duration_hours,
-        api_version,
     ):
         super().__init__(
             client_id,
             private_key,
             username,
             audience,
             session_duration_hours,
         )
 
-        self.auth_url = f"{domain}/services/data/v{api_version}/query"
+        self.auth_url = f"{domain}/services/oauth2/token"
 
     def authenticate(self):
         payload = {
             "grant_type": "urn:ietf:params:oauth:grant-type:jwt-bearer",
             "assertion": self.generate_token(),
         }
```

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import time
-from urllib.parse import quote
 
 import requests
 
 from ms_salesforce_to_bigquery.salesforce.Auth import SalesforceAuthenticator
 
 DEFAULT_SALESFORCE_VERSION = "57.0"
 SALESFORCE_QUERY_ENDPOINT = "/services/data/v{}/query/"
@@ -24,22 +23,19 @@
         super().__init__(
             client_id,
             username,
             domain,
             private_key,
             audience,
             session_duration_hours,
-            api_version,
         )
         self.endpoint = SALESFORCE_QUERY_ENDPOINT.format(api_version)
         self.access_token = self.authenticate()
 
     def fetch_data(self, query: str):
-        query = quote(query)
-
         if not self.access_token:
             logging.error("Authentication failed, cannot fetch data")
             return None
 
         headers = {"Authorization": f"Bearer {self.access_token}"}
 
         all_records = []
```

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,30 @@
         self.client_id = "dummy_client_id"
         self.username = "dummy_username"
         self.domain = "https://auth.example.com"
         self.private_key = rsa.generate_private_key(
             public_exponent=65537,
             key_size=2048,
         )
-        self.api_version = "57.0"
         self.authenticator = SalesforceAuthenticator(
             client_id=self.client_id,
             username=self.username,
             domain=self.domain,
             private_key=self.private_key,
             audience="http://fake-login.salesforce.com",
             session_duration_hours=1,
-            api_version=self.api_version,
         )
 
     def test_init(self):
         self.assertEqual(self.authenticator.client_id, self.client_id)
         self.assertEqual(self.authenticator.username, self.username)
         self.assertEqual(self.authenticator.private_key, self.private_key)
         self.assertEqual(
             self.authenticator.auth_url,
-            "https://auth.example.com/services/data/v57.0/query",
+            "https://auth.example.com/services/oauth2/token",
         )
 
     def test_authenticate_success(self):
         response_mock = MagicMock()
         response_mock.status_code = 200
         response_mock.json.return_value = {
             "access_token": "dummy_access_token"
@@ -46,15 +44,15 @@
             "requests.post",
             return_value=response_mock,
         ) as post_mock:
             access_token = self.authenticator.authenticate()
             self.assertEqual(access_token, "dummy_access_token")
 
             post_mock.assert_called_once_with(
-                f"{self.domain}/services/data/v57.0/query",
+                f"{self.domain}/services/oauth2/token",
                 data={
                     "grant_type": "urn:ietf:params:oauth:grant-type:jwt-bearer",  # noqa: E501
                     "assertion": self.authenticator.generate_token(),
                 },
             )
 
     def test_authenticate_error(self):
```

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__init__.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py` & `ms_salesforce_to_bigquery-0.0.5/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.4/pyproject.toml` & `ms_salesforce_to_bigquery-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-to-bigquery"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_to_bigquery"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_to_bigquery-0.0.4/PKG-INFO` & `ms_salesforce_to_bigquery-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-to-bigquery
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

