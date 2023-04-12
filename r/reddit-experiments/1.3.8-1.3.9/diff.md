# Comparing `tmp/reddit_experiments-1.3.8.tar.gz` & `tmp/reddit_experiments-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_experiments-1.3.8.tar", last modified: Wed Aug 17 20:47:48 2022, max compression
+gzip compressed data, was "reddit_experiments-1.3.9.tar", last modified: Mon Aug 22 18:52:58 2022, max compression
```

## Comparing `reddit_experiments-1.3.8.tar` & `reddit_experiments-1.3.9.tar`

### file list

```diff
@@ -1,72 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.961866 reddit_experiments-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.933866 reddit_experiments-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.937866 reddit_experiments-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-08-17 20:47:48.961866 reddit_experiments-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.937866 reddit_experiments-1.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4865 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.937866 reddit_experiments-1.3.8/reddit_decider/
--rw-r--r--   0 runner    (1001) docker     (121)    45027 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_decider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.937866 reddit_experiments-1.3.8/reddit_experiments/
--rw-r--r--   0 runner    (1001) docker     (121)    14589 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.937866 reddit_experiments-1.3.8/reddit_experiments/providers/
--rw-r--r--   0 runner    (1001) docker     (121)     5508 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/providers/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/providers/forced_variant.py
--rw-r--r--   0 runner    (1001) docker     (121)    13980 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/providers/r2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11799 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/providers/simple_experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.941866 reddit_experiments-1.3.8/reddit_experiments/targeting/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/targeting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/targeting/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8285 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/targeting/tree_targeting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.941866 reddit_experiments-1.3.8/reddit_experiments/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/variant_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/variant_sets/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/variant_sets/multi_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/variant_sets/range_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/variant_sets/rollout_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/reddit_experiments/variant_sets/single_variant_set.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.937866 reddit_experiments-1.3.8/reddit_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-08-17 20:47:48.000000 reddit_experiments-1.3.8/reddit_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-08-17 20:47:48.000000 reddit_experiments-1.3.8/reddit_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 20:47:48.000000 reddit_experiments-1.3.8/reddit_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-17 20:47:48.000000 reddit_experiments-1.3.8/reddit_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 20:47:48.000000 reddit_experiments-1.3.8/reddit_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 20:47:48.000000 reddit_experiments-1.3.8/reddit_experiments.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-08-17 20:47:48.961866 reddit_experiments-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.941866 reddit_experiments-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    69905 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/decider_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    36949 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.941866 reddit_experiments-1.3.8/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (121)    27412 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/feature_flag_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/forced_variant_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    29866 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/r2_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    18526 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/simple_experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.941866 reddit_experiments-1.3.8/tests/providers/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/variant_sets/multi_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/variant_sets/range_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     3115 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/variant_sets/rollout_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/providers/variant_sets/single_variant_set_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.941866 reddit_experiments-1.3.8/tests/range_variant_tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.961866 reddit_experiments-1.3.8/tests/range_variant_tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   154451 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/range_variant_tests/data/original_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (121) 14213529 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/range_variant_tests/data/output.json
--rw-r--r--   0 runner    (1001) docker     (121)   163729 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/range_variant_tests/data/range_variant_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/range_variant_tests/range_variant_parity_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:47:48.961866 reddit_experiments-1.3.8/tests/targeting/
--rw-r--r--   0 runner    (1001) docker     (121)    19814 2022-08-17 20:47:35.000000 reddit_experiments-1.3.8/tests/targeting/tree_targeting_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    53651 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/images/ddg-logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5700 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/docs/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/legacy/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/reddit_decider/
+-rw-r--r--   0 runner    (1001) docker     (121)    47376 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_decider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/
+-rw-r--r--   0 runner    (1001) docker     (121)    14628 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/providers/
+-rw-r--r--   0 runner    (1001) docker     (121)     5508 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/forced_variant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13980 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11799 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/simple_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/targeting/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/targeting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/targeting/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8285 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/targeting/tree_targeting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/multi_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/range_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/rollout_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/single_variant_set.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    69905 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/decider_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36949 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (121)    27412 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/feature_flag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/forced_variant_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29866 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/r2_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18526 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/simple_experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/providers/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/multi_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/range_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3115 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/rollout_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/single_variant_set_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/range_variant_tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/tests/range_variant_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   154451 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/data/original_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (121) 14213529 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/data/output.json
+-rw-r--r--   0 runner    (1001) docker     (121)   163729 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/data/range_variant_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/range_variant_parity_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/tests/targeting/
+-rw-r--r--   0 runner    (1001) docker     (121)    19814 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/targeting/tree_targeting_tests.py
```

### Comparing `reddit_experiments-1.3.8/.github/workflows/python-package.yaml` & `reddit_experiments-1.3.9/.github/workflows/python-package.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/.github/workflows/python-publish.yaml` & `reddit_experiments-1.3.9/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/LICENSE` & `reddit_experiments-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/Makefile` & `reddit_experiments-1.3.9/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/PKG-INFO` & `reddit_experiments-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_experiments
-Version: 1.3.8
+Version: 1.3.9
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
```

### Comparing `reddit_experiments-1.3.8/README.md` & `reddit_experiments-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/docs/conf.py` & `reddit_experiments-1.3.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # The encoding of source files.
 source_encoding = "utf-8"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = "Experiments"
+project = "Experiments.py"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -50,36 +50,37 @@
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "friendly"
 
 # -- Options for HTML output ----------------------------------------------
 
 html_theme_path = [alabaster.get_path()]
-html_static_path = []
+html_static_path = ["images"]
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "alabaster"
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title =
 
 # which templates to put in the sidebar.  we're just removing the relations
 # section from the defaults here, that's "next article" and "previous article"
 html_sidebars = {
-    "**": []
+    "**": ["about.html", "searchbox.html", "navigation.html"]
 }
 
 html_theme_options = {
     "description": "Reddit's Python Experiments Framework",
     "github_button": False,
     "github_repo": "experiments.py",
     "github_user": "reddit",
     "github_banner": True,
+    "logo": "ddg-logo.png",
     "logo_name": True,
     "show_powered_by": False,
     "show_related": False,
     "show_relbars": True,
     "page_width": "960px",
 }
```

### Comparing `reddit_experiments-1.3.8/docs/index.rst` & `reddit_experiments-1.3.9/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,305 +1,357 @@
-00000000: 6060 7265 6464 6974 5f65 7870 6572 696d  ``reddit_experim
-00000010: 656e 7473 6060 0a3d 3d3d 3d3d 3d3d 3d3d  ents``.=========
-00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000030: 3d3d 3d3d 3d3d 0a0a 2e2e 2061 7574 6f6d  ======.... autom
-00000040: 6f64 756c 653a 3a20 7265 6464 6974 5f64  odule:: reddit_d
-00000050: 6563 6964 6572 0a0a 0a50 7265 7265 7175  ecider...Prerequ
-00000060: 6973 6974 6520 7061 636b 6167 6573 0a2d  isite packages.-
-00000070: 2d2d 2d2d 2d2d 0a2e 2e20 636f 6465 2d62  ------... code-b
-00000080: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
-00000090: 2020 2062 6173 6570 6c61 7465 3e3d 322e     baseplate>=2.
-000000a0: 302e 300a 0a20 2020 2072 6564 6469 742d  0.0..    reddit-
-000000b0: 6564 6765 636f 6e74 6578 743e 3d31 2e30  edgecontext>=1.0
-000000c0: 2e30 0a0a 2020 2020 2320 7570 6772 6164  .0..    # upgrad
-000000d0: 6520 6f72 2069 6e74 6567 7261 7465 206c  e or integrate l
-000000e0: 6174 6573 7420 7265 6464 6974 2d76 322d  atest reddit-v2-
-000000f0: 6576 656e 7473 2070 6163 6b61 6765 0a20  events package. 
-00000100: 2020 2023 206f 7220 6d61 6e75 616c 6c79     # or manually
-00000110: 2075 7064 6174 6520 7468 7269 6674 2073   update thrift s
-00000120: 6368 656d 6173 0a20 2020 2023 2074 6f20  chemas.    # to 
-00000130: 616c 6c6f 7720 6576 656e 7420 6669 656c  allow event fiel
-00000140: 6473 2074 6f20 6265 2070 6f70 756c 6174  ds to be populat
-00000150: 6564 2069 6e20 6578 706f 7375 7265 730a  ed in exposures.
-00000160: 2020 2020 7265 6464 6974 2d76 322d 6576      reddit-v2-ev
-00000170: 656e 7473 0a0a 5072 6572 6571 7569 7369  ents..Prerequisi
-00000180: 7465 2069 6e66 7261 7374 7275 6374 7572  te infrastructur
-00000190: 650a 2d2d 2d2d 2d2d 2d0a 5365 7420 7570  e.-------.Set up
-000001a0: 2079 6f75 7220 7365 7276 6963 6520 746f   your service to
-000001b0: 2070 756c 6c20 646f 776e 2026 2073 796e   pull down & syn
-000001c0: 6368 726f 6e69 7a65 2065 7870 6572 696d  chronize experim
-000001d0: 656e 7420 636f 6e66 6967 7572 6174 696f  ent configuratio
-000001e0: 6e73 2066 726f 6d20 5a6f 6f6b 6565 7065  ns from Zookeepe
-000001f0: 7220 7669 6120 7468 6520 4261 7365 706c  r via the Basepl
-00000200: 6174 6520 606c 6976 652d 6461 7461 2077  ate `live-data w
-00000210: 6174 6368 6572 2073 6964 6563 6172 0a3c  atcher sidecar.<
-00000220: 6874 7470 733a 2f2f 6261 7365 706c 6174  https://baseplat
-00000230: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00000240: 2f65 6e2f 7374 6162 6c65 2f61 7069 2f62  /en/stable/api/b
-00000250: 6173 6570 6c61 7465 2f6c 6962 2f6c 6976  aseplate/lib/liv
-00000260: 655f 6461 7461 2e68 746d 6c3f 6869 6768  e_data.html?high
-00000270: 6c69 6768 743d 7369 6465 6361 7223 7761  light=sidecar#wa
-00000280: 7463 6865 722d 6461 656d 6f6e 3e60 5f20  tcher-daemon>`_ 
-00000290: 286d 696e 696d 756d 2076 322e 342e 3133  (minimum v2.4.13
-000002a0: 292e 0a59 6f75 276c 6c20 6861 7665 2074  )..You'll have t
-000002b0: 6f20 6d61 6b65 2073 7572 6520 7468 6174  o make sure that
-000002c0: 2079 6f75 7220 7365 7276 6963 6520 6973   your service is
-000002d0: 2061 7574 686f 7269 7a65 6420 746f 2066   authorized to f
-000002e0: 6574 6368 2074 6865 2061 7070 726f 7072  etch the appropr
-000002f0: 6961 7465 2073 6563 7265 7420 6672 6f6d  iate secret from
-00000300: 2056 6175 6c74 2e0a 0a50 7265 7265 7175   Vault...Prerequ
-00000310: 6973 6974 6520 636f 6e66 6967 7572 6174  isite configurat
-00000320: 696f 6e3a 0a2d 2d2d 2d2d 2d2d 0a53 6574  ion:.-------.Set
-00000330: 7570 203a 636f 6465 3a60 7265 6464 6974  up :code:`reddit
-00000340: 2d65 7870 6572 696d 656e 7473 6020 696e  -experiments` in
-00000350: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
-00000360: 6e27 7320 636f 6e66 6967 7572 6174 696f  n's configuratio
-00000370: 6e20 6669 6c65 3a0a 0a2e 2e20 636f 6465  n file:.... code
-00000380: 2d62 6c6f 636b 3a3a 2069 6e69 0a0a 2020  -block:: ini..  
-00000390: 205b 6170 703a 6d61 696e 5d0a 0a20 2020   [app:main]..   
-000003a0: 2e2e 2e0a 0a20 2020 2320 6f70 7469 6f6e  .....   # option
-000003b0: 616c 3a20 6120 7061 7468 2074 6f20 7468  al: a path to th
-000003c0: 6520 6669 6c65 2077 6865 7265 2065 7870  e file where exp
-000003d0: 6572 696d 656e 7420 636f 6e66 6967 7572  eriment configur
-000003e0: 6174 696f 6e20 6973 2077 7269 7474 656e  ation is written
-000003f0: 0a20 2020 2320 2864 6566 6175 6c74 3a20  .   # (default: 
-00000400: 2f76 6172 2f6c 6f63 616c 2f65 7870 6572  /var/local/exper
-00000410: 696d 656e 7473 2e6a 736f 6e29 0a20 2020  iments.json).   
-00000420: 6578 7065 7269 6d65 6e74 732e 7061 7468  experiments.path
-00000430: 203d 202f 7661 722f 6c6f 6361 6c2f 666f   = /var/local/fo
-00000440: 6f2e 6a73 6f6e 0a0a 2020 2023 206f 7074  o.json..   # opt
-00000450: 696f 6e61 6c3a 2068 6f77 206c 6f6e 6720  ional: how long 
-00000460: 746f 2077 6169 7420 666f 7220 7468 6520  to wait for the 
-00000470: 6578 7065 7269 6d65 6e74 7320 6669 6c65  experiments file
-00000480: 2074 6f20 6578 6973 7420 6265 666f 7265   to exist before
-00000490: 2066 6169 6c69 6e67 0a20 2020 2320 2864   failing.   # (d
-000004a0: 6566 6175 6c74 3a20 646f 206e 6f74 2077  efault: do not w
-000004b0: 6169 742e 2066 6169 6c20 696d 6d65 6469  ait. fail immedi
-000004c0: 6174 656c 7920 6966 206e 6f74 2061 7661  ately if not ava
-000004d0: 696c 6162 6c65 290a 2020 2065 7870 6572  ilable).   exper
-000004e0: 696d 656e 7473 2e74 696d 656f 7574 203d  iments.timeout =
-000004f0: 2036 3020 7365 636f 6e64 730a 0a20 2020   60 seconds..   
-00000500: 2320 6f70 7469 6f6e 616c 3a20 7468 6520  # optional: the 
-00000510: 6261 7365 2061 6d6f 756e 7420 6f66 2074  base amount of t
-00000520: 696d 6520 666f 7220 6578 706f 6e65 6e74  ime for exponent
-00000530: 6961 6c20 6261 636b 6f66 6620 7768 696c  ial backoff whil
-00000540: 6520 7761 6974 696e 670a 2020 2023 2066  e waiting.   # f
-00000550: 6f72 2074 6865 2066 696c 6520 746f 2062  or the file to b
-00000560: 6520 6176 6169 6c61 626c 652e 0a20 2020  e available..   
-00000570: 2320 2864 6566 6175 6c74 3a20 6e6f 2062  # (default: no b
-00000580: 6163 6b6f 6666 2074 696d 6520 6265 7477  ackoff time betw
-00000590: 6565 6e20 7472 6965 7329 0a20 2020 6578  een tries).   ex
-000005a0: 7065 7269 6d65 6e74 732e 6261 636b 6f66  periments.backof
-000005b0: 6620 3d20 3120 7365 636f 6e64 0a0a 2020  f = 1 second..  
-000005c0: 202e 2e2e 0a0a 0a49 6e74 6567 7261 7465   ......Integrate
-000005d0: 203a 636f 6465 3a60 7265 6464 6974 2d65   :code:`reddit-e
-000005e0: 7870 6572 696d 656e 7473 6020 696e 746f  xperiments` into
-000005f0: 2042 6173 6570 6c61 7465 2073 6572 7669   Baseplate servi
-00000600: 6365 0a2d 2d2d 2d2d 2d2d 0a49 6e20 796f  ce.-------.In yo
-00000610: 7572 2073 6572 7669 6365 2773 2069 6e69  ur service's ini
-00000620: 7469 616c 697a 6174 696f 6e20 7072 6f63  tialization proc
-00000630: 6573 732c 2061 6464 2061 203a 636f 6465  ess, add a :code
-00000640: 3a60 6465 6369 6465 7260 2069 6e73 7461  :`decider` insta
-00000650: 6e63 6520 746f 2062 6173 6570 6c61 7465  nce to baseplate
-00000660: 2773 2063 6f6e 7465 7874 3a0a 284e 6f74  's context:.(Not
-00000670: 6520 7468 6520 7573 6520 6f66 2074 6865  e the use of the
-00000680: 203a 636f 6465 3a60 4578 7065 7269 6d65   :code:`Experime
-00000690: 6e74 4c6f 6767 6572 602c 2077 6869 6368  ntLogger`, which
-000006a0: 2069 7320 7573 6564 2074 6f20 7075 626c   is used to publ
-000006b0: 6973 6820 6578 706f 7375 7265 2056 3220  ish exposure V2 
-000006c0: 6576 656e 7473 2c0a 616e 2065 7861 6d70  events,.an examp
-000006d0: 6c65 2063 616e 2062 6520 7365 656e 2060  le can be seen `
-000006e0: 6865 7265 203c 6874 7470 733a 2f2f 6769  here <https://gi
-000006f0: 7468 7562 2e73 6e6f 6f67 7574 732e 6e65  thub.snooguts.ne
-00000700: 742f 7265 6464 6974 2f72 6564 6469 742d  t/reddit/reddit-
-00000710: 7365 7276 6963 652d 6772 6170 6871 6c2f  service-graphql/
-00000720: 626c 6f62 2f33 3733 3462 3531 3733 3263  blob/3734b51732c
-00000730: 3239 6430 3765 6566 3332 6163 6564 3836  29d07eef32aced86
-00000740: 3637 3763 6365 3530 3634 6462 622f 6772  677cce5064dbb/gr
-00000750: 6170 6871 6c2d 7079 2f67 7261 7068 716c  aphql-py/graphql
-00000760: 5f61 7069 2f65 7665 6e74 732f 7574 696c  _api/events/util
-00000770: 732e 7079 234c 3230 353e 605f 290a 0a2e  s.py#L205>`_)...
-00000780: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00000790: 7974 686f 6e0a 0a20 2020 2023 2061 7070  ython..    # app
-000007a0: 6c69 6361 7469 6f6e 2063 6f64 650a 2020  lication code.  
-000007b0: 2020 6672 6f6d 2072 6564 6469 745f 6465    from reddit_de
-000007c0: 6369 6465 7220 696d 706f 7274 2064 6563  cider import dec
-000007d0: 6964 6572 5f63 6c69 656e 745f 6672 6f6d  ider_client_from
-000007e0: 5f63 6f6e 6669 670a 2020 2020 6672 6f6d  _config.    from
-000007f0: 2072 6564 6469 745f 6465 6369 6465 7220   reddit_decider 
-00000800: 696d 706f 7274 2044 6563 6964 6572 436c  import DeciderCl
-00000810: 6965 6e74 0a0a 2020 2020 2320 6f70 7469  ient..    # opti
-00000820: 6f6e 616c 0a20 2020 2066 726f 6d20 736f  onal.    from so
-00000830: 6d65 5f66 696c 6520 696d 706f 7274 206d  me_file import m
-00000840: 795f 6669 656c 645f 6578 7472 6163 746f  y_field_extracto
-00000850: 720a 0a0a 2020 2020 6465 6620 6d61 6b65  r...    def make
-00000860: 5f77 7367 695f 6170 7028 6170 705f 636f  _wsgi_app(app_co
-00000870: 6e66 6967 293a 0a20 2020 2020 2020 2062  nfig):.        b
-00000880: 6173 6570 6c61 7465 203d 2042 6173 6570  aseplate = Basep
-00000890: 6c61 7465 2861 7070 5f63 6f6e 6669 6729  late(app_config)
-000008a0: 0a20 2020 2020 2020 2064 6563 6964 6572  .        decider
-000008b0: 5f66 6163 746f 7279 203d 2064 6563 6964  _factory = decid
-000008c0: 6572 5f63 6c69 656e 745f 6672 6f6d 5f63  er_client_from_c
-000008d0: 6f6e 6669 6728 6170 705f 636f 6e66 6967  onfig(app_config
-000008e0: 3d61 7070 5f63 6f6e 6669 672c 0a20 2020  =app_config,.   
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000920: 2020 6576 656e 745f 6c6f 6767 6572 3d45    event_logger=E
-00000930: 7870 6572 696d 656e 744c 6f67 6765 722c  xperimentLogger,
-00000940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 2020 2020 7072 6566 6978 3d22 6578        prefix="ex
-00000980: 7065 7269 6d65 6e74 732e 222c 0a20 2020  periments.",.   
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 7265 7175 6573 745f 6669 656c 645f    request_field_
-000009d0: 6578 7472 6163 746f 723d 6d79 5f66 6965  extractor=my_fie
-000009e0: 6c64 5f65 7874 7261 6374 6f72 2920 2023  ld_extractor)  #
-000009f0: 2074 6869 7320 6973 206f 7074 696f 6e61   this is optiona
-00000a00: 6c2c 2063 616e 2062 6520 604e 6f6e 6560  l, can be `None`
-00000a10: 2069 6620 6564 6765 5f63 6f6e 7465 7874   if edge_context
-00000a20: 2063 6f6e 7461 696e 7320 616c 6c20 7468   contains all th
-00000a30: 6520 6669 656c 6473 2079 6f75 206e 6565  e fields you nee
-00000a40: 640a 2020 2020 2020 2020 6261 7365 706c  d.        basepl
-00000a50: 6174 652e 6164 645f 746f 5f63 6f6e 7465  ate.add_to_conte
-00000a60: 7874 2822 6465 6369 6465 7222 2c20 6465  xt("decider", de
-00000a70: 6369 6465 725f 6661 6374 6f72 7929 0a0a  cider_factory)..
-00000a80: 2020 2020 2020 2020 2320 4f72 2075 7365          # Or use
-00000a90: 2060 4465 6369 6465 7243 6c69 656e 7460   `DeciderClient`
-00000aa0: 2077 6974 6820 6063 6f6e 6669 6775 7265   with `configure
-00000ab0: 5f63 6f6e 7465 7874 2829 602c 0a20 2020  _context()`,.   
-00000ac0: 2020 2020 2023 2077 6869 6368 2069 6e74       # which int
-00000ad0: 6572 6e61 6c6c 7920 6361 6c6c 7320 6064  ernally calls `d
-00000ae0: 6563 6964 6572 5f63 6c69 656e 745f 6672  ecider_client_fr
-00000af0: 6f6d 5f63 6f6e 6669 6728 2960 0a20 2020  om_config()`.   
-00000b00: 2020 2020 2062 6173 6570 6c61 7465 2e63       baseplate.c
-00000b10: 6f6e 6669 6775 7265 5f63 6f6e 7465 7874  onfigure_context
-00000b20: 287b 0a20 2020 2020 2020 2020 2020 2022  ({.            "
-00000b30: 6465 6369 6465 7222 3a20 4465 6369 6465  decider": Decide
-00000b40: 7243 6c69 656e 7428 0a20 2020 2020 2020  rClient(.       
-00000b50: 2020 2020 2020 2020 2070 7265 6669 783d           prefix=
-00000b60: 2265 7870 6572 696d 656e 7473 2e22 2c0a  "experiments.",.
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 6576 656e 745f 6c6f 6767 6572 3d45 7665  event_logger=Eve
-00000b90: 6e74 4c6f 6767 6572 2c0a 2020 2020 2020  ntLogger,.      
-00000ba0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-00000bb0: 745f 6669 656c 645f 6578 7472 6163 746f  t_field_extracto
-00000bc0: 723d 6d79 5f66 6965 6c64 5f65 7874 7261  r=my_field_extra
-00000bd0: 6374 6f72 2020 2320 6f70 7469 6f6e 616c  ctor  # optional
-00000be0: 0a20 2020 2020 2020 207d 290a 0a4d 616b  .        })..Mak
-00000bf0: 6520 7375 7265 203a 636f 6465 3a60 6564  e sure :code:`ed
-00000c00: 6765 5f63 6f6e 7465 7874 6020 6973 2061  ge_context` is a
-00000c10: 6363 6573 7369 626c 6520 6f6e 203a 636f  ccessible on :co
-00000c20: 6465 3a60 7265 7175 6573 7460 206f 626a  de:`request` obj
-00000c30: 6563 7420 6c69 6b65 2073 6f3a 0a0a 2e2e  ect like so:....
-00000c40: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00000c50: 7468 6f6e 0a0a 2020 2020 7265 7175 6573  thon..    reques
-00000c60: 742e 6564 6765 5f63 6f6e 7465 7874 0a0a  t.edge_context..
-00000c70: 0a5b 4f70 7469 6f6e 616c 5d20 4465 6669  .[Optional] Defi
-00000c80: 6e65 2072 6571 7565 7374 2066 6965 6c64  ne request field
-00000c90: 2065 7874 7261 6374 6f72 2066 756e 6374   extractor funct
-00000ca0: 696f 6e20 2860 6578 616d 706c 6520 3c68  ion (`example <h
-00000cb0: 7474 7073 3a2f 2f67 6974 6875 622e 736e  ttps://github.sn
-00000cc0: 6f6f 6775 7473 2e6e 6574 2f72 6564 6469  ooguts.net/reddi
-00000cd0: 742f 7265 6464 6974 2d73 6572 7669 6365  t/reddit-service
-00000ce0: 2d67 7261 7068 716c 2f62 6c6f 622f 6d61  -graphql/blob/ma
-00000cf0: 7374 6572 2f67 7261 7068 716c 2d70 792f  ster/graphql-py/
-00000d00: 6772 6170 6871 6c5f 6170 692f 6d6f 6465  graphql_api/mode
-00000d10: 6c73 2f65 7870 6572 696d 656e 742e 7079  ls/experiment.py
-00000d20: 234c 3637 2d4c 3932 3e60 5f29 0a0a 2e2e  #L67-L92>`_)....
-00000d30: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00000d40: 7468 6f6e 0a0a 2020 2020 2320 4261 7365  thon..    # Base
-00000d50: 706c 6174 6520 6361 6c6c 7320 606d 616b  plate calls `mak
-00000d60: 655f 6f62 6a65 6374 5f66 6f72 5f63 6f6e  e_object_for_con
-00000d70: 7465 7874 2829 6020 616e 6420 6372 6561  text()` and crea
-00000d80: 7465 7320 6120 6044 6563 6964 6572 436f  tes a `DeciderCo
-00000d90: 6e74 6578 7460 0a20 2020 2023 2077 6869  ntext`.    # whi
-00000da0: 6368 2066 6574 6368 6573 2074 6865 2066  ch fetches the f
-00000db0: 6f6c 6c6f 7769 6e67 2066 6965 6c64 7320  ollowing fields 
-00000dc0: 6672 6f6d 2045 6467 6543 6f6e 7465 7874  from EdgeContext
-00000dd0: 2061 7574 6f6d 6174 6963 616c 6c79 3a0a   automatically:.
-00000de0: 2020 2020 2320 2020 2d20 7573 6572 5f69      #   - user_i
-00000df0: 640a 2020 2020 2320 2020 2d20 6465 7669  d.    #   - devi
-00000e00: 6365 5f69 640a 2020 2020 2320 2020 2d20  ce_id.    #   - 
-00000e10: 6c6f 6767 6564 5f69 6e0a 2020 2020 2320  logged_in.    # 
-00000e20: 2020 2d20 636f 6f6b 6965 5f63 7265 6174    - cookie_creat
-00000e30: 6564 5f74 696d 6573 7461 6d70 0a20 2020  ed_timestamp.   
-00000e40: 2023 2020 202d 206f 6175 7468 5f63 6c69   #   - oauth_cli
-00000e50: 656e 745f 6964 0a20 2020 2023 2020 202d  ent_id.    #   -
-00000e60: 2063 6f75 6e74 7279 5f63 6f64 650a 2020   country_code.  
-00000e70: 2020 2320 2020 2d20 6c6f 6361 6c65 0a20    #   - locale. 
-00000e80: 2020 2023 2020 202d 206f 7269 6769 6e5f     #   - origin_
-00000e90: 7365 7276 6963 650a 2020 2020 2320 2020  service.    #   
-00000ea0: 2d20 6973 5f65 6d70 6c6f 7965 650a 2020  - is_employee.  
-00000eb0: 2020 2320 2020 2d20 6c6f 6964 5f63 7265    #   - loid_cre
-00000ec0: 6174 6564 5f6d 730a 0a20 2020 2023 2043  ated_ms..    # C
-00000ed0: 7573 746f 6d69 7a65 6420 6669 656c 6473  ustomized fields
-00000ee0: 2063 616e 2062 6520 6465 6669 6e65 6420   can be defined 
-00000ef0: 6265 6c6f 7720 746f 2062 6520 6578 7472  below to be extr
-00000f00: 6163 7465 6420 6672 6f6d 2061 2062 6173  acted from a bas
-00000f10: 6570 6c61 7465 2072 6571 7565 7374 0a20  eplate request. 
-00000f20: 2020 2023 2061 6e64 2077 696c 6c20 6f76     # and will ov
-00000f30: 6572 7269 6465 2061 626f 7665 2065 6467  erride above edg
-00000f40: 655f 636f 6e74 6578 7420 6669 656c 6473  e_context fields
-00000f50: 2e0a 0a20 2020 2064 6566 206d 795f 6669  ...    def my_fi
-00000f60: 656c 645f 6578 7472 6163 746f 7228 7265  eld_extractor(re
-00000f70: 7175 6573 7429 3a0a 2020 2020 2020 2020  quest):.        
-00000f80: 2320 616e 2065 7861 6d70 6c65 206f 6620  # an example of 
-00000f90: 6375 7374 6f6d 697a 6564 2062 6173 6570  customized basep
-00000fa0: 6c61 7465 2072 6571 7565 7374 2066 6965  late request fie
-00000fb0: 6c64 2065 7874 7261 6374 6f72 3a0a 2020  ld extractor:.  
-00000fc0: 2020 2020 2020 7265 7475 726e 207b 2266        return {"f
-00000fd0: 6f6f 223a 2072 6571 7565 7374 2e68 6561  oo": request.hea
-00000fe0: 6465 7273 2e67 6574 2822 466f 6f22 292c  ders.get("Foo"),
-00000ff0: 2022 6261 7222 3a20 2273 6f6d 6574 6869   "bar": "somethi
-00001000: 6e67 227d 0a0a 0a55 7361 6765 0a2d 2d2d  ng"}...Usage.---
-00001010: 2d2d 2d2d 0a55 7365 2074 6865 2061 7474  ----.Use the att
-00001020: 6163 6865 6420 3a70 793a 636c 6173 733a  ached :py:class:
-00001030: 607e 7265 6464 6974 5f64 6563 6964 6572  `~reddit_decider
-00001040: 2e44 6563 6964 6572 6020 6f62 6a65 6374  .Decider` object
-00001050: 2069 6e20 7265 7175 6573 7420 616e 640a   in request and.
-00001060: 3a63 6f64 653a 6064 6563 6964 6572 2e67  :code:`decider.g
-00001070: 6574 5f76 6172 6961 6e74 2829 6020 2877  et_variant()` (w
-00001080: 6869 6368 2077 696c 6c20 6175 746f 6d61  hich will automa
-00001090: 7469 6361 6c6c 7920 7365 6e64 2061 6e20  tically send an 
-000010a0: 6578 706f 7365 2065 7665 6e74 293a 3a0a  expose event)::.
-000010b0: 0a20 2020 2064 6566 206d 795f 6d65 7468  .    def my_meth
-000010c0: 6f64 2872 6571 7565 7374 293a 0a20 2020  od(request):.   
-000010d0: 2020 2020 2069 6620 7265 7175 6573 742e       if request.
-000010e0: 6465 6369 6465 722e 6765 745f 7661 7269  decider.get_vari
-000010f0: 616e 7428 2266 6f6f 2229 203d 3d20 2262  ant("foo") == "b
-00001100: 6172 223a 0a20 2020 2020 2020 2020 2020  ar":.           
-00001110: 202e 2e2e 0a0a 6f72 206f 7074 696f 6e61   .....or optiona
-00001120: 6c6c 792c 2069 6620 6d61 6e75 616c 2065  lly, if manual e
-00001130: 7870 6f73 7572 6520 6973 206e 6563 6573  xposure is neces
-00001140: 7361 7279 2c20 7573 653a 3a0a 0a20 2020  sary, use::..   
-00001150: 2064 6566 206d 795f 6d65 7468 6f64 2872   def my_method(r
-00001160: 6571 7565 7374 293a 0a20 2020 2020 2020  equest):.       
-00001170: 2076 6172 6961 6e74 203d 2072 6571 7565   variant = reque
-00001180: 7374 2e64 6563 6964 6572 2e67 6574 5f76  st.decider.get_v
-00001190: 6172 6961 6e74 5f77 6974 686f 7574 5f65  ariant_without_e
-000011a0: 7870 6f73 6528 6578 7065 7269 6d65 6e74  xpose(experiment
-000011b0: 5f6e 616d 653d 2765 7870 6572 696d 656e  _name='experimen
-000011c0: 745f 6e61 6d65 2729 0a20 2020 2020 2020  t_name').       
-000011d0: 202e 2e2e 0a20 2020 2020 2020 2072 6571   ....        req
-000011e0: 7565 7374 2e64 6563 6964 6572 2e65 7870  uest.decider.exp
-000011f0: 6f73 6528 6578 7065 7269 6d65 6e74 5f6e  ose(experiment_n
-00001200: 616d 653d 2765 7870 6572 696d 656e 745f  ame='experiment_
-00001210: 6e61 6d65 272c 2076 6172 6961 6e74 5f6e  name', variant_n
-00001220: 616d 653d 7661 7269 616e 7429 0a0a 436f  ame=variant)..Co
-00001230: 6e66 6967 7572 6174 696f 6e20 436c 6173  nfiguration Clas
-00001240: 7365 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ses.------------
-00001250: 2d0a 0a2e 2e20 6175 746f 6675 6e63 7469  -.... autofuncti
-00001260: 6f6e 3a3a 2064 6563 6964 6572 5f63 6c69  on:: decider_cli
-00001270: 656e 745f 6672 6f6d 5f63 6f6e 6669 670a  ent_from_config.
-00001280: 0a0a 2e2e 2061 7574 6f63 6c61 7373 3a3a  .... autoclass::
-00001290: 2044 6563 6964 6572 436c 6965 6e74 0a0a   DeciderClient..
-000012a0: 0a2e 2e20 6175 746f 636c 6173 733a 3a20  ... autoclass:: 
-000012b0: 4465 6369 6465 7243 6f6e 7465 7874 4661  DeciderContextFa
-000012c0: 6374 6f72 790a 0a0a 4465 6369 6465 7220  ctory...Decider 
-000012d0: 4150 490a 2d2d 2d2d 2d2d 2d0a 0a2e 2e20  API.-------.... 
-000012e0: 6175 746f 636c 6173 733a 3a20 4465 6369  autoclass:: Deci
-000012f0: 6465 720a 2020 203a 6d65 6d62 6572 733a  der.   :members:
-00001300: 0a                                       .
+00000000: 202e 2e20 5f72 6564 6469 745f 6465 6369   .. _reddit_deci
+00000010: 6465 723a 0a0a 6060 7265 6464 6974 5f64  der:..``reddit_d
+00000020: 6563 6964 6572 6060 0a3d 3d3d 3d3d 3d3d  ecider``.=======
+00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000040: 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e 2061 7574  ========.... aut
+00000050: 6f6d 6f64 756c 653a 3a20 7265 6464 6974  omodule:: reddit
+00000060: 5f64 6563 6964 6572 0a0a 0a50 7265 7265  _decider...Prere
+00000070: 7175 6973 6974 6520 7061 636b 6167 6573  quisite packages
+00000080: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00000090: 2d2d 2d2d 2d2d 0a2e 2e20 636f 6465 2d62  ------... code-b
+000000a0: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+000000b0: 2020 2062 6173 6570 6c61 7465 3e3d 322e     baseplate>=2.
+000000c0: 302e 300a 0a20 2020 2072 6564 6469 742d  0.0..    reddit-
+000000d0: 6564 6765 636f 6e74 6578 743e 3d31 2e30  edgecontext>=1.0
+000000e0: 2e30 0a0a 2020 2020 2320 7570 6772 6164  .0..    # upgrad
+000000f0: 6520 6f72 2069 6e74 6567 7261 7465 206c  e or integrate l
+00000100: 6174 6573 7420 7265 6464 6974 2d76 322d  atest reddit-v2-
+00000110: 6576 656e 7473 2070 6163 6b61 6765 0a20  events package. 
+00000120: 2020 2023 206f 7220 6d61 6e75 616c 6c79     # or manually
+00000130: 2075 7064 6174 6520 7468 7269 6674 2073   update thrift s
+00000140: 6368 656d 6173 0a20 2020 2023 2074 6f20  chemas.    # to 
+00000150: 616c 6c6f 7720 6576 656e 7420 6669 656c  allow event fiel
+00000160: 6473 2074 6f20 6265 2070 6f70 756c 6174  ds to be populat
+00000170: 6564 2069 6e20 6578 706f 7375 7265 730a  ed in exposures.
+00000180: 2020 2020 7265 6464 6974 2d76 322d 6576      reddit-v2-ev
+00000190: 656e 7473 0a0a 5072 6572 6571 7569 7369  ents..Prerequisi
+000001a0: 7465 2069 6e66 7261 7374 7275 6374 7572  te infrastructur
+000001b0: 650a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e.--------------
+000001c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 5365  -------------.Se
+000001d0: 7420 7570 2079 6f75 7220 7365 7276 6963  t up your servic
+000001e0: 6520 746f 2070 756c 6c20 646f 776e 2026  e to pull down &
+000001f0: 2073 796e 6368 726f 6e69 7a65 2065 7870   synchronize exp
+00000200: 6572 696d 656e 7420 636f 6e66 6967 7572  eriment configur
+00000210: 6174 696f 6e73 2066 726f 6d20 5a6f 6f6b  ations from Zook
+00000220: 6565 7065 7220 7669 6120 7468 6520 4261  eeper via the Ba
+00000230: 7365 706c 6174 6520 606c 6976 652d 6461  seplate `live-da
+00000240: 7461 2077 6174 6368 6572 2073 6964 6563  ta watcher sidec
+00000250: 6172 0a3c 6874 7470 733a 2f2f 6261 7365  ar.<https://base
+00000260: 706c 6174 652e 7265 6164 7468 6564 6f63  plate.readthedoc
+00000270: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
+00000280: 7069 2f62 6173 6570 6c61 7465 2f6c 6962  pi/baseplate/lib
+00000290: 2f6c 6976 655f 6461 7461 2e68 746d 6c3f  /live_data.html?
+000002a0: 6869 6768 6c69 6768 743d 7369 6465 6361  highlight=sideca
+000002b0: 7223 7761 7463 6865 722d 6461 656d 6f6e  r#watcher-daemon
+000002c0: 3e60 5f20 286d 696e 696d 756d 2076 322e  >`_ (minimum v2.
+000002d0: 342e 3133 292e 0a59 6f75 276c 6c20 6861  4.13)..You'll ha
+000002e0: 7665 2074 6f20 6d61 6b65 2073 7572 6520  ve to make sure 
+000002f0: 7468 6174 2079 6f75 7220 7365 7276 6963  that your servic
+00000300: 6520 6973 2061 7574 686f 7269 7a65 6420  e is authorized 
+00000310: 746f 2066 6574 6368 2074 6865 2061 7070  to fetch the app
+00000320: 726f 7072 6961 7465 2073 6563 7265 7420  ropriate secret 
+00000330: 6672 6f6d 2056 6175 6c74 2e0a 0a50 7265  from Vault...Pre
+00000340: 7265 7175 6973 6974 6520 636f 6e66 6967  requisite config
+00000350: 7572 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d  uration.--------
+00000360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000370: 2d2d 2d0a 5365 7475 7020 3a63 6f64 653a  ---.Setup :code:
+00000380: 6072 6564 6469 742d 6578 7065 7269 6d65  `reddit-experime
+00000390: 6e74 7360 2069 6e20 796f 7572 2061 7070  nts` in your app
+000003a0: 6c69 6361 7469 6f6e 2773 2063 6f6e 6669  lication's confi
+000003b0: 6775 7261 7469 6f6e 2066 696c 653a 0a0a  guration file:..
+000003c0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000003d0: 696e 690a 0a20 2020 5b61 7070 3a6d 6169  ini..   [app:mai
+000003e0: 6e5d 0a0a 2020 202e 2e2e 0a0a 2020 2023  n]..   .....   #
+000003f0: 206f 7074 696f 6e61 6c3a 2061 2070 6174   optional: a pat
+00000400: 6820 746f 2074 6865 2066 696c 6520 7768  h to the file wh
+00000410: 6572 6520 6578 7065 7269 6d65 6e74 2063  ere experiment c
+00000420: 6f6e 6669 6775 7261 7469 6f6e 2069 7320  onfiguration is 
+00000430: 7772 6974 7465 6e0a 2020 2023 2028 6465  written.   # (de
+00000440: 6661 756c 743a 202f 7661 722f 6c6f 6361  fault: /var/loca
+00000450: 6c2f 6578 7065 7269 6d65 6e74 732e 6a73  l/experiments.js
+00000460: 6f6e 290a 2020 2065 7870 6572 696d 656e  on).   experimen
+00000470: 7473 2e70 6174 6820 3d20 2f76 6172 2f6c  ts.path = /var/l
+00000480: 6f63 616c 2f66 6f6f 2e6a 736f 6e0a 0a20  ocal/foo.json.. 
+00000490: 2020 2320 6f70 7469 6f6e 616c 3a20 686f    # optional: ho
+000004a0: 7720 6c6f 6e67 2074 6f20 7761 6974 2066  w long to wait f
+000004b0: 6f72 2074 6865 2065 7870 6572 696d 656e  or the experimen
+000004c0: 7473 2066 696c 6520 746f 2065 7869 7374  ts file to exist
+000004d0: 2062 6566 6f72 6520 6661 696c 696e 670a   before failing.
+000004e0: 2020 2023 2028 6465 6661 756c 743a 2064     # (default: d
+000004f0: 6f20 6e6f 7420 7761 6974 2e20 6661 696c  o not wait. fail
+00000500: 2069 6d6d 6564 6961 7465 6c79 2069 6620   immediately if 
+00000510: 6e6f 7420 6176 6169 6c61 626c 6529 0a20  not available). 
+00000520: 2020 6578 7065 7269 6d65 6e74 732e 7469    experiments.ti
+00000530: 6d65 6f75 7420 3d20 3630 2073 6563 6f6e  meout = 60 secon
+00000540: 6473 0a0a 2020 2023 206f 7074 696f 6e61  ds..   # optiona
+00000550: 6c3a 2074 6865 2062 6173 6520 616d 6f75  l: the base amou
+00000560: 6e74 206f 6620 7469 6d65 2066 6f72 2065  nt of time for e
+00000570: 7870 6f6e 656e 7469 616c 2062 6163 6b6f  xponential backo
+00000580: 6666 2077 6869 6c65 2077 6169 7469 6e67  ff while waiting
+00000590: 0a20 2020 2320 666f 7220 7468 6520 6669  .   # for the fi
+000005a0: 6c65 2074 6f20 6265 2061 7661 696c 6162  le to be availab
+000005b0: 6c65 2e0a 2020 2023 2028 6465 6661 756c  le..   # (defaul
+000005c0: 743a 206e 6f20 6261 636b 6f66 6620 7469  t: no backoff ti
+000005d0: 6d65 2062 6574 7765 656e 2074 7269 6573  me between tries
+000005e0: 290a 2020 2065 7870 6572 696d 656e 7473  ).   experiments
+000005f0: 2e62 6163 6b6f 6666 203d 2031 2073 6563  .backoff = 1 sec
+00000600: 6f6e 640a 0a20 2020 2e2e 2e0a 0a0a 496e  ond..   ......In
+00000610: 7465 6772 6174 6520 3a63 6f64 653a 6072  tegrate :code:`r
+00000620: 6564 6469 742d 6578 7065 7269 6d65 6e74  eddit-experiment
+00000630: 7360 2069 6e74 6f20 4261 7365 706c 6174  s` into Baseplat
+00000640: 6520 7365 7276 6963 650a 2d2d 2d2d 2d2d  e service.------
+00000650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000680: 2d2d 2d2d 2d0a 0a55 7067 7261 6465 206f  -----..Upgrade o
+00000690: 7220 696e 7465 6772 6174 6520 7265 6464  r integrate redd
+000006a0: 6974 2d65 7870 6572 696d 656e 7473 2070  it-experiments p
+000006b0: 6163 6b61 6765 3a0a 0a2e 2e20 636f 6465  ackage:.... code
+000006c0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+000006d0: 0a20 2020 2023 2069 6d70 6f72 7420 6c61  .    # import la
+000006e0: 7465 7374 2072 6564 6469 742d 6578 7065  test reddit-expe
+000006f0: 7269 6d65 6e74 7320 7061 636b 6167 6520  riments package 
+00000700: 696e 2073 6572 7669 6365 2072 6571 7569  in service requi
+00000710: 7265 6d65 6e74 732e 7478 740a 2020 2020  rements.txt.    
+00000720: 7265 6464 6974 2d65 7870 6572 696d 656e  reddit-experimen
+00000730: 7473 3e3d 312e 332e 390a 0a49 6e69 7469  ts>=1.3.9..Initi
+00000740: 616c 697a 6520 3a63 6f64 653a 6064 6563  alize :code:`dec
+00000750: 6964 6572 6020 696e 7374 616e 6365 206f  ider` instance o
+00000760: 6e20 4261 7365 706c 6174 6520 636f 6e74  n Baseplate cont
+00000770: 6578 740a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ext.------------
+00000780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000007a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 496e  ------------..In
+000007b0: 2079 6f75 7220 7365 7276 6963 6527 7320   your service's 
+000007c0: 696e 6974 6961 6c69 7a61 7469 6f6e 2070  initialization p
+000007d0: 726f 6365 7373 2c20 6164 6420 6120 3a63  rocess, add a :c
+000007e0: 6f64 653a 6064 6563 6964 6572 6020 696e  ode:`decider` in
+000007f0: 7374 616e 6365 2074 6f20 6261 7365 706c  stance to basepl
+00000800: 6174 6527 7320 636f 6e74 6578 743a 0a28  ate's context:.(
+00000810: 4e6f 7465 2074 6865 2075 7365 206f 6620  Note the use of 
+00000820: 7468 6520 3a63 6f64 653a 6045 7870 6572  the :code:`Exper
+00000830: 696d 656e 744c 6f67 6765 7260 2c20 7768  imentLogger`, wh
+00000840: 6963 6820 6973 2075 7365 6420 746f 2070  ich is used to p
+00000850: 7562 6c69 7368 2065 7870 6f73 7572 6520  ublish exposure 
+00000860: 5632 2065 7665 6e74 732c 0a61 6e20 6578  V2 events,.an ex
+00000870: 616d 706c 6520 6361 6e20 6265 2073 6565  ample can be see
+00000880: 6e20 6068 6572 6520 3c68 7474 7073 3a2f  n `here <https:/
+00000890: 2f67 6974 6875 622e 736e 6f6f 6775 7473  /github.snooguts
+000008a0: 2e6e 6574 2f72 6564 6469 742f 7265 6464  .net/reddit/redd
+000008b0: 6974 2d73 6572 7669 6365 2d67 7261 7068  it-service-graph
+000008c0: 716c 2f62 6c6f 622f 3337 3334 6235 3137  ql/blob/3734b517
+000008d0: 3332 6332 3964 3037 6565 6633 3261 6365  32c29d07eef32ace
+000008e0: 6438 3636 3737 6363 6535 3036 3464 6262  d86677cce5064dbb
+000008f0: 2f67 7261 7068 716c 2d70 792f 6772 6170  /graphql-py/grap
+00000900: 6871 6c5f 6170 692f 6576 656e 7473 2f75  hql_api/events/u
+00000910: 7469 6c73 2e70 7923 4c32 3035 3e60 5f29  tils.py#L205>`_)
+00000920: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+00000930: 3a20 7079 7468 6f6e 0a0a 2020 2020 2320  : python..    # 
+00000940: 6170 706c 6963 6174 696f 6e20 636f 6465  application code
+00000950: 0a20 2020 2066 726f 6d20 7265 6464 6974  .    from reddit
+00000960: 5f64 6563 6964 6572 2069 6d70 6f72 7420  _decider import 
+00000970: 6465 6369 6465 725f 636c 6965 6e74 5f66  decider_client_f
+00000980: 726f 6d5f 636f 6e66 6967 0a20 2020 2066  rom_config.    f
+00000990: 726f 6d20 7265 6464 6974 5f64 6563 6964  rom reddit_decid
+000009a0: 6572 2069 6d70 6f72 7420 4465 6369 6465  er import Decide
+000009b0: 7243 6c69 656e 740a 0a20 2020 2023 206f  rClient..    # o
+000009c0: 7074 696f 6e61 6c0a 2020 2020 6672 6f6d  ptional.    from
+000009d0: 2073 6f6d 655f 6669 6c65 2069 6d70 6f72   some_file impor
+000009e0: 7420 6d79 5f66 6965 6c64 5f65 7874 7261  t my_field_extra
+000009f0: 6374 6f72 0a0a 0a20 2020 2064 6566 206d  ctor...    def m
+00000a00: 616b 655f 7773 6769 5f61 7070 2861 7070  ake_wsgi_app(app
+00000a10: 5f63 6f6e 6669 6729 3a0a 2020 2020 2020  _config):.      
+00000a20: 2020 6261 7365 706c 6174 6520 3d20 4261    baseplate = Ba
+00000a30: 7365 706c 6174 6528 6170 705f 636f 6e66  seplate(app_conf
+00000a40: 6967 290a 2020 2020 2020 2020 6465 6369  ig).        deci
+00000a50: 6465 725f 6661 6374 6f72 7920 3d20 6465  der_factory = de
+00000a60: 6369 6465 725f 636c 6965 6e74 5f66 726f  cider_client_fro
+00000a70: 6d5f 636f 6e66 6967 2861 7070 5f63 6f6e  m_config(app_con
+00000a80: 6669 673d 6170 705f 636f 6e66 6967 2c0a  fig=app_config,.
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ac0: 2020 2020 2065 7665 6e74 5f6c 6f67 6765       event_logge
+00000ad0: 723d 4578 7065 7269 6d65 6e74 4c6f 6767  r=ExperimentLogg
+00000ae0: 6572 2829 2c0a 2020 2020 2020 2020 2020  er(),.          
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b10: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00000b20: 783d 2265 7870 6572 696d 656e 7473 2e22  x="experiments."
+00000b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2020 2020 2020 2072 6571 7565 7374 5f66         request_f
+00000b70: 6965 6c64 5f65 7874 7261 6374 6f72 3d6d  ield_extractor=m
+00000b80: 795f 6669 656c 645f 6578 7472 6163 746f  y_field_extracto
+00000b90: 7229 2020 2320 7468 6973 2069 7320 6f70  r)  # this is op
+00000ba0: 7469 6f6e 616c 2c20 6361 6e20 6265 2060  tional, can be `
+00000bb0: 4e6f 6e65 6020 6966 2065 6467 655f 636f  None` if edge_co
+00000bc0: 6e74 6578 7420 636f 6e74 6169 6e73 2061  ntext contains a
+00000bd0: 6c6c 2074 6865 2066 6965 6c64 7320 796f  ll the fields yo
+00000be0: 7520 6e65 6564 0a20 2020 2020 2020 2062  u need.        b
+00000bf0: 6173 6570 6c61 7465 2e61 6464 5f74 6f5f  aseplate.add_to_
+00000c00: 636f 6e74 6578 7428 2264 6563 6964 6572  context("decider
+00000c10: 222c 2064 6563 6964 6572 5f66 6163 746f  ", decider_facto
+00000c20: 7279 290a 0a20 2020 2020 2020 2023 204f  ry)..        # O
+00000c30: 7220 7573 6520 6044 6563 6964 6572 436c  r use `DeciderCl
+00000c40: 6965 6e74 6020 7769 7468 2060 636f 6e66  ient` with `conf
+00000c50: 6967 7572 655f 636f 6e74 6578 7428 2960  igure_context()`
+00000c60: 2c0a 2020 2020 2020 2020 2320 7768 6963  ,.        # whic
+00000c70: 6820 696e 7465 726e 616c 6c79 2063 616c  h internally cal
+00000c80: 6c73 2060 6465 6369 6465 725f 636c 6965  ls `decider_clie
+00000c90: 6e74 5f66 726f 6d5f 636f 6e66 6967 2829  nt_from_config()
+00000ca0: 600a 2020 2020 2020 2020 6261 7365 706c  `.        basepl
+00000cb0: 6174 652e 636f 6e66 6967 7572 655f 636f  ate.configure_co
+00000cc0: 6e74 6578 7428 7b0a 2020 2020 2020 2020  ntext({.        
+00000cd0: 2020 2020 2264 6563 6964 6572 223a 2044      "decider": D
+00000ce0: 6563 6964 6572 436c 6965 6e74 280a 2020  eciderClient(.  
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00000d00: 6566 6978 3d22 6578 7065 7269 6d65 6e74  efix="experiment
+00000d10: 732e 222c 0a20 2020 2020 2020 2020 2020  s.",.           
+00000d20: 2020 2020 2065 7665 6e74 5f6c 6f67 6765       event_logge
+00000d30: 723d 4578 7065 7269 6d65 6e74 4c6f 6767  r=ExperimentLogg
+00000d40: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00000d50: 2020 2020 7265 7175 6573 745f 6669 656c      request_fiel
+00000d60: 645f 6578 7472 6163 746f 723d 6d79 5f66  d_extractor=my_f
+00000d70: 6965 6c64 5f65 7874 7261 6374 6f72 2020  ield_extractor  
+00000d80: 2320 6f70 7469 6f6e 616c 0a20 2020 2020  # optional.     
+00000d90: 2020 207d 290a 0a4d 616b 6520 7375 7265     })..Make sure
+00000da0: 203a 636f 6465 3a60 4564 6765 436f 6e74   :code:`EdgeCont
+00000db0: 6578 7460 2069 7320 6163 6365 7373 6962  ext` is accessib
+00000dc0: 6c65 206f 6e20 3a63 6f64 653a 6072 6571  le on :code:`req
+00000dd0: 7565 7374 6020 6f62 6a65 6374 206c 696b  uest` object lik
+00000de0: 6520 736f 3a0a 0a2e 2e20 636f 6465 2d62  e so:.... code-b
+00000df0: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+00000e00: 2020 2072 6571 7565 7374 2e65 6467 655f     request.edge_
+00000e10: 636f 6e74 6578 740a 0a0a 5b4f 7074 696f  context...[Optio
+00000e20: 6e61 6c5d 2044 6566 696e 6520 7265 7175  nal] Define requ
+00000e30: 6573 7420 6669 656c 6420 6578 7472 6163  est field extrac
+00000e40: 746f 7220 6675 6e63 7469 6f6e 2028 6065  tor function (`e
+00000e50: 7861 6d70 6c65 203c 6874 7470 733a 2f2f  xample <https://
+00000e60: 6769 7468 7562 2e73 6e6f 6f67 7574 732e  github.snooguts.
+00000e70: 6e65 742f 7265 6464 6974 2f72 6564 6469  net/reddit/reddi
+00000e80: 742d 7365 7276 6963 652d 6772 6170 6871  t-service-graphq
+00000e90: 6c2f 626c 6f62 2f6d 6173 7465 722f 6772  l/blob/master/gr
+00000ea0: 6170 6871 6c2d 7079 2f67 7261 7068 716c  aphql-py/graphql
+00000eb0: 5f61 7069 2f6d 6f64 656c 732f 6578 7065  _api/models/expe
+00000ec0: 7269 6d65 6e74 2e70 7923 4c36 372d 4c39  riment.py#L67-L9
+00000ed0: 323e 605f 290a 0a2e 2e20 636f 6465 2d62  2>`_).... code-b
+00000ee0: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+00000ef0: 2020 2023 2042 6173 6570 6c61 7465 2063     # Baseplate c
+00000f00: 616c 6c73 2060 6d61 6b65 5f6f 626a 6563  alls `make_objec
+00000f10: 745f 666f 725f 636f 6e74 6578 7428 2960  t_for_context()`
+00000f20: 2061 6e64 2063 7265 6174 6573 2061 2060   and creates a `
+00000f30: 4465 6369 6465 7243 6f6e 7465 7874 600a  DeciderContext`.
+00000f40: 2020 2020 2320 7768 6963 6820 6665 7463      # which fetc
+00000f50: 6865 7320 7468 6520 666f 6c6c 6f77 696e  hes the followin
+00000f60: 6720 6669 656c 6473 2066 726f 6d20 4564  g fields from Ed
+00000f70: 6765 436f 6e74 6578 7420 6175 746f 6d61  geContext automa
+00000f80: 7469 6361 6c6c 793a 0a20 2020 2023 2020  tically:.    #  
+00000f90: 202d 2075 7365 725f 6964 0a20 2020 2023   - user_id.    #
+00000fa0: 2020 202d 2064 6576 6963 655f 6964 0a20     - device_id. 
+00000fb0: 2020 2023 2020 202d 206c 6f67 6765 645f     #   - logged_
+00000fc0: 696e 0a20 2020 2023 2020 202d 2063 6f6f  in.    #   - coo
+00000fd0: 6b69 655f 6372 6561 7465 645f 7469 6d65  kie_created_time
+00000fe0: 7374 616d 700a 2020 2020 2320 2020 2d20  stamp.    #   - 
+00000ff0: 6f61 7574 685f 636c 6965 6e74 5f69 640a  oauth_client_id.
+00001000: 2020 2020 2320 2020 2d20 636f 756e 7472      #   - countr
+00001010: 795f 636f 6465 0a20 2020 2023 2020 202d  y_code.    #   -
+00001020: 206c 6f63 616c 650a 2020 2020 2320 2020   locale.    #   
+00001030: 2d20 6f72 6967 696e 5f73 6572 7669 6365  - origin_service
+00001040: 0a20 2020 2023 2020 202d 2069 735f 656d  .    #   - is_em
+00001050: 706c 6f79 6565 0a20 2020 2023 2020 202d  ployee.    #   -
+00001060: 206c 6f69 645f 6372 6561 7465 645f 6d73   loid_created_ms
+00001070: 2028 3e3d 312e 332e 3929 0a0a 2020 2020   (>=1.3.9)..    
+00001080: 2320 4375 7374 6f6d 697a 6564 2066 6965  # Customized fie
+00001090: 6c64 7320 6361 6e20 6265 2064 6566 696e  lds can be defin
+000010a0: 6564 2062 656c 6f77 2074 6f20 6265 2065  ed below to be e
+000010b0: 7874 7261 6374 6564 2066 726f 6d20 6120  xtracted from a 
+000010c0: 6261 7365 706c 6174 6520 7265 7175 6573  baseplate reques
+000010d0: 740a 2020 2020 2320 616e 6420 7769 6c6c  t.    # and will
+000010e0: 206f 7665 7272 6964 6520 6162 6f76 6520   override above 
+000010f0: 6564 6765 5f63 6f6e 7465 7874 2066 6965  edge_context fie
+00001100: 6c64 732e 0a20 2020 2023 2054 6865 7365  lds..    # These
+00001110: 2066 6965 6c64 7320 6d61 7920 6265 2075   fields may be u
+00001120: 7365 6420 666f 7220 7461 7267 6574 696e  sed for targetin
+00001130: 672e 0a0a 2020 2020 6465 6620 6d79 5f66  g...    def my_f
+00001140: 6965 6c64 5f65 7874 7261 6374 6f72 2872  ield_extractor(r
+00001150: 6571 7565 7374 293a 0a20 2020 2020 2020  equest):.       
+00001160: 2023 2061 6e20 6578 616d 706c 6520 6f66   # an example of
+00001170: 2063 7573 746f 6d69 7a65 6420 6261 7365   customized base
+00001180: 706c 6174 6520 7265 7175 6573 7420 6669  plate request fi
+00001190: 656c 6420 6578 7472 6163 746f 723a 0a20  eld extractor:. 
+000011a0: 2020 2020 2020 2072 6574 7572 6e20 7b22         return {"
+000011b0: 666f 6f22 3a20 7265 7175 6573 742e 6865  foo": request.he
+000011c0: 6164 6572 732e 6765 7428 2246 6f6f 2229  aders.get("Foo")
+000011d0: 2c20 2262 6172 223a 2022 736f 6d65 7468  , "bar": "someth
+000011e0: 696e 6722 7d0a 0a0a 4261 7369 6320 5573  ing"}...Basic Us
+000011f0: 6167 650a 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  age.-----------.
+00001200: 5573 6520 7468 6520 6174 7461 6368 6564  Use the attached
+00001210: 203a 7079 3a63 6c61 7373 3a60 7e72 6564   :py:class:`~red
+00001220: 6469 745f 6465 6369 6465 722e 4465 6369  dit_decider.Deci
+00001230: 6465 7260 206f 626a 6563 7420 696e 2072  der` object in r
+00001240: 6571 7565 7374 2074 6f20 6361 6c6c 0a3a  equest to call.:
+00001250: 636f 6465 3a60 6465 6369 6465 722e 6765  code:`decider.ge
+00001260: 745f 7661 7269 616e 7428 2960 2028 6175  t_variant()` (au
+00001270: 746f 6d61 7469 6361 6c6c 7920 7365 6e64  tomatically send
+00001280: 7320 616e 2065 7870 6f73 6520 6576 656e  s an expose even
+00001290: 7429 3a3a 0a0a 2020 2020 6465 6620 6d79  t)::..    def my
+000012a0: 5f6d 6574 686f 6428 7265 7175 6573 7429  _method(request)
+000012b0: 3a0a 2020 2020 2020 2020 6966 2072 6571  :.        if req
+000012c0: 7565 7374 2e64 6563 6964 6572 2e67 6574  uest.decider.get
+000012d0: 5f76 6172 6961 6e74 2822 666f 6f22 2920  _variant("foo") 
+000012e0: 3d3d 2022 6261 7222 3a0a 2020 2020 2020  == "bar":.      
+000012f0: 2020 2020 2020 2e2e 2e0a 0a6f 7220 6f70        .....or op
+00001300: 7469 6f6e 616c 6c79 2c20 6966 206d 616e  tionally, if man
+00001310: 7561 6c20 6578 706f 7375 7265 2069 7320  ual exposure is 
+00001320: 6e65 6365 7373 6172 792c 2075 7365 3a3a  necessary, use::
+00001330: 0a0a 2020 2020 6465 6620 6d79 5f6d 6574  ..    def my_met
+00001340: 686f 6428 7265 7175 6573 7429 3a0a 2020  hod(request):.  
+00001350: 2020 2020 2020 7661 7269 616e 7420 3d20        variant = 
+00001360: 7265 7175 6573 742e 6465 6369 6465 722e  request.decider.
+00001370: 6765 745f 7661 7269 616e 745f 7769 7468  get_variant_with
+00001380: 6f75 745f 6578 706f 7365 2865 7870 6572  out_expose(exper
+00001390: 696d 656e 745f 6e61 6d65 3d27 6578 7065  iment_name='expe
+000013a0: 7269 6d65 6e74 5f6e 616d 6527 290a 2020  riment_name').  
+000013b0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+000013c0: 2020 7265 7175 6573 742e 6465 6369 6465    request.decide
+000013d0: 722e 6578 706f 7365 2865 7870 6572 696d  r.expose(experim
+000013e0: 656e 745f 6e61 6d65 3d27 6578 7065 7269  ent_name='experi
+000013f0: 6d65 6e74 5f6e 616d 6527 2c20 7661 7269  ment_name', vari
+00001400: 616e 745f 6e61 6d65 3d76 6172 6961 6e74  ant_name=variant
+00001410: 290a 0a61 6e64 2074 6869 7320 6973 2061  )..and this is a
+00001420: 6e20 6578 616d 706c 6520 6f66 2075 7369  n example of usi
+00001430: 6e67 2061 2064 796e 616d 6963 2063 6f6e  ng a dynamic con
+00001440: 6669 6775 7261 7469 6f6e 3a3a 0a0a 2020  figuration::..  
+00001450: 2020 6465 6620 6d79 5f6d 6574 686f 6428    def my_method(
+00001460: 7265 7175 6573 7429 3a0a 2020 2020 2020  request):.      
+00001470: 2020 6966 2072 6571 7565 7374 2e64 6563    if request.dec
+00001480: 6964 6572 2e67 6574 5f62 6f6f 6c28 2266  ider.get_bool("f
+00001490: 6f6f 2229 203d 3d20 5472 7565 3a0a 2020  oo") == True:.  
+000014a0: 2020 2020 2020 2020 2020 2e2e 2e0a 0a44            .....D
+000014b0: 6563 6964 6572 2041 5049 0a2d 2d2d 2d2d  ecider API.-----
+000014c0: 2d2d 2d2d 2d2d 0a0a 2e2e 2061 7574 6f63  ------.... autoc
+000014d0: 6c61 7373 3a3a 2044 6563 6964 6572 0a20  lass:: Decider. 
+000014e0: 2020 3a6d 656d 6265 7273 3a0a 0a43 6f6e    :members:..Con
+000014f0: 6669 6775 7261 7469 6f6e 2043 6c61 7373  figuration Class
+00001500: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00001510: 2d2d 2d2d 0a0a 2e2e 2061 7574 6f63 6c61  ----.... autocla
+00001520: 7373 3a3a 2044 6563 6964 6572 436c 6965  ss:: DeciderClie
+00001530: 6e74 0a0a 436f 6e66 6967 7572 6174 696f  nt..Configuratio
+00001540: 6e20 4675 6e63 7469 6f6e 0a2d 2d2d 2d2d  n Function.-----
+00001550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001560: 2d0a 0a2e 2e20 6175 746f 6675 6e63 7469  -.... autofuncti
+00001570: 6f6e 3a3a 2064 6563 6964 6572 5f63 6c69  on:: decider_cli
+00001580: 656e 745f 6672 6f6d 5f63 6f6e 6669 670a  ent_from_config.
+00001590: 0a0a 436f 6e66 6967 7572 6174 696f 6e20  ..Configuration 
+000015a0: 436f 6e74 6578 7420 4661 6374 6f72 790a  Context Factory.
+000015b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e  -------------...
+000015d0: 2e20 6175 746f 636c 6173 733a 3a20 4465  . autoclass:: De
+000015e0: 6369 6465 7243 6f6e 7465 7874 4661 6374  ciderContextFact
+000015f0: 6f72 790a 0a4c 6567 6163 7920 4150 4920  ory..Legacy API 
+00001600: 646f 6373 3a0a 2d2d 2d2d 2d2d 2d2d 2d2d  docs:.----------
+00001610: 2d2d 2d2d 2d2d 0a0a 2e2e 2074 6f63 7472  ------.... toctr
+00001620: 6565 3a3a 0a20 203a 6d61 7864 6570 7468  ee::.  :maxdepth
+00001630: 3a20 310a 0a20 206c 6567 6163 792f 696e  : 1..  legacy/in
+00001640: 6465 780a                                dex.
```

### Comparing `reddit_experiments-1.3.8/reddit_decider/__init__.py` & `reddit_experiments-1.3.9/reddit_decider/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,16 +165,14 @@
 
 class Decider:
     """Access to experiments with automatic refresh when changed.
 
     This decider client allows access to the experiments cached on disk by
     the experiment configuration fetcher daemon.
     It will automatically reload the cache when changed.
-    This client also handles logging bucketing events to the event pipeline
-    when it is determined that the request is part of an active variant.
     """
 
     def __init__(
         self,
         decider_context: DeciderContext,
         config_watcher: FileWatcher,
         server_span: Span,
@@ -345,15 +343,16 @@
         before the user will be exposed to the experiment,
         use :code:`get_variant_without_expose()` to disable exposure events
         and call :code:`expose()` manually later.
 
         :param experiment_name: Name of the experiment you want a variant for.
 
         :param exposure_kwargs:  Additional arguments that will be passed
-            to events_logger (keys must be part of v2 event schema).
+            to :code:`events_logger` (keys must be part of v2 event schema,
+            use dicts for nested fields) under :code:`inputs` and as :code:`kwargs`
 
         :return: Variant name if a variant is assigned, :code:`None` otherwise.
         """
         decider = self._get_decider()
         if decider is None:
             return None
 
@@ -383,17 +382,17 @@
     def get_variant_without_expose(self, experiment_name: str) -> Optional[str]:
         """Return a bucketing variant, if any, without emitting exposure event.
 
         The :code:`expose()` function is available to be manually called afterward.
 
         However, experiments in Holdout Groups will still send an exposure for
         the holdout parent experiment, since it is not possible to
-        manually expose the holdout later (because after exiting this function,
-        it's impossible to know if a returned :code:`None` or :code:`"control_1"` string
-        came from the holdout group or its child experiment).
+        manually expose the holdout later (because it's impossible to know if a
+        returned :code:`None` or :code:`"control_1"` string
+        came from the holdout group or its child experiment once this function exits).
 
         :param experiment_name: Name of the experiment you want a variant for.
 
         :return: Variant name if a variant is assigned, None otherwise.
         """
         decider = self._get_decider()
         if decider is None:
@@ -431,15 +430,16 @@
         since :code:`get_variant()` emits exposure event automatically.
 
         :param experiment_name: Name of the experiment that was exposed.
 
         :param variant_name: Name of the variant that was exposed.
 
         :param exposure_kwargs: Additional arguments that will be passed
-            to events_logger (keys must be part of v2 event schema).
+            to :code:`events_logger` (keys must be part of v2 event schema,
+            use dicts for nested fields) under :code:`inputs` and as :code:`kwargs`
         """
         decider = self._get_decider()
         if decider is None:
             return
 
         experiment = decider.get_experiment(experiment_name)
         error = experiment.err()
@@ -475,30 +475,31 @@
     def get_variant_for_identifier(
         self,
         experiment_name: str,
         identifier: str,
         identifier_type: Literal["user_id", "device_id", "canonical_url"],
         **exposure_kwargs: Optional[Dict[str, Any]],
     ) -> Optional[str]:
-        """Return a bucketing variant for identifier, if any, with auto-exposure.
+        """Return a bucketing variant, if any, with auto-exposure for a given :code:`identifier`.
 
         Since calling :code:`get_variant_for_identifier()` will fire an exposure event, it
         is best to call it when you are sure the user will be exposed to the experiment.
 
         :param experiment_name: Name of the experiment you want a variant for.
 
         :param identifier: an arbitary string used to bucket the experiment by
             being set on :code:`DeciderContext`'s :code:`identifier_type` field.
 
-        :param identifier_type: (one of ["user_id", "device_id", "canonical_url"])
-            Sets :code:`{identifier_type: identifier}` on DeciderContext and
+        :param identifier_type: Sets :code:`{identifier_type: identifier}` on DeciderContext and
             should match an experiment's :code:`bucket_val` to get a variant.
 
-        :param exposure_kwargs:  Additional arguments that will be passed
-            to events_logger under "inputs" key.
+        :param exposure_kwargs: Additional arguments that will be passed
+            to :code:`events_logger` (keys must be part of v2 event schema,
+            use dicts for nested fields) under :code:`inputs` and as :code:`kwargs`
+
 
         :return: Variant name if a variant is assigned, None otherwise.
         """
         if identifier_type not in IDENTIFIERS:
             logger.warning(
                 f'"{identifier_type}" is not one of supported "identifier_type": {IDENTIFIERS}.'
             )
@@ -539,32 +540,31 @@
 
     def get_variant_for_identifier_without_expose(
         self,
         experiment_name: str,
         identifier: str,
         identifier_type: Literal["user_id", "device_id", "canonical_url"],
     ) -> Optional[str]:
-        """Return a bucketing variant for :code:`identifier`, if any, without emitting exposure event.
+        """Return a bucketing variant, if any, without emitting exposure event for a given :code:`identifier`.
 
         The :code:`expose()` function is available to be manually called afterward to emit
         exposure event.
 
         However, experiments in Holdout Groups will still send an exposure for
         the holdout parent experiment, since it is not possible to
-        manually expose the holdout later (because after exiting this function,
-        it's impossible to know if a returned :code:`None` or :code:`"control_1"` string
-        came from the holdout group or its child experiment).
+        manually expose the holdout later (because it's impossible to know if a
+        returned :code:`None` or :code:`"control_1"` string
+        came from the holdout group or its child experiment once this function exits).
 
         :param experiment_name: Name of the experiment you want a variant for.
 
         :param identifier: an arbitary string used to bucket the experiment by
             being set on :code:`DeciderContext`'s :code:`identifier_type` field.
 
-        :param identifier_type: (one of ["user_id", "device_id", "canonical_url"])
-            Sets :code:`{identifier_type: identifier}` on DeciderContext and
+        :param identifier_type: Sets :code:`{identifier_type: identifier}` on DeciderContext and
             should match an experiment's :code:`bucket_val` to get a variant.
 
         :return: Variant name if a variant is assigned, None otherwise.
         """
         if identifier_type not in IDENTIFIERS:
             logger.warning(
                 f'"{identifier_type}" is not one of supported "identifier_type": {IDENTIFIERS}.'
@@ -611,30 +611,29 @@
                 [
                     {
                         "id": 1,
                         "name": "variant_1",
                         "version": "1",
                         "experimentName": "exp_1"
 
-                    },
-                    ...
+                    }
                 ]
 
             If an experiment has a variant of :code:`None`, it is not included
             in the returned list. All available experiments get bucketed.
             Exposure events are not emitted.
 
         The :code:`expose()` function is available to be manually called afterward to emit
         exposure event.
 
         However, experiments in Holdout Groups will still send an exposure for
         the holdout parent experiment, since it is not possible to
-        manually expose the holdout later (because after exiting this function,
-        it's impossible to know if a returned :code:`None` or :code:`"control_1"` string
-        came from the holdout group or its child experiment).
+        manually expose the holdout later (because it's impossible to know if a
+        returned :code:`None` or :code:`"control_1"` string
+        came from the holdout group or its child experiment once this function exits).
 
         :return: list of experiment dicts with non-:code:`None` variants.
         """
         decider = self._get_decider()
         if decider is None:
             return []
 
@@ -674,43 +673,41 @@
                 self._send_expose_if_holdout(event=event, exposure_fields=event_context_fields)
 
         return parsed_choices
 
     def get_all_variants_for_identifier_without_expose(
         self, identifier: str, identifier_type: Literal["user_id", "device_id", "canonical_url"]
     ) -> List[Dict[str, Union[str, int]]]:
-        """Return a list of experiment dicts in this format:
+        """Return a list of experiment dicts for a given :code:`identifier` in this format:
 
                 .. code-block:: json
 
                     [
                         {
                             "id": 1,
                             "name": "variant_1",
                             "version": "1",
                             "experimentName": "exp_1"
 
-                        },
-                        ...
+                        }
                     ]
             If an experiment has a variant of :code:`None`, it is not included
             in the returned list. All available experiments get bucketed.
             Exposure events are not emitted.
 
         However, experiments in Holdout Groups will still send an exposure for
         the holdout parent experiment, since it is not possible to
-        manually expose the holdout later (because after exiting this function,
-        it's impossible to know if a returned :code:`None` or :code:`"control_1"` string
-        came from the holdout group or its child experiment).
+        manually expose the holdout later (because it's impossible to know if a
+        returned :code:`None` or :code:`"control_1"` string
+        came from the holdout group or its child experiment once this function exits).
 
         :param identifier: an arbitary string used to bucket the experiment by
             being set on :code:`DeciderContext`'s :code:`identifier_type` field.
 
-        :param identifier_type: (one of ["user_id", "device_id", "canonical_url"])
-            Sets :code:`{identifier_type: identifier}` on DeciderContext and
+        :param identifier_type: Sets :code:`{identifier_type: identifier}` on DeciderContext and
             should match an experiment's :code:`bucket_val` to get a variant.
 
         :return: list of experiment dicts with non-:code:`None` variants.
         """
         if identifier_type not in IDENTIFIERS:
             logger.warning(
                 f'"{identifier_type}" is not one of supported "identifier_type": {IDENTIFIERS}.'
@@ -781,65 +778,112 @@
         if error:
             logger.warning(f"Encountered error {decider_func.__name__}: {error}")
             return default
 
         return res.val()
 
     def get_bool(self, feature_name: str, default: bool = False) -> bool:
+        """Fetch a Dynamic Configuration of boolean type.
+
+        :param feature_name: Name of the dynamic config you want a value for.
+
+        :param default: what is returned if dynamic config is not active
+            (:code:`False` unless overriden).
+
+        :return: the boolean value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
+        """
         decider = self._get_decider()
         if not decider:
             return default
         return self._get_dynamic_config_value(feature_name, decider.get_bool, default)
 
     def get_int(self, feature_name: str, default: int = 0) -> int:
+        """Fetch a Dynamic Configuration of int type.
+
+        :param feature_name: Name of the dynamic config you want a value for.
+
+        :param default: what is returned if dynamic config is not active
+            (:code:`0` unless overriden).
+
+        :return: the int value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
+        """
         decider = self._get_decider()
         if not decider:
             return default
         return self._get_dynamic_config_value(feature_name, decider.get_int, default)
 
     def get_float(self, feature_name: str, default: float = 0.0) -> float:
+        """Fetch a Dynamic Configuration of float type.
+
+        :param feature_name: Name of the dynamic config you want a value for.
+
+        :param default: what is returned if dynamic config is not active
+            (:code:`0.0` unless overriden).
+
+        :return: the float value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
+        """
         decider = self._get_decider()
         if not decider:
             return default
         return self._get_dynamic_config_value(feature_name, decider.get_float, default)
 
     def get_string(self, feature_name: str, default: str = "") -> str:
+        """Fetch a Dynamic Configuration of string type.
+
+        :param feature_name: Name of the dynamic config you want a value for.
+
+        :param default: what is returned if dynamic config is not active
+            (:code:`""` unless overriden).
+
+        :return: the string value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
+        """
         decider = self._get_decider()
         if not decider:
             return default
         return self._get_dynamic_config_value(feature_name, decider.get_string, default)
 
     def get_map(self, feature_name: str, default: Optional[dict] = None) -> Optional[dict]:
+        """Fetch a Dynamic Configuration of map type.
+
+        :param feature_name: Name of the dynamic config you want a value for.
+
+        :param default: what is returned if dynamic config is not active
+            (:code:`None` unless overriden).
+
+        :return: the map value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
+        """
         decider = self._get_decider()
         if not decider:
             return default
         return self._get_dynamic_config_value(feature_name, decider.get_map, default)
 
     def get_all_dynamic_configs(self) -> List[Dict[str, Any]]:
         """Return a list of dynamic configuration dicts in this format:
 
             .. code-block:: json
 
                 [
                     {
                         "name": "example_dc",
                         "type": "float",
-                        "value": 1.0,
-                    },
-                    ...
+                        "value": 1.0
+                    }
                 ]
 
         where "type" field can be one of:
-            "boolean", "integer", "float", "string", or "map"
+
+            .. code-block:: python
+
+                "boolean", "integer", "float", "string", "map"
 
         Dynamic Configurations that are malformed, fail parsing, or otherwise
         error for any reason are included in the response and have their respective default
         values set:
 
-        .. code-block:: json
+        .. code-block:: python
 
             "boolean" -> False
             "integer" -> 0
             "float"   -> 0.0
             "string"  -> ""
             "map"     -> {}
 
@@ -877,19 +921,21 @@
 
             if value_dict:
                 parsed_configs.append(value_dict)
 
         return parsed_configs
 
     def get_experiment(self, experiment_name: str) -> Optional[ExperimentConfig]:
-        """Get an :code:`ExperimentConfig` (dataclass) representation of an experiment or :code:`None` if not found.
+        """Get an :py:class:`~reddit_decider.ExperimentConfig` `dataclass <https://github.com/reddit/experiments.py/blob/728a9501faceab7072f9d62f4e391fa4c34a68b1/reddit_decider/__init__.py#L39-L47>`_
+        representation of an experiment or :code:`None` if not found.
 
         :param experiment_name: Name of the experiment to be fetched.
 
-        :return: an :code:`ExperimentConfig` dataclass representation of an experiment if found, else :code:`None`.
+        :return: an :py:class:`~reddit_decider.ExperimentConfig` `dataclass <https://github.com/reddit/experiments.py/blob/728a9501faceab7072f9d62f4e391fa4c34a68b1/reddit_decider/__init__.py#L39-L47>`_
+            representation of an experiment if found, else :code:`None`.
         """
         decider = self._get_decider()
         if decider is None:
             return None
 
         experiment = decider.get_experiment(experiment_name)
         error = experiment.err()
@@ -927,25 +973,27 @@
         will be created and used.
     :param timeout: How long, in seconds, to block instantiation waiting
         for the watched experiments file to become available (defaults to not
         blocking).
     :param backoff: retry backoff time for experiments file watcher. Defaults to
         None, which is mapped to DEFAULT_FILEWATCHER_BACKOFF.
     :param request_field_extractor: an optional function used to populate fields such as
-        "app_name" & "build_number" in DeciderContext() via :code:`extracted_fields` arg
+        "app_name" & "build_number" in DeciderContext() that may be used for targeting
 
     """
 
     def __init__(
         self,
         path: str,
         event_logger: Optional[EventLogger] = None,
         timeout: Optional[float] = None,
         backoff: Optional[float] = None,
-        request_field_extractor: Optional[Callable[[RequestContext], Dict[str, str]]] = None,
+        request_field_extractor: Optional[
+            Callable[[RequestContext], Dict[str, Union[str, int, float, bool]]]
+        ] = None,
     ):
         self._filewatcher = FileWatcher(
             path=path, parser=init_decider_parser, timeout=timeout, backoff=backoff
         )
         self._event_logger = event_logger
         self._request_field_extractor = request_field_extractor
 
@@ -1157,22 +1205,24 @@
     See :py:func:`decider_client_from_config` for available configuration settings.
 
     :param event_logger: The EventLogger instance to be used to log bucketing events.
 
     :param prefix: the prefix used to filter config keys (defaults to "experiments.").
 
     :param request_field_extractor: (optional) function used to populate fields such as
-        :code:`"app_name"` & :code:`"build_number"` in :code:`DeciderContext()` via :code:`extracted_fields` arg
+        :code:`"app_name"` & :code:`"build_number"` in :code:`DeciderContext()` that may be used for targeting
     """
 
     def __init__(
         self,
         event_logger: EventLogger,
         prefix: str = "experiments.",
-        request_field_extractor: Optional[Callable[[RequestContext], Dict[str, str]]] = None,
+        request_field_extractor: Optional[
+            Callable[[RequestContext], Dict[str, Union[str, int, float, bool]]]
+        ] = None,
     ):
         self._prefix = prefix
         self._event_logger = event_logger
         self._request_field_extractor = request_field_extractor
 
     def parse(self, _key_path: str, raw_config: config.RawConfig) -> DeciderContextFactory:
         # `_key_path` is ignored for prefix because most services will not change `app_config`
@@ -1185,40 +1235,41 @@
         )
 
 
 def decider_client_from_config(
     app_config: config.RawConfig,
     event_logger: EventLogger,
     prefix: str = "experiments.",
-    request_field_extractor: Optional[Callable[[RequestContext], Dict[str, str]]] = None,
+    request_field_extractor: Optional[
+        Callable[[RequestContext], Dict[str, Union[str, int, float, bool]]]
+    ] = None,
 ) -> DeciderContextFactory:
     """Configure and return an :py:class:`DeciderContextFactory` object.
 
-    The keys useful to :py:func:`decider_client_from_config` should be prefixed, e.g.
+    The keys used in your app's :code:`some_config.ini` file should be prefixed, e.g.
     ``experiments.path``, etc.
 
-    Supported keys:
+    Supported config keys:
 
-    ``path`` (optional)
-        The path to the experiment configuration file generated by the
-        experiment configuration fetcher daemon.
-    ``timeout`` (optional)
-        The time that we should wait for the file specified by ``path`` to
-        exist.  Defaults to `None` which is `infinite`.
-    ``backoff`` (optional)
-        The base amount of time for exponential backoff when trying to find the
-        experiments config file. Defaults to no backoff between tries.
-    ``request_field_extractor`` (optional) function used to populate fields such as
-        "app_name" & "build_number" in DeciderContext() via `extracted_fields` arg
+        ``path`` (optional)
+            The path to the experiment configuration file generated by the
+            experiment configuration fetcher daemon.
+        ``timeout`` (optional)
+            The time that we should wait for the file specified by ``path`` to
+            exist.  Defaults to `None` which is `infinite`.
+        ``backoff`` (optional)
+            The base amount of time for exponential backoff when trying to find the
+            experiments config file. Defaults to no backoff between tries.
 
-    :param raw_config: The application configuration which should have
-        settings for the experiments client.
+    :param app_config: The application configuration which should have
+        settings for the decider client.
     :param event_logger: The EventLogger to be used to log bucketing events.
     :param prefix: the prefix used to filter keys (defaults to "experiments.").
-
+    :param request_field_extractor: (optional) function used to populate fields such as
+        "app_name" & "build_number" in DeciderContext() that may be used for targeting
     """
     assert prefix.endswith(".")
     config_prefix = prefix[:-1]
 
     cfg = config.parse_config(
         app_config,
         {
```

### Comparing `reddit_experiments-1.3.8/reddit_experiments/__init__.py` & `reddit_experiments-1.3.9/reddit_experiments/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,28 +344,28 @@
 
 
 def experiments_client_from_config(
     app_config: config.RawConfig, event_logger: EventLogger, prefix: str = "experiments."
 ) -> ExperimentsContextFactory:
     """Configure and return an :py:class:`ExperimentsContextFactory` object.
 
-    The keys useful to :py:func:`experiments_client_from_config` should be prefixed, e.g.
+    The keys used in your app's :code:`some_config.ini` file should be prefixed, e.g.
     ``experiments.path``, etc.
 
-    Supported keys:
+    Supported config keys:
 
-    ``path`` (optional)
-        The path to the experiment configuration file generated by the
-        experiment configuration fetcher daemon.
-    ``timeout`` (optional)
-        The time that we should wait for the file specified by ``path`` to
-        exist.  Defaults to `None` which is `infinite`.
-    ``backoff`` (optional)
-        The base amount of time for exponential backoff when trying to find the
-        experiments config file. Defaults to no backoff between tries.
+        ``path`` (optional)
+            The path to the experiment configuration file generated by the
+            experiment configuration fetcher daemon.
+        ``timeout`` (optional)
+            The time that we should wait for the file specified by ``path`` to
+            exist.  Defaults to `None` which is `infinite`.
+        ``backoff`` (optional)
+            The base amount of time for exponential backoff when trying to find the
+            experiments config file. Defaults to no backoff between tries.
 
     :param raw_config: The application configuration which should have
         settings for the experiments client.
     :param event_logger: The EventLogger to be used to log bucketing events.
     :param prefix: the prefix used to filter keys (defaults to "experiments.").
 
     """
```

### Comparing `reddit_experiments-1.3.8/reddit_experiments/providers/__init__.py` & `reddit_experiments-1.3.9/reddit_experiments/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/providers/base.py` & `reddit_experiments-1.3.9/reddit_experiments/providers/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/providers/feature_flag.py` & `reddit_experiments-1.3.9/reddit_experiments/providers/feature_flag.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/providers/forced_variant.py` & `reddit_experiments-1.3.9/reddit_experiments/providers/forced_variant.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/providers/r2.py` & `reddit_experiments-1.3.9/reddit_experiments/providers/r2.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/providers/simple_experiment.py` & `reddit_experiments-1.3.9/reddit_experiments/providers/simple_experiment.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/targeting/tree_targeting.py` & `reddit_experiments-1.3.9/reddit_experiments/targeting/tree_targeting.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/variant_sets/base.py` & `reddit_experiments-1.3.9/reddit_experiments/variant_sets/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/variant_sets/multi_variant_set.py` & `reddit_experiments-1.3.9/reddit_experiments/variant_sets/multi_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/variant_sets/range_variant_set.py` & `reddit_experiments-1.3.9/reddit_experiments/variant_sets/range_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/variant_sets/rollout_variant_set.py` & `reddit_experiments-1.3.9/reddit_experiments/variant_sets/rollout_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments/variant_sets/single_variant_set.py` & `reddit_experiments-1.3.9/reddit_experiments/variant_sets/single_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/reddit_experiments.egg-info/PKG-INFO` & `reddit_experiments-1.3.9/reddit_experiments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-experiments
-Version: 1.3.8
+Version: 1.3.9
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
```

### Comparing `reddit_experiments-1.3.8/reddit_experiments.egg-info/SOURCES.txt` & `reddit_experiments-1.3.9/reddit_experiments.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 .dockerignore
 .gitignore
+.readthedocs.yaml
 Dockerfile
 LICENSE
 Makefile
 README.md
 pyproject.toml
 requirements-transitive.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/python-package.yaml
 .github/workflows/python-publish.yaml
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
+docs/images/ddg-logo.png
+docs/images/favicon.png
+docs/legacy/index.rst
 reddit_decider/__init__.py
 reddit_experiments/__init__.py
 reddit_experiments/py.typed
 reddit_experiments.egg-info/PKG-INFO
 reddit_experiments.egg-info/SOURCES.txt
 reddit_experiments.egg-info/dependency_links.txt
 reddit_experiments.egg-info/requires.txt
```

### Comparing `reddit_experiments-1.3.8/requirements-transitive.txt` & `reddit_experiments-1.3.9/requirements-transitive.txt`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/setup.cfg` & `reddit_experiments-1.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/setup.py` & `reddit_experiments-1.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     use_scm_version=True,
     packages=find_packages(),
     python_requires=">=3.7",
     setup_requires=["setuptools_scm"],
     install_requires=[
         "baseplate>=2.0.0a1,<3.0",
         "reddit-edgecontext>=1.0.0a3,<2.0",
-        "reddit-decider>=1.2.15",
-        "typing_extensions>=3.10.0.0",
+        "reddit-decider>=1.2.18,<2.0",
+        "typing_extensions>=3.10.0.0,<5.0",
     ],
     package_data={"reddit_experiments": ["py.typed"]},
     zip_safe=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
```

### Comparing `reddit_experiments-1.3.8/tests/decider_tests.py` & `reddit_experiments-1.3.9/tests/decider_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/experiment_tests.py` & `reddit_experiments-1.3.9/tests/experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/feature_flag_tests.py` & `reddit_experiments-1.3.9/tests/providers/feature_flag_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/forced_variant_tests.py` & `reddit_experiments-1.3.9/tests/providers/forced_variant_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/r2_tests.py` & `reddit_experiments-1.3.9/tests/providers/r2_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/simple_experiment_tests.py` & `reddit_experiments-1.3.9/tests/providers/simple_experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/variant_sets/multi_variant_set_tests.py` & `reddit_experiments-1.3.9/tests/providers/variant_sets/multi_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/variant_sets/range_variant_set_tests.py` & `reddit_experiments-1.3.9/tests/providers/variant_sets/range_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/variant_sets/rollout_variant_set_tests.py` & `reddit_experiments-1.3.9/tests/providers/variant_sets/rollout_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/providers/variant_sets/single_variant_set_tests.py` & `reddit_experiments-1.3.9/tests/providers/variant_sets/single_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/range_variant_tests/data/original_zk_config.json` & `reddit_experiments-1.3.9/tests/range_variant_tests/data/original_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/range_variant_tests/data/output.json` & `reddit_experiments-1.3.9/tests/range_variant_tests/data/output.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/range_variant_tests/data/range_variant_zk_config.json` & `reddit_experiments-1.3.9/tests/range_variant_tests/data/range_variant_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/range_variant_tests/range_variant_parity_tests.py` & `reddit_experiments-1.3.9/tests/range_variant_tests/range_variant_parity_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.8/tests/targeting/tree_targeting_tests.py` & `reddit_experiments-1.3.9/tests/targeting/tree_targeting_tests.py`

 * *Files identical despite different names*

