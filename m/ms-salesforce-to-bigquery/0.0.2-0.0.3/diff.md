# Comparing `tmp/ms_salesforce_to_bigquery-0.0.2.tar.gz` & `tmp/ms_salesforce_to_bigquery-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_to_bigquery-0.0.2.tar", max compression
+gzip compressed data, was "ms_salesforce_to_bigquery-0.0.3.tar", max compression
```

## Comparing `ms_salesforce_to_bigquery-0.0.2.tar` & `ms_salesforce_to_bigquery-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/LICENSE
--rw-r--r--   0        0        0     3400 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2110 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2668 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2403 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     3276 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     1419 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0     6908 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     3661 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0      980 2023-04-12 10:36:46.923037 ms_salesforce_to_bigquery-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 11:08:39.927595 ms_salesforce_to_bigquery-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3400 2023-04-12 11:08:39.927595 ms_salesforce_to_bigquery-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2111 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2668 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2403 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     3276 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     1419 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0     6908 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     3661 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0      980 2023-04-12 11:08:39.931595 ms_salesforce_to_bigquery-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.3/PKG-INFO
```

### Comparing `ms_salesforce_to_bigquery-0.0.2/LICENSE` & `ms_salesforce_to_bigquery-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/README.md` & `ms_salesforce_to_bigquery-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/Auth.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib.parse import quote
 
 import requests
 
 from ms_salesforce_to_bigquery.salesforce.Auth import SalesforceAuthenticator
 
 DEFAULT_SALESFORCE_VERSION = "57.0"
-SALESFORCE_QUERY_ENDPOINT = "/services/data/{}/query/"
+SALESFORCE_QUERY_ENDPOINT = "/services/data/v{}/query/"
 
 
 class SalesforceQueryExecutor(SalesforceAuthenticator):
     def __init__(
         self,
         client_id,
         username,
```

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__init__.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py` & `ms_salesforce_to_bigquery-0.0.3/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.2/pyproject.toml` & `ms_salesforce_to_bigquery-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-to-bigquery"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_to_bigquery"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_to_bigquery-0.0.2/PKG-INFO` & `ms_salesforce_to_bigquery-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-to-bigquery
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

