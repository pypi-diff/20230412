# Comparing `tmp/dvclive-2.6.2.tar.gz` & `tmp/dvclive-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvclive-2.6.2.tar", last modified: Wed Apr  5 10:39:19 2023, max compression
+gzip compressed data, was "dvclive-2.6.3.tar", last modified: Tue Apr 11 22:15:49 2023, max compression
```

## Comparing `dvclive-2.6.2.tar` & `dvclive-2.6.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.796150 dvclive-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-05 10:39:09.000000 dvclive-2.6.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 10:39:09.000000 dvclive-2.6.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.788150 dvclive-2.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-05 10:39:09.000000 dvclive-2.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-05 10:39:09.000000 dvclive-2.6.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.788150 dvclive-2.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-05 10:39:09.000000 dvclive-2.6.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-05 10:39:09.000000 dvclive-2.6.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-05 10:39:09.000000 dvclive-2.6.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-05 10:39:09.000000 dvclive-2.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-05 10:39:09.000000 dvclive-2.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-05 10:39:09.000000 dvclive-2.6.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-05 10:39:09.000000 dvclive-2.6.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-05 10:39:09.000000 dvclive-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-05 10:39:19.796150 dvclive-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-05 10:39:09.000000 dvclive-2.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-05 10:39:09.000000 dvclive-2.6.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-05 10:39:09.000000 dvclive-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-05 10:39:19.796150 dvclive-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-05 10:39:09.000000 dvclive-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.784150 dvclive-2.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.788150 dvclive-2.6.2/src/dvclive/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)    15851 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/optuna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.792150 dvclive-2.6.2/src/dvclive/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/plots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/plots/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/plots/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/plots/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-05 10:39:09.000000 dvclive-2.6.2/src/dvclive/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.792150 dvclive-2.6.2/src/dvclive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-05 10:39:19.000000 dvclive-2.6.2/src/dvclive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-05 10:39:19.000000 dvclive-2.6.2/src/dvclive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 10:39:19.000000 dvclive-2.6.2/src/dvclive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 10:39:19.000000 dvclive-2.6.2/src/dvclive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-05 10:39:19.000000 dvclive-2.6.2/src/dvclive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 10:39:19.000000 dvclive-2.6.2/src/dvclive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.792150 dvclive-2.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.792150 dvclive-2.6.2/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/plots/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/plots/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/plots/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:39:19.796150 dvclive-2.6.2/tests/test_frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_frameworks/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_log_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-05 10:39:09.000000 dvclive-2.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.128222 dvclive-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-11 22:15:38.000000 dvclive-2.6.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 22:15:38.000000 dvclive-2.6.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.120221 dvclive-2.6.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.120221 dvclive-2.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-11 22:15:38.000000 dvclive-2.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-11 22:15:38.000000 dvclive-2.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-11 22:15:38.000000 dvclive-2.6.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-11 22:15:38.000000 dvclive-2.6.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-11 22:15:38.000000 dvclive-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-11 22:15:49.128222 dvclive-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-11 22:15:38.000000 dvclive-2.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-11 22:15:38.000000 dvclive-2.6.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-11 22:15:38.000000 dvclive-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-11 22:15:49.128222 dvclive-2.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 22:15:38.000000 dvclive-2.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.116222 dvclive-2.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/src/dvclive/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/optuna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/src/dvclive/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/src/dvclive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:15:48.000000 dvclive-2.6.3/src/dvclive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.128222 dvclive-2.6.3/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/plots/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/plots/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/plots/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.128222 dvclive-2.6.3/tests/test_frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_log_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_utils.py
```

### Comparing `dvclive-2.6.2/.cruft.json` & `dvclive-2.6.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/.github/dependabot.yml` & `dvclive-2.6.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/.github/workflows/release.yml` & `dvclive-2.6.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/.github/workflows/tests.yml` & `dvclive-2.6.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/.gitignore` & `dvclive-2.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/.pre-commit-config.yaml` & `dvclive-2.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/CODE_OF_CONDUCT.rst` & `dvclive-2.6.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/CONTRIBUTING.rst` & `dvclive-2.6.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/LICENSE` & `dvclive-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/PKG-INFO` & `dvclive-2.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.6.2
+Version: 2.6.3
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
@@ -68,17 +68,17 @@
    :alt: Black
 
 DVCLive is a Python library for logging machine learning metrics and other metadata in simple file formats, which is fully compatible with DVC.
 
 `Documentation <https://dvc.org/doc/dvclive>`_
 ----------------------------------------------
 
-- `Get Started <https://dvc.org/doc/dvclive/get-started>`_
+- `Get Started <https://dvc.org/doc/start/experiments>`_
 - `How it Works <https://dvc.org/doc/dvclive/how-it-works>`_
-- `API Reference <https://dvc.org/doc/dvclive/api-reference>`_
+- `API Reference <https://dvc.org/doc/dvclive/live>`_
 
 Installation
 ------------
 
 You can install *dvclive* via pip_ from PyPI_:
 
 .. code:: console
```

### Comparing `dvclive-2.6.2/README.rst` & `dvclive-2.6.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
    :alt: Black
 
 DVCLive is a Python library for logging machine learning metrics and other metadata in simple file formats, which is fully compatible with DVC.
 
 `Documentation <https://dvc.org/doc/dvclive>`_
 ----------------------------------------------
 
-- `Get Started <https://dvc.org/doc/dvclive/get-started>`_
+- `Get Started <https://dvc.org/doc/start/experiments>`_
 - `How it Works <https://dvc.org/doc/dvclive/how-it-works>`_
-- `API Reference <https://dvc.org/doc/dvclive/api-reference>`_
+- `API Reference <https://dvc.org/doc/dvclive/live>`_
 
 Installation
 ------------
 
 You can install *dvclive* via pip_ from PyPI_:
 
 .. code:: console
```

### Comparing `dvclive-2.6.2/noxfile.py` & `dvclive-2.6.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/pyproject.toml` & `dvclive-2.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/setup.cfg` & `dvclive-2.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/catalyst.py` & `dvclive-2.6.3/src/dvclive/catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/dvc.py` & `dvclive-2.6.3/src/dvclive/dvc.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/error.py` & `dvclive-2.6.3/src/dvclive/error.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/fastai.py` & `dvclive-2.6.3/src/dvclive/fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/huggingface.py` & `dvclive-2.6.3/src/dvclive/huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/keras.py` & `dvclive-2.6.3/src/dvclive/keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/lgbm.py` & `dvclive-2.6.3/src/dvclive/lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/lightning.py` & `dvclive-2.6.3/src/dvclive/lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/live.py` & `dvclive-2.6.3/src/dvclive/live.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,19 @@
         self.summary = set_in(self.summary, data.summary_keys, val)
         logger.debug(f"Logged {name}: {val}")
 
     def log_image(self, name: str, val):
         if not Image.could_log(val):
             raise InvalidDataTypeError(name, type(val))
 
+        if isinstance(val, str) or isinstance(val, Path):
+            from PIL import Image as ImagePIL
+
+            val = ImagePIL.open(val)
+
         if name in self._images:
             data = self._images[name]
         else:
             data = Image(name, self.plots_dir)
             self._images[name] = data
 
         data.step = self.step
```

### Comparing `dvclive-2.6.2/src/dvclive/optuna.py` & `dvclive-2.6.3/src/dvclive/optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/plots/base.py` & `dvclive-2.6.3/src/dvclive/plots/base.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/plots/metric.py` & `dvclive-2.6.3/src/dvclive/plots/metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/plots/sklearn.py` & `dvclive-2.6.3/src/dvclive/plots/sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/plots/utils.py` & `dvclive-2.6.3/src/dvclive/plots/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/report.py` & `dvclive-2.6.3/src/dvclive/report.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/serialize.py` & `dvclive-2.6.3/src/dvclive/serialize.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/studio.py` & `dvclive-2.6.3/src/dvclive/studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/utils.py` & `dvclive-2.6.3/src/dvclive/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive/xgb.py` & `dvclive-2.6.3/src/dvclive/xgb.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive.egg-info/PKG-INFO` & `dvclive-2.6.3/src/dvclive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.6.2
+Version: 2.6.3
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
@@ -68,17 +68,17 @@
    :alt: Black
 
 DVCLive is a Python library for logging machine learning metrics and other metadata in simple file formats, which is fully compatible with DVC.
 
 `Documentation <https://dvc.org/doc/dvclive>`_
 ----------------------------------------------
 
-- `Get Started <https://dvc.org/doc/dvclive/get-started>`_
+- `Get Started <https://dvc.org/doc/start/experiments>`_
 - `How it Works <https://dvc.org/doc/dvclive/how-it-works>`_
-- `API Reference <https://dvc.org/doc/dvclive/api-reference>`_
+- `API Reference <https://dvc.org/doc/dvclive/live>`_
 
 Installation
 ------------
 
 You can install *dvclive* via pip_ from PyPI_:
 
 .. code:: console
```

### Comparing `dvclive-2.6.2/src/dvclive.egg-info/SOURCES.txt` & `dvclive-2.6.3/src/dvclive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/src/dvclive.egg-info/requires.txt` & `dvclive-2.6.3/src/dvclive.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/conftest.py` & `dvclive-2.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/plots/test_metric.py` & `dvclive-2.6.3/tests/plots/test_metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/plots/test_sklearn.py` & `dvclive-2.6.3/tests/plots/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_dvc.py` & `dvclive-2.6.3/tests/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_catalyst.py` & `dvclive-2.6.3/tests/test_frameworks/test_catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_fastai.py` & `dvclive-2.6.3/tests/test_frameworks/test_fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_huggingface.py` & `dvclive-2.6.3/tests/test_frameworks/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_keras.py` & `dvclive-2.6.3/tests/test_frameworks/test_keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_lgbm.py` & `dvclive-2.6.3/tests/test_frameworks/test_lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_lightning.py` & `dvclive-2.6.3/tests/test_frameworks/test_lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_optuna.py` & `dvclive-2.6.3/tests/test_frameworks/test_optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_frameworks/test_xgboost.py` & `dvclive-2.6.3/tests/test_frameworks/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_log_artifact.py` & `dvclive-2.6.3/tests/test_log_artifact.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_main.py` & `dvclive-2.6.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_report.py` & `dvclive-2.6.3/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_studio.py` & `dvclive-2.6.3/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.2/tests/test_utils.py` & `dvclive-2.6.3/tests/test_utils.py`

 * *Files identical despite different names*

