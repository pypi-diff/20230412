# Comparing `tmp/saic_ismart_client-1.1.4.tar.gz` & `tmp/saic_ismart_client-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.1.4.tar", last modified: Wed Mar 29 14:15:54 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.1.5.tar", last modified: Wed Apr 12 06:45:12 2023, max compression
```

## Comparing `saic_ismart_client-1.1.4.tar` & `saic_ismart_client-1.1.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.287751 saic_ismart_client-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-29 14:15:54.287751 saic_ismart_client-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 14:15:54.287751 saic_ismart_client-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.279751 saic_ismart_client-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.279751 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.283751 saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-29 14:15:54.000000 saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-29 14:15:54.000000 saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:15:54.000000 saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 14:15:54.000000 saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-29 14:15:54.000000 saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:15:54.287751 saic_ismart_client-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-03-29 14:15:40.000000 saic_ismart_client-1.1.4/tests/test_ws_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:45:12.386515 saic_ismart_client-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.378515 saic_ismart_client-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.378515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_ws_api.py
```

### Comparing `saic_ismart_client-1.1.4/LICENSE` & `saic_ismart_client-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/PKG-INFO` & `saic_ismart_client-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.1.4
+Version: 1.1.5
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.1.4/README.md` & `saic_ismart_client-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/pyproject.toml` & `saic_ismart_client-1.1.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.1.5/src/saic_ismart_client/saic_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,24 +94,24 @@
         self.message_v1_1_coder.initialize_message(
             UID_INIT[len(self.saic_user):] + self.saic_user,
             cast(str, None),
             application_id,
             application_data_protocol_version,
             1,
             login_request_message)
-        self.publish_json_value(application_id, application_data_protocol_version, login_request_message.get_data())
+        self.publish_json_request(application_id, application_data_protocol_version, login_request_message.get_data())
         login_request_hex = self.message_v1_1_coder.encode_request(login_request_message)
-        self.publish_raw_value(application_id, application_data_protocol_version, login_request_hex)
+        self.publish_raw_request(application_id, application_data_protocol_version, login_request_hex)
         login_response_hex = self.send_request(login_request_hex,
                                                urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mp'))
-        self.publish_raw_value(application_id, application_data_protocol_version, login_response_hex)
+        self.publish_raw_response(application_id, application_data_protocol_version, login_response_hex)
         logging_in_rsp = MpUserLoggingInRsp()
         login_response_message = MessageV11(header, MessageBodyV11(), logging_in_rsp)
         self.message_v1_1_coder.decode_response(login_response_hex, login_response_message)
-        self.publish_json_value(application_id, application_data_protocol_version, login_response_message.get_data())
+        self.publish_json_response(application_id, application_data_protocol_version, login_response_message.get_data())
         if login_response_message.body.error_message is not None:
             raise SaicApiException(login_response_message.body.error_message.decode(),
                                    login_response_message.body.result)
         else:
             self.uid = login_response_message.body.uid
             self.token = logging_in_rsp.token
             if logging_in_rsp.token_expiration is not None:
@@ -131,24 +131,25 @@
         self.message_v1_1_coder.initialize_message(
             self.uid,
             self.get_token(),
             application_id,
             application_data_protocol_version,
             1,
             alarm_switch_req_message)
-        self.publish_json_value(application_id, application_data_protocol_version, alarm_switch_req_message.get_data())
+        self.publish_json_request(application_id, application_data_protocol_version,
+                                  alarm_switch_req_message.get_data())
         alarm_switch_request_hex = self.message_v1_1_coder.encode_request(alarm_switch_req_message)
-        self.publish_raw_value(application_id, application_data_protocol_version, alarm_switch_request_hex)
+        self.publish_raw_request(application_id, application_data_protocol_version, alarm_switch_request_hex)
         alarm_switch_response_hex = self.send_request(alarm_switch_request_hex,
                                                       urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mp'))
-        self.publish_raw_value(application_id, application_data_protocol_version, alarm_switch_response_hex)
+        self.publish_raw_response(application_id, application_data_protocol_version, alarm_switch_response_hex)
         alarm_switch_response_message = MessageV11(header, MessageBodyV11())
         self.message_v1_1_coder.decode_response(alarm_switch_response_hex, alarm_switch_response_message)
-        self.publish_json_value(application_id, application_data_protocol_version,
-                                alarm_switch_response_message.get_data())
+        self.publish_json_response(application_id, application_data_protocol_version,
+                                   alarm_switch_response_message.get_data())
 
         if alarm_switch_response_message.body.error_message is not None:
             raise SaicApiException(alarm_switch_response_message.body.error_message.decode(),
                                    alarm_switch_response_message.body.result)
 
     def get_vehicle_status(self, vin_info: VinInfo, event_id: str = None) -> MessageV2:
         vehicle_status_req = OtaRvmVehicleStatusReq()
@@ -156,23 +157,23 @@
         vehicle_status_req_msg = MessageV2(MessageBodyV2(), vehicle_status_req)
         application_id = '511'
         application_data_protocol_version = 25857
         self.message_V2_1_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 1, vehicle_status_req_msg)
         if event_id is not None:
             vehicle_status_req_msg.body.event_id = event_id
-        self.publish_json_value(application_id, application_data_protocol_version, vehicle_status_req_msg.get_data())
+        self.publish_json_request(application_id, application_data_protocol_version, vehicle_status_req_msg.get_data())
         vehicle_status_req_hex = self.message_V2_1_coder.encode_request(vehicle_status_req_msg)
-        self.publish_raw_value(application_id, application_data_protocol_version, vehicle_status_req_hex)
+        self.publish_raw_request(application_id, application_data_protocol_version, vehicle_status_req_hex)
         vehicle_status_rsp_hex = self.send_request(vehicle_status_req_hex,
                                                    urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv21'))
-        self.publish_raw_value(application_id, application_data_protocol_version, vehicle_status_rsp_hex)
+        self.publish_raw_response(application_id, application_data_protocol_version, vehicle_status_rsp_hex)
         vehicle_status_rsp_msg = MessageV2(MessageBodyV2(), OtaRvmVehicleStatusResp25857())
         self.message_V2_1_coder.decode_response(vehicle_status_rsp_hex, vehicle_status_rsp_msg)
-        self.publish_json_value(application_id, application_data_protocol_version, vehicle_status_rsp_msg.get_data())
+        self.publish_json_response(application_id, application_data_protocol_version, vehicle_status_rsp_msg.get_data())
         return vehicle_status_rsp_msg
 
     def lock_vehicle(self, vin_info: VinInfo) -> None:
         rvc_params = []
         self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x01', rvc_params)
 
     def unlock_vehicle(self, vin_info: VinInfo) -> None:
@@ -284,44 +285,44 @@
         vehicle_control_cmd_req_msg = MessageV2(MessageBodyV2(), vehicle_control_req)
         application_id = '510'
         application_data_protocol_version = 25857
         self.message_V2_1_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 1, vehicle_control_cmd_req_msg)
         if event_id is not None:
             vehicle_control_cmd_req_msg.body.event_id = event_id
-        self.publish_json_value(application_id, application_data_protocol_version,
-                                vehicle_control_cmd_req_msg.get_data())
+        self.publish_json_request(application_id, application_data_protocol_version,
+                                  vehicle_control_cmd_req_msg.get_data())
         vehicle_control_cmd_req_msg_hex = self.message_V2_1_coder.encode_request(vehicle_control_cmd_req_msg)
-        self.publish_raw_value(application_id, application_data_protocol_version, vehicle_control_cmd_req_msg_hex)
+        self.publish_raw_request(application_id, application_data_protocol_version, vehicle_control_cmd_req_msg_hex)
         vehicle_control_cmd_rsp_msg_hex = self.send_request(vehicle_control_cmd_req_msg_hex,
                                                             urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv21'))
-        self.publish_raw_value(application_id, application_data_protocol_version, vehicle_control_cmd_rsp_msg_hex)
+        self.publish_raw_response(application_id, application_data_protocol_version, vehicle_control_cmd_rsp_msg_hex)
         vehicle_control_cmd_rsp_msg = MessageV2(MessageBodyV2())
         self.message_V2_1_coder.decode_response(vehicle_control_cmd_rsp_msg_hex, vehicle_control_cmd_rsp_msg)
-        self.publish_json_value(application_id, application_data_protocol_version,
-                                vehicle_control_cmd_rsp_msg.get_data())
+        self.publish_json_response(application_id, application_data_protocol_version,
+                                   vehicle_control_cmd_rsp_msg.get_data())
         return vehicle_control_cmd_rsp_msg
 
     def get_charging_status(self, vin_info: VinInfo, event_id: str = None) -> MessageV30:
         chrg_mgmt_data_req_msg = MessageV30(MessageBodyV30())
         application_id = '516'
         application_data_protocol_version = 768
         self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 5, chrg_mgmt_data_req_msg)
         if event_id is not None:
             chrg_mgmt_data_req_msg.body.event_id = event_id
-        self.publish_json_value(application_id, application_data_protocol_version, chrg_mgmt_data_req_msg.get_data())
+        self.publish_json_request(application_id, application_data_protocol_version, chrg_mgmt_data_req_msg.get_data())
         chrg_mgmt_data_req_hex = self.message_V3_0_coder.encode_request(chrg_mgmt_data_req_msg)
-        self.publish_raw_value(application_id, application_data_protocol_version, chrg_mgmt_data_req_hex)
+        self.publish_raw_request(application_id, application_data_protocol_version, chrg_mgmt_data_req_hex)
         chrg_mgmt_data_rsp_hex = self.send_request(chrg_mgmt_data_req_hex,
                                                    urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
-        self.publish_raw_value(application_id, application_data_protocol_version, chrg_mgmt_data_rsp_hex)
+        self.publish_raw_response(application_id, application_data_protocol_version, chrg_mgmt_data_rsp_hex)
         chrg_mgmt_data_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgMangDataResp())
         self.message_V3_0_coder.decode_response(chrg_mgmt_data_rsp_hex, chrg_mgmt_data_rsp_msg)
-        self.publish_json_value(application_id, application_data_protocol_version, chrg_mgmt_data_rsp_msg.get_data())
+        self.publish_json_response(application_id, application_data_protocol_version, chrg_mgmt_data_rsp_msg.get_data())
         return chrg_mgmt_data_rsp_msg
 
     def get_message_list(self, event_id: str = None) -> MessageV11:
         message_list_request = MessageListReq()
         message_list_request.start_end_number = StartEndNumber()
         message_list_request.start_end_number.start_number = 1
         message_list_request.start_end_number.end_number = 5
@@ -333,23 +334,23 @@
         message_list_req_msg = MessageV11(header, message_body, message_list_request)
         application_id = '531'
         application_data_protocol_version = 513
         self.message_v1_1_coder.initialize_message(self.uid, self.get_token(), application_id,
                                                    application_data_protocol_version, 1, message_list_req_msg)
         if event_id is not None:
             message_body.event_id = event_id
-        self.publish_json_value(application_id, application_data_protocol_version, message_list_req_msg.get_data())
+        self.publish_json_request(application_id, application_data_protocol_version, message_list_req_msg.get_data())
         message_list_req_hex = self.message_v1_1_coder.encode_request(message_list_req_msg)
-        self.publish_raw_value(application_id, application_data_protocol_version, message_list_req_hex)
+        self.publish_raw_request(application_id, application_data_protocol_version, message_list_req_hex)
         message_list_rsp_hex = self.send_request(message_list_req_hex,
                                                  urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mp'))
-        self.publish_raw_value(application_id, application_data_protocol_version, message_list_rsp_hex)
+        self.publish_raw_response(application_id, application_data_protocol_version, message_list_rsp_hex)
         message_list_rsp_msg = MessageV11(header, MessageBodyV11(), MessageListResp())
         self.message_v1_1_coder.decode_response(message_list_rsp_hex, message_list_rsp_msg)
-        self.publish_json_value(application_id, application_data_protocol_version, message_list_rsp_msg.get_data())
+        self.publish_json_response(application_id, application_data_protocol_version, message_list_rsp_msg.get_data())
         return message_list_rsp_msg
 
     def delete_message(self, message_id: int, event_id: str = None) -> None:
         abort_send_msg_req = AbortSendMessageReq()
         abort_send_msg_req.action_type = 'DELETE'
         abort_send_msg_req.message_id = message_id
 
@@ -359,36 +360,50 @@
         message_delete_req_msg = MessageV11(header, message_body, abort_send_msg_req)
         application_id = '615'
         application_protocol_version = 513
         self.message_v1_1_coder.initialize_message(self.uid, self.get_token(), application_id,
                                                    application_protocol_version, 1, message_delete_req_msg)
         if event_id is not None:
             message_body.event_id = event_id
-        self.publish_json_value(application_id, application_protocol_version, abort_send_msg_req.get_data())
+        self.publish_json_request(application_id, application_protocol_version, abort_send_msg_req.get_data())
         message_delete_req_hex = self.message_v1_1_coder.encode_request(message_delete_req_msg)
-        self.publish_raw_value(application_id, application_protocol_version, message_delete_req_hex)
+        self.publish_raw_request(application_id, application_protocol_version, message_delete_req_hex)
         message_delete_rsp_hex = self.send_request(message_delete_req_hex,
                                                    urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mp'))
-        self.publish_raw_value(application_id, application_protocol_version, message_delete_rsp_hex)
+        self.publish_raw_response(application_id, application_protocol_version, message_delete_rsp_hex)
         message_delete_rsp_msg = MessageV11(header, MessageBodyV11())
         self.message_v1_1_coder.decode_response(message_delete_rsp_hex, message_delete_rsp_msg)
-        self.publish_json_value(application_id, application_protocol_version, message_delete_rsp_msg.get_data())
+        self.publish_json_response(application_id, application_protocol_version, message_delete_rsp_msg.get_data())
         if message_delete_rsp_msg.body.error_message is not None:
             raise SaicApiException(message_delete_rsp_msg.body.error_message.decode(),
                                    message_delete_rsp_msg.body.result)
 
-    def publish_raw_value(self, application_id: str, application_data_protocol_version: int, raw: str):
-        key = f'{application_id}_{application_data_protocol_version}/raw'
+    def publish_raw_value(self, key: str, raw: str):
         if self.on_publish_raw_value is not None:
             self.on_publish_raw_value(key, raw)
         else:
             logging.debug(f'{key}: {raw}')
 
-    def publish_json_value(self, application_id: str, application_data_protocol_version: int, data: dict):
-        key = f'{application_id}_{application_data_protocol_version}/json'
+    def publish_raw_request(self, application_id: str, application_data_protocol_version: int, raw: str):
+        key = f'{application_id}_{application_data_protocol_version}/raw/request'
+        self.publish_raw_value(key, raw)
+
+    def publish_raw_response(self, application_id: str, application_data_protocol_version: int, raw: str):
+        key = f'{application_id}_{application_data_protocol_version}/raw/response'
+        self.publish_raw_value(key, raw)
+
+    def publish_json_request(self, application_id: str, application_data_protocol_version: int, data: dict):
+        key = f'{application_id}_{application_data_protocol_version}/json/request'
+        self.publish_json(key, data)
+
+    def publish_json_response(self, application_id: str, application_data_protocol_version: int, data: dict):
+        key = f'{application_id}_{application_data_protocol_version}/json/response'
+        self.publish_json(key, data)
+
+    def publish_json(self, key: str, data: dict):
         if self.on_publish_json_value is not None:
             self.on_publish_json_value(key, data)
         else:
             logging.debug(f'{key}: {data}')
 
     def send_request(self, hex_message: str, endpoint) -> str:
         headers = {
```

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.1.4/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/tests/test_Message_v1_1.py` & `saic_ismart_client-1.1.5/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/tests/test_Message_v2_1.py` & `saic_ismart_client-1.1.5/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/tests/test_Message_v3_0.py` & `saic_ismart_client-1.1.5/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.4/tests/test_ws_api.py` & `saic_ismart_client-1.1.5/tests/test_ws_api.py`

 * *Files identical despite different names*

