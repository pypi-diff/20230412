# Comparing `tmp/vds-api-client-2.1.5.tar.gz` & `tmp/vds-api-client-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vds-api-client-2.1.5.tar", last modified: Thu Aug 18 06:39:43 2022, max compression
+gzip compressed data, was "vds-api-client-2.1.6.tar", last modified: Wed Apr 12 08:36:07 2023, max compression
```

## Comparing `vds-api-client-2.1.5.tar` & `vds-api-client-2.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.969982 vds-api-client-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.961981 vds-api-client-2.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.965981 vds-api-client-2.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/.github/workflows/test-python-3-6.yml
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12335 2022-08-18 06:39:43.969982 vds-api-client-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11678 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/conda_environment37.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.965981 vds-api-client-2.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9356 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-08-18 06:39:43.969982 vds-api-client-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.961981 vds-api-client-2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.965981 vds-api-client-2.1.5/src/vds_api_client/
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/src/vds_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13091 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/src/vds_api_client/api_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    21038 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/src/vds_api_client/api_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7257 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/src/vds_api_client/requester.py
--rw-r--r--   0 runner    (1001) docker     (121)    11304 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/src/vds_api_client/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    17062 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/src/vds_api_client/vds_api_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.969982 vds-api-client-2.1.5/src/vds_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12335 2022-08-18 06:39:43.000000 vds-api-client-2.1.5/src/vds_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-08-18 06:39:43.000000 vds-api-client-2.1.5/src/vds_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 06:39:43.000000 vds-api-client-2.1.5/src/vds_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-18 06:39:43.000000 vds-api-client-2.1.5/src/vds_api_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 06:39:43.000000 vds-api-client-2.1.5/src/vds_api_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-18 06:39:43.000000 vds-api-client-2.1.5/src/vds_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-18 06:39:43.000000 vds-api-client-2.1.5/src/vds_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.969982 vds-api-client-2.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 06:39:43.969982 vds-api-client-2.1.5/tests/config_files/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/config_files/example_config_area.vds
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/config_files/example_config_ts.vds
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/test_rois.py
--rw-r--r--   0 runner    (1001) docker     (121)     8910 2022-08-18 06:39:26.000000 vds-api-client-2.1.5/tests/test_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.210707 vds-api-client-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.202706 vds-api-client-2.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.206707 vds-api-client-2.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/.github/workflows/test-python-3-6.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-12 08:36:07.210707 vds-api-client-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/conda_environment37.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.206707 vds-api-client-2.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-12 08:36:07.210707 vds-api-client-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.202706 vds-api-client-2.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.206707 vds-api-client-2.1.6/src/vds_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/src/vds_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/src/vds_api_client/api_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/src/vds_api_client/api_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/src/vds_api_client/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/src/vds_api_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17062 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/src/vds_api_client/vds_api_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.206707 vds-api-client-2.1.6/src/vds_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-12 08:36:07.000000 vds-api-client-2.1.6/src/vds_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-12 08:36:07.000000 vds-api-client-2.1.6/src/vds_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:36:07.000000 vds-api-client-2.1.6/src/vds_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 08:36:07.000000 vds-api-client-2.1.6/src/vds_api_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:36:07.000000 vds-api-client-2.1.6/src/vds_api_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 08:36:07.000000 vds-api-client-2.1.6/src/vds_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 08:36:07.000000 vds-api-client-2.1.6/src/vds_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.210707 vds-api-client-2.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:36:07.210707 vds-api-client-2.1.6/tests/config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/config_files/example_config_area.vds
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/config_files/example_config_ts.vds
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/test_rois.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-04-12 08:35:49.000000 vds-api-client-2.1.6/tests/test_v2.py
```

### Comparing `vds-api-client-2.1.5/.coveragerc` & `vds-api-client-2.1.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/.github/workflows/python-publish.yml` & `vds-api-client-2.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/.github/workflows/test-python-3-6.yml` & `vds-api-client-2.1.6/.github/workflows/test-python-3-6.yml`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/.gitignore` & `vds-api-client-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/CHANGELOG.rst` & `vds-api-client-2.1.6/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =========
 Changelog
 =========
 
 Unreleased
 ==========
 
+Version 2.1.6
+=============
+
+- Only start downloading data if status of API request is 'Ready'
+
 Version 2.1.5
 =============
 - Upgrade pyscaffold to 3.3.1
 
 Version 2.1.4
 =============
 - Remove Travis-ci from project
@@ -179,8 +184,8 @@
 - KeyboardInterrupt implementation fixed for multithreading
 - overwrite files swith added
 - debug switch implemented
 - log everything
 - implemented option for using stream
 - added multiple products to getarea command
 - added multiple dates to getarea commands
-- summary of performed operations
+- summary of performed operations
```

### Comparing `vds-api-client-2.1.5/CONTRIBUTING.md` & `vds-api-client-2.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/LICENSE.txt` & `vds-api-client-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/PKG-INFO` & `vds-api-client-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vds-api-client
-Version: 2.1.5
+Version: 2.1.6
 Summary: VanderSat API client package
 Home-page: https://www.planet.com
 Author: Teije
 Author-email: teije@planet.com
 License: mit
 Project-URL: Source Code, https://github.com/vandersat/vds-api-client
 Project-URL: PyPI, https://pypi.org/project/vds-api-client/
```

### Comparing `vds-api-client-2.1.5/README.rst` & `vds-api-client-2.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/docs/Makefile` & `vds-api-client-2.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/docs/conf.py` & `vds-api-client-2.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/docs/index.rst` & `vds-api-client-2.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/requirements.txt` & `vds-api-client-2.1.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/setup.cfg` & `vds-api-client-2.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/setup.py` & `vds-api-client-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/src/vds_api_client/api_cli.py` & `vds-api-client-2.1.6/src/vds_api_client/api_cli.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/src/vds_api_client/api_v2.py` & `vds-api-client-2.1.6/src/vds_api_client/api_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
 
     @retry(wait_exponential_multiplier=5000, wait_exponential_max=15000,
            stop_max_attempt_number=7, retry_on_exception=_no_type_error)
     def _uuid_status(self, uuid, wait_for_complete=True):
         status_url = f'https://{self.host}/api/v2/api-requests/{uuid}/status'
         self.logger.debug(f'Status request for UUID: {uuid}')
         status_dict = self.get_content(status_url)
-        while status_dict['percentage'] < 100 and wait_for_complete:
+        while status_dict['percentage'] < 100 and status_dict['status'] != 'Ready' and wait_for_complete:
             time.sleep(self._wait_time)
             status_dict = self.get_content(status_url)
             _ = sys.stderr.write('\t' * 20 + '\b\r')
             progress_bar(status_dict['percentage'] / 100.0)
         self.logger.info(f'Ready for download UUID: {uuid}')
         return status_dict
```

### Comparing `vds-api-client-2.1.5/src/vds_api_client/requester.py` & `vds-api-client-2.1.6/src/vds_api_client/requester.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/src/vds_api_client/types.py` & `vds-api-client-2.1.6/src/vds_api_client/types.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/src/vds_api_client/vds_api_base.py` & `vds-api-client-2.1.6/src/vds_api_client/vds_api_base.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/src/vds_api_client.egg-info/PKG-INFO` & `vds-api-client-2.1.6/src/vds_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vds-api-client
-Version: 2.1.5
+Version: 2.1.6
 Summary: VanderSat API client package
 Home-page: https://www.planet.com
 Author: Teije
 Author-email: teije@planet.com
 License: mit
 Project-URL: Source Code, https://github.com/vandersat/vds-api-client
 Project-URL: PyPI, https://pypi.org/project/vds-api-client/
```

### Comparing `vds-api-client-2.1.5/src/vds_api_client.egg-info/SOURCES.txt` & `vds-api-client-2.1.6/src/vds_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/tests/conftest.py` & `vds-api-client-2.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/tests/test_api_base.py` & `vds-api-client-2.1.6/tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/tests/test_cli.py` & `vds-api-client-2.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/tests/test_rois.py` & `vds-api-client-2.1.6/tests/test_rois.py`

 * *Files identical despite different names*

### Comparing `vds-api-client-2.1.5/tests/test_v2.py` & `vds-api-client-2.1.6/tests/test_v2.py`

 * *Files identical despite different names*

