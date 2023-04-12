# Comparing `tmp/pyatlan-0.0.21.tar.gz` & `tmp/pyatlan-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.21.tar", last modified: Tue Apr 11 12:30:56 2023, max compression
+gzip compressed data, was "pyatlan-0.0.22.tar", last modified: Wed Apr 12 16:58:44 2023, max compression
```

## Comparing `pyatlan-0.0.21.tar` & `pyatlan-0.0.22.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.171042 pyatlan-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-11 12:30:46.000000 pyatlan-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 12:30:46.000000 pyatlan-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 12:30:46.000000 pyatlan-0.0.21/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-11 12:30:56.167042 pyatlan-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 12:30:46.000000 pyatlan-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   745939 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:30:55.000000 pyatlan-0.0.21/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:30:56.171042 pyatlan-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-11 12:30:46.000000 pyatlan-0.0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29930 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    48559 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.774000 pyatlan-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-12 16:58:34.000000 pyatlan-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:58:34.000000 pyatlan-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 16:58:34.000000 pyatlan-0.0.22/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-12 16:58:44.774000 pyatlan-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 16:58:34.000000 pyatlan-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.766000 pyatlan-0.0.22/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   748743 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.766000 pyatlan-0.0.22/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:58:44.774000 pyatlan-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-12 16:58:34.000000 pyatlan-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.774000 pyatlan-0.0.22/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.774000 pyatlan-0.0.22/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48559 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.21/LICENSE` & `pyatlan-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/PKG-INFO` & `pyatlan-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.21
+Version: 0.0.22
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.21/README.md` & `pyatlan-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.22/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.22/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/cache/role_cache.py` & `pyatlan-0.0.22/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/client/atlan.py` & `pyatlan-0.0.22/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/client/constants.py` & `pyatlan-0.0.22/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/error.py` & `pyatlan-0.0.22/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/exceptions.py` & `pyatlan-0.0.22/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.22/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/model/assets.py` & `pyatlan-0.0.22/pyatlan/model/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -9094,14 +9094,15 @@
                 database_name=fields[3],
                 connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
                 database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
                 connector_name=connector_type.value,
+                atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
     attributes: "Table.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
@@ -10017,14 +10018,71 @@
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
         column_dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
             None, description="", alias="columnDbtModelColumns"
         )  # relationship
 
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls, *, name: str, parent_qualified_name: str, parent_type: type, order: int
+        ) -> Column.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(["parent_qualified_name"], [parent_qualified_name])
+            fields = parent_qualified_name.split("/")
+            if len(fields) != 6:
+                raise ValueError("Invalid parent_qualified_name")
+            try:
+                connector_type = AtlanConnectorType(fields[1])  # type:ignore
+            except ValueError as e:
+                raise ValueError("Invalid parent_qualified_name") from e
+            ret_value = Column.Attributes(
+                name=name,
+                qualified_name=f"{parent_qualified_name}/{name}",
+                connector_name=connector_type.value,
+                schema_name=fields[4],
+                schema_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}/{fields[4]}",
+                database_name=fields[3],
+                database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
+                connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
+                order=order,
+            )
+            if parent_type == Table:
+                ret_value.table_qualified_name = parent_qualified_name
+                ret_value.table = Table.ref_by_qualified_name(parent_qualified_name)
+            elif parent_type == View:
+                ret_value.view_qualified_name = parent_qualified_name
+                ret_value.view = View.ref_by_qualified_name(parent_qualified_name)
+            elif parent_type == MaterialisedView:
+                ret_value.view_qualified_name = parent_qualified_name
+                ret_value.materialised_view = MaterialisedView.ref_by_qualified_name(
+                    parent_qualified_name
+                )
+            else:
+                raise ValueError(
+                    "parent_type must be either Table, View or MaterializeView"
+                )
+            return ret_value
+
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls, *, name: str, parent_qualified_name: str, parent_type: type, order: int
+    ) -> Column:
+        return Column(
+            attributes=Column.Attributes.create(
+                name=name,
+                parent_qualified_name=parent_qualified_name,
+                parent_type=parent_type,
+                order=order,
+            )
+        )
+
     attributes: "Column.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
@@ -10144,14 +10202,15 @@
             return Schema.Attributes(
                 name=name,
                 database_name=fields[3],
                 connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
                 database_qualified_name=database_qualified_name,
                 qualified_name=f"{database_qualified_name}/{name}",
                 connector_name=connector_type.value,
+                database=Database.ref_by_qualified_name(database_qualified_name),
             )
 
     attributes: "Schema.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
@@ -10781,14 +10840,15 @@
                 database_name=fields[3],
                 connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
                 database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
                 connector_name=connector_type.value,
+                atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
     attributes: "View.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
```

### Comparing `pyatlan-0.0.21/pyatlan/model/core.py` & `pyatlan-0.0.22/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/model/enums.py` & `pyatlan-0.0.22/pyatlan/model/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -194,14 +194,25 @@
     DATABASE = "database"
     API = "API"
 
 
 class AtlanConnectorType(str, Enum):
     category: AtlanConnectionCategory
 
+    @classmethod
+    def _get_connector_type_from_qualified_name(
+        cls, qualified_name: str
+    ) -> "AtlanConnectorType":
+        tokens = qualified_name.split("/")
+        if len(tokens) > 1:
+            return AtlanConnectorType[tokens[1].upper()]
+        raise ValueError(
+            f"Could not determine AtlanConnectorType from {qualified_name}"
+        )
+
     def __new__(
         cls, value: str, category: AtlanConnectionCategory
     ) -> "AtlanConnectorType":
         obj = str.__new__(cls, value)
         obj._value_ = value
         obj.category = category
         return obj
```

### Comparing `pyatlan-0.0.21/pyatlan/model/response.py` & `pyatlan-0.0.22/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/model/role.py` & `pyatlan-0.0.22/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/model/search.py` & `pyatlan-0.0.22/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/model/structs.py` & `pyatlan-0.0.22/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/model/typedef.py` & `pyatlan-0.0.22/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan/utils.py` & `pyatlan-0.0.22/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.22/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.21
+Version: 0.0.22
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.21/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.22/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/setup.py` & `pyatlan-0.0.22/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/integration/classification_test.py` & `pyatlan-0.0.22/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.22/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/integration/role_test.py` & `pyatlan-0.0.22/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/integration/test_entity_model.py` & `pyatlan-0.0.22/tests/integration/test_entity_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import os
 import random
 import string
-import time
 
 import pytest
 import requests
 
 from pyatlan.cache.role_cache import RoleCache
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.error import NotFoundError
@@ -38,14 +37,15 @@
     "711b6004-1b84-49fe-ac42-e0d42bfa01fc",
     "34d8106a-1478-4816-bfe1-97814ffff78e",
     "04a4eca5-b7d5-4659-bbad-1dc2306ea9c3",
     "619daa76-ab3c-4f29-836a-6ec0ddefbe0c",
     "4af8d57c-61ef-4b57-983c-eff20e6d08b5",
     "57f5463d-cc2a-4859-bf28-e4fa52002e8e",
 }
+TEMP_CONNECTION_GUID = "b3a5c49a-0c7c-4e66-8453-f4da8d9ce222"
 
 
 @pytest.fixture(scope="module")
 def client() -> AtlanClient:
     return AtlanClient()
 
 
@@ -81,21 +81,21 @@
 
 def get_environment_variable(name) -> str:
     ret_value = os.environ[name]
     assert ret_value
     return ret_value
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def increment_counter():
-    i = random.randint(0, 1000)
+    i = 700
 
     def increment():
         nonlocal i
-        i += 1
+        i += 20
         return i
 
     return increment
 
 
 @pytest.fixture()
 def glossary_guids(atlan_host, headers):
@@ -183,14 +183,15 @@
         "AtlasGlossaryCategory",
         "AtlasGlossary",
         "Table",
         "Schema",
         "Database",
         "Connection",
         "View",
+        "Column",
     ]
     for type_name in type_names:
         print()
         delete_assets(atlan_host, headers, type_name)
     yield
     for type_name in type_names:
         delete_assets(atlan_host, headers, type_name)
@@ -519,157 +520,133 @@
     c = response.mutated_entities.CREATE[0]
     assert guid == c.guid
     c = client.get_asset_by_guid(c.guid, Connection)
     assert isinstance(c, Connection)
     assert c.guid == guid
 
 
-@pytest.mark.skip("Connection creation is still intermittently failing")
 def test_create_database(client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     suffix = increment_counter()
-    connection = Connection.create(
-        name=f"Integration {suffix}",
-        connector_type=AtlanConnectorType.SNOWFLAKE,
-        admin_roles=[role],
-        admin_groups=["admin"],
-    )
-    response = client.upsert(connection)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert isinstance(response.mutated_entities.CREATE[0], Connection)
-    connection = response.mutated_entities.CREATE[0]
-    connection = client.get_asset_by_guid(connection.guid, Connection)
+    # connection = Connection.create(
+    #     name=f"Integration {suffix}",
+    #     connector_type=AtlanConnectorType.SNOWFLAKE,
+    #     admin_roles=[role],
+    #     admin_groups=["admin"],
+    # )
+    # response = client.upsert(connection)
+    # assert response.mutated_entities
+    # assert response.mutated_entities.CREATE
+    # assert isinstance(response.mutated_entities.CREATE[0], Connection)
+    # connection = response.mutated_entities.CREATE[0]
+    # connection = client.get_asset_by_guid(connection.guid, Connection)
+    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
     database = Database.create(
         name=f"Integration_{suffix}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
     response = client.upsert(database)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     assert isinstance(response.mutated_entities.CREATE[0], Database)
     assert response.guid_assignments
-    assert database.guid in response.guid_assignments
-    guid = response.guid_assignments[database.guid]
     database = response.mutated_entities.CREATE[0]
-    assert guid == database.guid
-    database = client.get_asset_by_guid(guid, Database)
-    assert isinstance(database, Database)
-    assert guid == database.guid
+    client.get_asset_by_guid(database.guid, Database)
 
 
-@pytest.mark.skip("Connection creation is still intermittently failing")
 def test_create_schema(client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     suffix = increment_counter()
-    connection = Connection.create(
-        name=f"Integration {suffix}",
-        connector_type=AtlanConnectorType.SNOWFLAKE,
-        admin_roles=[role],
-        admin_groups=["admin"],
-    )
-    response = client.upsert(connection)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert isinstance(response.mutated_entities.CREATE[0], Connection)
-    connection = response.mutated_entities.CREATE[0]
-    time.sleep(30)
-    connection = client.get_asset_by_guid(connection.guid, Connection)
+    # connection = Connection.create(
+    #     name=f"Integration {suffix}",
+    #     connector_type=AtlanConnectorType.SNOWFLAKE,
+    #     admin_roles=[role],
+    #     admin_groups=["admin"],
+    # )
+    # response = client.upsert(connection)
+    # assert response.mutated_entities
+    # assert response.mutated_entities.CREATE
+    # assert isinstance(response.mutated_entities.CREATE[0], Connection)
+    # connection = response.mutated_entities.CREATE[0]
+    # time.sleep(30)
+    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
     database = Database.create(
         name=f"Integration_{suffix}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
     response = client.upsert(database)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert isinstance(response.mutated_entities.CREATE[0], Database)
-    database = response.mutated_entities.CREATE[0]
-    time.sleep(3)
-    database = client.get_asset_by_guid(database.guid, Database)
+    assert (databases := response.assets_created(asset_type=Database))
+    assert len(databases) == 1
+    database = client.get_asset_by_guid(databases[0].guid, Database)
     schema = Schema.create(
         name=f"Integration_{suffix}",
         database_qualified_name=database.attributes.qualified_name,
     )
     response = client.upsert(schema)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert len(response.mutated_entities.CREATE) == 1
-    assert isinstance(response.mutated_entities.CREATE[0], Schema)
-    assert response.guid_assignments
-    assert schema.guid in response.guid_assignments
-    guid = response.guid_assignments[schema.guid]
-    schema = response.mutated_entities.CREATE[0]
-    assert guid == schema.guid
-    time.sleep(3)
-    schema = client.get_asset_by_guid(guid, Schema)
-    assert isinstance(schema, Schema)
-    assert guid == schema.guid
+    assert (schemas := response.assets_created(asset_type=Schema))
+    assert len(schemas) == 1
+    schema = client.get_asset_by_guid(schemas[0].guid, Schema)
+    assert (databases := response.assets_updated(asset_type=Database))
+    assert len(databases) == 1
+    database = client.get_asset_by_guid(databases[0].guid, Database)
+    assert database.attributes.schemas
+    schemas = database.attributes.schemas
+    assert len(schemas) == 1
+    assert schemas[0].guid == schema.guid
 
 
-@pytest.mark.skip("Connection creation is still intermittently failing")
 def test_create_table(client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     suffix = increment_counter()
-    connection = Connection.create(
-        name=f"Integration {suffix}",
-        connector_type=AtlanConnectorType.SNOWFLAKE,
-        admin_roles=[role],
-        admin_groups=["admin"],
-    )
-    response = client.upsert(connection)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert isinstance(response.mutated_entities.CREATE[0], Connection)
-    connection = response.mutated_entities.CREATE[0]
-    time.sleep(30)
-    connection = client.get_asset_by_guid(connection.guid, Connection)
+    # connection = Connection.create(
+    #     name=f"Integration {suffix}",
+    #     connector_type=AtlanConnectorType.SNOWFLAKE,
+    #     admin_roles=[role],
+    #     admin_groups=["admin"],
+    # )
+    # response = client.upsert(connection)
+    # assert response.mutated_entities
+    # assert response.mutated_entities.CREATE
+    # assert isinstance(response.mutated_entities.CREATE[0], Connection)
+    # connection = response.mutated_entities.CREATE[0]
+    # time.sleep(30)
+    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
     database = Database.create(
         name=f"Integration_{suffix}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
     response = client.upsert(database)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert isinstance(response.mutated_entities.CREATE[0], Database)
-    database = response.mutated_entities.CREATE[0]
-    time.sleep(3)
-    database = client.get_asset_by_guid(database.guid, Database)
+    assert (databases := response.assets_created(asset_type=Database))
+    database = client.get_asset_by_guid(databases[0].guid, Database)
     schema = Schema.create(
         name=f"Integration_{suffix}",
         database_qualified_name=database.attributes.qualified_name,
     )
     response = client.upsert(schema)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert isinstance(response.mutated_entities.CREATE[0], Schema)
-    schema = response.mutated_entities.CREATE[0]
-    time.sleep(3)
-    schema = client.get_asset_by_guid(schema.guid, Schema)
+    assert (schemas := response.assets_created(asset_type=Schema))
+    schema = client.get_asset_by_guid(schemas[0].guid, Schema)
     table = Table.create(
         name=f"Integration_{suffix}",
         schema_qualified_name=schema.attributes.qualified_name,
     )
     response = client.upsert(table)
-    assert response.mutated_entities
-    assert response.mutated_entities.CREATE
-    assert len(response.mutated_entities.CREATE) == 1
-    assert isinstance(response.mutated_entities.CREATE[0], Table)
-    assert response.guid_assignments
-    assert table.guid in response.guid_assignments
-    guid = response.guid_assignments[table.guid]
-    table = response.mutated_entities.CREATE[0]
-    assert guid == table.guid
-    time.sleep(3)
-    table = client.get_asset_by_guid(guid, Table)
-    assert isinstance(table, Table)
-    assert guid == table.guid
+    assert (tables := response.assets_created(asset_type=Table))
+    assert len(tables) == 1
+    table = client.get_asset_by_guid(guid=tables[0].guid, asset_type=Table)
+    assert (schemas := response.assets_updated(asset_type=Schema))
+    assert len(schemas) == 1
+    schema = client.get_asset_by_guid(guid=schemas[0].guid, asset_type=Schema)
+    assert schema.attributes.tables
+    tables = schema.attributes.tables
+    assert len(tables) == 1
+    assert tables[0].guid == table.guid
 
 
 def test_get_by_qualified_name(client: AtlanClient):
     qualified_name = "default/snowflake/1646836521/ATLAN_SAMPLE_DATA/DBT_SARORA/RAW_CUSTOMERS/LAST_NAME"
     column = client.get_asset_by_qualified_name(
         qualified_name=qualified_name, asset_type=Column
     )
@@ -690,14 +667,69 @@
     assert response.guid_assignments
     assert view.guid in response.guid_assignments
     guid = response.guid_assignments[view.guid]
     view = response.mutated_entities.CREATE[0]
     assert guid == view.guid
 
 
+def test_create_column(client: AtlanClient, increment_counter):
+    role = RoleCache.get_id_for_name("$admin")
+    assert role
+    suffix = increment_counter()
+    # connection = Connection.create(
+    #     name=f"Integration {suffix}",
+    #     connector_type=AtlanConnectorType.SNOWFLAKE,
+    #     admin_roles=[role],
+    #     admin_groups=["admin"],
+    # )
+    # response = client.upsert(connection)
+    # assert response.mutated_entities
+    # assert response.mutated_entities.CREATE
+    # assert isinstance(response.mutated_entities.CREATE[0], Connection)
+    # connection = response.mutated_entities.CREATE[0]
+    # time.sleep(30)
+    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
+    database = Database.create(
+        name=f"Integration_{suffix}",
+        connection_qualified_name=connection.attributes.qualified_name,
+    )
+    response = client.upsert(database)
+    assert (databases := response.assets_created(asset_type=Database))
+    database = client.get_asset_by_guid(databases[0].guid, Database)
+    schema = Schema.create(
+        name=f"Integration_{suffix}",
+        database_qualified_name=database.attributes.qualified_name,
+    )
+    response = client.upsert(schema)
+    assert (schemas := response.assets_created(asset_type=Schema))
+    schema = client.get_asset_by_guid(schemas[0].guid, Schema)
+    table = Table.create(
+        name=f"Integration_{suffix}",
+        schema_qualified_name=schema.attributes.qualified_name,
+    )
+    response = client.upsert(table)
+    assert (tables := response.assets_created(asset_type=Table))
+    table = client.get_asset_by_guid(guid=tables[0].guid, asset_type=Table)
+    column = Column.create(
+        name=f"Integration_{suffix}_column",
+        parent_qualified_name=table.qualified_name,
+        parent_type=Table,
+        order=1,
+    )
+    response = client.upsert(column)
+    assert (columns := response.assets_created(asset_type=Column))
+    assert len(columns) == 1
+    column = client.get_asset_by_guid(asset_type=Column, guid=columns[0].guid)
+    table = client.get_asset_by_guid(asset_type=Table, guid=table.guid)
+    assert table.attributes.columns
+    columns = table.attributes.columns
+    assert len(columns) == 1
+    assert columns[0].guid == column.guid
+
+
 def test_add_and_remove_classifications(client: AtlanClient):
     glossary = AtlasGlossary.create(name="Integration Classification Test")
     glossary.attributes.user_description = "This is a description of the glossary"
     glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
     glossary_term = AtlasGlossaryTerm.create(
         name="Integration Classification Term", anchor=glossary
     )
```

### Comparing `pyatlan-0.0.21/tests/integration/test_index_search.py` & `pyatlan-0.0.22/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/unit/test_classification_name.py` & `pyatlan-0.0.22/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/unit/test_glossary_term.py` & `pyatlan-0.0.22/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/unit/test_model.py` & `pyatlan-0.0.22/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/unit/test_search_model.py` & `pyatlan-0.0.22/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.21/tests/unit/test_typedef_model.py` & `pyatlan-0.0.22/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

