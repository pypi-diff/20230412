# Comparing `tmp/gt4sd-1.1.9.tar.gz` & `tmp/gt4sd-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gt4sd-1.1.9.tar", last modified: Fri Feb 17 14:49:07 2023, max compression
+gzip compressed data, was "gt4sd-1.2.0.tar", last modified: Wed Apr 12 16:09:51 2023, max compression
```

## Comparing `gt4sd-1.1.9.tar` & `gt4sd-1.2.0.tar`

### file list

```diff
@@ -1,403 +1,406 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.050887 gt4sd-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-17 14:48:57.000000 gt4sd-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-02-17 14:49:07.050887 gt4sd-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-02-17 14:48:57.000000 gt4sd-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-17 14:48:57.000000 gt4sd-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-02-17 14:49:07.054887 gt4sd-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-17 14:48:57.000000 gt4sd-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:06.998886 gt4sd-1.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.010887 gt4sd-1.1.9/src/gt4sd/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.010887 gt4sd-1.1.9/src/gt4sd/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.010887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.010887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29460 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.010887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/key_bert/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/key_bert/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/molgx/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/molgx/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/paccmann_rl/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    49969 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/template/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/template/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/template/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.014887 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    34978 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.018887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/hugging_face/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/hugging_face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/hugging_face/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/hugging_face/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.022887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/moler/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/moler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/moler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/moler/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.022887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/paccmann_vae/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/paccmann_vae/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.022887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/pgt/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/pgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/pgt/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/pgt/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.022887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/polymer_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/polymer_blocks/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.022887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   128648 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/mol_dct.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_moler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_pgt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_torchdrug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.022887 gt4sd-1.1.9/src/gt4sd/algorithms/generation/torchdrug/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/torchdrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/torchdrug/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/generation/torchdrug/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.022887 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/paccmann/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/paccmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/paccmann/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/paccmann/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/tests/test_paccmann.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/topics_zero_shot/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/algorithms/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/argument_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4380 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/hf_to_st_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6910 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/load_arguments_from_dataclass.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4235 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/pl_to_hf_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7893 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/saving.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/trainer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8169 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/cli/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/domains/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/domains/materials/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/domains/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/domains/materials/protein_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/domains/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/domains/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.026887 gt4sd-1.1.9/src/gt4sd/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/cgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/cgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/cgcnn/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/cgcnn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32266 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/feature_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/tests/test_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/arg_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/arg_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/arg_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/loss/td_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.030887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34044 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/tests/qm9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/tests/test_gfn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/train/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/train/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/arg_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/arg_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/arg_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/arg_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.034887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    35475 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/no_encoding/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_mlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_rnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/granular/train/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/granular/train/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/frameworks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/frameworks/torch/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/properties/crystals/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/crystals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/crystals/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.038887 gt4sd-1.1.9/src/gt4sd/properties/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22654 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/molecules/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/molecules/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/properties/proteins/
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/proteins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/proteins/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/proteins/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/properties/scores/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/scores/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/properties/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/tests/test_properties_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/properties/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/training_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/training_pipelines/cgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/cgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/cgcnn/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/training_pipelines/crystals_crf/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/crystals_crf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/crystals_crf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/training_pipelines/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/diffusion/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/mock_training_pipeline.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.042887 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/organ/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/organ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/organ/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/vae/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/vae/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/vae/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/vae/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/granular/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/lm_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.046887 gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16348 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/terminator_training.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.050887 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/molecules.smi
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_cgnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_gflownet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_language_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.050887 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.050887 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/gcpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.050887 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/graphaf/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-02-17 14:48:57.000000 gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/unpatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:49:07.010887 gt4sd-1.1.9/src/gt4sd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-02-17 14:49:06.000000 gt4sd-1.1.9/src/gt4sd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-02-17 14:49:06.000000 gt4sd-1.1.9/src/gt4sd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:49:06.000000 gt4sd-1.1.9/src/gt4sd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-17 14:49:06.000000 gt4sd-1.1.9/src/gt4sd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-17 14:49:06.000000 gt4sd-1.1.9/src/gt4sd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-17 14:49:06.000000 gt4sd-1.1.9/src/gt4sd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.260422 gt4sd-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 16:09:37.000000 gt4sd-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-04-12 16:09:51.260422 gt4sd-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-04-12 16:09:37.000000 gt4sd-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-12 16:09:37.000000 gt4sd-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-12 16:09:51.264422 gt4sd-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 16:09:37.000000 gt4sd-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.116417 gt4sd-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.136417 gt4sd-1.2.0/src/gt4sd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.140417 gt4sd-1.2.0/src/gt4sd/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.140417 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.140417 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29460 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.144418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.144418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/key_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/key_bert/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.148418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/molgx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/molgx/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.148418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.152418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51522 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.152418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.152418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.156418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/template/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/template/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.156418 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.156418 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.156418 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.160418 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.160418 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.160418 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.160418 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.164418 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34978 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.164418 gt4sd-1.2.0/src/gt4sd/algorithms/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.164418 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.164418 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.164418 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.168419 gt4sd-1.2.0/src/gt4sd/algorithms/generation/hugging_face/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/hugging_face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/hugging_face/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/hugging_face/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.168419 gt4sd-1.2.0/src/gt4sd/algorithms/generation/moler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/moler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/moler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/moler/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.168419 gt4sd-1.2.0/src/gt4sd/algorithms/generation/paccmann_vae/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/paccmann_vae/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.168419 gt4sd-1.2.0/src/gt4sd/algorithms/generation/pgt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/pgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/pgt/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/pgt/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.168419 gt4sd-1.2.0/src/gt4sd/algorithms/generation/polymer_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/polymer_blocks/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.172419 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128648 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/mol_dct.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_moler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_pgt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_torchdrug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.172419 gt4sd-1.2.0/src/gt4sd/algorithms/generation/torchdrug/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/torchdrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/torchdrug/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/generation/torchdrug/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.172419 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.172419 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/paccmann/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/paccmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/paccmann/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/paccmann/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.176419 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/tests/test_paccmann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.176419 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/topics_zero_shot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.176419 gt4sd-1.2.0/src/gt4sd/algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/algorithms/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.184419 gt4sd-1.2.0/src/gt4sd/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/argument_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4380 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/hf_to_st_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6910 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/load_arguments_from_dataclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4235 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/pl_to_hf_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7893 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/saving.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/trainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8169 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/cli/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.184419 gt4sd-1.2.0/src/gt4sd/domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/domains/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.184419 gt4sd-1.2.0/src/gt4sd/domains/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/domains/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/domains/materials/protein_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.184419 gt4sd-1.2.0/src/gt4sd/domains/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/domains/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.184419 gt4sd-1.2.0/src/gt4sd/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.188419 gt4sd-1.2.0/src/gt4sd/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.188419 gt4sd-1.2.0/src/gt4sd/frameworks/cgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/cgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/cgcnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/cgcnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.188419 gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32266 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/feature_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.188419 gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.192419 gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/tests/test_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.192419 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.192419 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/arg_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/arg_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/arg_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.192419 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.196420 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.196420 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/loss/td_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.196420 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.196420 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34044 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.200420 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/tests/qm9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/tests/test_gfn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.200420 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/train/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.200420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.204420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/arg_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/arg_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/arg_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/arg_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.204420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.204420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.208420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.208420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.212420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35475 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.212420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.212420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.212420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.212420 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.216421 gt4sd-1.2.0/src/gt4sd/frameworks/granular/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.216421 gt4sd-1.2.0/src/gt4sd/frameworks/granular/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.216421 gt4sd-1.2.0/src/gt4sd/frameworks/granular/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/granular/train/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.216421 gt4sd-1.2.0/src/gt4sd/frameworks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/frameworks/torch/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.216421 gt4sd-1.2.0/src/gt4sd/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.220421 gt4sd-1.2.0/src/gt4sd/properties/crystals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/crystals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/crystals/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.220421 gt4sd-1.2.0/src/gt4sd/properties/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30897 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/molecules/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/molecules/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.224421 gt4sd-1.2.0/src/gt4sd/properties/proteins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/proteins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/proteins/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/proteins/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.224421 gt4sd-1.2.0/src/gt4sd/properties/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/scores/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.228421 gt4sd-1.2.0/src/gt4sd/properties/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/tests/test_properties_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/properties/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.228421 gt4sd-1.2.0/src/gt4sd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.232421 gt4sd-1.2.0/src/gt4sd/training_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.232421 gt4sd-1.2.0/src/gt4sd/training_pipelines/cgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/cgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/cgcnn/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.232421 gt4sd-1.2.0/src/gt4sd/training_pipelines/crystals_crf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/crystals_crf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/crystals_crf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.236421 gt4sd-1.2.0/src/gt4sd/training_pipelines/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/diffusion/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.236421 gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.236421 gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/mock_training_pipeline.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.236421 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.236421 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/organ/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/organ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/organ/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.240421 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/vae/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.240421 gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.240421 gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/vae/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.240421 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.244422 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.244422 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.252422 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/lm_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.252422 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.252422 gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/terminator_training.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.260422 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/molecules.smi
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_cgnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_gflownet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_language_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.260422 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.260422 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/gcpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.260422 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/graphaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-12 16:09:37.000000 gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/unpatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:09:51.140417 gt4sd-1.2.0/src/gt4sd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-04-12 16:09:51.000000 gt4sd-1.2.0/src/gt4sd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16224 2023-04-12 16:09:51.000000 gt4sd-1.2.0/src/gt4sd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:09:51.000000 gt4sd-1.2.0/src/gt4sd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 16:09:51.000000 gt4sd-1.2.0/src/gt4sd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-12 16:09:51.000000 gt4sd-1.2.0/src/gt4sd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 16:09:51.000000 gt4sd-1.2.0/src/gt4sd.egg-info/top_level.txt
```

### Comparing `gt4sd-1.1.9/LICENSE` & `gt4sd-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/PKG-INFO` & `gt4sd-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt4sd
-Version: 1.1.9
+Version: 1.2.0
 Summary: Generative Toolkit for Scientific Discovery (GT4SD).
 Author: GT4SD team
 Keywords: GT4SD Generative Models Inference Training
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gt4sd-1.1.9/README.md` & `gt4sd-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/setup.cfg` & `gt4sd-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,30 @@
 	accelerate
 	datasets
 	diffusers
 	importlib_metadata
 	importlib_resources
 	ipaddress
 	joblib
+	gt4sd-molformer
 	keras
 	keybert
 	minio
 	modlamp
 	molecule_generation
 	molgx
 	nglview
 	numpy
 	pytorch_lightning
+	pyarrow
 	pydantic
 	pymatgen
 	pyTDC!=0.3.8
 	pyyaml
-	rdkit-pypi
+	rdkit
 	regex
 	reinvent-chemistry
 	sacremoses
 	scikit-learn
 	scikit-optimize
 	scipy
 	sentencepiece
@@ -55,15 +57,14 @@
 	typing_extensions
 	wheel
 setup_requires = 
 	setuptools
 package_dir = 
 	= src
 packages = find_namespace:
-include_package_data = False  # would break package_data
 
 [options.entry_points]
 console_scripts = 
 	gt4sd-trainer = gt4sd.cli.trainer:main
 	gt4sd-inference = gt4sd.cli.inference:main
 	gt4sd-saving = gt4sd.cli.saving:main
 	gt4sd-upload = gt4sd.cli.upload:main
@@ -256,11 +257,20 @@
 
 [mypy-nglview.*]
 ignore_missing_imports = True
 
 [mypy-pymatgen.*]
 ignore_missing_imports = True
 
+[mypy-datasets.*]
+ignore_missing_imports = True
+
+[mypy-yaml.*]
+ignore_missing_imports = True
+
+[mypy-gt4sd_molformer.*]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gt4sd-1.1.9/src/gt4sd/__init__.py` & `gt4sd-1.2.0/src/gt4sd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Module initialization."""
 
-__version__ = "1.1.9"
+__version__ = "1.2.0"
 __name__ = "gt4sd"
 
 # NOTE: configure SSL to allow unverified contexts by default
 from .configuration import GT4SDConfiguration
 
 gt4sd_configuration_instance = GT4SDConfiguration.get_instance()
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/key_bert/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/key_bert/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/molgx/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/molgx/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,19 @@
 import numpy as np
 import torch
 from rdkit import Chem
 from terminator.collators import MaskedTextCollator, PropertyCollator
 from terminator.inference import InferenceRT
 from terminator.search import SEARCH_FACTORY, Search
 from terminator.selfies import decoder, encoder
-from terminator.tokenization import InferenceBertTokenizer, PolymerGraphTokenizer
+from terminator.tokenization import (
+    InferenceBertTokenizer,
+    PolymerGraphTokenizer,
+    SelfiesTokenizer,
+)
 from transformers import AutoConfig, AutoModelWithLMHead, XLNetLMHeadModel
 
 from ....domains.materials import MoleculeFormat, Sequence, validate_molecules
 from ....frameworks.torch import device_claim, map_tensor_dict
 from .utils import filter_stubbed, get_substructure_indices
 
 logger = logging.getLogger(__name__)
@@ -275,17 +279,18 @@
             and self.tokenizer.mask_token in number_sequence
         ):
             raise ValueError(
                 f"Do not mask number and text sequence at the same time like in {x}."
             )
         if isinstance(self.tokenizer.text_tokenizer, PolymerGraphTokenizer):
             self.validate_input_molecule(text_sequence, MoleculeFormat.copolymer)
+        elif isinstance(self.tokenizer.text_tokenizer, SelfiesTokenizer):
+            self.validate_input_molecule(text_sequence, MoleculeFormat.selfies)
         else:
-            # We can assume this to be a SELFIES
-            self.validate_input_molecule(text_sequence)
+            self.validate_input_molecule(text_sequence, MoleculeFormat.smiles)
 
         self.validate_input_numerical(number_sequence)
 
     def validate_input_molecule(
         self, sequence: str, input_type: str = "SELFIES"
     ) -> None:
         """
@@ -461,15 +466,20 @@
         # Combine predictions with the static part to obtain the full sequences
         generations = input_ids.cpu()
         generations[generations == self.tokenizer.mask_token_id] = predictions[
             generations == self.tokenizer.mask_token_id
         ]
 
         # Second part: Predict the properties of the just generated sequence
-        _input = self.property_collator.mask_tokens(generations)
+        try:
+            _input = self.property_collator.mask_tokens(generations)
+        except UnboundLocalError:
+            # NOTE: in case there are errors with the collator we can't have successes
+            return ()
+
         prediction_input = {
             "input_ids": _input[0],
             "perm_mask": _input[1],
             "target_mapping": _input[2],
             "attention_mask": self.property_collator.attention_mask(generations),
         }
 
@@ -812,14 +822,17 @@
                 logger.error(
                     f"\nSubstructure to keep in {keep} not found in seed sequence, ignoring it."
                 )
             else:
                 to_keep.append(keep)
 
         self.substructures_to_keep = to_keep
+        # Contains even the ones whose strings cant be found in seed string
+        self.all_substructures_to_keep = substructures_to_keep
+
         if len(set(self.substructures_to_keep + self.substructures_to_mask)) < len(
             self.substructures_to_keep
         ) + len(self.substructures_to_mask):
             raise ValueError(
                 "Substructures to mask and keep contain duplicates or overlap."
             )
 
@@ -901,15 +914,15 @@
         elif self.task == "generation":
             self.generate_batch = self.generate_batch_generation  # type: ignore
             self.batch_size = batch_size
             self.property_collator = PropertyCollator(
                 tokenizer=self.tokenizer,
                 property_tokens=self.properties,
                 num_tokens_to_mask=[-1] * len(self.properties),
-                ignore_errors=False,
+                ignore_errors=True,
             )
 
         else:
             raise ValueError(f"Unknown task: {self.task}")
 
         self.small_mol = True
 
@@ -987,20 +1000,23 @@
             List of atoms in SELFIES notation.
         """
         # To reflect double bonds
         tokens_to_mask.extend([f"={t}" for t in tokens_to_mask])
         return [encoder(a) for a in tokens_to_mask]  # type: ignore
 
     def language_encoding(self, seq: str) -> str:
-        if isinstance(self.tokenizer.text_tokenizer, PolymerGraphTokenizer):
+        if isinstance(self.tokenizer.text_tokenizer, SelfiesTokenizer):
+            selfie = encoder(seq)
+            if not isinstance(selfie, str):
+                raise TypeError(
+                    f"{seq} (type={type(seq)}) is not a SMILES sequence that can be converted to SELFIES."
+                )
+            return selfie
+        else:
             return seq
-        selfie = encoder(seq)
-        if not isinstance(selfie, str):
-            raise TypeError(f"{seq} (type={type(seq)}) is not a valid SMILES sequence.")
-        return selfie
 
     def filter_substructures(
         self, property_successes: Tuple[Tuple[str, str]]
     ) -> Tuple[Tuple[str, str]]:
         """
         Remove samples where user-required substructures are absent from generated samples.
 
@@ -1020,33 +1036,53 @@
 
         # Remove samples with stub-like sequences (spuriously small)
         property_successes = filter_stubbed(
             property_successes, target=self.target, threshold=0.5
         )
 
         successes: List[Tuple[str, str]] = []
-
-        subs_mols = []
-        for keep in self.substructures_to_keep:
-            subs_mols.append(Chem.MolFromSmiles(keep) or Chem.MolFromSmarts(keep))
-            if subs_mols[-1] is None:
+        subs_mols: List = []
+        for keep in self.all_substructures_to_keep:
+            subs_mol = Chem.MolFromSmiles(keep) or Chem.MolFromSmarts(keep)
+            if subs_mol is None:
                 logger.warning(
                     f"{keep} is not a valid SMILES/SELFIES. Instead substructure filtering "
                     f"based on sequence alone can be done and is set to: {self.text_filtering}"
                 )
+            if keep not in self.substructures_to_keep and not Chem.MolFromSmiles(
+                self.target
+            ).HasSubstructMatch(subs_mol):
+                logger.info(
+                    f"{keep} could not be identified in SMILES/SELFIES on text level AND no "
+                    "substructure match occurred, hence it will be ignored"
+                )
+                subs_mols.append(None)
+            elif keep not in self.substructures_to_keep:
+                logger.info(
+                    f"{keep} could not be identified in SMILES/SELFIES on *string*-level but since the"
+                    "RDKit match was successful, it will still be used for post-hoc filtering."
+                )
+                subs_mols.append(subs_mol)
+            else:
+                # "Normal" substructure
+                subs_mols.append(subs_mol)
 
         # Perform filtering
         for smi, prop in property_successes:
             if smi is None:
                 continue
             sane = True
             mol = Chem.MolFromSmiles(smi)
-            for subs_mol, subs_string in zip(subs_mols, self.substructures_to_keep):
+            for subs_mol, subs_string in zip(subs_mols, self.all_substructures_to_keep):
                 if subs_mol is None:
-                    if self.text_filtering and subs_string not in smi:
+                    if (
+                        self.text_filtering
+                        and subs_string not in smi
+                        and subs_string in self.substructures_to_keep
+                    ):
                         sane = False
                         break
                 else:
                     if not mol.HasSubstructMatch(subs_mol):
                         # Desired substructure not found
                         sane = False
                         break
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,24 @@
 
     seed_atoms = len(list(seed.GetAtoms()))
     seed_bonds = seed.GetNumBonds()
 
     smis: List[str] = []
     props: List[str] = []
     for smi, prop in property_sequences:
+        if smi == "":
+            continue
         try:
             mol = Chem.MolFromSmiles(smi)
+            num_atoms = len(list(mol.GetAtoms()))
+            num_bonds = mol.GetNumBonds()
+
+            if num_atoms > (threshold * seed_atoms) and num_bonds > (
+                threshold * seed_bonds
+            ):
+                smis.append(smi)
+                props.append(prop)
         except Exception:
             continue
 
-        num_atoms = len(list(mol.GetAtoms()))
-        num_bonds = mol.GetNumBonds()
-
-        if num_atoms > (threshold * seed_atoms) and num_bonds > (
-            threshold * seed_bonds
-        ):
-            smis.append(smi)
-            props.append(prop)
-
     successes = cast(Tuple[Tuple[str, str]], tuple(zip(smis, props)))
     return successes
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/template/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/template/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/template/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/template/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/template/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/diffusion/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/diffusion/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/hugging_face/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/hugging_face/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/hugging_face/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/hugging_face/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/hugging_face/implementation.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 (except for Alexei and Maria) are discovered.
 The voice of Nicholas's young son, Tsarevich Alexei Nikolaevich, narrates the
 remainder of the story. 1883 Western Siberia,
 a young Grigori Rasputin is asked by his father and a group of men to perform magic.
 Rasputin has a vision and denounces one of the men as a horse thief. Although his
 father initially slaps him for making such an accusation, Rasputin watches as the
 man is chased outside and beaten. Twenty years later, Rasputin sees a vision of
-the Virgin Mary, prompting him to become a priest. Rasputin quickly becomes famous,
-with people, even a bishop, begging for his blessing. <eod> </s> <eos>"""
+the Virgin Mary, prompting him to become a priest. <eod> </s> <eos>"""
 
 
 def set_seed(seed: int = 42) -> None:
     """Set seed for all random number generators.
 
     Args:
         seed: seed to set. Defaults to 42.
@@ -288,21 +287,18 @@
         generated_sequences: List[str] = []
 
         for generated_sequence in output_sequences:
             generated_sequence = generated_sequence.tolist()
             text = self.tokenizer.decode(
                 generated_sequence, clean_up_tokenization_spaces=True
             )
+
             text = text[: text.find(self.stop_token) if self.stop_token else None]
-            total_sequence = (
-                self.prompt
-                + text[
-                    len(
-                        self.tokenizer.decode(
-                            encoded_prompt[0], clean_up_tokenization_spaces=True
-                        )
-                    ) :
-                ]
-            )
+
+            if self.prompt not in text:
+                total_sequence = self.prefix + self.prompt + text
+            else:
+                total_sequence = text
+
             generated_sequences.append(total_sequence)
 
         return generated_sequences
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/moler/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/moler/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/moler/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/moler/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,14 +130,26 @@
         default=0,
         metadata=dict(description="Seed used for random number generation."),
     )
     num_workers: int = field(
         default=6,
         metadata=dict(description="Number of workers used for generation."),
     )
+    seed_smiles: str = field(
+        default="",
+        metadata=dict(
+            description="Dot-separated SMILES used to initialize the encoder. If empty, random codes are used."
+        ),
+    )
+    sigma: float = field(
+        default=0.0,
+        metadata=dict(
+            description="Variance of Gaussian noise being added to latent code."
+        ),
+    )
 
     def get_target_description(self) -> Optional[Dict[str, str]]:
         """Get description of the target for generation.
 
         Returns:
             target description, returns None in case no target is used.
         """
@@ -155,14 +167,16 @@
         return MoLeRGenerator(
             resources_path=resources_path,
             scaffolds=self.scaffolds,
             num_samples=self.num_samples,
             beam_size=self.beam_size,
             seed=self.seed,
             num_workers=self.num_workers,
+            seed_smiles=self.seed_smiles,
+            sigma=self.sigma,
         )
 
     def validate_item(self, item: str) -> SMILES:
         """Check that item is a valid SMILES.
 
         Args:
             item: a generated item that is possibly not valid.
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/moler/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/moler/implementation.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #
 """Implementation of MoLeR conditional generators."""
 
 import logging
 from itertools import cycle, islice
 from typing import List
 
+import numpy as np
 from rdkit import Chem
 from molecule_generation import VaeWrapper
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
@@ -41,58 +42,81 @@
         self,
         resources_path: str,
         scaffolds: str,
         num_samples: int,
         beam_size: int,
         seed: int,
         num_workers: int,
+        seed_smiles: str,
+        sigma: float,
     ) -> None:
         """Instantiate a MoLeR generator.
 
         Args:
             resources_path: path to the resources for model loading.
             scaffolds: scaffolds as '.'-separated SMILES. If empty, no scaffolds are used.
             num_samples: Number of molecules to sample per call.
             beam_size: beam size to use during decoding.
             seed: seed used for random number generation.
             num_workers: number of workers used for generation.
+            seed_smiles: dot-separated SMILES used to initialize the decoder. If empty,
+                random codes are sampled from the latent space.
+            sigma: variance of gaussian noise being added to the latent code.
 
         Raises:
             RuntimeError: in the case extras are disabled.
         """
         # loading artifacts
         self.resources_path = resources_path
-        self.scaffolds = scaffolds
         self.num_samples = num_samples
         self.beam_size = beam_size
         self.num_workers = num_workers
         self._seed = seed
+        self.sigma = sigma
+
+        # Process context
+        self.seed_smiles = [
+            smi for smi in seed_smiles.split(".") if Chem.MolFromSmiles(smi) is not None
+        ]
+        self.scaffolds = [
+            scaffold
+            for scaffold in scaffolds.split(".")
+            if Chem.MolFromSmiles(scaffold) is not None
+        ]
+        # Repeat scaffolds if needed
+        if self.scaffolds != [""] and len(self.scaffolds) < self.num_samples:
+            self.scaffolds = list(islice(cycle(self.scaffolds), self.num_samples))
+        # Repeat seed smiles if needed
+        if self.seed_smiles != [""] and len(self.seed_smiles) < self.num_samples:
+            self.seed_smiles = list(islice(cycle(self.seed_smiles), self.num_samples))
 
     def generate(self) -> List[str]:
         """Sample molecules using MoLeR.
 
         Returns:
             sampled molecule (SMILES).
         """
-        # process scaffolds
-        valid_scaffolds = [
-            scaffold
-            for scaffold in self.scaffolds.split(".")
-            if Chem.MolFromSmiles(scaffold) is not None
-        ]
         # generate molecules
         logger.info("running MoLeR...")
         with VaeWrapper(
             self.resources_path,
             beam_size=self.beam_size,
             seed=self._seed,
             num_workers=self.num_workers,
         ) as model:
-            latents = model.sample_latents(self.num_samples)
-            scaffolds = list(islice(cycle(valid_scaffolds), self.num_samples))
+            if self.seed_smiles == [""]:
+                latents = model.sample_latents(self.num_samples)
+            else:
+                latents = np.stack(model.encode(self.seed_smiles))
+
+            # Add noise to latent codes
+            latents = latents + self.sigma * np.random.randn(*latents.shape).astype(
+                np.float32
+            )
+            scaffolds = list(islice(cycle(self.scaffolds), self.num_samples))
             samples = model.decode(
                 latents=latents,
                 scaffolds=scaffolds if len(scaffolds) == self.num_samples else None,
             )
         # offset seed to guarantee uniqueness
         self._seed += 1
         logger.info("MoLeR run completed")
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/paccmann_vae/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/paccmann_vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/pgt/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/pgt/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/pgt/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/pgt/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/pgt/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/pgt/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/polymer_blocks/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/polymer_blocks/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/mol_dct.pkl` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/mol_dct.pkl`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_diffusion.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_hugging_face.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_hugging_face.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_moler.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,38 +17,41 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""MoLeR tests."""
+"""PolymerBlocks tests."""
 
 from typing import ClassVar, Type
 
 import pytest
 
 from gt4sd.algorithms.core import AlgorithmConfiguration
-from gt4sd.algorithms.generation.moler import MoLeR, MoLeRDefaultGenerator
+from gt4sd.algorithms.generation.polymer_blocks import (
+    PolymerBlocks,
+    PolymerBlocksGenerator,
+)
 from gt4sd.algorithms.registry import ApplicationsRegistry
 
 
 def get_classvar_type(class_var):
     """Extract type from ClassVar type annotation: `ClassVar[T]] -> T`."""
     return class_var.__args__[0]
 
 
 @pytest.mark.parametrize(
     "config_class, algorithm_type, domain, algorithm_name",
     [
         (
-            MoLeRDefaultGenerator,
+            PolymerBlocksGenerator,
             "generation",
             "materials",
-            MoLeR.__name__,
+            PolymerBlocks.__name__,
         )
     ],
 )
 def test_config_class(
     config_class: Type[AlgorithmConfiguration],
     algorithm_type: str,
     domain: str,
@@ -62,61 +65,62 @@
         if keyword in ("algorithm_type", "domain", "algorithm_name"):
             assert type_annotation.__origin__ is ClassVar  # type: ignore
             assert str == get_classvar_type(type_annotation)
 
 
 @pytest.mark.parametrize(
     "config_class",
-    [(MoLeRDefaultGenerator)],
+    [(PolymerBlocksGenerator)],
 )
 def test_config_instance(config_class: Type[AlgorithmConfiguration]):
     config = config_class()  # type:ignore
     assert config.algorithm_application == config_class.__name__
 
 
 @pytest.mark.parametrize(
     "config_class",
-    [(MoLeRDefaultGenerator)],
+    [(PolymerBlocksGenerator)],
 )
 def test_available_versions(config_class: Type[AlgorithmConfiguration]):
     versions = config_class.list_versions()
     assert "v0" in versions
 
 
 @pytest.mark.parametrize(
     "config, algorithm",
     [
         (
-            MoLeRDefaultGenerator,
-            MoLeR,
+            PolymerBlocksGenerator,
+            PolymerBlocks,
         )
     ],
 )
 def test_generation_via_import(config, algorithm):
     algorithm = algorithm(configuration=config())
     items = list(algorithm.sample(5))
     assert len(items) == 5
 
 
 @pytest.mark.parametrize(
     "algorithm_application, algorithm_type, domain, algorithm_name",
     [
         (
-            MoLeRDefaultGenerator.__name__,
+            PolymerBlocksGenerator.__name__,
             "generation",
             "materials",
-            MoLeR.__name__,
+            PolymerBlocks.__name__,
         ),
     ],
 )
 def test_generation_via_registry(
     algorithm_type, domain, algorithm_name, algorithm_application
 ):
     algorithm = ApplicationsRegistry.get_application_instance(
         target=None,
         algorithm_type=algorithm_type,
         domain=domain,
         algorithm_name=algorithm_name,
         algorithm_application=algorithm_application,
+        generated_length=5,
     )
     items = list(algorithm.sample(5))
     assert len(items) == 5
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 
 @pytest.mark.parametrize(
     "config_class",
     [(PaccMannVAEGenerator)],
 )
 def test_available_versions(config_class: Type[AlgorithmConfiguration]):
     versions = config_class.list_versions()
-    print("HERE", versions)
     assert "v0" in versions
 
 
 @pytest.mark.parametrize(
     "config, algorithm",
     [
         (
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_pgt.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_pgt.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,41 +17,38 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""PolymerBlocks tests."""
+"""TopicsZeroShot tests."""
 
 from typing import ClassVar, Type
 
 import pytest
 
 from gt4sd.algorithms.core import AlgorithmConfiguration
-from gt4sd.algorithms.generation.polymer_blocks import (
-    PolymerBlocks,
-    PolymerBlocksGenerator,
-)
+from gt4sd.algorithms.prediction.topics_zero_shot import TopicsPredictor, TopicsZeroShot
 from gt4sd.algorithms.registry import ApplicationsRegistry
 
 
 def get_classvar_type(class_var):
     """Extract type from ClassVar type annotation: `ClassVar[T]] -> T`."""
     return class_var.__args__[0]
 
 
 @pytest.mark.parametrize(
     "config_class, algorithm_type, domain, algorithm_name",
     [
         (
-            PolymerBlocksGenerator,
-            "generation",
-            "materials",
-            PolymerBlocks.__name__,
+            TopicsPredictor,
+            "prediction",
+            "nlp",
+            TopicsZeroShot.__name__,
         )
     ],
 )
 def test_config_class(
     config_class: Type[AlgorithmConfiguration],
     algorithm_type: str,
     domain: str,
@@ -65,62 +62,63 @@
         if keyword in ("algorithm_type", "domain", "algorithm_name"):
             assert type_annotation.__origin__ is ClassVar  # type: ignore
             assert str == get_classvar_type(type_annotation)
 
 
 @pytest.mark.parametrize(
     "config_class",
-    [(PolymerBlocksGenerator)],
+    [(TopicsPredictor)],
 )
 def test_config_instance(config_class: Type[AlgorithmConfiguration]):
     config = config_class()  # type:ignore
     assert config.algorithm_application == config_class.__name__
 
 
 @pytest.mark.parametrize(
     "config_class",
-    [(PolymerBlocksGenerator)],
+    [(TopicsPredictor)],
 )
 def test_available_versions(config_class: Type[AlgorithmConfiguration]):
     versions = config_class.list_versions()
-    assert "v0" in versions
+    assert "dbpedia" in versions
 
 
 @pytest.mark.parametrize(
-    "config, algorithm",
+    "config, target, algorithm",
     [
         (
-            PolymerBlocksGenerator,
-            PolymerBlocks,
+            TopicsPredictor,
+            "The dominant sequence transduction models are based on complex recurrent or convolutional neural networks in an encoder-decoder configuration.",
+            TopicsZeroShot,
         )
     ],
 )
-def test_generation_via_import(config, algorithm):
-    algorithm = algorithm(configuration=config())
+def test_generation_via_import(config, target, algorithm):
+    algorithm = algorithm(configuration=config(), target=target)
     items = list(algorithm.sample(5))
     assert len(items) == 5
 
 
 @pytest.mark.parametrize(
-    "algorithm_application, algorithm_type, domain, algorithm_name",
+    "algorithm_application, target, algorithm_type, domain, algorithm_name",
     [
         (
-            PolymerBlocksGenerator.__name__,
-            "generation",
-            "materials",
-            PolymerBlocks.__name__,
+            TopicsPredictor.__name__,
+            "The dominant sequence transduction models are based on complex recurrent or convolutional neural networks in an encoder-decoder configuration.",
+            "prediction",
+            "nlp",
+            TopicsZeroShot.__name__,
         ),
     ],
 )
 def test_generation_via_registry(
-    algorithm_type, domain, algorithm_name, algorithm_application
+    algorithm_type, target, domain, algorithm_name, algorithm_application
 ):
     algorithm = ApplicationsRegistry.get_application_instance(
-        target=None,
+        target=target,
         algorithm_type=algorithm_type,
         domain=domain,
         algorithm_name=algorithm_name,
         algorithm_application=algorithm_application,
-        generated_length=5,
     )
     items = list(algorithm.sample(5))
     assert len(items) == 5
```

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/tests/test_torchdrug.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/tests/test_torchdrug.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/torchdrug/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/torchdrug/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/torchdrug/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/torchdrug/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/generation/torchdrug/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/generation/torchdrug/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/paccmann/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/paccmann/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/paccmann/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/paccmann/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/paccmann/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/paccmann/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/tests/test_paccmann.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/tests/test_paccmann.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/registry.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/tests/test_config.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/algorithms/tests/test_registry.py` & `gt4sd-1.2.0/src/gt4sd/algorithms/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/__init__.py` & `gt4sd-1.2.0/src/gt4sd/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/algorithms.py` & `gt4sd-1.2.0/src/gt4sd/cli/algorithms.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/argument_parser.py` & `gt4sd-1.2.0/src/gt4sd/cli/argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             elif (
                 hasattr(field.type, "__origin__")
                 and re.search(r"^typing\.List\[(.*)\]$", str(field.type)) is not None
             ):
                 kwargs["nargs"] = "+"
                 kwargs["type"] = partial(none_checker, dtype=field.type.__args__[0])
                 assert all(
-                    x == kwargs["type"] for x in field.type.__args__
+                    x == kwargs["type"].keywords["dtype"] for x in field.type.__args__
                 ), f"{field.name} cannot be a List of mixed types: {field.type.__args__}"
                 if field.default_factory is not dataclasses.MISSING:  # type: ignore
                     kwargs["default"] = field.default_factory()  # type: ignore
                 elif field.default is dataclasses.MISSING:
                     kwargs["required"] = True
             else:
                 kwargs["type"] = partial(none_checker, dtype=field.type)
```

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/hf_to_st_converter.py` & `gt4sd-1.2.0/src/gt4sd/cli/hf_to_st_converter.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/inference.py` & `gt4sd-1.2.0/src/gt4sd/cli/inference.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/load_arguments_from_dataclass.py` & `gt4sd-1.2.0/src/gt4sd/cli/load_arguments_from_dataclass.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/pl_to_hf_converter.py` & `gt4sd-1.2.0/src/gt4sd/cli/pl_to_hf_converter.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/saving.py` & `gt4sd-1.2.0/src/gt4sd/cli/saving.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/trainer.py` & `gt4sd-1.2.0/src/gt4sd/cli/trainer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/cli/upload.py` & `gt4sd-1.2.0/src/gt4sd/cli/upload.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/configuration.py` & `gt4sd-1.2.0/src/gt4sd/configuration.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/conftest.py` & `gt4sd-1.2.0/src/gt4sd/conftest.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/domains/__init__.py` & `gt4sd-1.2.0/src/gt4sd/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/domains/core.py` & `gt4sd-1.2.0/src/gt4sd/domains/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/domains/materials/__init__.py` & `gt4sd-1.2.0/src/gt4sd/domains/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/domains/materials/protein_encoding.py` & `gt4sd-1.2.0/src/gt4sd/domains/materials/protein_encoding.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/domains/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/domains/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/exceptions.py` & `gt4sd-1.2.0/src/gt4sd/exceptions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/extras/__init__.py` & `gt4sd-1.2.0/src/gt4sd/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/cgcnn/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/cgcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/cgcnn/data.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/cgcnn/data.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/cgcnn/model.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/cgcnn/model.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv` & `gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/feature_engine.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/feature_engine.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/optimization.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/optimization.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/processing.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/processing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/enzeptional/tests/test_processing.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/enzeptional/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/arg_parser/parser.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/arg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/arg_parser/utils.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/arg_parser/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/data_module.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/data_module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/dataset.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/dataloader/sampler.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/dataloader/sampler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/envs/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/loss/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/loss/td_loss.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/loss/td_loss.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/models/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/ml/module.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/ml/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/tests/qm9.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/tests/qm9.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/tests/test_gfn.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/tests/test_gfn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/train/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/train/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/train/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/train/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/gflownet/util.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/gflownet/util.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/arg_parser/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/arg_parser/parser.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/arg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/arg_parser/utils.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/arg_parser/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/data_module.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/data_module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/dataset.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/dataloader/sampler.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/dataloader/sampler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/activation.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/activation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/base_model.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/base_model.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/loss.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/loss.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/model_builder.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/module.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/utils.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/ml/module.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/ml/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/tests/test_tokenizer.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/tokenizer/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/train/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/train/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/granular/train/core.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/granular/train/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/torch/__init__.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/frameworks/torch/vae.py` & `gt4sd-1.2.0/src/gt4sd/frameworks/torch/vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/__init__.py` & `gt4sd-1.2.0/src/gt4sd/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/core.py` & `gt4sd-1.2.0/src/gt4sd/properties/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/crystals/__init__.py` & `gt4sd-1.2.0/src/gt4sd/properties/crystals/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/crystals/core.py` & `gt4sd-1.2.0/src/gt4sd/properties/crystals/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/molecules/__init__.py` & `gt4sd-1.2.0/src/gt4sd/properties/molecules/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,20 @@
     Esol,
     IsScaffold,
     Lipinski,
     Logp,
     MolecularWeight,
     MoleculeOne,
     MoleculeOneParameters,
+    MolformerClassification,
+    MolformerClassificationParameters,
+    MolformerMultitaskClassification,
+    MolformerMultitaskClassificationParameters,
+    MolformerRegression,
+    MolformerRegressionParameters,
     NumberAromaticRings,
     NumberAtoms,
     NumberHAcceptors,
     NumberHDonors,
     NumberHeterocycles,
     NumberLargeRings,
     NumberRings,
@@ -103,14 +109,23 @@
     # properties predicted by models
     "scscore": (Scscore, ScscoreConfiguration),
     "activity_against_target": (ActivityAgainstTarget, ActivityAgainstTargetParameters),
     "tox21": (Tox21, Tox21Parameters),
     "sider": (Sider, SiderParameters),
     "organtox": (OrganTox, OrganToxParameters),
     "clintox": (ClinTox, ClinToxParameters),
+    "molformer_classification": (
+        MolformerClassification,
+        MolformerClassificationParameters,
+    ),
+    "molformer_multitask_classification": (
+        MolformerMultitaskClassification,
+        MolformerMultitaskClassificationParameters,
+    ),
+    "molformer_regression": (MolformerRegression, MolformerRegressionParameters),
     # # properties from models requiring authentification
     "askcos": (Askcos, AskcosParameters),
     "molecule_one": (MoleculeOne, MoleculeOneParameters),
     # # properties from models require additional installations
     "docking_tdc": (DockingTdc, DockingTdcParameters),
     "docking": (Docking, DockingParameters),
 }
```

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/molecules/core.py` & `gt4sd-1.2.0/src/gt4sd/properties/molecules/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,17 +17,47 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
+import os
 from enum import Enum
-from typing import List
+from typing import List, Optional, Union
 
+import importlib_resources
+import numpy as np
+import pandas as pd
+import torch
+import yaml
+from gt4sd_molformer.finetune.finetune_pubchem_light import (
+    LightningModule as RegressionLightningModule,
+)
+from gt4sd_molformer.finetune.finetune_pubchem_light import (
+    PropertyPredictionDataModule as RegressionDataModule,
+)
+from gt4sd_molformer.finetune.finetune_pubchem_light import (
+    PropertyPredictionDataset as RegressionDataset,
+)
+from gt4sd_molformer.finetune.finetune_pubchem_light_classification import (
+    LightningModule as ClassificationLightningModule,
+)
+from gt4sd_molformer.finetune.finetune_pubchem_light_classification import (
+    PropertyPredictionDataModule as ClassificationDataModule,
+)
+from gt4sd_molformer.finetune.finetune_pubchem_light_classification import (
+    PropertyPredictionDataset as ClassificationDataset,
+)
+from gt4sd_molformer.finetune.finetune_pubchem_light_classification_multitask import (
+    MultitaskEmbeddingDataset,
+    MultitaskModel,
+    PropertyPredictionDataModule,
+)
+from gt4sd_molformer.finetune.ft_tokenizer.ft_tokenizer import MolTranBertTokenizer
 from paccmann_generator.drug_evaluators import SIDER
 from paccmann_generator.drug_evaluators import ClinTox as _ClinTox
 from paccmann_generator.drug_evaluators import OrganDB as _OrganTox
 from paccmann_generator.drug_evaluators import SCScore
 from paccmann_generator.drug_evaluators import Tox21 as _Tox21
 from pydantic import Field
 from tdc import Oracle
@@ -35,14 +65,15 @@
 
 from ...algorithms.core import (
     ConfigurablePropertyAlgorithmConfiguration,
     Predictor,
     PredictorAlgorithm,
 )
 from ...domains.materials import SmallMolecule
+from ...frameworks.torch import device_claim
 from ..core import (
     ApiTokenParameters,
     CallablePropertyPredictor,
     ConfigurableCallablePropertyPredictor,
     DomainSubmodule,
     IpAdressParameters,
     PropertyPredictorParameters,
@@ -161,14 +192,35 @@
     box_size: List[float] = Field(example=[20, 20, 20], description="Docking box size")
 
 
 class S3ParametersMolecules(S3Parameters):
     domain: DomainSubmodule = DomainSubmodule("molecules")
 
 
+class MolformerParameters(S3ParametersMolecules):
+    algorithm_name: str = "molformer"
+    batch_size: int = Field(description="Prediction batch size", default=128)
+    workers: int = Field(description="Number of data loading workers", default=8)
+    device: Optional[str] = Field(
+        description="Device to be used for inference", default=None
+    )
+
+
+class MolformerClassificationParameters(MolformerParameters):
+    algorithm_application: str = "classification"
+
+
+class MolformerMultitaskClassificationParameters(MolformerParameters):
+    algorithm_application: str = "multitask_classification"
+
+
+class MolformerRegressionParameters(MolformerParameters):
+    algorithm_application: str = "regression"
+
+
 class MCAParameters(S3ParametersMolecules):
     algorithm_name: str = "MCA"
 
 
 class Tox21Parameters(MCAParameters):
     algorithm_application: str = "Tox21"
 
@@ -220,14 +272,221 @@
         default=ToxType.all,
         example=ToxType.chronic,
         description="type of toxicity for which predictions are made.",
         options=["chronic", "subchronic", "multigenerational", "all"],
     )
 
 
+class _Molformer(PredictorAlgorithm):
+    """Base class for all Molformer predictive algorithms."""
+
+    def __init__(self, parameters: MolformerParameters):
+
+        # Set up the configuration from the parameters
+        configuration = ConfigurablePropertyAlgorithmConfiguration(
+            algorithm_type=parameters.algorithm_type,
+            domain=parameters.domain,
+            algorithm_name=parameters.algorithm_name,
+            algorithm_application=parameters.algorithm_application,
+            algorithm_version=parameters.algorithm_version,
+        )
+
+        self.batch_size = parameters.batch_size
+        self.workers = parameters.workers
+
+        self.tokenizer_path = (
+            importlib_resources.files("gt4sd_molformer") / "finetune/bert_vocab.txt"
+        )
+
+        self.device = device_claim(parameters.device)
+
+        # The parent constructor calls `self.get_model`.
+        super().__init__(configuration=configuration)
+
+    def get_resources_path_and_config(self, resources_path: str):
+
+        model_path = os.path.join(resources_path, "model.ckpt")
+        config_path = os.path.join(resources_path, "hparams.yaml")
+
+        with open(config_path, "r") as stream:
+            config = yaml.safe_load(stream)
+
+        return config, model_path
+
+
+class MolformerClassification(_Molformer):
+    """Class for all Molformer classification algorithms."""
+
+    def get_model(self, resources_path: str) -> Predictor:
+        """Instantiate the actual model.
+
+        Args:
+            resources_path: local path to model files.
+
+        Returns:
+            Predictor: the model.
+        """
+
+        config, model_path = self.get_resources_path_and_config(resources_path)
+
+        config["num_workers"] = 0
+
+        tokenizer = MolTranBertTokenizer(self.tokenizer_path)
+
+        model = ClassificationLightningModule(config, tokenizer).load_from_checkpoint(
+            model_path,
+            strict=False,
+            config=config,
+            tokenizer=tokenizer,
+            vocab=len(tokenizer.vocab),
+        )
+
+        model.to(self.device)
+        model.eval()
+
+        # Wrapper to get the predictions
+        def informative_model(samples: Union[str, List[str]]) -> List[float]:
+
+            if isinstance(samples, str):
+                samples = [samples]
+
+            df = pd.DataFrame.from_dict({"smiles": samples})
+
+            dataset = ClassificationDataset(df)
+            datamodule = ClassificationDataModule(config, tokenizer)
+            datamodule.test_ds = dataset
+
+            preds = []
+            for batch in datamodule.test_dataloader():
+                with torch.no_grad():
+                    batch = [x.to(self.device) for x in batch]
+                    batch_output = model.testing_step(batch, 0, 0)
+
+                preds_cpu = batch_output["pred"][:, 1]
+                y_pred = np.where(preds_cpu >= 0.5, 1, 0)
+                preds += y_pred.tolist()
+
+            return preds
+
+        return informative_model
+
+
+class MolformerMultitaskClassification(_Molformer):
+    """Class for all Molformer multitask classification algorithms."""
+
+    def get_model(self, resources_path: str) -> Predictor:
+        """Instantiate the actual model.
+
+        Args:
+            resources_path: local path to model files.
+
+        Returns:
+            Predictor: the model.
+        """
+
+        config, model_path = self.get_resources_path_and_config(resources_path)
+
+        config["num_workers"] = 0
+
+        tokenizer = MolTranBertTokenizer(self.tokenizer_path)
+
+        model = MultitaskModel(config, tokenizer).load_from_checkpoint(
+            model_path,
+            strict=False,
+            config=config,
+            tokenizer=tokenizer,
+            vocab=len(tokenizer.vocab),
+        )
+
+        model.to(self.device)
+        model.eval()
+
+        # Wrapper to get the predictions
+        def informative_model(samples: Union[str, List[str]]) -> List[str]:
+
+            if isinstance(samples, str):
+                samples = [samples]
+
+            df = pd.DataFrame.from_dict({"smiles": samples})
+
+            dataset = MultitaskEmbeddingDataset(df)
+            datamodule = PropertyPredictionDataModule(config, tokenizer)
+            datamodule.test_ds = dataset
+
+            preds = []
+            for batch in datamodule.test_dataloader():
+
+                with torch.no_grad():
+                    batch = [x.to(self.device) for x in batch]
+                    batch_output = model.testing_step(batch, 0, 0)
+
+                batch_preds_idx = torch.argmax(batch_output["pred"], dim=1)
+                batch_preds = [config["measure_names"][i] for i in batch_preds_idx]
+                preds += batch_preds
+
+            return preds
+
+        return informative_model
+
+
+class MolformerRegression(_Molformer):
+    """Class for all Molformer regression algorithms."""
+
+    def get_model(self, resources_path: str) -> Predictor:
+        """Instantiate the actual model.
+
+        Args:
+            resources_path: local path to model files.
+
+        Returns:
+            Predictor: the model.
+        """
+
+        config, model_path = self.get_resources_path_and_config(resources_path)
+
+        config["num_workers"] = 0
+
+        tokenizer = MolTranBertTokenizer(self.tokenizer_path)
+
+        model = RegressionLightningModule(config, tokenizer).load_from_checkpoint(
+            model_path,
+            strict=False,
+            config=config,
+            tokenizer=tokenizer,
+            vocab=len(tokenizer.vocab),
+        )
+
+        model.to(self.device)
+        model.eval()
+
+        # Wrapper to get the predictions
+        def informative_model(samples: Union[str, List[str]]) -> List[float]:
+
+            if isinstance(samples, str):
+                samples = [samples]
+
+            df = pd.DataFrame.from_dict({"smiles": samples})
+
+            dataset = RegressionDataset(df, False, config["aug"])
+            datamodule = RegressionDataModule(config, tokenizer)
+            datamodule.test_ds = dataset
+
+            preds = []
+            for batch in datamodule.test_dataloader():
+                with torch.no_grad():
+                    batch = [x.to(self.device) for x in batch]
+                    batch_output = model.testing_step(batch, 0, 0)
+
+                preds += batch_output["pred"].view(-1).tolist()
+
+            return preds
+
+        return informative_model
+
+
 # NOTE: property prediction classes
 class Plogp(CallablePropertyPredictor):
     """Calculate the penalized logP of a molecule. This is the logP minus the number of
     rings with > 6 atoms minus the SAS.
     """
 
     def __init__(
```

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/molecules/functions.py` & `gt4sd-1.2.0/src/gt4sd/properties/molecules/functions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/proteins/__init__.py` & `gt4sd-1.2.0/src/gt4sd/properties/proteins/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/proteins/core.py` & `gt4sd-1.2.0/src/gt4sd/properties/proteins/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/proteins/functions.py` & `gt4sd-1.2.0/src/gt4sd/properties/proteins/functions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/scorer.py` & `gt4sd-1.2.0/src/gt4sd/properties/scorer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/scores/__init__.py` & `gt4sd-1.2.0/src/gt4sd/properties/scores/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/scores/core.py` & `gt4sd-1.2.0/src/gt4sd/properties/scores/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/properties/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/tests/test_properties.py` & `gt4sd-1.2.0/src/gt4sd/properties/tests/test_properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,14 +127,60 @@
     ) as file_path:
         out = model(input=file_path)  # type: ignore
         pred_dict = dict(zip(out["cif_ids"], out["predictions"]))  # type: ignore
         prediction = pred_dict["1000041"]
         assert np.isclose(prediction, crystal_ground_truths[property_key], atol=1e-2)
 
 
+def test_molformer_regression():
+
+    property_class, parameters_class = MOLECULE_PROPERTY_PREDICTOR_FACTORY[
+        "molformer_regression"
+    ]
+    model = property_class(
+        parameters_class(algorithm_version="molformer_alpha_public_test")  # type: ignore
+    )
+
+    output = model(input=["OC12COC3=NCC1C23"])  # type: ignore
+
+    assert isinstance(output, list)
+    assert len(output) == 1
+    assert np.isclose(output[0], 69.26847839355469, atol=1e-4)
+
+
+def test_molformer_classification():
+
+    property_class, parameters_class = MOLECULE_PROPERTY_PREDICTOR_FACTORY[
+        "molformer_classification"
+    ]
+    model = property_class(
+        parameters_class(algorithm_version="molformer_bace_public_test")  # type: ignore
+    )
+
+    output = model(input=["OC12COC3=NCC1C23"])  # type: ignore
+
+    assert isinstance(output, list)
+    assert len(output) == 1
+    assert output[0] == 1
+
+
+def test_molformer_multiclass_classification():
+
+    property_class, parameters_class = MOLECULE_PROPERTY_PREDICTOR_FACTORY[
+        "molformer_multitask_classification"
+    ]
+    model = property_class(parameters_class(algorithm_version="molformer_clintox_test"))  # type: ignore
+
+    output = model(input=["OC12COC3=NCC1C23"])  # type: ignore
+
+    assert isinstance(output, list)
+    assert len(output) == 1
+    assert output[0] == "FDA_APPROVED"
+
+
 def test_rfc():
     property_class, parameters_class = CRYSTALS_PROPERTY_PREDICTOR_FACTORY[
         "metal_nonmetal_classifier"
     ]
     model = property_class(parameters_class(algorithm_version="v0"))  # type: ignore
 
     with importlib_resources.as_file(
```

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/tests/test_properties_scorer.py` & `gt4sd-1.2.0/src/gt4sd/properties/tests/test_properties_scorer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/properties/utils.py` & `gt4sd-1.2.0/src/gt4sd/properties/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/s3.py` & `gt4sd-1.2.0/src/gt4sd/s3.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/tests/test_configuration.py` & `gt4sd-1.2.0/src/gt4sd/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/tests/test_exceptions.py` & `gt4sd-1.2.0/src/gt4sd/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/tests/test_s3.py` & `gt4sd-1.2.0/src/gt4sd/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/tests/utils.py` & `gt4sd-1.2.0/src/gt4sd/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,21 @@
 )
 from .pytorch_lightning.language_modeling.core import (
     LanguageModelingDataArguments,
     LanguageModelingModelArguments,
     LanguageModelingSavingArguments,
     LanguageModelingTrainingPipeline,
 )
+from .pytorch_lightning.molformer.core import (
+    MolformerDataArguments,
+    MolformerModelArguments,
+    MolformerSavingArguments,
+    MolformerTrainingArguments,
+    MolformerTrainingPipeline,
+)
 from .regression_transformer.core import (
     RegressionTransformerDataArguments,
     RegressionTransformerSavingArguments,
     RegressionTransformerTrainingArguments,
 )
 from .regression_transformer.implementation import (
     RegressionTransformerModelArguments,
@@ -186,14 +193,19 @@
         CGCNNTrainingArguments,
     ),
     "crystals-rfc": (
         CrystalsRFCDataArguments,
         CrystalsRFCModelArguments,
         CrystalsRFCTrainingArguments,
     ),
+    "molformer": (
+        MolformerDataArguments,
+        MolformerModelArguments,
+        MolformerTrainingArguments,
+    ),
 }
 
 TRAINING_PIPELINE_MAPPING = {
     "language-modeling-trainer": LanguageModelingTrainingPipeline,
     "paccmann-vae-trainer": PaccMannVAETrainingPipeline,
     "torchdrug-gcpn-trainer": TorchDrugGCPNTrainingPipeline,
     "torchdrug-graphaf-trainer": TorchDrugGraphAFTrainingPipeline,
@@ -202,14 +214,15 @@
     "moses-organ-trainer": MosesOrganTrainingPipeline,
     "moses-vae-trainer": MosesVAETrainingPipeline,
     "regression-transformer-trainer": RegressionTransformerTrainingPipeline,
     "diffusion-trainer": DiffusionForVisionTrainingPipeline,
     "gflownet-trainer": GFlowNetTrainingPipeline,
     "cgcnn": CGCNNTrainingPipeline,
     "crystals-rfc": CrystalsRFCTrainingPipeline,
+    "molformer": MolformerTrainingPipeline,
 }
 
 TRAINING_PIPELINE_ARGUMENTS_FOR_MODEL_SAVING = {
     "paccmann-vae-trainer": PaccMannSavingArguments,
     "torchdrug-gcpn-trainer": TorchDrugSavingArguments,
     "torchdrug-graphaf-trainer": TorchDrugSavingArguments,
     "granular-trainer": GranularSavingArguments,
@@ -218,14 +231,15 @@
     "moses-organ-trainer": MosesSavingArguments,
     "moses-vae-trainer": MosesSavingArguments,
     "regression-transformer-trainer": RegressionTransformerSavingArguments,
     "diffusion-trainer": DiffusionSavingArguments,
     "gflownet-trainer": GFlowNetSavingArguments,
     "cgcnn": CGCNNSavingArguments,
     "crystals-rfc": CrystalsRFCSavingArguments,
+    "molformer": MolformerSavingArguments,
 }
 
 
 def training_pipeline_name_to_metadata(name: str) -> Dict[str, Any]:
     """Retrieve training pipeline metadata from the name.
 
     Args:
```

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/cgcnn/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/cgcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/cgcnn/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/cgcnn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/crystals_crf/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/crystals_crf/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/crystals_crf/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/crystals_crf/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/diffusion/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/diffusion/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/diffusion/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/organ/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/organ/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/organ/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/organ/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/vae/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/moses/vae/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/moses/vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/vae/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/paccmann/vae/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/paccmann/vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/lm_datasets.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/lm_datasets.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/models.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/models.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,18 @@
             "help": "Per default, training alternates between property prediction and "
             "conditional generation. This argument specifies the alternation frequency."
             "If you set it to 0, no alternation occurs and we fall back to vanilla "
             "permutation language modeling (PLM). Default: 50."
         },
     )
     cc_loss: bool = field(
-        default=True,
+        default=False,
         metadata={
             "help": "Whether the cycle-consistency loss is computed during the conditional "
-            "generation task. Defaults to True."
+            "generation task. Defaults to False."
         },
     )
     cg_collator: str = field(
         default="vanilla_cg",
         metadata={
             "help": "The collator class. Following options are implemented: "
             "'vanilla_cg': Collator class that does not mask the properties but anything else as a regular DataCollatorForPermutationLanguageModeling. Can optionally replace the properties with sampled values. "
```

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/implementation.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/regression_transformer/utils.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/regression_transformer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     minimum: float = 0
     maximum: float = 0
     expression_separator: str = "|"
     normalize: bool = False
 
     def __init__(self, name: str):
         self.name = name
+        if not name.strip("<>").isalnum():
+            raise ValueError(f"Properties have to be alphanumerics, not {name}.")
         self.mask_lengths: List = []
 
     def update(self, line: str):
         prop = line.split(self.name)[-1].split(self.expression_separator)[0]
         try:
             val = float(prop)
         except ValueError:
```

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/terminator_training.json` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/terminator_training.json`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/molecules.smi` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/molecules.smi`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_argument_parser.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_cgnn.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_cgnn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_diffusion.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_diffusion.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_gflownet.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_gflownet.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_language_modeling.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_language_modeling.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_pipelines.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_pipelines.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/dataset.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd/training_pipelines/torchdrug/unpatch.py` & `gt4sd-1.2.0/src/gt4sd/training_pipelines/torchdrug/unpatch.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.1.9/src/gt4sd.egg-info/PKG-INFO` & `gt4sd-1.2.0/src/gt4sd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt4sd
-Version: 1.1.9
+Version: 1.2.0
 Summary: Generative Toolkit for Scientific Discovery (GT4SD).
 Author: GT4SD team
 Keywords: GT4SD Generative Models Inference Training
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gt4sd-1.1.9/src/gt4sd.egg-info/SOURCES.txt` & `gt4sd-1.2.0/src/gt4sd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,16 @@
 src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py
 src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py
 src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py
 src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/__init__.py
 src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/core.py
 src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/lm_datasets.py
 src/gt4sd/training_pipelines/pytorch_lightning/language_modeling/models.py
+src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py
+src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py
 src/gt4sd/training_pipelines/regression_transformer/__init__.py
 src/gt4sd/training_pipelines/regression_transformer/core.py
 src/gt4sd/training_pipelines/regression_transformer/implementation.py
 src/gt4sd/training_pipelines/regression_transformer/utils.py
 src/gt4sd/training_pipelines/tests/__init__.py
 src/gt4sd/training_pipelines/tests/molecules.smi
 src/gt4sd/training_pipelines/tests/test_argument_parser.py
```

