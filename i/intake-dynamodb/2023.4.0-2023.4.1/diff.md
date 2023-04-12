# Comparing `tmp/intake-dynamodb-2023.4.0.tar.gz` & `tmp/intake-dynamodb-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-dynamodb-2023.4.0.tar", last modified: Wed Apr 12 17:44:34 2023, max compression
+gzip compressed data, was "intake-dynamodb-2023.4.1.tar", last modified: Wed Apr 12 18:06:50 2023, max compression
```

## Comparing `intake-dynamodb-2023.4.0.tar` & `intake-dynamodb-2023.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/.ciocheck
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.836751 intake-dynamodb-2023.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/intake_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/intake_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/intake_dynamodb/dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 17:44:34.000000 intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-12 17:44:34.000000 intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:44:34.000000 intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 17:44:34.000000 intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 17:44:34.000000 intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 17:44:34.000000 intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.836751 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-files.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:44:34.840751 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-files.json
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-04-12 17:44:21.000000 intake-dynamodb-2023.4.0/tests/test_dynamodb_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.ciocheck
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/intake_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/intake_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/intake_dynamodb/dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/test_dynamodb_catalog.py
```

### Comparing `intake-dynamodb-2023.4.0/.ciocheck` & `intake-dynamodb-2023.4.1/.ciocheck`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/.github/workflows/python-package.yml` & `intake-dynamodb-2023.4.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/.github/workflows/python-publish.yml` & `intake-dynamodb-2023.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/.gitignore` & `intake-dynamodb-2023.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/.pre-commit-config.yaml` & `intake-dynamodb-2023.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/LICENSE` & `intake-dynamodb-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/PKG-INFO` & `intake-dynamodb-2023.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-dynamodb
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Intake plugin for reading data from dynamodb
 Author-email: Ray Bell <rayjohnbell0@gmail.com>
 Project-URL: repository, https://github.com/intake-dynamodb/intake-dynamodb
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `intake-dynamodb-2023.4.0/intake_dynamodb/dynamodb.py` & `intake-dynamodb-2023.4.1/intake_dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/PKG-INFO` & `intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-dynamodb
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Intake plugin for reading data from dynamodb
 Author-email: Ray Bell <rayjohnbell0@gmail.com>
 Project-URL: repository, https://github.com/intake-dynamodb/intake-dynamodb
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `intake-dynamodb-2023.4.0/intake_dynamodb.egg-info/SOURCES.txt` & `intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/pyproject.toml` & `intake-dynamodb-2023.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json` & `intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json` & `intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/tests/conftest.py` & `intake-dynamodb-2023.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/tests/test.yaml` & `intake-dynamodb-2023.4.1/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.0/tests/test_dynamodb_catalog.py` & `intake-dynamodb-2023.4.1/tests/test_dynamodb_catalog.py`

 * *Files identical despite different names*

