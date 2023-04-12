# Comparing `tmp/pydash-6.0.2.tar.gz` & `tmp/pydash-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash-6.0.2.tar", last modified: Fri Feb 24 03:01:27 2023, max compression
+gzip compressed data, was "pydash-7.0.0.tar", last modified: Wed Apr 12 02:25:49 2023, max compression
```

## Comparing `pydash-6.0.2.tar` & `pydash-7.0.0.tar`

### file list

```diff
@@ -1,76 +1,633 @@
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.160852 pydash-6.0.2/
--rw-r--r--   0 dgilland   (501) staff       (20)     1257 2021-06-27 18:15:07.000000 pydash-6.0.2/AUTHORS.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    38821 2023-02-24 02:32:23.000000 pydash-6.0.2/CHANGELOG.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-6.0.2/CONTRIBUTING.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-6.0.2/LICENSE.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      258 2021-01-05 22:53:19.000000 pydash-6.0.2/MANIFEST.in
--rw-r--r--   0 dgilland   (501) staff       (20)    42295 2023-02-24 03:01:27.160943 pydash-6.0.2/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-6.0.2/README.rst
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.137907 pydash-6.0.2/docs/
--rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/Makefile
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.138134 pydash-6.0.2/docs/_static/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-6.0.2/docs/_static/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/_static/theme_override.css
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.138276 pydash-6.0.2/docs/_templates/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-6.0.2/docs/_templates/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/api.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-6.0.2/docs/authors.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/callbacks.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-6.0.2/docs/chaining.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/changelog.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-6.0.2/docs/conf.py
--rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-6.0.2/docs/contributing.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/deeppath.rst
--rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-6.0.2/docs/devguide.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/differences.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-6.0.2/docs/index.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-6.0.2/docs/installation.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/kudos.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-6.0.2/docs/license.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/quickstart.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/templating.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-6.0.2/docs/upgrading.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-6.0.2/docs/versioning.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-6.0.2/pylintrc
--rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-6.0.2/pyproject.toml
--rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-6.0.2/requirements.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     2129 2023-02-24 03:01:27.162047 pydash-6.0.2/setup.cfg
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.132573 pydash-6.0.2/src/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.156505 pydash-6.0.2/src/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)     5373 2023-02-24 02:55:13.000000 pydash-6.0.2/src/pydash/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    59046 2021-06-27 18:15:05.000000 pydash-6.0.2/src/pydash/arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9089 2021-07-15 22:08:21.000000 pydash-6.0.2/src/pydash/chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    32109 2021-06-27 18:15:05.000000 pydash-6.0.2/src/pydash/collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)      401 2021-07-15 21:59:14.000000 pydash-6.0.2/src/pydash/exceptions.py
--rw-r--r--   0 dgilland   (501) staff       (20)    27327 2021-09-28 21:42:55.000000 pydash-6.0.2/src/pydash/functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8921 2023-02-24 02:26:36.000000 pydash-6.0.2/src/pydash/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)    16186 2021-09-28 21:40:18.000000 pydash-6.0.2/src/pydash/numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    47845 2023-02-16 02:13:09.000000 pydash-6.0.2/src/pydash/objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    25373 2022-09-23 13:22:37.000000 pydash-6.0.2/src/pydash/predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    57106 2022-09-23 13:31:18.000000 pydash-6.0.2/src/pydash/strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33862 2022-12-01 04:56:26.000000 pydash-6.0.2/src/pydash/utilities.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.157429 pydash-6.0.2/src/pydash.egg-info/
--rw-r--r--   0 dgilland   (501) staff       (20)    42295 2023-02-24 03:01:27.000000 pydash-6.0.2/src/pydash.egg-info/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1342 2023-02-24 03:01:27.000000 pydash-6.0.2/src/pydash.egg-info/SOURCES.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-02-24 03:01:27.000000 pydash-6.0.2/src/pydash.egg-info/dependency_links.txt
--rw-r--r--   0 dgilland   (501) staff       (20)      219 2023-02-24 03:01:27.000000 pydash-6.0.2/src/pydash.egg-info/requires.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-02-24 03:01:27.000000 pydash-6.0.2/src/pydash.egg-info/top_level.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     3743 2023-01-29 01:19:32.000000 pydash-6.0.2/tasks.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.160387 pydash-6.0.2/tests/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-6.0.2/tests/__init__.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.132736 pydash-6.0.2/tests/build/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-02-24 03:01:27.160711 pydash-6.0.2/tests/build/testresults/
--rw-r--r--   0 dgilland   (501) staff       (20)      337 2022-09-23 13:16:59.000000 pydash-6.0.2/tests/build/testresults/junit.xml
--rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-6.0.2/tests/conftest.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-6.0.2/tests/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-6.0.2/tests/test_annotations.py
--rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-6.0.2/tests/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     4220 2021-07-15 21:59:14.000000 pydash-6.0.2/tests/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-6.0.2/tests/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-6.0.2/tests/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-6.0.2/tests/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    28100 2023-02-24 02:30:12.000000 pydash-6.0.2/tests/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-6.0.2/tests/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33858 2022-05-15 22:03:39.000000 pydash-6.0.2/tests/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    18109 2023-01-28 17:29:56.000000 pydash-6.0.2/tests/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-6.0.2/tox.ini
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.289457 pydash-7.0.0/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.231011 pydash-7.0.0/.tox/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217568 pydash-7.0.0/.tox/.package/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217619 pydash-7.0.0/.tox/.package/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217668 pydash-7.0.0/.tox/.package/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217717 pydash-7.0.0/.tox/.package/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.237632 pydash-7.0.0/.tox/.package/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.0/.tox/.package/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217830 pydash-7.0.0/.tox/.pkg/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217877 pydash-7.0.0/.tox/.pkg/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217924 pydash-7.0.0/.tox/.pkg/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.217971 pydash-7.0.0/.tox/.pkg/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.237921 pydash-7.0.0/.tox/.pkg/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.0/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.218079 pydash-7.0.0/.tox/3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.218125 pydash-7.0.0/.tox/3.11/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.218170 pydash-7.0.0/.tox/3.11/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.220601 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.238199 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.238310 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.238421 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.238532 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.238844 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.238964 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239075 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239184 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239299 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239407 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239513 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239762 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239868 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.239971 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.240071 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.240169 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.219311 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.240258 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.240503 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.240593 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.240678 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.240929 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.241019 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.241243 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.241335 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.241524 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.241615 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.241836 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242066 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242166 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242258 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242349 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242439 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242530 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242753 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242838 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.242936 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243034 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243122 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243210 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243292 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.0/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.220718 pydash-7.0.0/.tox/py310/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.220763 pydash-7.0.0/.tox/py310/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.220809 pydash-7.0.0/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.223326 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243377 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243454 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243536 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243616 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243872 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.243954 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244034 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244111 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244194 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244276 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244359 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244578 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244657 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244739 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244823 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244908 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.244992 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.221954 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.245071 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.245324 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.245406 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.245497 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.245733 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.245814 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246034 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246123 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246345 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246426 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246621 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246826 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246910 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.246993 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247073 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247155 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247248 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247525 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247622 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247725 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247820 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.247908 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.248175 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.248278 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.248381 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.0/.tox/py310/lib/python3.10/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.223422 pydash-7.0.0/.tox/py311/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.223459 pydash-7.0.0/.tox/py311/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.223501 pydash-7.0.0/.tox/py311/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.225588 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.248478 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.248570 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.248665 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.248757 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249082 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249180 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249272 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249362 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249446 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249538 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249623 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.249913 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250011 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250098 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250183 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250284 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.224407 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250376 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250659 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250743 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.250820 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.251083 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.251174 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.251402 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.251491 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.251718 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.251812 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252029 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252271 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252356 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252442 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252534 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252620 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252705 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.252951 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253033 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253110 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253200 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253278 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253361 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253438 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.0/.tox/py311/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.225680 pydash-7.0.0/.tox/py37/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.225718 pydash-7.0.0/.tox/py37/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.225757 pydash-7.0.0/.tox/py37/lib/python3.7/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.228278 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253517 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253603 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253697 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.253784 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254020 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254102 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254180 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254264 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254362 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254442 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254700 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254784 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254870 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.254964 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.255061 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.255147 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.226855 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.255246 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.255495 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.255594 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.255699 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.255970 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.256048 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.256285 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.256365 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.256590 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.256670 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.256899 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257103 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257196 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257294 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.227705 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257393 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257476 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257554 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257642 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257873 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.257964 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258041 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258121 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258199 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258461 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258545 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.0/.tox/py37/lib/python3.7/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.228383 pydash-7.0.0/.tox/py38/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.228428 pydash-7.0.0/.tox/py38/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.228473 pydash-7.0.0/.tox/py38/lib/python3.8/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.230949 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258634 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258713 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258793 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.258877 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259139 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259235 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259332 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259427 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259523 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259617 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259715 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.259972 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260073 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260163 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260246 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260340 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260424 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260510 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.229576 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260597 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260853 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.260934 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.261012 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.261263 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.261339 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.261563 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.261645 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.261855 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.261939 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.262202 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.262482 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.262598 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.262713 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.262832 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.262941 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.263046 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.263339 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.263452 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.263567 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.263680 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.263780 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.264033 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.264146 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.264260 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.0/.tox/py38/lib/python3.8/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.231054 pydash-7.0.0/.tox/py39/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.231096 pydash-7.0.0/.tox/py39/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.231135 pydash-7.0.0/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.234204 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.264385 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.264497 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.264605 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.264718 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265001 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265110 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265225 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265322 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265423 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265539 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265650 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.265924 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266029 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266135 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266247 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266366 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266479 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.232337 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266595 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266867 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.266974 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.267082 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.267325 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.267429 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.267836 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.267946 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.268250 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.268367 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.268690 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.268923 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269036 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269156 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269271 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269382 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269483 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269741 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269848 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.269955 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.270065 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.270171 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.270423 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.270534 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.270702 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.0/.tox/py39/lib/python3.9/site-packages/twine/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)     1257 2021-06-27 18:15:07.000000 pydash-7.0.0/AUTHORS.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    40010 2023-04-12 02:20:23.000000 pydash-7.0.0/CHANGELOG.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.0/LICENSE.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.0/MANIFEST.in
+-rw-r--r--   0 dgilland   (501) staff       (20)    43484 2023-04-12 02:25:49.289544 pydash-7.0.0/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.0/README.rst
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.274016 pydash-7.0.0/docs/
+-rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/Makefile
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.274255 pydash-7.0.0/docs/_static/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.0/docs/_static/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/_static/theme_override.css
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.274410 pydash-7.0.0/docs/_templates/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.0/docs/_templates/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/api.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.0/docs/authors.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/callbacks.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.0/docs/chaining.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/changelog.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.0/docs/conf.py
+-rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.0/docs/contributing.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/deeppath.rst
+-rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.0/docs/devguide.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/differences.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.0/docs/index.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.0/docs/installation.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/kudos.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.0/docs/license.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/quickstart.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/templating.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.0/docs/upgrading.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.0/docs/versioning.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.0/pylintrc
+-rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.0/pyproject.toml
+-rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.0/requirements.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     2507 2023-04-12 02:25:49.289927 pydash-7.0.0/setup.cfg
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.234643 pydash-7.0.0/src/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.282172 pydash-7.0.0/src/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)     5373 2023-04-12 02:16:57.000000 pydash-7.0.0/src/pydash/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    69680 2023-04-12 02:13:49.000000 pydash-7.0.0/src/pydash/arrays.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.283912 pydash-7.0.0/src/pydash/chaining/
+-rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.0/src/pydash/chaining/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.0/src/pydash/chaining/all_funcs.py
+-rw-r--r--   0 dgilland   (501) staff       (20)   123183 2023-04-12 02:15:39.000000 pydash-7.0.0/src/pydash/chaining/all_funcs.pyi
+-rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.0/src/pydash/chaining/chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.0/src/pydash/collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.0/src/pydash/exceptions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.0/src/pydash/functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.0/src/pydash/helpers.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.0/src/pydash/numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.0/src/pydash/objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.0/src/pydash/predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.0/src/pydash/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.0/src/pydash/strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      593 2023-03-18 22:34:56.000000 pydash-7.0.0/src/pydash/types.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.0/src/pydash/utilities.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.282786 pydash-7.0.0/src/pydash.egg-info/
+-rw-r--r--   0 dgilland   (501) staff       (20)    43484 2023-04-12 02:25:47.000000 pydash-7.0.0/src/pydash.egg-info/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-04-12 02:25:49.000000 pydash-7.0.0/src/pydash.egg-info/SOURCES.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-04-12 02:25:47.000000 pydash-7.0.0/src/pydash.egg-info/dependency_links.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)      269 2023-04-12 02:25:47.000000 pydash-7.0.0/src/pydash.egg-info/requires.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-04-12 02:25:47.000000 pydash-7.0.0/src/pydash.egg-info/top_level.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.0/tasks.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.286862 pydash-7.0.0/tests/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.0/tests/__init__.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.234944 pydash-7.0.0/tests/build/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.287021 pydash-7.0.0/tests/build/testresults/
+-rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.0/tests/build/testresults/junit.xml
+-rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.0/tests/conftest.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.0/tests/helpers.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-12 02:25:49.289286 pydash-7.0.0/tests/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.0/tests/pytest_mypy_testing/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    16142 2023-04-12 02:13:49.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.0/tests/pytest_mypy_testing/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.0/tests/test_annotations.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.0/tests/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.0/tests/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.0/tests/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.0/tests/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.0/tests/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.0/tests/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.0/tests/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.0/tests/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.0/tests/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.0/tox.ini
```

### Comparing `pydash-6.0.2/AUTHORS.rst` & `pydash-7.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/CHANGELOG.rst` & `pydash-7.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.0 (2023-04-11)
+-------------------
+
+- Add type annotations to package. Raise an issue for any typing issues at https://github.com/dgilland/pydash/issues. Thanks DeviousStoat_! (**breaking change**)
+- Change behavior of ``to_dict`` to not using ``dict()`` internally. Previous behavior would be for something like ``to_dict([["k", "v"], ["x", "y"]])`` to return ``{"k": "v", "x": "y"}`` (equivalent to calling ``dict(...)``) but ``to_dict([["k"], ["v"], ["x"], ["y"]])`` would return ``{0: ["x"], 1: ["v"], 2: ["x"], 3: ["y"]}``. The new behavior is to always return iterables as dictionaries with their indexes as keys like ``{0: ["k", "v"], 1: ["x", "y"]}``. This is consistent with how iterable objects are iterated over and means that ``to_dict`` will have more reliable output. (**breaking change**)
+- Change behavior of ``slugify`` to remove single-quotes from output. Instead of ``slugify("the cat's meow") == "the-cat's-meow"``, the new behavior is to return ``"the-cats-meow"``. (**breaking change**)
+- Add support for negative indexes in ``get`` path keys. Thanks bl4ckst0ne_!
+
+
 v6.0.2 (2023-02-23)
 -------------------
 
 - Only prevent access to object paths containing ``__globals__`` or ``__builtins__`` instead of all dunder-methods for non-dict/list objects.
 
 
 v6.0.1 (2023-02-20)
@@ -1212,7 +1221,9 @@
 .. _efenka: https://github.com/efenka
 .. _jwilson8767: https://github.com/jwilson8767
 .. _elijose55: https://github.com/elijose55
 .. _gonzalonaveira: https://github.com/gonzalonaveira
 .. _zhaowb: https://github.com/zhaowb
 .. _mervynlee94: https://github.com/mervynlee94
 .. _weineel: https://github.com/weineel
+.. _bl4ckst0ne: https://github.com/bl4ckst0ne
+.. _DeviousStoat: https://github.com/DeviousStoat
```

### Comparing `pydash-6.0.2/CONTRIBUTING.rst` & `pydash-7.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/LICENSE.rst` & `pydash-7.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/PKG-INFO` & `pydash-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 6.0.2
+Version: 7.0.0
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,23 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.0 (2023-04-11)
+-------------------
+
+- Add type annotations to package. Raise an issue for any typing issues at https://github.com/dgilland/pydash/issues. Thanks DeviousStoat_! (**breaking change**)
+- Change behavior of ``to_dict`` to not using ``dict()`` internally. Previous behavior would be for something like ``to_dict([["k", "v"], ["x", "y"]])`` to return ``{"k": "v", "x": "y"}`` (equivalent to calling ``dict(...)``) but ``to_dict([["k"], ["v"], ["x"], ["y"]])`` would return ``{0: ["x"], 1: ["v"], 2: ["x"], 3: ["y"]}``. The new behavior is to always return iterables as dictionaries with their indexes as keys like ``{0: ["k", "v"], 1: ["x", "y"]}``. This is consistent with how iterable objects are iterated over and means that ``to_dict`` will have more reliable output. (**breaking change**)
+- Change behavior of ``slugify`` to remove single-quotes from output. Instead of ``slugify("the cat's meow") == "the-cat's-meow"``, the new behavior is to return ``"the-cats-meow"``. (**breaking change**)
+- Add support for negative indexes in ``get`` path keys. Thanks bl4ckst0ne_!
+
+
 v6.0.2 (2023-02-23)
 -------------------
 
 - Only prevent access to object paths containing ``__globals__`` or ``__builtins__`` instead of all dunder-methods for non-dict/list objects.
 
 
 v6.0.1 (2023-02-20)
@@ -1274,14 +1283,16 @@
 .. _efenka: https://github.com/efenka
 .. _jwilson8767: https://github.com/jwilson8767
 .. _elijose55: https://github.com/elijose55
 .. _gonzalonaveira: https://github.com/gonzalonaveira
 .. _zhaowb: https://github.com/zhaowb
 .. _mervynlee94: https://github.com/mervynlee94
 .. _weineel: https://github.com/weineel
+.. _bl4ckst0ne: https://github.com/bl4ckst0ne
+.. _DeviousStoat: https://github.com/DeviousStoat
 
 MIT License
 
 Copyright (c) 2020 Derrick Gilland
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pydash-6.0.2/README.rst` & `pydash-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/Makefile` & `pydash-7.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/api.rst` & `pydash-7.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/callbacks.rst` & `pydash-7.0.0/docs/callbacks.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/chaining.rst` & `pydash-7.0.0/docs/chaining.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/conf.py` & `pydash-7.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/deeppath.rst` & `pydash-7.0.0/docs/deeppath.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/differences.rst` & `pydash-7.0.0/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/index.rst` & `pydash-7.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/quickstart.rst` & `pydash-7.0.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/templating.rst` & `pydash-7.0.0/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/docs/upgrading.rst` & `pydash-7.0.0/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/pylintrc` & `pydash-7.0.0/pylintrc`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/setup.cfg` & `pydash-7.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	Topic :: Utilities
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
+include_package_data = True
 install_requires = 
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
@@ -43,32 +44,45 @@
 	flake8
 	flake8-black
 	flake8-bugbear
 	flake8-isort
 	importlib_metadata<5; python_version=="3.7"
 	invoke
 	isort
+	mypy
 	pylint
 	pytest
+	pytest-mypy-testing
 	pytest-cov
 	Sphinx
 	sphinx-rtd-theme
 	tox
 	twine
 	wheel
+	sphinx-autodoc-typehints
 
 [bdist_wheel]
 python_tag = py3
 
 [flake8]
 exclude = .tox,venv,env
 max_line_length = 100
 max_complexity = 12
 ignore = F401,F811,E203,W503
 
+[mypy]
+show_column_numbers = True
+show_error_context = False
+ignore_missing_imports = True
+warn_return_any = False
+strict_optional = True
+warn_no_return = True
+warn_redundant_casts = False
+warn_unused_ignores = False
+
 [tool:isort]
 line_length = 100
 multi_line_output = 3
 lines_after_imports = 2
 combine_as_imports = true
 include_trailing_comma = true
 force_sort_within_sections = true
@@ -88,12 +102,18 @@
 	--junitxml=build/testresults/junit.xml
 
 [coverage:run]
 omit = 
 	*/tests/*
 	*/test_*
 	*/_compat.py
+	*/types.py
+
+[coverage:report]
+exclude_lines = 
+	pragma: no cover
+	@t.overload
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pydash-6.0.2/src/pydash/__init__.py` & `pydash-7.0.0/src/pydash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python port of Lo-Dash."""
 
-__version__ = "6.0.2"
+__version__ = "7.0.0"
 
 from .arrays import (
     chunk,
     compact,
     concat,
     difference,
     difference_by,
```

### Comparing `pydash-6.0.2/src/pydash/arrays.py` & `pydash-7.0.0/src/pydash/arrays.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 
 .. versionadded:: 1.0.0
 """
 
 from bisect import bisect_left, bisect_right
 from functools import cmp_to_key
 from math import ceil
+import typing as t
 
 import pydash as pyd
 
 from .helpers import base_get, iteriteratee, parse_iteratee
+from .types import IterateeObjT
+
+
+if t.TYPE_CHECKING:
+    from _typeshed import SupportsRichComparisonT  # pragma: no cover
 
 
 __all__ = (
     "chunk",
     "compact",
     "concat",
     "difference",
@@ -86,119 +92,140 @@
     "xor_with",
     "zip_",
     "zip_object",
     "zip_object_deep",
     "zip_with",
 )
 
+T = t.TypeVar("T")
+T2 = t.TypeVar("T2")
+SequenceT = t.TypeVar("SequenceT", bound=t.Sequence)
+MutableSequenceT = t.TypeVar("MutableSequenceT", bound=t.MutableSequence)
+
 
-def chunk(array, size=1):
+def chunk(array: t.Sequence[T], size: int = 1) -> t.List[t.Sequence[T]]:
     """
     Creates a list of elements split into groups the length of `size`. If `array` can't be split
     evenly, the final chunk will be the remaining elements.
 
     Args:
-        array (list): List to chunk.
-        size (int, optional): Chunk size. Defaults to ``1``.
+        array: List to chunk.
+        size: Chunk size. Defaults to ``1``.
 
     Returns:
-        list: New list containing chunks of `array`.
+        New list containing chunks of `array`.
 
     Example:
 
         >>> chunk([1, 2, 3, 4, 5], 2)
         [[1, 2], [3, 4], [5]]
 
     .. versionadded:: 1.1.0
     """
     chunks = int(ceil(len(array) / float(size)))
     return [array[i * size : (i + 1) * size] for i in range(chunks)]
 
 
-def compact(array):
+def compact(array: t.Iterable[t.Union[T, None]]) -> t.List[T]:
     """
     Creates a list with all falsey values of array removed.
 
     Args:
-        array (list): List to compact.
+        array: List to compact.
 
     Returns:
-        list: Compacted list.
+        Compacted list.
 
     Example:
 
         >>> compact(['', 1, 0, True, False, None])
         [1, True]
 
     .. versionadded:: 1.0.0
     """
     return [item for item in array if item]
 
 
-def concat(*arrays):
+def concat(*arrays: t.Iterable[T]) -> t.List[T]:
     """
     Concatenates zero or more lists into one.
 
     Args:
-        arrays (list): Lists to concatenate.
+        arrays: Lists to concatenate.
 
     Returns:
-        list: Concatenated list.
+        Concatenated list.
 
     Example:
 
         >>> concat([1, 2], [3, 4], [[5], [6]])
         [1, 2, 3, 4, [5], [6]]
 
     .. versionadded:: 2.0.0
 
     .. versionchanged:: 4.0.0
         Renamed from ``cat`` to ``concat``.
     """
     return flatten(arrays)
 
 
-def difference(array, *others):
+def difference(array: t.Iterable[T], *others: t.Iterable[T]) -> t.List[T]:
     """
     Creates a list of list elements not present in others.
 
     Args:
-        array (list): List to process.
-        others (list): Lists to check.
+        array: List to process.
+        others: Lists to check.
 
     Returns:
-        list: Difference between `others`.
+        Difference between `others`.
 
     Example:
 
         >>> difference([1, 2, 3], [1], [2])
         [3]
 
     .. versionadded:: 1.0.0
     """
     return difference_with(array, *others)
 
 
+@t.overload
+def difference_by(
+    array: t.Iterable[T],
+    *others: t.Iterable[T],
+    iteratee: t.Union[IterateeObjT, t.Callable[[T], T], None],
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def difference_by(
+    array: t.Iterable[T], *others: t.Union[IterateeObjT, t.Iterable[T], t.Callable[[T], T]]
+) -> t.List[T]:
+    ...
+
+
 def difference_by(array, *others, **kwargs):
     """
     This method is like :func:`difference` except that it accepts an iteratee which is invoked for
     each element of each array to generate the criterion by which they're compared. The order and
     references of result values are determined by `array`. The iteratee is invoked with one
     argument: ``(value)``.
 
     Args:
-        array (list): The array to find the difference of.
-        others (list): Lists to check for difference with `array`.
+        array: The array to find the difference of.
+        others: Lists to check for difference with `array`.
 
     Keyword Args:
-        iteratee (mixed, optional): Function to transform the elements of the arrays. Defaults to
+        iteratee: Function to transform the elements of the arrays. Defaults to
             :func:`.identity`.
 
     Returns:
-        list: Difference between `others`.
+        Difference between `others`.
 
     Example:
 
         >>> difference_by([1.2, 1.5, 1.7, 2.8], [0.9, 3.2], round)
         [1.5, 1.7]
 
     .. versionadded:: 4.0.0
@@ -215,30 +242,46 @@
         if not other:
             continue
         array = list(iterdifference(array, other, iteratee=iteratee))
 
     return array
 
 
+@t.overload
+def difference_with(
+    array: t.Iterable[T],
+    *others: t.Iterable[T2],
+    comparator: t.Union[t.Callable[[T, T2], t.Any], None],
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def difference_with(
+    array: t.Iterable[T], *others: t.Union[t.Iterable[T2], t.Callable[[T, T2], t.Any]]
+) -> t.List[T]:
+    ...
+
+
 def difference_with(array, *others, **kwargs):
     """
     This method is like :func:`difference` except that it accepts a comparator which is invoked to
     compare the elements of all arrays. The order and references of result values are determined by
     the first array. The comparator is invoked with two arguments: ``(arr_val, oth_val)``.
 
     Args:
-        array (list): The array to find the difference of.
-        others (list): Lists to check for difference with `array`.
+        array: The array to find the difference of.
+        others: Lists to check for difference with `array`.
 
     Keyword Args:
-        comparator (callable, optional): Function to compare the elements of the arrays. Defaults to
+        comparator: Function to compare the elements of the arrays. Defaults to
             :func:`.is_equal`.
 
     Returns:
-        list: Difference between `others`.
+        Difference between `others`.
 
     Example:
 
         >>> array = ['apple', 'banana', 'pear']
         >>> others = (['avocado', 'pumpkin'], ['peach'])
         >>> comparator = lambda a, b: a[0] == b[0]
         >>> difference_with(array, *others, comparator=comparator)
@@ -263,24 +306,24 @@
         if not other:
             continue
         array = list(iterdifference(array, other, comparator=comparator))
 
     return array
 
 
-def drop(array, n=1):
+def drop(array: t.Sequence[T], n: int = 1) -> t.List[T]:
     """
     Creates a slice of `array` with `n` elements dropped from the beginning.
 
     Args:
-        array (list): List to process.
-        n (int, optional): Number of elements to drop. Defaults to ``1``.
+        array: List to process.
+        n: Number of elements to drop. Defaults to ``1``.
 
     Returns:
-        list: Dropped list.
+        Dropped list.
 
     Example:
 
         >>> drop([1, 2, 3, 4], 2)
         [3, 4]
 
     .. versionadded:: 1.0.0
@@ -290,24 +333,24 @@
 
     .. versionchanged:: 3.0.0
         Made ``n`` default to ``1``.
     """
     return drop_while(array, lambda _, index: index < n)
 
 
-def drop_right(array, n=1):
+def drop_right(array: t.Sequence[T], n: int = 1) -> t.List[T]:
     """
     Creates a slice of `array` with `n` elements dropped from the end.
 
     Args:
-        array (list): List to process.
-        n (int, optional): Number of elements to drop. Defaults to ``1``.
+        array: List to process.
+        n: Number of elements to drop. Defaults to ``1``.
 
     Returns:
-        list: Dropped list.
+        Dropped list.
 
     Example:
 
         >>> drop_right([1, 2, 3, 4], 2)
         [1, 2]
 
     .. versionadded:: 1.1.0
@@ -315,26 +358,48 @@
     .. versionchanged:: 3.0.0
         Made ``n`` default to ``1``.
     """
     length = len(array)
     return drop_right_while(array, lambda _, index: (length - index) <= n)
 
 
+@t.overload
+def drop_right_while(
+    array: t.Sequence[T], predicate: t.Callable[[T, int, t.List[T]], t.Any]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def drop_right_while(array: t.Sequence[T], predicate: t.Callable[[T, int], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def drop_right_while(array: t.Sequence[T], predicate: t.Callable[[T], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def drop_right_while(array: t.Sequence[T], predicate: None = None) -> t.List[T]:
+    ...
+
+
 def drop_right_while(array, predicate=None):
     """
     Creates a slice of `array` excluding elements dropped from the end. Elements are dropped until
     the `predicate` returns falsey. The `predicate` is invoked with three arguments: ``(value,
     index, array)``.
 
     Args:
-        array (list): List to process.
-        predicate (mixed): Predicate called per iteration
+        array: List to process.
+        predicate: Predicate called per iteration
 
     Returns:
-        list: Dropped list.
+        Dropped list.
 
     Example:
 
         >>> drop_right_while([1, 2, 3, 4], lambda x: x >= 3)
         [1, 2]
 
     .. versionadded:: 1.1.0
@@ -345,26 +410,48 @@
             n -= 1
         else:
             break
 
     return array[:n]
 
 
+@t.overload
+def drop_while(
+    array: t.Sequence[T], predicate: t.Callable[[T, int, t.List[T]], t.Any]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def drop_while(array: t.Sequence[T], predicate: t.Callable[[T, int], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def drop_while(array: t.Sequence[T], predicate: t.Callable[[T], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def drop_while(array: t.Sequence[T], predicate: None = None) -> t.List[T]:
+    ...
+
+
 def drop_while(array, predicate=None):
     """
     Creates a slice of `array` excluding elements dropped from the beginning. Elements are dropped
     until the `predicate` returns falsey. The `predicate` is invoked with three arguments: ``(value,
     index, array)``.
 
     Args:
-        array (list): List to process.
-        predicate (mixed): Predicate called per iteration
+        array: List to process.
+        predicate: Predicate called per iteration
 
     Returns:
-        list: Dropped list.
+        Dropped list.
 
     Example:
 
         >>> drop_while([1, 2, 3, 4], lambda x: x < 3)
         [3, 4]
 
     .. versionadded:: 1.1.0
@@ -375,62 +462,66 @@
             n += 1
         else:
             break
 
     return array[n:]
 
 
-def duplicates(array, iteratee=None):
+def duplicates(
+    array: t.Sequence[T], iteratee: t.Union[t.Callable[[T], t.Any], IterateeObjT, None] = None
+) -> t.List[T]:
     """
     Creates a unique list of duplicate values from `array`. If iteratee is passed, each element of
-    array is passed through a iteratee before duplicates are computed. The iteratee is invoked with
+    array is passed through an iteratee before duplicates are computed. The iteratee is invoked with
     three arguments: ``(value, index, array)``. If an object path is passed for iteratee, the
     created iteratee will return the path value of the given element. If an object is passed for
     iteratee, the created filter style iteratee will return ``True`` for elements that have the
     properties of the given object, else ``False``.
 
     Args:
-        array (list): List to process.
-        iteratee (mixed, optional): Iteratee applied per iteration.
+        array: List to process.
+        iteratee: Iteratee applied per iteration.
 
     Returns:
-        list: List of duplicates.
+        List of duplicates.
 
     Example:
 
         >>> duplicates([0, 1, 3, 2, 3, 1])
         [3, 1]
 
     .. versionadded:: 3.0.0
     """
     if iteratee:
         cbk = pyd.iteratee(iteratee)
         computed = [cbk(item) for item in array]
     else:
-        computed = array
+        computed = array  # type: ignore
 
     # NOTE: Using array[i] instead of item since iteratee could have modified
     # returned item values.
     lst = uniq(array[i] for i, _ in iterduplicates(computed))
 
     return lst
 
 
-def fill(array, value, start=0, end=None):
+def fill(
+    array: t.Sequence[T], value: T2, start: int = 0, end: t.Union[int, None] = None
+) -> t.List[t.Union[T, T2]]:
     """
     Fills elements of array with value from `start` up to, but not including, `end`.
 
     Args:
-        array (list): List to fill.
-        value (mixed): Value to fill with.
-        start (int, optional): Index to start filling. Defaults to ``0``.
-        end (int, optional): Index to end filling. Defaults to ``len(array)``.
+        array: List to fill.
+        value: Value to fill with.
+        start: Index to start filling. Defaults to ``0``.
+        end: Index to end filling. Defaults to ``len(array)``.
 
     Returns:
-        list: Filled `array`.
+        Filled `array`.
 
     Example:
 
         >>> fill([1, 2, 3, 4, 5], 0)
         [0, 0, 0, 0, 0]
         >>> fill([1, 2, 3, 4, 5], 0, 1, 3)
         [1, 0, 0, 4, 5]
@@ -444,77 +535,127 @@
     """
     if end is None:
         end = len(array)
     else:
         end = min(end, len(array))
 
     # Use this style of assignment so that `array` is mutated.
-    array[:] = array[:start] + [value] * len(array[start:end]) + array[end:]
-    return array
+    array[:] = array[:start] + [value] * len(array[start:end]) + array[end:]  # type: ignore
+    return array  # type: ignore
+
+
+@t.overload
+def find_index(array: t.Iterable[T], predicate: t.Callable[[T, int, t.List[T]], t.Any]) -> int:
+    ...
+
+
+@t.overload
+def find_index(array: t.Iterable[T], predicate: t.Callable[[T, int], t.Any]) -> int:
+    ...
+
+
+@t.overload
+def find_index(array: t.Iterable[T], predicate: t.Callable[[T], t.Any]) -> int:
+    ...
+
+
+@t.overload
+def find_index(array: t.Iterable[t.Any], predicate: None = None) -> int:
+    ...
 
 
 def find_index(array, predicate=None):
     """
     This method is similar to :func:`pydash.collections.find`, except that it returns the index of
     the element that passes the predicate check, instead of the element itself.
 
     Args:
-        array (list): List to process.
-        predicate (mixed, optional): Predicate applied per iteration.
+        array: List to process.
+        predicate: Predicate applied per iteration.
 
     Returns:
-        int: Index of found item or ``-1`` if not found.
+        Index of found item or ``-1`` if not found.
 
     Example:
 
         >>> find_index([1, 2, 3, 4], lambda x: x >= 3)
         2
         >>> find_index([1, 2, 3, 4], lambda x: x > 4)
         -1
 
     .. versionadded:: 1.0.0
     """
     search = (i for is_true, _, i, _ in iteriteratee(array, predicate) if is_true)
     return next(search, -1)
 
 
+@t.overload
+def find_last_index(array: t.Iterable[T], predicate: t.Callable[[T, int, t.List[T]], t.Any]) -> int:
+    ...
+
+
+@t.overload
+def find_last_index(array: t.Iterable[T], predicate: t.Callable[[T, int], t.Any]) -> int:
+    ...
+
+
+@t.overload
+def find_last_index(array: t.Iterable[T], predicate: t.Callable[[T], t.Any]) -> int:
+    ...
+
+
+@t.overload
+def find_last_index(array: t.Iterable[t.Any], predicate: None = None) -> int:
+    ...
+
+
 def find_last_index(array, predicate=None):
     """
     This method is similar to :func:`find_index`, except that it iterates over elements from right
     to left.
 
     Args:
-        array (list): List to process.
-        predicate (mixed, optional): Predicate applied per iteration.
+        array: List to process.
+        predicate: Predicate applied per iteration.
 
     Returns:
-        int: Index of found item or ``-1`` if not found.
+        Index of found item or ``-1`` if not found.
 
     Example:
 
         >>> find_last_index([1, 2, 3, 4], lambda x: x >= 3)
         3
         >>> find_last_index([1, 2, 3, 4], lambda x: x > 4)
         -1
 
     .. versionadded:: 1.0.0
     """
     search = (i for is_true, _, i, _ in iteriteratee(array, predicate, reverse=True) if is_true)
     return next(search, -1)
 
 
+@t.overload
+def flatten(array: t.Iterable[t.Iterable[T]]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def flatten(array: t.Iterable[T]) -> t.List[T]:
+    ...
+
+
 def flatten(array):
     """
     Flattens array a single level deep.
 
     Args:
-        array (list): List to flatten.
+        array: List to flatten.
 
     Returns:
-        list: Flattened list.
+        Flattened list.
 
     Example:
 
         >>> flatten([[1], [2, [3]], [[4]]])
         [1, 2, [3], [4]]
 
 
@@ -526,44 +667,44 @@
 
     .. versionchanged:: 4.0.0
         Removed ``is_deep`` option. Use :func:`flatten_deep` instead.
     """
     return flatten_depth(array, depth=1)
 
 
-def flatten_deep(array):
+def flatten_deep(array: t.Iterable) -> t.List:
     """
     Flattens an array recursively.
 
     Args:
-        array (list): List to flatten.
+        array: List to flatten.
 
     Returns:
-        list: Flattened list.
+        Flattened list.
 
     Example:
 
         >>> flatten_deep([[1], [2, [3]], [[4]]])
         [1, 2, 3, 4]
 
     .. versionadded:: 2.0.0
     """
     return flatten_depth(array, depth=-1)
 
 
-def flatten_depth(array, depth=1):
+def flatten_depth(array: t.Iterable, depth: int = 1) -> t.List:
     """
     Recursively flatten `array` up to `depth` times.
 
     Args:
-        array (list): List to flatten.
-        depth (int, optional): Depth to flatten to. Defaults to ``1``.
+        array: List to flatten.
+        depth: Depth to flatten to. Defaults to ``1``.
 
     Returns:
-        list: Flattened list.
+        Flattened list.
 
     Example:
 
         >>> flatten_depth([[[1], [2, [3]], [[4]]]], 1)
         [[1], [2, [3]], [[4]]]
         >>> flatten_depth([[[1], [2, [3]], [[4]]]], 2)
         [1, 2, [3], [4]]
@@ -573,68 +714,78 @@
         [1, 2, 3, 4]
 
     .. versionadded:: 4.0.0
     """
     return list(iterflatten(array, depth=depth))
 
 
+@t.overload
+def from_pairs(pairs: t.Iterable[t.Tuple[T, T2]]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def from_pairs(pairs: t.Iterable[t.List[t.Union[T, T2]]]) -> t.Dict[t.Union[T, T2], t.Union[T, T2]]:
+    ...
+
+
 def from_pairs(pairs):
     """
     Returns a dict from the given list of pairs.
 
     Args:
-        pairs (list): List of key-value pairs.
+        pairs: List of key-value pairs.
 
     Returns:
         dict
 
     Example:
 
         >>> from_pairs([['a', 1], ['b', 2]]) == {'a': 1, 'b': 2}
         True
 
     .. versionadded:: 4.0.0
     """
     return dict(pairs)
 
 
-def head(array):
+def head(array: t.Sequence[T]) -> t.Union[T, None]:
     """
     Return the first element of `array`.
 
     Args:
-        array (list): List to process.
+        array: List to process.
 
     Returns:
-        mixed: First element of list.
+        First element of list.
 
     Example:
 
         >>> head([1, 2, 3, 4])
         1
 
     .. versionadded:: 1.0.0
 
     .. versionchanged::
         Renamed from ``first`` to ``head``.
     """
     return base_get(array, 0, default=None)
 
 
-def index_of(array, value, from_index=0):
+def index_of(array: t.Sequence[T], value: T, from_index: int = 0) -> int:
     """
     Gets the index at which the first occurrence of value is found.
 
     Args:
-        array (list): List to search.
-        value (mixed): Value to search for.
-        from_index (int, optional): Index to search from.
+        array: List to search.
+        value: Value to search for.
+        from_index: Index to search from.
 
     Returns:
-        int: Index of found item or ``-1`` if not found.
+        Index of found item or ``-1`` if not found.
 
     Example:
 
         >>> index_of([1, 2, 3, 4], 2)
         1
         >>> index_of([2, 1, 2, 3], 2, from_index=1)
         2
@@ -643,87 +794,97 @@
     """
     try:
         return array.index(value, from_index)
     except ValueError:
         return -1
 
 
-def initial(array):
+def initial(array: t.Sequence[T]) -> t.Sequence[T]:
     """
     Return all but the last element of `array`.
 
     Args:
-        array (list): List to process.
+        array: List to process.
 
     Returns:
-        list: Initial part of `array`.
+        Initial part of `array`.
 
     Example:
 
         >>> initial([1, 2, 3, 4])
         [1, 2, 3]
 
     .. versionadded:: 1.0.0
     """
     return array[:-1]
 
 
+@t.overload
+def intercalate(array: t.Iterable[t.Iterable[T]], separator: T2) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def intercalate(array: t.Iterable[T], separator: T2) -> t.List[t.Union[T, T2]]:
+    ...
+
+
 def intercalate(array, separator):
     """
     Like :func:`intersperse` for lists of lists but shallowly flattening the result.
 
     Args:
-        array (list): List to intercalate.
-        separator (mixed): Element to insert.
+        array: List to intercalate.
+        separator: Element to insert.
 
     Returns:
-        list: Intercalated list.
+        Intercalated list.
 
     Example:
 
         >>> intercalate([1, [2], [3], 4], 'x')
         [1, 'x', 2, 'x', 3, 'x', 4]
 
 
     .. versionadded:: 2.0.0
     """
     return flatten(intersperse(array, separator))
 
 
-def interleave(*arrays):
+def interleave(*arrays: t.Iterable[T]) -> t.List[T]:
     """
     Merge multiple lists into a single list by inserting the next element of each list by sequential
     round-robin into the new list.
 
     Args:
-        arrays (list): Lists to interleave.
+        arrays: Lists to interleave.
 
     Returns:
-        list: Interleaved list.
+        Interleaved list.
 
     Example:
 
         >>> interleave([1, 2, 3], [4, 5, 6], [7, 8, 9])
         [1, 4, 7, 2, 5, 8, 3, 6, 9]
 
     .. versionadded:: 2.0.0
     """
     return list(iterinterleave(*arrays))
 
 
-def intersection(array, *others):
+def intersection(array: t.Sequence[T], *others: t.Iterable[t.Any]) -> t.List[T]:
     """
     Computes the intersection of all the passed-in arrays.
 
     Args:
-        array (list): The array to find the intersection of.
-        others (list): Lists to check for intersection with `array`.
+        array: The array to find the intersection of.
+        others: Lists to check for intersection with `array`.
 
     Returns:
-        list: Intersection of provided lists.
+        Intersection of provided lists.
 
     Example:
 
         >>> intersection([1, 2, 3], [1, 2, 3, 4, 5], [2, 3])
         [2, 3]
 
         >>> intersection([1, 2, 3])
@@ -733,31 +894,47 @@
 
     .. versionchanged:: 4.0.0
         Support finding intersection of unhashable types.
     """
     return intersection_with(array, *others)
 
 
+@t.overload
+def intersection_by(
+    array: t.Sequence[T],
+    *others: t.Iterable[t.Any],
+    iteratee: t.Union[t.Callable[[T], T], IterateeObjT],
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def intersection_by(
+    array: t.Sequence[T], *others: t.Union[t.Iterable[t.Any], t.Callable[[T], T], IterateeObjT]
+) -> t.List[T]:
+    ...
+
+
 def intersection_by(array, *others, **kwargs):
     """
     This method is like :func:`intersection` except that it accepts an iteratee which is invoked for
     each element of each array to generate the criterion by which they're compared. The order and
     references of result values are determined by `array`. The iteratee is invoked with one
     argument: ``(value)``.
 
     Args:
-        array (list): The array to find the intersection of.
-        others (list): Lists to check for intersection with `array`.
+        array: The array to find the intersection of.
+        others: Lists to check for intersection with `array`.
 
     Keyword Args:
-        iteratee (mixed, optional): Function to transform the elements of the arrays. Defaults to
+        iteratee: Function to transform the elements of the arrays. Defaults to
             :func:`.identity`.
 
     Returns:
-        list: Intersection of provided lists.
+        Intersection of provided lists.
 
     Example:
 
         >>> intersection_by([1.2, 1.5, 1.7, 2.8], [0.9, 3.2], round)
         [1.2, 2.8]
 
     .. versionadded:: 4.0.0
@@ -776,30 +953,44 @@
         array = list(iterintersection(array, other, iteratee=iteratee))
         if not array:
             break
 
     return array
 
 
+@t.overload
+def intersection_with(
+    array: t.Sequence[T], *others: t.Iterable[T2], comparator: t.Callable[[T, T2], t.Any]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def intersection_with(
+    array: t.Sequence[T], *others: t.Union[t.Iterable[T2], t.Callable[[T, T2], t.Any]]
+) -> t.List[T]:
+    ...
+
+
 def intersection_with(array, *others, **kwargs):
     """
     This method is like :func:`intersection` except that it accepts a comparator which is invoked to
     compare the elements of all arrays. The order and references of result values are determined by
     the first array. The comparator is invoked with two arguments: ``(arr_val, oth_val)``.
 
     Args:
-        array (list): The array to find the intersection of.
-        others (list): Lists to check for intersection with `array`.
+        array: The array to find the intersection of.
+        others: Lists to check for intersection with `array`.
 
     Keyword Args:
-        comparator (callable, optional): Function to compare the elements of the arrays. Defaults to
+        comparator: Function to compare the elements of the arrays. Defaults to
             :func:`.is_equal`.
 
     Returns:
-        list: Intersection of provided lists.
+        Intersection of provided lists.
 
     Example:
 
         >>> array = ['apple', 'banana', 'pear']
         >>> others = (['avocado', 'pumpkin'], ['peach'])
         >>> comparator = lambda a, b: a[0] == b[0]
         >>> intersection_with(array, *others, comparator=comparator)
@@ -821,125 +1012,172 @@
         array = list(iterintersection(array, other, comparator=comparator))
         if not array:
             break
 
     return array
 
 
-def intersperse(array, separator):
+def intersperse(array: t.Iterable[T], separator: T2) -> t.List[t.Union[T, T2]]:
     """
     Insert a separating element between the elements of `array`.
 
     Args:
-        array (list): List to intersperse.
-        separator (mixed): Element to insert.
+        array: List to intersperse.
+        separator: Element to insert.
 
     Returns:
-        list: Interspersed list.
+        Interspersed list.
 
     Example:
 
         >>> intersperse([1, [2], [3], 4], 'x')
         [1, 'x', [2], 'x', [3], 'x', 4]
 
     .. versionadded:: 2.0.0
     """
     return list(iterintersperse(array, separator))
 
 
-def last(array):
+def last(array: t.Sequence[T]) -> t.Union[T, None]:
     """
     Return the last element of `array`.
 
     Args:
-        array (list): List to process.
+        array: List to process.
 
     Returns:
-        mixed: Last part of `array`.
+        Last part of `array`.
 
     Example:
 
         >>> last([1, 2, 3, 4])
         4
 
     .. versionadded:: 1.0.0
     """
     return base_get(array, -1, default=None)
 
 
-def last_index_of(array, value, from_index=None):
+def last_index_of(
+    array: t.Sequence[t.Any], value: t.Any, from_index: t.Union[int, None] = None
+) -> int:
     """
     Gets the index at which the last occurrence of value is found.
 
     Args:
-        array (list): List to search.
-        value (mixed): Value to search for.
-        from_index (int, optional): Index to search from.
+        array: List to search.
+        value: Value to search for.
+        from_index: Index to search from.
 
     Returns:
-        int: Index of found item or ``False`` if not found.
+        Index of found item or ``-1`` if not found.
 
     Example:
 
         >>> last_index_of([1, 2, 2, 4], 2)
         2
         >>> last_index_of([1, 2, 2, 4], 2, from_index=1)
         1
 
     .. versionadded:: 1.0.0
     """
     index = array_len = len(array)
 
     try:
-        from_index = int(from_index)
+        # safe as we are catching any type errors
+        from_index = int(from_index)  # type: ignore
     except (TypeError, ValueError):
         pass
     else:
         # Set starting index base on from_index offset.
         index = max(0, index + from_index) if from_index < 0 else min(from_index, index - 1)
 
     while index:
         if index < array_len and array[index] == value:
             return index
         index -= 1
     return -1
 
 
+@t.overload
+def mapcat(
+    array: t.Iterable[T],
+    iteratee: t.Callable[[T, int, t.List[T]], t.Union[t.List[T2], t.List[t.List[T2]]]],
+) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def mapcat(array: t.Iterable[T], iteratee: t.Callable[[T, int, t.List[T]], T2]) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def mapcat(
+    array: t.Iterable[T], iteratee: t.Callable[[T, int], t.Union[t.List[T2], t.List[t.List[T2]]]]
+) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def mapcat(array: t.Iterable[T], iteratee: t.Callable[[T, int], T2]) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def mapcat(
+    array: t.Iterable[T], iteratee: t.Callable[[T], t.Union[t.List[T2], t.List[t.List[T2]]]]
+) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def mapcat(array: t.Iterable[T], iteratee: t.Callable[[T], T2]) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def mapcat(
+    array: t.Iterable[t.Union[t.List[T], t.List[t.List[T]]]], iteratee: None = None
+) -> t.List[t.Union[T, t.List[T]]]:
+    ...
+
+
 def mapcat(array, iteratee=None):
     """
-    Map a iteratee to each element of a list and concatenate the results into a single list using
+    Map an iteratee to each element of a list and concatenate the results into a single list using
     :func:`concat`.
 
     Args:
-        array (list): List to map and concatenate.
-        iteratee (mixed): Iteratee to apply to each element.
+        array: List to map and concatenate.
+        iteratee: Iteratee to apply to each element.
 
     Returns:
-        list: Mapped and concatenated list.
+        Mapped and concatenated list.
 
     Example:
 
         >>> mapcat(range(4), lambda x: list(range(x)))
         [0, 0, 1, 0, 1, 2]
 
     .. versionadded:: 2.0.0
     """
     return concat(*pyd.map_(array, iteratee))
 
 
-def nth(array, pos=0):
+def nth(array: t.Iterable[T], pos: int = 0) -> t.Union[T, None]:
     """
     Gets the element at index n of array.
 
     Args:
-        array (list): List passed in by the user.
-        pos (int): Index of element to return.
+        array: List passed in by the user.
+        pos: Index of element to return.
 
     Returns:
-        mixed: Returns the element at :attr:`pos`.
+        Returns the element at :attr:`pos`.
 
     Example:
 
         >>> nth([1, 2, 3], 0)
         1
         >>> nth([3, 4, 5, 6], 2)
         5
@@ -949,24 +1187,24 @@
         11
 
     .. versionadded:: 4.0.0
     """
     return pyd.get(array, pos)
 
 
-def pop(array, index=-1):
+def pop(array: t.List[T], index: int = -1) -> T:
     """
     Remove element of array at `index` and return element.
 
     Args:
-        array (list): List to pop from.
-        index (int, optional): Index to remove element from. Defaults to ``-1``.
+        array: List to pop from.
+        index: Index to remove element from. Defaults to ``-1``.
 
     Returns:
-        mixed: Value at `index`.
+        Value at `index`.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> array = [1, 2, 3, 4]
@@ -982,24 +1220,24 @@
         [2, 3]
 
     .. versionadded:: 2.2.0
     """
     return array.pop(index)
 
 
-def pull(array, *values):
+def pull(array: t.List[T], *values: T) -> t.List[T]:
     """
     Removes all provided values from the given array.
 
     Args:
-        array (list): List to pull from.
-        values (mixed): Values to remove.
+        array: List to pull from.
+        values: Values to remove.
 
     Returns:
-        list: Modified `array`.
+        Modified `array`.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> pull([1, 2, 2, 3, 3, 4], 2, 3)
@@ -1010,78 +1248,86 @@
     .. versionchanged:: 4.0.0
         :func:`pull` method now calls :func:`pull_all` method for the desired
         functionality.
     """
     return pull_all(array, values)
 
 
-def pull_all(array, values):
+def pull_all(array: t.List[T], values: t.Iterable[T]) -> t.List[T]:
     """
     Removes all provided values from the given array.
 
     Args:
-        array (list): Array to modify.
-        values (list): Values to remove.
+        array: Array to modify.
+        values: Values to remove.
 
     Returns:
-        list: Modified `array`.
+        Modified `array`.
 
     Example:
 
         >>> pull_all([1, 2, 2, 3, 3, 4], [2, 3])
         [1, 4]
 
     .. versionadded:: 4.0.0
     """
     # Use this style of assignment so that `array` is mutated.
     array[:] = without(array, *values)
     return array
 
 
-def pull_all_by(array, values, iteratee=None):
+def pull_all_by(
+    array: t.List[T],
+    values: t.Iterable[T],
+    iteratee: t.Union[IterateeObjT, t.Callable[[T], t.Any], None] = None,
+) -> t.List[T]:
     """
     This method is like :func:`pull_all` except that it accepts iteratee which is invoked for each
     element of array and values to generate the criterion by which they're compared. The iteratee is
     invoked with one argument: ``(value)``.
 
     Args:
-        array (list): Array to modify.
-        values (list): Values to remove.
-        iteratee (mixed, optional): Function to transform the elements of the arrays. Defaults to
+        array: Array to modify.
+        values: Values to remove.
+        iteratee: Function to transform the elements of the arrays. Defaults to
             :func:`.identity`.
 
     Returns:
-        list: Modified `array`.
+        Modified `array`.
 
     Example:
 
         >>> array = [{'x': 1}, {'x': 2}, {'x': 3}, {'x': 1}]
         >>> pull_all_by(array, [{'x': 1}, {'x': 3}], 'x')
         [{'x': 2}]
 
     .. versionadded:: 4.0.0
     """
     values = difference(array, difference_by(array, values, iteratee=iteratee))
     return pull_all(array, values)
 
 
-def pull_all_with(array, values, comparator=None):
+def pull_all_with(
+    array: t.List[T],
+    values: t.Iterable[T],
+    comparator: t.Union[t.Callable[[T, T], t.Any], None] = None,
+) -> t.List[T]:
     """
     This method is like :func:`pull_all` except that it accepts comparator which is invoked to
     compare elements of array to values. The comparator is invoked with two arguments: ``(arr_val,
     oth_val)``.
 
     Args:
-        array (list): Array to modify.
-        values (list): Values to remove.
-        comparator (callable, optional): Function to compare the elements of the arrays. Defaults to
+        array: Array to modify.
+        values: Values to remove.
+        comparator: Function to compare the elements of the arrays. Defaults to
             :func:`.is_equal`.
 
     Returns:
-        list: Modified `array`.
+        Modified `array`.
 
     Example:
 
         >>> array = [{'x': 1, 'y': 2}, {'x': 3, 'y': 4}, {'x': 5, 'y': 6}]
         >>> res = pull_all_with(array, [{'x': 3, 'y': 4}], lambda a, b: a == b)
         >>> res == [{'x': 1, 'y': 2}, {'x': 5, 'y': 6}]
         True
@@ -1092,53 +1338,53 @@
 
     .. versionadded:: 4.0.0
     """
     values = difference(array, difference_with(array, values, comparator=comparator))
     return pull_all(array, values)
 
 
-def pull_at(array, *indexes):
+def pull_at(array: t.List[T], *indexes: int) -> t.List[T]:
     """
     Removes elements from `array` corresponding to the specified indexes and returns a list of the
     removed elements. Indexes may be specified as a list of indexes or as individual arguments.
 
     Args:
-        array (list): List to pull from.
-        indexes (int): Indexes to pull.
+        array: List to pull from.
+        indexes: Indexes to pull.
 
     Returns:
-        list: Modified `array`.
+        Modified `array`.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> pull_at([1, 2, 3, 4], 0, 2)
         [2, 4]
 
     .. versionadded:: 1.1.0
     """
-    indexes = flatten(indexes)
-    for index in sorted(indexes, reverse=True):
+    flat_indexes = flatten(indexes)
+    for index in sorted(flat_indexes, reverse=True):
         del array[index]
 
     return array
 
 
-def push(array, *items):
+def push(array: t.List[T], *items: T2) -> t.List[t.Union[T, T2]]:
     """
     Push items onto the end of `array` and return modified `array`.
 
     Args:
-        array (list): List to push to.
-        items (mixed): Items to append.
+        array: List to push to.
+        items: Items to append.
 
     Returns:
-        list: Modified `array`.
+        Modified `array`.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> array = [1, 2, 3]
@@ -1147,29 +1393,37 @@
 
     .. versionadded:: 2.2.0
 
     .. versionchanged:: 4.0.0
         Removed alias ``append``.
     """
     for item in items:
-        array.append(item)
-    return array
+        array.append(item)  # type: ignore
+    return array  # type: ignore
 
 
-def remove(array, predicate=None):
+def remove(
+    array: t.List[T],
+    predicate: t.Union[
+        t.Callable[[T, int, t.List[T]], t.Any],
+        t.Callable[[T, int], t.Any],
+        t.Callable[[T], t.Any],
+        None,
+    ] = None,
+) -> t.List[T]:
     """
     Removes all elements from a list that the predicate returns truthy for and returns an array of
     removed elements.
 
     Args:
-        array (list): List to remove elements from.
-        predicate (mixed, optional): Predicate applied per iteration.
+        array: List to remove elements from.
+        predicate: Predicate applied per iteration.
 
     Returns:
-        list: Removed elements of `array`.
+        Removed elements of `array`.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> array = [1, 2, 3, 4]
@@ -1192,45 +1446,44 @@
 
     # Modify array in place.
     array[:] = kept
 
     return removed
 
 
-def reverse(array):
+def reverse(array: SequenceT) -> SequenceT:
     """
     Return `array` in reverse order.
 
     Args:
-        array (list|string): Object to process.
+        array: Object to process.
 
     Returns:
-        list|string: Reverse of object.
+        Reverse of object.
 
     Example:
 
         >>> reverse([1, 2, 3, 4])
         [4, 3, 2, 1]
 
     .. versionadded:: 2.2.0
     """
-    # NOTE: Using this method to reverse object since it works for both lists
-    # and strings.
-    return array[::-1]
+    # NOTE: Using this method to reverse object since it works for both lists and strings.
+    return array[::-1]  # type: ignore
 
 
-def shift(array):
+def shift(array: t.List[T]) -> T:
     """
     Remove the first element of `array` and return it.
 
     Args:
-        array (list): List to shift.
+        array: List to shift.
 
     Returns:
-        mixed: First element of `array`.
+        First element of `array`.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> array = [1, 2, 3, 4]
@@ -1241,25 +1494,25 @@
         [2, 3, 4]
 
     .. versionadded:: 2.2.0
     """
     return pop(array, 0)
 
 
-def slice_(array, start=0, end=None):
+def slice_(array: SequenceT, start: int = 0, end: t.Union[int, None] = None) -> SequenceT:
     """
     Slices `array` from the `start` index up to, but not including, the `end` index.
 
     Args:
-        array (list): Array to slice.
-        start (int, optional): Start index. Defaults to ``0``.
-        end (int, optional): End index. Defaults to selecting the value at ``start`` index.
+        array: Array to slice.
+        start: Start index. Defaults to ``0``.
+        end: End index. Defaults to selecting the value at ``start`` index.
 
     Returns:
-        list: Sliced list.
+        Sliced list.
 
     Example:
 
         >>> slice_([1, 2, 3, 4])
         [1]
         >>> slice_([1, 2, 3, 4], 1)
         [2]
@@ -1267,41 +1520,64 @@
         [2, 3]
 
     .. versionadded:: 1.1.0
     """
     if end is None:
         end = (start + 1) if start >= 0 else (len(array) + start + 1)
 
-    return array[start:end]
+    return array[start:end]  # type: ignore
+
+
+@t.overload
+def sort(
+    array: t.List["SupportsRichComparisonT"],
+    comparator: None = None,
+    key: None = None,
+    reverse: bool = False,
+) -> t.List["SupportsRichComparisonT"]:
+    ...
+
+
+@t.overload
+def sort(
+    array: t.List[T], comparator: t.Callable[[T, T], int], *, reverse: bool = False
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def sort(
+    array: t.List[T], *, key: t.Callable[[T], "SupportsRichComparisonT"], reverse: bool = False
+) -> t.List[T]:
+    ...
 
 
 def sort(array, comparator=None, key=None, reverse=False):
     """
     Sort `array` using optional `comparator`, `key`, and `reverse` options and return sorted
     `array`.
 
     Note:
         Python 3 removed the option to pass a custom comparator function and instead only allows a
         key function. Therefore, if a comparator function is passed in, it will be converted to a
         key function automatically using ``functools.cmp_to_key``.
 
     Args:
-        array (list): List to sort.
-        comparator (callable, optional): A custom comparator function used to sort the list.
+        array: List to sort.
+        comparator: A custom comparator function used to sort the list.
             Function should accept two arguments and return a negative, zero, or position number
             depending on whether the first argument is considered smaller than, equal to, or larger
             than the second argument. Defaults to ``None``. This argument is mutually exclusive with
             `key`.
-        key (iteratee, optional): A function of one argument used to extract a a comparator key from
-            each list element. Defaults to ``None``. This argument is mutually exclusive with
-            `comparator`.
-        reverse (bool, optional): Whether to reverse the sort. Defaults to ``False``.
+        key: A function of one argument used to extract a comparator key from each list element.
+            Defaults to ``None``. This argument is mutually exclusive with `comparator`.
+        reverse: Whether to reverse the sort. Defaults to ``False``.
 
     Returns:
-        list: Sorted list.
+        Sorted list.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> sort([2, 1, 4, 3])
@@ -1324,52 +1600,72 @@
     if comparator:
         key = cmp_to_key(comparator)
 
     array.sort(key=key, reverse=reverse)
     return array
 
 
-def sorted_index(array, value):
+def sorted_index(
+    array: t.Sequence["SupportsRichComparisonT"], value: "SupportsRichComparisonT"
+) -> int:
     """
     Uses a binary search to determine the lowest index at which `value` should be inserted into
     `array` in order to maintain its sort order.
 
     Args:
-        array (list): List to inspect.
-        value (mixed): Value to evaluate.
+        array: List to inspect.
+        value: Value to evaluate.
 
     Returns:
-        int: Returns the index at which `value` should be inserted into `array`.
+        Returns the index at which `value` should be inserted into `array`.
 
     Example:
 
         >>> sorted_index([1, 2, 2, 3, 4], 2)
         1
 
     .. versionadded:: 1.0.0
 
     .. versionchanged:: 4.0.0
         Move iteratee support to :func:`sorted_index_by`.
     """
     return sorted_index_by(array, value)
 
 
+@t.overload
+def sorted_index_by(
+    array: t.Sequence[T],
+    value: T,
+    iteratee: t.Union[IterateeObjT, t.Callable[[T], "SupportsRichComparisonT"]],
+) -> int:
+    ...
+
+
+@t.overload
+def sorted_index_by(
+    array: t.Sequence["SupportsRichComparisonT"],
+    value: "SupportsRichComparisonT",
+    iteratee: None = None,
+) -> int:
+    ...
+
+
 def sorted_index_by(array, value, iteratee=None):
     """
     This method is like :func:`sorted_index` except that it accepts iteratee which is invoked for
     `value` and each element of `array` to compute their sort ranking. The iteratee is invoked with
     one argument: ``(value)``.
 
     Args:
-        array (list): List to inspect.
-        value (mixed): Value to evaluate.
-        iteratee (mixed, optional): The iteratee invoked per element. Defaults to :func:`.identity`.
+        array: List to inspect.
+        value: Value to evaluate.
+        iteratee: The iteratee invoked per element. Defaults to :func:`.identity`.
 
     Returns:
-        int: Returns the index at which `value` should be inserted into `array`.
+        Returns the index at which `value` should be inserted into `array`.
 
     Example:
 
         >>> array = [{'x': 4}, {'x': 5}]
         >>> sorted_index_by(array, {'x': 4}, lambda o: o['x'])
         0
         >>> sorted_index_by(array, {'x': 4}, 'x')
@@ -1382,24 +1678,26 @@
         iteratee = pyd.iteratee(iteratee)
         array = sorted(iteratee(item) for item in array)
         value = iteratee(value)
 
     return bisect_left(array, value)
 
 
-def sorted_index_of(array, value):
+def sorted_index_of(
+    array: t.Sequence["SupportsRichComparisonT"], value: "SupportsRichComparisonT"
+) -> int:
     """
     Returns the index of the matched `value` from the sorted `array`, else ``-1``.
 
     Args:
-        array (list): Array to inspect.
-        value (mixed): Value to search for.
+        array: Array to inspect.
+        value: Value to search for.
 
     Returns:
-        int: Returns the index of the first matched value, else ``-1``.
+        Returns the index of the first matched value, else ``-1``.
 
     Example:
 
         >>> sorted_index_of([3, 5, 7, 10], 3)
         0
         >>> sorted_index_of([10, 10, 5, 7, 3], 10)
         -1
@@ -1410,52 +1708,72 @@
 
     if index < len(array) and array[index] == value:
         return index
     else:
         return -1
 
 
-def sorted_last_index(array, value):
+def sorted_last_index(
+    array: t.Sequence["SupportsRichComparisonT"], value: "SupportsRichComparisonT"
+) -> int:
     """
     This method is like :func:`sorted_index` except that it returns the highest index at which
     `value` should be inserted into `array` in order to maintain its sort order.
 
     Args:
-        array (list): List to inspect.
-        value (mixed): Value to evaluate.
+        array: List to inspect.
+        value: Value to evaluate.
 
     Returns:
-        int: Returns the index at which `value` should be inserted into `array`.
+        Returns the index at which `value` should be inserted into `array`.
 
     Example:
 
         >>> sorted_last_index([1, 2, 2, 3, 4], 2)
         3
 
     .. versionadded:: 1.1.0
 
     .. versionchanged:: 4.0.0
         Move iteratee support to :func:`sorted_last_index_by`.
     """
     return sorted_last_index_by(array, value)
 
 
+@t.overload
+def sorted_last_index_by(
+    array: t.Sequence[T],
+    value: T,
+    iteratee: t.Union[IterateeObjT, t.Callable[[T], "SupportsRichComparisonT"]],
+) -> int:
+    ...
+
+
+@t.overload
+def sorted_last_index_by(
+    array: t.Sequence["SupportsRichComparisonT"],
+    value: "SupportsRichComparisonT",
+    iteratee: None = None,
+) -> int:
+    ...
+
+
 def sorted_last_index_by(array, value, iteratee=None):
     """
     This method is like :func:`sorted_last_index` except that it accepts iteratee which is invoked
     for `value` and each element of `array` to compute their sort ranking. The iteratee is invoked
     with one argument: ``(value)``.
 
     Args:
-        array (list): List to inspect.
-        value (mixed): Value to evaluate.
-        iteratee (mixed, optional): The iteratee invoked per element. Defaults to :func:`.identity`.
+        array: List to inspect.
+        value: Value to evaluate.
+        iteratee: The iteratee invoked per element. Defaults to :func:`.identity`.
 
     Returns:
-        int: Returns the index at which `value` should be inserted into `array`.
+        Returns the index at which `value` should be inserted into `array`.
 
     Example:
 
         >>> array = [{'x': 4}, {'x': 5}]
         >>> sorted_last_index_by(array, {'x': 4}, lambda o: o['x'])
         1
         >>> sorted_last_index_by(array, {'x': 4}, 'x')
@@ -1466,25 +1784,27 @@
         iteratee = pyd.iteratee(iteratee)
         array = sorted(iteratee(item) for item in array)
         value = iteratee(value)
 
     return bisect_right(array, value)
 
 
-def sorted_last_index_of(array, value):
+def sorted_last_index_of(
+    array: t.Sequence["SupportsRichComparisonT"], value: "SupportsRichComparisonT"
+) -> int:
     """
     This method is like :func:`last_index_of` except that it performs a binary search on a sorted
     `array`.
 
     Args:
-        array (list): Array to inspect.
-        value (mixed): Value to search for.
+        array: Array to inspect.
+        value: Value to search for.
 
     Returns:
-        int: Returns the index of the matched value, else ``-1``.
+        Returns the index of the matched value, else ``-1``.
 
     Example:
 
         >>> sorted_last_index_of([4, 5, 5, 5, 6], 5)
         3
         >>> sorted_last_index_of([6, 5, 5, 5, 4], 6)
         -1
@@ -1495,76 +1815,83 @@
 
     if index < len(array) and array[index] == value:
         return index
     else:
         return -1
 
 
-def sorted_uniq(array):
+def sorted_uniq(array: t.Iterable["SupportsRichComparisonT"]) -> t.List["SupportsRichComparisonT"]:
     """
     Return sorted array with unique elements.
 
     Args:
-        array (list): List of values to be sorted.
+        array: List of values to be sorted.
 
     Returns:
-        list: List of unique elements in a sorted fashion.
+        List of unique elements in a sorted fashion.
 
     Example:
 
         >>> sorted_uniq([4, 2, 2, 5])
         [2, 4, 5]
         >>> sorted_uniq([-2, -2, 4, 1])
         [-2, 1, 4]
 
     .. versionadded:: 4.0.0
     """
     return sorted(uniq(array))
 
 
-def sorted_uniq_by(array, iteratee=None):
+def sorted_uniq_by(
+    array: t.Iterable["SupportsRichComparisonT"],
+    iteratee: t.Union[
+        t.Callable[["SupportsRichComparisonT"], "SupportsRichComparisonT"], None
+    ] = None,
+) -> t.List["SupportsRichComparisonT"]:
     """
     This method is like :func:`sorted_uniq` except that it accepts iteratee which is invoked for
     each element in array to generate the criterion by which uniqueness is computed. The order of
     result values is determined by the order they occur in the array. The iteratee is invoked with
     one argument: ``(value)``.
 
     Args:
-        array (list): List of values to be sorted.
-        iteratee (mixed, optional): Function to transform the elements of the arrays. Defaults to
+        array: List of values to be sorted.
+        iteratee: Function to transform the elements of the arrays. Defaults to
             :func:`.identity`.
 
     Returns:
-        list: Unique list.
+        Unique list.
 
     Example:
 
         >>> sorted_uniq_by([3, 2, 1, 3, 2, 1], lambda val: val % 2)
         [2, 3]
 
     .. versionadded:: 4.0.0
     """
     return sorted(uniq_by(array, iteratee=iteratee))
 
 
-def splice(array, start, count=None, *items):
+def splice(
+    array: MutableSequenceT, start: int, count: t.Union[int, None] = None, *items: t.Any
+) -> MutableSequenceT:
     """
     Modify the contents of `array` by inserting elements starting at index `start` and removing
     `count` number of elements after.
 
     Args:
-        array (list|str): List to splice.
-        start (int): Start to splice at.
-        count (int, optional): Number of items to remove starting at `start`. If ``None`` then all
+        array: List to splice.
+        start: Start to splice at.
+        count: Number of items to remove starting at `start`. If ``None`` then all
             items after `start` are removed. Defaults to ``None``.
-        items (mixed): Elements to insert starting at `start`. Each item is inserted in the order
+        items: Elements to insert starting at `start`. Each item is inserted in the order
             given.
 
     Returns:
-        list|str: The removed elements of `array` or the spliced string.
+        The removed elements of `array` or the spliced string.
 
     Warning:
         `array` is modified in place if ``list``.
 
     Example:
 
         >>> array = [1, 2, 3, 4]
@@ -1590,82 +1917,83 @@
     """
     if count is None:
         count = len(array) - start
 
     is_string = pyd.is_string(array)
 
     if is_string:
-        array = list(array)
+        # allow reassignment with different type
+        array = list(array)  # type: ignore
 
     removed = array[start : start + count]
     del array[start : start + count]
 
     for item in reverse(items):
         array.insert(start, item)
 
     if is_string:
-        return "".join(array)
+        return "".join(array)  # type: ignore
     else:
-        return removed
+        return removed  # type: ignore
 
 
-def split_at(array, index):
+def split_at(array: t.Sequence[T], index: int) -> t.List[t.Sequence[T]]:
     """
     Returns a list of two lists composed of the split of `array` at `index`.
 
     Args:
-        array (list): List to split.
-        index (int): Index to split at.
+        array: List to split.
+        index: Index to split at.
 
     Returns:
-        list: Split list.
+        Split list.
 
     Example:
 
         >>> split_at([1, 2, 3, 4], 2)
         [[1, 2], [3, 4]]
 
     .. versionadded:: 2.0.0
     """
     return [array[:index], array[index:]]
 
 
-def tail(array):
+def tail(array: t.Sequence[T]) -> t.Sequence[T]:
     """
     Return all but the first element of `array`.
 
     Args:
-        array (list): List to process.
+        array: List to process.
 
     Returns:
-        list: Rest of the list.
+        Rest of the list.
 
     Example:
 
         >>> tail([1, 2, 3, 4])
         [2, 3, 4]
 
     .. versionadded:: 1.0.0
 
     .. versionchanged:: 4.0.0
         Renamed from ``rest`` to ``tail``.
     """
     return array[1:]
 
 
-def take(array, n=1):
+def take(array: t.Sequence[T], n: int = 1) -> t.Sequence[T]:
     """
     Creates a slice of `array` with `n` elements taken from the beginning.
 
     Args:
-        array (list): List to process.
-        n (int, optional): Number of elements to take. Defaults to ``1``.
+        array: List to process.
+        n: Number of elements to take. Defaults to ``1``.
 
     Returns:
-        list: Taken list.
+        Taken list.
 
     Example:
 
         >>> take([1, 2, 3, 4], 2)
         [1, 2]
 
     .. versionadded:: 1.0.0
@@ -1675,24 +2003,24 @@
 
     .. versionchanged:: 3.0.0
         Made ``n`` default to ``1``.
     """
     return take_while(array, lambda _, index: index < n)
 
 
-def take_right(array, n=1):
+def take_right(array: t.Sequence[T], n: int = 1) -> t.Sequence[T]:
     """
     Creates a slice of `array` with `n` elements taken from the end.
 
     Args:
-        array (list): List to process.
-        n (int, optional): Number of elements to take. Defaults to ``1``.
+        array: List to process.
+        n: Number of elements to take. Defaults to ``1``.
 
     Returns:
-        list: Taken list.
+        Taken list.
 
     Example:
 
         >>> take_right([1, 2, 3, 4], 2)
         [3, 4]
 
     .. versionadded:: 1.1.0
@@ -1700,26 +2028,48 @@
     .. versionchanged:: 3.0.0
         Made ``n`` default to ``1``.
     """
     length = len(array)
     return take_right_while(array, lambda _, index: (length - index) <= n)
 
 
+@t.overload
+def take_right_while(
+    array: t.Sequence[T], predicate: t.Callable[[T, int, t.List[T]], t.Any]
+) -> t.Sequence[T]:
+    ...
+
+
+@t.overload
+def take_right_while(array: t.Sequence[T], predicate: t.Callable[[T, int], t.Any]) -> t.Sequence[T]:
+    ...
+
+
+@t.overload
+def take_right_while(array: t.Sequence[T], predicate: t.Callable[[T], t.Any]) -> t.Sequence[T]:
+    ...
+
+
+@t.overload
+def take_right_while(array: t.Sequence[T], predicate: None = None) -> t.Sequence[T]:
+    ...
+
+
 def take_right_while(array, predicate=None):
     """
     Creates a slice of `array` with elements taken from the end. Elements are taken until the
     `predicate` returns falsey. The `predicate` is invoked with three arguments: ``(value, index,
     array)``.
 
     Args:
-        array (list): List to process.
-        predicate (mixed): Predicate called per iteration
+        array: List to process.
+        predicate: Predicate called per iteration
 
     Returns:
-        list: Dropped list.
+        Dropped list.
 
     Example:
 
         >>> take_right_while([1, 2, 3, 4], lambda x: x >= 3)
         [3, 4]
 
     .. versionadded:: 1.1.0
@@ -1730,26 +2080,48 @@
             n -= 1
         else:
             break
 
     return array[n:]
 
 
+@t.overload
+def take_while(
+    array: t.Sequence[T], predicate: t.Callable[[T, int, t.List[T]], t.Any]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def take_while(array: t.Sequence[T], predicate: t.Callable[[T, int], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def take_while(array: t.Sequence[T], predicate: t.Callable[[T], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def take_while(array: t.Sequence[T], predicate: None = None) -> t.List[T]:
+    ...
+
+
 def take_while(array, predicate=None):
     """
     Creates a slice of `array` with elements taken from the beginning. Elements are taken until the
     `predicate` returns falsey. The `predicate` is invoked with three arguments: ``(value, index,
     array)``.
 
     Args:
-        array (list): List to process.
-        predicate (mixed): Predicate called per iteration
+        array: List to process.
+        predicate: Predicate called per iteration
 
     Returns:
-        list: Taken list.
+        Taken list.
 
     Example:
 
         >>> take_while([1, 2, 3, 4], lambda x: x < 3)
         [1, 2]
 
     .. versionadded:: 1.1.0
@@ -1760,52 +2132,76 @@
             n += 1
         else:
             break
 
     return array[:n]
 
 
+@t.overload
+def union(array: t.Sequence[T]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def union(array: t.Sequence[T], *others: t.Sequence[T2]) -> t.List[t.Union[T, T2]]:
+    ...
+
+
 def union(array, *others):
     """
     Computes the union of the passed-in arrays.
 
     Args:
-        array (list): List to union with.
-        others (list): Lists to unionize with `array`.
+        array: List to union with.
+        others: Lists to unionize with `array`.
 
     Returns:
-        list: Unionized list.
+        Unionized list.
 
     Example:
 
         >>> union([1, 2, 3], [2, 3, 4], [3, 4, 5])
         [1, 2, 3, 4, 5]
 
     .. versionadded:: 1.0.0
     """
     if not others:
         return array[:]
 
     return uniq(flatten([array] + list(others)))
 
 
+@t.overload
+def union_by(
+    array: t.Sequence[T], *others: t.Iterable[T], iteratee: t.Callable[[T], t.Any]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def union_by(
+    array: t.Sequence[T], *others: t.Union[t.Iterable[T], t.Callable[[T], T]]
+) -> t.List[T]:
+    ...
+
+
 def union_by(array, *others, **kwargs):
     """
     This method is similar to :func:`union` except that it accepts iteratee which is invoked for
-    each element of each arrays to generate the criterion by which uniqueness is computed.
+    each element of each array to generate the criterion by which uniqueness is computed.
 
     Args:
-        array (list): List to unionize with.
-        others (list): Lists to unionize with `array`.
+        array: List to unionize with.
+        others: Lists to unionize with `array`.
 
     Keyword Args:
-        iteratee (callable): Function to invoke on each element.
+        iteratee: Function to invoke on each element.
 
     Returns:
-        list: Unionized list.
+        Unionized list.
 
     Example:
 
         >>> union_by([1, 2, 3], [2, 3, 4], iteratee=lambda x: x % 2)
         [1, 2]
         >>> union_by([1, 2, 3], [2, 3, 4], iteratee=lambda x: x % 9)
         [1, 2, 3, 4]
@@ -1816,29 +2212,43 @@
         return array[:]
 
     iteratee, others = parse_iteratee("iteratee", *others, **kwargs)
 
     return uniq_by(flatten([array] + list(others)), iteratee=iteratee)
 
 
+@t.overload
+def union_with(
+    array: t.Sequence[T], *others: t.Iterable[T2], comparator: t.Callable[[T, T2], t.Any]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def union_with(
+    array: t.Sequence[T], *others: t.Union[t.Iterable[T2], t.Callable[[T, T2], t.Any]]
+) -> t.List[T]:
+    ...
+
+
 def union_with(array, *others, **kwargs):
     """
     This method is like :func:`union` except that it accepts comparator which is invoked to compare
     elements of arrays. Result values are chosen from the first array in which the value occurs.
 
     Args:
-        array (list): List to unionize with.
-        others (list): Lists to unionize with `array`.
+        array: List to unionize with.
+        others: Lists to unionize with `array`.
 
     Keyword Args:
-        comparator (callable, optional): Function to compare the elements of the arrays. Defaults to
+        comparator: Function to compare the elements of the arrays. Defaults to
             :func:`.is_equal`.
 
     Returns:
-        list: Unionized list.
+        Unionized list.
 
     Example:
 
         >>> comparator = lambda a, b: (a % 2) == (b % 2)
         >>> union_with([1, 2, 3], [2, 3, 4], comparator=comparator)
         [1, 2]
         >>> union_with([1, 2, 3], [2, 3, 4])
@@ -1850,28 +2260,28 @@
         return array[:]
 
     comparator, others = parse_iteratee("comparator", *others, **kwargs)
 
     return uniq_with(flatten([array] + list(others)), comparator=comparator)
 
 
-def uniq(array):
+def uniq(array: t.Iterable[T]) -> t.List[T]:
     """
     Creates a duplicate-value-free version of the array. If iteratee is passed, each element of
-    array is passed through a iteratee before uniqueness is computed. The iteratee is invoked with
+    array is passed through an iteratee before uniqueness is computed. The iteratee is invoked with
     three arguments: ``(value, index, array)``. If an object path is passed for iteratee, the
     created iteratee will return the path value of the given element. If an object is passed for
     iteratee, the created filter style iteratee will return ``True`` for elements that have the
     properties of the given object, else ``False``.
 
     Args:
-        array (list): List to process.
+        array: List to process.
 
     Returns:
-        list: Unique list.
+        Unique list.
 
     Example:
 
         >>> uniq([1, 2, 3, 1, 2, 3])
         [1, 2, 3]
 
     .. versionadded:: 1.0.0
@@ -1880,73 +2290,75 @@
 
         - Moved `iteratee` argument to :func:`uniq_by`.
         - Removed alias ``unique``.
     """
     return uniq_by(array)
 
 
-def uniq_by(array, iteratee=None):
+def uniq_by(array: t.Iterable[T], iteratee: t.Union[t.Callable[[T], T], None] = None) -> t.List[T]:
     """
     This method is like :func:`uniq` except that it accepts iteratee which is invoked for each
     element in array to generate the criterion by which uniqueness is computed. The order of result
     values is determined by the order they occur in the array. The iteratee is invoked with one
     argument: ``(value)``.
 
     Args:
-        array (list): List to process.
-        iteratee (mixed, optional): Function to transform the elements of the arrays. Defaults to
+        array: List to process.
+        iteratee: Function to transform the elements of the arrays. Defaults to
             :func:`.identity`.
 
     Returns:
-        list: Unique list.
+        Unique list.
 
     Example:
 
         >>> uniq_by([1, 2, 3, 1, 2, 3], lambda val: val % 2)
         [1, 2]
 
     .. versionadded:: 4.0.0
     """
     return list(iterunique(array, iteratee=iteratee))
 
 
-def uniq_with(array, comparator=None):
+def uniq_with(
+    array: t.Sequence[T], comparator: t.Union[t.Callable[[T, T], t.Any], None] = None
+) -> t.List[T]:
     """
     This method is like :func:`uniq` except that it accepts comparator which is invoked to compare
     elements of array. The order of result values is determined by the order they occur in the
     array.The comparator is invoked with two arguments: ``(value, other)``.
 
     Args:
-        array (list): List to process.
-        comparator (callable, optional): Function to compare the elements of the arrays. Defaults to
+        array: List to process.
+        comparator: Function to compare the elements of the arrays. Defaults to
             :func:`.is_equal`.
 
     Returns:
-        list: Unique list.
+        Unique list.
 
     Example:
 
         >>> uniq_with([1, 2, 3, 4, 5], lambda a, b: (a % 2) == (b % 2))
         [1, 2]
 
     .. versionadded:: 4.0.0
     """
     return list(iterunique(array, comparator=comparator))
 
 
-def unshift(array, *items):
+def unshift(array: t.List[T], *items: T2) -> t.List[t.Union[T, T2]]:
     """
     Insert the given elements at the beginning of `array` and return the modified list.
 
     Args:
-        array (list): List to modify.
-        items (mixed): Items to insert.
+        array: List to modify.
+        items: Items to insert.
 
     Returns:
-        list: Modified list.
+        Modified list.
 
     Warning:
         `array` is modified in place.
 
     Example:
 
         >>> array = [1, 2, 3, 4]
@@ -1954,52 +2366,73 @@
         [-1, -2, 1, 2, 3, 4]
         >>> array
         [-1, -2, 1, 2, 3, 4]
 
     .. versionadded:: 2.2.0
     """
     for item in reverse(items):
-        array.insert(0, item)
+        array.insert(0, item)  # type: ignore
 
-    return array
+    return array  # type: ignore
 
 
-def unzip(array):
+def unzip(array: t.Iterable[t.Iterable[T]]) -> t.List[t.List[T]]:
     """
     The inverse of :func:`zip_`, this method splits groups of elements into lists composed of
     elements from each group at their corresponding indexes.
 
     Args:
-        array (list): List to process.
+        array: List to process.
 
     Returns:
-        list: Unzipped list.
+        Unzipped list.
 
     Example:
 
         >>> unzip([[1, 4, 7], [2, 5, 8], [3, 6, 9]])
         [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
 
     .. versionadded:: 1.0.0
     """
     return zip_(*array)
 
 
+@t.overload
+def unzip_with(
+    array: t.Iterable[t.Iterable[T]],
+    iteratee: t.Union[
+        t.Callable[[T, T, int, t.List[T]], T2],
+        t.Callable[[T, T, int], T2],
+        t.Callable[[T, T], T2],
+        t.Callable[[T], T2],
+    ],
+) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def unzip_with(
+    array: t.Iterable[t.Iterable[T]],
+    iteratee: None = None,
+) -> t.List[t.List[T]]:
+    ...
+
+
 def unzip_with(array, iteratee=None):
     """
-    This method is like :func:`unzip` except that it accepts a iteratee to specify how regrouped
+    This method is like :func:`unzip` except that it accepts an iteratee to specify how regrouped
     values should be combined. The iteratee is invoked with four arguments: ``(accumulator, value,
     index, group)``.
 
     Args:
-        array (list): List to process.
-        iteratee (callable, optional): Function to combine regrouped values.
+        array: List to process.
+        iteratee: Function to combine regrouped values.
 
     Returns:
-        list: Unzipped list.
+        Unzipped list.
 
     Example:
 
         >>> from pydash import add
         >>> unzip_with([[1, 10, 100], [2, 20, 200]], add)
         [3, 30, 300]
 
@@ -2015,73 +2448,85 @@
 
     def cbk(group):
         return pyd.reduce_(group, iteratee)
 
     return pyd.map_(result, cbk)
 
 
-def without(array, *values):
+def without(array: t.Iterable[T], *values: T) -> t.List[T]:
     """
     Creates an array with all occurrences of the passed values removed.
 
     Args:
-        array (list): List to filter.
-        values (mixed): Values to remove.
+        array: List to filter.
+        values: Values to remove.
 
     Returns:
-        list: Filtered list.
+        Filtered list.
 
     Example:
 
         >>> without([1, 2, 3, 2, 4, 4], 2, 4)
         [1, 3]
 
     .. versionadded:: 1.0.0
     """
     return [item for item in array if item not in values]
 
 
-def xor(array, *lists):
+def xor(array: t.Iterable[T], *lists: t.Iterable[T]) -> t.List[T]:
     """
     Creates a list that is the symmetric difference of the provided lists.
 
     Args:
-        array (list): List to process.
-        *lists (list): Lists to xor with.
+        array: List to process.
+        *lists: Lists to xor with.
 
     Returns:
-        list: XOR'd list.
+        XOR'd list.
 
     Example:
 
         >>> xor([1, 3, 4], [1, 2, 4], [2])
         [3]
 
     .. versionadded:: 1.0.0
     """
     return xor_by(array, *lists)
 
 
+@t.overload
+def xor_by(
+    array: t.Iterable[T], *lists: t.Iterable[T], iteratee: t.Union[t.Callable[[T], T], IterateeObjT]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def xor_by(array: t.Iterable[T], *lists: t.Union[t.Iterable[T], t.Callable[[T], T]]) -> t.List[T]:
+    ...
+
+
 def xor_by(array, *lists, **kwargs):
     """
     This method is like :func:`xor` except that it accepts iteratee which is invoked for each
-    element of each arrays to generate the criterion by which by which they're compared. The order
-    of result values is determined by the order they occur in the arrays. The iteratee is invoked
-    with one argument: ``(value)``.
+    element of each arras to generate the criterion by which they're compared. The order of result
+    values is determined by the order they occur in the arrays. The iteratee is invoked with one
+    argument: ``(value)``.
 
     Args:
-        array (list): List to process.
-        *lists (list): Lists to xor with.
+        array: List to process.
+        *lists: Lists to xor with.
 
     Keyword Args:
-        iteratee (mixed, optional): Function to transform the elements of the arrays. Defaults to
+        iteratee: Function to transform the elements of the arrays. Defaults to
             :func:`.identity`.
 
     Returns:
-        list: XOR'd list.
+        XOR'd list.
 
     Example:
 
         >>> xor_by([2.1, 1.2], [2.3, 3.4], round)
         [1.2, 3.4]
         >>> xor_by([{'x': 1}], [{'x': 2}, {'x': 1}], 'x')
         [{'x': 2}]
@@ -2097,34 +2542,48 @@
         uniq(
             difference_by(
                 array + lists[0],
                 intersection_by(array, lists[0], iteratee=iteratee),
                 iteratee=iteratee,
             )
         ),
-        *lists[1:]
+        *lists[1:],
     )
 
 
+@t.overload
+def xor_with(
+    array: t.Sequence[T], *lists: t.Iterable[T2], comparator: t.Callable[[T, T2], t.Any]
+) -> t.List[T]:
+    ...
+
+
+@t.overload
+def xor_with(
+    array: t.Sequence[T], *lists: t.Union[t.Iterable[T2], t.Callable[[T, T2], t.Any]]
+) -> t.List[T]:
+    ...
+
+
 def xor_with(array, *lists, **kwargs):
     """
     This method is like :func:`xor` except that it accepts comparator which is invoked to compare
     elements of arrays. The order of result values is determined by the order they occur in the
     arrays. The comparator is invoked with two arguments: ``(arr_val, oth_val)``.
 
     Args:
-        array (list): List to process.
-        *lists (list): Lists to xor with.
+        array: List to process.
+        *lists: Lists to xor with.
 
     Keyword Args:
-        comparator (callable, optional): Function to compare the elements of the arrays. Defaults to
+        comparator: Function to compare the elements of the arrays. Defaults to
             :func:`.is_equal`.
 
     Returns:
-        list: XOR'd list.
+        XOR'd list.
 
     Example:
 
         >>> objects = [{'x': 1, 'y': 2}, {'x': 2, 'y': 1}]
         >>> others = [{'x': 1, 'y': 1}, {'x': 1, 'y': 2}]
         >>> expected = [{'y': 1, 'x': 2}, {'y': 1, 'x': 1}]
         >>> xor_with(objects, others, lambda a, b: a == b) == expected
@@ -2141,52 +2600,69 @@
         uniq(
             difference_with(
                 array + lists[0],
                 intersection_with(array, lists[0], comparator=comp),
                 comparator=comp,
             )
         ),
-        *lists[1:]
+        *lists[1:],
     )
 
 
-def zip_(*arrays):
+def zip_(*arrays: t.Iterable[T]) -> t.List[t.List[T]]:
     """
     Groups the elements of each array at their corresponding indexes. Useful for separate data
     sources that are coordinated through matching array indexes.
 
     Args:
-        arrays (list): Lists to process.
+        arrays: Lists to process.
 
     Returns:
-        list: Zipped list.
+        Zipped list.
 
     Example:
 
         >>> zip_([1, 2, 3], [4, 5, 6], [7, 8, 9])
         [[1, 4, 7], [2, 5, 8], [3, 6, 9]]
 
     .. versionadded:: 1.0.0
     """
     # zip returns as a list of tuples so convert to list of lists
     return [list(item) for item in zip(*arrays)]
 
 
+@t.overload
+def zip_object(keys: t.Iterable[t.Tuple[T, T2]], values: None = None) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def zip_object(
+    keys: t.Iterable[t.List[t.Union[T, T2]]], values: None = None
+) -> t.Dict[t.Union[T, T2], t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def zip_object(keys: t.Iterable[T], values: t.List[T2]) -> t.Dict[T, T2]:
+    ...
+
+
 def zip_object(keys, values=None):
     """
-    Creates a dict composed from lists of keys and values. Pass either a single two dimensional
-    list, i.e. ``[[key1, value1], [key2, value2]]``, or two lists, one of keys and one of
-    corresponding values.
+    Creates a dict composed of lists of keys and values. Pass either a single two-dimensional list,
+    i.e. ``[[key1, value1], [key2, value2]]``, or two lists, one of keys and one of corresponding
+    values.
 
     Args:
-        keys (list): Either a list of keys or a list of ``[key, value]`` pairs.
-        values (list, optional): List of values to zip.
+        keys: Either a list of keys or a list of ``[key, value]`` pairs.
+        values: List of values to zip.
 
     Returns:
-        dict: Zipped dict.
+        Zipped dict.
 
     Example:
 
         >>> zip_object([1, 2, 3], [4, 5, 6])
         {1: 4, 2: 5, 3: 6}
 
     .. versionadded:: 1.0.0
@@ -2197,57 +2673,88 @@
 
     if values is None:
         keys, values = unzip(keys)
 
     return dict(zip(keys, values))
 
 
-def zip_object_deep(keys, values=None):
+def zip_object_deep(keys: t.Iterable[t.Any], values: t.Union[t.List[t.Any], None] = None) -> t.Dict:
     """
     This method is like :func:`zip_object` except that it supports property paths.
 
     Args:
-        keys (list): Either a list of keys or a list of ``[key, value]`` pairs.
-        values (list, optional): List of values to zip.
+        keys: Either a list of keys or a list of ``[key, value]`` pairs.
+        values: List of values to zip.
 
     Returns:
-        dict: Zipped dict.
+        Zipped dict.
 
     Example:
 
         >>> expected = {'a': {'b': {'c': 1, 'd': 2}}}
         >>> zip_object_deep(['a.b.c', 'a.b.d'], [1, 2]) == expected
         True
 
     .. versionadded:: 4.0.0
     """
     if values is None:  # pragma: no cover
         keys, values = unzip(keys)
 
-    obj = {}
+    obj: t.Dict = {}
     for idx, key in enumerate(keys):
         obj = pyd.set_(obj, key, pyd.get(values, idx))
 
     return obj
 
 
+@t.overload
+def zip_with(
+    *arrays: t.Iterable[T],
+    iteratee: t.Union[
+        t.Callable[[T, T, int, t.List[T]], T2],
+        t.Callable[[T, T, int], T2],
+        t.Callable[[T, T], T2],
+        t.Callable[[T], T2],
+    ],
+) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def zip_with(*arrays: t.Iterable[T]) -> t.List[t.List[T]]:
+    ...
+
+
+@t.overload
+def zip_with(
+    *arrays: t.Union[
+        t.Iterable[T],
+        t.Callable[[T, T, int, t.List[T]], T2],
+        t.Callable[[T, T, int], T2],
+        t.Callable[[T, T], T2],
+        t.Callable[[T], T2],
+    ],
+) -> t.List[t.Union[t.List[T], T2]]:
+    ...
+
+
 def zip_with(*arrays, **kwargs):
     """
-    This method is like :func:`zip` except that it accepts a iteratee to specify how grouped values
+    This method is like :func:`zip` except that it accepts an iteratee to specify how grouped values
     should be combined. The iteratee is invoked with four arguments: ``(accumulator, value, index,
     group)``.
 
     Args:
-        *arrays (list): Lists to process.
+        *arrays: Lists to process.
 
     Keyword Args:
         iteratee (callable): Function to combine grouped values.
 
     Returns:
-        list: Zipped list of grouped elements.
+        Zipped list of grouped elements.
 
     Example:
 
         >>> from pydash import add
         >>> zip_with([1, 2], [10, 20], [100, 200], add)
         [111, 222]
         >>> zip_with([1, 2], [10, 20], [100, 200], iteratee=add)
```

### Comparing `pydash-6.0.2/src/pydash/chaining.py` & `pydash-7.0.0/src/pydash/chaining/chaining.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,159 +1,126 @@
 """
 Method chaining interface.
 
 .. versionadded:: 1.0.0
 """
 
+import typing as t
+
 import pydash as pyd
+from pydash.exceptions import InvalidMethod
 
-from .helpers import UNSET
+from ..helpers import UNSET, Unset
+from .all_funcs import AllFuncs
 
 
 __all__ = (
     "chain",
     "tap",
     "thru",
 )
 
+Value_coT = t.TypeVar("Value_coT", covariant=True)
+T = t.TypeVar("T")
+T2 = t.TypeVar("T2")
+
 
-class Chain(object):
+class Chain(AllFuncs, t.Generic[Value_coT]):
     """Enables chaining of :attr:`module` functions."""
 
     #: Object that contains attribute references to available methods.
     module = pyd
+    invalid_method_exception = InvalidMethod
 
-    def __init__(self, value=UNSET):
+    def __init__(self, value: t.Union[Value_coT, Unset] = UNSET) -> None:
         self._value = value
 
-    def value(self):
+    def _wrap(self, func) -> "ChainWrapper":
+        """Implement `AllFuncs` interface."""
+        return ChainWrapper(self._value, func)
+
+    def value(self) -> Value_coT:
         """
         Return current value of the chain operations.
 
         Returns:
-            mixed: Current value of chain operations.
+            Current value of chain operations.
         """
         return self(self._value)
 
-    def to_string(self):
+    def to_string(self) -> str:
         """
         Return current value as string.
 
         Returns:
-            str: Current value of chain operations casted to ``str``.
+            Current value of chain operations casted to ``str``.
         """
         return self.module.to_string(self.value())
 
-    def commit(self):
+    def commit(self) -> "Chain[Value_coT]":
         """
         Executes the chained sequence and returns the wrapped result.
 
         Returns:
-            Chain: New instance of :class:`Chain` with resolved value from
+            New instance of :class:`Chain` with resolved value from
                 previous :class:`Class`.
         """
         return Chain(self.value())
 
-    def plant(self, value):
+    def plant(self, value: t.Any) -> "Chain[Value_coT]":
         """
         Return a clone of the chained sequence planting `value` as the wrapped value.
 
         Args:
-            value (mixed): Value to plant as the initial chain value.
+            value: Value to plant as the initial chain value.
         """
         # pylint: disable=no-member,maybe-no-member
         wrapper = self._value
         wrappers = []
 
         if hasattr(wrapper, "_value"):
             wrappers = [wrapper]
 
             while isinstance(wrapper._value, ChainWrapper):
-                wrapper = wrapper._value
+                wrapper = wrapper._value  # type: ignore
                 wrappers.insert(0, wrapper)
 
-        clone = Chain(value)
+        clone: Chain[t.Any] = Chain(value)
 
         for wrap in wrappers:
-            clone = ChainWrapper(clone._value, wrap.method)(*wrap.args, **wrap.kwargs)
+            clone = ChainWrapper(clone._value, wrap.method)(  # type: ignore
+                *wrap.args, **wrap.kwargs  # type: ignore
+            )
 
         return clone
 
-    @classmethod
-    def get_method(cls, name):
-        """
-        Return valid :attr:`module` method.
-
-        Args:
-            name (str): Name of pydash method to get.
-
-        Returns:
-            function: :attr:`module` callable.
-
-        Raises:
-            InvalidMethod: Raised if `name` is not a valid :attr:`module` method.
-        """
-        # Python 3.5 issue with pytest doctest call where inspect module tries
-        # to unwrap this class. If we don't return here, we get an
-        # InvalidMethod exception.
-        if name in ("__wrapped__",):  # pragma: no cover
-            return cls
-
-        method = getattr(cls.module, name, None)
-
-        if not callable(method) and not name.endswith("_"):
-            # Alias method names not ending in underscore to their underscore
-            # counterpart. This allows chaining of functions like "map_()"
-            # using "map()" instead.
-            method = getattr(cls.module, name + "_", None)
-
-        if not callable(method):
-            raise cls.module.InvalidMethod(f"Invalid pydash method: {name}")
-
-        return method
-
-    def __getattr__(self, attr):
-        """
-        Proxy attribute access to :attr:`module`.
-
-        Args:
-            attr (str): Name of :attr:`module` function to chain.
-
-        Returns:
-            ChainWrapper: New instance of :class:`ChainWrapper` with value passed on.
-
-        Raises:
-            InvalidMethod: Raised if `attr` is not a valid function.
-        """
-        return ChainWrapper(self._value, self.get_method(attr))
-
-    def __call__(self, value):
+    def __call__(self, value) -> Value_coT:
         """
         Return result of passing `value` through chained methods.
 
         Args:
-            value (mixed): Initial value to pass through chained methods.
+            value: Initial value to pass through chained methods.
 
         Returns:
-            mixed: Result of method chain evaluation of `value`.
+            Result of method chain evaluation of `value`.
         """
         if isinstance(self._value, ChainWrapper):
             # pylint: disable=maybe-no-member
             value = self._value.unwrap(value)
         return value
 
 
-class ChainWrapper(object):
+class ChainWrapper(t.Generic[Value_coT]):
     """Wrap :class:`Chain` method call within a :class:`ChainWrapper` context."""
 
-    def __init__(self, value, method):
+    def __init__(self, value: Value_coT, method) -> None:
         self._value = value
         self.method = method
         self.args = ()
-        self.kwargs = {}
+        self.kwargs: t.Dict = {}
 
     def _generate(self):
         """Generate a copy of this instance."""
         # pylint: disable=attribute-defined-outside-init
         new = self.__class__.__new__(self.__class__)
         new.__dict__ = self.__dict__.copy()
         return new
@@ -186,15 +153,15 @@
 
     def __call__(self, *args, **kwargs):
         """
         Invoke the :attr:`method` with :attr:`value` as the first argument and return a new
         :class:`Chain` object with the return value.
 
         Returns:
-            Chain: New instance of :class:`Chain` with the results of :attr:`method` passed in as
+            New instance of :class:`Chain` with the results of :attr:`method` passed in as
                 value.
         """
         self.args = args
         self.kwargs = kwargs
         return Chain(self)
 
 
@@ -202,29 +169,29 @@
     """Class that provides attribute access to valid :mod:`pydash` methods and callable access to
     :mod:`pydash` method chaining."""
 
     def __getattr__(self, attr):
         """Proxy to :meth:`Chain.get_method`."""
         return Chain.get_method(attr)
 
-    def __call__(self, value=UNSET):
+    def __call__(self, value: t.Union[Value_coT, Unset] = UNSET) -> Chain[Value_coT]:
         """Return a new instance of :class:`Chain` with `value` as the seed."""
         return Chain(value)
 
 
-def chain(value=UNSET):
+def chain(value: t.Union[T, Unset] = UNSET) -> Chain[T]:
     """
     Creates a :class:`Chain` object which wraps the given value to enable intuitive method chaining.
     Chaining is lazy and won't compute a final value until :meth:`Chain.value` is called.
 
     Args:
-        value (mixed): Value to initialize chain operations with.
+        value: Value to initialize chain operations with.
 
     Returns:
-        :class:`Chain`: Instance of :class:`Chain` initialized with `value`.
+        Instance of :class:`Chain` initialized with `value`.
 
     Example:
 
         >>> chain([1, 2, 3, 4]).map(lambda x: x * 2).sum().value()
         20
         >>> chain().map(lambda x: x * 2).sum()([1, 2, 3, 4])
         20
@@ -263,26 +230,26 @@
         - Added :meth:`Chain.plant` for replacing initial chain value.
         - Added :meth:`Chain.commit` for returning a new :class:`Chain` instance initialized with
           the results from calling :meth:`Chain.value`.
     """
     return Chain(value)
 
 
-def tap(value, interceptor):
+def tap(value: T, interceptor: t.Callable[[T], t.Any]) -> T:
     """
     Invokes `interceptor` with the `value` as the first argument and then returns `value`. The
     purpose of this method is to "tap into" a method chain in order to perform operations on
     intermediate results within the chain.
 
     Args:
-        value (mixed): Current value of chain operation.
-        interceptor (callable): Function called on `value`.
+        value: Current value of chain operation.
+        interceptor: Function called on `value`.
 
     Returns:
-        mixed: `value` after `interceptor` call.
+        `value` after `interceptor` call.
 
     Example:
 
         >>> data = []
         >>> def log(value): data.append(value)
         >>> chain([1, 2, 3, 4]).map(lambda x: x * 2).tap(log).value()
         [2, 4, 6, 8]
@@ -291,25 +258,25 @@
 
     .. versionadded:: 1.0.0
     """
     interceptor(value)
     return value
 
 
-def thru(value, interceptor):
+def thru(value: T, interceptor: t.Callable[[T], T2]) -> T2:
     """
     Returns the result of calling `interceptor` on `value`. The purpose of this method is to pass
     `value` through a function during a method chain.
 
     Args:
-        value (mixed): Current value of chain operation.
-        interceptor (callable): Function called with `value`.
+        value: Current value of chain operation.
+        interceptor: Function called with `value`.
 
     Returns:
-        mixed: Results of ``interceptor(value)``.
+        Results of ``interceptor(value)``.
 
     Example:
 
         >>> chain([1, 2, 3, 4]).thru(lambda x: x * 2).value()
         [1, 2, 3, 4, 1, 2, 3, 4]
 
     .. versionadded:: 2.0.0
```

### Comparing `pydash-6.0.2/src/pydash/helpers.py` & `pydash-7.0.0/src/pydash/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from inspect import getfullargspec
 import warnings
 
 import pydash as pyd
 
 
 #: Singleton object that differentiates between an explicit ``None`` value and an unset value.
-UNSET = object()
+#: As a class so it has its own type
+class Unset:
+    ...
+
+
+UNSET = Unset()
 
 #: Tuple of number types.
 NUMBER_TYPES = (int, float, Decimal)
 
 #: Dictionary of builtins with keys as the builtin function and values as the string name.
 BUILTINS = {value: key for key, value in builtins.__dict__.items() if isinstance(value, Hashable)}
 
@@ -118,20 +123,20 @@
 
 
 def base_get(obj, key, default=UNSET):
     """
     Safely get an item by `key` from a sequence or mapping object when `default` provided.
 
     Args:
-        obj (list|dict): Sequence or mapping to retrieve item from.
-        key (mixed): Key or index identifying which item to retrieve.
-        default (mixed, optional): Default value to return if `key` not found in `obj`.
+        obj: Sequence or mapping to retrieve item from.
+        key: Key or index identifying which item to retrieve.
+        default: Default value to return if `key` not found in `obj`.
 
     Returns:
-        mixed: `obj[key]`, `obj.key`, or `default`.
+        `obj[key]`, `obj.key`, or `default`.
 
     Raises:
         KeyError: If `obj` is missing key, index, or attribute and no default value provided.
     """
     if isinstance(obj, dict):
         value = _base_get_dict(obj, key, default=default)
     elif not isinstance(obj, (Mapping, Sequence)) or (
@@ -198,31 +203,31 @@
 
 def base_set(obj, key, value, allow_override=True):
     """
     Set an object's `key` to `value`. If `obj` is a ``list`` and the `key` is the next available
     index position, append to list; otherwise, pad the list of ``None`` and then append to the list.
 
     Args:
-        obj (list|dict): Object to assign value to.
-        key (mixed): Key or index to assign to.
-        value (mixed): Value to assign.
-        allow_override (bool): Whether to allow overriding a previously set key.
+        obj: Object to assign value to.
+        key: Key or index to assign to.
+        value: Value to assign.
+        allow_override: Whether to allow overriding a previously set key.
     """
     if isinstance(obj, dict):
         if allow_override or key not in obj:
             obj[key] = value
     elif isinstance(obj, list):
         key = int(key)
 
         if key < len(obj):
             if allow_override:
                 obj[key] = value
         else:
             if key > len(obj):
-                # Pad list object with None values up to the index key so we can append the value
+                # Pad list object with None values up to the index key, so we can append the value
                 # into the key index.
                 obj[:] = (obj + [None] * key)[:key]
             obj.append(value)
     elif (allow_override or not hasattr(obj, key)) and obj is not None:
         _raise_if_restricted_key(key)
         setattr(obj, key, value)
```

### Comparing `pydash-6.0.2/src/pydash/objects.py` & `pydash-7.0.0/src/pydash/objects.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 .. versionadded:: 1.0.0
 """
 
 import copy
 from functools import partial
 import math
 import re
+import typing as t
 
 import pydash as pyd
 
 from .helpers import UNSET, base_get, base_set, callit, getargcount, iterator, iteriteratee
+from .types import IterateeObjT, PathT
 from .utilities import PathToken, to_path, to_path_tokens
 
 
+if t.TYPE_CHECKING:
+    from _typeshed import SupportsRichComparisonT  # pragma: no cover
+
 __all__ = (
     "assign",
     "assign_with",
     "callables",
     "clone",
     "clone_deep",
     "clone_deep_with",
@@ -58,25 +63,45 @@
     "transform",
     "unset",
     "update",
     "update_with",
     "values",
 )
 
+T = t.TypeVar("T")
+T2 = t.TypeVar("T2")
+T3 = t.TypeVar("T3")
+T4 = t.TypeVar("T4")
+T5 = t.TypeVar("T5")
+
+
+@t.overload
+def assign(
+    obj: t.Mapping[T, T2], *sources: t.Mapping[T3, T4]
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T4]]:
+    ...
+
 
-def assign(obj, *sources):
+@t.overload
+def assign(
+    obj: t.Union[t.Tuple[T, ...], t.List[T]], *sources: t.Mapping[int, T2]
+) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+def assign(obj, *sources) -> t.Union[t.List, t.Dict]:
     """
     Assigns properties of source object(s) to the destination object.
 
     Args:
-        obj (dict): Destination object whose properties will be modified.
-        sources (dict): Source objects to assign to `obj`.
+        obj: Destination object whose properties will be modified.
+        sources: Source objects to assign to `obj`.
 
     Returns:
-        dict: Modified `obj`.
+        Modified `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> obj = {}
@@ -98,48 +123,99 @@
         Shallow copy each `source` instead of deep copying.
 
     .. versionchanged:: 4.0.0
 
         - Moved `iteratee` argument to :func:`assign_with`.
         - Removed alias ``extend``.
     """
-    return assign_with(obj, *sources)
+    return assign_with(obj, *sources)  # type: ignore
+
+
+@t.overload
+def assign_with(
+    obj: t.Mapping[T, T2],
+    *sources: t.Mapping[T3, t.Any],
+    customizer: t.Callable[[t.Union[T2, None]], T5],
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T5]]:
+    ...
+
+
+@t.overload
+def assign_with(
+    obj: t.Mapping[T, T2],
+    *sources: t.Mapping[T3, T4],
+    customizer: t.Callable[[t.Union[T2, None], T4], T5],
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T5]]:
+    ...
+
+
+@t.overload
+def assign_with(
+    obj: t.Mapping[T, T2],
+    *sources: t.Mapping[T3, T4],
+    customizer: t.Callable[[t.Union[T2, None], T4, T3], T5],
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T5]]:
+    ...
+
+
+@t.overload
+def assign_with(
+    obj: t.Mapping[T, T2],
+    *sources: t.Mapping[T3, T4],
+    customizer: t.Callable[[t.Union[T2, None], T4, T3, t.Dict[T, T2]], T5],
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T5]]:
+    ...
+
+
+@t.overload
+def assign_with(
+    obj: t.Mapping[T, T2],
+    *sources: t.Mapping[T3, T4],
+    customizer: t.Callable[[t.Union[T2, None], T4, T3, t.Dict[T, T2], t.Dict[T3, T4]], T5],
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T5]]:
+    ...
+
+
+@t.overload
+def assign_with(
+    obj: t.Mapping[T, T2], *sources: t.Mapping[T3, T4], customizer: None = None
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T4]]:
+    ...
 
 
-def assign_with(obj, *sources, **kwargs):
+def assign_with(obj, *sources, customizer=None):
     """
     This method is like :func:`assign` except that it accepts customizer which is invoked to produce
     the assigned values. If customizer returns ``None``, assignment is handled by the method
     instead. The customizer is invoked with five arguments: ``(obj_value, src_value, key, obj,
     source)``.
 
     Args:
-        obj (dict): Destination object whose properties will be modified.
-        sources (dict): Source objects to assign to `obj`.
+        obj: Destination object whose properties will be modified.
+        sources: Source objects to assign to `obj`.
 
     Keyword Args:
-        customizer (mixed, optional): Customizer applied per iteration.
+        customizer: Customizer applied per iteration.
 
     Returns:
-        dict: Modified `obj`.
+        Modified `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> customizer = lambda o, s: s if o is None else o
-        >>> results = assign({'a': 1}, {'b': 2}, {'a': 3}, customizer)
+        >>> results = assign_with({'a': 1}, {'b': 2}, {'a': 3}, customizer)
         >>> results == {'a': 1, 'b': 2}
         True
 
     .. versionadded:: 4.0.0
     """
     sources = list(sources)
-    customizer = kwargs.get("customizer")
 
     if customizer is None and callable(sources[-1]):
         customizer = sources.pop()
 
     if customizer is not None:
         argcount = getargcount(customizer, maxargs=5)
     else:
@@ -155,23 +231,35 @@
                     value = val
 
             obj[key] = value
 
     return obj
 
 
-def callables(obj):
+@t.overload
+def callables(
+    obj: t.Mapping["SupportsRichComparisonT", t.Any]
+) -> t.List["SupportsRichComparisonT"]:
+    ...
+
+
+@t.overload
+def callables(obj: t.Iterable[T]) -> t.List[T]:
+    ...
+
+
+def callables(obj) -> t.List:
     """
     Creates a sorted list of keys of an object that are callable.
 
     Args:
-        obj (list|dict): Object to inspect.
+        obj: Object to inspect.
 
     Returns:
-        list: All keys whose values are callable.
+        All keys whose values are callable.
 
     Example:
 
         >>> callables({'a': 1, 'b': lambda: 2, 'c': lambda: 3})
         ['b', 'c']
 
     .. versionadded:: 1.0.0
@@ -181,77 +269,125 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``methods``.
     """
     return sorted(key for key, value in iterator(obj) if callable(value))
 
 
-def clone(value):
+def clone(value: T) -> T:
     """
     Creates a clone of `value`.
 
     Args:
-        value (list|dict): Object to clone.
+        value: Object to clone.
 
     Example:
 
         >>> x = {'a': 1, 'b': 2, 'c': {'d': 3}}
         >>> y = clone(x)
         >>> y == y
         True
         >>> x is y
         False
         >>> x['c'] is y['c']
         True
 
     Returns:
-        list|dict: Cloned object.
+        Cloned object.
 
     .. versionadded:: 1.0.0
 
     .. versionchanged:: 4.0.0
         Moved 'iteratee' parameter to :func:`clone_with`.
     """
     return base_clone(value)
 
 
+@t.overload
+def clone_with(
+    value: t.Mapping[T, T2], customizer: t.Callable[[T2, T, t.Mapping[T, T2]], T3]
+) -> t.Dict[T, t.Union[T2, T3]]:
+    ...
+
+
+@t.overload
+def clone_with(
+    value: t.Mapping[T, T2], customizer: t.Callable[[T2, T], T3]
+) -> t.Dict[T, t.Union[T2, T3]]:
+    ...
+
+
+@t.overload
+def clone_with(
+    value: t.Mapping[T, T2], customizer: t.Callable[[T2], T3]
+) -> t.Dict[T, t.Union[T2, T3]]:
+    ...
+
+
+@t.overload
+def clone_with(
+    value: t.List[T], customizer: t.Callable[[T, int, t.List[T]], T2]
+) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def clone_with(value: t.List[T], customizer: t.Callable[[T, int], T2]) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def clone_with(value: t.List[T], customizer: t.Callable[[T], T2]) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def clone_with(value: T, customizer: None = None) -> T:
+    ...
+
+
+@t.overload
+def clone_with(value: t.Any, customizer: t.Callable) -> t.Any:
+    ...
+
+
 def clone_with(value, customizer=None):
     """
     This method is like :func:`clone` except that it accepts customizer which is invoked to produce
     the cloned value. If customizer returns ``None``, cloning is handled by the method instead. The
     customizer is invoked with up to three arguments: ``(value, index|key, object)``.
 
     Args:
-        value (list|dict): Object to clone.
-        customizer (callable, optional): Function to customize cloning.
+        value: Object to clone.
+        customizer: Function to customize cloning.
 
     Returns:
-        list|dict: Cloned object.
+        Cloned object.
 
     Example:
 
         >>> x = {'a': 1, 'b': 2, 'c': {'d': 3}}
         >>> cbk = lambda v, k: v + 2 if isinstance(v, int) and k else None
         >>> y = clone_with(x, cbk)
         >>> y == {'a': 3, 'b': 4, 'c': {'d': 3}}
         True
     """
     return base_clone(value, customizer=customizer)
 
 
-def clone_deep(value):
+def clone_deep(value: T) -> T:
     """
-    Creates a deep clone of `value`. If a iteratee is provided it will be executed to produce the
+    Creates a deep clone of `value`. If an iteratee is provided it will be executed to produce the
     cloned values.
 
     Args:
-        value (list|dict): Object to clone.
+        value: Object to clone.
 
     Returns:
-        list|dict: Cloned object.
+        Cloned object.
 
     Example:
 
         >>> x = {'a': 1, 'b': 2, 'c': {'d': 3}}
         >>> y = clone_deep(x)
         >>> y == y
         True
@@ -264,39 +400,91 @@
 
     .. versionchanged:: 4.0.0
         Moved 'iteratee' parameter to :func:`clone_deep_with`.
     """
     return base_clone(value, is_deep=True)
 
 
+@t.overload
+def clone_deep_with(
+    value: t.Mapping[T, T2], customizer: t.Callable[[T2, T, t.Mapping[T, T2]], T3]
+) -> t.Dict[T, t.Union[T2, T3]]:
+    ...
+
+
+@t.overload
+def clone_deep_with(
+    value: t.Mapping[T, T2], customizer: t.Callable[[T2, T], T3]
+) -> t.Dict[T, t.Union[T2, T3]]:
+    ...
+
+
+@t.overload
+def clone_deep_with(
+    value: t.Mapping[T, T2], customizer: t.Callable[[T2], T3]
+) -> t.Dict[T, t.Union[T2, T3]]:
+    ...
+
+
+@t.overload
+def clone_deep_with(
+    value: t.List[T], customizer: t.Callable[[T, int, t.List[T]], T2]
+) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def clone_deep_with(
+    value: t.List[T], customizer: t.Callable[[T, int], T2]
+) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def clone_deep_with(value: t.List[T], customizer: t.Callable[[T], T2]) -> t.List[t.Union[T, T2]]:
+    ...
+
+
+@t.overload
+def clone_deep_with(value: T, customizer: None = None) -> T:
+    ...
+
+
+@t.overload
+def clone_deep_with(value: t.Any, customizer: t.Callable) -> t.Any:
+    ...
+
+
 def clone_deep_with(value, customizer=None):
     """
     This method is like :func:`clone_with` except that it recursively clones `value`.
 
     Args:
-        value (list|dict): Object to clone.
-        customizer (callable, optional): Function to customize cloning.
+        value: Object to clone.
+        customizer: Function to customize cloning.
 
     Returns:
-        list|dict: Cloned object.
+        Cloned object.
     """
     return base_clone(value, is_deep=True, customizer=customizer)
 
 
-def defaults(obj, *sources):
+def defaults(
+    obj: t.Dict[T, T2], *sources: t.Dict[T3, T4]
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T4]]:
     """
     Assigns properties of source object(s) to the destination object for all destination properties
     that resolve to undefined.
 
     Args:
-        obj (dict): Destination object whose properties will be modified.
-        sources (dict): Source objects to assign to `obj`.
+        obj: Destination object whose properties will be modified.
+        sources: Source objects to assign to `obj`.
 
     Returns:
-        dict: Modified `obj`.
+        Modified `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> obj = {'a': 1}
@@ -306,29 +494,31 @@
         >>> obj == {'a': 1, 'b': 2, 'c': 3}
         True
 
     .. versionadded:: 1.0.0
     """
     for source in sources:
         for key, value in source.items():
-            obj.setdefault(key, value)
+            obj.setdefault(key, value)  # type: ignore
 
-    return obj
+    return obj  # type: ignore
 
 
-def defaults_deep(obj, *sources):
+def defaults_deep(
+    obj: t.Dict[T, T2], *sources: t.Dict[T3, T4]
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T4]]:
     """
     This method is like :func:`defaults` except that it recursively assigns default properties.
 
     Args:
-        obj (dict): Destination object whose properties will be modified.
-        sources (dict): Source objects to assign to `obj`.
+        obj: Destination object whose properties will be modified.
+        sources: Source objects to assign to `obj`.
 
     Returns:
-        dict: Modified `obj`.
+        Modified `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> obj = {'a': {'b': 1}}
@@ -344,25 +534,71 @@
     def setter(obj, key, value):
         if hasattr(obj, "setdefault"):
             obj.setdefault(key, value)
 
     return merge_with(obj, *sources, _setter=setter)
 
 
+@t.overload
+def find_key(
+    obj: t.Mapping[T, T2], predicate: t.Callable[[T2, T, t.Dict[T, T2]], t.Any]
+) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_key(obj: t.Mapping[T, T2], predicate: t.Callable[[T2, T], t.Any]) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_key(obj: t.Mapping[T, T2], predicate: t.Callable[[T2], t.Any]) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_key(obj: t.Mapping[T, t.Any], predicate: None = None) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_key(
+    collection: t.Iterable[T], iteratee: t.Callable[[T, int, t.List[T]], t.Any]
+) -> t.Union[int, None]:
+    ...
+
+
+@t.overload
+def find_key(
+    collection: t.Iterable[T], iteratee: t.Callable[[T, int], t.Any]
+) -> t.Union[int, None]:
+    ...
+
+
+@t.overload
+def find_key(collection: t.Iterable[T], iteratee: t.Callable[[T], t.Any]) -> t.Union[int, None]:
+    ...
+
+
+@t.overload
+def find_key(collection: t.Iterable[t.Any], iteratee: None = None) -> t.Union[int, None]:
+    ...
+
+
 def find_key(obj, predicate=None):
     """
     This method is like :func:`pydash.arrays.find_index` except that it returns the key of the first
     element that passes the predicate check, instead of the element itself.
 
     Args:
-        obj (list|dict): Object to search.
-        predicate (mixed): Predicate applied per iteration.
+        obj: Object to search.
+        predicate: Predicate applied per iteration.
 
     Returns:
-        mixed: Found key or ``None``.
+        Found key or ``None``.
 
     Example:
 
         >>> find_key({'a': 1, 'b': 2, 'c': 3}, lambda x: x == 1)
         'a'
         >>> find_key([1, 2, 3, 4], lambda x: x == 1)
         0
@@ -370,25 +606,73 @@
     .. versionadded:: 1.0.0
     """
     for result, _, key, _ in iteriteratee(obj, predicate):
         if result:
             return key
 
 
+@t.overload
+def find_last_key(
+    obj: t.Mapping[T, T2], predicate: t.Callable[[T2, T, t.Dict[T, T2]], t.Any]
+) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_last_key(obj: t.Mapping[T, T2], predicate: t.Callable[[T2, T], t.Any]) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_last_key(obj: t.Mapping[T, T2], predicate: t.Callable[[T2], t.Any]) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_last_key(obj: t.Mapping[T, t.Any], predicate: None = None) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def find_last_key(
+    collection: t.Iterable[T], iteratee: t.Callable[[T, int, t.List[T]], t.Any]
+) -> t.Union[int, None]:
+    ...
+
+
+@t.overload
+def find_last_key(
+    collection: t.Iterable[T], iteratee: t.Callable[[T, int], t.Any]
+) -> t.Union[int, None]:
+    ...
+
+
+@t.overload
+def find_last_key(
+    collection: t.Iterable[T], iteratee: t.Callable[[T], t.Any]
+) -> t.Union[int, None]:
+    ...
+
+
+@t.overload
+def find_last_key(collection: t.Iterable[t.Any], iteratee: None = None) -> t.Union[int, None]:
+    ...
+
+
 def find_last_key(obj, predicate=None):
     """
     This method is like :func:`find_key` except that it iterates over elements of a collection in
     the opposite order.
 
     Args:
-        obj (list|dict): Object to search.
-        predicate (mixed): Predicate applied per iteration.
+        obj: Object to search.
+        predicate: Predicate applied per iteration.
 
     Returns:
-        mixed: Found key or ``None``.
+        Found key or ``None``.
 
     Example:
 
         >>> find_last_key({'a': 1, 'b': 2, 'c': 3}, lambda x: x == 1)
         'a'
         >>> find_last_key([1, 2, 3, 1], lambda x: x == 1)
         3
@@ -399,25 +683,67 @@
     """
     reversed_obj = reversed(list(iteriteratee(obj, predicate)))
     for result, _, key, _ in reversed_obj:
         if result:
             return key
 
 
+@t.overload
+def for_in(
+    obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T, t.Dict[T, T2]], t.Any]
+) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in(obj: t.Mapping[T, T2], iteratee: None = None) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in(obj: t.Sequence[T], iteratee: t.Callable[[T, int, t.List[T]], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def for_in(obj: t.Sequence[T], iteratee: t.Callable[[T, int], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def for_in(obj: t.Sequence[T], iteratee: t.Callable[[T], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def for_in(obj: t.Sequence[T], iteratee: None = None) -> t.List[T]:
+    ...
+
+
 def for_in(obj, iteratee=None):
     """
     Iterates over own and inherited enumerable properties of `obj`, executing `iteratee` for each
     property.
 
     Args:
-        obj (list|dict): Object to process.
-        iteratee (mixed): Iteratee applied per iteration.
+        obj: Object to process.
+        iteratee: Iteratee applied per iteration.
 
     Returns:
-        list|dict: `obj`.
+        `obj`.
 
     Example:
 
         >>> obj = {}
         >>> def cb(v, k): obj[k] = v
         >>> results = for_in({'a': 1, 'b': 2, 'c': 3}, cb)
         >>> results == {'a': 1, 'b': 2, 'c': 3}
@@ -431,24 +757,66 @@
         Removed alias ``for_own``.
     """
     walk = (None for ret, _, _, _ in iteriteratee(obj, iteratee) if ret is False)
     next(walk, None)
     return obj
 
 
+@t.overload
+def for_in_right(
+    obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T, t.Dict[T, T2]], t.Any]
+) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in_right(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in_right(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in_right(obj: t.Mapping[T, T2], iteratee: None = None) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def for_in_right(obj: t.Sequence[T], iteratee: t.Callable[[T, int, t.List[T]], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def for_in_right(obj: t.Sequence[T], iteratee: t.Callable[[T, int], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def for_in_right(obj: t.Sequence[T], iteratee: t.Callable[[T], t.Any]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def for_in_right(obj: t.Sequence[T], iteratee: None = None) -> t.List[T]:
+    ...
+
+
 def for_in_right(obj, iteratee=None):
     """
     This function is like :func:`for_in` except it iterates over the properties in reverse order.
 
     Args:
-        obj (list|dict): Object to process.
-        iteratee (mixed): Iteratee applied per iteration.
+        obj: Object to process.
+        iteratee: Iteratee applied per iteration.
 
     Returns:
-        list|dict: `obj`.
+        `obj`.
 
     Example:
 
         >>> data = {'product': 1}
         >>> def cb(v): data['product'] *= v
         >>> for_in_right([1, 2, 3, 4], cb)
         [1, 2, 3, 4]
@@ -461,26 +829,41 @@
         Removed alias ``for_own_right``.
     """
     walk = (None for ret, _, _, _ in iteriteratee(obj, iteratee, reverse=True) if ret is False)
     next(walk, None)
     return obj
 
 
-def get(obj, path, default=None):
+@t.overload
+def get(obj: t.List[T], path: int, default: T2) -> t.Union[T, T2]:
+    ...
+
+
+@t.overload
+def get(obj: t.List[T], path: int, default: None = None) -> t.Union[T, None]:
+    ...
+
+
+@t.overload
+def get(obj: t.Any, path: PathT, default: t.Any = None) -> t.Any:
+    ...
+
+
+def get(obj: t.Any, path: PathT, default: t.Any = None) -> t.Any:
     """
     Get the value at any depth of a nested object based on the path described by `path`. If path
     doesn't exist, `default` is returned.
 
     Args:
-        obj (list|dict|Sequence|Mapping): Object to process.
-        path (str|list): List or ``.`` delimited string of path describing path.
-        default (mixed): Default value to return if path doesn't exist. Defaults to ``None``.
+        obj: Object to process.
+        path: List or ``.`` delimited string of path describing path.
+        default: Default value to return if path doesn't exist. Defaults to ``None``.
 
     Returns:
-        mixed: Value of `obj` at path.
+        Value of `obj` at path.
 
     Example:
 
         >>> get({}, 'a.b.c') is None
         True
         >>> get({'a': {'b': {'c': [1, 2, 3, 4]}}}, 'a.b.c[1]')
         2
@@ -516,40 +899,40 @@
         Fixed bug where getattr is used on Mappings and Sequence in Python 3.5+
     """
     if default is UNSET:
         # When NoValue given for default, then this method will raise if path is not present in obj.
         sentinel = default
     else:
         # When a returnable default is given, use a sentinel value to detect when base_get() returns
-        # a default value for a missing path so we can exit early from the loop and not mistakenly
+        # a default value for a missing path, so we can exit early from the loop and not mistakenly
         # iterate over the default.
         sentinel = object()
 
     for key in to_path(path):
         obj = base_get(obj, key, default=sentinel)
 
         if obj is sentinel:
             # Path doesn't exist so set return obj to the default.
             obj = default
             break
 
     return obj
 
 
-def has(obj, path):
+def has(obj: t.Any, path: PathT) -> bool:
     """
     Checks if `path` exists as a key of `obj`.
 
     Args:
-        obj (mixed): Object to test.
-        path (mixed): Path to test for. Can be a list of nested keys or a ``.`` delimited string of
+        obj: Object to test.
+        path: Path to test for. Can be a list of nested keys or a ``.`` delimited string of
             path describing the path.
 
     Returns:
-        bool: Whether `obj` has `path`.
+        Whether `obj` has `path`.
 
     Example:
 
         >>> has([1, 2, 3], 1)
         True
         >>> has({'a': 1, 'b': 2}, 'b')
         True
@@ -578,23 +961,33 @@
         exists = True
     except (KeyError, IndexError, TypeError, ValueError):
         exists = False
 
     return exists
 
 
-def invert(obj):
+@t.overload
+def invert(obj: t.Mapping[T, T2]) -> t.Dict[T2, T]:
+    ...
+
+
+@t.overload
+def invert(obj: t.Iterable[T]) -> t.Dict[T, int]:
+    ...
+
+
+def invert(obj) -> t.Dict:
     """
     Creates an object composed of the inverted keys and values of the given object.
 
     Args:
-        obj (dict): Dict to invert.
+        obj: Dict to invert.
 
     Returns:
-        dict: Inverted dict.
+        Inverted dict.
 
     Example:
 
         >>> results = invert({'a': 1, 'b': 2, 'c': 3})
         >>> results == {1: 'a', 2: 'b', 3: 'c'}
         True
 
@@ -608,27 +1001,47 @@
 
     .. versionchanged:: 4.0.0
         Moved ``multivalue=True`` functionality to :func:`invert_by`.
     """
     return {value: key for key, value in iterator(obj)}
 
 
+@t.overload
+def invert_by(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2], T3]) -> t.Dict[T3, t.List[T]]:
+    ...
+
+
+@t.overload
+def invert_by(obj: t.Mapping[T, T2], iteratee: None = None) -> t.Dict[T2, t.List[T]]:
+    ...
+
+
+@t.overload
+def invert_by(obj: t.Iterable[T], iteratee: t.Callable[[T], T2]) -> t.Dict[T2, t.List[int]]:
+    ...
+
+
+@t.overload
+def invert_by(obj: t.Iterable[T], iteratee: None = None) -> t.Dict[T, t.List[int]]:
+    ...
+
+
 def invert_by(obj, iteratee=None):
     """
     This method is like :func:`invert` except that the inverted object is generated from the results
-    of running each element of object thru iteratee. The corresponding inverted value of each
+    of running each element of object through iteratee. The corresponding inverted value of each
     inverted key is a list of keys responsible for generating the inverted value. The iteratee is
     invoked with one argument: ``(value)``.
 
     Args:
-        obj (dict): Object to invert.
-        iteratee (mixed): Iteratee applied per iteration.
+        obj: Object to invert.
+        iteratee: Iteratee applied per iteration.
 
     Returns:
-        dict: Inverted dict.
+        Inverted dict.
 
     Example:
 
         >>> obj = {'a': 1, 'b': 2, 'c': 1}
         >>> results = invert_by(obj)  # {1: ['a', 'c'], 2: ['b']}
         >>> set(results[1]) == set(['a', 'c'])
         True
@@ -650,26 +1063,26 @@
 
     for key, value in iterator(obj):
         result.setdefault(callback(value), []).append(key)
 
     return result
 
 
-def invoke(obj, path, *args, **kwargs):
+def invoke(obj: t.Any, path: PathT, *args: t.Any, **kwargs: t.Any) -> t.Any:
     """
     Invokes the method at path of object.
 
     Args:
-        obj (dict): The object to query.
-        path (list|str): The path of the method to invoke.
-        args (optional): Arguments to pass to method call.
-        kwargs (optional): Keyword arguments to pass to method call.
+        obj: The object to query.
+        path: The path of the method to invoke.
+        args: Arguments to pass to method call.
+        kwargs: Keyword arguments to pass to method call.
 
     Returns:
-        mixed: Result of the invoked method.
+        Result of the invoked method.
 
     Example:
 
         >>> obj = {'a': [{'b': {'c': [1, 2, 3, 4]}}]}
         >>> invoke(obj, 'a[0].b.c.pop', 1)
         2
         >>> obj
@@ -678,32 +1091,43 @@
     .. versionadded:: 1.0.0
     """
     paths = to_path(path)
     target_path = pyd.initial(paths)
     method_name = pyd.last(paths)
 
     try:
-        method = getattr(get(obj, target_path), method_name)
+        # potential error is caught
+        method = getattr(get(obj, target_path), method_name)  # type: ignore
     except AttributeError:
         ret = None
     else:
         ret = method(*args, **kwargs)
 
     return ret
 
 
+@t.overload
+def keys(obj: t.Iterable[T]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def keys(obj: t.Any) -> t.List:
+    ...
+
+
 def keys(obj):
     """
     Creates a list composed of the keys of `obj`.
 
     Args:
-        obj (mixed): Object to extract keys from.
+        obj: Object to extract keys from.
 
     Returns:
-        list: List of keys.
+        List of keys.
 
     Example:
 
         >>> keys([1, 2, 3])
         [0, 1, 2]
         >>> set(keys({'a': 1, 'b': 2, 'c': 3})) == set(['a', 'b', 'c'])
         True
@@ -715,51 +1139,125 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``keys_in``.
     """
     return [key for key, _ in iterator(obj)]
 
 
+@t.overload
+def map_keys(
+    obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T, t.Dict[T, T2]], T3]
+) -> t.Dict[T3, T2]:
+    ...
+
+
+@t.overload
+def map_keys(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T], T3]) -> t.Dict[T3, T2]:
+    ...
+
+
+@t.overload
+def map_keys(obj: t.Mapping[t.Any, T2], iteratee: t.Callable[[T2], T3]) -> t.Dict[T3, T2]:
+    ...
+
+
+@t.overload
+def map_keys(obj: t.Iterable[T], iteratee: t.Callable[[T, int, t.List[T]], T2]) -> t.Dict[T2, T]:
+    ...
+
+
+@t.overload
+def map_keys(obj: t.Iterable[T], iteratee: t.Callable[[T, int], T2]) -> t.Dict[T2, T]:
+    ...
+
+
+@t.overload
+def map_keys(obj: t.Iterable[T], iteratee: t.Callable[[T], T2]) -> t.Dict[T2, T]:
+    ...
+
+
+@t.overload
+def map_keys(obj: t.Iterable, iteratee: t.Union[IterateeObjT, None] = None) -> t.Dict:
+    ...
+
+
 def map_keys(obj, iteratee=None):
     """
     The opposite of :func:`map_values`, this method creates an object with the same values as object
-    and keys generated by running each own enumerable string keyed property of object thru iteratee.
-    The iteratee is invoked with three arguments: ``(value, key, object)``.
+    and keys generated by running each own enumerable string keyed property of object through
+    iteratee. The iteratee is invoked with three arguments: ``(value, key, object)``.
 
     Args:
-        obj (list|dict): Object to map.
-        iteratee (mixed): Iteratee applied per iteration.
+        obj: Object to map.
+        iteratee: Iteratee applied per iteration.
 
     Returns:
-        list|dict: Results of running `obj` through `iteratee`.
+        Results of running `obj` through `iteratee`.
 
     Example:
 
         >>> callback = lambda value, key: key * 2
         >>> results = map_keys({'a': 1, 'b': 2, 'c': 3}, callback)
         >>> results == {'aa': 1, 'bb': 2, 'cc': 3}
         True
 
     .. versionadded:: 3.3.0
     """
     return {result: value for result, value, _, _ in iteriteratee(obj, iteratee)}
 
 
+@t.overload
+def map_values(
+    obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T, t.Dict[T, T2]], T3]
+) -> t.Dict[T, T3]:
+    ...
+
+
+@t.overload
+def map_values(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T], T3]) -> t.Dict[T, T3]:
+    ...
+
+
+@t.overload
+def map_values(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2], T3]) -> t.Dict[T, T3]:
+    ...
+
+
+@t.overload
+def map_values(obj: t.Iterable[T], iteratee: t.Callable[[T, int, t.List[T]], T2]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def map_values(obj: t.Iterable[T], iteratee: t.Callable[[T, int], T2]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def map_values(obj: t.Iterable[T], iteratee: t.Callable[[T], T2]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def map_values(obj: t.Iterable, iteratee: t.Union[IterateeObjT, None] = None) -> t.Dict:
+    ...
+
+
 def map_values(obj, iteratee=None):
     """
     Creates an object with the same keys as object and values generated by running each string keyed
-    property of object thru iteratee. The iteratee is invoked with three arguments: ``(value, key,
-    object)``.
+    property of object through iteratee. The iteratee is invoked with three arguments: ``(value,
+    key, object)``.
 
     Args:
-        obj (list|dict): Object to map.
-        iteratee (mixed): Iteratee applied per iteration.
+        obj: Object to map.
+        iteratee: Iteratee applied per iteration.
 
     Returns:
-        list|dict: Results of running `obj` through `iteratee`.
+        Results of running `obj` through `iteratee`.
 
     Example:
 
         >>> results = map_values({'a': 1, 'b': 2, 'c': 3}, lambda x: x * 2)
         >>> results == {'a': 2, 'b': 4, 'c': 6}
         True
         >>> results = map_values({'a': 1, 'b': {'d': 4}, 'c': 3}, {'d': 4})
@@ -767,27 +1265,29 @@
         True
 
     .. versionadded:: 1.0.0
     """
     return {key: result for result, _, key, _ in iteriteratee(obj, iteratee)}
 
 
-def map_values_deep(obj, iteratee=None, property_path=UNSET):
+def map_values_deep(
+    obj: t.Iterable, iteratee: t.Union[t.Callable, None] = None, property_path: t.Any = UNSET
+) -> t.Any:
     """
     Map all non-object values in `obj` with return values from `iteratee`. The iteratee is invoked
     with two arguments: ``(obj_value, property_path)`` where ``property_path`` contains the list of
     path keys corresponding to the path of ``obj_value``.
 
     Args:
-        obj (list|dict): Object to map.
-        iteratee (callable): Iteratee applied to each value.
-        property_path (mixed, optional): Path key(s) to access.
+        obj: Object to map.
+        iteratee: Iteratee applied to each value.
+        property_path: Path key(s) to access.
 
     Returns:
-        mixed: The modified object.
+        The modified object.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> x = {'a': 1, 'b': {'c': 2}}
@@ -809,30 +1309,42 @@
     properties = to_path(property_path)
 
     if pyd.is_object(obj):
 
         def deep_iteratee(value, key):
             return map_values_deep(value, iteratee, pyd.flatten([properties, key]))
 
-        return assign(obj, map_values(obj, deep_iteratee))
+        return assign(obj, map_values(obj, deep_iteratee))  # type: ignore
     else:
         return callit(iteratee, obj, properties)
 
 
+@t.overload
+def merge(
+    obj: t.Mapping[T, T2], *sources: t.Mapping[T3, T4]
+) -> t.Dict[t.Union[T, T3], t.Union[T2, T4]]:
+    ...
+
+
+@t.overload
+def merge(obj: t.Sequence[T], *sources: t.Sequence[T2]) -> t.List[t.Union[T, T2]]:
+    ...
+
+
 def merge(obj, *sources):
     """
     Recursively merges properties of the source object(s) into the destination object. Subsequent
     sources will overwrite property assignments of previous sources.
 
     Args:
-        obj (dict): Destination object to merge source(s) into.
-        sources (dict): Source objects to merge from. subsequent sources overwrite previous ones.
+        obj: Destination object to merge source(s) into.
+        sources: Source objects to merge from. subsequent sources overwrite previous ones.
 
     Returns:
-        dict: Merged object.
+        Merged object.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> obj = {'a': 2}
@@ -855,32 +1367,32 @@
 
     .. versionchanged:: 4.9.3
         Fixed regression in v4.8.0 that caused exception when `obj` was ``None``.
     """
     return merge_with(obj, *sources)
 
 
-def merge_with(obj, *sources, **kwargs):
+def merge_with(obj: t.Any, *sources: t.Any, **kwargs: t.Any) -> t.Any:
     """
     This method is like :func:`merge` except that it accepts customizer which is invoked to produce
     the merged values of the destination and source properties. If customizer returns ``None``,
     merging is handled by this method instead. The customizer is invoked with five arguments:
     ``(obj_value, src_value, key, obj, source)``.
 
     Args:
-        obj (dict): Destination object to merge source(s) into.
-        sources (dict): Source objects to merge from. subsequent sources
+        obj: Destination object to merge source(s) into.
+        sources: Source objects to merge from. subsequent sources
             overwrite previous ones.
 
     Keyword Args:
-        iteratee (callable, optional): Iteratee function to handle merging
+        iteratee: Iteratee function to handle merging
             (must be passed in as keyword argument).
 
     Returns:
-        dict: Merged object.
+        Merged object.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> cbk = lambda obj_val, src_val: obj_val + src_val
@@ -894,28 +1406,28 @@
 
     .. versionchanged:: 4.9.3
         Fixed regression in v4.8.0 that caused exception when `obj` was ``None``.
     """
     if obj is None:
         return None
 
-    sources = list(sources)
+    list_sources = list(sources)
     iteratee = kwargs.pop("iteratee", None)
 
-    if iteratee is None and sources and callable(sources[-1]):
-        iteratee = sources.pop()
+    if iteratee is None and list_sources and callable(list_sources[-1]):
+        iteratee = list_sources.pop()
 
-    sources = [copy.deepcopy(source) for source in sources]
+    list_sources = [copy.deepcopy(source) for source in list_sources]
 
     if callable(iteratee):
         iteratee = partial(callit, iteratee, argcount=getargcount(iteratee, maxargs=5))
     else:
         iteratee = None
 
-    return _merge_with(obj, *sources, iteratee=iteratee, **kwargs)
+    return _merge_with(obj, *list_sources, iteratee=iteratee, **kwargs)
 
 
 def _merge_with(obj, *sources, **kwargs):
     iteratee = kwargs.get("iteratee")
     setter = kwargs.get("_setter")
 
     if setter is None:
@@ -939,25 +1451,40 @@
                 result = src_value
 
             setter(obj, key, result)
 
     return obj
 
 
+@t.overload
+def omit(obj: t.Mapping[T, T2], *properties: PathT) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def omit(obj: t.Iterable[T], *properties: PathT) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def omit(obj: t.Any, *properties: PathT) -> t.Dict:
+    ...
+
+
 def omit(obj, *properties):
     """
     The opposite of :func:`pick`. This method creates an object composed of the property paths of
     `obj` that are not omitted.
 
     Args:
-        obj (mixed): Object to process.
-        *properties (str): Property values to omit.
+        obj: Object to process.
+        *properties: Property values to omit.
 
     Returns:
-        dict: Results of omitting properties.
+        Results of omitting properties.
 
     Example:
 
         >>> omit({'a': 1, 'b': 2, 'c': 3}, 'b', 'c') == {'a': 1}
         True
         >>> omit({'a': 1, 'b': 2, 'c': 3 }, ['a', 'c']) == {'b': 2}
         True
@@ -973,26 +1500,61 @@
 
     .. versionchanged:: 4.2.0
         Support deep paths.
     """
     return omit_by(obj, pyd.flatten(properties))
 
 
+@t.overload
+def omit_by(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def omit_by(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def omit_by(obj: t.Dict[T, T2], iteratee: None = None) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def omit_by(obj: t.Iterable[T], iteratee: t.Callable[[T, int], t.Any]) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def omit_by(obj: t.Iterable[T], iteratee: t.Callable[[T], t.Any]) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def omit_by(obj: t.List[T], iteratee: None = None) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def omit_by(obj: t.Any, iteratee: t.Union[t.Callable, None] = None) -> t.Dict:
+    ...
+
+
 def omit_by(obj, iteratee=None):
     """
     The opposite of :func:`pick_by`. This method creates an object composed of the string keyed
     properties of object that predicate doesn't return truthy for. The predicate is invoked with two
     arguments: ``(value, key)``.
 
     Args:
-        obj (mixed): Object to process.
-        iteratee (mixed, optional): Iteratee used to determine which properties to omit.
+        obj: Object to process.
+        iteratee: Iteratee used to determine which properties to omit.
 
     Returns:
-        dict: Results of omitting properties.
+        Results of omitting properties.
 
     Example:
 
         >>> omit_by({'a': 1, 'b': '2', 'c': 3}, lambda v: isinstance(v, int))
         {'b': '2'}
 
     .. versionadded:: 4.0.0
@@ -1021,26 +1583,26 @@
             for key, value in iterator(obj)
             if not callit(iteratee, value, key, argcount=argcount)
         }
 
     return ret
 
 
-def parse_int(value, radix=None):
+def parse_int(value: t.Any, radix: t.Union[int, None] = None) -> t.Union[int, None]:
     """
     Converts the given `value` into an integer of the specified `radix`. If `radix` is falsey, a
     radix of ``10`` is used unless the `value` is a hexadecimal, in which case a radix of 16 is
     used.
 
     Args:
-        value (mixed): Value to parse.
-        radix (int, optional): Base to convert to.
+        value: Value to parse.
+        radix: Base to convert to.
 
     Returns:
-        mixed: Integer if parsable else ``None``.
+        Integer if parsable else ``None``.
 
     Example:
 
         >>> parse_int('5')
         5
         >>> parse_int('12', 8)
         10
@@ -1068,49 +1630,103 @@
         parsed = int(*args)
     except (ValueError, TypeError):
         parsed = None
 
     return parsed
 
 
+@t.overload
+def pick(obj: t.Mapping[T, T2], *properties: PathT) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def pick(obj: t.Union[t.Tuple[T, ...], t.List[T]], *properties: PathT) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def pick(obj: t.Any, *properties: PathT) -> t.Dict:
+    ...
+
+
 def pick(obj, *properties):
     """
     Creates an object composed of the picked object properties.
 
     Args:
-        obj (list|dict): Object to pick from.
-        properties (str): Property values to pick.
+        obj: Object to pick from.
+        properties: Property values to pick.
 
     Returns:
-        dict: Dict containing picked properties.
+        Dict containing picked properties.
 
     Example:
 
         >>> pick({'a': 1, 'b': 2, 'c': 3}, 'a', 'b') == {'a': 1, 'b': 2}
         True
 
     .. versionadded:: 1.0.0
 
     .. versionchanged:: 4.0.0
         Moved iteratee argument to :func:`pick_by`.
     """
     return pick_by(obj, pyd.flatten(properties))
 
 
+@t.overload
+def pick_by(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def pick_by(obj: t.Mapping[T, T2], iteratee: t.Callable[[T2, T], t.Any]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def pick_by(obj: t.Dict[T, T2], iteratee: None = None) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def pick_by(
+    obj: t.Union[t.Tuple[T, ...], t.List[T]], iteratee: t.Callable[[T, int], t.Any]
+) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def pick_by(
+    obj: t.Union[t.Tuple[T, ...], t.List[T]], iteratee: t.Callable[[T], t.Any]
+) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def pick_by(obj: t.Union[t.Tuple[T, ...], t.List[T]], iteratee: None = None) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def pick_by(obj: t.Any, iteratee: t.Union[t.Callable, None] = None) -> t.Dict:
+    ...
+
+
 def pick_by(obj, iteratee=None):
     """
     Creates an object composed of the object properties predicate returns truthy for. The predicate
     is invoked with two arguments: ``(value, key)``.
 
     Args:
-        obj (list|dict): Object to pick from.
-        iteratee (mixed, optional): Iteratee used to determine which properties to pick.
+        obj: Object to pick from.
+        iteratee: Iteratee used to determine which properties to pick.
 
     Returns:
-        dict: Dict containing picked properties.
+        Dict containing picked properties.
 
     Example:
 
         >>> obj = {'a': 1, 'b': '2', 'c': 3 }
         >>> pick_by(obj, lambda v: isinstance(v, int)) == {'a': 1, 'c': 3}
         True
 
@@ -1140,49 +1756,49 @@
 
         if callit(iteratee, value, path, argcount=argcount):
             set_(result, path, value)
 
     return result
 
 
-def rename_keys(obj, key_map):
+def rename_keys(obj: t.Dict[T, T2], key_map: t.Dict[t.Any, T3]) -> t.Dict[t.Union[T, T3], T2]:
     """
     Rename the keys of `obj` using `key_map` and return new object.
 
     Args:
-        obj (dict): Object to rename.
-        key_map (dict): Renaming map whose keys correspond to existing keys in `obj` and whose
+        obj: Object to rename.
+        key_map: Renaming map whose keys correspond to existing keys in `obj` and whose
             values are the new key name.
 
     Returns:
-        dict: Renamed `obj`.
+        Renamed `obj`.
 
     Example:
 
         >>> obj = rename_keys({'a': 1, 'b': 2, 'c': 3}, {'a': 'A', 'b': 'B'})
         >>> obj == {'A': 1, 'B': 2, 'c': 3}
         True
 
     .. versionadded:: 2.0.0
     """
     return {key_map.get(key, key): value for key, value in obj.items()}
 
 
-def set_(obj, path, value):
+def set_(obj: T, path: PathT, value: t.Any) -> T:
     """
     Sets the value of an object described by `path`. If any part of the object path doesn't exist,
     it will be created.
 
     Args:
-        obj (list|dict): Object to modify.
-        path (str | list): Target path to set value to.
-        value (mixed): Value to set.
+        obj: Object to modify.
+        path: Target path to set value to.
+        value: Value to set.
 
     Returns:
-        mixed: Modified `obj`.
+        Modified `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> set_({}, 'a.b.c', 1)
@@ -1205,28 +1821,28 @@
         - Support creating default path values as ``list`` or ``dict`` based on whether key or index
           substrings are used.
         - Remove alias ``deep_set``.
     """
     return set_with(obj, path, value)
 
 
-def set_with(obj, path, value, customizer=None):
+def set_with(obj: T, path: PathT, value: t.Any, customizer: t.Union[t.Callable, None] = None) -> T:
     """
     This method is like :func:`set_` except that it accepts customizer which is invoked to produce
     the objects of path. If customizer returns undefined path creation is handled by the method
     instead. The customizer is invoked with three arguments: ``(nested_value, key, nested_object)``.
 
     Args:
-        obj (list|dict): Object to modify.
-        path (str | list): Target path to set value to.
-        value (mixed): Value to set.
-        customizer (callable, optional): The function to customize assigned values.
+        obj: Object to modify.
+        path: Target path to set value to.
+        value: Value to set.
+        customizer: The function to customize assigned values.
 
     Returns:
-        mixed: Modified `obj`.
+        Modified `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> set_with({}, '[0][1]', 'a', lambda: {})
@@ -1236,32 +1852,36 @@
 
     .. versionchanged:: 4.3.1
         Fixed bug where a callable `value` was called when being set.
     """
     return update_with(obj, path, pyd.constant(value), customizer=customizer)
 
 
-def to_boolean(obj, true_values=("true", "1"), false_values=("false", "0")):
+def to_boolean(
+    obj: t.Any,
+    true_values: t.Tuple[str, ...] = ("true", "1"),
+    false_values: t.Tuple[str, ...] = ("false", "0"),
+) -> t.Union[bool, None]:
     """
-    Convert `obj` to boolean. This is not like the builtin ``bool`` function. By default commonly
+    Convert `obj` to boolean. This is not like the builtin ``bool`` function. By default, commonly
     considered strings values are converted to their boolean equivalent, i.e., ``'0'`` and
     ``'false'`` are converted to ``False`` while ``'1'`` and ``'true'`` are converted to ``True``.
     If a string value is provided that isn't recognized as having a common boolean conversion, then
     the returned value is ``None``. Non-string values of `obj` are converted using ``bool``.
     Optionally, `true_values` and `false_values` can be overridden but each value must be a string.
 
     Args:
-        obj (mixed): Object to convert.
-        true_values (tuple, optional): Values to consider ``True``. Each value must be a string.
+        obj: Object to convert.
+        true_values: Values to consider ``True``. Each value must be a string.
             Comparision is case-insensitive. Defaults to ``('true', '1')``.
-        false_values (tuple, optional): Values to consider ``False``. Each value must be a string.
+        false_values: Values to consider ``False``. Each value must be a string.
             Comparision is case-insensitive. Defaults to ``('false', '0')``.
 
     Returns:
-        bool: Boolean value of `obj`.
+        Boolean value of `obj`.
 
     Example:
 
         >>> to_boolean('true')
         True
         >>> to_boolean('1')
         True
@@ -1290,23 +1910,38 @@
             value = None
     else:
         value = bool(obj)
 
     return value
 
 
+@t.overload
+def to_dict(obj: t.Mapping[T, T2]) -> t.Dict[T, T2]:
+    ...
+
+
+@t.overload
+def to_dict(obj: t.Iterable[T]) -> t.Dict[int, T]:
+    ...
+
+
+@t.overload
+def to_dict(obj: t.Any) -> t.Dict:
+    ...
+
+
 def to_dict(obj):
     """
     Convert `obj` to ``dict`` by creating a new ``dict`` using `obj` keys and values.
 
     Args:
-        obj: (mixed): Object to convert.
+        obj: Object to convert.
 
     Returns:
-        dict: Object converted to ``dict``.
+        Object converted to ``dict``.
 
     Example:
 
         >>> obj = {'a': 1, 'b': 2}
         >>> obj2 = to_dict(obj)
         >>> obj2 == obj
         True
@@ -1321,29 +1956,26 @@
     .. versionchanged:: 4.2.0
         Use ``pydash.helpers.iterator`` to generate key/value pairs.
 
     .. versionchanged:: 4.7.1
         Try to convert to ``dict`` using ``dict()`` first, then fallback to using
         ``pydash.helpers.iterator``.
     """
-    try:
-        return dict(obj)
-    except Exception:
-        return dict(iterator(obj))
+    return dict(iterator(obj))
 
 
-def to_integer(obj):
+def to_integer(obj: t.Any) -> int:
     """
     Converts `obj` to an integer.
 
     Args:
-        obj (str|int|float): Object to convert.
+        obj: Object to convert.
 
     Returns:
-        int: Converted integer or ``0`` if it can't be converted.
+        Converted integer or ``0`` if it can't be converted.
 
     Example:
 
         >>> to_integer(3.2)
         3
         >>> to_integer('3.2')
         3
@@ -1360,25 +1992,40 @@
         num = int(float(obj))
     except (ValueError, TypeError):
         num = 0
 
     return num
 
 
+@t.overload
+def to_list(obj: t.Dict[t.Any, T], split_strings: bool = True) -> t.List[T]:
+    ...
+
+
+@t.overload
+def to_list(obj: t.Iterable[T], split_strings: bool = True) -> t.List[T]:
+    ...
+
+
+@t.overload
+def to_list(obj: T, split_strings: bool = True) -> t.List[T]:
+    ...
+
+
 def to_list(obj, split_strings=True):
     """
-    Converts a obj, an iterable or a single item to a list.
+    Converts an obj, an iterable or a single item to a list.
 
     Args:
-        obj (mixed): Object to convert item or wrap.
-        split_strings (bool, optional): Whether to split strings into single chars. Defaults to
+        obj: Object to convert item or wrap.
+        split_strings: Whether to split strings into single chars. Defaults to
             ``True``.
 
     Returns:
-        list: Converted obj or wrapped item.
+        Converted obj or wrapped item.
 
     Example:
 
         >>> results = to_list({'a': 1, 'b': 2, 'c': 3})
         >>> assert set(results) == set([1, 2, 3])
 
         >>> to_list((1, 2, 3, 4))
@@ -1419,26 +2066,26 @@
     else:
         try:
             return list(obj)
         except TypeError:
             return [obj]
 
 
-def to_number(obj, precision=0):
+def to_number(obj: t.Any, precision: int = 0) -> t.Union[float, None]:
     """
     Convert `obj` to a number. All numbers are retuned as ``float``. If precision is negative, round
     `obj` to the nearest positive integer place. If `obj` can't be converted to a number, ``None``
     is returned.
 
     Args:
-        obj (str|int|float): Object to convert.
-        precision (int, optional): Precision to round number to. Defaults to ``0``.
+        obj: Object to convert.
+        precision: Precision to round number to. Defaults to ``0``.
 
     Returns:
-        float: Converted number or ``None`` if can't be converted.
+        Converted number or ``None`` if it can't be converted.
 
     Example:
 
         >>> to_number('1234.5678')
         1235.0
         >>> to_number('1234.5678', 4)
         1234.5678
@@ -1449,35 +2096,50 @@
     """
     try:
         factor = pow(10, precision)
 
         if precision < 0:
             # Round down since negative `precision` means we are going to the nearest positive
             # integer place.
-            rounder = math.floor
+            rounder: t.Callable = math.floor
         else:
             rounder = round
 
         num = rounder(float(obj) * factor) / factor
     except Exception:
         num = None
 
     return num
 
 
+@t.overload
+def to_pairs(obj: t.Mapping[T, T2]) -> t.List[t.List[t.Union[T, T2]]]:
+    ...
+
+
+@t.overload
+def to_pairs(obj: t.Iterable[T]) -> t.List[t.List[t.Union[int, T]]]:
+    ...
+
+
+@t.overload
+def to_pairs(obj: t.Any) -> t.List:
+    ...
+
+
 def to_pairs(obj):
     """
-    Creates a two dimensional list of an object's key-value pairs, i.e. ``[[key1, value1], [key2,
+    Creates a two-dimensional list of an object's key-value pairs, i.e., ``[[key1, value1], [key2,
     value2]]``.
 
     Args:
-        obj (mixed): Object to process.
+        obj: Object to process.
 
     Returns:
-        list: Two dimensional list of object's key-value pairs.
+        Two dimensional list of object's key-value pairs.
 
     Example:
 
         >>> to_pairs([1, 2, 3, 4])
         [[0, 1], [1, 2], [2, 3], [3, 4]]
         >>> to_pairs({'a': 1})
         [['a', 1]]
@@ -1486,23 +2148,23 @@
 
     .. versionchanged:: 4.0.0
         Renamed from ``pairs`` to ``to_pairs``.
     """
     return [[key, value] for key, value in iterator(obj)]
 
 
-def to_string(obj):
+def to_string(obj: t.Any) -> str:
     """
     Converts an object to string.
 
     Args:
-        obj (mixed): Object to convert.
+        obj: Object to convert.
 
     Returns:
-        str: String representation of `obj`.
+        String representation of `obj`.
 
     Example:
 
         >>> to_string(1) == '1'
         True
         >>> to_string(None) == ''
         True
@@ -1521,29 +2183,84 @@
     elif obj is None:
         res = ""
     else:
         res = str(obj)
     return res
 
 
+@t.overload
+def transform(
+    obj: t.Mapping[T, T2], iteratee: t.Callable[[T3, T2, T, t.Dict[T, T2]], t.Any], accumulator: T3
+) -> T3:
+    ...
+
+
+@t.overload
+def transform(
+    obj: t.Mapping[T, T2], iteratee: t.Callable[[T3, T2, T], t.Any], accumulator: T3
+) -> T3:
+    ...
+
+
+@t.overload
+def transform(
+    obj: t.Mapping[t.Any, T2], iteratee: t.Callable[[T3, T2], t.Any], accumulator: T3
+) -> T3:
+    ...
+
+
+@t.overload
+def transform(
+    obj: t.Mapping[t.Any, t.Any], iteratee: t.Callable[[T3], t.Any], accumulator: T3
+) -> T3:
+    ...
+
+
+@t.overload
+def transform(
+    obj: t.Iterable[T], iteratee: t.Callable[[T3, T, int, t.List[T]], t.Any], accumulator: T3
+) -> T3:
+    ...
+
+
+@t.overload
+def transform(obj: t.Iterable[T], iteratee: t.Callable[[T3, T, int], t.Any], accumulator: T3) -> T3:
+    ...
+
+
+@t.overload
+def transform(obj: t.Iterable[T], iteratee: t.Callable[[T3, T], t.Any], accumulator: T3) -> T3:
+    ...
+
+
+@t.overload
+def transform(obj: t.Iterable[t.Any], iteratee: t.Callable[[T3], t.Any], accumulator: T3) -> T3:
+    ...
+
+
+@t.overload
+def transform(obj: t.Any, iteratee: t.Any = None, accumulator: t.Any = None) -> t.Any:
+    ...
+
+
 def transform(obj, iteratee=None, accumulator=None):
     """
     An alernative to :func:`pydash.collections.reduce`, this method transforms `obj` to a new
-    accumulator object which is the result of running each of its properties through a iteratee,
+    accumulator object which is the result of running each of its properties through an iteratee,
     with each iteratee execution potentially mutating the accumulator object. The iteratee is
     invoked with four arguments: ``(accumulator, value, key, object)``. Iteratees may exit iteration
     early by explicitly returning ``False``.
 
     Args:
-        obj (list|dict): Object to process.
-        iteratee (mixed): Iteratee applied per iteration.
-        accumulator (mixed, optional): Accumulated object. Defaults to ``list``.
+        obj: Object to process.
+        iteratee: Iteratee applied per iteration.
+        accumulator: Accumulated object. Defaults to ``list``.
 
     Returns:
-        mixed: Accumulated object.
+        Accumulated object.
 
     Example:
 
         >>> transform([1, 2, 3, 4], lambda acc, v, k: acc.append((k, v)))
         [(0, 1), (1, 2), (2, 3), (3, 4)]
 
     .. versionadded:: 1.0.0
@@ -1563,27 +2280,54 @@
         if callit(iteratee, accumulator, item, key, obj, argcount=argcount) is False
     )
     next(walk, None)
 
     return accumulator
 
 
+@t.overload
+def update(
+    obj: t.Dict[t.Any, T2],
+    path: PathT,
+    updater: t.Callable[[T2], t.Any],
+) -> t.Dict:
+    ...
+
+
+@t.overload
+def update(
+    obj: t.List[T],
+    path: PathT,
+    updater: t.Callable[[T], t.Any],
+) -> t.List:
+    ...
+
+
+@t.overload
+def update(
+    obj: T,
+    path: PathT,
+    updater: t.Callable,
+) -> T:
+    ...
+
+
 def update(obj, path, updater):
     """
     This method is like :func:`set_` except that accepts updater to produce the value to set. Use
     :func:`update_with` to customize path creation. The updater is invoked with one argument:
     ``(value)``.
 
     Args:
-        obj (list|dict): Object to modify.
-        path (str|list): A string or list of keys that describe the object path to modify.
-        updater (callable): Function that returns updated value.
+        obj: Object to modify.
+        path: A string or list of keys that describe the object path to modify.
+        updater: Function that returns updated value.
 
     Returns:
-        mixed: Updated `obj`.
+        Updated `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> update({}, ['a', 'b'], lambda value: value)
@@ -1592,28 +2336,58 @@
         [[1]]
 
     .. versionadded:: 4.0.0
     """
     return update_with(obj, path, updater)
 
 
+@t.overload
+def update_with(
+    obj: t.Dict[t.Any, T2],
+    path: PathT,
+    updater: t.Callable[[T2], t.Any],
+    customizer: t.Union[t.Callable, None],
+) -> t.Dict:
+    ...
+
+
+@t.overload
+def update_with(
+    obj: t.List[T],
+    path: PathT,
+    updater: t.Callable[[T], t.Any],
+    customizer: t.Union[t.Callable, None] = None,
+) -> t.List:
+    ...
+
+
+@t.overload
+def update_with(
+    obj: T,
+    path: PathT,
+    updater: t.Callable,
+    customizer: t.Union[t.Callable, None] = None,
+) -> T:
+    ...
+
+
 def update_with(obj, path, updater, customizer=None):  # noqa: C901
     """
     This method is like :func:`update` except that it accepts customizer which is invoked to produce
     the objects of path. If customizer returns ``None``, path creation is handled by the method
     instead. The customizer is invoked with three arguments: ``(nested_value, key, nested_object)``.
 
     Args:
-        obj (list|dict): Object to modify.
-        path (str|list): A string or list of keys that describe the object path to modify.
-        updater (callable): Function that returns updated value.
-        customizer (callable, optional): The function to customize assigned values.
+        obj: Object to modify.
+        path: A string or list of keys that describe the object path to modify.
+        updater: Function that returns updated value.
+        customizer: The function to customize assigned values.
 
     Returns:
-        mixed: Updated `obj`.
+        Updated `obj`.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> update_with({}, '[0][1]', lambda: 'a', lambda: {})
@@ -1677,27 +2451,27 @@
 
     value = base_get(target, last_key, default=None)
     base_set(target, last_key, callit(updater, value))
 
     return obj
 
 
-def unset(obj, path):  # noqa: C901
+def unset(obj: t.Union[t.List, t.Dict], path: PathT) -> bool:  # noqa: C901
     """
     Removes the property at `path` of `obj`.
 
     Note:
         Only ``list``, ``dict``, or objects with a ``pop()`` method can be unset by this function.
 
     Args:
-        obj (mixed): The object to modify.
-        path (mixed): The path of the property to unset.
+        obj: The object to modify.
+        path: The path of the property to unset.
 
     Returns:
-        bool: Whether the property was deleted.
+        Whether the property was deleted.
 
     Warning:
         `obj` is modified in place.
 
     Example:
 
         >>> obj = {'a': [{'b': {'c': 7}}]}
@@ -1728,15 +2502,16 @@
 
         try:
             try:
                 target = target[key]
             except TypeError:
                 target = target[int(key)]
         except Exception:
-            target = UNSET
+            # Allow different types reassignment
+            target = UNSET  # type: ignore
 
         if target is UNSET:
             break
 
     did_unset = False
 
     if target is not UNSET:
@@ -1749,23 +2524,38 @@
                 did_unset = True
         except Exception:
             pass
 
     return did_unset
 
 
+@t.overload
+def values(obj: t.Mapping[t.Any, T2]) -> t.List[T2]:
+    ...
+
+
+@t.overload
+def values(obj: t.Iterable[T]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def values(obj: t.Any) -> t.List:
+    ...
+
+
 def values(obj):
     """
     Creates a list composed of the values of `obj`.
 
     Args:
-        obj (mixed): Object to extract values from.
+        obj: Object to extract values from.
 
     Returns:
-        list: List of values.
+        List of values.
 
     Example:
 
         >>> results = values({'a': 1, 'b': 2, 'c': 3})
         >>> set(results) == set([1, 2, 3])
         True
         >>> values([2, 4, 6, 8])
```

### Comparing `pydash-6.0.2/src/pydash/predicates.py` & `pydash-7.0.0/src/pydash/predicates.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,33 @@
 from collections.abc import Iterable, Mapping
 import datetime
 from itertools import islice
 import json
 import operator
 import re
 from types import BuiltinFunctionType
+import typing as t
+
+from typing_extensions import TypeGuard
 
 import pydash as pyd
 
 from .helpers import BUILTINS, NUMBER_TYPES, UNSET, base_get, callit, iterator
 
 
+if t.TYPE_CHECKING:
+    from _typeshed import (  # pragma: no cover
+        SupportsDunderGE,
+        SupportsDunderGT,
+        SupportsDunderLE,
+        SupportsDunderLT,
+        SupportsRichComparison,
+    )
+
+
 __all__ = (
     "eq",
     "gt",
     "gte",
     "lt",
     "lte",
     "in_range",
@@ -60,28 +73,31 @@
     "is_strictly_decreasing",
     "is_strictly_increasing",
     "is_string",
     "is_tuple",
     "is_zero",
 )
 
+T = t.TypeVar("T")
+T2 = t.TypeVar("T2")
+T3 = t.TypeVar("T3")
 
 RegExp = type(re.compile(""))
 
 
-def eq(value, other):
+def eq(value: t.Any, other: t.Any) -> bool:
     """
     Checks if :attr:`value` is equal to :attr:`other`.
 
     Args:
-        value (mixed): Value to compare.
-        other (mixed): Other value to compare.
+        value: Value to compare.
+        other: Other value to compare.
 
     Returns:
-        bool: Whether :attr:`value` is equal to :attr:`other`.
+        Whether :attr:`value` is equal to :attr:`other`.
 
     Example:
 
         >>> eq(None, None)
         True
         >>> eq(None, '')
         False
@@ -91,24 +107,24 @@
         False
 
     .. versionadded:: 4.0.0
     """
     return value is other
 
 
-def gt(value, other):
+def gt(value: "SupportsDunderGT[T]", other: T) -> bool:
     """
     Checks if `value` is greater than `other`.
 
     Args:
-        value (number): Value to compare.
-        other (number): Other value to compare.
+        value: Value to compare.
+        other: Other value to compare.
 
     Returns:
-        bool: Whether `value` is greater than `other`.
+        Whether `value` is greater than `other`.
 
     Example:
 
         >>> gt(5, 3)
         True
         >>> gt(3, 5)
         False
@@ -116,24 +132,24 @@
         False
 
     .. versionadded:: 3.3.0
     """
     return value > other
 
 
-def gte(value, other):
+def gte(value: "SupportsDunderGE[T]", other: T) -> bool:
     """
     Checks if `value` is greater than or equal to `other`.
 
     Args:
-        value (number): Value to compare.
-        other (number): Other value to compare.
+        value: Value to compare.
+        other: Other value to compare.
 
     Returns:
-        bool: Whether `value` is greater than or equal to `other`.
+        Whether `value` is greater than or equal to `other`.
 
     Example:
 
         >>> gte(5, 3)
         True
         >>> gte(3, 5)
         False
@@ -141,24 +157,24 @@
         True
 
     .. versionadded:: 3.3.0
     """
     return value >= other
 
 
-def lt(value, other):
+def lt(value: "SupportsDunderLT[T]", other: T) -> bool:
     """
     Checks if `value` is less than `other`.
 
     Args:
-        value (number): Value to compare.
-        other (number): Other value to compare.
+        value: Value to compare.
+        other: Other value to compare.
 
     Returns:
-        bool: Whether `value` is less than `other`.
+        Whether `value` is less than `other`.
 
     Example:
 
         >>> lt(5, 3)
         False
         >>> lt(3, 5)
         True
@@ -166,24 +182,24 @@
         False
 
     .. versionadded:: 3.3.0
     """
     return value < other
 
 
-def lte(value, other):
+def lte(value: "SupportsDunderLE[T]", other: T) -> bool:
     """
     Checks if `value` is less than or equal to `other`.
 
     Args:
-        value (number): Value to compare.
-        other (number): Other value to compare.
+        value: Value to compare.
+        other: Other value to compare.
 
     Returns:
-        bool: Whether `value` is less than or equal to `other`.
+        Whether `value` is less than or equal to `other`.
 
     Example:
 
         >>> lte(5, 3)
         False
         >>> lte(3, 5)
         True
@@ -191,27 +207,27 @@
         True
 
     .. versionadded:: 3.3.0
     """
     return value <= other
 
 
-def in_range(value, start=0, end=None):
+def in_range(value: t.Any, start: t.Any = 0, end: t.Any = None) -> bool:
     """
     Checks if `value` is between `start` and up to but not including `end`. If `end` is not
     specified it defaults to `start` with `start` becoming ``0``.
 
     Args:
 
-        value (int|float): Number to check.
-        start (int|float, optional): Start of range inclusive. Defaults to ``0``.
-        end (int|float, optional): End of range exclusive. Defaults to `start`.
+        value: Number to check.
+        start: Start of range inclusive. Defaults to ``0``.
+        end: End of range exclusive. Defaults to `start`.
 
     Returns:
-        bool: Whether `value` is in range.
+        Whether `value` is in range.
 
     Example:
 
         >>> in_range(2, 4)
         True
         >>> in_range(4, 2)
         False
@@ -237,23 +253,23 @@
         start = 0
     elif not is_number(end):
         end = 0
 
     return start <= value < end
 
 
-def is_associative(value):
+def is_associative(value: t.Any) -> bool:
     """
     Checks if `value` is an associative object meaning that it can be accessed via an index or key.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is associative.
+        Whether `value` is associative.
 
     Example:
 
         >>> is_associative([])
         True
         >>> is_associative({})
         True
@@ -263,23 +279,23 @@
         False
 
     .. versionadded:: 2.0.0
     """
     return hasattr(value, "__getitem__")
 
 
-def is_blank(text):
+def is_blank(text: t.Any) -> TypeGuard[str]:
     r"""
     Checks if `text` contains only whitespace characters.
 
     Args:
-        text (str): String to test.
+        text: String to test.
 
     Returns:
-        bool: Whether `text` is blank.
+        Whether `text` is blank.
 
     Example:
 
         >>> is_blank('')
         True
         >>> is_blank(' \r\n ')
         True
@@ -292,23 +308,23 @@
         ret = bool(re.match(r"^(\s+)?$", text))
     except TypeError:
         ret = False
 
     return ret
 
 
-def is_boolean(value):
+def is_boolean(value: t.Any) -> TypeGuard[bool]:
     """
     Checks if `value` is a boolean value.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a boolean.
+        Whether `value` is a boolean.
 
     Example:
 
         >>> is_boolean(True)
         True
         >>> is_boolean(False)
         True
@@ -322,23 +338,23 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``is_bool``.
     """
     return isinstance(value, bool)
 
 
-def is_builtin(value):
+def is_builtin(value: t.Any) -> bool:
     """
     Checks if `value` is a Python builtin function or method.
 
     Args:
-        value (callable): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a Python builtin function or method.
+        Whether `value` is a Python builtin function or method.
 
     Example:
 
         >>> is_builtin(1)
         True
         >>> is_builtin(list)
         True
@@ -352,23 +368,23 @@
     """
     try:
         return isinstance(value, BuiltinFunctionType) or value in BUILTINS
     except TypeError:  # pragma: no cover
         return False
 
 
-def is_date(value):
+def is_date(value: t.Any) -> bool:
     """
     Check if `value` is a date object.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a date object.
+        Whether `value` is a date object.
 
     Example:
 
         >>> import datetime
         >>> is_date(datetime.date.today())
         True
         >>> is_date(datetime.datetime.today())
@@ -380,47 +396,49 @@
         This will also return ``True`` for datetime objects.
 
     .. versionadded:: 1.0.0
     """
     return isinstance(value, datetime.date)
 
 
-def is_decreasing(value):
+def is_decreasing(
+    value: t.Union["SupportsRichComparison", t.List["SupportsRichComparison"]]
+) -> bool:
     """
     Check if `value` is monotonically decreasing.
 
     Args:
-        value (list): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is monotonically decreasing.
+        Whether `value` is monotonically decreasing.
 
     Example:
 
         >>> is_decreasing([5, 4, 4, 3])
         True
         >>> is_decreasing([5, 5, 5])
         True
         >>> is_decreasing([5, 4, 5])
         False
 
     .. versionadded:: 2.0.0
     """
-    return is_monotone(value, operator.ge)
+    return is_monotone(value, operator.ge)  # type: ignore
 
 
-def is_dict(value):
+def is_dict(value: t.Any) -> bool:
     """
     Checks if `value` is a ``dict``.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a ``dict``.
+        Whether `value` is a ``dict``.
 
     Example:
 
         >>> is_dict({})
         True
         >>> is_dict([])
         False
@@ -432,23 +450,23 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``is_plain_object``.
     """
     return isinstance(value, dict)
 
 
-def is_empty(value):
+def is_empty(value: t.Any) -> bool:
     """
     Checks if `value` is empty.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is empty.
+        Whether `value` is empty.
 
     Example:
 
         >>> is_empty(0)
         True
         >>> is_empty(1)
         True
@@ -465,24 +483,24 @@
         Returns ``True`` for booleans and numbers.
 
     .. versionadded:: 1.0.0
     """
     return is_boolean(value) or is_number(value) or not value
 
 
-def is_equal(value, other):
+def is_equal(value: t.Any, other: t.Any) -> bool:
     """
     Performs a comparison between two values to determine if they are equivalent to each other.
 
     Args:
-        value (list|dict): Object to compare.
-        other (list|dict): Object to compare.
+        value: Object to compare.
+        other: Object to compare.
 
     Returns:
-        bool: Whether `value` and `other` are equal.
+        Whether `value` and `other` are equal.
 
     Example:
 
         >>> is_equal([1, 2, 3], [1, 2, 3])
         True
         >>> is_equal('a', 'A')
         False
@@ -492,28 +510,43 @@
     .. versionchanged:: 4.0.0
         Removed :attr:`iteratee` from :func:`is_equal` and added it in
         :func:`is_equal_with`.
     """
     return is_equal_with(value, other, customizer=None)
 
 
+@t.overload
+def is_equal_with(value: T, other: T2, customizer: t.Callable[[T, T2], T3]) -> T3:
+    ...
+
+
+@t.overload
+def is_equal_with(value: t.Any, other: t.Any, customizer: t.Callable) -> bool:
+    ...
+
+
+@t.overload
+def is_equal_with(value: t.Any, other: t.Any, customizer: None) -> bool:
+    ...
+
+
 def is_equal_with(value, other, customizer):
     """
     This method is like :func:`is_equal` except that it accepts customizer which is invoked to
     compare values. A customizer is provided which will be executed to compare values. If the
     customizer returns ``None``, comparisons will be handled by the method instead. The customizer
     is invoked with two arguments: ``(value, other)``.
 
     Args:
-        value (list|dict): Object to compare.
-        other (list|dict): Object to compare.
-        customizer (mixed, optional): Customizer used to compare values from `value` and `other`.
+        value: Object to compare.
+        other: Object to compare.
+        customizer: Customizer used to compare values from `value` and `other`.
 
     Returns:
-        bool: Whether `value` and `other` are equal.
+        Whether `value` and `other` are equal.
 
     Example:
 
         >>> is_equal_with([1, 2, 3], [1, 2, 3], None)
         True
         >>> is_equal_with('a', 'A', None)
         False
@@ -547,23 +580,23 @@
     else:
         # Use basic == comparison.
         equal = value == other
 
     return equal
 
 
-def is_error(value):
+def is_error(value: t.Any) -> bool:
     """
     Checks if `value` is an ``Exception``.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is an exception.
+        Whether `value` is an exception.
 
     Example:
 
         >>> is_error(Exception())
         True
         >>> is_error(Exception)
         False
@@ -571,23 +604,23 @@
         False
 
     .. versionadded:: 1.1.0
     """
     return isinstance(value, Exception)
 
 
-def is_even(value):
+def is_even(value: t.Any) -> bool:
     """
     Checks if `value` is even.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is even.
+        Whether `value` is even.
 
     Example:
 
         >>> is_even(2)
         True
         >>> is_even(3)
         False
@@ -595,45 +628,45 @@
         False
 
     .. versionadded:: 2.0.0
     """
     return is_number(value) and value % 2 == 0
 
 
-def is_float(value):
+def is_float(value: t.Any) -> TypeGuard[float]:
     """
     Checks if `value` is a float.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a float.
+        Whether `value` is a float.
 
     Example:
 
         >>> is_float(1.0)
         True
         >>> is_float(1)
         False
 
     .. versionadded:: 2.0.0
     """
     return isinstance(value, float)
 
 
-def is_function(value):
+def is_function(value: t.Any) -> bool:
     """
     Checks if `value` is a function.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is callable.
+        Whether `value` is callable.
 
     Example:
 
         >>> is_function(list)
         True
         >>> is_function(lambda: True)
         True
@@ -641,49 +674,51 @@
         False
 
     .. versionadded:: 1.0.0
     """
     return callable(value)
 
 
-def is_increasing(value):
+def is_increasing(
+    value: t.Union["SupportsRichComparison", t.List["SupportsRichComparison"]]
+) -> bool:
     """
     Check if `value` is monotonically increasing.
 
     Args:
-        value (list): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is monotonically increasing.
+        Whether `value` is monotonically increasing.
 
     Example:
 
         >>> is_increasing([1, 3, 5])
         True
         >>> is_increasing([1, 1, 2, 3, 3])
         True
         >>> is_increasing([5, 5, 5])
         True
         >>> is_increasing([1, 2, 4, 3])
         False
 
     .. versionadded:: 2.0.0
     """
-    return is_monotone(value, operator.le)
+    return is_monotone(value, operator.le)  # type: ignore
 
 
-def is_indexed(value):
+def is_indexed(value: t.Any) -> bool:
     """
     Checks if `value` is integer indexed, i.e., ``list``, ``str`` or ``tuple``.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is integer indexed.
+        Whether `value` is integer indexed.
 
     Example:
 
         >>> is_indexed('')
         True
         >>> is_indexed([])
         True
@@ -696,47 +731,47 @@
 
     .. versionchanged:: 3.0.0
         Return ``True`` for tuples.
     """
     return isinstance(value, (list, tuple, str))
 
 
-def is_instance_of(value, types):
+def is_instance_of(value: t.Any, types: t.Union[type, t.Tuple[type, ...]]) -> bool:
     """
     Checks if `value` is an instance of `types`.
 
     Args:
-        value (mixed): Value to check.
-        types (mixed): Types to check against. Pass as ``tuple`` to check if `value` is one of
+        value: Value to check.
+        types: Types to check against. Pass as ``tuple`` to check if `value` is one of
             multiple types.
 
     Returns:
-        bool: Whether `value` is an instance of `types`.
+        Whether `value` is an instance of `types`.
 
     Example:
 
         >>> is_instance_of({}, dict)
         True
         >>> is_instance_of({}, list)
         False
 
     .. versionadded:: 2.0.0
     """
     return isinstance(value, types)
 
 
-def is_integer(value):
+def is_integer(value: t.Any) -> TypeGuard[int]:
     """
     Checks if `value` is a integer.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is an integer.
+        Whether `value` is an integer.
 
     Example:
 
         >>> is_integer(1)
         True
         >>> is_integer(1.0)
         False
@@ -750,23 +785,23 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``is_int``.
     """
     return is_number(value) and isinstance(value, int)
 
 
-def is_iterable(value):
+def is_iterable(value: t.Any) -> bool:
     """
     Checks if `value` is an iterable.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is an iterable.
+        Whether `value` is an iterable.
 
     Example:
 
         >>> is_iterable([])
         True
         >>> is_iterable({})
         True
@@ -783,23 +818,23 @@
         iter(value)
     except TypeError:
         return False
     else:
         return True
 
 
-def is_json(value):
+def is_json(value: t.Any) -> bool:
     """
     Checks if `value` is a valid JSON string.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is JSON.
+        Whether `value` is JSON.
 
     Example:
 
         >>> is_json({})
         False
         >>> is_json('{}')
         True
@@ -813,23 +848,23 @@
     try:
         json.loads(value)
         return True
     except Exception:
         return False
 
 
-def is_list(value):
+def is_list(value: t.Any) -> bool:
     """
     Checks if `value` is a list.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a list.
+        Whether `value` is a list.
 
     Example:
 
         >>> is_list([])
         True
         >>> is_list({})
         False
@@ -837,25 +872,25 @@
         False
 
     .. versionadded:: 1.0.0
     """
     return isinstance(value, list)
 
 
-def is_match(obj, source):
+def is_match(obj: t.Any, source: t.Any) -> bool:
     """
     Performs a partial deep comparison between `obj` and `source` to determine if `obj` contains
     equivalent property values.
 
     Args:
-        obj (list|dict): Object to compare.
-        source (list|dict): Object of property values to match.
+        obj: Object to compare.
+        source: Object of property values to match.
 
     Returns:
-        bool: Whether `obj` is a match or not.
+        Whether `obj` is a match or not.
 
     Example:
 
         >>> is_match({'a': 1, 'b': 2}, {'b': 2})
         True
         >>> is_match({'a': 1, 'b': 2}, {'b': 3})
         False
@@ -871,28 +906,35 @@
 
     .. versionchanged:: 4.0.0
         Move `iteratee` argument to :func:`is_match_with`.
     """
     return is_match_with(obj, source)
 
 
-def is_match_with(obj, source, customizer=None, _key=UNSET, _obj=UNSET, _source=UNSET):
+def is_match_with(
+    obj: t.Any,
+    source: t.Any,
+    customizer: t.Any = None,
+    _key: t.Any = UNSET,
+    _obj: t.Any = UNSET,
+    _source: t.Any = UNSET,
+) -> bool:
     """
     This method is like :func:`is_match` except that it accepts customizer which is invoked to
     compare values. If customizer returns ``None``, comparisons are handled by the method instead.
     The customizer is invoked with five arguments: ``(obj_value, src_value, index|key, obj,
     source)``.
 
     Args:
-        obj (list|dict): Object to compare.
-        source (list|dict): Object of property values to match.
-        customizer (mixed, optional): Customizer used to compare values from `obj` and `source`.
+        obj: Object to compare.
+        source: Object of property values to match.
+        customizer: Customizer used to compare values from `obj` and `source`.
 
     Returns:
-        bool: Whether `obj` is a match or not.
+        Whether `obj` is a match or not.
 
     Example:
 
         >>> is_greeting = lambda val: val in ('hello', 'hi')
         >>> customizer = lambda ov, sv: is_greeting(ov) and is_greeting(sv)
         >>> obj = {'greeting': 'hello'}
         >>> src = {'greeting': 'hi'}
@@ -908,15 +950,16 @@
         _source = source
 
     if not callable(customizer):
 
         def cbk(obj_value, src_value):
             return obj_value == src_value
 
-        cbk._argcount = 2
+        # no attribute `_argcount`
+        cbk._argcount = 2  # type: ignore
     else:
         cbk = customizer
 
     if isinstance(source, (Mapping, Iterable)) and not isinstance(source, str):
         # Set equal to True if source is empty, otherwise, False and then allow deep comparison to
         # determine equality.
         equal = not source
@@ -933,51 +976,55 @@
                 break
     else:
         equal = callit(cbk, obj, source, _key, _obj, _source)
 
     return equal
 
 
-def is_monotone(value, op):
+def is_monotone(value: t.Union[T, t.List[T]], op: t.Callable[[T, T], t.Any]) -> bool:
     """
     Checks if `value` is monotonic when `operator` used for comparison.
 
     Args:
-        value (list): Value to check.
-        op (callable): Operation to used for comparison.
+        value: Value to check.
+        op: Operation to used for comparison.
 
     Returns:
-        bool: Whether `value` is monotone.
+        Whether `value` is monotone.
 
     Example:
 
         >>> is_monotone([1, 1, 2, 3], operator.le)
         True
         >>> is_monotone([1, 1, 2, 3], operator.lt)
         False
 
     .. versionadded:: 2.0.0
     """
     if not is_list(value):
-        value = [value]
+        l_value = [value]
+    else:
+        l_value = value  # type: ignore
 
-    search = (False for x, y in zip(value, islice(value, 1, None)) if not op(x, y))
+    search = (
+        False for x, y in zip(l_value, islice(l_value, 1, None)) if not op(x, y)  # type: ignore
+    )
 
     return next(search, True)
 
 
-def is_nan(value):
+def is_nan(value: t.Any) -> bool:
     """
     Checks if `value` is not a number.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is not a number.
+        Whether `value` is not a number.
 
     Example:
 
         >>> is_nan('a')
         True
         >>> is_nan(1)
         False
@@ -985,23 +1032,23 @@
         False
 
     .. versionadded:: 1.0.0
     """
     return not is_number(value)
 
 
-def is_negative(value):
+def is_negative(value: t.Any) -> bool:
     """
     Checks if `value` is negative.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is negative.
+        Whether `value` is negative.
 
     Example:
 
         >>> is_negative(-1)
         True
         >>> is_negative(0)
         False
@@ -1009,45 +1056,45 @@
         False
 
     .. versionadded:: 2.0.0
     """
     return is_number(value) and value < 0
 
 
-def is_none(value):
+def is_none(value: t.Any) -> TypeGuard[None]:
     """
     Checks if `value` is `None`.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is ``None``.
+        Whether `value` is ``None``.
 
     Example:
 
         >>> is_none(None)
         True
         >>> is_none(False)
         False
 
     .. versionadded:: 1.0.0
     """
     return value is None
 
 
-def is_number(value):
+def is_number(value: t.Any) -> bool:
     """
     Checks if `value` is a number.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a number.
+        Whether `value` is a number.
 
     Note:
         Returns ``True`` for ``int``, ``long`` (PY2), ``float``, and
         ``decimal.Decimal``.
 
     Example:
 
@@ -1065,23 +1112,23 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``is_num``.
     """
     return not is_boolean(value) and isinstance(value, NUMBER_TYPES)
 
 
-def is_object(value):
+def is_object(value: t.Any) -> bool:
     """
     Checks if `value` is a ``list`` or ``dict``.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is ``list`` or ``dict``.
+        Whether `value` is ``list`` or ``dict``.
 
     Example:
 
         >>> is_object([])
         True
         >>> is_object({})
         True
@@ -1091,23 +1138,23 @@
         False
 
     .. versionadded:: 1.0.0
     """
     return isinstance(value, (list, dict))
 
 
-def is_odd(value):
+def is_odd(value: t.Any) -> bool:
     """
     Checks if `value` is odd.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is odd.
+        Whether `value` is odd.
 
     Example:
 
         >>> is_odd(3)
         True
         >>> is_odd(2)
         False
@@ -1115,23 +1162,23 @@
         False
 
     .. versionadded:: 2.0.0
     """
     return is_number(value) and value % 2 != 0
 
 
-def is_positive(value):
+def is_positive(value: t.Any) -> bool:
     """
     Checks if `value` is positive.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is positive.
+        Whether `value` is positive.
 
     Example:
 
         >>> is_positive(1)
         True
         >>> is_positive(0)
         False
@@ -1139,23 +1186,23 @@
         False
 
     .. versionadded:: 2.0.0
     """
     return is_number(value) and value > 0
 
 
-def is_reg_exp(value):
+def is_reg_exp(value: t.Any) -> TypeGuard[re.Pattern]:
     """
     Checks if `value` is a ``RegExp`` object.
 
     Args:
-        value (mxied): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a RegExp object.
+        Whether `value` is a RegExp object.
 
     Example:
 
         >>> is_reg_exp(re.compile(''))
         True
         >>> is_reg_exp('')
         False
@@ -1164,111 +1211,115 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``is_re``.
     """
     return isinstance(value, RegExp)
 
 
-def is_set(value):
+def is_set(value: t.Any) -> bool:
     """
     Checks if the given value is a set object or not.
 
     Args:
-        value (mixed): Value passed in by the user.
+        value: Value passed in by the user.
 
     Returns:
-        bool: True if the given value is a set else False.
+        True if the given value is a set else False.
 
     Example:
 
         >>> is_set(set([1, 2]))
         True
         >>> is_set([1, 2, 3])
         False
 
     .. versionadded:: 4.0.0
     """
     return isinstance(value, set)
 
 
-def is_strictly_decreasing(value):
+def is_strictly_decreasing(
+    value: t.Union["SupportsRichComparison", t.List["SupportsRichComparison"]]
+) -> bool:
     """
     Check if `value` is strictly decreasing.
 
     Args:
-        value (list): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is strictly decreasing.
+        Whether `value` is strictly decreasing.
 
     Example:
 
         >>> is_strictly_decreasing([4, 3, 2, 1])
         True
         >>> is_strictly_decreasing([4, 4, 2, 1])
         False
 
     .. versionadded:: 2.0.0
     """
-    return is_monotone(value, operator.gt)
+    return is_monotone(value, operator.gt)  # type: ignore
 
 
-def is_strictly_increasing(value):
+def is_strictly_increasing(
+    value: t.Union["SupportsRichComparison", t.List["SupportsRichComparison"]]
+) -> bool:
     """
     Check if `value` is strictly increasing.
 
     Args:
-        value (list): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is strictly increasing.
+        Whether `value` is strictly increasing.
 
     Example:
 
         >>> is_strictly_increasing([1, 2, 3, 4])
         True
         >>> is_strictly_increasing([1, 1, 3, 4])
         False
 
     .. versionadded:: 2.0.0
     """
-    return is_monotone(value, operator.lt)
+    return is_monotone(value, operator.lt)  # type: ignore
 
 
-def is_string(value):
+def is_string(value: t.Any) -> TypeGuard[str]:
     """
     Checks if `value` is a string.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a string.
+        Whether `value` is a string.
 
     Example:
 
         >>> is_string('')
         True
         >>> is_string(1)
         False
 
     .. versionadded:: 1.0.0
     """
     return isinstance(value, str)
 
 
-def is_tuple(value):
+def is_tuple(value: t.Any) -> bool:
     """
     Checks if `value` is a tuple.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is a tuple.
+        Whether `value` is a tuple.
 
     Example:
 
         >>> is_tuple(())
         True
         >>> is_tuple({})
         False
@@ -1276,23 +1327,23 @@
         False
 
     .. versionadded:: 3.0.0
     """
     return isinstance(value, tuple)
 
 
-def is_zero(value):
+def is_zero(value: t.Any) -> TypeGuard[int]:
     """
     Checks if `value` is ``0``.
 
     Args:
-        value (mixed): Value to check.
+        value: Value to check.
 
     Returns:
-        bool: Whether `value` is ``0``.
+        Whether `value` is ``0``.
 
     Example:
 
         >>> is_zero(0)
         True
         >>> is_zero(1)
         False
```

### Comparing `pydash-6.0.2/src/pydash/strings.py` & `pydash-7.0.0/src/pydash/strings.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 .. versionadded:: 1.1.0
 """
 
 import html
 import math
 import re
 import typing
+import typing as t
 import unicodedata
 from urllib.parse import parse_qsl, urlencode, urlsplit, urlunsplit
 
 import pydash as pyd
 
-from .helpers import UNSET
+from .helpers import UNSET, Unset
+from .types import NumberT
 
 
 __all__ = (
     "camel_case",
     "capitalize",
     "chop",
     "chop_right",
@@ -81,44 +83,47 @@
     "unquote",
     "upper_case",
     "upper_first",
     "url",
     "words",
 )
 
+T = t.TypeVar("T")
+T2 = t.TypeVar("T2")
+
 
 class JSRegExp:
     """
     Javascript-style regular expression pattern.
 
     Converts a Javascript-style regular expression to the equivalent Python version.
     """
 
-    def __init__(self, reg_exp):
+    def __init__(self, reg_exp: str) -> None:
         pattern, options = reg_exp[1:].rsplit("/", 1)
 
         self._global = "g" in options
         self._ignore_case = "i" in options
 
         flags = re.I if self._ignore_case else 0
         self.pattern = re.compile(pattern, flags=flags)
 
-    def find(self, text):
+    def find(self, text: str) -> t.List[str]:
         """Return list of regular expression matches."""
         if self._global:
             results = self.pattern.findall(text)
         else:
             res = self.pattern.search(text)
             if res:
                 results = [res.group()]
             else:
                 results = []
         return results
 
-    def replace(self, text, repl):
+    def replace(self, text: str, repl: t.Union[str, t.Callable[[re.Match], str]]) -> str:
         """Replace parts of text that match the regular expression."""
         count = 0 if self._global else 1
         return self.pattern.sub(repl, text, count=count)
 
 
 HTML_ESCAPES = {"&": "&amp;", "<": "&lt;", ">": "&gt;", '"': "&quot;", "'": "&#39;", "`": "&#96;"}
 
@@ -277,23 +282,23 @@
 JS_RE_UNICODE_WORDS = JSRegExp(RS_UNICODE_WORDS)
 JS_RE_LATIN1 = JSRegExp(RS_LATIN1)
 RE_HAS_UNICODE_WORD = re.compile(RS_HAS_UNICODE_WORD)
 RE_APOS = re.compile(RS_APOS)
 RE_HTML_TAGS = re.compile(r"<\/?[^>]+>")
 
 
-def camel_case(text):
+def camel_case(text: t.Any) -> str:
     """
     Converts `text` to camel case.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to camel case.
+        String converted to camel case.
 
     Example:
 
         >>> camel_case('FOO BAR_bAz')
         'fooBarBAz'
 
     .. versionadded:: 1.1.0
@@ -301,24 +306,24 @@
     .. versionchanged:: 5.0.0
         Improved unicode word support.
     """
     text = "".join(word.title() for word in compounder(text))
     return text[:1].lower() + text[1:]
 
 
-def capitalize(text, strict=True):
+def capitalize(text: t.Any, strict: bool = True) -> str:
     """
     Capitalizes the first character of `text`.
 
     Args:
-        text (str): String to capitalize.
-        strict (bool, optional): Whether to cast rest of string to lower case. Defaults to ``True``.
+        text: String to capitalize.
+        strict: Whether to cast rest of string to lower case. Defaults to ``True``.
 
     Returns:
-        str: Capitalized string.
+        Capitalized string.
 
     Example:
 
         >>> capitalize('once upon a TIME')
         'Once upon a time'
         >>> capitalize('once upon a TIME', False)
         'Once upon a TIME'
@@ -328,44 +333,44 @@
     .. versionchanged:: 3.0.0
         Added `strict` option.
     """
     text = pyd.to_string(text)
     return text.capitalize() if strict else text[:1].upper() + text[1:]
 
 
-def chars(text):
+def chars(text: t.Any) -> t.List[str]:
     """
     Split `text` into a list of single characters.
 
     Args:
-        text (str): String to split up.
+        text: String to split up.
 
     Returns:
-        list: List of individual characters.
+        List of individual characters.
 
     Example:
 
         >>> chars('onetwo')
         ['o', 'n', 'e', 't', 'w', 'o']
 
     .. versionadded:: 3.0.0
     """
     return list(pyd.to_string(text))
 
 
-def chop(text, step):
+def chop(text: t.Any, step: int) -> t.List[str]:
     """
     Break up `text` into intervals of length `step`.
 
     Args:
-        text (str): String to chop.
-        step (int): Interval to chop `text`.
+        text: String to chop.
+        step: Interval to chop `text`.
 
     Returns:
-        list: List of chopped characters. If `text` is `None` an empty list is returned.
+        List of chopped characters. If `text` is `None` an empty list is returned.
 
     Example:
 
         >>> chop('abcdefg', 3)
         ['abc', 'def', 'g']
 
     .. versionadded:: 3.0.0
@@ -379,24 +384,24 @@
         chopped = [text]
     else:
         chopped = [text[i : i + step] for i in range(0, len(text), step)]
 
     return chopped
 
 
-def chop_right(text, step):
+def chop_right(text: t.Any, step: int) -> t.List[str]:
     """
     Like :func:`chop` except `text` is chopped from right.
 
     Args:
-        text (str): String to chop.
-        step (int): Interval to chop `text`.
+        text: String to chop.
+        step: Interval to chop `text`.
 
     Returns:
-        list: List of chopped characters.
+        List of chopped characters.
 
     Example:
 
         >>> chop_right('abcdefg', 3)
         ['a', 'bcd', 'efg']
 
     .. versionadded:: 3.0.0
@@ -411,45 +416,45 @@
     else:
         text_len = len(text)
         chopped = [text[-(i + step) : text_len - i] for i in range(0, text_len, step)][::-1]
 
     return chopped
 
 
-def clean(text):
+def clean(text: t.Any) -> str:
     """
     Trim and replace multiple spaces with a single space.
 
     Args:
-        text (str): String to clean.
+        text: String to clean.
 
     Returns:
-        str: Cleaned string.
+        Cleaned string.
 
     Example:
 
         >>> clean('a  b   c    d')
         'a b c d'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return " ".join(pyd.compact(text.split()))
 
 
-def count_substr(text, subtext):
+def count_substr(text: t.Any, subtext: t.Any) -> int:
     """
     Count the occurrences of `subtext` in `text`.
 
     Args:
-        text (str): Source string to count from.
-        subtext (str): String to count.
+        text: Source string to count from.
+        subtext: String to count.
 
     Returns:
-        int: Number of occurrences of `subtext` in `text`.
+        Number of occurrences of `subtext` in `text`.
 
     Example:
 
         >>> count_substr('aabbccddaabbccdd', 'bc')
         2
 
     .. versionadded:: 3.0.0
@@ -459,23 +464,23 @@
 
     text = pyd.to_string(text)
     subtext = pyd.to_string(subtext)
 
     return text.count(subtext)
 
 
-def deburr(text):
+def deburr(text: t.Any) -> str:
     """
     Deburrs `text` by converting latin-1 supplementary letters to basic latin letters.
 
     Args:
-        text (str): String to deburr.
+        text: String to deburr.
 
     Returns:
-        str: Deburred string.
+        Deburred string.
 
     Example:
 
         >>> deburr('déjà vu')
         '...
         >>> 'deja vu'
         'deja vu'
@@ -484,46 +489,46 @@
     """
     text = pyd.to_string(text)
     return JS_RE_LATIN1.replace(
         text, lambda match: DEBURRED_LETTERS.get(match.group(), match.group())
     )
 
 
-def decapitalize(text):
+def decapitalize(text: t.Any) -> str:
     """
     Decaptitalizes the first character of `text`.
 
     Args:
-        text (str): String to decapitalize.
+        text: String to decapitalize.
 
     Returns:
-        str: Decapitalized string.
+        Decapitalized string.
 
     Example:
 
         >>> decapitalize('FOO BAR')
         'fOO BAR'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return text[:1].lower() + text[1:]
 
 
-def ends_with(text, target, position=None):
+def ends_with(text: t.Any, target: t.Any, position: t.Union[int, None] = None) -> bool:
     """
     Checks if `text` ends with a given target string.
 
     Args:
-        text (str): String to check.
-        target (str): String to check for.
-        position (int, optional): Position to search from. Defaults to end of `text`.
+        text: String to check.
+        target: String to check for.
+        position: Position to search from. Defaults to end of `text`.
 
     Returns:
-        bool: Whether `text` ends with `target`.
+        Whether `text` ends with `target`.
 
     Example:
 
         >>> ends_with('abc def', 'def')
         True
         >>> ends_with('abc def', 4)
         False
@@ -535,25 +540,25 @@
 
     if position is None:
         position = len(text)
 
     return text[:position].endswith(target)
 
 
-def ensure_ends_with(text, suffix):
+def ensure_ends_with(text: t.Any, suffix: t.Any) -> str:
     """
     Append a given suffix to a string, but only if the source string does not end with that suffix.
 
     Args:
-        text (str): Source string to append `suffix` to.
-        suffix (str): String to append to the source string if the source string does not end with
+        text: Source string to append `suffix` to.
+        suffix: String to append to the source string if the source string does not end with
             `suffix`.
 
     Returns:
-        str: source string possibly extended by `suffix`.
+        source string possibly extended by `suffix`.
 
     Example:
 
         >>> ensure_ends_with('foo bar', '!')
         'foo bar!'
         >>> ensure_ends_with('foo bar!', '!')
         'foo bar!'
@@ -563,26 +568,26 @@
     text = pyd.to_string(text)
     suffix = pyd.to_string(suffix)
     if text.endswith(suffix):
         return text
     return f"{text}{suffix}"
 
 
-def ensure_starts_with(text, prefix):
+def ensure_starts_with(text: t.Any, prefix: t.Any) -> str:
     """
     Prepend a given prefix to a string, but only if the source string does not start with that
     prefix.
 
     Args:
-        text (str): Source string to prepend `prefix` to.
-        prefix (str): String to prepend to the source string if the source string does not start
+        text: Source string to prepend `prefix` to.
+        prefix: String to prepend to the source string if the source string does not start
             with `prefix`.
 
     Returns:
-        str: source string possibly prefixed by `prefix`
+        source string possibly prefixed by `prefix`
 
     Example:
 
         >>> ensure_starts_with('foo bar', 'Oh my! ')
         'Oh my! foo bar'
         >>> ensure_starts_with('Oh my! foo bar', 'Oh my! ')
         'Oh my! foo bar'
@@ -592,50 +597,50 @@
     text = pyd.to_string(text)
     prefix = pyd.to_string(prefix)
     if text.startswith(prefix):
         return text
     return f"{prefix}{text}"
 
 
-def escape(text):
+def escape(text: t.Any) -> str:
     r"""
     Converts the characters ``&``, ``<``, ``>``, ``"``, ``'``, and ``\``` in `text` to their
     corresponding HTML entities.
 
     Args:
-        text (str): String to escape.
+        text: String to escape.
 
     Returns:
-        str: HTML escaped string.
+        HTML escaped string.
 
     Example:
 
         >>> escape('"1 > 2 && 3 < 4"')
         '&quot;1 &gt; 2 &amp;&amp; 3 &lt; 4&quot;'
 
     .. versionadded:: 1.0.0
 
     .. versionchanged:: 1.1.0
         Moved function to :mod:`pydash.strings`.
     """
     text = pyd.to_string(text)
-    # NOTE: Not using html.escape because Lo-Dash escapes certain chars differently (e.g. "'" isn't
+    # NOTE: Not using html.escape because Lo-Dash escapes certain chars differently (e.g. `'` isn't
     # escaped by html.escape() but is by Lo-Dash).
     return "".join(HTML_ESCAPES.get(char, char) for char in text)
 
 
-def escape_reg_exp(text):
+def escape_reg_exp(text: t.Any) -> str:
     """
     Escapes the RegExp special characters in `text`.
 
     Args:
-        text (str): String to escape.
+        text: String to escape.
 
     Returns:
-        str: RegExp escaped string.
+        RegExp escaped string.
 
     Example:
 
         >>> escape_reg_exp('[()]')
         '\\\\[\\\\(\\\\)\\\\]'
 
     .. versionadded:: 1.1.0
@@ -643,24 +648,24 @@
     .. versionchanged:: 4.0.0
         Removed alias ``escape_re``
     """
     text = pyd.to_string(text)
     return re.escape(text)
 
 
-def has_substr(text, subtext):
+def has_substr(text: t.Any, subtext: t.Any) -> bool:
     """
     Returns whether `subtext` is included in `text`.
 
     Args:
-        text (str): String to search.
-        subtext (str): String to search for.
+        text: String to search.
+        subtext: String to search for.
 
     Returns:
-        bool: Whether `subtext` is found in `text`.
+        Whether `subtext` is found in `text`.
 
     Example:
 
         >>> has_substr('abcdef', 'bc')
         True
         >>> has_substr('abcdef', 'bb')
         False
@@ -668,24 +673,24 @@
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     subtext = pyd.to_string(subtext)
     return text.find(subtext) >= 0
 
 
-def human_case(text):
+def human_case(text: t.Any) -> str:
     """
     Converts `text` to human case which has only the first letter capitalized and each word
     separated by a space.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to human case.
+        String converted to human case.
 
     Example:
 
         >>> human_case('abc-def_hij lmn')
         'Abc def hij lmn'
         >>> human_case('user_id')
         'User'
@@ -701,48 +706,48 @@
         .reg_exp_replace("_id$", "")
         .replace("_", " ")
         .capitalize()
         .value()
     )
 
 
-def insert_substr(text, index, subtext):
+def insert_substr(text: t.Any, index: int, subtext: t.Any) -> str:
     """
     Insert `subtext` in `text` starting at position `index`.
 
     Args:
-        text (str): String to add substring to.
-        index (int): String index to insert into.
-        subtext (str): String to insert.
+        text: String to add substring to.
+        index: String index to insert into.
+        subtext: String to insert.
 
     Returns:
-        str: Modified string.
+        Modified string.
 
     Example:
 
         >>> insert_substr('abcdef', 3, '--')
         'abc--def'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     subtext = pyd.to_string(subtext)
     return text[:index] + subtext + text[index:]
 
 
-def join(array, separator=""):
+def join(array: t.Iterable[t.Any], separator: t.Any = "") -> str:
     """
     Joins an iterable into a string using `separator` between each element.
 
     Args:
-        array (iterable): Iterable to implode.
-        separator (str, optional): Separator to using when joining. Defaults to ``''``.
+        array: Iterable to implode.
+        separator: Separator to using when joining. Defaults to ``''``.
 
     Returns:
-        str: Joined string.
+        Joined string.
 
     Example:
 
         >>> join(['a', 'b', 'c']) == 'abc'
         True
         >>> join([1, 2, 3, 4], '&') == '1&2&3&4'
         True
@@ -753,67 +758,67 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``implode``.
     """
     return pyd.to_string(separator).join(pyd.map_(array or (), pyd.to_string))
 
 
-def kebab_case(text):
+def kebab_case(text: t.Any) -> str:
     """
     Converts `text` to kebab case (a.k.a. spinal case).
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to kebab case.
+        String converted to kebab case.
 
     Example:
 
         >>> kebab_case('a b c_d-e!f')
         'a-b-c-d-e-f'
 
     .. versionadded:: 1.1.0
 
     .. versionchanged:: 5.0.0
         Improved unicode word support.
     """
     return "-".join(word.lower() for word in compounder(text) if word)
 
 
-def lines(text):
+def lines(text: t.Any) -> t.List[str]:
     r"""
     Split lines in `text` into an array.
 
     Args:
-        text (str): String to split.
+        text: String to split.
 
     Returns:
-        list: String split by lines.
+        String split by lines.
 
     Example:
 
         >>> lines('a\nb\r\nc')
         ['a', 'b', 'c']
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return text.splitlines()
 
 
-def lower_case(text):
+def lower_case(text: t.Any) -> str:
     """
     Converts string to lower case as space separated words.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to lower case as space separated words.
+        String converted to lower case as space separated words.
 
     Example:
 
         >>> lower_case('fooBar')
         'foo bar'
         >>> lower_case('--foo-Bar--')
         'foo bar'
@@ -824,23 +829,23 @@
 
     .. versionchanged:: 5.0.0
         Improved unicode word support.
     """
     return " ".join(compounder(text)).lower()
 
 
-def lower_first(text):
+def lower_first(text: str) -> str:
     """
     Converts the first character of string to lower case.
 
     Args:
-        text (str): String passed in by the user.
+        text: String passed in by the user.
 
     Returns:
-        str: String in which the first character is converted to lower case.
+        String in which the first character is converted to lower case.
 
     Example:
 
         >>> lower_first('FRED')
         'fRED'
         >>> lower_first('Foo Bar')
         'foo Bar'
@@ -850,26 +855,28 @@
         ';foobar'
 
     .. versionadded:: 4.0.0
     """
     return text[:1].lower() + text[1:]
 
 
-def number_format(number, scale=0, decimal_separator=".", order_separator=","):
+def number_format(
+    number: NumberT, scale: int = 0, decimal_separator: str = ".", order_separator: str = ","
+) -> str:
     """
     Format a number to scale with custom decimal and order separators.
 
     Args:
-        number (int|float): Number to format.
-        scale (int, optional): Number of decimals to include. Defaults to ``0``.
-        decimal_separator (str, optional): Decimal separator to use. Defaults to ``'.'``.
-        order_separator (str, optional): Order separator to use. Defaults to ``','``.
+        number: Number to format.
+        scale: Number of decimals to include. Defaults to ``0``.
+        decimal_separator: Decimal separator to use. Defaults to ``'.'``.
+        order_separator: Order separator to use. Defaults to ``','``.
 
     Returns:
-        str: Formatted number as string.
+        Number formatted as string.
 
     Example:
 
         >>> number_format(1234.5678)
         '1,235'
         >>> number_format(1234.5678, 2, ',', '.')
         '1.234,57'
@@ -892,27 +899,27 @@
         int_part = order_separator.join(chop(int_part[::-1], 3))[::-1]
 
         text = decimal_separator.join(pyd.compact([int_part, dec_part]))
 
     return text
 
 
-def pad(text, length, chars=" "):
+def pad(text: t.Any, length: int, chars: t.Any = " ") -> str:
     """
     Pads `text` on the left and right sides if it is shorter than the given padding length. The
     `chars` string may be truncated if the number of padding characters can't be evenly divided by
     the padding length.
 
     Args:
-        text (str): String to pad.
-        length (int): Amount to pad.
-        chars (str, optional): Characters to pad with. Defaults to ``" "``.
+        text: String to pad.
+        length: Amount to pad.
+        chars: Characters to pad with. Defaults to ``" "``.
 
     Returns:
-        str: Padded string.
+        Padded string.
 
     Example:
 
         >>> pad('abc', 5)
         ' abc '
         >>> pad('abc', 6, 'x')
         'xabcxx'
@@ -935,27 +942,27 @@
     left_len = int(math.floor(mid))
     right_len = int(math.ceil(mid))
     chars = pad_end("", right_len, chars)
 
     return chars[:left_len] + text + chars
 
 
-def pad_end(text, length, chars=" "):
+def pad_end(text: t.Any, length: int, chars: t.Any = " ") -> str:
     """
     Pads `text` on the right side if it is shorter than the given padding length. The `chars` string
     may be truncated if the number of padding characters can't be evenly divided by the padding
     length.
 
     Args:
-        text (str): String to pad.
-        length (int): Amount to pad.
-        chars (str, optional): Characters to pad with. Defaults to ``" "``.
+        text: String to pad.
+        length: Amount to pad.
+        chars: Characters to pad with. Defaults to ``" "``.
 
     Returns:
-        str: Padded string.
+        Padded string.
 
     Example:
 
         >>> pad_end('abc', 5)
         'abc  '
         >>> pad_end('abc', 5, '.')
         'abc..'
@@ -967,27 +974,27 @@
     """
     # pylint: disable=redefined-outer-name
     text = pyd.to_string(text)
     length = max((length, len(text)))
     return (text + repeat(chars, length))[:length]
 
 
-def pad_start(text, length, chars=" "):
+def pad_start(text: t.Any, length: int, chars: t.Any = " ") -> str:
     """
     Pads `text` on the left side if it is shorter than the given padding length. The `chars` string
     may be truncated if the number of padding characters can't be evenly divided by the padding
     length.
 
     Args:
-        text (str): String to pad.
-        length (int): Amount to pad.
-        chars (str, optional): Characters to pad with. Defaults to ``" "``.
+        text: String to pad.
+        length: Amount to pad.
+        chars: Characters to pad with. Defaults to ``" "``.
 
     Returns:
-        str: Padded string.
+        Padded string.
 
     Example:
 
         >>> pad_start('abc', 5)
         '  abc'
         >>> pad_start('abc', 5, '.')
         '..abc'
@@ -999,24 +1006,24 @@
     """
     # pylint: disable=redefined-outer-name
     text = pyd.to_string(text)
     length = max(length, len(text))
     return (repeat(chars, length) + text)[-length:]
 
 
-def pascal_case(text, strict=True):
+def pascal_case(text: t.Any, strict: bool = True) -> str:
     """
     Like :func:`camel_case` except the first letter is capitalized.
 
     Args:
-        text (str): String to convert.
-        strict (bool, optional): Whether to cast rest of string to lower case. Defaults to ``True``.
+        text: String to convert.
+        strict: Whether to cast rest of string to lower case. Defaults to ``True``.
 
     Returns:
-        str: String converted to class case.
+        String converted to class case.
 
     Example:
 
         >>> pascal_case('FOO BAR_bAz')
         'FooBarBaz'
         >>> pascal_case('FOO BAR_bAz', False)
         'FooBarBAz'
@@ -1030,23 +1037,23 @@
 
     if strict:
         text = text.lower()
 
     return capitalize(camel_case(text), strict=False)
 
 
-def predecessor(char):
+def predecessor(char: t.Any) -> str:
     """
     Return the predecessor character of `char`.
 
     Args:
-        char (str): Character to find the predecessor of.
+        char: Character to find the predecessor of.
 
     Returns:
-        str: Predecessor character.
+        Predecessor character.
 
     Example:
 
         >>> predecessor('c')
         'b'
         >>> predecessor('C')
         'B'
@@ -1055,28 +1062,28 @@
 
     .. versionadded:: 3.0.0
     """
     char = pyd.to_string(char)
     return chr(ord(char) - 1)
 
 
-def prune(text, length=0, omission="..."):
+def prune(text: t.Any, length: int = 0, omission: str = "...") -> str:
     """
     Like :func:`truncate` except it ensures that the pruned string doesn't exceed the original
     length, i.e., it avoids half-chopped words when truncating. If the pruned text + `omission` text
     is longer than the original text, then the original text is returned.
 
     Args:
-        text (str): String to prune.
-        length (int, optional): Target prune length. Defaults to ``0``.
-        omission (str, optional): Omission text to append to the end of the pruned string. Defaults
+        text: String to prune.
+        length: Target prune length. Defaults to ``0``.
+        omission: Omission text to append to the end of the pruned string. Defaults
             to ``'...'``.
 
     Returns:
-        str: Pruned string.
+        Pruned string.
 
     Example:
 
         >>> prune('Fe fi fo fum', 5)
         'Fe fi...'
         >>> prune('Fe fi fo fum', 6)
         'Fe fi...'
@@ -1108,55 +1115,55 @@
     else:
         # Last character (at least) is whitespace. So remove that character as well as any other
         # whitespace.
         subtext = subtext[:-1].rstrip()
 
     subtext_len = len(subtext)
 
-    # Only add omission text if doing so will result in a string that is equal two or smaller in
-    # length than the original.
+    # Only add omission text if doing so will result in a string that is equal to or smaller than
+    # the original.
     if (subtext_len + omission_len) <= text_len:
         text = text[:subtext_len] + omission
 
     return text
 
 
-def quote(text, quote_char='"'):
+def quote(text: t.Any, quote_char: t.Any = '"') -> str:
     """
     Quote a string with another string.
 
     Args:
-        text (str): String to be quoted.
-        quote_char (str, optional): the quote character. Defaults to ``"``.
+        text: String to be quoted.
+        quote_char: the quote character. Defaults to ``'"'``.
 
     Returns:
-        str: the quoted string.
+        the quoted string.
 
     Example:
 
         >>> quote('To be or not to be')
         '"To be or not to be"'
         >>> quote('To be or not to be', "'")
         "'To be or not to be'"
 
     .. versionadded:: 2.4.0
     """
     return surround(text, quote_char)
 
 
-def reg_exp_js_match(text, reg_exp):
+def reg_exp_js_match(text: t.Any, reg_exp: str) -> t.List[str]:
     """
     Return list of matches using Javascript style regular expression.
 
     Args:
-        text (str): String to evaluate.
-        reg_exp (str): Javascript style regular expression.
+        text: String to evaluate.
+        reg_exp: Javascript style regular expression.
 
     Returns:
-        list: List of matches.
+        List of matches.
 
     Example:
 
         >>> reg_exp_js_match('aaBBcc', '/bb/')
         []
         >>> reg_exp_js_match('aaBBcc', '/bb/i')
         ['BB']
@@ -1173,25 +1180,27 @@
     .. versionchanged:: 4.0.0
         Renamed from ``js_match`` to ``reg_exp_js_match``.
     """
     text = pyd.to_string(text)
     return JSRegExp(reg_exp).find(text)
 
 
-def reg_exp_js_replace(text, reg_exp, repl):
+def reg_exp_js_replace(
+    text: t.Any, reg_exp: str, repl: t.Union[str, t.Callable[[re.Match], str]]
+) -> str:
     """
     Replace `text` with `repl` using Javascript style regular expression to find matches.
 
     Args:
-        text (str): String to evaluate.
-        reg_exp (str): Javascript style regular expression.
-        repl (str|callable): Replacement string or callable.
+        text: String to evaluate.
+        reg_exp: Javascript style regular expression.
+        repl: Replacement string or callable.
 
     Returns:
-        str: Modified string.
+        Modified string.
 
     Example:
 
         >>> reg_exp_js_replace('aaBBcc', '/bb/', 'X')
         'aaBBcc'
         >>> reg_exp_js_replace('aaBBcc', '/bb/i', 'X')
         'aaXcc'
@@ -1210,29 +1219,35 @@
     """
     text = pyd.to_string(text)
     if not pyd.is_function(repl):
         repl = pyd.to_string(repl)
     return JSRegExp(reg_exp).replace(text, repl)
 
 
-def reg_exp_replace(text, pattern, repl, ignore_case=False, count=0):
+def reg_exp_replace(
+    text: t.Any,
+    pattern: t.Any,
+    repl: t.Union[str, t.Callable[[re.Match], str]],
+    ignore_case: bool = False,
+    count: int = 0,
+) -> str:
     """
     Replace occurrences of regex `pattern` with `repl` in `text`. Optionally, ignore case when
     replacing. Optionally, set `count` to limit number of replacements.
 
     Args:
-        text (str): String to replace.
-        pattern (str|typing.Pattern): Pattern to find and replace.
-        repl (str): String to substitute `pattern` with.
-        ignore_case (bool, optional): Whether to ignore case when replacing. Defaults to ``False``.
-        count (int, optional): Maximum number of occurrences to replace. Defaults to ``0`` which
+        text: String to replace.
+        pattern: Pattern to find and replace.
+        repl: String to substitute `pattern` with.
+        ignore_case: Whether to ignore case when replacing. Defaults to ``False``.
+        count: Maximum number of occurrences to replace. Defaults to ``0`` which
             replaces all.
 
     Returns:
-        str: Replaced string.
+        Replaced string.
 
     Example:
 
         >>> reg_exp_replace('aabbcc', 'b', 'X')
         'aaXXcc'
         >>> reg_exp_replace('aabbcc', 'B', 'X', ignore_case=True)
         'aaXXcc'
@@ -1248,57 +1263,64 @@
     """
     if pattern is None:
         return pyd.to_string(text)
 
     return replace(text, pattern, repl, ignore_case=ignore_case, count=count, escape=False)
 
 
-def repeat(text, n=0):
+def repeat(text: t.Any, n: t.SupportsInt = 0) -> str:
     """
     Repeats the given string `n` times.
 
     Args:
-        text (str): String to repeat.
-        n (int, optional): Number of times to repeat the string.
+        text: String to repeat.
+        n: Number of times to repeat the string.
 
     Returns:
-        str: Repeated string.
+        Repeated string.
 
     Example:
 
         >>> repeat('.', 5)
         '.....'
 
     .. versionadded:: 1.1.0
     """
     return pyd.to_string(text) * int(n)
 
 
 def replace(
-    text, pattern, repl, ignore_case=False, count=0, escape=True, from_start=False, from_end=False
-):
+    text: t.Any,
+    pattern: t.Any,
+    repl: t.Union[str, t.Callable[[re.Match], str]],
+    ignore_case: bool = False,
+    count: int = 0,
+    escape: bool = True,
+    from_start: bool = False,
+    from_end: bool = False,
+) -> str:
     """
     Replace occurrences of `pattern` with `repl` in `text`. Optionally, ignore case when replacing.
     Optionally, set `count` to limit number of replacements.
 
     Args:
-        text (str): String to replace.
-        pattern (str|typing.Pattern): Pattern to find and replace.
-        repl (str): String to substitute `pattern` with.
-        ignore_case (bool, optional): Whether to ignore case when replacing. Defaults to ``False``.
-        count (int, optional): Maximum number of occurrences to replace. Defaults to ``0`` which
+        text: String to replace.
+        pattern: Pattern to find and replace.
+        repl: String to substitute `pattern` with.
+        ignore_case: Whether to ignore case when replacing. Defaults to ``False``.
+        count: Maximum number of occurrences to replace. Defaults to ``0`` which
             replaces all.
-        escape (bool, optional): Whether to escape `pattern` when searching. This is needed if a
+        escape: Whether to escape `pattern` when searching. This is needed if a
             literal replacement is desired when `pattern` may contain special regular expression
             characters. Defaults to ``True``.
-        from_start (bool, optional): Whether to limit replacement to start of string.
-        from_end (bool, optional): Whether to limit replacement to end of string.
+        from_start: Whether to limit replacement to start of string.
+        from_end: Whether to limit replacement to end of string.
 
     Returns:
-        str: Replaced string.
+        Replaced string.
 
     Example:
 
         >>> replace('aabbcc', 'b', 'X')
         'aaXXcc'
         >>> replace('aabbcc', 'B', 'X', ignore_case=True)
         'aaXXcc'
@@ -1342,109 +1364,126 @@
             pattern += "$"
 
         pat = re.compile(pattern, flags=flags)
 
     return pat.sub(repl, text, count=count)
 
 
-def replace_end(text, pattern, repl, ignore_case=False, escape=True):
+def replace_end(
+    text: t.Any,
+    pattern: t.Any,
+    repl: t.Union[str, t.Callable[[re.Match], str]],
+    ignore_case: bool = False,
+    escape: bool = True,
+) -> str:
     """
     Like :func:`replace` except it only replaces `text` with `repl` if `pattern` mathces the end of
     `text`.
 
     Args:
-        text (str): String to replace.
-        pattern (str|typing.Pattern): Pattern to find and replace.
-        repl (str): String to substitute `pattern` with.
-        ignore_case (bool, optional): Whether to ignore case when replacing. Defaults to ``False``.
-        escape (bool, optional): Whether to escape `pattern` when searching. This is needed if a
+        text: String to replace.
+        pattern: Pattern to find and replace.
+        repl: String to substitute `pattern` with.
+        ignore_case: Whether to ignore case when replacing. Defaults to ``False``.
+        escape: Whether to escape `pattern` when searching. This is needed if a
             literal replacement is desired when `pattern` may contain special regular expression
             characters. Defaults to ``True``.
 
     Returns:
-        str: Replaced string.
+        Replaced string.
 
     Example:
 
         >>> replace_end('aabbcc', 'b', 'X')
         'aabbcc'
         >>> replace_end('aabbcc', 'c', 'X')
         'aabbcX'
 
     .. versionadded:: 4.1.0
     """
     return replace(text, pattern, repl, ignore_case=ignore_case, escape=escape, from_end=True)
 
 
-def replace_start(text, pattern, repl, ignore_case=False, escape=True):
+def replace_start(
+    text: t.Any,
+    pattern: t.Any,
+    repl: t.Union[str, t.Callable[[re.Match], str]],
+    ignore_case: bool = False,
+    escape: bool = True,
+) -> str:
     """
     Like :func:`replace` except it only replaces `text` with `repl` if `pattern` mathces the start
     of `text`.
 
     Args:
-        text (str): String to replace.
-        pattern (str|typing.Pattern): Pattern to find and replace.
-        repl (str): String to substitute `pattern` with.
-        ignore_case (bool, optional): Whether to ignore case when replacing. Defaults to ``False``.
-        escape (bool, optional): Whether to escape `pattern` when searching. This is needed if a
+        text: String to replace.
+        pattern: Pattern to find and replace.
+        repl: String to substitute `pattern` with.
+        ignore_case: Whether to ignore case when replacing. Defaults to ``False``.
+        escape: Whether to escape `pattern` when searching. This is needed if a
             literal replacement is desired when `pattern` may contain special regular expression
             characters. Defaults to ``True``.
 
     Returns:
-        str: Replaced string.
+        Replaced string.
 
     Example:
 
         >>> replace_start('aabbcc', 'b', 'X')
         'aabbcc'
         >>> replace_start('aabbcc', 'a', 'X')
         'Xabbcc'
 
     .. versionadded:: 4.1.0
     """
     return replace(text, pattern, repl, ignore_case=ignore_case, escape=escape, from_start=True)
 
 
-def separator_case(text, separator):
+def separator_case(text: t.Any, separator: str) -> str:
     """
     Splits `text` on words and joins with `separator`.
 
     Args:
-        text (str): String to convert.
-        separator (str): Separator to join words with.
+        text: String to convert.
+        separator: Separator to join words with.
 
     Returns:
-        str: Converted string.
+        Converted string.
 
     Example:
 
         >>> separator_case('a!!b___c.d', '-')
         'a-b-c-d'
 
     .. versionadded:: 3.0.0
 
     .. versionchanged:: 5.0.0
         Improved unicode word support.
     """
     return separator.join(word.lower() for word in words(text) if word)
 
 
-def series_phrase(items, separator=", ", last_separator=" and ", serial=False):
+def series_phrase(
+    items: t.List[t.Any],
+    separator: t.Any = ", ",
+    last_separator: t.Any = " and ",
+    serial: bool = False,
+) -> str:
     """
     Join items into a grammatical series phrase, e.g., ``"item1, item2, item3 and item4"``.
 
     Args:
-        items (list): List of string items to join.
-        separator (str, optional): Item separator. Defaults to ``', '``.
-        last_separator (str, optional): Last item separator. Defaults to ``' and '``.
-        serial (bool, optional): Whether to include `separator` with `last_separator` when number of
+        items: List of string items to join.
+        separator: Item separator. Defaults to ``', '``.
+        last_separator: Last item separator. Defaults to ``' and '``.
+        serial: Whether to include `separator` with `last_separator` when number of
             items is greater than 2. Defaults to ``False``.
 
     Returns:
-        str: Joined string.
+        Joined string.
 
     Example:
 
         >>> series_phrase(['apples', 'bananas', 'peaches'])
         'apples, bananas and peaches'
         >>> series_phrase(['apples', 'bananas', 'peaches'], serial=True)
         'apples, bananas, and peaches'
@@ -1465,80 +1504,88 @@
 
     if item_count >= 2:
         items = items[:-2] + [last_separator.join(items[-2:])]
 
     return separator.join(items)
 
 
-def series_phrase_serial(items, separator=", ", last_separator=" and "):
+def series_phrase_serial(
+    items: t.List[t.Any], separator: t.Any = ", ", last_separator: t.Any = " and "
+) -> str:
     """
     Join items into a grammatical series phrase using a serial separator, e.g., ``"item1, item2,
     item3, and item4"``.
 
     Args:
-        items (list): List of string items to join.
-        separator (str, optional): Item separator. Defaults to ``', '``.
-        last_separator (str, optional): Last item separator. Defaults to ``' and '``.
+        items: List of string items to join.
+        separator: Item separator. Defaults to ``', '``.
+        last_separator: Last item separator. Defaults to ``' and '``.
 
     Returns:
-        str: Joined string.
+        Joined string.
 
     Example:
 
         >>> series_phrase_serial(['apples', 'bananas', 'peaches'])
         'apples, bananas, and peaches'
 
     .. versionadded:: 3.0.0
     """
     return series_phrase(items, separator, last_separator, serial=True)
 
 
-def slugify(text, separator="-"):
+def slugify(text: t.Any, separator: str = "-") -> str:
     """
     Convert `text` into an ASCII slug which can be used safely in URLs. Incoming `text` is converted
     to unicode and noramlzied using the ``NFKD`` form. This results in some accented characters
     being converted to their ASCII "equivalent" (e.g. ``é`` is converted to ``e``). Leading and
     trailing whitespace is trimmed and any remaining whitespace or other special characters without
     an ASCII equivalent are replaced with ``-``.
 
     Args:
-        text (str): String to slugify.
-        separator (str, optional): Separator to use. Defaults to ``'-'``.
+        text: String to slugify.
+        separator: Separator to use. Defaults to ``'-'``.
 
     Returns:
-        str: Slugified string.
+        Slugified string.
 
     Example:
 
         >>> slugify('This is a slug.') == 'this-is-a-slug'
         True
         >>> slugify('This is a slug.', '+') == 'this+is+a+slug'
         True
 
     .. versionadded:: 3.0.0
 
     .. versionchanged:: 5.0.0
         Improved unicode word support.
+
+    .. versionchanged:: 7.0.0
+        Remove single quotes from output.
     """
     normalized = (
-        unicodedata.normalize("NFKD", pyd.to_string(text)).encode("ascii", "ignore").decode("utf8")
+        unicodedata.normalize("NFKD", pyd.to_string(text))
+        .encode("ascii", "ignore")
+        .decode("utf8")
+        .replace("'", "")
     )
 
     return separator_case(normalized, separator)
 
 
-def snake_case(text):
+def snake_case(text: t.Any) -> str:
     """
     Converts `text` to snake case.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to snake case.
+        String converted to snake case.
 
     Example:
 
         >>> snake_case('This is Snake Case!')
         'this_is_snake_case'
 
     .. versionadded:: 1.1.0
@@ -1548,25 +1595,25 @@
 
     .. versionchanged:: 5.0.0
         Improved unicode word support.
     """
     return "_".join(word.lower() for word in compounder(text) if word)
 
 
-def split(text, separator=UNSET):
+def split(text: t.Any, separator: t.Union[str, Unset, None] = UNSET) -> t.List[str]:
     """
     Splits `text` on `separator`. If `separator` not provided, then `text` is split on whitespace.
     If `separator` is falsey, then `text` is split on every character.
 
     Args:
-        text (str): String to explode.
-        separator (str, optional): Separator string to split on. Defaults to ``NoValue``.
+        text: String to explode.
+        separator: Separator string to split on. Defaults to ``NoValue``.
 
     Returns:
-        list: Split string.
+        Split string.
 
     Example:
 
         >>> split('one potato, two potatoes, three potatoes, four!')
         ['one', 'potato,', 'two', 'potatoes,', 'three', 'potatoes,', 'four!']
         >>> split('one potato, two potatoes, three potatoes, four!', ',')
         ['one potato', ' two potatoes', ' three potatoes', ' four!']
@@ -1587,48 +1634,48 @@
         ret = text.split(separator)
     else:
         ret = chars(text)
 
     return ret
 
 
-def start_case(text):
+def start_case(text: t.Any) -> str:
     """
     Convert `text` to start case.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to start case.
+        String converted to start case.
 
     Example:
 
         >>> start_case("fooBar")
         'Foo Bar'
 
     .. versionadded:: 3.1.0
 
     .. versionchanged:: 5.0.0
         Improved unicode word support.
     """
     return " ".join(capitalize(word, strict=False) for word in compounder(text))
 
 
-def starts_with(text, target, position=0):
+def starts_with(text: t.Any, target: t.Any, position: int = 0) -> bool:
     """
     Checks if `text` starts with a given target string.
 
     Args:
-        text (str): String to check.
-        target (str): String to check for.
-        position (int, optional): Position to search from. Defaults to beginning of `text`.
+        text: String to check.
+        target: String to check for.
+        position: Position to search from. Defaults to beginning of `text`.
 
     Returns:
-        bool: Whether `text` starts with `target`.
+        Whether `text` starts with `target`.
 
     Example:
 
         >>> starts_with('abcdef', 'a')
         True
         >>> starts_with('abcdef', 'b')
         False
@@ -1638,135 +1685,135 @@
     .. versionadded:: 1.1.0
     """
     text = pyd.to_string(text)
     target = pyd.to_string(target)
     return text[position:].startswith(target)
 
 
-def strip_tags(text):
+def strip_tags(text: t.Any) -> str:
     """
     Removes all HTML tags from `text`.
 
     Args:
-        text (str): String to strip.
+        text: String to strip.
 
     Returns:
-        str: String without HTML tags.
+        String without HTML tags.
 
     Example:
 
         >>> strip_tags('<a href="#">Some link</a>')
         'Some link'
 
     .. versionadded:: 3.0.0
     """
     return RE_HTML_TAGS.sub("", pyd.to_string(text))
 
 
-def substr_left(text, subtext):
+def substr_left(text: t.Any, subtext: str) -> str:
     """
     Searches `text` from left-to-right for `subtext` and returns a substring consisting of the
     characters in `text` that are to the left of `subtext` or all string if no match found.
 
     Args:
-        text (str): String to partition.
-        subtext (str): String to search for.
+        text: String to partition.
+        subtext: String to search for.
 
     Returns:
-        str: Substring to left of `subtext`.
+        Substring to left of `subtext`.
 
     Example:
 
         >>> substr_left('abcdefcdg', 'cd')
         'ab'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return text.partition(subtext)[0] if subtext else text
 
 
-def substr_left_end(text, subtext):
+def substr_left_end(text: t.Any, subtext: str) -> str:
     """
     Searches `text` from right-to-left for `subtext` and returns a substring consisting of the
     characters in `text` that are to the left of `subtext` or all string if no match found.
 
     Args:
-        text (str): String to partition.
-        subtext (str): String to search for.
+        text: String to partition.
+        subtext: String to search for.
 
     Returns:
-        str: Substring to left of `subtext`.
+        Substring to left of `subtext`.
 
     Example:
 
         >>> substr_left_end('abcdefcdg', 'cd')
         'abcdef'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return text.rpartition(subtext)[0] or text if subtext else text
 
 
-def substr_right(text, subtext):
+def substr_right(text: t.Any, subtext: str) -> str:
     """
     Searches `text` from right-to-left for `subtext` and returns a substring consisting of the
     characters in `text` that are to the right of `subtext` or all string if no match found.
 
     Args:
-        text (str): String to partition.
-        subtext (str): String to search for.
+        text: String to partition.
+        subtext: String to search for.
 
     Returns:
-        str: Substring to right of `subtext`.
+        Substring to right of `subtext`.
 
     Example:
 
         >>> substr_right('abcdefcdg', 'cd')
         'efcdg'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return text.partition(subtext)[2] or text if subtext else text
 
 
-def substr_right_end(text, subtext):
+def substr_right_end(text: t.Any, subtext: str) -> str:
     """
     Searches `text` from left-to-right for `subtext` and returns a substring consisting of the
     characters in `text` that are to the right of `subtext` or all string if no match found.
 
     Args:
-        text (str): String to partition.
-        subtext (str): String to search for.
+        text: String to partition.
+        subtext: String to search for.
 
     Returns:
-        str: Substring to right of `subtext`.
+        Substring to right of `subtext`.
 
     Example:
 
         >>> substr_right_end('abcdefcdg', 'cd')
         'g'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return text.rpartition(subtext)[2] if subtext else text
 
 
-def successor(char):
+def successor(char: t.Any) -> str:
     """
     Return the successor character of `char`.
 
     Args:
-        char (str): Character to find the successor of.
+        char: Character to find the successor of.
 
     Returns:
-        str: Successor character.
+        Successor character.
 
     Example:
 
         >>> successor('b')
         'c'
         >>> successor('B')
         'C'
@@ -1775,24 +1822,24 @@
 
     .. versionadded:: 3.0.0
     """
     char = pyd.to_string(char)
     return chr(ord(char) + 1)
 
 
-def surround(text, wrapper):
+def surround(text: t.Any, wrapper: t.Any) -> str:
     """
     Surround a string with another string.
 
     Args:
-        text (str): String to surround with `wrapper`.
-        wrapper (str): String by which `text` is to be surrounded.
+        text: String to surround with `wrapper`.
+        wrapper: String by which `text` is to be surrounded.
 
     Returns:
-        str: Surrounded string.
+        Surrounded string.
 
     Example:
 
         >>> surround('abc', '"')
         '"abc"'
         >>> surround('abc', '!')
         '!abc!'
@@ -1800,66 +1847,66 @@
     .. versionadded:: 2.4.0
     """
     text = pyd.to_string(text)
     wrapper = pyd.to_string(wrapper)
     return f"{wrapper}{text}{wrapper}"
 
 
-def swap_case(text):
+def swap_case(text: t.Any) -> str:
     """
     Swap case of `text` characters.
 
     Args:
-        text (str): String to swap case.
+        text: String to swap case.
 
     Returns:
-        str: String with swapped case.
+        String with swapped case.
 
     Example:
 
         >>> swap_case('aBcDeF')
         'AbCdEf'
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     return text.swapcase()
 
 
-def title_case(text):
+def title_case(text: t.Any) -> str:
     """
     Convert `text` to title case.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to title case.
+        String converted to title case.
 
     Example:
 
         >>> title_case("bob's shop")
         "Bob's Shop"
 
     .. versionadded:: 3.0.0
     """
     text = pyd.to_string(text)
     # NOTE: Can't use text.title() since it doesn't handle apostrophes.
     return " ".join(word.capitalize() for word in re.split(" ", text))
 
 
-def to_lower(text):
+def to_lower(text: t.Any) -> str:
     """
     Converts the given :attr:`text` to lower text.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to lower case.
+        String converted to lower case.
 
     Example:
 
         >>> to_lower('--Foo-Bar--')
         '--foo-bar--'
         >>> to_lower('fooBar')
         'foobar'
@@ -1867,23 +1914,23 @@
         '__foo_bar__'
 
     .. versionadded:: 4.0.0
     """
     return pyd.to_string(text).lower()
 
 
-def to_upper(text):
+def to_upper(text: t.Any) -> str:
     """
     Converts the given :attr:`text` to upper text.
 
     Args:
-        text (str): String to convert.
+        text: String to convert.
 
     Returns:
-        str: String converted to upper case.
+        String converted to upper case.
 
     Example:
 
         >>> to_upper('--Foo-Bar--')
         '--FOO-BAR--'
         >>> to_upper('fooBar')
         'FOOBAR'
@@ -1891,47 +1938,47 @@
         '__FOO_BAR__'
 
     .. versionadded:: 4.0.0
     """
     return pyd.to_string(text).upper()
 
 
-def trim(text, chars=None):
+def trim(text: t.Any, chars: t.Union[str, None] = None) -> str:
     r"""
     Removes leading and trailing whitespace or specified characters from `text`.
 
     Args:
-        text (str): String to trim.
-        chars (str, optional): Specific characters to remove.
+        text: String to trim.
+        chars: Specific characters to remove.
 
     Returns:
-        str: Trimmed string.
+        Trimmed string.
 
     Example:
 
         >>> trim('  abc efg\r\n ')
         'abc efg'
 
     .. versionadded:: 1.1.0
     """
     # pylint: disable=redefined-outer-name
     text = pyd.to_string(text)
     return text.strip(chars)
 
 
-def trim_end(text, chars=None):
+def trim_end(text: t.Any, chars: t.Union[str, None] = None) -> str:
     r"""
     Removes trailing whitespace or specified characters from `text`.
 
     Args:
-        text (str): String to trim.
-        chars (str, optional): Specific characters to remove.
+        text: String to trim.
+        chars: Specific characters to remove.
 
     Returns:
-        str: Trimmed string.
+        Trimmed string.
 
     Example:
 
         >>> trim_end('  abc efg\r\n ')
         '  abc efg'
 
     .. versionadded:: 1.1.0
@@ -1939,24 +1986,24 @@
     .. versionchanged:: 4.0.0
         Renamed from ``trim_right`` to ``trim_end``.
     """
     text = pyd.to_string(text)
     return text.rstrip(chars)
 
 
-def trim_start(text, chars=None):
+def trim_start(text: t.Any, chars: t.Union[str, None] = None) -> str:
     r"""
     Removes leading  whitespace or specified characters from `text`.
 
     Args:
-        text (str): String to trim.
-        chars (str, optional): Specific characters to remove.
+        text: String to trim.
+        chars: Specific characters to remove.
 
     Returns:
-        str: Trimmed string.
+        Trimmed string.
 
     Example:
 
         >>> trim_start('  abc efg\r\n ')
         'abc efg\r\n '
 
     .. versionadded:: 1.1.0
@@ -1964,27 +2011,32 @@
     .. versionchanged:: 4.0.0
         Renamed from ``trim_left`` to ``trim_start``.
     """
     text = pyd.to_string(text)
     return text.lstrip(chars)
 
 
-def truncate(text, length=30, omission="...", separator=None):
+def truncate(
+    text: t.Any,
+    length: int = 30,
+    omission: str = "...",
+    separator: t.Union[str, re.Pattern, None] = None,
+) -> str:
     """
     Truncates `text` if it is longer than the given maximum string length. The last characters of
     the truncated string are replaced with the omission string which defaults to ``...``.
 
     Args:
-        text (str): String to truncate.
-        length (int, optional): Maximum string length. Defaults to ``30``.
-        omission (str, optional): String to indicate text is omitted.
-        separator (mixed, optional): Separator pattern to truncate to.
+        text: String to truncate.
+        length: Maximum string length. Defaults to ``30``.
+        omission: String to indicate text is omitted.
+        separator: Separator pattern to truncate to.
 
     Returns:
-        str: Truncated string.
+        Truncated string.
 
     Example:
 
         >>> truncate('hello world', 5)
         'he...'
         >>> truncate('hello world', 5, '..')
         'hel..'
@@ -2018,24 +2070,24 @@
 
         if last is not None:
             trunc_len = last.start()
 
     return text[:trunc_len] + omission
 
 
-def unescape(text):
+def unescape(text: t.Any) -> str:
     """
     The inverse of :func:`escape`. This method converts the HTML entities ``&amp;``, ``&lt;``,
     ``&gt;``, ``&quot;``, ``&#39;``, and ``&#96;`` in `text` to their corresponding characters.
 
     Args:
-        text (str): String to unescape.
+        text: String to unescape.
 
     Returns:
-        str: HTML unescaped string.
+        HTML unescaped string.
 
     Example:
 
         >>> results = unescape('&quot;1 &gt; 2 &amp;&amp; 3 &lt; 4&quot;')
         >>> results == '"1 > 2 && 3 < 4"'
         True
 
@@ -2044,23 +2096,23 @@
     .. versionchanged:: 1.1.0
         Moved to :mod:`pydash.strings`.
     """
     text = pyd.to_string(text)
     return html.unescape(text)
 
 
-def upper_case(text):
+def upper_case(text: t.Any) -> str:
     """
     Converts string to upper case, as space separated words.
 
     Args:
-        text (str): String to be converted to uppercase.
+        text: String to be converted to uppercase.
 
     Returns:
-        str: String converted to uppercase, as space separated words.
+        String converted to uppercase, as space separated words.
 
     Example:
 
         >>> upper_case('--foo-bar--')
         'FOO BAR'
         >>> upper_case('fooBar')
         'FOO BAR'
@@ -2071,23 +2123,23 @@
 
     .. versionchanged:: 5.0.0
         Improved unicode word support.
     """
     return " ".join(compounder(text)).upper()
 
 
-def upper_first(text):
+def upper_first(text: str) -> str:
     """
     Converts the first character of string to upper case.
 
     Args:
-        text (str): String passed in by the user.
+        text: String passed in by the user.
 
     Returns:
-        str: String in which the first character is converted to upper case.
+        String in which the first character is converted to upper case.
 
     Example:
 
         >>> upper_first('fred')
         'Fred'
         >>> upper_first('foo bar')
         'Foo bar'
@@ -2097,24 +2149,24 @@
         ';foobar'
 
     .. versionadded:: 4.0.0
     """
     return text[:1].upper() + text[1:]
 
 
-def unquote(text, quote_char='"'):
+def unquote(text: t.Any, quote_char: t.Any = '"') -> str:
     """
     Unquote `text` by removing `quote_char` if `text` begins and ends with it.
 
     Args:
-        text (str): String to unquote.
-        quote_char (str, optional): Quote character to remove. Defaults to `"`.
+        text: String to unquote.
+        quote_char: Quote character to remove. Defaults to `"`.
 
     Returns:
-        str: Unquoted string.
+        Unquoted string.
 
     Example:
 
         >>> unquote('"abc"')
         'abc'
         >>> unquote('"abc"', '#')
         '"abc"'
@@ -2130,40 +2182,41 @@
 
     if text == f"{quote_char}{inner}{quote_char}":
         text = inner
 
     return text
 
 
-def url(*paths, **params):
+def url(*paths: t.Any, **params: t.Any) -> str:
     """
     Combines a series of URL paths into a single URL. Optionally, pass in keyword arguments to
     append query parameters.
 
     Args:
-        paths (str): URL paths to combine.
+        paths: URL paths to combine.
 
     Keyword Args:
-        params (str, optional): Query parameters.
+        params: Query parameters.
 
     Returns:
-        str: URL string.
+        URL string.
 
     Example:
 
         >>> link = url('a', 'b', ['c', 'd'], '/', q='X', y='Z')
         >>> path, params = link.split('?')
         >>> path == 'a/b/c/d/'
         True
         >>> set(params.split('&')) == set(['q=X', 'y=Z'])
         True
 
     .. versionadded:: 2.2.0
     """
-    paths = pyd.chain(paths).flatten_deep().map(pyd.to_string).value()
+    # allow reassignment different type
+    paths = pyd.chain(paths).flatten_deep().map(pyd.to_string).value()  # type: ignore
     paths_list = []
     params_list = flatten_url_params(params)
 
     for path in paths:
         scheme, netloc, path, query, fragment = urlsplit(path)
         query = parse_qsl(query)
         params_list += query
@@ -2172,27 +2225,27 @@
     path = delimitedpathjoin("/", *paths_list)
     scheme, netloc, path, query, fragment = urlsplit(path)
     query = urlencode(params_list)
 
     return urlunsplit((scheme, netloc, path, query, fragment))
 
 
-def words(text, pattern=None):
+def words(text: t.Any, pattern: t.Union[str, None] = None) -> t.List[str]:
     """
     Return list of words contained in `text`.
 
     References:
         https://github.com/lodash/lodash/blob/master/words.js#L30
 
     Args:
-        text (str): String to split.
-        pattern (str, optional): Custom pattern to split words on. Defaults to ``None``.
+        text: String to split.
+        pattern: Custom pattern to split words on. Defaults to ``None``.
 
     Returns:
-        list: List of words.
+        List of words.
 
     Example:
 
         >>> words('a b, c; d-e')
         ['a', 'b', 'c', 'd', 'e']
         >>> words('fred, barney, & pebbles', '/[^, ]+/g')
         ['fred', 'barney', '&', 'pebbles']
@@ -2276,28 +2329,33 @@
         trailing = delimiter if paths and paths[-1].endswith(delimiter) else ""
         middle = delimiter.join([path.strip(delimiter) for path in paths if path.strip(delimiter)])
         path = "".join([leading, middle, trailing])
 
     return path
 
 
-def flatten_url_params(params):
+def flatten_url_params(
+    params: t.Union[
+        t.Dict[T, t.Union[T2, t.Iterable[T2]]],
+        t.List[t.Tuple[T, t.Union[T2, t.Iterable[T2]]]],
+    ],
+) -> t.List[t.Tuple[T, T2]]:
     """
     Flatten URL params into list of tuples. If any param value is a list or tuple, then map each
     value to the param key.
 
     >>> params = [('a', 1), ('a', [2, 3])]
     >>> assert flatten_url_params(params) == [('a', 1), ('a', 2), ('a', 3)]
     >>> params = {'a': [1, 2, 3]}
     >>> assert flatten_url_params(params) == [('a', 1), ('a', 2), ('a', 3)]
     """
     if isinstance(params, dict):
         params = list(params.items())
 
-    flattened = []
+    flattened: t.List = []
     for param, value in params:
         if isinstance(value, (list, tuple)):
             flattened += zip([param] * len(value), value)
         else:
             flattened.append((param, value))
 
     return flattened
```

### Comparing `pydash-6.0.2/src/pydash/utilities.py` & `pydash-7.0.0/src/pydash/utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,18 +7,22 @@
 from collections import namedtuple
 from datetime import datetime
 from functools import partial, wraps
 import math
 from random import randint, uniform
 import re
 import time
+import typing as t
+
+from typing_extensions import Literal, ParamSpec, Protocol, Type
 
 import pydash as pyd
 
 from .helpers import NUMBER_TYPES, UNSET, base_get, callit, getargcount, iterator
+from .types import PathT
 
 
 __all__ = (
     "attempt",
     "cond",
     "conforms",
     "conforms_to",
@@ -52,66 +56,87 @@
     "stub_string",
     "stub_true",
     "times",
     "to_path",
     "unique_id",
 )
 
+T = t.TypeVar("T")
+T2 = t.TypeVar("T2")
+CallableT = t.TypeVar("CallableT", bound=t.Callable)
+P = ParamSpec("P")
+
 # These regexes are used in to_path() to parse deep path strings.
 
 # This is used to split a deep path string into dict keys or list indexes. This matches "." as
 # delimiter (unless it is escaped by "//") and "[<integer>]" as delimiter while keeping the
 # "[<integer>]" as an item.
-RE_PATH_KEY_DELIM = re.compile(r"(?<!\\)(?:\\\\)*\.|(\[\d+\])")
+RE_PATH_KEY_DELIM = re.compile(r"(?<!\\)(?:\\\\)*\.|(\[-?\d+\])")
 
 # Matches on path strings like "[<integer>]". This is used to test whether a path string part is a
 # list index.
-RE_PATH_LIST_INDEX = re.compile(r"^\[\d+\]$")
+RE_PATH_LIST_INDEX = re.compile(r"^\[-?\d+\]$")
 
 
 ID_COUNTER = 0
 
 PathToken = namedtuple("PathToken", ["key", "default_factory"])
 
 
-def attempt(func, *args, **kwargs):
+def attempt(func: t.Callable[P, T], *args: "P.args", **kwargs: "P.kwargs") -> t.Union[T, Exception]:
     """
     Attempts to execute `func`, returning either the result or the caught error object.
 
     Args:
-        func (callable): The function to attempt.
+        func: The function to attempt.
 
     Returns:
-        mixed: Returns the `func` result or error object.
+        Returns the `func` result or error object.
 
     Example:
 
         >>> results = attempt(lambda x: x/0, 1)
         >>> assert isinstance(results, ZeroDivisionError)
 
     .. versionadded:: 1.1.0
     """
     try:
         ret = func(*args, **kwargs)
     except Exception as ex:
-        ret = ex
+        # allow different type reassignment
+        ret = ex  # type: ignore
 
     return ret
 
 
+@t.overload
+def cond(
+    pairs: t.List[t.Tuple[t.Callable[P, t.Any], t.Callable[P, T]]],
+    *extra_pairs: t.Tuple[t.Callable[P, t.Any], t.Callable[P, T]],
+) -> t.Callable[P, T]:
+    ...
+
+
+@t.overload
+def cond(
+    pairs: t.List[t.List[t.Callable[P, t.Any]]], *extra_pairs: t.List[t.Callable[P, t.Any]]
+) -> t.Callable[P, t.Any]:
+    ...
+
+
 def cond(pairs, *extra_pairs):
     """
     Creates a function that iterates over `pairs` and invokes the corresponding function of the
     first predicate to return truthy.
 
     Args:
-        pairs (list): A list of predicate-function pairs.
+        pairs: A list of predicate-function pairs.
 
     Returns:
-        callable: Returns the new composite function.
+        Returns the new composite function.
 
     Example:
 
         >>> func = cond([[matches({'a': 1}), constant('matches A')],\
                          [matches({'b': 2}), constant('matches B')],\
                          [stub_true, lambda value: value]])
         >>> func({'a': 1, 'b': 2})
@@ -149,25 +174,35 @@
 
             if callit(predicate, *args):
                 return iteratee(*args)
 
     return _cond
 
 
-def conforms(source):
+@t.overload
+def conforms(source: t.Dict[T, t.Callable[[T2], t.Any]]) -> t.Callable[[t.Dict[T, T2]], bool]:
+    ...
+
+
+@t.overload
+def conforms(source: t.List[t.Callable[[T], t.Any]]) -> t.Callable[[t.List[T]], bool]:
+    ...
+
+
+def conforms(source: t.Union[t.List, t.Dict]) -> t.Callable:
     """
     Creates a function that invokes the predicate properties of `source` with the corresponding
     property values of a given object, returning ``True`` if all predicates return truthy, else
     ``False``.
 
     Args:
-        source (dict|list): The object of property predicates to conform to.
+        source: The object of property predicates to conform to.
 
     Returns:
-        callable: Returns the new spec function.
+        Returns the new spec function.
 
     Example:
 
         >>> func = conforms({'b': lambda n: n > 1})
         >>> func({'b': 2})
         True
         >>> func({'b': 0})
@@ -186,22 +221,32 @@
             if not pyd.has(obj, key) or not predicate(obj[key]):
                 return False
         return True
 
     return _conforms
 
 
+@t.overload
+def conforms_to(obj: t.Dict[T, T2], source: t.Dict[T, t.Callable[[T2], t.Any]]) -> bool:
+    ...
+
+
+@t.overload
+def conforms_to(obj: t.List[T], source: t.List[t.Callable[[T], t.Any]]) -> bool:
+    ...
+
+
 def conforms_to(obj, source):
     """
     Checks if `obj` conforms to `source` by invoking the predicate properties of `source` with the
     corresponding property values of `obj`.
 
     Args:
-        obj (dict|list): The object to inspect.
-        source (dict|list): The object of property predicates to conform to.
+        obj: The object to inspect.
+        source: The object of property predicates to conform to.
 
     Example:
 
         >>> conforms_to({'b': 2}, {'b': lambda n: n > 1})
         True
         >>> conforms_to({'b': 0}, {'b': lambda n: n > 1})
         False
@@ -211,23 +256,23 @@
         False
 
     .. versionadded:: 4.0.0
     """
     return conforms(source)(obj)
 
 
-def constant(value):
+def constant(value: T) -> t.Callable[..., T]:
     """
     Creates a function that returns `value`.
 
     Args:
-        value (mixed): Constant value to return.
+        value: Constant value to return.
 
     Returns:
-        callable: Function that always returns `value`.
+        Function that always returns `value`.
 
     Example:
 
         >>> pi = constant(3.14)
         >>> pi() == 3.14
         True
 
@@ -235,49 +280,100 @@
 
     .. versionchanged:: 4.0.0
         Returned function ignores arguments instead of raising exception.
     """
     return partial(identity, value)
 
 
-def default_to(value, default_value):
+def default_to(value: t.Union[T, None], default_value: T2) -> t.Union[T, T2]:
     """
     Checks `value` to determine whether a default value should be returned in its place. The
     `default_value` is returned if value is None.
 
     Args:
-        value (mixed): Value passed in by the user.
-        default_value (mixed): Default value passed in by the user.
+        default_value: Default value passed in by the user.
 
     Returns:
-        mixed: Returns `value` if :attr:`value` is given otherwise returns `default_value`.
+        Returns `value` if :attr:`value` is given otherwise returns `default_value`.
 
     Example:
 
         >>> default_to(1, 10)
         1
         >>> default_to(None, 10)
         10
 
     .. versionadded:: 4.0.0
     """
     return default_to_any(value, default_value)
 
 
+@t.overload
+def default_to_any(value: None, *default_values: None) -> None:
+    ...
+
+
+@t.overload
+def default_to_any(
+    value: t.Union[T, None],
+    default_value1: None,
+    default_value2: T2,
+) -> t.Union[T, T2]:
+    ...
+
+
+@t.overload
+def default_to_any(
+    value: t.Union[T, None],
+    default_value1: None,
+    default_value2: None,
+    default_value3: T2,
+) -> t.Union[T, T2]:
+    ...
+
+
+@t.overload
+def default_to_any(
+    value: t.Union[T, None],
+    default_value1: None,
+    default_value2: None,
+    default_value3: None,
+    default_value4: T2,
+) -> t.Union[T, T2]:
+    ...
+
+
+@t.overload
+def default_to_any(
+    value: t.Union[T, None],
+    default_value1: None,
+    default_value2: None,
+    default_value3: None,
+    default_value4: None,
+    default_value5: T2,
+) -> t.Union[T, T2]:
+    ...
+
+
+@t.overload
+def default_to_any(value: t.Union[T, None], *default_values: T2) -> t.Union[T, T2]:
+    ...
+
+
 def default_to_any(value, *default_values):
     """
     Checks `value` to determine whether a default value should be returned in its place. The first
     item that is not None of the `default_values` is returned.
 
     Args:
-        value (mixed): Value passed in by the user.
-        *default_values (mixed): Default values passed in by the user.
+        value: Value passed in by the user.
+        *default_values: Default values passed in by the user.
 
     Returns:
-        mixed: Returns `value` if :attr:`value` is given otherwise returns the first not None value
+        Returns `value` if :attr:`value` is given otherwise returns the first not None value
             of `default_values`.
 
     Example:
 
         >>> default_to_any(1, 10, 20)
         1
         >>> default_to_any(None, 10, 20)
@@ -290,23 +386,33 @@
     """
     values = (value,) + default_values
     for val in values:
         if val is not None:
             return val
 
 
+@t.overload
+def identity(arg: T, *args: t.Any) -> T:
+    ...
+
+
+@t.overload
+def identity(arg: None = None, *args: t.Any) -> None:
+    ...
+
+
 def identity(arg=None, *args):
     """
     Return the first argument provided to it.
 
     Args:
-        *args (mixed): Arguments.
+        *args: Arguments.
 
     Returns:
-        mixed: First argument or ``None``.
+        First argument or ``None``.
 
     Example:
 
         >>> identity(1)
         1
         >>> identity(1, 2, 3)
         1
@@ -314,26 +420,36 @@
         True
 
     .. versionadded:: 1.0.0
     """
     return arg
 
 
+@t.overload
+def iteratee(func: t.Callable[P, T]) -> t.Callable[P, T]:
+    ...
+
+
+@t.overload
+def iteratee(func: t.Any) -> t.Callable:
+    ...
+
+
 def iteratee(func):
     """
     Return a pydash style iteratee. If `func` is a property name the created iteratee will return
     the property value for a given element. If `func` is an object the created iteratee will return
     ``True`` for elements that contain the equivalent object properties, otherwise it will return
     ``False``.
 
     Args:
-        func (mixed): Object to create iteratee function from.
+        func: Object to create iteratee function from.
 
     Returns:
-        callable: Iteratee function.
+        Iteratee function.
 
     Example:
 
         >>> get_data = iteratee('data')
         >>> get_data({'data': [1, 2, 3]})
         [1, 2, 3]
         >>> is_active = iteratee({'active': True})
@@ -397,25 +513,25 @@
         # Optimize iteratee by specifying the exact number of arguments the iteratee takes so that
         # arg inspection (costly process) can be skipped in helpers.callit().
         cbk._argcount = 1
 
     return cbk
 
 
-def matches(source):
+def matches(source: t.Any) -> t.Callable[[t.Any], bool]:
     """
     Creates a matches-style predicate function which performs a deep comparison between a given
     object and the `source` object, returning ``True`` if the given object has equivalent property
     values, else ``False``.
 
     Args:
-        source (dict): Source object used for comparision.
+        source: Source object used for comparision.
 
     Returns:
-        callable: Function that compares an object to `source` and returns whether the two objects
+        Function that compares an object to `source` and returns whether the two objects
             contain the same items.
 
     Example:
 
         >>> matches({'a': {'b': 2}})({'a': {'b': 2, 'c':3}})
         True
         >>> matches({'a': 1})({'b': 2, 'a': 1})
@@ -427,24 +543,24 @@
 
     .. versionchanged:: 3.0.0
         Use :func:`pydash.predicates.is_match` as matching function.
     """
     return lambda obj: pyd.is_match(obj, source)
 
 
-def matches_property(key, value):
+def matches_property(key: t.Any, value: t.Any) -> t.Callable[[t.Any], bool]:
     """
     Creates a function that compares the property value of `key` on a given object to `value`.
 
     Args:
-        key (str): Object key to match against.
-        value (mixed): Value to compare to.
+        key: Object key to match against.
+        value: Value to compare to.
 
     Returns:
-        callable: Function that compares `value` to an object's `key` and returns whether they are
+        Function that compares `value` to an object's `key` and returns whether they are
             equal.
 
     Example:
 
         >>> matches_property('a', 1)({'a': 1, 'b': 2})
         True
         >>> matches_property(0, 1)([1, 2, 3])
@@ -454,27 +570,46 @@
 
     .. versionadded:: 3.1.0
     """
     prop_accessor = property_(key)
     return lambda obj: matches(value)(prop_accessor(obj))
 
 
+class MemoizedFunc(Protocol[P, T, T2]):
+    cache: t.Dict[T2, T]
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
+        ...  # pragma: no cover
+
+
+@t.overload
+def memoize(func: t.Callable[P, T], resolver: None = None) -> MemoizedFunc[P, T, str]:
+    ...
+
+
+@t.overload
+def memoize(
+    func: t.Callable[P, T], resolver: t.Union[t.Callable[P, T2], None] = None
+) -> MemoizedFunc[P, T, T2]:
+    ...
+
+
 def memoize(func, resolver=None):
     """
     Creates a function that memoizes the result of `func`. If `resolver` is provided it will be used
     to determine the cache key for storing the result based on the arguments provided to the
     memoized function. By default, all arguments provided to the memoized function are used as the
     cache key. The result cache is exposed as the cache property on the memoized function.
 
     Args:
-        func (callable): Function to memoize.
-        resolver (callable, optional): Function that returns the cache key to use.
+        func: Function to memoize.
+        resolver: Function that returns the cache key to use.
 
     Returns:
-        callable: Memoized function.
+        Memoized function.
 
     Example:
 
         >>> ident = memoize(identity)
         >>> ident(1)
         1
         >>> ident.cache['(1,){}'] == 1
@@ -483,42 +618,42 @@
         1
         >>> ident.cache['(1, 2, 3){}'] == 1
         True
 
     .. versionadded:: 1.0.0
     """
 
-    def memoized(*args, **kwargs):
+    def memoized(*args: P.args, **kwargs: P.kwargs):
         if resolver:
             key = resolver(*args, **kwargs)
         else:
             key = f"{args}{kwargs}"
 
-        if key not in memoized.cache:
-            memoized.cache[key] = func(*args, **kwargs)
+        if key not in memoized.cache:  # type: ignore
+            memoized.cache[key] = func(*args, **kwargs)  # type:ignore
 
-        return memoized.cache[key]
+        return memoized.cache[key]  # type: ignore
 
     memoized.cache = {}
 
     return memoized
 
 
-def method(path, *args, **kwargs):
+def method(path: PathT, *args: t.Any, **kwargs: t.Any) -> t.Callable[..., t.Any]:
     """
     Creates a function that invokes the method at `path` on a given object. Any additional arguments
     are provided to the invoked method.
 
     Args:
-        path (str): Object path of method to invoke.
-        *args (mixed): Global arguments to apply to method when invoked.
-        **kwargs (mixed): Global keyword argument to apply to method when invoked.
+        path: Object path of method to invoke.
+        *args: Global arguments to apply to method when invoked.
+        **kwargs: Global keyword argument to apply to method when invoked.
 
     Returns:
-        callable: Function that invokes method located at path for object.
+        Function that invokes method located at path for object.
 
     Example:
 
         >>> obj = {'a': {'b': [None, lambda x: x]}}
         >>> echo = method('a.b.1')
         >>> echo(obj, 1) == 1
         True
@@ -531,26 +666,26 @@
     def _method(obj, *_args, **_kwargs):
         func = pyd.partial(pyd.get(obj, path), *args, **kwargs)
         return func(*_args, **_kwargs)
 
     return _method
 
 
-def method_of(obj, *args, **kwargs):
+def method_of(obj: t.Any, *args: t.Any, **kwargs: t.Any) -> t.Callable[..., t.Any]:
     """
     The opposite of :func:`method`. This method creates a function that invokes the method at a
     given path on object. Any additional arguments are provided to the invoked method.
 
     Args:
-        obj (mixed): The object to query.
-        *args (mixed): Global arguments to apply to method when invoked.
-        **kwargs (mixed): Global keyword argument to apply to method when invoked.
+        obj: The object to query.
+        *args: Global arguments to apply to method when invoked.
+        **kwargs: Global keyword argument to apply to method when invoked.
 
     Returns:
-        callable: Function that invokes method located at path for object.
+        Function that invokes method located at path for object.
 
     Example:
 
         >>> obj = {'a': {'b': [None, lambda x: x]}}
         >>> dispatch = method_of(obj)
         >>> dispatch('a.b.1', 1) == 1
         True
@@ -563,33 +698,33 @@
     def _method_of(path, *_args, **_kwargs):
         func = pyd.partial(pyd.get(obj, path), *args, **kwargs)
         return func(*_args, **_kwargs)
 
     return _method_of
 
 
-def noop(*args, **kwargs):  # pylint: disable=unused-argument
+def noop(*args: t.Any, **kwargs: t.Any) -> None:  # pylint: disable=unused-argument
     """
     A no-operation function.
 
     .. versionadded:: 1.0.0
     """
     pass
 
 
-def nth_arg(pos=0):
+def nth_arg(pos: int = 0) -> t.Callable[..., t.Any]:
     """
     Creates a function that gets the argument at index n. If n is negative, the nth argument from
     the end is returned.
 
     Args:
-        pos (int): The index of the argument to return.
+        pos: The index of the argument to return.
 
     Returns:
-        callable: Returns the new pass-thru function.
+        Returns the new pass-thru function.
 
     Example:
 
         >>> func = nth_arg(1)
         >>> func(11, 22, 33, 44)
         22
         >>> func = nth_arg(-1)
@@ -606,21 +741,21 @@
             position = 0
 
         return pyd.get(args, position)
 
     return _nth_arg
 
 
-def now():
+def now() -> int:
     """
     Return the number of milliseconds that have elapsed since the Unix epoch (1 January 1970
     00:00:00 UTC).
 
     Returns:
-        int: Milliseconds since Unix epoch.
+        Milliseconds since Unix epoch.
 
     .. versionadded:: 1.0.0
 
     .. versionchanged:: 3.0.0
         Use ``datetime`` module for calculating elapsed time.
     """
     epoch = datetime.utcfromtimestamp(0)
@@ -633,101 +768,101 @@
         seconds = (
             delta.microseconds + (delta.seconds + delta.days * 24 * 3600) * 10**6
         ) / 10**6
 
     return int(seconds * 1000)
 
 
-def over(funcs):
+def over(funcs: t.Iterable[t.Callable[P, T]]) -> t.Callable[P, t.List[T]]:
     """
     Creates a function that invokes all functions in `funcs` with the arguments it receives and
     returns their results.
 
     Args:
-        funcs (list): List of functions to be invoked.
+        funcs: List of functions to be invoked.
 
     Returns:
-        callable: Returns the new pass-thru function.
+        Returns the new pass-thru function.
 
     Example:
 
         >>> func = over([max, min])
         >>> func(1, 2, 3, 4)
         [4, 1]
 
     .. versionadded:: 4.0.0
     """
 
-    def _over(*args):
-        return [func(*args) for func in funcs]
+    def _over(*args: P.args, **kwargs: P.kwargs) -> t.List[T]:
+        return [func(*args, **kwargs) for func in funcs]
 
     return _over
 
 
-def over_every(funcs):
+def over_every(funcs: t.Iterable[t.Callable[P, t.Any]]) -> t.Callable[P, bool]:
     """
-    Creates a function that checks if all of the functions in `funcs` return truthy when invoked
-    with the arguments it receives.
+    Creates a function that checks if all the functions in `funcs` return truthy when invoked with
+    the arguments it receives.
 
     Args:
-        funcs (list): List of functions to be invoked.
+        funcs: List of functions to be invoked.
 
     Returns:
-        callable: Returns the new pass-thru function.
+        Returns the new pass-thru function.
 
     Example:
 
         >>> func = over_every([bool, lambda x: x is not None])
         >>> func(1)
         True
 
     .. versionadded:: 4.0.0
     """
 
-    def _over_every(*args):
-        return all(func(*args) for func in funcs)
+    def _over_every(*args: P.args, **kwargs: P.kwargs) -> bool:
+        return all(func(*args, **kwargs) for func in funcs)
 
     return _over_every
 
 
-def over_some(funcs):
+def over_some(funcs: t.Iterable[t.Callable[P, t.Any]]) -> t.Callable[P, bool]:
     """
     Creates a function that checks if any of the functions in `funcs` return truthy when invoked
     with the arguments it receives.
 
     Args:
-        funcs (list): List of functions to be invoked.
+        funcs: List of functions to be invoked.
 
     Returns:
-        callable: Returns the new pass-thru function.
+        Returns the new pass-thru function.
 
     Example:
 
         >>> func = over_some([bool, lambda x: x is None])
         >>> func(1)
         True
 
     .. versionadded:: 4.0.0
     """
 
-    def _over_some(*args):
-        return any(func(*args) for func in funcs)
+    def _over_some(*args: P.args, **kwargs: P.kwargs) -> bool:
+        return any(func(*args, **kwargs) for func in funcs)
 
     return _over_some
 
 
-def property_(path):
+def property_(path: PathT) -> t.Callable[[t.Any], t.Any]:
     """
     Creates a function that returns the value at path of a given object.
 
     Args:
-        path (str|list): Path value to fetch from object.
+        path: Path value to fetch from object.
 
     Returns:
-        callable: Function that returns object's path value.
+        Function that returns object's path value.
 
     Example:
 
         >>> get_data = property_('data')
         >>> get_data({'data': 1})
         1
         >>> get_data({}) is None
@@ -740,45 +875,45 @@
 
     .. versionchanged:: 4.0.1
         Made property accessor work with deep path strings.
     """
     return lambda obj: pyd.get(obj, path)
 
 
-def properties(*paths):
+def properties(*paths: t.Any) -> t.Callable[[t.Any], t.Any]:
     """
     Like :func:`property_` except that it returns a list of values at each path in `paths`.
 
     Args:
-        *path (str|list): Path values to fetch from object.
+        *path: Path values to fetch from object.
 
     Returns:
-        callable: Function that returns object's path value.
+        Function that returns object's path value.
 
     Example:
 
         >>> getter = properties('a', 'b', ['c', 'd', 'e'])
         >>> getter({'a': 1, 'b': 2, 'c': {'d': {'e': 3}}})
         [1, 2, 3]
 
     .. versionadded:: 4.1.0
     """
     return lambda obj: [getter(obj) for getter in (pyd.property_(path) for path in paths)]
 
 
-def property_of(obj):
+def property_of(obj: t.Any) -> t.Callable[[PathT], t.Any]:
     """
     The inverse of :func:`property_`. This method creates a function that returns the key value of a
     given key on `obj`.
 
     Args:
-        obj (dict|list): Object to fetch values from.
+        obj: Object to fetch values from.
 
     Returns:
-        callable: Function that returns object's key value.
+        Function that returns object's key value.
 
     Example:
 
         >>> getter = property_of({'a': 1, 'b': 2, 'c': 3})
         >>> getter('a')
         1
         >>> getter('b')
@@ -790,29 +925,56 @@
 
     .. versionchanged:: 4.0.0
         Removed alias ``prop_of``.
     """
     return lambda key: pyd.get(obj, key)
 
 
-def random(start=0, stop=1, floating=False):
+@t.overload
+def random(start: int = 0, stop: int = 1, *, floating: Literal[False] = False) -> int:
+    ...
+
+
+@t.overload
+def random(start: float, stop: int = 1, floating: bool = False) -> float:
+    ...
+
+
+@t.overload
+def random(start: int = 0, *, stop: float, floating: bool = False) -> float:
+    ...
+
+
+@t.overload
+def random(start: float, stop: float, floating: bool = False) -> float:
+    ...
+
+
+@t.overload
+def random(
+    start: t.Union[float, int] = 0, stop: t.Union[float, int] = 1, *, floating: Literal[True]
+) -> float:
+    ...
+
+
+def random(start: t.Union[float, int] = 0, stop: t.Union[float, int] = 1, floating: bool = False):
     """
     Produces a random number between `start` and `stop` (inclusive). If only one argument is
     provided a number between 0 and the given number will be returned. If floating is truthy or
     either `start` or `stop` are floats a floating-point number will be returned instead of an
     integer.
 
     Args:
-        start (int): Minimum value.
-        stop (int): Maximum value.
-        floating (bool, optional): Whether to force random value to ``float``. Defaults to
+        start: Minimum value.
+        stop: Maximum value.
+        floating: Whether to force random value to ``float``. Defaults to
             ``False``.
 
     Returns:
-        int|float: Random value.
+        Random value.
 
     Example:
 
         >>> 0 <= random() <= 1
         True
         >>> 5 <= random(5, 10) <= 10
         True
@@ -825,32 +987,42 @@
 
     if stop < start:
         stop, start = start, stop
 
     if floating:
         rnd = uniform(start, stop)
     else:
-        rnd = randint(start, stop)
+        rnd = randint(start, stop)  # type: ignore
 
     return rnd
 
 
+@t.overload
+def range_(stop: int) -> t.Generator[int, None, None]:
+    ...
+
+
+@t.overload
+def range_(start: int, stop: int, step: int = 1) -> t.Generator[int, None, None]:
+    ...
+
+
 def range_(*args):
     """
     Creates a list of numbers (positive and/or negative) progressing from start up to but not
     including end. If `start` is less than `stop`, a zero-length range is created unless a negative
     `step` is specified.
 
     Args:
-        start (int, optional): Integer to start with. Defaults to ``0``.
-        stop (int): Integer to stop at.
-        step (int, optional): The value to increment or decrement by. Defaults to ``1``.
+        start: Integer to start with. Defaults to ``0``.
+        stop: Integer to stop at.
+        step: The value to increment or decrement by. Defaults to ``1``.
 
     Yields:
-        int: Next integer in range.
+        Next integer in range.
 
     Example:
 
         >>> list(range_(5))
         [0, 1, 2, 3, 4]
         >>> list(range_(1, 4))
         [1, 2, 3]
@@ -869,26 +1041,36 @@
 
     .. versionchanged:: 4.0.0
         Support decrementing when start argument is greater than stop argument.
     """
     return base_range(*args)
 
 
+@t.overload
+def range_right(stop: int) -> t.Generator[int, None, None]:
+    ...
+
+
+@t.overload
+def range_right(start: int, stop: int, step: int = 1) -> t.Generator[int, None, None]:
+    ...
+
+
 def range_right(*args):
     """
     Similar to :func:`range_`, except that it populates the values in descending order.
 
     Args:
-        start (int, optional): Integer to start with. Defaults to ``0``.
-        stop (int): Integer to stop at.
-        step (int, optional): The value to increment or decrement by. Defaults to ``1`` if `start`
+        start: Integer to start with. Defaults to ``0``.
+        stop: Integer to stop at.
+        step: The value to increment or decrement by. Defaults to ``1`` if `start`
             < `stop` else ``-1``.
 
     Yields:
-        int: Next integer in range.
+        Next integer in range.
 
     Example:
 
         >>> list(range_right(5))
         [4, 3, 2, 1, 0]
         >>> list(range_right(1, 4))
         [3, 2, 1]
@@ -896,27 +1078,43 @@
         [4, 2, 0]
 
     .. versionadded:: 4.0.0
     """
     return base_range(*args, from_right=True)
 
 
+# TODO
+@t.overload
+def result(obj: None, key: t.Any, default: None = None) -> None:
+    ...
+
+
+@t.overload
+def result(obj: None, key: t.Any, default: T) -> T:
+    ...
+
+
+@t.overload
+def result(obj: t.Any, key: t.Any, default: t.Any = None) -> t.Any:
+    ...
+
+
 def result(obj, key, default=None):
     """
     Return the value of property `key` on `obj`. If `key` value is a function it will be invoked and
     its result returned, else the property value is returned. If `obj` is falsey then `default` is
     returned.
 
     Args:
-        obj (list|dict): Object to retrieve result from.
-        key (mixed): Key or index to get result from.
-        default (mixed, optional): Default value to return if `obj` is falsey. Defaults to ``None``.
+        obj: Object to retrieve result from.
+        key: Key or index to get result from.
+        default: Default value to return if `obj` is falsey. Defaults to ``None``.
 
     Returns:
-        mixed: Result of ``obj[key]`` or ``None``.
+        Result of ``obj[key]`` or ``None``.
 
     Example:
 
         >>> result({'a': 1, 'b': lambda: 2}, 'a')
         1
         >>> result({'a': 1, 'b': lambda: 2}, 'b')
         2
@@ -938,47 +1136,47 @@
     if callable(ret):
         ret = ret()
 
     return ret
 
 
 def retry(  # noqa: C901
-    attempts=3,
-    delay=0.5,
-    max_delay=150.0,
-    scale=2.0,
-    jitter=0,
-    exceptions=(Exception,),
-    on_exception=None,
-):
+    attempts: int = 3,
+    delay: t.Union[int, float] = 0.5,
+    max_delay: t.Union[int, float] = 150.0,
+    scale: t.Union[int, float] = 2.0,
+    jitter: t.Union[int, float, t.Tuple[t.Union[int, float], t.Union[int, float]]] = 0,
+    exceptions: t.Iterable[Type[Exception]] = (Exception,),
+    on_exception: t.Union[t.Callable[[Exception, int], t.Any], None] = None,
+) -> t.Callable[[CallableT], CallableT]:
     """
     Decorator that retries a function multiple times if it raises an exception with an optional
     delay between each attempt.
 
     When a `delay` is supplied, there will be a sleep period in between retry
     attempts. The first delay time will always be equal to `delay`. After
     subsequent retries, the delay time will be scaled by `scale` up to
     `max_delay`. If `max_delay` is ``0``, then `delay` can increase unbounded.
 
     Args:
-        attempts (int, optional): Number of retry attempts. Defaults to ``3``.
-        delay (int|float, optional): Base amount of seconds to sleep between retry attempts.
+        attempts: Number of retry attempts. Defaults to ``3``.
+        delay: Base amount of seconds to sleep between retry attempts.
             Defaults to ``0.5``.
-        max_delay (int|float, optional): Maximum number of seconds to sleep between retries. Is
+        max_delay: Maximum number of seconds to sleep between retries. Is
             ignored when equal to ``0``. Defaults to ``150.0`` (2.5 minutes).
-        scale (int|float, optional): Scale factor to increase `delay` after first retry fails.
+        scale: Scale factor to increase `delay` after first retry fails.
             Defaults to ``2.0``.
-        jitter (int|float|tuple, optional): Random jitter to add to `delay` time. Can be a positive
+        jitter: Random jitter to add to `delay` time. Can be a positive
             number or 2-item tuple of numbers representing the random range to choose from. When a
             number is given, the random range will be from ``[0, jitter]``. When jitter is a float
             or contains a float, then a random float will be chosen; otherwise, a random integer
             will be selected. Defaults to ``0`` which disables jitter.
-        exceptions (tuple, optional): Tuple of exceptions that trigger a retry attempt. Exceptions
+        exceptions: Tuple of exceptions that trigger a retry attempt. Exceptions
             not in the tuple will be ignored. Defaults to ``(Exception,)`` (all exceptions).
-        on_exception (callable, optional): Function that is called when a retryable exception is
+        on_exception: Function that is called when a retryable exception is
             caught. It is invoked with ``on_exception(exc, attempt)`` where ``exc`` is the caught
             exception and ``attempt`` is the attempt count. All arguments are optional. Defaults to
             ``None``.
 
     Example:
 
         >>> @retry(attempts=3, delay=0)
@@ -1063,110 +1261,120 @@
                     delay_time *= scale
 
         return decorated
 
     return decorator
 
 
-def stub_list():
+def stub_list() -> t.List:
     """
     Returns empty "list".
 
     Returns:
-        list: Empty list.
+        Empty list.
 
     Example:
 
         >>> stub_list()
         []
 
     .. versionadded:: 4.0.0
     """
     return []
 
 
-def stub_dict():
+def stub_dict() -> t.Dict:
     """
     Returns empty "dict".
 
     Returns:
-        dict: Empty dict.
+        Empty dict.
 
     Example:
 
         >>> stub_dict()
         {}
 
     .. versionadded:: 4.0.0
     """
     return {}
 
 
-def stub_false():
+def stub_false() -> Literal[False]:
     """
     Returns ``False``.
 
     Returns:
-        bool: False
+        False
 
     Example:
 
         >>> stub_false()
         False
 
     .. versionadded:: 4.0.0
     """
     return False
 
 
-def stub_string():
+def stub_string() -> str:
     """
     Returns an empty string.
 
     Returns:
-        str: Empty string
+        Empty string
 
     Example:
 
         >>> stub_string()
         ''
 
     .. versionadded:: 4.0.0
     """
     return ""
 
 
-def stub_true():
+def stub_true() -> Literal[True]:
     """
     Returns ``True``.
 
     Returns:
-        bool: True
+        True
 
     Example:
 
         >>> stub_true()
         True
 
     .. versionadded:: 4.0.0
     """
     return True
 
 
-def times(n, iteratee=None):
+@t.overload
+def times(n: int, iteratee: t.Callable[..., T]) -> t.List[T]:
+    ...
+
+
+@t.overload
+def times(n: int, iteratee: None = None) -> t.List[int]:
+    ...
+
+
+def times(n: int, iteratee=None):
     """
     Executes the iteratee `n` times, returning a list of the results of each iteratee execution. The
     iteratee is invoked with one argument: ``(index)``.
 
     Args:
-        n (int): Number of times to execute `iteratee`.
-        iteratee (callable): Function to execute.
+        n: Number of times to execute `iteratee`.
+        iteratee: Function to execute.
 
     Returns:
-        list: A list of results from calling `iteratee`.
+        A list of results from calling `iteratee`.
 
     Example:
 
         >>> times(5, lambda i: i)
         [0, 1, 2, 3, 4]
 
     .. versionadded:: 1.0.0
@@ -1184,23 +1392,23 @@
         argcount = 1
     else:
         argcount = getargcount(iteratee, maxargs=1)
 
     return [callit(iteratee, index, argcount=argcount) for index in range(n)]
 
 
-def to_path(value):
+def to_path(value: PathT) -> t.List[t.Hashable]:
     """
     Converts values to a property path array.
 
     Args:
-        value (mixed): Value to convert.
+        value: Value to convert.
 
     Returns:
-        list: Returns the new property path array.
+        Returns the new property path array.
 
     Example:
 
         >>> to_path('a.b.c')
         ['a', 'b', 'c']
         >>> to_path('a[0].b.c')
         ['a', 0, 'b', 'c']
@@ -1218,23 +1426,23 @@
             token.key if isinstance(token, PathToken) else token for token in to_path_tokens(value)
         ]
     else:
         path = [tokens]
     return path
 
 
-def unique_id(prefix=None):
+def unique_id(prefix: t.Union[str, None] = None) -> str:
     """
     Generates a unique ID. If `prefix` is provided the ID will be appended to  it.
 
     Args:
-        prefix (str, optional): String prefix to prepend to ID value.
+        prefix: String prefix to prepend to ID value.
 
     Returns:
-        str: ID value.
+        ID value.
 
     Example:
 
         >>> unique_id()
         '1'
         >>> unique_id('id_')
         'id_2'
```

### Comparing `pydash-6.0.2/src/pydash.egg-info/PKG-INFO` & `pydash-7.0.0/src/pydash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 6.0.2
+Version: 7.0.0
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,23 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.0 (2023-04-11)
+-------------------
+
+- Add type annotations to package. Raise an issue for any typing issues at https://github.com/dgilland/pydash/issues. Thanks DeviousStoat_! (**breaking change**)
+- Change behavior of ``to_dict`` to not using ``dict()`` internally. Previous behavior would be for something like ``to_dict([["k", "v"], ["x", "y"]])`` to return ``{"k": "v", "x": "y"}`` (equivalent to calling ``dict(...)``) but ``to_dict([["k"], ["v"], ["x"], ["y"]])`` would return ``{0: ["x"], 1: ["v"], 2: ["x"], 3: ["y"]}``. The new behavior is to always return iterables as dictionaries with their indexes as keys like ``{0: ["k", "v"], 1: ["x", "y"]}``. This is consistent with how iterable objects are iterated over and means that ``to_dict`` will have more reliable output. (**breaking change**)
+- Change behavior of ``slugify`` to remove single-quotes from output. Instead of ``slugify("the cat's meow") == "the-cat's-meow"``, the new behavior is to return ``"the-cats-meow"``. (**breaking change**)
+- Add support for negative indexes in ``get`` path keys. Thanks bl4ckst0ne_!
+
+
 v6.0.2 (2023-02-23)
 -------------------
 
 - Only prevent access to object paths containing ``__globals__`` or ``__builtins__`` instead of all dunder-methods for non-dict/list objects.
 
 
 v6.0.1 (2023-02-20)
@@ -1274,14 +1283,16 @@
 .. _efenka: https://github.com/efenka
 .. _jwilson8767: https://github.com/jwilson8767
 .. _elijose55: https://github.com/elijose55
 .. _gonzalonaveira: https://github.com/gonzalonaveira
 .. _zhaowb: https://github.com/zhaowb
 .. _mervynlee94: https://github.com/mervynlee94
 .. _weineel: https://github.com/weineel
+.. _bl4ckst0ne: https://github.com/bl4ckst0ne
+.. _DeviousStoat: https://github.com/DeviousStoat
 
 MIT License
 
 Copyright (c) 2020 Derrick Gilland
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pydash-6.0.2/tests/helpers.py` & `pydash-7.0.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/tests/test_arrays.py` & `pydash-7.0.0/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/tests/test_chaining.py` & `pydash-7.0.0/tests/test_chaining.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 
 def test_chaining_plant():
     value = [1, 2, 3, 4]
     square_sum1 = _.chain(value).power(2).sum()
 
     def root_value(wrapper):
-        if isinstance(wrapper._value, _.chaining.ChainWrapper):
+        if isinstance(wrapper._value, _.chaining.chaining.ChainWrapper):
             return root_value(wrapper._value)
         return wrapper._value
 
     assert root_value(square_sum1._value) == value
 
     test_value = [5, 6, 7, 8]
     square_sum2 = square_sum1.plant(test_value)
```

### Comparing `pydash-6.0.2/tests/test_collections.py` & `pydash-7.0.0/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/tests/test_functions.py` & `pydash-7.0.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/tests/test_numerical.py` & `pydash-7.0.0/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/tests/test_objects.py` & `pydash-7.0.0/tests/test_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from . import helpers
 
 
 parametrize = pytest.mark.parametrize
 
 today = dt.date.today()
 
+SomeNamedTuple = namedtuple("SomeNamedTuple", ["a", "b"])
+
 
 @parametrize(
     "case,expected",
     [
         (({"name": "fred"}, {"employer": "slate"}), {"name": "fred", "employer": "slate"}),
         (
             ({"name": "fred"}, {"employer": "slate"}, {"employer": "medium"}),
@@ -344,27 +346,29 @@
         (({"one": {"two": {"three": [{"a": 1}]}}}, "one.four.three.0.a", "haha"), "haha"),
         (({"one": {"two": {"three": 4}}}, "five"), None),
         (({"one": ["two", {"three": [4, 5]}]}, ["one", 1, "three", 1]), 5),
         (({"one": ["two", {"three": [4, 5]}]}, "one.[1].three.[1]"), 5),
         (({"one": ["two", {"three": [4, 5]}]}, "one.1.three.1"), 5),
         ((["one", {"two": {"three": [4, 5]}}], "[1].two.three.[0]"), 4),
         ((["one", {"two": {"three": [4, [{"four": [5]}]]}}], "[1].two.three[1][0].four[0]"), 5),
+        ((["one", {"two": {"three": [4, [{"four": [5]}], 6]}}], "[1].two.three[-2][0].four[0]"), 5),
         ((range(50), "[42]"), 42),
+        ((range(50), "[-1]"), 49),
         (([[[[[[[[[[42]]]]]]]]]], "[0][0][0][0][0][0][0][0][0][0]"), 42),
         (([range(50)], "[0][42]"), 42),
         (({"a": [{"b": range(50)}]}, "a[0].b[42]"), 42),
         (
             ({"lev.el1": {"lev\\el2": {"level3": ["value"]}}}, "lev\\.el1.lev\\\\el2.level3.[0]"),
             "value",
         ),
         (({"one": ["hello", "there"]}, "one.bad.hello", []), []),
         (({"one": ["hello", None]}, "one.1.hello"), None),
-        ((namedtuple("a", ["a", "b"])(1, 2), "a"), 1),
-        ((namedtuple("a", ["a", "b"])(1, 2), 0), 1),
-        ((namedtuple("a", ["a", "b"])({"c": {"d": 1}}, 2), "a.c.d"), 1),
+        ((SomeNamedTuple(1, 2), "a"), 1),
+        ((SomeNamedTuple(1, 2), 0), 1),
+        ((SomeNamedTuple({"c": {"d": 1}}, 2), "a.c.d"), 1),
         (({}, "update"), None),
         (([], "extend"), None),
         (({(1,): {(2,): 3}}, (1,)), {(2,): 3}),
         (({(1,): {(2,): 3}}, [(1,), (2,)]), 3),
         (({object: 1}, object), 1),
         (({object: {object: 1}}, [object, object]), 1),
         (({1: {"name": "John Doe"}}, "1.name"), "John Doe"),
@@ -381,15 +385,15 @@
     assert data == {}
 
 
 @parametrize(
     "obj,path",
     [
         (helpers.Object(), "__init__.__globals__"),
-        (namedtuple("a", ["a"])(a=1), "__globals__"),
+        (SomeNamedTuple(1, 2), "__globals__"),
         (helpers.Object(subobj=helpers.Object()), "subobj.__builtins__"),
         (helpers.Object(subobj=helpers.Object()), "__builtins__"),
     ],
 )
 def test_get__raises_for_objects_when_path_restricted(obj, path):
     with pytest.raises(KeyError, match="access to restricted key"):
         _.get(obj, path)
```

### Comparing `pydash-6.0.2/tests/test_predicates.py` & `pydash-7.0.0/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-6.0.2/tests/test_strings.py` & `pydash-7.0.0/tests/test_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -784,15 +784,16 @@
 
 
 @parametrize(
     "case,expected",
     [
         ("Foo Bar", "foo-bar"),
         (" foo bar ", "foo-bar"),
-        ("Un éléphant à l'orée du bois", "un-elephant-a-l-oree-du-bois"),
+        ("Un éléphant à l'orée du bois", "un-elephant-a-loree-du-bois"),
+        ("shouldn't couldn't wouldn't", "shouldnt-couldnt-wouldnt"),
         ("", ""),
         (5, "5"),
         (None, ""),
     ],
 )
 def test_slugify(case, expected):
     assert _.slugify(case) == expected
```

### Comparing `pydash-6.0.2/tests/test_utilities.py` & `pydash-7.0.0/tests/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,14 +617,16 @@
 
 @parametrize(
     "case,expected",
     [
         ("a.b.c", ["a", "b", "c"]),
         ("a[0].b.c", ["a", 0, "b", "c"]),
         ("a[0][1][2].b.c", ["a", 0, 1, 2, "b", "c"]),
+        ("a[0][1][2].b.c", ["a", 0, 1, 2, "b", "c"]),
+        ("a[0][-1][-2].b.c", ["a", 0, -1, -2, "b", "c"]),
     ],
 )
 def test_to_path(case, expected):
     assert _.to_path(case) == expected
 
 
 def test_unique_id_setup():
```

