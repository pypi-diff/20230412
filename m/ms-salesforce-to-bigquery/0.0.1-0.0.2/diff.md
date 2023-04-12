# Comparing `tmp/ms_salesforce_to_bigquery-0.0.1.tar.gz` & `tmp/ms_salesforce_to_bigquery-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_to_bigquery-0.0.1.tar", max compression
+gzip compressed data, was "ms_salesforce_to_bigquery-0.0.2.tar", max compression
```

## Comparing `ms_salesforce_to_bigquery-0.0.1.tar` & `ms_salesforce_to_bigquery-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-06 13:55:01.972839 ms_salesforce_to_bigquery-0.0.1/LICENSE
--rw-r--r--   0        0        0      614 2023-04-06 13:55:01.972839 ms_salesforce_to_bigquery-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-06 13:55:01.976839 ms_salesforce_to_bigquery-0.0.1/ms_salesforce_to_bigquery/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-06 13:55:01.976839 ms_salesforce_to_bigquery-0.0.1/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0       32 2023-04-06 13:55:01.976839 ms_salesforce_to_bigquery-0.0.1/ms_salesforce_to_bigquery/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 13:55:01.976839 ms_salesforce_to_bigquery-0.0.1/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2295 2023-04-06 13:55:01.976839 ms_salesforce_to_bigquery-0.0.1/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0      786 2023-04-06 13:55:01.976839 ms_salesforce_to_bigquery-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3400 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2110 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2668 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2403 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     3276 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     1419 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0     6908 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     3661 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0      980 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.2/PKG-INFO
```

### Comparing `ms_salesforce_to_bigquery-0.0.1/LICENSE` & `ms_salesforce_to_bigquery-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.1/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 class JWTGenerator:
     def __init__(
         self,
         client_id,
         private_key,
         username,
-        audience="https://login.salesforce.com",
-        session_duration_hours=1,
+        audience,
+        session_duration_hours,
     ):
         self.client_id = client_id
         self.private_key = private_key
         self.username = username
         self.audience = audience
         self.session_duration_hours = session_duration_hours
```

### Comparing `ms_salesforce_to_bigquery-0.0.1/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,22 @@
         )
         self.public_key = self.private_key.public_key()
 
     def test_generate_token(self):
         client_id = "example_client_id"
         username = "example_username"
         audience = "https://login.salesforce.com"
+        session_duration_hours = 1
 
         jwt_generator = JWTGenerator(
-            client_id, self.private_key, username, audience
+            client_id,
+            self.private_key,
+            username,
+            audience,
+            session_duration_hours,
         )
 
         token = jwt_generator.generate_token()
         self.assertIsNotNone(token)
 
         # Verify that the generated token has the correct data
         decoded_payload = jwt.decode(
```

