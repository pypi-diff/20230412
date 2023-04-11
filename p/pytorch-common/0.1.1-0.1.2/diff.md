# Comparing `tmp/pytorch-common-0.1.1.tar.gz` & `tmp/pytorch-common-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-common-0.1.1.tar", max compression
+gzip compressed data, was "pytorch-common-0.1.2.tar", max compression
```

## Comparing `pytorch-common-0.1.1.tar` & `pytorch-common-0.1.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     6896 2023-03-25 14:00:35.753299 pytorch-common-0.1.1/README.md
--rw-r--r--   0        0        0      668 2023-04-11 23:29:44.015706 pytorch-common-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-06 20:48:11.714056 pytorch-common-0.1.1/pytorch_common/__init__.py
--rw-r--r--   0        0        0      252 2022-02-17 01:26:29.554482 pytorch-common-0.1.1/pytorch_common/callbacks/__init__.py
--rw-r--r--   0        0        0      490 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      368 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2001 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/callback.cpython-310.pyc
--rw-r--r--   0        0        0     2088 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/callback.cpython-39.pyc
--rw-r--r--   0        0        0     1427 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/callback_manager.cpython-310.pyc
--rw-r--r--   0        0        0     1562 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/early_stop.cpython-310.pyc
--rw-r--r--   0        0        0     3978 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-310.pyc
--rw-r--r--   0        0        0     2413 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-39.pyc
--rw-r--r--   0        0        0     2011 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/save_best_model_checkpoint.cpython-310.pyc
--rw-r--r--   0        0        0     1814 2023-04-06 17:10:38.167508 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0        0        0     1682 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/validation.cpython-39.pyc
--rw-r--r--   0        0        0     1160 2022-02-18 23:40:01.317970 pytorch-common-0.1.1/pytorch_common/callbacks/callback.py
--rw-r--r--   0        0        0      807 2023-04-06 16:01:08.445308 pytorch-common-0.1.1/pytorch_common/callbacks/callback_manager.py
--rw-r--r--   0        0        0      927 2022-02-18 23:40:55.132415 pytorch-common-0.1.1/pytorch_common/callbacks/early_stop.py
--rw-r--r--   0        0        0     2674 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/callbacks/mixin/__pycache__/metric_improve_mixin.cpython-310.pyc
--rw-r--r--   0        0        0     1738 2022-02-19 21:30:07.556994 pytorch-common-0.1.1/pytorch_common/callbacks/mixin/metric_improve_mixin.py
--rw-r--r--   0        0        0      183 2022-08-13 22:39:37.132234 pytorch-common-0.1.1/pytorch_common/callbacks/output/__init__.py
--rw-r--r--   0        0        0      399 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      340 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1336 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-310.pyc
--rw-r--r--   0        0        0     1205 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-39.pyc
--rw-r--r--   0        0        0     1582 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-310.pyc
--rw-r--r--   0        0        0     1557 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-39.pyc
--rw-r--r--   0        0        0      793 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/output_hook_callback.cpython-310.pyc
--rw-r--r--   0        0        0      627 2022-02-18 22:32:24.693573 pytorch-common-0.1.1/pytorch_common/callbacks/output/logger_callback.py
--rw-r--r--   0        0        0      722 2022-02-18 23:39:18.767021 pytorch-common-0.1.1/pytorch_common/callbacks/output/output_callback.py
--rw-r--r--   0        0        0      280 2022-08-13 22:29:58.789478 pytorch-common-0.1.1/pytorch_common/callbacks/output/output_hook_callback.py
--rw-r--r--   0        0        0        2 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__init__.py
--rw-r--r--   0        0        0      190 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      814 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-310.pyc
--rw-r--r--   0        0        0      799 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-39.pyc
--rw-r--r--   0        0        0     1640 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-310.pyc
--rw-r--r--   0        0        0     1648 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-39.pyc
--rw-r--r--   0        0        0      724 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-310.pyc
--rw-r--r--   0        0        0      681 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-39.pyc
--rw-r--r--   0        0        0      259 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/metric_logger.py
--rw-r--r--   0        0        0     1045 2022-02-17 00:53:40.878623 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/metrics_plotter.py
--rw-r--r--   0        0        0      536 2023-03-25 14:13:30.104415 pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/plot.py
--rw-r--r--   0        0        0     3814 2022-02-19 21:31:03.207848 pytorch-common-0.1.1/pytorch_common/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0        0        0     1405 2022-02-19 21:30:18.417170 pytorch-common-0.1.1/pytorch_common/callbacks/save_best_model_checkpoint.py
--rw-r--r--   0        0        0     1533 2023-04-06 16:39:15.512635 pytorch-common-0.1.1/pytorch_common/callbacks/validation.py
--rw-r--r--   0        0        0      110 2022-02-17 01:32:40.208875 pytorch-common-0.1.1/pytorch_common/error/__init__.py
--rw-r--r--   0        0        0      814 2022-02-17 01:28:00.334728 pytorch-common-0.1.1/pytorch_common/error/assertions.py
--rw-r--r--   0        0        0     2432 2022-02-17 01:29:21.788291 pytorch-common-0.1.1/pytorch_common/error/checker.py
--rw-r--r--   0        0        0      273 2022-02-16 22:18:12.700000 pytorch-common-0.1.1/pytorch_common/error/common_exception.py
--rw-r--r--   0        0        0      176 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/kfoldcv/__init__.py
--rw-r--r--   0        0        0     1146 2022-01-10 22:59:53.558378 pytorch-common-0.1.1/pytorch_common/kfoldcv/k_fold_cv.py
--rw-r--r--   0        0        0        0 2022-01-09 21:00:39.557219 pytorch-common-0.1.1/pytorch_common/kfoldcv/strategy/__init__.py
--rw-r--r--   0        0        0      194 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/kfoldcv/strategy/k_fold_cv_strategy.py
--rw-r--r--   0        0        0      335 2022-01-10 22:59:53.565045 pytorch-common-0.1.1/pytorch_common/kfoldcv/strategy/non_parallel_k_fold_cv_strategy.py
--rw-r--r--   0        0        0      536 2022-01-10 22:59:53.568378 pytorch-common-0.1.1/pytorch_common/kfoldcv/strategy/parallel_k_fold_cv_strategy.py
--rw-r--r--   0        0        0      257 2023-04-06 16:00:59.165265 pytorch-common-0.1.1/pytorch_common/modules/__init__.py
--rw-r--r--   0        0        0      454 2023-04-06 16:21:38.194340 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      284 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      963 2023-04-06 16:21:38.197673 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/common_mixin.cpython-310.pyc
--rw-r--r--   0        0        0      948 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/common_mixin.cpython-39.pyc
--rw-r--r--   0        0        0     1512 2023-04-06 17:32:23.790493 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fit_context.cpython-310.pyc
--rw-r--r--   0        0        0     2020 2023-04-06 17:32:23.790493 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fit_mixin.cpython-310.pyc
--rw-r--r--   0        0        0     1651 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fit_mixin.cpython-39.pyc
--rw-r--r--   0        0        0     2534 2023-04-06 19:17:53.117811 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fn.cpython-310.pyc
--rw-r--r--   0        0        0      989 2023-04-06 17:32:23.793826 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/persistent_mixin.cpython-310.pyc
--rw-r--r--   0        0        0     1502 2023-04-06 17:32:23.793826 pytorch-common-0.1.1/pytorch_common/modules/__pycache__/predict_mixin.cpython-310.pyc
--rw-r--r--   0        0        0      382 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/modules/common_mixin.py
--rw-r--r--   0        0        0     1272 2023-04-06 17:24:42.168161 pytorch-common-0.1.1/pytorch_common/modules/fit_context.py
--rw-r--r--   0        0        0     1981 2023-04-06 17:28:37.839367 pytorch-common-0.1.1/pytorch_common/modules/fit_mixin.py
--rw-r--r--   0        0        0     2386 2023-04-06 19:17:50.767798 pytorch-common-0.1.1/pytorch_common/modules/fn.py
--rw-r--r--   0        0        0      553 2023-04-06 17:23:47.241207 pytorch-common-0.1.1/pytorch_common/modules/persistent_mixin.py
--rw-r--r--   0        0        0      978 2023-04-11 23:28:05.941440 pytorch-common-0.1.1/pytorch_common/modules/predict_mixin.py
--rw-r--r--   0        0        0      338 2022-02-19 22:44:03.514014 pytorch-common-0.1.1/pytorch_common/util/__init__.py
--rw-r--r--   0        0        0      617 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      717 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/data_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1142 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/device_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1712 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0      503 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/module_utils.cpython-310.pyc
--rw-r--r--   0        0        0      347 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/os_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1106 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/stopwatch.cpython-310.pyc
--rw-r--r--   0        0        0      324 2023-04-06 16:21:38.191007 pytorch-common-0.1.1/pytorch_common/util/__pycache__/tensor_utils.cpython-310.pyc
--rw-r--r--   0        0        0      529 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/util/data_utils.py
--rw-r--r--   0        0        0      690 2022-02-17 01:17:30.513340 pytorch-common-0.1.1/pytorch_common/util/device_utils.py
--rw-r--r--   0        0        0      919 2022-02-19 22:40:31.886000 pytorch-common-0.1.1/pytorch_common/util/logger.py
--rw-r--r--   0        0        0      108 2022-02-17 01:22:32.403896 pytorch-common-0.1.1/pytorch_common/util/module_utils.py
--rw-r--r--   0        0        0      110 2022-01-15 02:50:45.422814 pytorch-common-0.1.1/pytorch_common/util/os_utils.py
--rw-r--r--   0        0        0      435 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/util/stopwatch.py
--rw-r--r--   0        0        0       66 2022-01-09 19:51:07.727683 pytorch-common-0.1.1/pytorch_common/util/tensor_utils.py
--rw-r--r--   0        0        0     8302 2023-04-11 23:29:55.219695 pytorch-common-0.1.1/setup.py
--rw-r--r--   0        0        0     7846 2023-04-11 23:29:55.220030 pytorch-common-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6896 2023-03-25 14:00:35.753299 pytorch-common-0.1.2/README.md
+-rw-r--r--   0        0        0      668 2023-04-11 23:34:33.428126 pytorch-common-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-11 23:34:37.808160 pytorch-common-0.1.2/pytorch_common/__init__.py
+-rw-r--r--   0        0        0      252 2022-02-17 01:26:29.554482 pytorch-common-0.1.2/pytorch_common/callbacks/__init__.py
+-rw-r--r--   0        0        0      490 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      368 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2001 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/callback.cpython-310.pyc
+-rw-r--r--   0        0        0     2088 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/callback.cpython-39.pyc
+-rw-r--r--   0        0        0     1427 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/callback_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     1562 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/early_stop.cpython-310.pyc
+-rw-r--r--   0        0        0     3978 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-310.pyc
+-rw-r--r--   0        0        0     2413 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-39.pyc
+-rw-r--r--   0        0        0     2011 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/save_best_model_checkpoint.cpython-310.pyc
+-rw-r--r--   0        0        0     1814 2023-04-06 17:10:38.167508 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0     1682 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/validation.cpython-39.pyc
+-rw-r--r--   0        0        0     1160 2022-02-18 23:40:01.317970 pytorch-common-0.1.2/pytorch_common/callbacks/callback.py
+-rw-r--r--   0        0        0      807 2023-04-06 16:01:08.445308 pytorch-common-0.1.2/pytorch_common/callbacks/callback_manager.py
+-rw-r--r--   0        0        0      927 2022-02-18 23:40:55.132415 pytorch-common-0.1.2/pytorch_common/callbacks/early_stop.py
+-rw-r--r--   0        0        0     2674 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/callbacks/mixin/__pycache__/metric_improve_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0     1738 2022-02-19 21:30:07.556994 pytorch-common-0.1.2/pytorch_common/callbacks/mixin/metric_improve_mixin.py
+-rw-r--r--   0        0        0      183 2022-08-13 22:39:37.132234 pytorch-common-0.1.2/pytorch_common/callbacks/output/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      340 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1336 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-310.pyc
+-rw-r--r--   0        0        0     1205 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-39.pyc
+-rw-r--r--   0        0        0     1582 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-310.pyc
+-rw-r--r--   0        0        0     1557 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-39.pyc
+-rw-r--r--   0        0        0      793 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/output_hook_callback.cpython-310.pyc
+-rw-r--r--   0        0        0      627 2022-02-18 22:32:24.693573 pytorch-common-0.1.2/pytorch_common/callbacks/output/logger_callback.py
+-rw-r--r--   0        0        0      722 2022-02-18 23:39:18.767021 pytorch-common-0.1.2/pytorch_common/callbacks/output/output_callback.py
+-rw-r--r--   0        0        0      280 2022-08-13 22:29:58.789478 pytorch-common-0.1.2/pytorch_common/callbacks/output/output_hook_callback.py
+-rw-r--r--   0        0        0        2 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      814 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-310.pyc
+-rw-r--r--   0        0        0      799 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-39.pyc
+-rw-r--r--   0        0        0     1640 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-310.pyc
+-rw-r--r--   0        0        0     1648 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-39.pyc
+-rw-r--r--   0        0        0      724 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-310.pyc
+-rw-r--r--   0        0        0      681 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-39.pyc
+-rw-r--r--   0        0        0      259 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/metric_logger.py
+-rw-r--r--   0        0        0     1045 2022-02-17 00:53:40.878623 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/metrics_plotter.py
+-rw-r--r--   0        0        0      536 2023-03-25 14:13:30.104415 pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/plot.py
+-rw-r--r--   0        0        0     3814 2022-02-19 21:31:03.207848 pytorch-common-0.1.2/pytorch_common/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0        0        0     1405 2022-02-19 21:30:18.417170 pytorch-common-0.1.2/pytorch_common/callbacks/save_best_model_checkpoint.py
+-rw-r--r--   0        0        0     1533 2023-04-06 16:39:15.512635 pytorch-common-0.1.2/pytorch_common/callbacks/validation.py
+-rw-r--r--   0        0        0      110 2022-02-17 01:32:40.208875 pytorch-common-0.1.2/pytorch_common/error/__init__.py
+-rw-r--r--   0        0        0      814 2022-02-17 01:28:00.334728 pytorch-common-0.1.2/pytorch_common/error/assertions.py
+-rw-r--r--   0        0        0     2432 2022-02-17 01:29:21.788291 pytorch-common-0.1.2/pytorch_common/error/checker.py
+-rw-r--r--   0        0        0      273 2022-02-16 22:18:12.700000 pytorch-common-0.1.2/pytorch_common/error/common_exception.py
+-rw-r--r--   0        0        0      176 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/kfoldcv/__init__.py
+-rw-r--r--   0        0        0     1146 2022-01-10 22:59:53.558378 pytorch-common-0.1.2/pytorch_common/kfoldcv/k_fold_cv.py
+-rw-r--r--   0        0        0        0 2022-01-09 21:00:39.557219 pytorch-common-0.1.2/pytorch_common/kfoldcv/strategy/__init__.py
+-rw-r--r--   0        0        0      194 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/kfoldcv/strategy/k_fold_cv_strategy.py
+-rw-r--r--   0        0        0      335 2022-01-10 22:59:53.565045 pytorch-common-0.1.2/pytorch_common/kfoldcv/strategy/non_parallel_k_fold_cv_strategy.py
+-rw-r--r--   0        0        0      536 2022-01-10 22:59:53.568378 pytorch-common-0.1.2/pytorch_common/kfoldcv/strategy/parallel_k_fold_cv_strategy.py
+-rw-r--r--   0        0        0      257 2023-04-06 16:00:59.165265 pytorch-common-0.1.2/pytorch_common/modules/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-06 16:21:38.194340 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      284 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      963 2023-04-06 16:21:38.197673 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/common_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/common_mixin.cpython-39.pyc
+-rw-r--r--   0        0        0     1512 2023-04-06 17:32:23.790493 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fit_context.cpython-310.pyc
+-rw-r--r--   0        0        0     2020 2023-04-06 17:32:23.790493 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fit_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0     1651 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fit_mixin.cpython-39.pyc
+-rw-r--r--   0        0        0     2534 2023-04-06 19:17:53.117811 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fn.cpython-310.pyc
+-rw-r--r--   0        0        0      989 2023-04-06 17:32:23.793826 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/persistent_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0     1502 2023-04-06 17:32:23.793826 pytorch-common-0.1.2/pytorch_common/modules/__pycache__/predict_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0      382 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/modules/common_mixin.py
+-rw-r--r--   0        0        0     1272 2023-04-06 17:24:42.168161 pytorch-common-0.1.2/pytorch_common/modules/fit_context.py
+-rw-r--r--   0        0        0     1981 2023-04-06 17:28:37.839367 pytorch-common-0.1.2/pytorch_common/modules/fit_mixin.py
+-rw-r--r--   0        0        0     2425 2023-04-11 23:34:22.358041 pytorch-common-0.1.2/pytorch_common/modules/fn.py
+-rw-r--r--   0        0        0      553 2023-04-06 17:23:47.241207 pytorch-common-0.1.2/pytorch_common/modules/persistent_mixin.py
+-rw-r--r--   0        0        0      978 2023-04-11 23:28:05.941440 pytorch-common-0.1.2/pytorch_common/modules/predict_mixin.py
+-rw-r--r--   0        0        0      338 2022-02-19 22:44:03.514014 pytorch-common-0.1.2/pytorch_common/util/__init__.py
+-rw-r--r--   0        0        0      617 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      717 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/data_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1142 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/device_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1712 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0      503 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/module_utils.cpython-310.pyc
+-rw-r--r--   0        0        0      347 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/os_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1106 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/stopwatch.cpython-310.pyc
+-rw-r--r--   0        0        0      324 2023-04-06 16:21:38.191007 pytorch-common-0.1.2/pytorch_common/util/__pycache__/tensor_utils.cpython-310.pyc
+-rw-r--r--   0        0        0      529 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/util/data_utils.py
+-rw-r--r--   0        0        0      690 2022-02-17 01:17:30.513340 pytorch-common-0.1.2/pytorch_common/util/device_utils.py
+-rw-r--r--   0        0        0      919 2022-02-19 22:40:31.886000 pytorch-common-0.1.2/pytorch_common/util/logger.py
+-rw-r--r--   0        0        0      108 2022-02-17 01:22:32.403896 pytorch-common-0.1.2/pytorch_common/util/module_utils.py
+-rw-r--r--   0        0        0      110 2022-01-15 02:50:45.422814 pytorch-common-0.1.2/pytorch_common/util/os_utils.py
+-rw-r--r--   0        0        0      435 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/util/stopwatch.py
+-rw-r--r--   0        0        0       66 2022-01-09 19:51:07.727683 pytorch-common-0.1.2/pytorch_common/util/tensor_utils.py
+-rw-r--r--   0        0        0     8302 2023-04-11 23:35:37.971699 pytorch-common-0.1.2/setup.py
+-rw-r--r--   0        0        0     7846 2023-04-11 23:35:37.972024 pytorch-common-0.1.2/PKG-INFO
```

### Comparing `pytorch-common-0.1.1/README.md` & `pytorch-common-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pyproject.toml` & `pytorch-common-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch-common"
-version = "0.1.1"
+version = "0.1.2"
 description = "Common torch tools and extension"
 authors = ["adrianmarino <adrianmarino@gmail.com>"]
 keywords = ["pytorch", "common"]
 include = ["pytorch_common/**/*.py"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/adrianmarino/pytorch-common/tree/master"
```

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/callback.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/callback.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/callback.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/callback.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/callback_manager.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/callback_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/early_stop.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/early_stop.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/reduce_lr_on_plateau.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/save_best_model_checkpoint.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/save_best_model_checkpoint.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/validation.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/validation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/__pycache__/validation.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/__pycache__/validation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/callback.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/callback_manager.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/callback_manager.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/early_stop.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/mixin/__pycache__/metric_improve_mixin.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/mixin/__pycache__/metric_improve_mixin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/mixin/metric_improve_mixin.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/mixin/metric_improve_mixin.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/logger_callback.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/output_callback.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/__pycache__/output_hook_callback.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/__pycache__/output_hook_callback.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/logger_callback.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/logger_callback.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/output_callback.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/output_callback.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metric_logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/metrics_plotter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/__pycache__/plot.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/metrics_plotter.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/metrics_plotter.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/output/plot/plot.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/output/plot/plot.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/reduce_lr_on_plateau.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/save_best_model_checkpoint.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/save_best_model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/callbacks/validation.py` & `pytorch-common-0.1.2/pytorch_common/callbacks/validation.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/error/assertions.py` & `pytorch-common-0.1.2/pytorch_common/error/assertions.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/error/checker.py` & `pytorch-common-0.1.2/pytorch_common/error/checker.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/kfoldcv/k_fold_cv.py` & `pytorch-common-0.1.2/pytorch_common/kfoldcv/k_fold_cv.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/kfoldcv/strategy/parallel_k_fold_cv_strategy.py` & `pytorch-common-0.1.2/pytorch_common/kfoldcv/strategy/parallel_k_fold_cv_strategy.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/common_mixin.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/common_mixin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/common_mixin.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/common_mixin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fit_context.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fit_context.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fit_mixin.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fit_mixin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fit_mixin.cpython-39.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fit_mixin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/fn.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/fn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/persistent_mixin.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/persistent_mixin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/__pycache__/predict_mixin.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/modules/__pycache__/predict_mixin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/fit_context.py` & `pytorch-common-0.1.2/pytorch_common/modules/fit_context.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/fit_mixin.py` & `pytorch-common-0.1.2/pytorch_common/modules/fit_mixin.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/fn.py` & `pytorch-common-0.1.2/pytorch_common/modules/fn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch          import as_tensor
 from .fit_context   import FitContextFactory
-
+import numpy as np
 
 
 class Fn:
     @staticmethod
     def train(ctx, data_loader):
         """Default train function. It perform a nomal trainig process.
 
@@ -30,15 +30,15 @@
             total_loss += loss.item()
 
         return total_loss / len(data_loader)
 
 
     @staticmethod
     def validation(ctx, data_loader):
-        """Default validation function. It perform a nomal model validation process.
+        """Default validation function. It perform a normal model validation process.
 
         Args:
             ctx: Contain all object required to perform a train process. See FitContextFactory class to see a context detail.
             data_loader: Data loader with validation data.
 
         Returns:
             a (y_pred, y_true) tuple.
@@ -48,15 +48,15 @@
         with torch.no_grad():
             for index, (features, target) in enumerate(data_loader):
                 prediction = ctx.model(features.to(ctx.model.device))
 
                 y_pred.extend(prediction.cpu().numpy())
                 y_true.extend(target.cpu().numpy())
 
-        return as_tensor(y_pred).cpu(), as_tensor(y_true).cpu()
+        return as_tensor(np.array(y_pred)).cpu(), as_tensor(np.array(y_true)).cpu()
 
 
     @staticmethod
     def validation_score(model, data_loader, score_fn):
         """Apply an score function to Fn.validation function result.
 
         Args:
```

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/persistent_mixin.py` & `pytorch-common-0.1.2/pytorch_common/modules/persistent_mixin.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/modules/predict_mixin.py` & `pytorch-common-0.1.2/pytorch_common/modules/predict_mixin.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/__pycache__/__init__.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/util/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/__pycache__/data_utils.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/util/__pycache__/data_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/__pycache__/device_utils.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/util/__pycache__/device_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/__pycache__/logger.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/util/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/__pycache__/stopwatch.cpython-310.pyc` & `pytorch-common-0.1.2/pytorch_common/util/__pycache__/stopwatch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/data_utils.py` & `pytorch-common-0.1.2/pytorch_common/util/data_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/device_utils.py` & `pytorch-common-0.1.2/pytorch_common/util/device_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/pytorch_common/util/logger.py` & `pytorch-common-0.1.2/pytorch_common/util/logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-common-0.1.1/setup.py` & `pytorch-common-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'numpy>=1.20',
  'scikit-learn>=1.0.2',
  'seaborn>=0.11.2',
  'torch>=1.10.1']
 
 setup_kwargs = {
     'name': 'pytorch-common',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Common torch tools and extension',
     'long_description': "# pytorch-common\n\nA [Pypi module](https://pypi.org/project/pytorch-common/) with pytorch common tools like:\n\n\n## Build release\n\n**Step 1**: Increase version into next files:\n\n```bash\npytorch_common/__init__.py\npyproject.toml\n```\n\n**Step 2**: Build release.\n\n```bash\n$ poetry build                                                                                                                                                                                                                 \ue0b2 ✔ \ue0b3 \n\nBuilding pytorch-common (0.0.22)\n  - Building sdist\n  - Built pytorch-common-0.0.22.tar.gz\n  - Building wheel\n  - Built pytorch_common-0.0.22-py3-none-any.whl\n```\n\n**Step 3**: Publish release to PyPI repository.\n\n```bash\n$ poetry build                                                                                                                                                                                                                 \ue0b2 ✔ \ue0b3 \n\nUsername: user_name\nPassword: a pass\n\nPublishing pytorch-common (0.0.22) to PyPI\n - Uploading pytorch-common-0.0.22.tar.gz 100%\n - Uploading pytorch_common-0.0.22-py3-none-any.whl 100%\n```\n\n\n## Features\n\n* **Callbacks** (keras style)\n  * **Validation**: Model validation.\n  * **ReduceLROnPlateau**:\n    * Reduce learning rate when a metric has stopped improving.\n    * Models often benefit from reducing the learning rate by a factor\n      of 2-10 once learning stagnates. This scheduler reads a metrics\n      quantity and if no improvement is seen for a 'patience' number\n      of epochs, the learning rate is reduced.\n  * **EarlyStop**:\n    * Stop training when model has stopped improving a specified metric.\n  * **SaveBestModel**:\n    * Save model weights to file while model validation metric improve.\n  * **Logger**:\n    * Logs context properties.\n    * In general is used to log performance metrics every n epochs.\n  * **MetricsPlotter**:\n    * Plot evaluation metrics.\n    * This graph is updated every n epochs during training process.\n  * **Callback** and **OutputCallback**:\n    * Base classes.\n  * **CallbackManager**:\n    * Simplify callbacks support to fit custom models.\n* **StratifiedKFoldCV**:\n  * Support parallel fold processing on CPU.\n* **Mixins**\n  * FiMixin\n  * CommonMixin\n  * PredictMixin\n  * PersistentMixin\n* **Utils**\n  * device management\n  * stopwatch\n  * data split\n  * os\n  * model\n  * LoggerBuilder\n\n## Examples\n\n### Device management\n\n\n```python\nimport pytorch_common.util as pu\n\n# Setup prefered device.\npu.set_device_name('gpu') # / 'cpu'\n\n# Setup GPU memory fraction for a process (%).\npu.set_device_memory(\n  'gpu' # / 'cpu',\n  process_memory_fraction=0.5\n)\n\n# Get prefered device.\n# Note: In case the preferred device is not found, it returns CPU as fallback.\ndevice = pu.get_device()\n```\n\n### Logging\n\n\n```python\nimport logging\nimport pytorch_common.util as pu\n\n## Default loggin in console...\npu.LoggerBuilder() \\\n .on_console() \\\n .build()\n\n## Setup format and level...\npu.LoggerBuilder() \\\n .level(logging.ERROR) \\\n .on_console('%(asctime)s - %(levelname)s - %(message)s') \\\n .build()\n```\n\n\n### Stopwatch\n\n\n```python\nimport logging\nimport pytorch_common.util as pu\n\nsw = pu.Stopwatch()\n\n# Call any demanding process...\n\n# Get resposne time.\nresposne_time = sw.elapsed_time()\n\n# Log resposne time.\nlogging.info(sw.to_str())\n```\n\n\n### Dataset split\n\n\n```python\nimport pytorch_common.util as pu\n\ndataset = ... # <-- Torch.utils.data.Dataset\n\ntrain_subset, test_subset = pu.train_val_split(\n  dataset,\n  train_percent = .7\n)\n\ntrain_subset, val_subset, test_subset = pu.train_val_test_split(\n  dataset,\n  train_percent = .7,\n  val_percent   = .15\n)\n```\n\n\n### Kfolding\n\n```python\nimport logging\nfrom pytorch_common.kfoldcv import StratifiedKFoldCV, \\\n                                   ParallelKFoldCVStrategy, \\\n                                   NonParallelKFoldCVStrategy\n\n# Call your model under this function..\ndef train_fold_fn(dataset, train_idx, val_idx, params, fold):\n  pass\n\n# Get dataset labels\ndef get_y_values_fn(dataset):\n  pass\n\ncv = StratifiedKFoldCV(\n  train_fold_fn,\n  get_y_values_fn,\n  strategy=NonParallelKFoldCVStrategy() # or ParallelKFoldCVStrategy()\n  k_fold = 5\n)\n\n# Model hyperparams...\nparams = {\n    'seed': 42,\n    'lr': 0.01,\n    'epochs': 50,\n    'batch_size': 4000,\n    ...\n}\n\n# Train model...\nresult = cv.train(dataset, params)\n\nlogging.info('CV results: {}'.format(result))\n```\n\n\n### Assertions\n\n\n```python\nfrom pytorch_common.error import Assertions, Checker\n\n# Check functions and construtor params usign assertions..\n\nparam_value = -1\n\n# Raise an exception with 404103 eror code when the condition is not met \nAssertions.positive_int(404103, param_value, 'param name')\n\nAssertions.positive_float(404103, param_value, 'param name')\n\n# Other options\nAssertions.is_class(404205, param_value, 'param name', aClass)\n\nAssertions.is_tensor(404401, param_value, 'param name')\n\nAssertions.has_shape(404401, param_value, (3, 4), 'param name')\n\n# Assertions was impelemented using a Checker builder:\n\n Checker(error_code, value, name) \\\n    .is_not_none() \\\n    .is_int() \\\n    .is_positive() \\\n    .check()\n\n# Other checker options..\n#   .is_not_none()\n#   .is_int()\n#   .is_float()\n#   .is_positive()\n#   .is_a(aclass)\n#   .is_tensor()\n#   .has_shape(shape)\n```\n\n\n### Callbacks\n\n```python\nfrom pytorch_common.callbacks import CallbackManager\n\nfrom pytorch_common.callbacks import EarlyStop, \\\n                                     ReduceLROnPlateau, \\\n                                     Validation\n\nfrom pytorch_common.callbacks.output import Logger, \\\n                                            MetricsPlotter\n\n\ndef train_method(model, epochs, optimizer, loss_fn, callbacks):\n\n callback_manager = CallbackManager(epochs, optimizer, loss_fn, model, callbacks)\n\n for epoch in range(epochs):\n            callback_manager.on_epoch_start(epoch)\n\n            # train model...\n\n            callback_manager.on_epoch_end(train_loss)\n\n            if callback_manager.break_training():\n                break\n\n  return callback_manager.ctx\n\n\nmodel     = # Create my model...\noptimizer = # My optimizer...\nloss_fn   = # my lost function\n\ncallbacks = [\n   # Log context variables after each epoch...\n   Logger(['fold', 'time', 'epoch', 'lr', 'train_loss', 'val_loss', ... ]),\n\n   EarlyStop(metric='val_auc', mode='max', patience=3),\n   \n   ReduceLROnPlateau(metric='val_auc'),\n  \n   Validation(\n       val_set,\n       metrics = {\n           'my_metric_name': lambda y_pred, y_true: # calculate validation metic,\n           ...\n       },\n       each_n_epochs=5\n   ),\n   \n   SaveBestModel(metric='val_loss'),\n   \n   MetricsPlotter(metrics=['train_loss', 'val_loss'])\n]\n\n\ntrain_method(model, epochs=100, optimizer, loss_fn, callbacks)\n```\n\nGo to next projects to see funcional code examples:\n\n- https://github.com/adrianmarino/deep-fm\n- https://github.com/adrianmarino/attention\n\n\n",
     'author': 'adrianmarino',
     'author_email': 'adrianmarino@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/adrianmarino/pytorch-common/tree/master',
```

### Comparing `pytorch-common-0.1.1/PKG-INFO` & `pytorch-common-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-common
-Version: 0.1.1
+Version: 0.1.2
 Summary: Common torch tools and extension
 Home-page: https://github.com/adrianmarino/pytorch-common/tree/master
 License: MIT
 Keywords: pytorch,common
 Author: adrianmarino
 Author-email: adrianmarino@gmail.com
 Requires-Python: >=3.7
```

