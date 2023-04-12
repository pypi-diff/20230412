# Comparing `tmp/fklearn-2.3.0rc0.tar.gz` & `tmp/fklearn-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fklearn-2.3.0rc0.tar", last modified: Tue Mar 28 13:10:14 2023, max compression
+gzip compressed data, was "fklearn-2.3.1.tar", last modified: Wed Apr 12 12:56:29 2023, max compression
```

## Comparing `fklearn-2.3.0rc0.tar` & `fklearn-2.3.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.668120 fklearn-2.3.0rc0/
--rw-r--r--   0 runner    (1001) docker     (122)    11348 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2299 2023-03-28 13:10:14.668120 fklearn-2.3.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/requirements_catboost.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/requirements_demos.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/requirements_lgbm.txt
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/requirements_tools.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/requirements_xgboost.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 13:10:14.668120 fklearn-2.3.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.652120 fklearn-2.3.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.656120 fklearn-2.3.0rc0/src/fklearn/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/causal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/causal/cate_learning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/cate_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7897 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/cate_learning/double_machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (122)    14729 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/cate_learning/meta_learners.py
--rw-r--r--   0 runner    (1001) docker     (122)     8895 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/debias.py
--rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/effects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/causal/validation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6623 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/validation/auc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6793 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/validation/cate.py
--rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/causal/validation/curves.py
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/common_docstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3655 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/data/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/metrics/pd_extractors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/preprocessing/rebalancing.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/preprocessing/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8511 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/preprocessing/splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.660120 fklearn-2.3.0rc0/src/fklearn/resources/
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/resources/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.664120 fklearn-2.3.0rc0/src/fklearn/training/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6328 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)    30761 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4434 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/imputation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)    27118 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/regression.py
--rw-r--r--   0 runner    (1001) docker     (122)    36662 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/transformation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.664120 fklearn-2.3.0rc0/src/fklearn/tuning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/tuning/model_agnostic_fc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8606 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/tuning/parameter_tuners.py
--rw-r--r--   0 runner    (1001) docker     (122)     6614 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/tuning/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)    17901 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/tuning/selectors.py
--rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/tuning/stoppers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/tuning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.664120 fklearn-2.3.0rc0/src/fklearn/types/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.664120 fklearn-2.3.0rc0/src/fklearn/validation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36847 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/validation/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/validation/perturbators.py
--rw-r--r--   0 runner    (1001) docker     (122)    32870 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/validation/splitters.py
--rw-r--r--   0 runner    (1001) docker     (122)    12367 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/validation/validator.py
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-03-28 13:09:57.000000 fklearn-2.3.0rc0/src/fklearn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:10:14.656120 fklearn-2.3.0rc0/src/fklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2299 2023-03-28 13:10:14.000000 fklearn-2.3.0rc0/src/fklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2091 2023-03-28 13:10:14.000000 fklearn-2.3.0rc0/src/fklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 13:10:14.000000 fklearn-2.3.0rc0/src/fklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 13:10:14.000000 fklearn-2.3.0rc0/src/fklearn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-03-28 13:10:14.000000 fklearn-2.3.0rc0/src/fklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-28 13:10:14.000000 fklearn-2.3.0rc0/src/fklearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.168983 fklearn-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11348 2023-04-12 12:56:20.000000 fklearn-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-12 12:56:20.000000 fklearn-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-04-12 12:56:29.168983 fklearn-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1674 2023-04-12 12:56:20.000000 fklearn-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-12 12:56:20.000000 fklearn-2.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-12 12:56:20.000000 fklearn-2.3.1/requirements_catboost.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-12 12:56:20.000000 fklearn-2.3.1/requirements_demos.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-12 12:56:20.000000 fklearn-2.3.1/requirements_lgbm.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-12 12:56:20.000000 fklearn-2.3.1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 12:56:20.000000 fklearn-2.3.1/requirements_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-12 12:56:20.000000 fklearn-2.3.1/requirements_xgboost.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 12:56:29.168983 fklearn-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-04-12 12:56:20.000000 fklearn-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.156983 fklearn-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/causal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/causal/cate_learning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/cate_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7897 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/cate_learning/double_machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14729 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/cate_learning/meta_learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8895 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/debias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/effects.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/causal/validation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6623 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/validation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6793 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/validation/cate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/causal/validation/curves.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/common_docstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3655 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/data/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/metrics/pd_extractors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/preprocessing/rebalancing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/preprocessing/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8511 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/preprocessing/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/resources/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.168983 fklearn-2.3.1/src/fklearn/training/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6328 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30802 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4434 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27118 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36662 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.168983 fklearn-2.3.1/src/fklearn/tuning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/tuning/model_agnostic_fc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8606 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/tuning/parameter_tuners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6614 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/tuning/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17901 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/tuning/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/tuning/stoppers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/tuning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.168983 fklearn-2.3.1/src/fklearn/types/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.168983 fklearn-2.3.1/src/fklearn/validation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36847 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/validation/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/validation/perturbators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32870 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/validation/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12367 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/validation/validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-04-12 12:56:20.000000 fklearn-2.3.1/src/fklearn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 12:56:29.164983 fklearn-2.3.1/src/fklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-04-12 12:56:29.000000 fklearn-2.3.1/src/fklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2091 2023-04-12 12:56:29.000000 fklearn-2.3.1/src/fklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 12:56:29.000000 fklearn-2.3.1/src/fklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 12:56:28.000000 fklearn-2.3.1/src/fklearn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-12 12:56:29.000000 fklearn-2.3.1/src/fklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-12 12:56:29.000000 fklearn-2.3.1/src/fklearn.egg-info/top_level.txt
```

### Comparing `fklearn-2.3.0rc0/LICENSE` & `fklearn-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/PKG-INFO` & `fklearn-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fklearn
-Version: 2.3.0rc0
+Version: 2.3.1
 Summary: Functional machine learning
 Home-page: https://github.com/nubank/fklearn
 Author: Nubank
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 # fklearn: Functional Machine Learning
 
 ![PyPI](https://img.shields.io/pypi/v/fklearn.svg?style=flat-square)
 [![Documentation Status](https://readthedocs.org/projects/fklearn/badge/?version=latest)](https://fklearn.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/fklearn-python/community.svg)](https://gitter.im/fklearn-python/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-![Tests](https://github.com/nubank/fklearn/actions/workflows/push.yaml/badge.svg?branch=master)]
+![Tests](https://github.com/nubank/fklearn/actions/workflows/push.yaml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 **fklearn** uses functional programming principles to make it easier to solve real problems with Machine Learning.
 
 The name is a reference to the widely known [scikit-learn](https://scikit-learn.org/stable/) library.
 
 **fklearn Principles**
@@ -38,15 +38,15 @@
 2. Production models should match validated models.
 3. Models should be production-ready with few extra steps.
 4. Reproducibility and in-depth analysis of model results should be easy to achieve.
 
 
 [Documentation](https://fklearn.readthedocs.io/en/latest/) |
 [Getting Started](https://fklearn.readthedocs.io/en/latest/getting_started.html) |
-[API Docs](https://fklearn.readthedocs.io/en/latest/api.html) |
+[API Docs](https://fklearn.readthedocs.io/en/latest/api/modules.html) |
 [Contributing](https://fklearn.readthedocs.io/en/latest/contributing.html) |
 
 
 ## Installation
 
 To install via pip:
```

### Comparing `fklearn-2.3.0rc0/README.md` & `fklearn-2.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # fklearn: Functional Machine Learning
 
 ![PyPI](https://img.shields.io/pypi/v/fklearn.svg?style=flat-square)
 [![Documentation Status](https://readthedocs.org/projects/fklearn/badge/?version=latest)](https://fklearn.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/fklearn-python/community.svg)](https://gitter.im/fklearn-python/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-![Tests](https://github.com/nubank/fklearn/actions/workflows/push.yaml/badge.svg?branch=master)]
+![Tests](https://github.com/nubank/fklearn/actions/workflows/push.yaml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 **fklearn** uses functional programming principles to make it easier to solve real problems with Machine Learning.
 
 The name is a reference to the widely known [scikit-learn](https://scikit-learn.org/stable/) library.
 
 **fklearn Principles**
@@ -16,15 +16,15 @@
 2. Production models should match validated models.
 3. Models should be production-ready with few extra steps.
 4. Reproducibility and in-depth analysis of model results should be easy to achieve.
 
 
 [Documentation](https://fklearn.readthedocs.io/en/latest/) |
 [Getting Started](https://fklearn.readthedocs.io/en/latest/getting_started.html) |
-[API Docs](https://fklearn.readthedocs.io/en/latest/api.html) |
+[API Docs](https://fklearn.readthedocs.io/en/latest/api/modules.html) |
 [Contributing](https://fklearn.readthedocs.io/en/latest/contributing.html) |
 
 
 ## Installation
 
 To install via pip:
```

### Comparing `fklearn-2.3.0rc0/setup.py` & `fklearn-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/causal/cate_learning/double_machine_learning.py` & `fklearn-2.3.1/src/fklearn/causal/cate_learning/double_machine_learning.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/causal/cate_learning/meta_learners.py` & `fklearn-2.3.1/src/fklearn/causal/cate_learning/meta_learners.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/causal/debias.py` & `fklearn-2.3.1/src/fklearn/causal/debias.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/causal/effects.py` & `fklearn-2.3.1/src/fklearn/causal/effects.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/causal/validation/auc.py` & `fklearn-2.3.1/src/fklearn/causal/validation/auc.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/causal/validation/cate.py` & `fklearn-2.3.1/src/fklearn/causal/validation/cate.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/causal/validation/curves.py` & `fklearn-2.3.1/src/fklearn/causal/validation/curves.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/common_docstrings.py` & `fklearn-2.3.1/src/fklearn/common_docstrings.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/data/datasets.py` & `fklearn-2.3.1/src/fklearn/data/datasets.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/exceptions/exceptions.py` & `fklearn-2.3.1/src/fklearn/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/metrics/pd_extractors.py` & `fklearn-2.3.1/src/fklearn/metrics/pd_extractors.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/preprocessing/rebalancing.py` & `fklearn-2.3.1/src/fklearn/preprocessing/rebalancing.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/preprocessing/schema.py` & `fklearn-2.3.1/src/fklearn/preprocessing/schema.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/preprocessing/splitting.py` & `fklearn-2.3.1/src/fklearn/preprocessing/splitting.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/calibration.py` & `fklearn-2.3.1/src/fklearn/training/calibration.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/classification.py` & `fklearn-2.3.1/src/fklearn/training/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from typing import List, Any, Optional, Callable, Tuple, Union
+from typing import List, Any, Optional, Callable, Tuple, Union, TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
-from lightgbm import Booster
 from pathlib import Path
 from toolz import curry, merge, assoc
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.linear_model import LogisticRegression
 from sklearn import __version__ as sk_version
 
 from fklearn.types import LearnerReturnType, LogType
 from fklearn.common_docstrings import learner_return_docstring, learner_pred_fn_docstring
 from fklearn.training.utils import log_learner_time, expand_features_encoded
 
 
+if TYPE_CHECKING:
+    from lightgbm import Booster
+
+
 @curry
 @log_learner_time(learner_name='logistic_classification_learner')
 def logistic_classification_learner(df: pd.DataFrame,
                                     features: List[str],
                                     target: str,
                                     params: LogType = None,
                                     prediction_column: str = "prediction",
@@ -509,15 +512,15 @@
                                 encode_extra_cols: bool = True,
                                 valid_sets: Optional[List[pd.DataFrame]] = None,
                                 valid_names: Optional[List[str]] = None,
                                 feval: Optional[Union[
                                     Callable[[np.ndarray, pd.DataFrame], Tuple[str, float, bool]],
                                     List[Callable[[np.ndarray, pd.DataFrame], Tuple[str, float, bool]]]]
                                 ] = None,
-                                init_model: Optional[Union[str, Path, Booster]] = None,
+                                init_model: Optional[Union[str, Path, 'Booster']] = None,
                                 feature_name: Union[List[str], str] = 'auto',
                                 categorical_feature: Union[List[str], List[int], str] = 'auto',
                                 keep_training_booster: bool = False,
                                 callbacks: Optional[List[Callable]] = None,
                                 dataset_init_score: Optional[Union[
                                     List, List[List], np.ndarray, pd.Series, pd.DataFrame]
                                 ] = None) -> LearnerReturnType:
```

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/ensemble.py` & `fklearn-2.3.1/src/fklearn/training/ensemble.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/imputation.py` & `fklearn-2.3.1/src/fklearn/training/imputation.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/pipeline.py` & `fklearn-2.3.1/src/fklearn/training/pipeline.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/regression.py` & `fklearn-2.3.1/src/fklearn/training/regression.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/transformation.py` & `fklearn-2.3.1/src/fklearn/training/transformation.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/unsupervised.py` & `fklearn-2.3.1/src/fklearn/training/unsupervised.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/training/utils.py` & `fklearn-2.3.1/src/fklearn/training/utils.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/tuning/model_agnostic_fc.py` & `fklearn-2.3.1/src/fklearn/tuning/model_agnostic_fc.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/tuning/parameter_tuners.py` & `fklearn-2.3.1/src/fklearn/tuning/parameter_tuners.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/tuning/samplers.py` & `fklearn-2.3.1/src/fklearn/tuning/samplers.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/tuning/selectors.py` & `fklearn-2.3.1/src/fklearn/tuning/selectors.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/tuning/stoppers.py` & `fklearn-2.3.1/src/fklearn/tuning/stoppers.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/tuning/utils.py` & `fklearn-2.3.1/src/fklearn/tuning/utils.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/types/types.py` & `fklearn-2.3.1/src/fklearn/types/types.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/validation/evaluators.py` & `fklearn-2.3.1/src/fklearn/validation/evaluators.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/validation/perturbators.py` & `fklearn-2.3.1/src/fklearn/validation/perturbators.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/validation/splitters.py` & `fklearn-2.3.1/src/fklearn/validation/splitters.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn/validation/validator.py` & `fklearn-2.3.1/src/fklearn/validation/validator.py`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn.egg-info/PKG-INFO` & `fklearn-2.3.1/src/fklearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fklearn
-Version: 2.3.0rc0
+Version: 2.3.1
 Summary: Functional machine learning
 Home-page: https://github.com/nubank/fklearn
 Author: Nubank
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 # fklearn: Functional Machine Learning
 
 ![PyPI](https://img.shields.io/pypi/v/fklearn.svg?style=flat-square)
 [![Documentation Status](https://readthedocs.org/projects/fklearn/badge/?version=latest)](https://fklearn.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/fklearn-python/community.svg)](https://gitter.im/fklearn-python/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-![Tests](https://github.com/nubank/fklearn/actions/workflows/push.yaml/badge.svg?branch=master)]
+![Tests](https://github.com/nubank/fklearn/actions/workflows/push.yaml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 **fklearn** uses functional programming principles to make it easier to solve real problems with Machine Learning.
 
 The name is a reference to the widely known [scikit-learn](https://scikit-learn.org/stable/) library.
 
 **fklearn Principles**
@@ -38,15 +38,15 @@
 2. Production models should match validated models.
 3. Models should be production-ready with few extra steps.
 4. Reproducibility and in-depth analysis of model results should be easy to achieve.
 
 
 [Documentation](https://fklearn.readthedocs.io/en/latest/) |
 [Getting Started](https://fklearn.readthedocs.io/en/latest/getting_started.html) |
-[API Docs](https://fklearn.readthedocs.io/en/latest/api.html) |
+[API Docs](https://fklearn.readthedocs.io/en/latest/api/modules.html) |
 [Contributing](https://fklearn.readthedocs.io/en/latest/contributing.html) |
 
 
 ## Installation
 
 To install via pip:
```

### Comparing `fklearn-2.3.0rc0/src/fklearn.egg-info/SOURCES.txt` & `fklearn-2.3.1/src/fklearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fklearn-2.3.0rc0/src/fklearn.egg-info/requires.txt` & `fklearn-2.3.1/src/fklearn.egg-info/requires.txt`

 * *Files identical despite different names*

