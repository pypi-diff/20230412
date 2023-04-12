# Comparing `tmp/gymnax-0.0.5.tar.gz` & `tmp/gymnax-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnax-0.0.5.tar", last modified: Wed Aug 24 10:34:38 2022, max compression
+gzip compressed data, was "gymnax-0.0.6.tar", last modified: Wed Apr 12 10:41:43 2023, max compression
```

## Comparing `gymnax-0.0.5.tar` & `gymnax-0.0.6.tar`

### file list

```diff
@@ -1,67 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.903502 gymnax-0.0.5/
--rwxr-xr-x   0 runner    (1001) docker     (121)    10238 2022-08-24 10:34:31.000000 gymnax-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18246 2022-08-24 10:34:38.903502 gymnax-0.0.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)    17525 2022-08-24 10:34:31.000000 gymnax-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.887501 gymnax-0.0.5/gymnax/
--rwxr-xr-x   0 runner    (1001) docker     (121)       88 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.891501 gymnax-0.0.5/gymnax/environments/
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.895501 gymnax-0.0.5/gymnax/environments/bsuite/
--rwxr-xr-x   0 runner    (1001) docker     (121)      394 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3461 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/bandit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5812 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/catch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7373 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/deep_sea.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3929 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/discounting_chain.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4990 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/memory_chain.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3546 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/mnist.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4758 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/bsuite/umbrella_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.895501 gymnax-0.0.5/gymnax/environments/classic_control/
--rwxr-xr-x   0 runner    (1001) docker     (121)      299 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/classic_control/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8193 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/classic_control/acrobot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5760 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/classic_control/cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5001 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/classic_control/continuous_mountain_car.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4481 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/classic_control/mountain_car.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5048 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/classic_control/pendulum.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3398 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.895501 gymnax-0.0.5/gymnax/environments/minatar/
--rwxr-xr-x   0 runner    (1001) docker     (121)      291 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/minatar/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13951 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/minatar/asterix.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9826 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/minatar/breakout.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10796 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/minatar/freeway.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18373 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/minatar/seaquest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13355 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/minatar/space_invaders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.899502 gymnax-0.0.5/gymnax/environments/misc/
--rwxr-xr-x   0 runner    (1001) docker     (121)      298 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/misc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4419 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/misc/bernoulli_bandit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5058 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/misc/gaussian_bandit.py
--rw-r--r--   0 runner    (1001) docker     (121)     9414 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/misc/meta_maze.py
--rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/misc/point_robot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8335 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/misc/rooms.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4003 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/environments/spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.899502 gymnax-0.0.5/gymnax/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/experimental/rollout.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3294 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.899502 gymnax-0.0.5/gymnax/utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)      276 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2807 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/utils/load_mnist.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11090 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/utils/state_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2344 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/utils/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.903502 gymnax-0.0.5/gymnax/visualize/
--rwxr-xr-x   0 runner    (1001) docker     (121)       69 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/visualize/vis_catch.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/visualize/vis_circle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/visualize/vis_gym.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/visualize/vis_maze.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/visualize/vis_minatar.py
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-08-24 10:34:31.000000 gymnax-0.0.5/gymnax/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:34:38.891501 gymnax-0.0.5/gymnax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18246 2022-08-24 10:34:38.000000 gymnax-0.0.5/gymnax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-08-24 10:34:38.000000 gymnax-0.0.5/gymnax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 10:34:38.000000 gymnax-0.0.5/gymnax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 10:34:38.000000 gymnax-0.0.5/gymnax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-24 10:34:38.000000 gymnax-0.0.5/gymnax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-24 10:34:38.000000 gymnax-0.0.5/gymnax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 10:34:38.903502 gymnax-0.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1925 2022-08-24 10:34:31.000000 gymnax-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.525940 gymnax-0.0.6/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10238 2023-04-12 10:41:31.000000 gymnax-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-04-12 10:41:43.525940 gymnax-0.0.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18579 2023-04-12 10:41:31.000000 gymnax-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.517939 gymnax-0.0.6/gymnax/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.517939 gymnax-0.0.6/gymnax/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.517939 gymnax-0.0.6/gymnax/environments/bsuite/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      394 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3461 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/bandit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5812 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/catch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7373 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/deep_sea.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4067 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/discounting_chain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4990 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/memory_chain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/mnist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4758 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/bsuite/umbrella_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.517939 gymnax-0.0.6/gymnax/environments/classic_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/classic_control/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8348 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/classic_control/acrobot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5790 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/classic_control/cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5035 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/classic_control/continuous_mountain_car.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/classic_control/mountain_car.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5112 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/classic_control/pendulum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3404 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.521939 gymnax-0.0.6/gymnax/environments/minatar/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/minatar/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13951 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/minatar/asterix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9826 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/minatar/breakout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10796 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/minatar/freeway.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18370 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/minatar/seaquest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13355 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/minatar/space_invaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.521939 gymnax-0.0.6/gymnax/environments/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4947 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/bernoulli_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/gaussian_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/meta_maze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/point_robot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12650 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/pong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/reacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/misc/swimmer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5146 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/environments/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.521939 gymnax-0.0.6/gymnax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/experimental/rollout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3688 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.521939 gymnax-0.0.6/gymnax/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2807 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/utils/load_mnist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11090 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/utils/state_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2688 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/utils/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.521939 gymnax-0.0.6/gymnax/visualize/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/visualize/vis_catch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/visualize/vis_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/visualize/vis_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/visualize/vis_maze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/visualize/vis_minatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.521939 gymnax-0.0.6/gymnax/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/wrappers/brax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/wrappers/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/wrappers/evojax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/wrappers/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-12 10:41:31.000000 gymnax-0.0.6/gymnax/wrappers/purerl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:41:43.517939 gymnax-0.0.6/gymnax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-04-12 10:41:43.000000 gymnax-0.0.6/gymnax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-12 10:41:43.000000 gymnax-0.0.6/gymnax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:41:43.000000 gymnax-0.0.6/gymnax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:41:43.000000 gymnax-0.0.6/gymnax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:41:43.000000 gymnax-0.0.6/gymnax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 10:41:43.000000 gymnax-0.0.6/gymnax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:41:43.525940 gymnax-0.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1942 2023-04-12 10:41:31.000000 gymnax-0.0.6/setup.py
```

### Comparing `gymnax-0.0.5/LICENSE` & `gymnax-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/PKG-INFO` & `gymnax-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gymnax
-Version: 0.0.5
+Version: 0.0.6
 Summary: JAX-compatible version of Open AI's gym environments
 Home-page: https://github.com/RobertTLange/gymnax
-Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.5.tar.gz
+Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.6.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -85,14 +85,17 @@
 | [`SimpleBandit-bsuite`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/bsuite/bandit.py) | [Osband et al. (2019)](https://openreview.net/forum?id=rygf-kSYwH) | [Click](https://github.com/deepmind/bsuite/blob/master/bsuite/environments/bandit.py)  | - | -
 |  |  |  |  | 
 | [`FourRooms-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/rooms.py) | [Sutton et al. (1999)](https://people.cs.umass.edu/~barto/courses/cs687/Sutton-Precup-Singh-AIJ99.pdf) | [Click](https://github.com/howardh/gym-fourrooms) | [PPO, ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/FourRooms-misc) (R: 1) | 0.07
 | [`MetaMaze-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/meta_maze.py) | [Micconi et al. (2020)](https://arxiv.org/abs/2002.10585)  | [Click](https://github.com/uber-research/backpropamine/blob/master/simplemaze/maze.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/MetaMaze-misc) (R: 32) | 0.09
 | [`PointRobot-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/point_robot.py) | [Dorfman et al. (2021)](https://openreview.net/pdf?id=IBdEfhLveS) | [Click](https://github.com/Rondorf/BOReL/blob/main/environments/toy_navigation/point_robot.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/PointRobot-misc) (R: 10) | 0.08
 | [`BernoulliBandit-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/bernoulli_bandit.py) | [Wang et al. (2017)](https://arxiv.org/abs/1611.05763) | [Click](https://github.com/RobertTLange/minimal-meta-rl/blob/main/bandits/bandit_env.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/BernoulliBandit-misc) (R: 90) | 0.08
 | [`GaussianBandit-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/gaussian_bandit.py) | [Lange & Sprekeler (2022)](https://arxiv.org/abs/2010.04466) | [Click](https://github.com/RobertTLange/learning-not-to-learn) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07
+| [`Reacher-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/reacher.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://github.com/unifyai/gym/blob/master/ivy_gym/reacher.py) | 
+| [`Swimmer-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/swimmer.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://github.com/unifyai/gym/blob/master/ivy_gym/swimmer.py) |
+| [`Pong-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/pong.py) | [Kirsch (2018)](https://github.com/BlackHC/batch_pong_poc) | [Click](https://github.com/BlackHC/batch_pong_poc/blob/master/src/vanilla_pong.py) |  
 
 \* All displayed speeds are estimated for 1M step transitions (random policy) on a NVIDIA A100 GPU using `jit` compiled episode rollouts with 2000 environment workers. For more detailed speed comparisons on different accelerators (CPU, RTX 2080Ti) and MLP policies, please refer to the [`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines) documentation.
 
 
 ## Installation ⏳
 
 The latest `gymnax` release can directly be installed from PyPI:
@@ -109,14 +112,15 @@
 
 In order to use JAX on your accelerators, you can find more details in the [JAX documentation](https://github.com/google/jax#installation).
 
 ## Examples 📖
 * 📓 [Environment API](examples/getting_started.ipynb) - Get started with the basic `gymnax` API.
 * 📓 [Distributed Anakin Agent](examples/01_anakin.ipynb) - Train an Anakin [(Hessel et al., 2021)](https://arxiv.org/pdf/2104.06272.pdf) agent on `SpaceInvaders-MinAtar`.
 * 📓 [ES with `gymnax`](examples/02_evolution.ipynb) - Meta-evolve an LSTM controller that controls 2 link pendula of different lengths.
+* 📓 [Bandit A2C Meta-RL](examples/03_meta_a2c.ipynb) - Meta-learn an A2C LSTM that learns to explore/exploit in multi-arm bandit tasks.
 * 📓 [Trained baselines](https://github.com/RobertTLange/gymnax-blines) - Check out the trained baseline agents (PPO/ES) in `gymnax-blines`.
 
 ## Key Selling Points 💵
 
 - **Environment vectorization & acceleration**: Easy composition of JAX primitives (e.g. `jit`, `vmap`, `pmap`):
 
   ```python
@@ -217,15 +221,16 @@
       rng_batch, batch_params
   )
   ```
 
 ## Resources & Other Great Tools 📝
 * 💻 [Brax](https://github.com/google/brax): JAX-based library for rigid body physics by Google Brain with JAX-style MuJoCo substitutes.
 * 💻 [envpool](https://github.com/sail-sg/envpool): Vectorized parallel environment execution engine.
-
+* 💻 [Jumaji](https://github.com/instadeepai/jumanji): Industry-driven JAX-based RL environments.
+* 💻 [Pgx](https://github.com/sotetsuk/pgx): JAX-based classic board game environments.
 
 ### Acknowledgements & Citing `gymnax` ✏️
 
 If you use `gymnax` in your research, please cite it as follows:
 
 ```
 @software{gymnax2022github,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: gymnax Version: 0.0.5 Summary: JAX-compatible
+Metadata-Version: 2.1 Name: gymnax Version: 0.0.6 Summary: JAX-compatible
 version of Open AI's gym environments Home-page: https://github.com/
 RobertTLange/gymnax Download-URL: https://github.com/RobertTLange/gymnax/
-archive/v0.0.5.tar.gz Author: Robert Tjarko Lange Author-email:
+archive/v0.0.6.tar.gz Author: Robert Tjarko Lange Author-email:
 robertlange0@gmail.com Platform: any Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
         ****** [https://github.com/RobertTLange/gymnax/blob/main/docs/
@@ -142,49 +142,60 @@
 (https://arxiv.org/abs/1611.05763) | [Click](https://github.com/RobertTLange/
 minimal-meta-rl/blob/main/bandits/bandit_env.py) | [ES](https://github.com/
 RobertTLange/gymnax-blines/tree/main/agents/BernoulliBandit-misc) (R: 90) |
 0.08 | [`GaussianBandit-misc`](https://github.com/RobertTLange/gymnax/blob/
 main/gymnax/environments/misc/gaussian_bandit.py) | [Lange & Sprekeler (2022)]
 (https://arxiv.org/abs/2010.04466) | [Click](https://github.com/RobertTLange/
 learning-not-to-learn) | [ES](https://github.com/RobertTLange/gymnax-blines/
-tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07 \* All displayed speeds are
-estimated for 1M step transitions (random policy) on a NVIDIA A100 GPU using
-`jit` compiled episode rollouts with 2000 environment workers. For more
-detailed speed comparisons on different accelerators (CPU, RTX 2080Ti) and MLP
-policies, please refer to the [`gymnax-blines`](https://github.com/
-RobertTLange/gymnax-blines) documentation. ## Installation â³ The latest
-`gymnax` release can directly be installed from PyPI: ``` pip install gymnax
-``` If you want to get the most recent commit, please install directly from the
-repository: ``` pip install git+https://github.com/RobertTLange/gymnax.git@main
-``` In order to use JAX on your accelerators, you can find more details in the
-[JAX documentation](https://github.com/google/jax#installation). ## Examples
-ð * ð [Environment API](examples/getting_started.ipynb) - Get started
-with the basic `gymnax` API. * ð [Distributed Anakin Agent](examples/
-01_anakin.ipynb) - Train an Anakin [(Hessel et al., 2021)](https://arxiv.org/
-pdf/2104.06272.pdf) agent on `SpaceInvaders-MinAtar`. * ð [ES with `gymnax`]
-(examples/02_evolution.ipynb) - Meta-evolve an LSTM controller that controls 2
-link pendula of different lengths. * ð [Trained baselines](https://
-github.com/RobertTLange/gymnax-blines) - Check out the trained baseline agents
-(PPO/ES) in `gymnax-blines`. ## Key Selling Points ðµ - **Environment
-vectorization & acceleration**: Easy composition of JAX primitives (e.g. `jit`,
-`vmap`, `pmap`): ```python # Jit-accelerated step transition jit_step = jax.jit
-(env.step) # map (vmap/pmap) across random keys for batch rollouts reset_rng =
-jax.vmap(env.reset, in_axes=(0, None)) step_rng = jax.vmap(env.step, in_axes=
-(0, 0, 0, None)) # map (vmap/pmap) across env parameters (e.g. for meta-
-learning) reset_params = jax.vmap(env.reset, in_axes=(None, 0)) step_params =
-jax.vmap(env.step, in_axes=(None, 0, 0, 0)) ``` For speed comparisons with
-standard vectorized NumPy environments check out [`gymnax-blines`](https://
-github.com/RobertTLange/gymnax-blines). - **Scan through entire episode
-rollouts**: You can also `lax.scan` through entire `reset`, `step` episode
-loops for fast compilation: ```python def rollout(rng_input, policy_params,
-env_params, steps_in_episode): """Rollout a jitted gymnax episode with
-lax.scan.""" # Reset the environment rng_reset, rng_episode = jax.random.split
-(rng_input) obs, state = env.reset(rng_reset, env_params) def policy_step
-(state_input, tmp): """lax.scan compatible step transition in jax env.""" obs,
-state, policy_params, rng = state_input rng, rng_step, rng_net =
+tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07 | [`Reacher-misc`](https://
+github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/reacher.py) |
+[Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://
+github.com/unifyai/gym/blob/master/ivy_gym/reacher.py) | | [`Swimmer-misc`]
+(https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/
+swimmer.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click]
+(https://github.com/unifyai/gym/blob/master/ivy_gym/swimmer.py) | | [`Pong-
+misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/
+misc/pong.py) | [Kirsch (2018)](https://github.com/BlackHC/batch_pong_poc) |
+[Click](https://github.com/BlackHC/batch_pong_poc/blob/master/src/
+vanilla_pong.py) | \* All displayed speeds are estimated for 1M step
+transitions (random policy) on a NVIDIA A100 GPU using `jit` compiled episode
+rollouts with 2000 environment workers. For more detailed speed comparisons on
+different accelerators (CPU, RTX 2080Ti) and MLP policies, please refer to the
+[`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines) documentation.
+## Installation â³ The latest `gymnax` release can directly be installed from
+PyPI: ``` pip install gymnax ``` If you want to get the most recent commit,
+please install directly from the repository: ``` pip install git+https://
+github.com/RobertTLange/gymnax.git@main ``` In order to use JAX on your
+accelerators, you can find more details in the [JAX documentation](https://
+github.com/google/jax#installation). ## Examples ð * ð [Environment API]
+(examples/getting_started.ipynb) - Get started with the basic `gymnax` API. *
+ð [Distributed Anakin Agent](examples/01_anakin.ipynb) - Train an Anakin [
+(Hessel et al., 2021)](https://arxiv.org/pdf/2104.06272.pdf) agent on
+`SpaceInvaders-MinAtar`. * ð [ES with `gymnax`](examples/02_evolution.ipynb)
+- Meta-evolve an LSTM controller that controls 2 link pendula of different
+lengths. * ð [Bandit A2C Meta-RL](examples/03_meta_a2c.ipynb) - Meta-learn
+an A2C LSTM that learns to explore/exploit in multi-arm bandit tasks. * ð
+[Trained baselines](https://github.com/RobertTLange/gymnax-blines) - Check out
+the trained baseline agents (PPO/ES) in `gymnax-blines`. ## Key Selling Points
+ðµ - **Environment vectorization & acceleration**: Easy composition of JAX
+primitives (e.g. `jit`, `vmap`, `pmap`): ```python # Jit-accelerated step
+transition jit_step = jax.jit(env.step) # map (vmap/pmap) across random keys
+for batch rollouts reset_rng = jax.vmap(env.reset, in_axes=(0, None)) step_rng
+= jax.vmap(env.step, in_axes=(0, 0, 0, None)) # map (vmap/pmap) across env
+parameters (e.g. for meta-learning) reset_params = jax.vmap(env.reset, in_axes=
+(None, 0)) step_params = jax.vmap(env.step, in_axes=(None, 0, 0, 0)) ``` For
+speed comparisons with standard vectorized NumPy environments check out
+[`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines). - **Scan
+through entire episode rollouts**: You can also `lax.scan` through entire
+`reset`, `step` episode loops for fast compilation: ```python def rollout
+(rng_input, policy_params, env_params, steps_in_episode): """Rollout a jitted
+gymnax episode with lax.scan.""" # Reset the environment rng_reset, rng_episode
+= jax.random.split(rng_input) obs, state = env.reset(rng_reset, env_params) def
+policy_step(state_input, tmp): """lax.scan compatible step transition in jax
+env.""" obs, state, policy_params, rng = state_input rng, rng_step, rng_net =
 jax.random.split(rng, 3) action = model.apply(policy_params, obs) next_obs,
 next_state, reward, done, _ = env.step( rng_step, state, action, env_params )
 carry = [next_obs, next_state, policy_params, rng] return carry, [obs, action,
 reward, next_obs, done] # Scan over episode step loop _, scan_out =
 jax.lax.scan( policy_step, [obs, state, policy_params, rng_episode], (),
 steps_in_episode ) # Return masked sum of rewards accumulated by agent in
 episode obs, action, reward, next_obs, done = scan_out return obs, action,
@@ -213,20 +224,22 @@
 policy_params ) # Multiple rollouts for different networks + rng (e.g. for ES)
 batch_params = jax.tree_map( # Stack parameters or use different lambda x:
 jnp.tile(x, (5, 1)).reshape(5, *x.shape), policy_params ) obs, action, reward,
 next_obs, done, cum_ret = manager.population_rollout( rng_batch, batch_params )
 ``` ## Resources & Other Great Tools ð * ð» [Brax](https://github.com/
 google/brax): JAX-based library for rigid body physics by Google Brain with
 JAX-style MuJoCo substitutes. * ð» [envpool](https://github.com/sail-sg/
-envpool): Vectorized parallel environment execution engine. ###
-Acknowledgements & Citing `gymnax` âï¸ If you use `gymnax` in your research,
-please cite it as follows: ``` @software{gymnax2022github, author = {Robert
-Tjarko Lange}, title = {{gymnax}: A {JAX}-based Reinforcement Learning
-Environment Library}, url = {http://github.com/RobertTLange/gymnax}, version =
-{0.0.4}, year = {2022}, } ``` We acknowledge financial support by the [Google
-TRC](https://sites.research.google/trc/about/) and the Deutsche
-Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's
-Excellence Strategy - EXC 2002/1 ["Science of Intelligence"](https://
-www.scienceofintelligence.de/) - project number 390523135. ## Development ð·
-You can run the test suite via `python -m pytest -vv --all`. If you find a bug
-or are missing your favourite feature, feel free to create an issue and/or
-start [contributing](CONTRIBUTING.md) ð¤.
+envpool): Vectorized parallel environment execution engine. * ð» [Jumaji]
+(https://github.com/instadeepai/jumanji): Industry-driven JAX-based RL
+environments. * ð» [Pgx](https://github.com/sotetsuk/pgx): JAX-based classic
+board game environments. ### Acknowledgements & Citing `gymnax` âï¸ If you
+use `gymnax` in your research, please cite it as follows: ``` @software
+{gymnax2022github, author = {Robert Tjarko Lange}, title = {{gymnax}: A {JAX}-
+based Reinforcement Learning Environment Library}, url = {http://github.com/
+RobertTLange/gymnax}, version = {0.0.4}, year = {2022}, } ``` We acknowledge
+financial support by the [Google TRC](https://sites.research.google/trc/about/
+) and the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation)
+under Germany's Excellence Strategy - EXC 2002/1 ["Science of Intelligence"]
+(https://www.scienceofintelligence.de/) - project number 390523135. ##
+Development ð· You can run the test suite via `python -m pytest -vv --all`.
+If you find a bug or are missing your favourite feature, feel free to create an
+issue and/or start [contributing](CONTRIBUTING.md) ð¤.
```

### Comparing `gymnax-0.0.5/README.md` & `gymnax-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 | [`SimpleBandit-bsuite`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/bsuite/bandit.py) | [Osband et al. (2019)](https://openreview.net/forum?id=rygf-kSYwH) | [Click](https://github.com/deepmind/bsuite/blob/master/bsuite/environments/bandit.py)  | - | -
 |  |  |  |  | 
 | [`FourRooms-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/rooms.py) | [Sutton et al. (1999)](https://people.cs.umass.edu/~barto/courses/cs687/Sutton-Precup-Singh-AIJ99.pdf) | [Click](https://github.com/howardh/gym-fourrooms) | [PPO, ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/FourRooms-misc) (R: 1) | 0.07
 | [`MetaMaze-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/meta_maze.py) | [Micconi et al. (2020)](https://arxiv.org/abs/2002.10585)  | [Click](https://github.com/uber-research/backpropamine/blob/master/simplemaze/maze.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/MetaMaze-misc) (R: 32) | 0.09
 | [`PointRobot-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/point_robot.py) | [Dorfman et al. (2021)](https://openreview.net/pdf?id=IBdEfhLveS) | [Click](https://github.com/Rondorf/BOReL/blob/main/environments/toy_navigation/point_robot.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/PointRobot-misc) (R: 10) | 0.08
 | [`BernoulliBandit-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/bernoulli_bandit.py) | [Wang et al. (2017)](https://arxiv.org/abs/1611.05763) | [Click](https://github.com/RobertTLange/minimal-meta-rl/blob/main/bandits/bandit_env.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/BernoulliBandit-misc) (R: 90) | 0.08
 | [`GaussianBandit-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/gaussian_bandit.py) | [Lange & Sprekeler (2022)](https://arxiv.org/abs/2010.04466) | [Click](https://github.com/RobertTLange/learning-not-to-learn) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07
+| [`Reacher-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/reacher.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://github.com/unifyai/gym/blob/master/ivy_gym/reacher.py) | 
+| [`Swimmer-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/swimmer.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://github.com/unifyai/gym/blob/master/ivy_gym/swimmer.py) |
+| [`Pong-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/pong.py) | [Kirsch (2018)](https://github.com/BlackHC/batch_pong_poc) | [Click](https://github.com/BlackHC/batch_pong_poc/blob/master/src/vanilla_pong.py) |  
 
 \* All displayed speeds are estimated for 1M step transitions (random policy) on a NVIDIA A100 GPU using `jit` compiled episode rollouts with 2000 environment workers. For more detailed speed comparisons on different accelerators (CPU, RTX 2080Ti) and MLP policies, please refer to the [`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines) documentation.
 
 
 ## Installation ⏳
 
 The latest `gymnax` release can directly be installed from PyPI:
@@ -90,14 +93,15 @@
 
 In order to use JAX on your accelerators, you can find more details in the [JAX documentation](https://github.com/google/jax#installation).
 
 ## Examples 📖
 * 📓 [Environment API](examples/getting_started.ipynb) - Get started with the basic `gymnax` API.
 * 📓 [Distributed Anakin Agent](examples/01_anakin.ipynb) - Train an Anakin [(Hessel et al., 2021)](https://arxiv.org/pdf/2104.06272.pdf) agent on `SpaceInvaders-MinAtar`.
 * 📓 [ES with `gymnax`](examples/02_evolution.ipynb) - Meta-evolve an LSTM controller that controls 2 link pendula of different lengths.
+* 📓 [Bandit A2C Meta-RL](examples/03_meta_a2c.ipynb) - Meta-learn an A2C LSTM that learns to explore/exploit in multi-arm bandit tasks.
 * 📓 [Trained baselines](https://github.com/RobertTLange/gymnax-blines) - Check out the trained baseline agents (PPO/ES) in `gymnax-blines`.
 
 ## Key Selling Points 💵
 
 - **Environment vectorization & acceleration**: Easy composition of JAX primitives (e.g. `jit`, `vmap`, `pmap`):
 
   ```python
@@ -198,15 +202,16 @@
       rng_batch, batch_params
   )
   ```
 
 ## Resources & Other Great Tools 📝
 * 💻 [Brax](https://github.com/google/brax): JAX-based library for rigid body physics by Google Brain with JAX-style MuJoCo substitutes.
 * 💻 [envpool](https://github.com/sail-sg/envpool): Vectorized parallel environment execution engine.
-
+* 💻 [Jumaji](https://github.com/instadeepai/jumanji): Industry-driven JAX-based RL environments.
+* 💻 [Pgx](https://github.com/sotetsuk/pgx): JAX-based classic board game environments.
 
 ### Acknowledgements & Citing `gymnax` ✏️
 
 If you use `gymnax` in your research, please cite it as follows:
 
 ```
 @software{gymnax2022github,
```

#### html2text {}

```diff
@@ -132,49 +132,60 @@
 (https://arxiv.org/abs/1611.05763) | [Click](https://github.com/RobertTLange/
 minimal-meta-rl/blob/main/bandits/bandit_env.py) | [ES](https://github.com/
 RobertTLange/gymnax-blines/tree/main/agents/BernoulliBandit-misc) (R: 90) |
 0.08 | [`GaussianBandit-misc`](https://github.com/RobertTLange/gymnax/blob/
 main/gymnax/environments/misc/gaussian_bandit.py) | [Lange & Sprekeler (2022)]
 (https://arxiv.org/abs/2010.04466) | [Click](https://github.com/RobertTLange/
 learning-not-to-learn) | [ES](https://github.com/RobertTLange/gymnax-blines/
-tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07 \* All displayed speeds are
-estimated for 1M step transitions (random policy) on a NVIDIA A100 GPU using
-`jit` compiled episode rollouts with 2000 environment workers. For more
-detailed speed comparisons on different accelerators (CPU, RTX 2080Ti) and MLP
-policies, please refer to the [`gymnax-blines`](https://github.com/
-RobertTLange/gymnax-blines) documentation. ## Installation â³ The latest
-`gymnax` release can directly be installed from PyPI: ``` pip install gymnax
-``` If you want to get the most recent commit, please install directly from the
-repository: ``` pip install git+https://github.com/RobertTLange/gymnax.git@main
-``` In order to use JAX on your accelerators, you can find more details in the
-[JAX documentation](https://github.com/google/jax#installation). ## Examples
-ð * ð [Environment API](examples/getting_started.ipynb) - Get started
-with the basic `gymnax` API. * ð [Distributed Anakin Agent](examples/
-01_anakin.ipynb) - Train an Anakin [(Hessel et al., 2021)](https://arxiv.org/
-pdf/2104.06272.pdf) agent on `SpaceInvaders-MinAtar`. * ð [ES with `gymnax`]
-(examples/02_evolution.ipynb) - Meta-evolve an LSTM controller that controls 2
-link pendula of different lengths. * ð [Trained baselines](https://
-github.com/RobertTLange/gymnax-blines) - Check out the trained baseline agents
-(PPO/ES) in `gymnax-blines`. ## Key Selling Points ðµ - **Environment
-vectorization & acceleration**: Easy composition of JAX primitives (e.g. `jit`,
-`vmap`, `pmap`): ```python # Jit-accelerated step transition jit_step = jax.jit
-(env.step) # map (vmap/pmap) across random keys for batch rollouts reset_rng =
-jax.vmap(env.reset, in_axes=(0, None)) step_rng = jax.vmap(env.step, in_axes=
-(0, 0, 0, None)) # map (vmap/pmap) across env parameters (e.g. for meta-
-learning) reset_params = jax.vmap(env.reset, in_axes=(None, 0)) step_params =
-jax.vmap(env.step, in_axes=(None, 0, 0, 0)) ``` For speed comparisons with
-standard vectorized NumPy environments check out [`gymnax-blines`](https://
-github.com/RobertTLange/gymnax-blines). - **Scan through entire episode
-rollouts**: You can also `lax.scan` through entire `reset`, `step` episode
-loops for fast compilation: ```python def rollout(rng_input, policy_params,
-env_params, steps_in_episode): """Rollout a jitted gymnax episode with
-lax.scan.""" # Reset the environment rng_reset, rng_episode = jax.random.split
-(rng_input) obs, state = env.reset(rng_reset, env_params) def policy_step
-(state_input, tmp): """lax.scan compatible step transition in jax env.""" obs,
-state, policy_params, rng = state_input rng, rng_step, rng_net =
+tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07 | [`Reacher-misc`](https://
+github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/reacher.py) |
+[Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://
+github.com/unifyai/gym/blob/master/ivy_gym/reacher.py) | | [`Swimmer-misc`]
+(https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/
+swimmer.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click]
+(https://github.com/unifyai/gym/blob/master/ivy_gym/swimmer.py) | | [`Pong-
+misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/
+misc/pong.py) | [Kirsch (2018)](https://github.com/BlackHC/batch_pong_poc) |
+[Click](https://github.com/BlackHC/batch_pong_poc/blob/master/src/
+vanilla_pong.py) | \* All displayed speeds are estimated for 1M step
+transitions (random policy) on a NVIDIA A100 GPU using `jit` compiled episode
+rollouts with 2000 environment workers. For more detailed speed comparisons on
+different accelerators (CPU, RTX 2080Ti) and MLP policies, please refer to the
+[`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines) documentation.
+## Installation â³ The latest `gymnax` release can directly be installed from
+PyPI: ``` pip install gymnax ``` If you want to get the most recent commit,
+please install directly from the repository: ``` pip install git+https://
+github.com/RobertTLange/gymnax.git@main ``` In order to use JAX on your
+accelerators, you can find more details in the [JAX documentation](https://
+github.com/google/jax#installation). ## Examples ð * ð [Environment API]
+(examples/getting_started.ipynb) - Get started with the basic `gymnax` API. *
+ð [Distributed Anakin Agent](examples/01_anakin.ipynb) - Train an Anakin [
+(Hessel et al., 2021)](https://arxiv.org/pdf/2104.06272.pdf) agent on
+`SpaceInvaders-MinAtar`. * ð [ES with `gymnax`](examples/02_evolution.ipynb)
+- Meta-evolve an LSTM controller that controls 2 link pendula of different
+lengths. * ð [Bandit A2C Meta-RL](examples/03_meta_a2c.ipynb) - Meta-learn
+an A2C LSTM that learns to explore/exploit in multi-arm bandit tasks. * ð
+[Trained baselines](https://github.com/RobertTLange/gymnax-blines) - Check out
+the trained baseline agents (PPO/ES) in `gymnax-blines`. ## Key Selling Points
+ðµ - **Environment vectorization & acceleration**: Easy composition of JAX
+primitives (e.g. `jit`, `vmap`, `pmap`): ```python # Jit-accelerated step
+transition jit_step = jax.jit(env.step) # map (vmap/pmap) across random keys
+for batch rollouts reset_rng = jax.vmap(env.reset, in_axes=(0, None)) step_rng
+= jax.vmap(env.step, in_axes=(0, 0, 0, None)) # map (vmap/pmap) across env
+parameters (e.g. for meta-learning) reset_params = jax.vmap(env.reset, in_axes=
+(None, 0)) step_params = jax.vmap(env.step, in_axes=(None, 0, 0, 0)) ``` For
+speed comparisons with standard vectorized NumPy environments check out
+[`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines). - **Scan
+through entire episode rollouts**: You can also `lax.scan` through entire
+`reset`, `step` episode loops for fast compilation: ```python def rollout
+(rng_input, policy_params, env_params, steps_in_episode): """Rollout a jitted
+gymnax episode with lax.scan.""" # Reset the environment rng_reset, rng_episode
+= jax.random.split(rng_input) obs, state = env.reset(rng_reset, env_params) def
+policy_step(state_input, tmp): """lax.scan compatible step transition in jax
+env.""" obs, state, policy_params, rng = state_input rng, rng_step, rng_net =
 jax.random.split(rng, 3) action = model.apply(policy_params, obs) next_obs,
 next_state, reward, done, _ = env.step( rng_step, state, action, env_params )
 carry = [next_obs, next_state, policy_params, rng] return carry, [obs, action,
 reward, next_obs, done] # Scan over episode step loop _, scan_out =
 jax.lax.scan( policy_step, [obs, state, policy_params, rng_episode], (),
 steps_in_episode ) # Return masked sum of rewards accumulated by agent in
 episode obs, action, reward, next_obs, done = scan_out return obs, action,
@@ -203,20 +214,22 @@
 policy_params ) # Multiple rollouts for different networks + rng (e.g. for ES)
 batch_params = jax.tree_map( # Stack parameters or use different lambda x:
 jnp.tile(x, (5, 1)).reshape(5, *x.shape), policy_params ) obs, action, reward,
 next_obs, done, cum_ret = manager.population_rollout( rng_batch, batch_params )
 ``` ## Resources & Other Great Tools ð * ð» [Brax](https://github.com/
 google/brax): JAX-based library for rigid body physics by Google Brain with
 JAX-style MuJoCo substitutes. * ð» [envpool](https://github.com/sail-sg/
-envpool): Vectorized parallel environment execution engine. ###
-Acknowledgements & Citing `gymnax` âï¸ If you use `gymnax` in your research,
-please cite it as follows: ``` @software{gymnax2022github, author = {Robert
-Tjarko Lange}, title = {{gymnax}: A {JAX}-based Reinforcement Learning
-Environment Library}, url = {http://github.com/RobertTLange/gymnax}, version =
-{0.0.4}, year = {2022}, } ``` We acknowledge financial support by the [Google
-TRC](https://sites.research.google/trc/about/) and the Deutsche
-Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's
-Excellence Strategy - EXC 2002/1 ["Science of Intelligence"](https://
-www.scienceofintelligence.de/) - project number 390523135. ## Development ð·
-You can run the test suite via `python -m pytest -vv --all`. If you find a bug
-or are missing your favourite feature, feel free to create an issue and/or
-start [contributing](CONTRIBUTING.md) ð¤.
+envpool): Vectorized parallel environment execution engine. * ð» [Jumaji]
+(https://github.com/instadeepai/jumanji): Industry-driven JAX-based RL
+environments. * ð» [Pgx](https://github.com/sotetsuk/pgx): JAX-based classic
+board game environments. ### Acknowledgements & Citing `gymnax` âï¸ If you
+use `gymnax` in your research, please cite it as follows: ``` @software
+{gymnax2022github, author = {Robert Tjarko Lange}, title = {{gymnax}: A {JAX}-
+based Reinforcement Learning Environment Library}, url = {http://github.com/
+RobertTLange/gymnax}, version = {0.0.4}, year = {2022}, } ``` We acknowledge
+financial support by the [Google TRC](https://sites.research.google/trc/about/
+) and the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation)
+under Germany's Excellence Strategy - EXC 2002/1 ["Science of Intelligence"]
+(https://www.scienceofintelligence.de/) - project number 390523135. ##
+Development ð· You can run the test suite via `python -m pytest -vv --all`.
+If you find a bug or are missing your favourite feature, feel free to create an
+issue and/or start [contributing](CONTRIBUTING.md) ð¤.
```

### Comparing `gymnax-0.0.5/gymnax/environments/__init__.py` & `gymnax-0.0.6/gymnax/environments/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .environment import EnvParams, EnvState
 from .classic_control import (
     Pendulum,
     CartPole,
     MountainCar,
     ContinuousMountainCar,
     Acrobot,
 )
@@ -26,18 +27,23 @@
 
 from .misc import (
     BernoulliBandit,
     GaussianBandit,
     FourRooms,
     MetaMaze,
     PointRobot,
+    Reacher,
+    Swimmer,
+    Pong,
 )
 
 
 __all__ = [
+    "EnvParams",
+    "EnvState",
     "Pendulum",
     "CartPole",
     "MountainCar",
     "ContinuousMountainCar",
     "Acrobot",
     "Catch",
     "DeepSea",
@@ -52,8 +58,11 @@
     "MinSeaquest",
     "MinSpaceInvaders",
     "BernoulliBandit",
     "GaussianBandit",
     "FourRooms",
     "MetaMaze",
     "PointRobot",
+    "Reacher",
+    "Swimmer",
+    "Pong",
 ]
```

### Comparing `gymnax-0.0.5/gymnax/environments/bsuite/bandit.py` & `gymnax-0.0.6/gymnax/environments/bsuite/bandit.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/bsuite/catch.py` & `gymnax-0.0.6/gymnax/environments/bsuite/catch.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/bsuite/deep_sea.py` & `gymnax-0.0.6/gymnax/environments/bsuite/deep_sea.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/bsuite/discounting_chain.py` & `gymnax-0.0.6/gymnax/environments/bsuite/discounting_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import jax
 import jax.numpy as jnp
 from jax import lax
 from gymnax.environments import environment, spaces
 from typing import Tuple, Optional
 import chex
 from flax import struct
 
@@ -12,15 +11,15 @@
     rewards: chex.Array
     context: int
     time: int
 
 
 @struct.dataclass
 class EnvParams:
-    reward_timestep: chex.Array = jnp.array([1, 3, 10, 30, 100])
+    reward_timestep: chex.Array
     optimal_return: float = 1.1
     max_steps_in_episode: int = 100
 
 
 class DiscountingChain(environment.Environment):
     """
     JAX Compatible version of DiscountingChain bsuite environment. Source:
@@ -28,21 +27,18 @@
     """
 
     def __init__(self, n_actions: int = 5, mapping_seed: int = 0):
         super().__init__()
         self.n_actions = n_actions
         self.mapping_seed = mapping_seed
 
-        # Setup reward fct fron mapping seed - random sampling outside of env
-        self.reward = jnp.ones(self.n_actions).at[self.mapping_seed].set(1.1)
-
     @property
     def default_params(self) -> EnvParams:
         # Default environment parameters
-        return EnvParams()
+        return EnvParams(reward_timestep=jnp.array([1, 3, 10, 30, 100]))
 
     def step_env(
         self, key: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
     ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
         """Perform single timestep state transition."""
         state = EnvState(
             state.rewards,
@@ -66,15 +62,21 @@
             info,
         )
 
     def reset_env(
         self, key: chex.PRNGKey, params: EnvParams
     ) -> Tuple[chex.Array, EnvState]:
         """Reset environment state by sampling initial position."""
-        state = EnvState(self.reward, -1, 0)
+        # Setup reward fct from mapping seed - random sampling outside of env
+        reward = (
+            jnp.ones(self.n_actions)
+            .at[self.mapping_seed]
+            .set(params.optimal_return)
+        )
+        state = EnvState(reward, -1, 0)
         return self.get_obs(state, params), state
 
     def get_obs(self, state: EnvState, params: EnvParams) -> chex.Array:
         """Return observation from raw state trafo."""
         obs = jnp.zeros(shape=(2,), dtype=jnp.float32)
         obs = obs.at[0].set(state.context)
         obs = obs.at[1].set(
@@ -108,15 +110,18 @@
         return spaces.Box(-1, self.n_actions, (2,), dtype=jnp.float32)
 
     def state_space(self, params: EnvParams) -> spaces.Dict:
         """State space of the environment."""
         return spaces.Dict(
             {
                 "rewards": spaces.Box(
-                    1, 1.1, (self.n_actions,), dtype=jnp.float32
+                    1,
+                    params.optimal_return,
+                    (self.n_actions,),
+                    dtype=jnp.float32,
                 ),
                 "context": spaces.Box(
                     -1, self.n_actions, (), dtype=jnp.float32
                 ),
                 "time": spaces.Discrete(params.max_steps_in_episode),
             }
         )
```

### Comparing `gymnax-0.0.5/gymnax/environments/bsuite/memory_chain.py` & `gymnax-0.0.6/gymnax/environments/bsuite/memory_chain.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/bsuite/mnist.py` & `gymnax-0.0.6/gymnax/environments/bsuite/mnist.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/bsuite/umbrella_chain.py` & `gymnax-0.0.6/gymnax/environments/bsuite/umbrella_chain.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/classic_control/acrobot.py` & `gymnax-0.0.6/gymnax/environments/classic_control/acrobot.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     JAX Compatible version of Acrobot-v1 OpenAI gym environment. Source:
     github.com/openai/gym/blob/master/gym/envs/classic_control/acrobot.py
     Note that we only implement the default 'book' version.
     """
 
     def __init__(self):
         super().__init__()
+        self.obs_shape = (6,)
 
     @property
     def default_params(self) -> EnvParams:
         # Default environment parameters
         return EnvParams(available_torque=jnp.array([-1.0, 0.0, +1.0]))
 
     def step_env(
@@ -231,20 +232,20 @@
     ddtheta1 = -(d2 * ddtheta2 + phi1) / d1
     return jnp.array([dtheta1, dtheta2, ddtheta1, ddtheta2, 0.0])
 
 
 def wrap(x: float, m: float, M: float) -> float:
     """For example, m = -180, M = 180 (degrees), x = 360 --> returns 0."""
     diff = M - m
-    diff_x_M = x - M
-    diff_x_m = x - m
-    go_down = diff_x_M > 0
-    go_up = diff_x_m < 0
+    go_up = x < m     # Wrap if x is outside the left bound
+    go_down = x >= M  # Wrap if x is outside OR on the right bound
+
     how_often = (
-        jnp.ceil(diff_x_M / diff) * go_down + jnp.ceil(diff_x_m / diff) * go_up
+        go_up * jnp.ceil((m - x) / diff)           # if m - x is an integer, keep it
+        + go_down * jnp.floor((x - M) / diff + 1)  # if x - M is an integer, round up
     )
     x_out = x - how_often * diff * go_down + how_often * diff * go_up
     return x_out
 
 
 def rk4(y0: chex.Array, params: EnvParams):
     """Runge-Kutta integration of ODE - Difference to OpenAI: Only 1 step!"""
```

### Comparing `gymnax-0.0.5/gymnax/environments/classic_control/cartpole.py` & `gymnax-0.0.6/gymnax/environments/classic_control/cartpole.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     """
     JAX Compatible version of CartPole-v1 OpenAI gym environment. Source:
     github.com/openai/gym/blob/master/gym/envs/classic_control/cartpole.py
     """
 
     def __init__(self):
         super().__init__()
+        self.obs_shape = (4,)
 
     @property
     def default_params(self) -> EnvParams:
         # Default environment parameters for CartPole-v1
         return EnvParams()
 
     def step_env(
```

### Comparing `gymnax-0.0.5/gymnax/environments/classic_control/continuous_mountain_car.py` & `gymnax-0.0.6/gymnax/environments/classic_control/continuous_mountain_car.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             1 - (position >= params.goal_position) * (velocity < 0)
         )
 
         reward = -0.1 * action ** 2 + 100 * (
             (position >= params.goal_position)
             * (velocity >= params.goal_velocity)
         )
+        reward = reward.squeeze()
 
         # Update state dict and evaluate termination conditions
         state = EnvState(position.squeeze(), velocity.squeeze(), state.time + 1)
         done = self.is_terminal(state, params)
         return (
             lax.stop_gradient(self.get_obs(state)),
             lax.stop_gradient(state),
```

### Comparing `gymnax-0.0.5/gymnax/environments/classic_control/mountain_car.py` & `gymnax-0.0.6/gymnax/environments/classic_control/mountain_car.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/classic_control/pendulum.py` & `gymnax-0.0.6/gymnax/environments/classic_control/pendulum.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
     JAX Compatible version of Pendulum-v0 OpenAI gym environment. Source:
     github.com/openai/gym/blob/master/gym/envs/classic_control/pendulum.py
     """
 
     def __init__(self):
         super().__init__()
+        self.obs_shape = (3,)
 
     @property
     def default_params(self) -> EnvParams:
         """Default environment parameters for Pendulum-v0."""
         return EnvParams()
 
     def step_env(
@@ -50,14 +51,15 @@
         """Integrate pendulum ODE and return transition."""
         u = jnp.clip(action, -params.max_torque, params.max_torque)
         reward = -(
             angle_normalize(state.theta) ** 2
             + 0.1 * state.theta_dot ** 2
             + 0.001 * (u ** 2)
         )
+        reward = reward.squeeze()
 
         newthdot = state.theta_dot + (
             (
                 3 * params.g / (2 * params.l) * jnp.sin(state.theta)
                 + 3.0 / (params.m * params.l ** 2) * u
             )
             * params.dt
```

### Comparing `gymnax-0.0.5/gymnax/environments/environment.py` & `gymnax-0.0.6/gymnax/environments/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     @partial(jax.jit, static_argnums=(0,))
     def step(
         self,
         key: chex.PRNGKey,
         state: EnvState,
         action: Union[int, float],
         params: Optional[EnvParams] = None,
-    ) -> Tuple[chex.Array, EnvState, float, bool]:
+    ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
         """Performs step transitions in the environment."""
         # Use default env parameters if no others specified
         if params is None:
             params = self.default_params
         key, key_reset = jax.random.split(key)
         obs_st, state_st, reward, done, info = self.step_env(
             key, state, action, params
```

### Comparing `gymnax-0.0.5/gymnax/environments/minatar/asterix.py` & `gymnax-0.0.6/gymnax/environments/minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/minatar/breakout.py` & `gymnax-0.0.6/gymnax/environments/minatar/breakout.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/minatar/freeway.py` & `gymnax-0.0.6/gymnax/environments/minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/minatar/seaquest.py` & `gymnax-0.0.6/gymnax/environments/minatar/seaquest.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         + (action == 4) * jnp.minimum(8, state["sub_y"] + 1)
         + not_u_or_d * state["sub_y"]
     )
 
     # Update friendly bullets based on f action and shot_timer
     bullet_cond = jnp.logical_and(action == 5, state["shot_timer"] == 0)
     state["shot_timer"] = lax.select(
-        bullet_cond, env_params["shot_cool_down"], state["shot_timer"]
+        bullet_cond, env_params.shot_cool_down, state["shot_timer"]
     )
     bullet_array = jnp.array([state["sub_x"], state["sub_y"], state["sub_or"]])
     # Use counter to keep track of row idx to update!
     f_bullets_add = jax.ops.index_update(
         state["f_bullets"], jax.ops.index[state["f_bullet_count"]], bullet_array
     )
     state["f_bullets"] = lax.select(
```

### Comparing `gymnax-0.0.5/gymnax/environments/minatar/space_invaders.py` & `gymnax-0.0.6/gymnax/environments/minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/misc/bernoulli_bandit.py` & `gymnax-0.0.6/gymnax/environments/misc/bernoulli_bandit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from typing import Optional, Tuple
+
+import chex
 import jax
 import jax.numpy as jnp
+from flax import struct
 from jax import lax
+
 from gymnax.environments import environment, spaces
-from typing import Tuple, Optional
-import chex
-from flax import struct
 
 
 @struct.dataclass
 class EnvState:
     last_action: int
     last_reward: int
     exp_reward_best: float
@@ -16,15 +18,18 @@
     time: float
 
 
 @struct.dataclass
 class EnvParams:
     reward_prob: float = 0.1
     normalize_time: bool = True
-    max_steps_in_episode: int = 100
+    max_steps_in_episode: float = 100.0
+    min_lim: float = -1.0
+    max_lim: float = 1.0
+    t_max: int = 100
 
 
 class BernoulliBandit(environment.Environment):
     """
     JAX version of a Bernoulli bandit environment as in Wang et al. 2017
     """
 
@@ -79,15 +84,19 @@
         )
         return self.get_obs(state, params), state
 
     def get_obs(self, state: EnvState, params: EnvParams) -> chex.Array:
         """Concatenate reward, one-hot action and time stamp."""
         action_one_hot = jax.nn.one_hot(state.last_action, 2).squeeze()
         time_rep = jax.lax.select(
-            params.normalize_time, time_normalization(state.time), state.time
+            params.normalize_time,
+            time_normalization(
+                state.time, params.min_lim, params.max_lim, params.t_max
+            ),
+            state.time,
         )
         return jnp.hstack([state.last_reward, action_one_hot, time_rep])
 
     def is_terminal(self, state: EnvState, params: EnvParams) -> bool:
         """Check whether state is terminal."""
         # Check number of steps in episode termination condition
         done = state.time >= params.max_steps_in_episode
@@ -108,19 +117,33 @@
     ) -> spaces.Discrete:
         """Action space of the environment."""
         return spaces.Discrete(self.num_actions)
 
     def observation_space(self, params: EnvParams) -> spaces.Box:
         """Observation space of the environment."""
         low = jnp.array(
-            [0, 0, 0, 0],
+            [
+                0,
+                0,
+                0,
+                jax.lax.select(params.normalize_time, params.min_lim, 0.0),
+            ],
             dtype=jnp.float32,
         )
         high = jnp.array(
-            [self.num_actions, 1, 1, params.max_steps_in_episode],
+            [
+                self.num_actions,
+                1,
+                1,
+                jax.lax.select(
+                    params.normalize_time,
+                    params.max_lim,
+                    params.max_steps_in_episode,
+                ),
+            ],
             dtype=jnp.float32,
         )
         return spaces.Box(low, high, (4,), jnp.float32)
 
     def state_space(self, params: EnvParams) -> spaces.Dict:
         """State space of the environment."""
         return spaces.Dict(
```

### Comparing `gymnax-0.0.5/gymnax/environments/misc/gaussian_bandit.py` & `gymnax-0.0.6/gymnax/environments/misc/gaussian_bandit.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/misc/meta_maze.py` & `gymnax-0.0.6/gymnax/environments/misc/meta_maze.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/misc/point_robot.py` & `gymnax-0.0.6/gymnax/environments/misc/point_robot.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/environments/misc/rooms.py` & `gymnax-0.0.6/gymnax/environments/misc/rooms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import jax
 import jax.numpy as jnp
 from jax import lax
 from gymnax.environments import environment, spaces
-from typing import Tuple, Optional
+from typing import Tuple, Optional, List
 import chex
 from flax import struct
 
 
 @struct.dataclass
 class EnvState:
     pos: chex.Array
@@ -52,16 +52,16 @@
     Source: Comparable to https://github.com/howardh/gym-fourrooms
     Since gymnax automatically resets env at done, we abstract different resets
     """
 
     def __init__(
         self,
         use_visual_obs: bool = False,
-        goal_fixed: chex.Array = jnp.array([8, 9]),
-        pos_fixed: chex.Array = jnp.array([4, 1]),
+        goal_fixed: List[int] = [8, 9],
+        pos_fixed: List[int] = [4, 1],
     ):
         super().__init__()
         self.env_map = string_to_bool_map(four_rooms_map)
         self.occupied_map = 1 - self.env_map
         coords = []
         for y in range(self.env_map.shape[0]):
             for x in range(self.env_map.shape[1]):
```

### Comparing `gymnax-0.0.5/gymnax/environments/spaces.py` & `gymnax-0.0.6/gymnax/environments/spaces.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-from typing import Tuple, Union
+from typing import Tuple, Sequence, Any, Dict
 from collections import OrderedDict
 import chex
 import jax
 import jax.numpy as jnp
+import numpy as np
+from gym import spaces as gspc
 
 
-# TODO: Add abstract class for general space (2 methods - sample, contains)
+class Space:
+    """
+    Minimal jittable class for abstract gymnax space.
+    """
+
+    def sample(self, rng: chex.PRNGKey) -> chex.Array:
+        raise NotImplementedError
+
+    def contains(self, x: jnp.int_) -> bool:
+        raise NotImplementedError
 
 
-class Discrete(object):
+class Discrete(Space):
     """
     Minimal jittable class for discrete gymnax spaces.
     TODO: For now this is a 1d space. Make composable for multi-discrete.
     """
 
     def __init__(self, num_categories: int):
         assert num_categories >= 0
@@ -30,15 +41,15 @@
         """Check whether specific object is within space."""
         # type_cond = isinstance(x, self.dtype)
         # shape_cond = (x.shape == self.shape)
         range_cond = jnp.logical_and(x >= 0, x < self.n)
         return range_cond
 
 
-class Box(object):
+class Box(Space):
     """
     Minimal jittable class for array-shaped gymnax spaces.
     TODO: Add unboundedness - sampling from other distributions, etc.
     """
 
     def __init__(
         self,
@@ -64,61 +75,86 @@
         # shape_cond = (x.shape == self.shape)
         range_cond = jnp.logical_and(
             jnp.all(x >= self.low), jnp.all(x <= self.high)
         )
         return range_cond
 
 
-class Dict(object):
+class Dict(Space):
     """Minimal jittable class for dictionary of simpler jittable spaces."""
 
-    def __init__(self, spaces: dict):
+    def __init__(self, spaces: Dict[Any, Space]):
         self.spaces = spaces
         self.num_spaces = len(spaces)
 
-    def sample(self, rng: chex.PRNGKey) -> dict:
+    def sample(self, rng: chex.PRNGKey) -> Dict:
         """Sample random action from all subspaces."""
         key_split = jax.random.split(rng, self.num_spaces)
         return OrderedDict(
             [
                 (k, self.spaces[k].sample(key_split[i]))
                 for i, k in enumerate(self.spaces)
             ]
         )
 
     def contains(self, x: jnp.int_) -> bool:
         """Check whether dimensions of object are within subspace."""
-        # type_cond = isinstance(x, dict)
+        # type_cond = isinstance(x, Dict)
         # num_space_cond = len(x) != len(self.spaces)
         # Check for each space individually
         out_of_space = 0
         for k, space in self.spaces.items():
             out_of_space += 1 - space.contains(getattr(x, k))
         return out_of_space == 0
 
 
-class Tuple(object):
+class Tuple(Space):
     """Minimal jittable class for tuple (product) of jittable spaces."""
 
-    def __init__(self, spaces: Union[tuple, list]):
+    def __init__(self, spaces: Sequence[Space]):
         self.spaces = spaces
         self.num_spaces = len(spaces)
 
     def sample(self, rng: chex.PRNGKey) -> Tuple[chex.Array]:
         """Sample random action from all subspaces."""
         key_split = jax.random.split(rng, self.num_spaces)
         return tuple(
-            [
-                self.spaces[k].sample(key_split[i])
-                for i, k in enumerate(self.spaces)
-            ]
+            [s.sample(key_split[i]) for i, s in enumerate(self.spaces)]
         )
 
     def contains(self, x: jnp.int_) -> bool:
         """Check whether dimensions of object are within subspace."""
         # type_cond = isinstance(x, tuple)
         # num_space_cond = len(x) != len(self.spaces)
         # Check for each space individually
         out_of_space = 0
-        for space in self.spaces:
-            out_of_space += 1 - space.contains(x)
+        for i, space in enumerate(self.spaces):
+            out_of_space += 1 - space.contains(x[i])
         return out_of_space == 0
+
+
+def gymnax_space_to_gym_space(space: Space) -> gspc.Space:
+    """Convert Gymnax space to equivalent Gym space"""
+    if isinstance(space, Discrete):
+        return gspc.Discrete(space.n)
+    elif isinstance(space, Box):
+        low = (
+            float(space.low)
+            if (np.isscalar(space.low) or space.low.size == 1)
+            else np.array(space.low)
+        )
+        high = (
+            float(space.high)
+            if (np.isscalar(space.high) or space.low.size == 1)
+            else np.array(space.high)
+        )
+        return gspc.Box(low, high, space.shape, space.dtype)
+    elif isinstance(space, Dict):
+        return gspc.Dict(
+            {k: gymnax_space_to_gym_space(v) for k, v in space.spaces}
+        )
+    elif isinstance(space, Tuple):
+        return gspc.Tuple(space.spaces)
+    else:
+        raise NotImplementedError(
+            f"Conversion of {space.__class__.__name__} not supported"
+        )
```

### Comparing `gymnax-0.0.5/gymnax/experimental/rollout.py` & `gymnax-0.0.6/gymnax/experimental/rollout.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/registration.py` & `gymnax-0.0.6/gymnax/registration.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     MinSeaquest,
     MinSpaceInvaders,
     BernoulliBandit,
     GaussianBandit,
     FourRooms,
     MetaMaze,
     PointRobot,
+    Reacher,
+    Swimmer,
+    Pong,
 )
 
 # =============================================================================
 
 
 def make(env_id: str, **env_kwargs):
     """A JAX-version of OpenAI's infamous env.make(env_name)"""
@@ -63,14 +66,15 @@
     elif env_id == "Asterix-MinAtar":
         env = MinAsterix(**env_kwargs)
     elif env_id == "Breakout-MinAtar":
         env = MinBreakout(**env_kwargs)
     elif env_id == "Freeway-MinAtar":
         env = MinFreeway(**env_kwargs)
     elif env_id == "Seaquest-MinAtar":
+        raise NotImplementedError("Seaquest is not yet supported.")
         env = MinSeaquest(**env_kwargs)
     elif env_id == "SpaceInvaders-MinAtar":
         env = MinSpaceInvaders(**env_kwargs)
 
     # 4. Miscellanoues Environments
     elif env_id == "BernoulliBandit-misc":
         env = BernoulliBandit(**env_kwargs)
@@ -78,14 +82,20 @@
         env = GaussianBandit(**env_kwargs)
     elif env_id == "FourRooms-misc":
         env = FourRooms(**env_kwargs)
     elif env_id == "MetaMaze-misc":
         env = MetaMaze(**env_kwargs)
     elif env_id == "PointRobot-misc":
         env = PointRobot(**env_kwargs)
+    elif env_id == "Reacher-misc":
+        env = Reacher(**env_kwargs)
+    elif env_id == "Swimmer-misc":
+        env = Swimmer(**env_kwargs)
+    elif env_id == "Pong-misc":
+        env = Pong(**env_kwargs)
     else:
         raise ValueError("Environment ID is not registered.")
 
     # Create a jax PRNG key for random seed control
     return env, env.default_params
 
 
@@ -94,21 +104,25 @@
     "Pendulum-v1",
     "Acrobot-v1",
     "MountainCar-v0",
     "MountainCarContinuous-v0",
     "Asterix-MinAtar",
     "Breakout-MinAtar",
     "Freeway-MinAtar",
+    # "Seaquest-MinAtar",
     "SpaceInvaders-MinAtar",
     "Catch-bsuite",
     "DeepSea-bsuite",
     "MemoryChain-bsuite",
     "UmbrellaChain-bsuite",
     "DiscountingChain-bsuite",
     "MNISTBandit-bsuite",
     "SimpleBandit-bsuite",
     "FourRooms-misc",
     "MetaMaze-misc",
     "PointRobot-misc",
     "BernoulliBandit-misc",
     "GaussianBandit-misc",
+    "Reacher-misc",
+    "Swimmer-misc",
+    "Pong-misc",
 ]
```

### Comparing `gymnax-0.0.5/gymnax/utils/load_mnist.py` & `gymnax-0.0.6/gymnax/utils/load_mnist.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/utils/state_translate.py` & `gymnax-0.0.6/gymnax/utils/state_translate.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/utils/test_helpers.py` & `gymnax-0.0.6/gymnax/utils/test_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,32 @@
     for k in state_gym.keys():
         jax_value = getattr(state_jax, k)
         # print(k, jax_value, state_gym[k])
         if k not in ["time", "terminal"]:
             if type(jax_value) in [
                 jax.interpreters.xla._DeviceArray,
                 jaxlib.xla_extension.Buffer,
+                jaxlib.xla_extension.ArrayImpl,
                 np.ndarray,
             ]:
                 assert np.allclose(jax_value, state_gym[k], atol=atol)
             else:
                 # print(k, state_gym[k], state_jax[k])
                 # Exclude extra time and terminal state from assertion
-                if type(state_gym[k]) in [float, np.float64]:
+                if type(state_gym[k]) in [
+                    float,
+                    np.float64,
+                    jax.interpreters.xla._DeviceArray,
+                    jaxlib.xla_extension.Buffer,
+                    np.ndarray,
+                    jaxlib.xla_extension.ArrayImpl,
+                ]:
                     np.allclose(state_gym[k], jax_value, atol=atol)
                 else:
+                    print(type(state_gym[k]), k)
                     assert state_gym[k] == jax_value
 
 
 def assert_correct_transit(
     obs_gym,
     reward_gym,
     done_gym,
```

### Comparing `gymnax-0.0.5/gymnax/visualize/vis_catch.py` & `gymnax-0.0.6/gymnax/visualize/vis_catch.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/visualize/vis_circle.py` & `gymnax-0.0.6/gymnax/visualize/vis_circle.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/visualize/vis_gym.py` & `gymnax-0.0.6/gymnax/visualize/vis_gym.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/visualize/vis_maze.py` & `gymnax-0.0.6/gymnax/visualize/vis_maze.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/visualize/vis_minatar.py` & `gymnax-0.0.6/gymnax/visualize/vis_minatar.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.5/gymnax/visualize/visualizer.py` & `gymnax-0.0.6/gymnax/visualize/visualizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
 from typing import Optional
-from .vis_gym import init_gym, update_gym
-from .vis_minatar import init_minatar, update_minatar
-from .vis_circle import init_circle, update_circle
-from .vis_maze import init_maze, update_maze
-from .vis_catch import init_catch, update_catch
+from gymnax.visualize.vis_gym import init_gym, update_gym
+from gymnax.visualize.vis_minatar import init_minatar, update_minatar
+from gymnax.visualize.vis_circle import init_circle, update_circle
+from gymnax.visualize.vis_maze import init_maze, update_maze
+from gymnax.visualize.vis_catch import init_catch, update_catch
 
 
 class Visualizer(object):
     def __init__(self, env, env_params, state_seq, reward_seq=None):
         self.env = env
         self.env_params = env_params
         self.state_seq = state_seq
@@ -71,14 +71,15 @@
             )
         elif self.env.name in [
             "Asterix-MinAtar",
             "Breakout-MinAtar",
             "Freeway-MinAtar",
             "Seaquest-MinAtar",
             "SpaceInvaders-MinAtar",
+            "Pong-misc",
         ]:
             self.im = init_minatar(self.ax, self.env, self.state_seq[0])
         elif self.env.name == "PointRobot-misc":
             self.im = init_circle(
                 self.ax, self.env, self.state_seq[0], self.env_params
             )
         elif self.env.name in ["MetaMaze-misc", "FourRooms-misc"]:
@@ -100,14 +101,15 @@
             self.im = update_catch(self.im, self.env, self.state_seq[frame])
         elif self.env.name in [
             "Asterix-MinAtar",
             "Breakout-MinAtar",
             "Freeway-MinAtar",
             "Seaquest-MinAtar",
             "SpaceInvaders-MinAtar",
+            "Pong-misc",
         ]:
             update_minatar(self.im, self.env, self.state_seq[frame])
         elif self.env.name == "PointRobot-misc":
             self.im = update_circle(self.im, self.env, self.state_seq[frame])
         elif self.env.name in ["MetaMaze-misc", "FourRooms-misc"]:
             self.im = update_maze(self.im, self.env, self.state_seq[frame])
 
@@ -118,7 +120,37 @@
         else:
             self.ax.set_title(
                 "{}: Step {:4.0f} - Return {:7.2f}".format(
                     self.env.name, frame + 1, self.reward_seq[frame]
                 ),
                 fontsize=15,
             )
+
+
+if __name__ == "__main__":
+    import jax
+    import jax.numpy as jnp
+    import gymnax
+
+    rng = jax.random.PRNGKey(0)
+    env, env_params = gymnax.make("Pong-misc")
+
+    state_seq, reward_seq = [], []
+    rng, rng_reset = jax.random.split(rng)
+    obs, env_state = env.reset(rng_reset, env_params)
+    while True:
+        state_seq.append(env_state)
+        rng, rng_act, rng_step = jax.random.split(rng, 3)
+        action = env.action_space(env_params).sample(rng_act)
+        next_obs, next_env_state, reward, done, info = env.step(
+            rng_step, env_state, action, env_params
+        )
+        reward_seq.append(reward)
+        if done:
+            break
+        else:
+            obs = next_obs
+            env_state = next_env_state
+
+    cum_rewards = jnp.cumsum(jnp.array(reward_seq))
+    vis = Visualizer(env, env_params, state_seq, cum_rewards)
+    vis.animate(f"anim.gif")
```

### Comparing `gymnax-0.0.5/gymnax.egg-info/PKG-INFO` & `gymnax-0.0.6/gymnax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gymnax
-Version: 0.0.5
+Version: 0.0.6
 Summary: JAX-compatible version of Open AI's gym environments
 Home-page: https://github.com/RobertTLange/gymnax
-Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.5.tar.gz
+Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.6.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -85,14 +85,17 @@
 | [`SimpleBandit-bsuite`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/bsuite/bandit.py) | [Osband et al. (2019)](https://openreview.net/forum?id=rygf-kSYwH) | [Click](https://github.com/deepmind/bsuite/blob/master/bsuite/environments/bandit.py)  | - | -
 |  |  |  |  | 
 | [`FourRooms-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/rooms.py) | [Sutton et al. (1999)](https://people.cs.umass.edu/~barto/courses/cs687/Sutton-Precup-Singh-AIJ99.pdf) | [Click](https://github.com/howardh/gym-fourrooms) | [PPO, ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/FourRooms-misc) (R: 1) | 0.07
 | [`MetaMaze-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/meta_maze.py) | [Micconi et al. (2020)](https://arxiv.org/abs/2002.10585)  | [Click](https://github.com/uber-research/backpropamine/blob/master/simplemaze/maze.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/MetaMaze-misc) (R: 32) | 0.09
 | [`PointRobot-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/point_robot.py) | [Dorfman et al. (2021)](https://openreview.net/pdf?id=IBdEfhLveS) | [Click](https://github.com/Rondorf/BOReL/blob/main/environments/toy_navigation/point_robot.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/PointRobot-misc) (R: 10) | 0.08
 | [`BernoulliBandit-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/bernoulli_bandit.py) | [Wang et al. (2017)](https://arxiv.org/abs/1611.05763) | [Click](https://github.com/RobertTLange/minimal-meta-rl/blob/main/bandits/bandit_env.py) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/BernoulliBandit-misc) (R: 90) | 0.08
 | [`GaussianBandit-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/gaussian_bandit.py) | [Lange & Sprekeler (2022)](https://arxiv.org/abs/2010.04466) | [Click](https://github.com/RobertTLange/learning-not-to-learn) | [ES](https://github.com/RobertTLange/gymnax-blines/tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07
+| [`Reacher-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/reacher.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://github.com/unifyai/gym/blob/master/ivy_gym/reacher.py) | 
+| [`Swimmer-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/swimmer.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://github.com/unifyai/gym/blob/master/ivy_gym/swimmer.py) |
+| [`Pong-misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/pong.py) | [Kirsch (2018)](https://github.com/BlackHC/batch_pong_poc) | [Click](https://github.com/BlackHC/batch_pong_poc/blob/master/src/vanilla_pong.py) |  
 
 \* All displayed speeds are estimated for 1M step transitions (random policy) on a NVIDIA A100 GPU using `jit` compiled episode rollouts with 2000 environment workers. For more detailed speed comparisons on different accelerators (CPU, RTX 2080Ti) and MLP policies, please refer to the [`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines) documentation.
 
 
 ## Installation ⏳
 
 The latest `gymnax` release can directly be installed from PyPI:
@@ -109,14 +112,15 @@
 
 In order to use JAX on your accelerators, you can find more details in the [JAX documentation](https://github.com/google/jax#installation).
 
 ## Examples 📖
 * 📓 [Environment API](examples/getting_started.ipynb) - Get started with the basic `gymnax` API.
 * 📓 [Distributed Anakin Agent](examples/01_anakin.ipynb) - Train an Anakin [(Hessel et al., 2021)](https://arxiv.org/pdf/2104.06272.pdf) agent on `SpaceInvaders-MinAtar`.
 * 📓 [ES with `gymnax`](examples/02_evolution.ipynb) - Meta-evolve an LSTM controller that controls 2 link pendula of different lengths.
+* 📓 [Bandit A2C Meta-RL](examples/03_meta_a2c.ipynb) - Meta-learn an A2C LSTM that learns to explore/exploit in multi-arm bandit tasks.
 * 📓 [Trained baselines](https://github.com/RobertTLange/gymnax-blines) - Check out the trained baseline agents (PPO/ES) in `gymnax-blines`.
 
 ## Key Selling Points 💵
 
 - **Environment vectorization & acceleration**: Easy composition of JAX primitives (e.g. `jit`, `vmap`, `pmap`):
 
   ```python
@@ -217,15 +221,16 @@
       rng_batch, batch_params
   )
   ```
 
 ## Resources & Other Great Tools 📝
 * 💻 [Brax](https://github.com/google/brax): JAX-based library for rigid body physics by Google Brain with JAX-style MuJoCo substitutes.
 * 💻 [envpool](https://github.com/sail-sg/envpool): Vectorized parallel environment execution engine.
-
+* 💻 [Jumaji](https://github.com/instadeepai/jumanji): Industry-driven JAX-based RL environments.
+* 💻 [Pgx](https://github.com/sotetsuk/pgx): JAX-based classic board game environments.
 
 ### Acknowledgements & Citing `gymnax` ✏️
 
 If you use `gymnax` in your research, please cite it as follows:
 
 ```
 @software{gymnax2022github,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: gymnax Version: 0.0.5 Summary: JAX-compatible
+Metadata-Version: 2.1 Name: gymnax Version: 0.0.6 Summary: JAX-compatible
 version of Open AI's gym environments Home-page: https://github.com/
 RobertTLange/gymnax Download-URL: https://github.com/RobertTLange/gymnax/
-archive/v0.0.5.tar.gz Author: Robert Tjarko Lange Author-email:
+archive/v0.0.6.tar.gz Author: Robert Tjarko Lange Author-email:
 robertlange0@gmail.com Platform: any Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
         ****** [https://github.com/RobertTLange/gymnax/blob/main/docs/
@@ -142,49 +142,60 @@
 (https://arxiv.org/abs/1611.05763) | [Click](https://github.com/RobertTLange/
 minimal-meta-rl/blob/main/bandits/bandit_env.py) | [ES](https://github.com/
 RobertTLange/gymnax-blines/tree/main/agents/BernoulliBandit-misc) (R: 90) |
 0.08 | [`GaussianBandit-misc`](https://github.com/RobertTLange/gymnax/blob/
 main/gymnax/environments/misc/gaussian_bandit.py) | [Lange & Sprekeler (2022)]
 (https://arxiv.org/abs/2010.04466) | [Click](https://github.com/RobertTLange/
 learning-not-to-learn) | [ES](https://github.com/RobertTLange/gymnax-blines/
-tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07 \* All displayed speeds are
-estimated for 1M step transitions (random policy) on a NVIDIA A100 GPU using
-`jit` compiled episode rollouts with 2000 environment workers. For more
-detailed speed comparisons on different accelerators (CPU, RTX 2080Ti) and MLP
-policies, please refer to the [`gymnax-blines`](https://github.com/
-RobertTLange/gymnax-blines) documentation. ## Installation â³ The latest
-`gymnax` release can directly be installed from PyPI: ``` pip install gymnax
-``` If you want to get the most recent commit, please install directly from the
-repository: ``` pip install git+https://github.com/RobertTLange/gymnax.git@main
-``` In order to use JAX on your accelerators, you can find more details in the
-[JAX documentation](https://github.com/google/jax#installation). ## Examples
-ð * ð [Environment API](examples/getting_started.ipynb) - Get started
-with the basic `gymnax` API. * ð [Distributed Anakin Agent](examples/
-01_anakin.ipynb) - Train an Anakin [(Hessel et al., 2021)](https://arxiv.org/
-pdf/2104.06272.pdf) agent on `SpaceInvaders-MinAtar`. * ð [ES with `gymnax`]
-(examples/02_evolution.ipynb) - Meta-evolve an LSTM controller that controls 2
-link pendula of different lengths. * ð [Trained baselines](https://
-github.com/RobertTLange/gymnax-blines) - Check out the trained baseline agents
-(PPO/ES) in `gymnax-blines`. ## Key Selling Points ðµ - **Environment
-vectorization & acceleration**: Easy composition of JAX primitives (e.g. `jit`,
-`vmap`, `pmap`): ```python # Jit-accelerated step transition jit_step = jax.jit
-(env.step) # map (vmap/pmap) across random keys for batch rollouts reset_rng =
-jax.vmap(env.reset, in_axes=(0, None)) step_rng = jax.vmap(env.step, in_axes=
-(0, 0, 0, None)) # map (vmap/pmap) across env parameters (e.g. for meta-
-learning) reset_params = jax.vmap(env.reset, in_axes=(None, 0)) step_params =
-jax.vmap(env.step, in_axes=(None, 0, 0, 0)) ``` For speed comparisons with
-standard vectorized NumPy environments check out [`gymnax-blines`](https://
-github.com/RobertTLange/gymnax-blines). - **Scan through entire episode
-rollouts**: You can also `lax.scan` through entire `reset`, `step` episode
-loops for fast compilation: ```python def rollout(rng_input, policy_params,
-env_params, steps_in_episode): """Rollout a jitted gymnax episode with
-lax.scan.""" # Reset the environment rng_reset, rng_episode = jax.random.split
-(rng_input) obs, state = env.reset(rng_reset, env_params) def policy_step
-(state_input, tmp): """lax.scan compatible step transition in jax env.""" obs,
-state, policy_params, rng = state_input rng, rng_step, rng_net =
+tree/main/agents/GaussianBandit-misc) (R: 0) | 0.07 | [`Reacher-misc`](https://
+github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/reacher.py) |
+[Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click](https://
+github.com/unifyai/gym/blob/master/ivy_gym/reacher.py) | | [`Swimmer-misc`]
+(https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/misc/
+swimmer.py) | [Lenton et al. (2021)](https://github.com/unifyai/gym/) | [Click]
+(https://github.com/unifyai/gym/blob/master/ivy_gym/swimmer.py) | | [`Pong-
+misc`](https://github.com/RobertTLange/gymnax/blob/main/gymnax/environments/
+misc/pong.py) | [Kirsch (2018)](https://github.com/BlackHC/batch_pong_poc) |
+[Click](https://github.com/BlackHC/batch_pong_poc/blob/master/src/
+vanilla_pong.py) | \* All displayed speeds are estimated for 1M step
+transitions (random policy) on a NVIDIA A100 GPU using `jit` compiled episode
+rollouts with 2000 environment workers. For more detailed speed comparisons on
+different accelerators (CPU, RTX 2080Ti) and MLP policies, please refer to the
+[`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines) documentation.
+## Installation â³ The latest `gymnax` release can directly be installed from
+PyPI: ``` pip install gymnax ``` If you want to get the most recent commit,
+please install directly from the repository: ``` pip install git+https://
+github.com/RobertTLange/gymnax.git@main ``` In order to use JAX on your
+accelerators, you can find more details in the [JAX documentation](https://
+github.com/google/jax#installation). ## Examples ð * ð [Environment API]
+(examples/getting_started.ipynb) - Get started with the basic `gymnax` API. *
+ð [Distributed Anakin Agent](examples/01_anakin.ipynb) - Train an Anakin [
+(Hessel et al., 2021)](https://arxiv.org/pdf/2104.06272.pdf) agent on
+`SpaceInvaders-MinAtar`. * ð [ES with `gymnax`](examples/02_evolution.ipynb)
+- Meta-evolve an LSTM controller that controls 2 link pendula of different
+lengths. * ð [Bandit A2C Meta-RL](examples/03_meta_a2c.ipynb) - Meta-learn
+an A2C LSTM that learns to explore/exploit in multi-arm bandit tasks. * ð
+[Trained baselines](https://github.com/RobertTLange/gymnax-blines) - Check out
+the trained baseline agents (PPO/ES) in `gymnax-blines`. ## Key Selling Points
+ðµ - **Environment vectorization & acceleration**: Easy composition of JAX
+primitives (e.g. `jit`, `vmap`, `pmap`): ```python # Jit-accelerated step
+transition jit_step = jax.jit(env.step) # map (vmap/pmap) across random keys
+for batch rollouts reset_rng = jax.vmap(env.reset, in_axes=(0, None)) step_rng
+= jax.vmap(env.step, in_axes=(0, 0, 0, None)) # map (vmap/pmap) across env
+parameters (e.g. for meta-learning) reset_params = jax.vmap(env.reset, in_axes=
+(None, 0)) step_params = jax.vmap(env.step, in_axes=(None, 0, 0, 0)) ``` For
+speed comparisons with standard vectorized NumPy environments check out
+[`gymnax-blines`](https://github.com/RobertTLange/gymnax-blines). - **Scan
+through entire episode rollouts**: You can also `lax.scan` through entire
+`reset`, `step` episode loops for fast compilation: ```python def rollout
+(rng_input, policy_params, env_params, steps_in_episode): """Rollout a jitted
+gymnax episode with lax.scan.""" # Reset the environment rng_reset, rng_episode
+= jax.random.split(rng_input) obs, state = env.reset(rng_reset, env_params) def
+policy_step(state_input, tmp): """lax.scan compatible step transition in jax
+env.""" obs, state, policy_params, rng = state_input rng, rng_step, rng_net =
 jax.random.split(rng, 3) action = model.apply(policy_params, obs) next_obs,
 next_state, reward, done, _ = env.step( rng_step, state, action, env_params )
 carry = [next_obs, next_state, policy_params, rng] return carry, [obs, action,
 reward, next_obs, done] # Scan over episode step loop _, scan_out =
 jax.lax.scan( policy_step, [obs, state, policy_params, rng_episode], (),
 steps_in_episode ) # Return masked sum of rewards accumulated by agent in
 episode obs, action, reward, next_obs, done = scan_out return obs, action,
@@ -213,20 +224,22 @@
 policy_params ) # Multiple rollouts for different networks + rng (e.g. for ES)
 batch_params = jax.tree_map( # Stack parameters or use different lambda x:
 jnp.tile(x, (5, 1)).reshape(5, *x.shape), policy_params ) obs, action, reward,
 next_obs, done, cum_ret = manager.population_rollout( rng_batch, batch_params )
 ``` ## Resources & Other Great Tools ð * ð» [Brax](https://github.com/
 google/brax): JAX-based library for rigid body physics by Google Brain with
 JAX-style MuJoCo substitutes. * ð» [envpool](https://github.com/sail-sg/
-envpool): Vectorized parallel environment execution engine. ###
-Acknowledgements & Citing `gymnax` âï¸ If you use `gymnax` in your research,
-please cite it as follows: ``` @software{gymnax2022github, author = {Robert
-Tjarko Lange}, title = {{gymnax}: A {JAX}-based Reinforcement Learning
-Environment Library}, url = {http://github.com/RobertTLange/gymnax}, version =
-{0.0.4}, year = {2022}, } ``` We acknowledge financial support by the [Google
-TRC](https://sites.research.google/trc/about/) and the Deutsche
-Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's
-Excellence Strategy - EXC 2002/1 ["Science of Intelligence"](https://
-www.scienceofintelligence.de/) - project number 390523135. ## Development ð·
-You can run the test suite via `python -m pytest -vv --all`. If you find a bug
-or are missing your favourite feature, feel free to create an issue and/or
-start [contributing](CONTRIBUTING.md) ð¤.
+envpool): Vectorized parallel environment execution engine. * ð» [Jumaji]
+(https://github.com/instadeepai/jumanji): Industry-driven JAX-based RL
+environments. * ð» [Pgx](https://github.com/sotetsuk/pgx): JAX-based classic
+board game environments. ### Acknowledgements & Citing `gymnax` âï¸ If you
+use `gymnax` in your research, please cite it as follows: ``` @software
+{gymnax2022github, author = {Robert Tjarko Lange}, title = {{gymnax}: A {JAX}-
+based Reinforcement Learning Environment Library}, url = {http://github.com/
+RobertTLange/gymnax}, version = {0.0.4}, year = {2022}, } ``` We acknowledge
+financial support by the [Google TRC](https://sites.research.google/trc/about/
+) and the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation)
+under Germany's Excellence Strategy - EXC 2002/1 ["Science of Intelligence"]
+(https://www.scienceofintelligence.de/) - project number 390523135. ##
+Development ð· You can run the test suite via `python -m pytest -vv --all`.
+If you find a bug or are missing your favourite feature, feel free to create an
+issue and/or start [contributing](CONTRIBUTING.md) ð¤.
```

### Comparing `gymnax-0.0.5/gymnax.egg-info/SOURCES.txt` & `gymnax-0.0.6/gymnax.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -34,21 +34,30 @@
 gymnax/environments/minatar/seaquest.py
 gymnax/environments/minatar/space_invaders.py
 gymnax/environments/misc/__init__.py
 gymnax/environments/misc/bernoulli_bandit.py
 gymnax/environments/misc/gaussian_bandit.py
 gymnax/environments/misc/meta_maze.py
 gymnax/environments/misc/point_robot.py
+gymnax/environments/misc/pong.py
+gymnax/environments/misc/reacher.py
 gymnax/environments/misc/rooms.py
+gymnax/environments/misc/swimmer.py
 gymnax/experimental/__init__.py
 gymnax/experimental/rollout.py
 gymnax/utils/__init__.py
 gymnax/utils/load_mnist.py
 gymnax/utils/state_translate.py
 gymnax/utils/test_helpers.py
 gymnax/visualize/__init__.py
 gymnax/visualize/vis_catch.py
 gymnax/visualize/vis_circle.py
 gymnax/visualize/vis_gym.py
 gymnax/visualize/vis_maze.py
 gymnax/visualize/vis_minatar.py
-gymnax/visualize/visualizer.py
+gymnax/visualize/visualizer.py
+gymnax/wrappers/__init__.py
+gymnax/wrappers/brax.py
+gymnax/wrappers/dm_env.py
+gymnax/wrappers/evojax.py
+gymnax/wrappers/gym.py
+gymnax/wrappers/purerl.py
```

### Comparing `gymnax-0.0.5/setup.py` & `gymnax-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     verstr = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 git_tar = f"https://github.com/RobertTLange/gymnax/archive/v{verstr}.tar.gz"
 
-requires = ["jax", "jaxlib", "chex", "flax", "pyyaml"]
-test_requires = ["gym", "bsuite"]
+requires = ["jax", "jaxlib", "chex", "flax", "pyyaml", "gym>=0.26"]
+test_requires = ["bsuite", "minatar"]
 
 setup(
     name="gymnax",
     version=verstr,
     author="Robert Tjarko Lange",
     author_email="robertlange0@gmail.com",
     description="JAX-compatible version of Open AI's gym environments",
```

