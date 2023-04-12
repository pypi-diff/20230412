# Comparing `tmp/UtilsRL-0.5.6.tar.gz` & `tmp/UtilsRL-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UtilsRL-0.5.6.tar", last modified: Tue Apr 11 03:05:11 2023, max compression
+gzip compressed data, was "UtilsRL-0.5.7.tar", last modified: Wed Apr 12 12:38:21 2023, max compression
```

## Comparing `UtilsRL-0.5.6.tar` & `UtilsRL-0.5.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/data_structure/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/data_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/data_structure/data_structure.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/env/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/env/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/atari_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/dmc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/mujoco_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/exp/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/composite_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/text_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/math/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/math/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/chore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/net/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/plot/tb_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/UtilsRL/rl/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/prioritized_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/transition_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/trjectory_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/video_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/UtilsRL/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/third_party/tqdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.710516 UtilsRL-0.5.7/UtilsRL/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.710516 UtilsRL-0.5.7/UtilsRL/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/data_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/data_structure/data_structure.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.710516 UtilsRL-0.5.7/UtilsRL/env/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.714516 UtilsRL-0.5.7/UtilsRL/env/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/env/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/env/wrapper/atari_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/env/wrapper/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/env/wrapper/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/env/wrapper/dmc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/env/wrapper/mujoco_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.714516 UtilsRL-0.5.7/UtilsRL/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/exp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/exp/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/exp/_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/exp/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/exp/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/exp/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.714516 UtilsRL-0.5.7/UtilsRL/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/logger/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/logger/composite_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/logger/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/logger/text_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/logger/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.714516 UtilsRL-0.5.7/UtilsRL/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/math/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.714516 UtilsRL-0.5.7/UtilsRL/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/misc/chore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/misc/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/misc/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/UtilsRL/net/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/net/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/net/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/net/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/net/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/UtilsRL/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/plot/tb_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/UtilsRL/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/UtilsRL/rl/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/buffer/prioritized_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/buffer/transition_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/buffer/trjectory_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/rl/video_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/UtilsRL/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/UtilsRL/third_party/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:21.710516 UtilsRL-0.5.7/UtilsRL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-12 12:38:21.000000 UtilsRL-0.5.7/UtilsRL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 12:38:21.000000 UtilsRL-0.5.7/UtilsRL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:38:21.000000 UtilsRL-0.5.7/UtilsRL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 12:38:21.000000 UtilsRL-0.5.7/UtilsRL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 12:38:21.000000 UtilsRL-0.5.7/UtilsRL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:38:21.718516 UtilsRL-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-12 12:38:13.000000 UtilsRL-0.5.7/setup.py
```

### Comparing `UtilsRL-0.5.6/LICENSE` & `UtilsRL-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/PKG-INFO` & `UtilsRL-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.5.6
+Version: 0.5.7
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `UtilsRL-0.5.6/README.md` & `UtilsRL-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/data_structure/data_structure.cc` & `UtilsRL-0.5.7/UtilsRL/data_structure/data_structure.cc`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/env/wrapper/atari_wrapper.py` & `UtilsRL-0.5.7/UtilsRL/env/wrapper/atari_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/env/wrapper/base_wrapper.py` & `UtilsRL-0.5.7/UtilsRL/env/wrapper/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/env/wrapper/compat.py` & `UtilsRL-0.5.7/UtilsRL/env/wrapper/compat.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/env/wrapper/dmc_wrapper.py` & `UtilsRL-0.5.7/UtilsRL/env/wrapper/dmc_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/env/wrapper/mujoco_wrapper.py` & `UtilsRL-0.5.7/UtilsRL/env/wrapper/mujoco_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/exp/__init__.py` & `UtilsRL-0.5.7/UtilsRL/exp/__init__.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/exp/_device.py` & `UtilsRL-0.5.7/UtilsRL/exp/_device.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/exp/argparse.py` & `UtilsRL-0.5.7/UtilsRL/exp/argparse.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/exp/precision.py` & `UtilsRL-0.5.7/UtilsRL/exp/precision.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/exp/snapshot.py` & `UtilsRL-0.5.7/UtilsRL/exp/snapshot.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/logger/base_logger.py` & `UtilsRL-0.5.7/UtilsRL/logger/base_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/logger/composite_logger.py` & `UtilsRL-0.5.7/UtilsRL/logger/composite_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/logger/tensorboard_logger.py` & `UtilsRL-0.5.7/UtilsRL/logger/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/logger/text_logger.py` & `UtilsRL-0.5.7/UtilsRL/logger/text_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/logger/wandb_logger.py` & `UtilsRL-0.5.7/UtilsRL/logger/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/math/distributions.py` & `UtilsRL-0.5.7/UtilsRL/math/distributions.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/misc/chore.py` & `UtilsRL-0.5.7/UtilsRL/misc/chore.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/misc/decorator.py` & `UtilsRL-0.5.7/UtilsRL/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/misc/namespace.py` & `UtilsRL-0.5.7/UtilsRL/misc/namespace.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/monitor.py` & `UtilsRL-0.5.7/UtilsRL/monitor.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/net/basic.py` & `UtilsRL-0.5.7/UtilsRL/net/basic.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/net/cnn.py` & `UtilsRL-0.5.7/UtilsRL/net/cnn.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/net/mlp.py` & `UtilsRL-0.5.7/UtilsRL/net/mlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 activation_list = activation
             else:
                 activation_list = [activation for _ in range(len(hidden_dims))]
         else:
             activation_list = [None]*len(hidden_dims)
         
         if dropout:
-            if isinstance(dropout. list):
+            if isinstance(dropout, list):
                 assert len(dropout) == len(hidden_dims)
                 dropout_list = dropout
             else:
                 dropout_list = [dropout for _ in range(len(hidden_dims))]
         else:
             dropout_list = [None]*len(hidden_dims)
                         
@@ -143,15 +143,15 @@
                 activation_list = activation
             else:
                 activation_list = [activation for _ in range(len(hidden_dims))]
         else:
             activation_list = [None]*len(hidden_dims)
             
         if dropout:
-            if isinstance(dropout. list):
+            if isinstance(dropout, list):
                 assert len(dropout) == len(hidden_dims)
                 dropout_list = dropout
             else:
                 dropout_list = [dropout for _ in range(len(hidden_dims))]
         else:
             dropout_list = [None]*len(hidden_dims)
```

### Comparing `UtilsRL-0.5.6/UtilsRL/net/rnn.py` & `UtilsRL-0.5.7/UtilsRL/net/rnn.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/plot/tb_parser.py` & `UtilsRL-0.5.7/UtilsRL/plot/tb_parser.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/actor.py` & `UtilsRL-0.5.7/UtilsRL/rl/actor.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/buffer/__init__.py` & `UtilsRL-0.5.7/UtilsRL/rl/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/buffer/base.py` & `UtilsRL-0.5.7/UtilsRL/rl/buffer/base.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/buffer/prioritized_replay.py` & `UtilsRL-0.5.7/UtilsRL/rl/buffer/prioritized_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/buffer/transition_replay.py` & `UtilsRL-0.5.7/UtilsRL/rl/buffer/transition_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/buffer/trjectory_replay.py` & `UtilsRL-0.5.7/UtilsRL/rl/buffer/trjectory_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/critic.py` & `UtilsRL-0.5.7/UtilsRL/rl/critic.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/normalizer.py` & `UtilsRL-0.5.7/UtilsRL/rl/normalizer.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/rl/video_recorder.py` & `UtilsRL-0.5.7/UtilsRL/rl/video_recorder.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL/third_party/tqdm.py` & `UtilsRL-0.5.7/UtilsRL/third_party/tqdm.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/UtilsRL.egg-info/PKG-INFO` & `UtilsRL-0.5.7/UtilsRL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.5.6
+Version: 0.5.7
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `UtilsRL-0.5.6/UtilsRL.egg-info/SOURCES.txt` & `UtilsRL-0.5.7/UtilsRL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.6/setup.py` & `UtilsRL-0.5.7/setup.py`

 * *Files identical despite different names*

