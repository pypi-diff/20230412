# Comparing `tmp/etos_test_runner-2.5.0.tar.gz` & `tmp/etos_test_runner-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_test_runner-2.5.0.tar", last modified: Mon Apr  3 08:17:10 2023, max compression
+gzip compressed data, was "etos_test_runner-3.0.0.tar", last modified: Wed Apr 12 11:04:19 2023, max compression
```

## Comparing `etos_test_runner-2.5.0.tar` & `etos_test_runner-3.0.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/
--rw-r--r--   0 fredjn    (9531) axusers    (500)      599 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/.coveragerc
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.041558 etos_test_runner-2.5.0/.github/
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.045558 etos_test_runner-2.5.0/.github/workflows/
--rw-r--r--   0 fredjn    (9531) axusers    (500)      850 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/.github/workflows/main.yml
--rw-r--r--   0 fredjn    (9531) axusers    (500)      408 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/.gitignore
--rw-r--r--   0 fredjn    (9531) axusers    (500)        5 2023-03-29 17:59:55.000000 etos_test_runner-2.5.0/.python-version
--rw-r--r--   0 fredjn    (9531) axusers    (500)      174 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/AUTHORS.rst
--rw-r--r--   0 fredjn    (9531) axusers    (500)       37 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/CODEOWNERS
--rw-r--r--   0 fredjn    (9531) axusers    (500)    10850 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/LICENSE.txt
--rw-r--r--   0 fredjn    (9531) axusers    (500)     1420 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/PKG-INFO
--rw-r--r--   0 fredjn    (9531) axusers    (500)      814 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/README.rst
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.045558 etos_test_runner-2.5.0/docs/
--rw-r--r--   0 fredjn    (9531) axusers    (500)     7626 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/Makefile
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.045558 etos_test_runner-2.5.0/docs/_static/
--rw-r--r--   0 fredjn    (9531) axusers    (500)       18 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/_static/.gitignore
--rw-r--r--   0 fredjn    (9531) axusers    (500)       41 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/authors.rst
--rw-r--r--   0 fredjn    (9531) axusers    (500)       43 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/changelog.rst
--rw-r--r--   0 fredjn    (9531) axusers    (500)     9209 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/conf.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)      472 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/index.rst
--rw-r--r--   0 fredjn    (9531) axusers    (500)       74 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/license.rst
--rw-r--r--   0 fredjn    (9531) axusers    (500)       39 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/readme.rst
--rw-r--r--   0 fredjn    (9531) axusers    (500)       59 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/docs/requirements.txt
--rw-r--r--   0 fredjn    (9531) axusers    (500)       58 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/pylintrc
--rw-r--r--   0 fredjn    (9531) axusers    (500)      698 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/requirements.txt
--rw-r--r--   0 fredjn    (9531) axusers    (500)     1408 2023-04-03 08:17:10.053558 etos_test_runner-2.5.0/setup.cfg
--rw-r--r--   0 fredjn    (9531) axusers    (500)      560 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/setup.py
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.045558 etos_test_runner-2.5.0/src/
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/src/etos_test_runner/
--rw-r--r--   0 fredjn    (9531) axusers    (500)     1079 2023-03-29 12:58:10.000000 etos_test_runner-2.5.0/src/etos_test_runner/__init__.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)     5339 2023-03-30 09:57:56.000000 etos_test_runner-2.5.0/src/etos_test_runner/etr.py
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/src/etos_test_runner/lib/
--rw-r--r--   0 fredjn    (9531) axusers    (500)      705 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/__init__.py
--rwxr-xr-x   0 fredjn    (9531) axusers    (500)      678 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/checkout.sh
--rwxr-xr-x   0 fredjn    (9531) axusers    (500)      678 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/environ.sh
--rw-r--r--   0 fredjn    (9531) axusers    (500)    15529 2023-03-30 10:00:10.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/executor.py
--rwxr-xr-x   0 fredjn    (9531) axusers    (500)     1022 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/executor.sh
--rw-r--r--   0 fredjn    (9531) axusers    (500)     3938 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/iut.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)     4883 2023-03-30 09:57:37.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/iut_monitoring.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)    12679 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/log_area.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)    10057 2023-03-30 09:58:27.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/testrunner.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)     7408 2023-03-30 09:49:22.000000 etos_test_runner-2.5.0/src/etos_test_runner/lib/workspace.py
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/src/etos_test_runner/plugins/
--rw-r--r--   0 fredjn    (9531) axusers    (500)     1033 2023-01-27 16:48:06.000000 etos_test_runner-2.5.0/src/etos_test_runner/plugins/__init__.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)     3737 2023-01-27 16:48:06.000000 etos_test_runner-2.5.0/src/etos_test_runner/plugins/plugin.py
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/src/etos_test_runner.egg-info/
--rw-r--r--   0 fredjn    (9531) axusers    (500)     1420 2023-04-03 08:17:09.000000 etos_test_runner-2.5.0/src/etos_test_runner.egg-info/PKG-INFO
--rw-r--r--   0 fredjn    (9531) axusers    (500)     1417 2023-04-03 08:17:09.000000 etos_test_runner-2.5.0/src/etos_test_runner.egg-info/SOURCES.txt
--rw-r--r--   0 fredjn    (9531) axusers    (500)        1 2023-04-03 08:17:09.000000 etos_test_runner-2.5.0/src/etos_test_runner.egg-info/dependency_links.txt
--rw-r--r--   0 fredjn    (9531) axusers    (500)        1 2023-03-29 13:31:39.000000 etos_test_runner-2.5.0/src/etos_test_runner.egg-info/not-zip-safe
--rw-r--r--   0 fredjn    (9531) axusers    (500)       85 2023-04-03 08:17:09.000000 etos_test_runner-2.5.0/src/etos_test_runner.egg-info/requires.txt
--rw-r--r--   0 fredjn    (9531) axusers    (500)       32 2023-04-03 08:17:09.000000 etos_test_runner-2.5.0/src/etos_test_runner.egg-info/top_level.txt
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/src/etr_send_event/
--rw-r--r--   0 fredjn    (9531) axusers    (500)     4894 2023-01-27 16:48:06.000000 etos_test_runner-2.5.0/src/etr_send_event/__init__.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)       27 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/test-requirements.txt
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/tests/
--rw-r--r--   0 fredjn    (9531) axusers    (500)      696 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/tests/__init__.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)     1282 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/tests/conftest.py
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/tests/lib/
--rw-r--r--   0 fredjn    (9531) axusers    (500)      694 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/tests/lib/__init__.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)    16120 2023-03-29 19:57:36.000000 etos_test_runner-2.5.0/tests/lib/test_iut_monitoring.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)    11332 2023-03-30 09:59:20.000000 etos_test_runner-2.5.0/tests/lib/test_workspace.py
-drwxr-xr-x   0 fredjn    (9531) axusers    (500)        0 2023-04-03 08:17:10.049558 etos_test_runner-2.5.0/tests/scenarios/
--rw-r--r--   0 fredjn    (9531) axusers    (500)      925 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/tests/scenarios/__init__.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)     7988 2023-01-27 16:48:06.000000 etos_test_runner-2.5.0/tests/scenarios/test_full_execution.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)    19588 2023-01-27 16:48:06.000000 etos_test_runner-2.5.0/tests/scenarios/test_log_upload.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)     6895 2023-01-27 16:48:06.000000 etos_test_runner-2.5.0/tests/scenarios/test_no_detected_test_name.py
--rw-r--r--   0 fredjn    (9531) axusers    (500)      900 2022-08-17 09:28:26.000000 etos_test_runner-2.5.0/tox.ini
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.833995 etos_test_runner-3.0.0/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      599 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/.coveragerc
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/.github/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/.github/workflows/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/.github/workflows/main.yml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      408 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/AUTHORS.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/CODEOWNERS
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/LICENSE.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1418 2023-04-12 11:04:19.833995 etos_test_runner-3.0.0/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      814 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/README.rst
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/docs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7626 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/Makefile
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/docs/_static/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/_static/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/authors.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/changelog.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     9209 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/conf.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      472 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/index.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/license.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/readme.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/docs/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       58 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/pylintrc
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      698 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1408 2023-04-12 11:04:19.833995 etos_test_runner-3.0.0/setup.cfg
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      560 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/setup.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/src/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/src/etos_test_runner/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1079 2023-04-12 08:00:56.000000 etos_test_runner-3.0.0/src/etos_test_runner/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5544 2023-04-12 11:03:34.000000 etos_test_runner-3.0.0/src/etos_test_runner/etr.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/src/etos_test_runner/lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      705 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/__init__.py
+-rwxr-xr-x   0 tobiaspn (21118) axusers    (500)      678 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/checkout.sh
+-rwxr-xr-x   0 tobiaspn (21118) axusers    (500)      678 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/environ.sh
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    15529 2023-04-12 08:00:56.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/executor.py
+-rwxr-xr-x   0 tobiaspn (21118) axusers    (500)     1022 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/executor.sh
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3938 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/iut.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4883 2023-04-12 08:00:56.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/iut_monitoring.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    12679 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/log_area.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10151 2023-04-12 11:03:32.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/testrunner.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7408 2023-04-12 08:00:56.000000 etos_test_runner-3.0.0/src/etos_test_runner/lib/workspace.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/src/etos_test_runner/plugins/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1033 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner/plugins/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3787 2023-04-12 11:03:32.000000 etos_test_runner-3.0.0/src/etos_test_runner/plugins/plugin.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/src/etos_test_runner.egg-info/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1418 2023-04-12 11:04:19.000000 etos_test_runner-3.0.0/src/etos_test_runner.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1401 2023-04-12 11:04:19.000000 etos_test_runner-3.0.0/src/etos_test_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-04-12 11:04:19.000000 etos_test_runner-3.0.0/src/etos_test_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etos_test_runner.egg-info/not-zip-safe
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       85 2023-04-12 11:04:19.000000 etos_test_runner-3.0.0/src/etos_test_runner.egg-info/requires.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       32 2023-04-12 11:04:19.000000 etos_test_runner-3.0.0/src/etos_test_runner.egg-info/top_level.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/src/etr_send_event/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4894 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/src/etr_send_event/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       27 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/test-requirements.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/tests/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      696 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tests/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1282 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tests/conftest.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.829995 etos_test_runner-3.0.0/tests/lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      694 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tests/lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    16120 2023-04-12 08:00:56.000000 etos_test_runner-3.0.0/tests/lib/test_iut_monitoring.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    11332 2023-04-12 08:00:56.000000 etos_test_runner-3.0.0/tests/lib/test_workspace.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-04-12 11:04:19.833995 etos_test_runner-3.0.0/tests/scenarios/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      925 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tests/scenarios/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7988 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tests/scenarios/test_full_execution.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    19588 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tests/scenarios/test_log_upload.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     6895 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tests/scenarios/test_no_detected_test_name.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      900 2023-03-09 08:23:58.000000 etos_test_runner-3.0.0/tox.ini
```

### Comparing `etos_test_runner-2.5.0/.coveragerc` & `etos_test_runner-3.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/.github/workflows/main.yml` & `etos_test_runner-3.0.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/LICENSE.txt` & `etos_test_runner-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/PKG-INFO` & `etos_test_runner-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_test_runner
-Version: 2.5.0
+Version: 3.0.0
 Summary: ETOS Test Runner
 Home-page: https://github.com/eiffel-community/etos-test-runner
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -47,9 +47,7 @@
 
 
 Support
 =======
 
 If you are having issues, please let us know.
 There is a mailing list at: etos-maintainers@googlegroups.com or just write an Issue.
-
-
```

### Comparing `etos_test_runner-2.5.0/README.rst` & `etos_test_runner-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/docs/Makefile` & `etos_test_runner-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/docs/conf.py` & `etos_test_runner-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/requirements.txt` & `etos_test_runner-3.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/setup.cfg` & `etos_test_runner-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/setup.py` & `etos_test_runner-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/__init__.py` & `etos_test_runner-3.0.0/src/etos_test_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/etr.py` & `etos_test_runner-3.0.0/src/etos_test_runner/etr.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,18 +99,23 @@
         """
         iut = Iut(self.etos.config.get("test_config").get("iut"))
         test_runner = TestRunner(iut, self.etos)
         return test_runner.execute()
 
     def load_plugins(self):
         """Load plugins from environment using the name etr_."""
+        disable_plugins = os.getenv("DISABLE_PLUGINS")
+        disabled_plugins = []
+        if disable_plugins:
+            disabled_plugins = disable_plugins.split(",")
+
         discovered_plugins = {
             name: importlib.import_module(name)
             for _, name, _ in pkgutil.iter_modules()
-            if name.startswith("etr_")
+            if name.startswith("etr_") and name not in disabled_plugins
         }
         plugins = []
         for name, module in discovered_plugins.items():
             _LOGGER.info("Loading plugin: %r", name)
             if not hasattr(module, "ETRPlugin"):
                 raise AttributeError(f"{name} does not have an ETRPlugin class!")
             plugins.append(module.ETRPlugin(self.etos))
```

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/__init__.py` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/checkout.sh` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/checkout.sh`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/environ.sh` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/environ.sh`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/executor.py` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/executor.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/executor.sh` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/executor.sh`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/iut.py` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/iut.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/iut_monitoring.py` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/iut_monitoring.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/log_area.py` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/testrunner.py` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/testrunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,22 +162,22 @@
 
         :param name: Name of test suite that triggered.
         :type name: str
         """
         for plugin in self.plugins:
             plugin.on_test_suite_triggered(name)
 
-    def _test_suite_started(self, name):
+    def _test_suite_started(self, test_suite_started):
         """Call on_test_suite_started for all ETR plugins.
 
-        :param name: Name of test suite that finished.
-        :type name: str
+        :param test_suite_started: The test suite started event
+        :type test_suite_started: :obj:`eiffellib.events.EiffelTestSuiteStartedEvent`
         """
         for plugin in self.plugins:
-            plugin.on_test_suite_started(name)
+            plugin.on_test_suite_started(test_suite_started)
 
     def _test_suite_finished(self, name, outcome):
         """Call on_test_suite_finished for all ETR plugins.
 
         :param name: Name of test suite that finished.
         :type name: str
         :param outcome: Outcome of test suite execution.
@@ -190,16 +190,16 @@
         """Execute all tests in test suite.
 
         :return: Result of execution. Linux exit code.
         :rtype: int
         """
         self._test_suite_triggered(self.config.get("name"))
         self.logger.info("Send test suite started event.")
-        self._test_suite_started(self.config.get("name"))
         test_suite_started = self.test_suite_started()
+        self._test_suite_started(test_suite_started)
         sub_suite_id = test_suite_started.meta.event_id
 
         self.logger.info("Send test environment events.")
         self.environment(sub_suite_id)
         self.etos.config.set("sub_suite_id", sub_suite_id)
 
         result = True
```

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/lib/workspace.py` & `etos_test_runner-3.0.0/src/etos_test_runner/lib/workspace.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/plugins/__init__.py` & `etos_test_runner-3.0.0/src/etos_test_runner/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner/plugins/plugin.py` & `etos_test_runner-3.0.0/src/etos_test_runner/plugins/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     def on_test_suite_triggered(self, test_suite_name):
         """Call when a test suite has been triggered.
 
         :param test_suite_name: Name of test suite that has been triggered.
         :type test_suite_name: str
         """
 
-    def on_test_suite_started(self, test_suite_name):
+    def on_test_suite_started(self, test_suite_started):
         """Call when a test suite has started.
 
-        :param test_suite_name: Name of test suite that has started.
-        :type test_suite_name: str
+        :param test_suite_started: The test suite started event.
+        :type test_suite_started: :obj:`eiffellib.events.EiffelTestSuiteStartedEvent`
         """
 
     def on_test_suite_finished(self, test_suite_name, outcome):
         """Call when a test suite has finished.
 
         :param test_suite_name: Name of test suite that has finished.
         :type test_suite_name: str
```

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner.egg-info/PKG-INFO` & `etos_test_runner-3.0.0/src/etos_test_runner.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos-test-runner
-Version: 2.5.0
+Version: 3.0.0
 Summary: ETOS Test Runner
 Home-page: https://github.com/eiffel-community/etos-test-runner
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -47,9 +47,7 @@
 
 
 Support
 =======
 
 If you are having issues, please let us know.
 There is a mailing list at: etos-maintainers@googlegroups.com or just write an Issue.
-
-
```

### Comparing `etos_test_runner-2.5.0/src/etos_test_runner.egg-info/SOURCES.txt` & `etos_test_runner-3.0.0/src/etos_test_runner.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .coveragerc
 .gitignore
-.python-version
 AUTHORS.rst
 CODEOWNERS
 LICENSE.txt
 README.rst
 pylintrc
 requirements.txt
 setup.cfg
```

### Comparing `etos_test_runner-2.5.0/src/etr_send_event/__init__.py` & `etos_test_runner-3.0.0/src/etr_send_event/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/__init__.py` & `etos_test_runner-3.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/conftest.py` & `etos_test_runner-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/lib/__init__.py` & `etos_test_runner-3.0.0/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/lib/test_iut_monitoring.py` & `etos_test_runner-3.0.0/tests/lib/test_iut_monitoring.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/lib/test_workspace.py` & `etos_test_runner-3.0.0/tests/lib/test_workspace.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/scenarios/__init__.py` & `etos_test_runner-3.0.0/tests/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/scenarios/test_full_execution.py` & `etos_test_runner-3.0.0/tests/scenarios/test_full_execution.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/scenarios/test_log_upload.py` & `etos_test_runner-3.0.0/tests/scenarios/test_log_upload.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tests/scenarios/test_no_detected_test_name.py` & `etos_test_runner-3.0.0/tests/scenarios/test_no_detected_test_name.py`

 * *Files identical despite different names*

### Comparing `etos_test_runner-2.5.0/tox.ini` & `etos_test_runner-3.0.0/tox.ini`

 * *Files identical despite different names*

