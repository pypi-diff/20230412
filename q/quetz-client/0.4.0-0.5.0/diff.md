# Comparing `tmp/quetz_client-0.4.0.tar.gz` & `tmp/quetz_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quetz_client-0.4.0.tar", last modified: Fri Apr  7 11:37:27 2023, max compression
+gzip compressed data, was "quetz_client-0.5.0.tar", last modified: Wed Apr 12 06:32:41 2023, max compression
```

## Comparing `quetz_client-0.4.0.tar` & `quetz_client-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:37:27.716427 quetz_client-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-07 11:36:41.000000 quetz_client-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-07 11:37:27.716427 quetz_client-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-07 11:36:41.000000 quetz_client-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-07 11:36:55.000000 quetz_client-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-07 11:37:27.716427 quetz_client-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:37:27.716427 quetz_client-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:37:27.716427 quetz_client-0.4.0/src/quetz_client/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-07 11:36:41.000000 quetz_client-0.4.0/src/quetz_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-07 11:36:55.000000 quetz_client-0.4.0/src/quetz_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-07 11:36:41.000000 quetz_client-0.4.0/src/quetz_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-04-07 11:36:41.000000 quetz_client-0.4.0/src/quetz_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:37:27.716427 quetz_client-0.4.0/src/quetz_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-07 11:37:27.000000 quetz_client-0.4.0/src/quetz_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-07 11:37:27.000000 quetz_client-0.4.0/src/quetz_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:37:27.000000 quetz_client-0.4.0/src/quetz_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-07 11:37:27.000000 quetz_client-0.4.0/src/quetz_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-07 11:37:27.000000 quetz_client-0.4.0/src/quetz_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 11:37:27.000000 quetz_client-0.4.0/src/quetz_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:37:27.716427 quetz_client-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-07 11:36:41.000000 quetz_client-0.4.0/tests/test_both.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-07 11:36:41.000000 quetz_client-0.4.0/tests/test_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-07 11:36:41.000000 quetz_client-0.4.0/tests/test_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:32:41.279534 quetz_client-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-12 06:31:50.000000 quetz_client-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-12 06:32:41.279534 quetz_client-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 06:31:50.000000 quetz_client-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-12 06:32:05.000000 quetz_client-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-12 06:32:41.279534 quetz_client-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:32:41.275534 quetz_client-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:32:41.275534 quetz_client-0.5.0/src/quetz_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 06:31:50.000000 quetz_client-0.5.0/src/quetz_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 06:32:05.000000 quetz_client-0.5.0/src/quetz_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-12 06:31:50.000000 quetz_client-0.5.0/src/quetz_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-04-12 06:31:50.000000 quetz_client-0.5.0/src/quetz_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:32:41.279534 quetz_client-0.5.0/src/quetz_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-12 06:32:41.000000 quetz_client-0.5.0/src/quetz_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 06:32:41.000000 quetz_client-0.5.0/src/quetz_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:32:41.000000 quetz_client-0.5.0/src/quetz_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 06:32:41.000000 quetz_client-0.5.0/src/quetz_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 06:32:41.000000 quetz_client-0.5.0/src/quetz_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 06:32:41.000000 quetz_client-0.5.0/src/quetz_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:32:41.279534 quetz_client-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-12 06:31:50.000000 quetz_client-0.5.0/tests/test_both.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-12 06:31:50.000000 quetz_client-0.5.0/tests/test_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-12 06:31:50.000000 quetz_client-0.5.0/tests/test_mock.py
```

### Comparing `quetz_client-0.4.0/LICENSE` & `quetz_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quetz_client-0.4.0/PKG-INFO` & `quetz_client-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: quetz_client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python client to interact with a Quetz server.
 Home-page: https://github.com/mamba-org/quetz-client
 Author: QuantCo, Inc.
 Author-email: noreply@quantco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quetz-client
 
-A Python client to interact with a Quetz server. Compatible with `quetz>=0.6.1`.
+A Python client to interact with a Quetz server. This client is compatible with all `quetz` versions listed [here](./.quetz-server-versions).
 
 ## Installation
 
 ### From conda-forge
 
 ```bash
 mamba install quetz-client
```

### Comparing `quetz_client-0.4.0/README.md` & `quetz_client-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # quetz-client
 
-A Python client to interact with a Quetz server. Compatible with `quetz>=0.6.1`.
+A Python client to interact with a Quetz server. This client is compatible with all `quetz` versions listed [here](./.quetz-server-versions).
 
 ## Installation
 
 ### From conda-forge
 
 ```bash
 mamba install quetz-client
```

### Comparing `quetz_client-0.4.0/pyproject.toml` & `quetz_client-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 check_untyped_defs = true
 
 [tool.pytest.ini_options]
 # This will be pytest's future default.
 addopts = "--import-mode=importlib"
 
 [tool.tbump.version]
-current = "0.4.0"
+current = "0.5.0"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [[tool.tbump.field]]
 name = "channel"
```

### Comparing `quetz_client-0.4.0/setup.cfg` & `quetz_client-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `quetz_client-0.4.0/src/quetz_client/cli.py` & `quetz_client-0.5.0/src/quetz_client/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional
+from typing import Optional, cast
 
 import fire
 from requests.adapters import HTTPAdapter, Retry
 
 from quetz_client.client import QuetzClient
 
 
@@ -30,25 +30,29 @@
     insecure: bool
         Allow quetz-client to perform "insecure" SSL connections.
 
     retry: bool
         Allow to retry requests on transient errors and 5xx server
         respones.
     """
-    # Initialize the client
-    url = url or os.environ["QUETZ_SERVER_URL"]
-    token = token or os.environ["QUETZ_API_KEY"]
+    # Initialize the client (do not force the env variables to be set of help on the
+    # subcommands does not work without setting them)
+    url = cast(str, url or os.getenv("QUETZ_SERVER_URL", ""))
+    token = cast(str, token or os.getenv("QUETZ_API_KEY", ""))
     client = QuetzClient.from_token(url, token)
 
     # Configure the client with additional flags passed to the CLI
     client.session.verify = not insecure
     if retry:
         # Retry a total of 10 times, starting with an initial backoff of one second.
         retry_config = Retry(
-            total=10, status_forcelist=range(500, 600), backoff_factor=1
+            total=10,
+            status_forcelist=range(500, 600),
+            backoff_factor=1,
+            allowed_methods=["GET", "POST", "PUT", "DELETE"],
         )
         adapter = HTTPAdapter(max_retries=retry_config)
         client.session.mount(url, adapter)
 
     return client
```

### Comparing `quetz_client-0.4.0/src/quetz_client/client.py` & `quetz_client-0.5.0/src/quetz_client/client.py`

 * *Files identical despite different names*

### Comparing `quetz_client-0.4.0/src/quetz_client.egg-info/PKG-INFO` & `quetz_client-0.5.0/src/quetz_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: quetz-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python client to interact with a Quetz server.
 Home-page: https://github.com/mamba-org/quetz-client
 Author: QuantCo, Inc.
 Author-email: noreply@quantco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quetz-client
 
-A Python client to interact with a Quetz server. Compatible with `quetz>=0.6.1`.
+A Python client to interact with a Quetz server. This client is compatible with all `quetz` versions listed [here](./.quetz-server-versions).
 
 ## Installation
 
 ### From conda-forge
 
 ```bash
 mamba install quetz-client
```

### Comparing `quetz_client-0.4.0/tests/test_both.py` & `quetz_client-0.5.0/tests/test_both.py`

 * *Files identical despite different names*

### Comparing `quetz_client-0.4.0/tests/test_live.py` & `quetz_client-0.5.0/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `quetz_client-0.4.0/tests/test_mock.py` & `quetz_client-0.5.0/tests/test_mock.py`

 * *Files identical despite different names*

