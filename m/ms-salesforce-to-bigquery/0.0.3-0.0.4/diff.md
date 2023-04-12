# Comparing `tmp/ms_salesforce_to_bigquery-0.0.3.tar.gz` & `tmp/ms_salesforce_to_bigquery-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_to_bigquery-0.0.3.tar", max compression
+gzip compressed data, was "ms_salesforce_to_bigquery-0.0.4.tar", max compression
```

## Comparing `ms_salesforce_to_bigquery-0.0.3.tar` & `ms_salesforce_to_bigquery-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-12 11:08:39.927595 ms_salesforce_to_bigquery-0.0.3/LICENSE
--rw-r--r--   0        0        0     3400 2023-04-12 11:08:39.927595 ms_salesforce_to_bigquery-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2111 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2668 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2403 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     3276 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     1419 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0     6908 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     3661 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0      980 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3396 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2132 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2403 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     3268 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     1419 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0     6900 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     3661 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0      980 2023-04-12 13:49:15.058733 ms_salesforce_to_bigquery-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.4/PKG-INFO
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/LICENSE` & `ms_salesforce_to_bigquery-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.3/README.md` & `ms_salesforce_to_bigquery-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 Then, initialize the `Project` class with your Salesforce credentials:
 
 ```python
 project = Project(
     client_id="your_client_id",
     username="your_username",
-    auth_url="your_auth_url",
+    domain="your_domain",
     private_key="your_private_key",
     audience="https://login.salesforce.com", # Default value
     session_duration_hours=1, # Default value
     api_version='57.0',  # Default value
 )
 ```
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/Auth.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/Auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 
 
 class SalesforceAuthenticator(JWTGenerator):
     def __init__(
         self,
         client_id,
         username,
-        auth_url,
+        domain,
         private_key,
         audience,
         session_duration_hours,
+        api_version,
     ):
         super().__init__(
             client_id,
             private_key,
             username,
             audience,
             session_duration_hours,
         )
-        self.auth_url = auth_url
+
+        self.auth_url = f"{domain}/services/data/v{api_version}/query"
 
     def authenticate(self):
         payload = {
             "grant_type": "urn:ietf:params:oauth:grant-type:jwt-bearer",
             "assertion": self.generate_token(),
         }
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 
 
 class SalesforceQueryExecutor(SalesforceAuthenticator):
     def __init__(
         self,
         client_id,
         username,
-        auth_url,
+        domain,
         private_key,
         audience="https://login.salesforce.com",
         session_duration_hours=1,
         api_version=DEFAULT_SALESFORCE_VERSION,
     ):
         super().__init__(
             client_id,
             username,
-            auth_url,
+            domain,
             private_key,
             audience,
             session_duration_hours,
+            api_version,
         )
         self.endpoint = SALESFORCE_QUERY_ENDPOINT.format(api_version)
         self.access_token = self.authenticate()
 
     def fetch_data(self, query: str):
         query = quote(query)
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,33 +6,38 @@
 from ms_salesforce_to_bigquery.salesforce.Auth import SalesforceAuthenticator
 
 
 class TestSalesforceAuthenticator(unittest.TestCase):
     def setUp(self):
         self.client_id = "dummy_client_id"
         self.username = "dummy_username"
-        self.auth_url = "https://auth.example.com"
+        self.domain = "https://auth.example.com"
         self.private_key = rsa.generate_private_key(
             public_exponent=65537,
             key_size=2048,
         )
+        self.api_version = "57.0"
         self.authenticator = SalesforceAuthenticator(
             client_id=self.client_id,
             username=self.username,
-            auth_url=self.auth_url,
+            domain=self.domain,
             private_key=self.private_key,
             audience="http://fake-login.salesforce.com",
             session_duration_hours=1,
+            api_version=self.api_version,
         )
 
     def test_init(self):
         self.assertEqual(self.authenticator.client_id, self.client_id)
         self.assertEqual(self.authenticator.username, self.username)
-        self.assertEqual(self.authenticator.auth_url, self.auth_url)
         self.assertEqual(self.authenticator.private_key, self.private_key)
+        self.assertEqual(
+            self.authenticator.auth_url,
+            "https://auth.example.com/services/data/v57.0/query",
+        )
 
     def test_authenticate_success(self):
         response_mock = MagicMock()
         response_mock.status_code = 200
         response_mock.json.return_value = {
             "access_token": "dummy_access_token"
         }
@@ -41,15 +46,15 @@
             "requests.post",
             return_value=response_mock,
         ) as post_mock:
             access_token = self.authenticator.authenticate()
             self.assertEqual(access_token, "dummy_access_token")
 
             post_mock.assert_called_once_with(
-                self.auth_url,
+                f"{self.domain}/services/data/v57.0/query",
                 data={
                     "grant_type": "urn:ietf:params:oauth:grant-type:jwt-bearer",  # noqa: E501
                     "assertion": self.authenticator.generate_token(),
                 },
             )
 
     def test_authenticate_error(self):
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 
 
 class TestSalesforceQueryExecutor(unittest.TestCase):
     def setUp(self):
         self.client_id = "test_client_id"
         self.username = "test_username"
-        self.auth_url = "https://auth.example.com"
+        self.domain = "https://auth.example.com"
         self.private_key = "test_private_key"
         self.audience = "https://login.salesforce.com"
 
     def mocked_requests_post(self, *args, **kwargs):
         mock_response = Mock()
         mock_response.status_code = 200
         mock_response.json.return_value = {"access_token": "test_access_token"}
@@ -43,15 +43,15 @@
     def test_fetch_data_success(self, mock_get, mock_post):
         mock_post.side_effect = self.mocked_requests_post
         mock_get.side_effect = self.mocked_requests_get_success
 
         query_executor = SalesforceQueryExecutor(
             self.client_id,
             self.username,
-            self.auth_url,
+            self.domain,
             self.private_key,
             self.audience,
         )
 
         query = "SELECT Id, Name FROM Account"
         records = query_executor.fetch_data(query)
 
@@ -68,15 +68,15 @@
     def test_fetch_data_failure(self, mock_get, mock_post):
         mock_post.side_effect = self.mocked_requests_post
         mock_get.side_effect = self.mocked_requests_get_failure
 
         query_executor = SalesforceQueryExecutor(
             self.client_id,
             self.username,
-            self.auth_url,
+            self.domain,
             self.private_key,
             self.audience,
         )
 
         query = "SELECT Id, Name FROM Account"
         records = query_executor.fetch_data(query)
 
@@ -87,13 +87,13 @@
     )
     def test_auth_failure(self, mock_post):
         mock_post.return_value = Mock(status_code=400)
 
         query_executor = SalesforceQueryExecutor(
             self.client_id,
             self.username,
-            self.auth_url,
+            self.domain,
             self.private_key,
             self.audience,
         )
 
         self.assertIsNone(query_executor.access_token)
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__init__.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,21 +77,21 @@
     def test_get_opportunities(self, mock_make_request, mock_authenticate):
         mock_authenticate.return_value = "access_token"
         mock_make_request.return_value = MagicMock()
         mock_make_request.return_value.json.return_value = EXAMPLE_RESPONSE
 
         client_id = "client_id"
         username = "username"
-        auth_url = "https://auth.example.com"
+        domain = "https://auth.example.com"
         private_key = "private_key"
 
         project = Project(
             client_id,
             username,
-            auth_url,
+            domain,
             private_key,
             audience="https://login.salesforce.com",
         )
         query = "SELECT * FROM Opportunity"
 
         opportunities = project.get_opportunities(query)
         self.assertEqual(len(opportunities), 1)
@@ -153,21 +153,21 @@
         self, mock_make_request, mock_authenticate
     ):
         mock_authenticate.return_value = "access_token"
         mock_make_request.return_value = None
 
         client_id = "client_id"
         username = "username"
-        auth_url = "https://auth.example.com"
+        domain = "https://auth.example.com"
         private_key = "private_key"
 
         project = Project(
             client_id,
             username,
-            auth_url,
+            domain,
             private_key,
             audience="https://login.salesforce.com",
         )
         query = "SELECT * FROM Opportunity"
 
         opportunities = project.get_opportunities(query)
         self.assertEqual(opportunities, [])
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py` & `ms_salesforce_to_bigquery-0.0.4/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.3/pyproject.toml` & `ms_salesforce_to_bigquery-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-to-bigquery"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_to_bigquery"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_to_bigquery-0.0.3/PKG-INFO` & `ms_salesforce_to_bigquery-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-to-bigquery
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -69,15 +69,15 @@
 
 Then, initialize the `Project` class with your Salesforce credentials:
 
 ```python
 project = Project(
     client_id="your_client_id",
     username="your_username",
-    auth_url="your_auth_url",
+    domain="your_domain",
     private_key="your_private_key",
     audience="https://login.salesforce.com", # Default value
     session_duration_hours=1, # Default value
     api_version='57.0',  # Default value
 )
 ```
```

