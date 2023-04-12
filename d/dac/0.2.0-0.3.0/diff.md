# Comparing `tmp/dac-0.2.0.tar.gz` & `tmp/dac-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dac-0.2.0.tar", last modified: Mon Feb 27 10:08:09 2023, max compression
+gzip compressed data, was "dac-0.3.0.tar", last modified: Wed Apr 12 12:22:14 2023, max compression
```

## Comparing `dac-0.2.0.tar` & `dac-0.3.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.713947 dac-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.701942 dac-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.705944 dac-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-02-27 10:07:49.000000 dac-0.2.0/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-27 10:07:49.000000 dac-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-27 10:07:49.000000 dac-0.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-27 10:07:49.000000 dac-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-27 10:07:49.000000 dac-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-27 10:07:49.000000 dac-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-27 10:08:09.713947 dac-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-02-27 10:07:49.000000 dac-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.705944 dac-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-27 10:07:49.000000 dac-0.2.0/docs/examples.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.705944 dac-0.2.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   206100 2023-02-27 10:07:49.000000 dac-0.2.0/docs/img/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-02-27 10:07:49.000000 dac-0.2.0/docs/img/motto.png
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-02-27 10:07:49.000000 dac-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-27 10:07:49.000000 dac-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-27 10:07:49.000000 dac-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-27 10:07:49.000000 dac-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-27 10:07:49.000000 dac-0.2.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-27 10:07:49.000000 dac-0.2.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 10:08:09.713947 dac-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.705944 dac-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.705944 dac-0.2.0/src/dac/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/_file_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/src/dac/_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/_input/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/_input/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-02-27 10:07:49.000000 dac-0.2.0/src/dac/_pyproject_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/src/dac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-27 10:08:09.000000 dac-0.2.0/src/dac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-27 10:08:09.000000 dac-0.2.0/src/dac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 10:08:09.000000 dac-0.2.0/src/dac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-27 10:08:09.000000 dac-0.2.0/src/dac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-27 10:08:09.000000 dac-0.2.0/src/dac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-27 10:08:09.000000 dac-0.2.0/src/dac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-02-27 10:07:49.000000 dac-0.2.0/test/cli_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-02-27 10:07:49.000000 dac-0.2.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/data/load/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/load/missing_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/load/missing_load_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/load/missing_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/load/parquet_as_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/load/return_wrong_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/load/self_contained_as_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/pack_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/data/parquet/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/parquet/sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/data/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/requirements/parquet_as_pandas.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/data/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/schema/incompatible_with_sample_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/schema/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/schema/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/schema/self_contained.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-27 10:07:49.000000 dac-0.2.0/test/data/schema/wrong_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/integration_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/integration_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-02-27 10:07:49.000000 dac-0.2.0/test/integration_test/pack_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/unit_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/unit_test/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_cli/help_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_cli/info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_cli/pack_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.709945 dac-0.2.0/test/unit_test/_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_input/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_input/pyproject_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 10:08:09.713947 dac-0.2.0/test/unit_test/_packing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_packing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_packing/build_wheel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_packing/data_as_code_project_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-27 10:07:49.000000 dac-0.2.0/test/unit_test/_packing/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.780995 dac-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.756995 dac-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-12 12:21:44.000000 dac-0.3.0/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 12:21:44.000000 dac-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 12:21:44.000000 dac-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-12 12:21:44.000000 dac-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-12 12:21:44.000000 dac-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 12:21:44.000000 dac-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-12 12:22:14.776996 dac-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-12 12:21:44.000000 dac-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-12 12:21:44.000000 dac-0.3.0/docs/examples.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   206100 2023-04-12 12:21:44.000000 dac-0.3.0/docs/img/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-04-12 12:21:44.000000 dac-0.3.0/docs/img/motto.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-12 12:21:44.000000 dac-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 12:21:44.000000 dac-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-12 12:21:44.000000 dac-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 12:21:44.000000 dac-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 12:21:44.000000 dac-0.3.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 12:21:44.000000 dac-0.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:22:14.780995 dac-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.756995 dac-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/src/dac/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_file_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.768995 dac-0.3.0/src/dac/_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_input/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_input/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_pyproject_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.768995 dac-0.3.0/src/dac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.768995 dac-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 12:21:44.000000 dac-0.3.0/test/cli_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-12 12:21:44.000000 dac-0.3.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/load/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/missing_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/missing_load_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/missing_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/parquet_as_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/return_wrong_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/self_contained_as_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/pack_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/parquet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/parquet/sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/requirements/parquet_as_pandas.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/incompatible_with_sample_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/self_contained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/wrong_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/integration_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-12 12:21:44.000000 dac-0.3.0/test/integration_test/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/help_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_input/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_input/pyproject_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/_packing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/build_wheel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/data_as_code_project_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/pack_test.py
```

### Comparing `dac-0.2.0/.github/workflows/actions.yml` & `dac-0.3.0/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/.gitlab-ci.yml` & `dac-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/.pre-commit-config.yaml` & `dac-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/CHANGELOG.md` & `dac-0.3.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,10 +5,15 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 **IMPORTANT**: Currently the project is in the initial development phase, this is why releases are marked as `0.z.y`.
 (following [semantic versioning 2.0.0](https://semver.org/): "Major version zero (0.y.z) is for initial development.
 Anything MAY change at any time. The public API SHOULD NOT be considered stable.").
 While in this phase, we will denote breaking changes with a minor increase.
 
+
+## 0.3.0
+### Changed
+* Dependencies passed in CLI `--pkg-dependencies` or `PyProjectConfig` must be separated by `;` or newline (previously was `,` or newline)
+
 ## 0.2.0
 ### Added
 * First release of `dac`
```

### Comparing `dac-0.2.0/LICENSE` & `dac-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/PKG-INFO` & `dac-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dac
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tool to distribute data as code
 Author-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 License: MIT
 Project-URL: homepage, https://data-as-code.github.io/dac/
 Project-URL: documentation, https://data-as-code.github.io/dac/
 Project-URL: repository, https://github.com/data-as-code/dac
```

### Comparing `dac-0.2.0/README.md` & `dac-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/docs/img/logo.jpg` & `dac-0.3.0/docs/img/logo.jpg`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/docs/img/motto.png` & `dac-0.3.0/docs/img/motto.png`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/docs/index.md` & `dac-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/mkdocs.yml` & `dac-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/pyproject.toml` & `dac-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -49,7 +49,10 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 120
+
+[tool.ruff]
+line-length = 120
```

### Comparing `dac-0.2.0/src/dac/_cli.py` & `dac-0.3.0/src/dac/_cli.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/src/dac/_input/config.py` & `dac-0.3.0/src/dac/_input/config.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/src/dac/_input/pyproject.py` & `dac-0.3.0/src/dac/_input/pyproject.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
                     "dependencies": self._get_list_of_project_dependencies(),
                 }
             }
         )
 
     def _get_list_of_project_dependencies(self) -> List[str]:
         splitted_by_newline = self.project_dependencies.splitlines()
-        splitted_by_newline_or_comma = [s for ss in splitted_by_newline for s in ss.split(",")]
+        splitted_by_newline_or_comma = [s for ss in splitted_by_newline for s in ss.split(";")]
         return sorted(map(lambda x: x.strip(), splitted_by_newline_or_comma))
```

### Comparing `dac-0.2.0/src/dac/_packing.py` & `dac-0.3.0/src/dac/_packing.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/src/dac/_pyproject_factory.py` & `dac-0.3.0/src/dac/_pyproject_factory.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/src/dac.egg-info/PKG-INFO` & `dac-0.3.0/src/dac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dac
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tool to distribute data as code
 Author-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 License: MIT
 Project-URL: homepage, https://data-as-code.github.io/dac/
 Project-URL: documentation, https://data-as-code.github.io/dac/
 Project-URL: repository, https://github.com/data-as-code/dac
```

### Comparing `dac-0.2.0/src/dac.egg-info/SOURCES.txt` & `dac-0.3.0/src/dac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/cli_utilities.py` & `dac-0.3.0/test/cli_utilities.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/conftest.py` & `dac-0.3.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/data/__init__.py` & `dac-0.3.0/test/data/__init__.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/data/pack_input.py` & `dac-0.3.0/test/data/pack_input.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/data/parquet/sample.parquet` & `dac-0.3.0/test/data/parquet/sample.parquet`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/integration_test/pack_test.py` & `dac-0.3.0/test/integration_test/pack_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/unit_test/_cli/pack_test.py` & `dac-0.3.0/test/unit_test/_cli/pack_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/unit_test/_input/config_test.py` & `dac-0.3.0/test/unit_test/_input/config_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/unit_test/_input/pyproject_test.py` & `dac-0.3.0/test/unit_test/_input/pyproject_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from test.data import get_path_to_parquet_as_pandas_requirements
 
 import pytest
 import toml  # type: ignore
-
 from dac._input.pyproject import PyProjectConfig
 
 
 @pytest.mark.parametrize("project_name,project_version", [("project_1", "0.1.2"), ("test_project", "6.6.6")])
 def test_if_dependencies_are_passed_as_comma_separated_then_valid_pyproject_is_produced(
     project_name: str, project_version: str
 ):
     pm = PyProjectConfig(
-        project_name=project_name, project_version=project_version, project_dependencies="pandas,adlfs, pyarrow"
+        project_name=project_name,
+        project_version=project_version,
+        project_dependencies="pandas;adlfs; pyarrow",
     )
     toml_content = pm.generate_pyproject_toml()
     parsed_toml = toml.loads(toml_content)
     assert parsed_toml["project"]["name"] == pm.project_name
     assert parsed_toml["project"]["version"] == pm.project_version
     assert parsed_toml["project"]["dependencies"] == ["adlfs", "pandas", "pyarrow"]
 
@@ -42,17 +43,25 @@
 
 @pytest.mark.parametrize(
     "name",
     ["3nta"] + [f"in{c}valid" for c in [chr(i) for i in range(256)] if not c.isalnum() and c != "_" and c != "-"],
 )
 def test_if_invalid_project_name_then_raise_error(name: str):
     with pytest.raises(ValueError) as e:
-        PyProjectConfig(project_name=name, project_version="0.1.2", project_dependencies="pandas,adlfs,pyarrow")
+        PyProjectConfig(
+            project_name=name,
+            project_version="0.1.2",
+            project_dependencies="pandas,adlfs,pyarrow",
+        )
     assert "Invalid project name" in str(e.value)
 
 
 @pytest.mark.parametrize(
     "name",
     ["valid", "va_lid"],
 )
 def test_if_valid_project_name_then_dont_raise_error(name: str):
-    PyProjectConfig(project_name=name, project_version="0.1.2", project_dependencies="pandas,adlfs,pyarrow")
+    PyProjectConfig(
+        project_name=name,
+        project_version="0.1.2",
+        project_dependencies="pandas,adlfs,pyarrow",
+    )
```

### Comparing `dac-0.2.0/test/unit_test/_packing/build_wheel_test.py` & `dac-0.3.0/test/unit_test/_packing/build_wheel_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/unit_test/_packing/data_as_code_project_test.py` & `dac-0.3.0/test/unit_test/_packing/data_as_code_project_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.2.0/test/unit_test/_packing/pack_test.py` & `dac-0.3.0/test/unit_test/_packing/pack_test.py`

 * *Files identical despite different names*

