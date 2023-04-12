# Comparing `tmp/dhali-py-0.0.5.tar.gz` & `tmp/dhali-py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhali-py-0.0.5.tar", last modified: Mon Mar 20 10:34:12 2023, max compression
+gzip compressed data, was "dhali-py-0.0.6.tar", last modified: Wed Apr 12 13:17:25 2023, max compression
```

## Comparing `dhali-py-0.0.5.tar` & `dhali-py-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.273349 dhali-py-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.269349 dhali-py-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-20 10:34:03.000000 dhali-py-0.0.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.269349 dhali-py-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-20 10:34:03.000000 dhali-py-0.0.5/.github/workflows/package_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-20 10:34:03.000000 dhali-py-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-20 10:34:03.000000 dhali-py-0.0.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-20 10:34:03.000000 dhali-py-0.0.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-03-20 10:34:03.000000 dhali-py-0.0.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-20 10:34:03.000000 dhali-py-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-20 10:34:12.273349 dhali-py-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-20 10:34:03.000000 dhali-py-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.269349 dhali-py-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.269349 dhali-py-0.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-20 10:34:03.000000 dhali-py-0.0.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-20 10:34:03.000000 dhali-py-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-20 10:34:12.273349 dhali-py-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-20 10:34:03.000000 dhali-py-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.269349 dhali-py-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.269349 dhali-py-0.0.5/src/dhali/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-20 10:34:03.000000 dhali-py-0.0.5/src/dhali/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-03-20 10:34:03.000000 dhali-py-0.0.5/src/dhali/transaction_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.273349 dhali-py-0.0.5/src/dhali_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-20 10:34:12.000000 dhali-py-0.0.5/src/dhali_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-20 10:34:12.000000 dhali-py-0.0.5/src/dhali_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:34:12.000000 dhali-py-0.0.5/src/dhali_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:34:11.000000 dhali-py-0.0.5/src/dhali_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-20 10:34:12.000000 dhali-py-0.0.5/src/dhali_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-20 10:34:12.000000 dhali-py-0.0.5/src/dhali_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:34:12.273349 dhali-py-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-20 10:34:03.000000 dhali-py-0.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-20 10:34:03.000000 dhali-py-0.0.5/tests/test_transaction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-20 10:34:03.000000 dhali-py-0.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 13:17:16.000000 dhali-py-0.0.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 13:17:16.000000 dhali-py-0.0.6/.github/workflows/package_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-12 13:17:16.000000 dhali-py-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-12 13:17:16.000000 dhali-py-0.0.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 13:17:16.000000 dhali-py-0.0.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-04-12 13:17:16.000000 dhali-py-0.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-12 13:17:16.000000 dhali-py-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-12 13:17:25.213679 dhali-py-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 13:17:16.000000 dhali-py-0.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 13:17:16.000000 dhali-py-0.0.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 13:17:16.000000 dhali-py-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-12 13:17:25.213679 dhali-py-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-12 13:17:16.000000 dhali-py-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.209679 dhali-py-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/src/dhali/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-12 13:17:16.000000 dhali-py-0.0.6/src/dhali/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-12 13:17:16.000000 dhali-py-0.0.6/src/dhali/transaction_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/src/dhali_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-12 13:17:25.000000 dhali-py-0.0.6/src/dhali_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 13:17:25.000000 dhali-py-0.0.6/src/dhali_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:17:25.000000 dhali-py-0.0.6/src/dhali_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:17:24.000000 dhali-py-0.0.6/src/dhali_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-12 13:17:25.000000 dhali-py-0.0.6/src/dhali_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 13:17:25.000000 dhali-py-0.0.6/src/dhali_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:17:25.213679 dhali-py-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-12 13:17:16.000000 dhali-py-0.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-12 13:17:16.000000 dhali-py-0.0.6/tests/test_transaction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-12 13:17:16.000000 dhali-py-0.0.6/tox.ini
```

### Comparing `dhali-py-0.0.5/.github/workflows/package_test.yaml` & `dhali-py-0.0.6/.github/workflows/package_test.yaml`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/.github/workflows/release.yaml` & `dhali-py-0.0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/CONTRIBUTING.rst` & `dhali-py-0.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/LICENSE` & `dhali-py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/PKG-INFO` & `dhali-py-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhali-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for interfacing with Dhali
 Home-page: https://github.com/Dhali-org/Dhali-py
 Author: Dhali Holdings Ltd
 Author-email: engagement@dhali.io
 License: BSD 3-Clause License
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dhali-py-0.0.5/README.rst` & `dhali-py-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/docs/Makefile` & `dhali-py-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/docs/conf.py` & `dhali-py-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/docs/index.rst` & `dhali-py-0.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/setup.cfg` & `dhali-py-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/setup.py` & `dhali-py-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/src/dhali/__init__.py` & `dhali-py-0.0.6/src/dhali/__init__.py`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/src/dhali/transaction_utils.py` & `dhali-py-0.0.6/src/dhali/transaction_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         return to_claim
     else:
         raise HTTPException(status_code=402)
 
 
 # TODO - Test this!
 async def validate_claim(
-    client, claim, single_request_cost_estimate: int, db, settle_delay=15768000
+    client, claim, single_request_cost_estimate: int, db, destination_account: str, settle_delay=15768000
 ):
     """
     TODO
 
     Parameters
     ----------
     client : xrpl.clients.JsonRpcClient
@@ -273,14 +273,22 @@
 
     for key in keys:
         if key not in parsed_claim.keys():
             raise HTTPException(
                 status_code=402,
                 detail=f"Your claim must be in Json format, providing the following fields: {keys}",
             )
+
+    if destination_account != parsed_claim["destination_account"]:
+        raise HTTPException(
+            status_code=402,
+            detail=f"Your claim has an incorrect destination_account",
+        )
+
+
     uuid_channel_id = str(uuid.uuid5(uuid.NAMESPACE_URL, parsed_claim["channel_id"]))
     collection_name = "payment_channels"
 
     transaction = db.transaction()
     payment_claim_doc_ref = db.collection(collection_name).document(uuid_channel_id)
     to_claim = transactional_validation(
         transaction,
```

### Comparing `dhali-py-0.0.5/src/dhali_py.egg-info/PKG-INFO` & `dhali-py-0.0.6/src/dhali_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhali-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for interfacing with Dhali
 Home-page: https://github.com/Dhali-org/Dhali-py
 Author: Dhali Holdings Ltd
 Author-email: engagement@dhali.io
 License: BSD 3-Clause License
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dhali-py-0.0.5/src/dhali_py.egg-info/SOURCES.txt` & `dhali-py-0.0.6/src/dhali_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/tests/test_transaction_utils.py` & `dhali-py-0.0.6/tests/test_transaction_utils.py`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.5/tox.ini` & `dhali-py-0.0.6/tox.ini`

 * *Files identical despite different names*

