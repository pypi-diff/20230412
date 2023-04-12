# Comparing `tmp/laue_dials-0.1.3.tar.gz` & `tmp/laue_dials-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laue_dials-0.1.3.tar", last modified: Tue Mar 28 20:22:20 2023, max compression
+gzip compressed data, was "laue_dials-0.1.4.tar", last modified: Wed Apr 12 05:54:53 2023, max compression
```

## Comparing `laue_dials-0.1.3.tar` & `laue_dials-0.1.4.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.812361 laue_dials-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.820361 laue_dials-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-28 20:20:24.000000 laue_dials-0.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-28 20:20:24.000000 laue_dials-0.1.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-28 20:20:24.000000 laue_dials-0.1.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-03-28 20:20:24.000000 laue_dials-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-28 20:20:24.000000 laue_dials-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-28 20:22:20.824361 laue_dials-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-28 20:20:24.000000 laue_dials-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.820361 laue_dials-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.820361 laue_dials-0.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/api/laue_dials.algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/api/laue_dials.command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/api/laue_dials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/api/laue_dials.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-28 20:20:24.000000 laue_dials-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-28 20:20:24.000000 laue_dials-0.1.3/examples/initial_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-28 20:20:24.000000 laue_dials-0.1.3/examples/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-28 20:20:24.000000 laue_dials-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-28 20:22:20.824361 laue_dials-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-28 20:20:24.000000 laue_dials-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.812361 laue_dials-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/src/laue_dials/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/src/laue_dials/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/algorithms/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/algorithms/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/src/laue_dials/command_line/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/command_line/initial_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/command_line/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/command_line/optimize_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/command_line/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/command_line/refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/src/laue_dials/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/utils/expt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-28 20:20:24.000000 laue_dials-0.1.3/src/laue_dials/utils/refl_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/src/laue_dials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-28 20:22:20.000000 laue_dials-0.1.3/src/laue_dials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-28 20:22:20.000000 laue_dials-0.1.3/src/laue_dials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:22:20.000000 laue_dials-0.1.3/src/laue_dials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-28 20:22:20.000000 laue_dials-0.1.3/src/laue_dials.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:22:20.000000 laue_dials-0.1.3/src/laue_dials.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-28 20:22:20.000000 laue_dials-0.1.3/src/laue_dials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-28 20:22:20.000000 laue_dials-0.1.3/src/laue_dials.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:22:20.824361 laue_dials-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-28 20:20:24.000000 laue_dials-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-28 20:20:24.000000 laue_dials-0.1.3/tests/test_initial_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-28 20:20:24.000000 laue_dials-0.1.3/tests/test_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-28 20:20:24.000000 laue_dials-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.039720 laue_dials-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.047720 laue_dials-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 05:52:37.000000 laue_dials-0.1.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 05:52:37.000000 laue_dials-0.1.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-12 05:52:37.000000 laue_dials-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 05:52:37.000000 laue_dials-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 05:54:53.055720 laue_dials-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-12 05:52:37.000000 laue_dials-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.047720 laue_dials-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.047720 laue_dials-0.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 05:52:37.000000 laue_dials-0.1.4/examples/initial_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 05:52:37.000000 laue_dials-0.1.4/examples/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 05:52:37.000000 laue_dials-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-12 05:54:53.059721 laue_dials-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 05:52:37.000000 laue_dials-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.039720 laue_dials-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/src/laue_dials/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/src/laue_dials/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/algorithms/diffgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/algorithms/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/algorithms/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/src/laue_dials/command_line/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/initial_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/optimize_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/src/laue_dials/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/utils/expt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/utils/refl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/src/laue_dials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/algorithms/test_diffgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/algorithms/test_laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/test_initial_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/test_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tox.ini
```

### Comparing `laue_dials-0.1.3/.coveragerc` & `laue_dials-0.1.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/.github/workflows/build.yml` & `laue_dials-0.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/.github/workflows/docs.yml` & `laue_dials-0.1.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/.github/workflows/format.yml` & `laue_dials-0.1.4/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/.gitignore` & `laue_dials-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/.readthedocs.yml` & `laue_dials-0.1.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/CONTRIBUTING.rst` & `laue_dials-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/LICENSE.txt` & `laue_dials-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/PKG-INFO` & `laue_dials-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laue_dials
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for analyzing Laue x-ray crystallography data using the DIALS framework.
 Home-page: https://github.com/rs-station/laue_dials
 Author: Rick A. Hewitt
 Author-email: rahewitt@g.harvard.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laue_dials-0.1.3/README.rst` & `laue_dials-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/docs/Makefile` & `laue_dials-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/docs/api/laue_dials.command_line.rst` & `laue_dials-0.1.4/docs/api/laue_dials.command_line.rst`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/docs/api/laue_dials.utils.rst` & `laue_dials-0.1.4/docs/api/laue_dials.utils.rst`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/docs/conf.py` & `laue_dials-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/docs/index.rst` & `laue_dials-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/setup.cfg` & `laue_dials-0.1.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
 	laue.initial_solution = laue_dials.command_line.initial_solution:dials_version
-	laue.optimize_indexing = laue_dials.command_line.optimize_indexing:index_image
+	laue.optimize_indexing = laue_dials.command_line.optimize_indexing:run
 	laue.refine = laue_dials.command_line.refine:refine_geometry
 	laue.predict = laue_dials.command_line.predict:predict_spots
 	laue.integrate = laue_dials.command_line.integrate:integrate_dataset
 
 [tool:pytest]
 addopts = 
 	--cov laue_dials --cov-report xml
```

### Comparing `laue_dials-0.1.3/setup.py` & `laue_dials-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/src/laue_dials/__init__.py` & `laue_dials-0.1.4/src/laue_dials/__init__.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/src/laue_dials/skeleton.py` & `laue_dials-0.1.4/src/laue_dials/skeleton.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/src/laue_dials.egg-info/PKG-INFO` & `laue_dials-0.1.4/src/laue_dials.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laue-dials
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for analyzing Laue x-ray crystallography data using the DIALS framework.
 Home-page: https://github.com/rs-station/laue_dials
 Author: Rick A. Hewitt
 Author-email: rahewitt@g.harvard.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laue_dials-0.1.3/src/laue_dials.egg-info/SOURCES.txt` & `laue_dials-0.1.4/src/laue_dials.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,23 @@
 src/laue_dials.egg-info/PKG-INFO
 src/laue_dials.egg-info/SOURCES.txt
 src/laue_dials.egg-info/dependency_links.txt
 src/laue_dials.egg-info/entry_points.txt
 src/laue_dials.egg-info/not-zip-safe
 src/laue_dials.egg-info/requires.txt
 src/laue_dials.egg-info/top_level.txt
+src/laue_dials/algorithms/diffgeo.py
 src/laue_dials/algorithms/laue.py
 src/laue_dials/algorithms/outliers.py
 src/laue_dials/command_line/initial_solution.py
 src/laue_dials/command_line/integrate.py
 src/laue_dials/command_line/optimize_indexing.py
 src/laue_dials/command_line/predict.py
 src/laue_dials/command_line/refine.py
 src/laue_dials/utils/expt_utils.py
 src/laue_dials/utils/plots.py
 src/laue_dials/utils/refl_utils.py
 tests/conftest.py
 tests/test_initial_solution.py
-tests/test_skeleton.py
+tests/test_skeleton.py
+tests/algorithms/test_diffgeo.py
+tests/algorithms/test_laue.py
```

### Comparing `laue_dials-0.1.3/tests/test_skeleton.py` & `laue_dials-0.1.4/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.3/tox.ini` & `laue_dials-0.1.4/tox.ini`

 * *Files identical despite different names*

