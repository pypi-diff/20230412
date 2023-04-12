# Comparing `tmp/dvc-studio-client-0.6.1.tar.gz` & `tmp/dvc-studio-client-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-studio-client-0.6.1.tar", last modified: Wed Mar 15 21:05:47 2023, max compression
+gzip compressed data, was "dvc-studio-client-0.6.2.tar", last modified: Wed Apr 12 08:59:25 2023, max compression
```

## Comparing `dvc-studio-client-0.6.1.tar` & `dvc-studio-client-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.902802 dvc-studio-client-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.898802 dvc-studio-client-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.898802 dvc-studio-client-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.898802 dvc-studio-client-0.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-03-15 21:05:47.902802 dvc-studio-client-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.898802 dvc-studio-client-0.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.898802 dvc-studio-client-0.6.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-15 21:05:47.902802 dvc-studio-client-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.898802 dvc-studio-client-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.902802 dvc-studio-client-0.6.1/src/dvc_studio_client/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/src/dvc_studio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/src/dvc_studio_client/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/src/dvc_studio_client/post_live_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/src/dvc_studio_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/src/dvc_studio_client/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.902802 dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-03-15 21:05:47.000000 dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-15 21:05:47.000000 dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:05:47.000000 dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:05:47.000000 dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-15 21:05:47.000000 dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-15 21:05:47.000000 dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:47.902802 dvc-studio-client-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-03-15 21:05:36.000000 dvc-studio-client-0.6.1/tests/test_post_live_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.475060 dvc-studio-client-0.6.2/src/dvc_studio_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/post_live_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/src/dvc_studio_client/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 08:59:25.000000 dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:59:25.479060 dvc-studio-client-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-04-12 08:59:15.000000 dvc-studio-client-0.6.2/tests/test_post_live_metrics.py
```

### Comparing `dvc-studio-client-0.6.1/.cruft.json` & `dvc-studio-client-0.6.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/.github/dependabot.yml` & `dvc-studio-client-0.6.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/.github/workflows/docs.yml` & `dvc-studio-client-0.6.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/.github/workflows/pre-commit.yml` & `dvc-studio-client-0.6.2/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/.github/workflows/release.yml` & `dvc-studio-client-0.6.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/.github/workflows/tests.yml` & `dvc-studio-client-0.6.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/.gitignore` & `dvc-studio-client-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/.pre-commit-config.yaml` & `dvc-studio-client-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/CODE_OF_CONDUCT.rst` & `dvc-studio-client-0.6.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/CONTRIBUTING.rst` & `dvc-studio-client-0.6.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/LICENSE` & `dvc-studio-client-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/PKG-INFO` & `dvc-studio-client-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/DVC Studio Client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.6.1/README.rst` & `dvc-studio-client-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/docs/assets/logo.svg` & `dvc-studio-client-0.6.2/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/docs/gen_ref_pages.py` & `dvc-studio-client-0.6.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/mkdocs.yml` & `dvc-studio-client-0.6.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/pyproject.toml` & `dvc-studio-client-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/setup.cfg` & `dvc-studio-client-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/src/dvc_studio_client/post_live_metrics.py` & `dvc-studio-client-0.6.2/src/dvc_studio_client/post_live_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/src/dvc_studio_client/schema.py` & `dvc-studio-client-0.6.2/src/dvc_studio_client/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from voluptuous import All, Any, Lower, Match, Required, Schema
+from voluptuous import All, Any, Exclusive, Lower, Match, Required, Schema
 
 
 def Choices(*choices):
     """Checks that value belongs to the specified set of values"""
     return Any(*choices, msg=f"expected one of {', '.join(choices)}")
 
 
@@ -28,15 +28,22 @@
     }
 )
 SCHEMAS_BY_TYPE = {
     "start": BASE_SCHEMA,
     "data": BASE_SCHEMA.extend(
         {
             Required("step"): int,
-            "plots": {str: {"data": [dict], "props": dict, "error": ERROR_SCHEMA}},
+            "plots": {
+                str: {
+                    Exclusive("data", "data"): [dict],
+                    "props": dict,
+                    "error": ERROR_SCHEMA,
+                    Exclusive("image", "data"): str,
+                }
+            },
         }
     ),
     "done": BASE_SCHEMA.extend(
         {
             "experiment_rev": Sha,
         }
     ),
```

### Comparing `dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/PKG-INFO` & `dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/DVC Studio Client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.6.1/src/dvc_studio_client.egg-info/SOURCES.txt` & `dvc-studio-client-0.6.2/src/dvc_studio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.6.1/tests/test_post_live_metrics.py` & `dvc-studio-client-0.6.2/tests/test_post_live_metrics.py`

 * *Files identical despite different names*

