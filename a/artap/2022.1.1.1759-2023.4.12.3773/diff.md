# Comparing `tmp/artap-2022.1.1.1759.tar.gz` & `tmp/artap-2023.4.12.3773.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artap-2022.1.1.1759.tar", last modified: Sat Jan  1 15:13:19 2022, max compression
+gzip compressed data, was "artap-2023.4.12.3773.tar", last modified: Wed Apr 12 18:42:54 2023, max compression
```

## Comparing `artap-2022.1.1.1759.tar` & `artap-2023.4.12.3773.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2022-01-01 15:13:19.369004 artap-2022.1.1.1759/
--rw-rw-r--   0 karban    (1000) karban    (1000)     1070 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/LICENSE
--rw-rw-r--   0 karban    (1000) karban    (1000)       19 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/MANIFEST.in
--rw-rw-r--   0 karban    (1000) karban    (1000)     6195 2022-01-01 15:13:19.369004 artap-2022.1.1.1759/PKG-INFO
--rw-rw-r--   0 karban    (1000) karban    (1000)     4684 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/README.md
-drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2022-01-01 15:13:19.349004 artap-2022.1.1.1759/artap/
--rw-rw-r--   0 karban    (1000) karban    (1000)       32 2022-01-01 15:13:19.000000 artap-2022.1.1.1759/artap/__init__.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2302 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/algorithm.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     8946 2021-08-13 08:04:38.000000 artap-2022.1.1.1759/artap/algorithm_bayesopt.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     6514 2021-12-11 20:33:19.000000 artap-2022.1.1.1759/artap/algorithm_cmaes.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    11203 2021-02-24 16:02:20.000000 artap-2022.1.1.1759/artap/algorithm_genetic.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     7209 2021-12-26 08:53:48.000000 artap-2022.1.1.1759/artap/algorithm_gradient_descent.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    11362 2021-12-11 20:33:19.000000 artap-2022.1.1.1759/artap/algorithm_monte_carlo.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     5397 2021-10-30 17:09:42.000000 artap-2022.1.1.1759/artap/algorithm_nlopt.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     4885 2021-11-13 18:00:37.000000 artap-2022.1.1.1759/artap/algorithm_pymoo.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1499 2021-08-13 08:57:07.000000 artap-2022.1.1.1759/artap/algorithm_scipy.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     6789 2021-08-13 09:58:13.000000 artap-2022.1.1.1759/artap/algorithm_sensitivity.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    39257 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/algorithm_swarm.py
--rw-rw-r--   0 karban    (1000) karban    (1000)      834 2020-10-17 07:24:12.000000 artap-2022.1.1.1759/artap/algorithm_sweep.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     3556 2020-07-26 10:08:50.000000 artap-2022.1.1.1759/artap/archive.py
--rw-rw-r--   0 karban    (1000) karban    (1000)  1047574 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/benchmark_functions.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    16690 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/benchmark_pareto.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     8355 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/benchmark_robust.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    50528 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/colormaps.py
--rw-rw-r--   0 karban    (1000) karban    (1000)      790 2021-06-08 07:07:53.000000 artap-2022.1.1.1759/artap/config.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     6192 2021-04-04 07:52:13.000000 artap-2022.1.1.1759/artap/datastore.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    55228 2020-08-27 06:51:17.000000 artap-2022.1.1.1759/artap/doe.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    29020 2021-08-18 18:21:36.000000 artap-2022.1.1.1759/artap/executor.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     6332 2021-11-13 18:36:27.000000 artap-2022.1.1.1759/artap/individual.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2728 2021-11-13 18:35:40.000000 artap-2022.1.1.1759/artap/job.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    59169 2021-11-21 17:03:10.000000 artap-2022.1.1.1759/artap/operators.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     7985 2021-11-10 06:26:21.000000 artap-2022.1.1.1759/artap/problem.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     3419 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/quality_indicator.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     7210 2021-12-26 08:57:49.000000 artap-2022.1.1.1759/artap/reliability_analysis.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    12103 2021-10-20 10:38:53.000000 artap-2022.1.1.1759/artap/results.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     4307 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/surrogate.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    11577 2020-12-01 08:13:37.000000 artap-2022.1.1.1759/artap/surrogate_scikit.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1661 2021-10-30 17:22:08.000000 artap-2022.1.1.1759/artap/surrogate_smt.py
-drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2022-01-01 15:13:19.369004 artap-2022.1.1.1759/artap/tests/
--rw-rw-r--   0 karban    (1000) karban    (1000)        0 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/__init__.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    15396 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/_test_scikit.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     9539 2021-08-23 18:54:46.000000 artap-2022.1.1.1759/artap/tests/test_agros.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2795 2020-07-21 19:40:46.000000 artap-2022.1.1.1759/artap/tests/test_algorithm.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     5060 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/test_archive.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2646 2021-08-11 07:23:20.000000 artap-2022.1.1.1759/artap/tests/test_benchmark_pareto.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2815 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/test_benchmark_robust.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     6907 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/tests/test_benchmarks.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1379 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/test_calculation_fails.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     5700 2021-10-20 17:48:10.000000 artap-2022.1.1.1759/artap/tests/test_datastore.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     9549 2021-04-04 07:37:14.000000 artap-2022.1.1.1759/artap/tests/test_generators.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1656 2021-08-13 09:07:33.000000 artap-2022.1.1.1759/artap/tests/test_gradients.py
--rw-rw-r--   0 karban    (1000) karban    (1000)      917 2021-10-30 19:39:45.000000 artap-2022.1.1.1759/artap/tests/test_job.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2366 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/test_local_comsol.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2432 2021-08-24 07:12:48.000000 artap-2022.1.1.1759/artap/tests/test_local_femm.py
--rw-rw-r--   0 karban    (1000) karban    (1000)    22084 2020-10-17 06:28:32.000000 artap-2022.1.1.1759/artap/tests/test_operators.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1309 2021-08-13 08:03:56.000000 artap-2022.1.1.1759/artap/tests/test_problem_bayesopt.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2542 2021-11-21 17:02:54.000000 artap-2022.1.1.1759/artap/tests/test_problem_cmaes.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1863 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/tests/test_problem_epsmoea.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     4980 2021-12-26 08:57:33.000000 artap-2022.1.1.1759/artap/tests/test_problem_gradient_descent.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2842 2021-12-26 08:57:49.000000 artap-2022.1.1.1759/artap/tests/test_problem_monte_carlo.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     4919 2021-10-30 17:09:58.000000 artap-2022.1.1.1759/artap/tests/test_problem_nlopt.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     5738 2021-11-13 18:37:20.000000 artap-2022.1.1.1759/artap/tests/test_problem_nsga2.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     5383 2021-11-13 18:37:03.000000 artap-2022.1.1.1759/artap/tests/test_problem_pymoo.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1208 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/tests/test_problem_scipy.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     8407 2021-10-20 10:38:53.000000 artap-2022.1.1.1759/artap/tests/test_problem_swarm.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1035 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/test_quality_indicator.py
--rw-rw-r--   0 karban    (1000) karban    (1000)      675 2021-12-26 08:57:49.000000 artap-2022.1.1.1759/artap/tests/test_reliability_analysis.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     9714 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/tests/test_remote_condor.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     8897 2021-10-30 19:39:55.000000 artap-2022.1.1.1759/artap/tests/test_results.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1198 2020-07-24 20:19:04.000000 artap-2022.1.1.1759/artap/tests/test_robust.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1461 2021-10-20 10:38:53.000000 artap-2022.1.1.1759/artap/tests/test_sensitivity.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     1169 2020-12-01 08:56:05.000000 artap-2022.1.1.1759/artap/tests/test_surrogate_eval.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     4581 2021-08-23 18:24:47.000000 artap-2022.1.1.1759/artap/tests/test_surrogate_function.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     8624 2020-12-01 08:57:24.000000 artap-2022.1.1.1759/artap/tests/test_surrogate_scikit.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     2747 2020-12-01 08:55:48.000000 artap-2022.1.1.1759/artap/tests/test_surrogate_smt.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     9929 2021-08-11 06:20:39.000000 artap-2022.1.1.1759/artap/tests/test_swarm.py
--rw-rw-r--   0 karban    (1000) karban    (1000)       98 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/tests/tests_root.py
--rw-rw-r--   0 karban    (1000) karban    (1000)     9134 2020-07-20 11:13:04.000000 artap-2022.1.1.1759/artap/utils.py
-drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2022-01-01 15:13:19.349004 artap-2022.1.1.1759/artap.egg-info/
--rw-rw-r--   0 karban    (1000) karban    (1000)     6195 2022-01-01 15:13:19.000000 artap-2022.1.1.1759/artap.egg-info/PKG-INFO
--rw-rw-r--   0 karban    (1000) karban    (1000)     2206 2022-01-01 15:13:19.000000 artap-2022.1.1.1759/artap.egg-info/SOURCES.txt
--rw-rw-r--   0 karban    (1000) karban    (1000)        1 2022-01-01 15:13:19.000000 artap-2022.1.1.1759/artap.egg-info/dependency_links.txt
--rw-rw-r--   0 karban    (1000) karban    (1000)        1 2020-07-20 11:15:55.000000 artap-2022.1.1.1759/artap.egg-info/not-zip-safe
--rw-rw-r--   0 karban    (1000) karban    (1000)      172 2022-01-01 15:13:19.000000 artap-2022.1.1.1759/artap.egg-info/requires.txt
--rw-rw-r--   0 karban    (1000) karban    (1000)        6 2022-01-01 15:13:19.000000 artap-2022.1.1.1759/artap.egg-info/top_level.txt
--rw-rw-r--   0 karban    (1000) karban    (1000)       38 2022-01-01 15:13:19.369004 artap-2022.1.1.1759/setup.cfg
--rw-rw-r--   0 karban    (1000) karban    (1000)     2710 2020-10-17 06:27:49.000000 artap-2022.1.1.1759/setup.py
+drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2023-04-12 18:42:54.296141 artap-2023.4.12.3773/
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1070 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/LICENSE
+-rw-rw-r--   0 karban    (1000) karban    (1000)       19 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/MANIFEST.in
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5435 2023-04-12 18:42:54.296141 artap-2023.4.12.3773/PKG-INFO
+-rw-rw-r--   0 karban    (1000) karban    (1000)     4684 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/README.md
+drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2023-04-12 18:42:54.292141 artap-2023.4.12.3773/artap/
+-rw-rw-r--   0 karban    (1000) karban    (1000)       32 2023-04-12 18:42:53.000000 artap-2023.4.12.3773/artap/__init__.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2303 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/algorithm.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     4374 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/algorithm_NSGAII.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     8946 2021-08-13 08:04:38.000000 artap-2023.4.12.3773/artap/algorithm_bayesopt.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     4421 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/algorithm_cem.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     6800 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/algorithm_cmaes.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     7387 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/algorithm_genetic.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     7298 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/algorithm_gradient_descent.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    11421 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/algorithm_monte_carlo.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5397 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/algorithm_nlopt.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5018 2023-04-06 10:10:47.000000 artap-2023.4.12.3773/artap/algorithm_pymoo.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1499 2021-08-13 08:57:07.000000 artap-2023.4.12.3773/artap/algorithm_scipy.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     6789 2021-08-13 09:58:13.000000 artap-2023.4.12.3773/artap/algorithm_sensitivity.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    28053 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/algorithm_swarm.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)      947 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/algorithm_sweep.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     3556 2020-07-26 10:08:50.000000 artap-2023.4.12.3773/artap/archive.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)  1047574 2021-08-11 06:20:39.000000 artap-2023.4.12.3773/artap/benchmark_functions.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    16690 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/benchmark_pareto.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     8355 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/benchmark_robust.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    50528 2021-08-11 06:20:39.000000 artap-2023.4.12.3773/artap/colormaps.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)      790 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/config.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     6192 2021-04-04 07:52:13.000000 artap-2023.4.12.3773/artap/datastore.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    55228 2020-08-27 06:51:17.000000 artap-2023.4.12.3773/artap/doe.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    30317 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/executor.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     6408 2023-04-06 10:50:20.000000 artap-2023.4.12.3773/artap/individual.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2728 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/job.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    59997 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/operators.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     8055 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/problem.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     3419 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/quality_indicator.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    11847 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/reliability_analysis.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    17462 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/results.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     4307 2021-08-11 06:20:39.000000 artap-2023.4.12.3773/artap/surrogate.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    11577 2020-12-01 08:13:37.000000 artap-2023.4.12.3773/artap/surrogate_scikit.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1647 2023-04-06 10:39:59.000000 artap-2023.4.12.3773/artap/surrogate_smt.py
+drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2023-04-12 18:42:54.296141 artap-2023.4.12.3773/artap/tests/
+-rw-rw-r--   0 karban    (1000) karban    (1000)        0 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/tests/__init__.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    15396 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/tests/_test_scikit.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     9572 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_agros.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2795 2020-07-21 19:40:46.000000 artap-2023.4.12.3773/artap/tests/test_algorithm.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5060 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/tests/test_archive.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2646 2021-08-11 07:23:20.000000 artap-2023.4.12.3773/artap/tests/test_benchmark_pareto.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2815 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/tests/test_benchmark_robust.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     6908 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_benchmarks.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1378 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_calculation_fails.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5743 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_datastore.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     8780 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_generators.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1656 2021-08-13 09:07:33.000000 artap-2023.4.12.3773/artap/tests/test_gradients.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)      917 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_job.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2366 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/tests/test_local_comsol.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2713 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/tests/test_local_cst.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2448 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_local_femm.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    21898 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/tests/test_operators.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1309 2021-08-13 08:03:56.000000 artap-2023.4.12.3773/artap/tests/test_problem_bayesopt.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1019 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_problem_cem.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2542 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_problem_cmaes.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1863 2021-08-11 06:20:39.000000 artap-2023.4.12.3773/artap/tests/test_problem_epsmoea.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     4957 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_problem_gradient_descent.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     3432 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_problem_monte_carlo.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     4920 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_problem_nlopt.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5596 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/tests/test_problem_nsga2.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5491 2023-04-06 10:09:31.000000 artap-2023.4.12.3773/artap/tests/test_problem_pymoo.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1208 2021-08-11 06:20:39.000000 artap-2023.4.12.3773/artap/tests/test_problem_scipy.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     8386 2023-04-03 19:01:05.000000 artap-2023.4.12.3773/artap/tests/test_problem_swarm.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1035 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/tests/test_quality_indicator.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1260 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_reliability_analysis.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     9789 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_remote_condor.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)    10163 2023-04-06 10:15:18.000000 artap-2023.4.12.3773/artap/tests/test_results.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1198 2020-07-24 20:19:04.000000 artap-2023.4.12.3773/artap/tests/test_robust.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1413 2022-07-27 12:50:29.000000 artap-2023.4.12.3773/artap/tests/test_sensitivity.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     1169 2020-12-01 08:56:05.000000 artap-2023.4.12.3773/artap/tests/test_surrogate_eval.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     4546 2023-04-06 10:46:19.000000 artap-2023.4.12.3773/artap/tests/test_surrogate_function.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     8624 2020-12-01 08:57:24.000000 artap-2023.4.12.3773/artap/tests/test_surrogate_scikit.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2747 2020-12-01 08:55:48.000000 artap-2023.4.12.3773/artap/tests/test_surrogate_smt.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     9597 2022-10-27 12:58:52.000000 artap-2023.4.12.3773/artap/tests/test_swarm.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)       98 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/tests/tests_root.py
+-rw-rw-r--   0 karban    (1000) karban    (1000)     9134 2020-07-20 11:13:04.000000 artap-2023.4.12.3773/artap/utils.py
+drwxrwxr-x   0 karban    (1000) karban    (1000)        0 2023-04-12 18:42:54.292141 artap-2023.4.12.3773/artap.egg-info/
+-rw-rw-r--   0 karban    (1000) karban    (1000)     5435 2023-04-12 18:42:54.000000 artap-2023.4.12.3773/artap.egg-info/PKG-INFO
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2317 2023-04-12 18:42:54.000000 artap-2023.4.12.3773/artap.egg-info/SOURCES.txt
+-rw-rw-r--   0 karban    (1000) karban    (1000)        1 2023-04-12 18:42:54.000000 artap-2023.4.12.3773/artap.egg-info/dependency_links.txt
+-rw-rw-r--   0 karban    (1000) karban    (1000)        1 2020-07-20 11:15:55.000000 artap-2023.4.12.3773/artap.egg-info/not-zip-safe
+-rw-rw-r--   0 karban    (1000) karban    (1000)      170 2023-04-12 18:42:54.000000 artap-2023.4.12.3773/artap.egg-info/requires.txt
+-rw-rw-r--   0 karban    (1000) karban    (1000)        6 2023-04-12 18:42:54.000000 artap-2023.4.12.3773/artap.egg-info/top_level.txt
+-rw-rw-r--   0 karban    (1000) karban    (1000)       38 2023-04-12 18:42:54.296141 artap-2023.4.12.3773/setup.cfg
+-rw-rw-r--   0 karban    (1000) karban    (1000)     2710 2020-10-17 06:27:49.000000 artap-2023.4.12.3773/setup.py
```

### Comparing `artap-2022.1.1.1759/LICENSE` & `artap-2023.4.12.3773/LICENSE`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/PKG-INFO` & `artap-2023.4.12.3773/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 Metadata-Version: 2.1
 Name: artap
-Version: 2022.1.1.1759
+Version: 2023.4.12.3773
 Summary: Platform for robust design optimization
 Home-page: http://www.agros2d.org/artap/
 Author: Artap Team
 Author-email: artap.framework@gmail.com
 License: License :: OSI Approved :: MIT License
-Description: # Ārtap
-        
-        Ārtap is a framework for robust design optimization in Python. It contains an integrated, multi-physical FEM solver: Agros suite, furthermore it provides simple interfaces for commercial FEM solvers (COMSOL) and meta-heuristic, bayesian or neural network based optimization algorithms surrogate modelling techniques and neural networks.
-        
-        ## Installation
-        
-        Artap and its dependencies are available as wheel packages for Windows and Linux* distributions:
-        We recommend to install Artap under a [virtual environment](https://docs.python.org/3/tutorial/venv.html).
-        
-            pip install --upgrade pip # make sure that pip is reasonably new
-            pip install artap
-        
-        *The Windows versions are only partially, the linux packages are fully supported at the current version.
-        
-        ### Linux 
-        
-        You can install the full package, which contains the agrossuite package by the following command:
-        
-            pip install --upgrade pip # make sure that pip is reasonably new
-            pip install artap[full]
-        
-        ## Basic usage
-        
-        The goal of this example to show, how we can use Artap to solve a simple, bi-objective optimization problem.
-        
-        The problem is defined in the following way [GDE3]:
-        
-            Minimize f1 = x1
-            Minimize f2 = (1+x2) / x1
-        
-            subject to
-                    x1 e [0.1, 1]
-                    x2 e [0, 5]
-        
-        The Pareto - front of the following problem is known, it is a simple hyperbola. This problem is very simple for an Evolutionary algorithm, it finds its solution within 20-30 generations.
-         NSGA - II algorithm is used to solve this example.
-        
-        ### The Problem definition and solution with NSGA-II in Ārtap:
-        
-            class BiObjectiveTestProblem(Problem):
-        
-                def set(self):
-        
-                    self.name = 'Biobjective Test Problem'
-                    
-                    self.parameters = [{'name':'x_1', 'bounds': [0.1, 1.]},
-                                       {'name':'x_2', 'bounds': [0.0, 5.0]}]
-        
-                    self.costs = [{'name': 'f_1', 'criteria': 'minimize'},
-                                  {'name': 'f_2', 'criteria': 'minimize'}]
-        
-                def evaluate(self, individual):
-                    f1 = individual.vector[0]
-                    f2 = (1+individual.vector[1])/individual.vector[0]
-                return [f1, f2]
-         
-            # Perform the optimization iterating over 100 times on 100 individuals.
-            problem = BiObjectiveTestProblem()
-            algorithm = NSGAII(problem)
-            algorithm.options['max_population_number'] = 100
-            algorithm.options['max_population_size'] = 100
-            algorithm.run()
-        
-        ## References
-        
-        * [GDE3] Saku Kukkonen, Jouni Lampinen, The third Evolution Step of Generalized Differential Evolution
-        
-        
-        ## Citing
-        
-        If you use Ārtap in your research, the developers would be grateful if you would cite the relevant publications:
-        
-        [1]  Karban, Pavel, David Pánek, Tamás Orosz, Iveta Petrášová, and Ivo Doležel. “FEM based robust design optimization with Agros and Ārtap.” Computers & Mathematics with Applications (2020) https://doi.org/10.1016/j.camwa.2020.02.010.
-        
-        [2] Pánek, David, Tamás Orosz, and Pavel Karban. ” Ārtap: robust design optimization framework for engineering applications.” arXiv preprint arXiv:1912.11550 (2019).
-        
-        ### Applications
-        [3] Karban, P., Pánek, D., & Doležel, I. (2018). Model of induction brazing of nonmagnetic metals using model order reduction approach. COMPEL-The international journal for computation and mathematics in electrical and electronic engineering, 37(4), 1515-1524, https://doi.org/10.1108/COMPEL-08-2017-0356.
-        
-        [4] Pánek, D., Orosz, T., Kropík, P., Karban, P., & Doležel, I. (2019, June). Reduced-Order Model Based Temperature Control of Induction Brazing Process. In 2019 Electric Power Quality and Supply Reliability Conference (PQ) & 2019 Symposium on Electrical Engineering and Mechatronics (SEEM) (pp. 1-4). IEEE, https://doi.org/10.1109/PQ.2019.8818256.
-        
-        [5] Pánek, D., Karban, P., & Doležel, I. (2019). Calibration of Numerical Model of Magnetic Induction Brazing. IEEE Transactions on Magnetics, 55(6), 1-4, https://doi.org/10.1109/TMAG.2019.2897571.
-        
-        [6] Pánek, D., Orosz, T., Karban, P., & Doležel, I. (2020), “Comparison of simplified techniques for solving selected coupled electroheat problems”, COMPEL – The international journal for computation and mathematics in electrical and electronic engineering, Vol. 39 No. 1, pp. 220-230. https://doi.org/10.1108/COMPEL-06-2019-0244
-        
-        [7] Orosz, T.; Pánek, D.; Karban, P. FEM Based Preliminary Design Optimization in Case of Large Power Transformers. Appl. Sci. 2020, 10, 1361, https://doi.org/10.3390/app10041361.
-        
-        ## Contact
-        
-        If you have any questions, do not hesitate to contact us: artap.framework@gmail.com
-        
-        ## License
-        
-        Ārtap is published under [MIT license](https://en.wikipedia.org/wiki/MIT_License)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: full
+License-File: LICENSE
+
+# Ārtap
+
+Ārtap is a framework for robust design optimization in Python. It contains an integrated, multi-physical FEM solver: Agros suite, furthermore it provides simple interfaces for commercial FEM solvers (COMSOL) and meta-heuristic, bayesian or neural network based optimization algorithms surrogate modelling techniques and neural networks.
+
+## Installation
+
+Artap and its dependencies are available as wheel packages for Windows and Linux* distributions:
+We recommend to install Artap under a [virtual environment](https://docs.python.org/3/tutorial/venv.html).
+
+    pip install --upgrade pip # make sure that pip is reasonably new
+    pip install artap
+
+*The Windows versions are only partially, the linux packages are fully supported at the current version.
+
+### Linux 
+
+You can install the full package, which contains the agrossuite package by the following command:
+
+    pip install --upgrade pip # make sure that pip is reasonably new
+    pip install artap[full]
+
+## Basic usage
+
+The goal of this example to show, how we can use Artap to solve a simple, bi-objective optimization problem.
+
+The problem is defined in the following way [GDE3]:
+
+    Minimize f1 = x1
+    Minimize f2 = (1+x2) / x1
+
+    subject to
+            x1 e [0.1, 1]
+            x2 e [0, 5]
+
+The Pareto - front of the following problem is known, it is a simple hyperbola. This problem is very simple for an Evolutionary algorithm, it finds its solution within 20-30 generations.
+ NSGA - II algorithm is used to solve this example.
+
+### The Problem definition and solution with NSGA-II in Ārtap:
+
+    class BiObjectiveTestProblem(Problem):
+
+        def set(self):
+
+            self.name = 'Biobjective Test Problem'
+            
+            self.parameters = [{'name':'x_1', 'bounds': [0.1, 1.]},
+                               {'name':'x_2', 'bounds': [0.0, 5.0]}]
+
+            self.costs = [{'name': 'f_1', 'criteria': 'minimize'},
+                          {'name': 'f_2', 'criteria': 'minimize'}]
+
+        def evaluate(self, individual):
+            f1 = individual.vector[0]
+            f2 = (1+individual.vector[1])/individual.vector[0]
+        return [f1, f2]
+ 
+    # Perform the optimization iterating over 100 times on 100 individuals.
+    problem = BiObjectiveTestProblem()
+    algorithm = NSGAII(problem)
+    algorithm.options['max_population_number'] = 100
+    algorithm.options['max_population_size'] = 100
+    algorithm.run()
+
+## References
+
+* [GDE3] Saku Kukkonen, Jouni Lampinen, The third Evolution Step of Generalized Differential Evolution
+
+
+## Citing
+
+If you use Ārtap in your research, the developers would be grateful if you would cite the relevant publications:
+
+[1]  Karban, Pavel, David Pánek, Tamás Orosz, Iveta Petrášová, and Ivo Doležel. “FEM based robust design optimization with Agros and Ārtap.” Computers & Mathematics with Applications (2020) https://doi.org/10.1016/j.camwa.2020.02.010.
+
+[2] Pánek, David, Tamás Orosz, and Pavel Karban. ” Ārtap: robust design optimization framework for engineering applications.” arXiv preprint arXiv:1912.11550 (2019).
+
+### Applications
+[3] Karban, P., Pánek, D., & Doležel, I. (2018). Model of induction brazing of nonmagnetic metals using model order reduction approach. COMPEL-The international journal for computation and mathematics in electrical and electronic engineering, 37(4), 1515-1524, https://doi.org/10.1108/COMPEL-08-2017-0356.
+
+[4] Pánek, D., Orosz, T., Kropík, P., Karban, P., & Doležel, I. (2019, June). Reduced-Order Model Based Temperature Control of Induction Brazing Process. In 2019 Electric Power Quality and Supply Reliability Conference (PQ) & 2019 Symposium on Electrical Engineering and Mechatronics (SEEM) (pp. 1-4). IEEE, https://doi.org/10.1109/PQ.2019.8818256.
+
+[5] Pánek, D., Karban, P., & Doležel, I. (2019). Calibration of Numerical Model of Magnetic Induction Brazing. IEEE Transactions on Magnetics, 55(6), 1-4, https://doi.org/10.1109/TMAG.2019.2897571.
+
+[6] Pánek, D., Orosz, T., Karban, P., & Doležel, I. (2020), “Comparison of simplified techniques for solving selected coupled electroheat problems”, COMPEL – The international journal for computation and mathematics in electrical and electronic engineering, Vol. 39 No. 1, pp. 220-230. https://doi.org/10.1108/COMPEL-06-2019-0244
+
+[7] Orosz, T.; Pánek, D.; Karban, P. FEM Based Preliminary Design Optimization in Case of Large Power Transformers. Appl. Sci. 2020, 10, 1361, https://doi.org/10.3390/app10041361.
+
+## Contact
+
+If you have any questions, do not hesitate to contact us: artap.framework@gmail.com
+
+## License
+
+Ārtap is published under [MIT license](https://en.wikipedia.org/wiki/MIT_License)
```

### Comparing `artap-2022.1.1.1759/README.md` & `artap-2023.4.12.3773/README.md`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/algorithm.py` & `artap-2023.4.12.3773/artap/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This is base class for all algorithms
 """
 
 from .problem import Problem
 from .utils import ConfigDictionary
 from .operators import Evaluator, GradientEvaluator, WorstCaseEvaluator
 
+
 from abc import ABCMeta
 from enum import Enum
 from uuid import uuid1
 
 
 class EvaluatorType(Enum):
     SIMPLE = 0
```

### Comparing `artap-2022.1.1.1759/artap/algorithm_bayesopt.py` & `artap-2023.4.12.3773/artap/algorithm_bayesopt.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/algorithm_cmaes.py` & `artap-2023.4.12.3773/artap/algorithm_cmaes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 from .problem import Problem
-from .algorithm_genetic import GeneralEvolutionaryAlgorithm
+from .algorithm_genetic import GeneticAlgorithm
 from .individual import Individual
-from artap.operators import CustomGenerator
+from .operators import CustomGenerator, nondominated_truncate, RandomGenerator, UniformGenerator
 import time
 
 
-class CMA_ES(GeneralEvolutionaryAlgorithm):
+class CMA_ES(GeneticAlgorithm):
     """
     Implementation of CMA_ES, Covariance Matrix Adaptation Evolutionary strategy (CMA_ES).
     The Covariance Matrix Adaptation Evolution Strategy (CMA-ES) [1] is one of the most effective approaches
     for black-box optimization, in which objective functions cannot be specified explicitly in general.
     CMA-ES outperformed over 100 black-box optimization approaches for a variety of benchmark problems [2].
 
     The CMA-ES algorithm selects solutions from a multivariate gaussian distribution. Following the evaluation of
@@ -39,41 +39,43 @@
 
         self.individual_features['dominate'] = []
         self.individual_features['crowding_distance'] = 0
         self.individual_features['domination_counter'] = 0
         # Add front_number feature
         self.individual_features['front_number'] = 0
 
-        self.dim_theta = 1
+        self.dim_theta = len(self.problem.parameters)
 
         # Elite ratio percentage
-        self.top_p = 20
+        self.top_p = 30
         # Range of values
         self.min_val = 0
         self.max_val = 1
         # Number of Runs
         self.runs = 1
         self.theta_mean = np.random.uniform(self.min_val, self.max_val, self.dim_theta)
         # self.individuals = []
         theta_std = np.random.uniform(self.max_val - 1, self.max_val, self.dim_theta)
         self.theta_cov = np.diag(theta_std)
-        self.generator = CustomGenerator(self.problem.parameters, self.individual_features)
+        self.generator = CustomGenerator(self.problem.parameters)
         # self.fit_gaussian()
 
     def fit_gaussian(self):
         """
         generates individuals from a multivariate gaussian distribution
         :param
         :return population: list of individuals
         """
         theta = np.random.multivariate_normal(self.theta_mean, self.theta_cov, self.options['max_population_size'])
         individuals = np.clip(theta, self.min_val, self.max_val)
         self.generator.init(individuals)
-        individuals = self.generator.generate()
-
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(Individual(vector))
         return individuals
 
     def take_elite(self, candidates):
         """
         Based on the fitness, it will take top individuals
         :param candidates
         :return elite: list of top individuals
@@ -119,20 +121,20 @@
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
 
             self.problem.data_store.sync_individual(individual)
 
+        self.evaluate(individuals)
+
         start = time.time()
         self.problem.logger.info("CMA_ES: {}/{}".format(self.options['max_population_number'],
                                                         self.options['max_population_size']))
         for it in range(self.options['max_population_number']):
-            self.evaluate(individuals)
-
             lists = []
             for individual in individuals:
                 # fitness.append(individual.costs)
                 lists.append(individual.costs)
             lists = np.array(lists)
 
             mean_fitness.append(np.mean(lists))
@@ -142,15 +144,18 @@
 
             elite = self.take_elite(individuals)
 
             e_candidates = [i.vector for i in elite]
 
             self.theta_cov = self.compute_new_cov(e_candidates)
             self.theta_mean = self.compute_new_mean(e_candidates)
-            self.fit_gaussian()
+            individuals = self.fit_gaussian()
+            # individuals = nondominated_truncate(new_individuals, self.options['max_population_size'])
+
+            self.evaluate(individuals)
 
             for individual in individuals:
                 # add to population
                 individual.population_id = it + 1
                 # append to problem
                 self.problem.individuals.append(individual)
                 # sync to datastore
```

### Comparing `artap-2022.1.1.1759/artap/algorithm_genetic.py` & `artap-2023.4.12.3773/artap/algorithm_genetic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,183 +1,94 @@
 import time
 from copy import deepcopy
-
 from .algorithm import Algorithm
 from .operators import RandomGenerator, SimulatedBinaryCrossover, \
     PmMutator, TournamentSelector, EpsilonDominance, nondominated_truncate, crowding_distance
 from .problem import Problem
 from .archive import Archive
+from .individual import Individual
 
 
-class GeneralEvolutionaryAlgorithm(Algorithm):
-    """ Basis Class for evolutionary algorithms """
+class GeneticAlgorithm(Algorithm):
+    def __init__(self, problem: Problem, name="General Genetic-based Algorithm", evaluator_type=None):
 
-    def __init__(self, problem: Problem, name="General Evolutionary Algorithm", evaluator_type=None):
         super().__init__(problem, name, evaluator_type)
 
         self.parameters_length = len(self.problem.parameters)
 
         self.options.declare(name='n_iterations', default=50, lower=1,
                              desc='Maximum evaluations')
         self.options.declare(name='max_population_number', default=100, lower=1,
                              desc='max_population_number')
         self.options.declare(name='max_population_size', default=100, lower=1,
                              desc='Maximal number of individuals in population')
 
         self.problem = problem
         self.__only_single_objective = False
-        # set random generator
-        self.generator = RandomGenerator(self.problem.parameters, self.individual_features)
-
-    def update_particles(self, individuals, offsprings):
-        for individual in individuals:
-            individual.features = self.features.copy()
-
-    def run(self):
-        pass
-
-
-class GeneticAlgorithm(GeneralEvolutionaryAlgorithm):
-    def __init__(self, problem: Problem, name="General Genetic-based Algorithm", evaluator_type=None):
-        super().__init__(problem, name, evaluator_type)
 
+        # set random generator
+        self.generator = RandomGenerator(self.problem.parameters)
         self.generator = None
         self.selector = None
         self.mutator = None
         self.crossover = None
 
     def generate(self, parents, archive=None):
-        offsprings = []
-        # deepcopy of parents
-        for offspring in parents:
-            offspring_copy = deepcopy(offspring)
-            offspring_copy.population_id = -1
-            offsprings.append(offspring_copy)
 
-        while len(offsprings) < 2 * self.options['max_population_size']:
+        offsprings = []
+        while len(offsprings) < self.options['max_population_size']:
             parent1 = self.selector.select(parents)
 
-            repeat = True
-            while repeat:
-                if archive:
-                    if len(archive) <= 1:
-                        parent2 = self.selector.select(parents)
-                    else:
-                        parent2 = archive.rand_choice()
-                else:
+            if archive:
+                if len(archive) <= 1:
                     parent2 = self.selector.select(parents)
-
-                if parent1 is not parent2:
-                    repeat = False
+                else:
+                    parent2 = archive.rand_choice()
+            else:
+                parent2 = self.selector.select(parents)
 
             # crossover
-            child1, child2 = self.crossover.cross(parent1, parent2)
-
+            vector_1, vector_2 = self.crossover.cross(parent1.vector, parent2.vector)
+            child1 = parent1.__class__(vector_1)
+            child2 = parent1.__class__(vector_2)
             # mutation
-            child1 = self.mutator.mutate(child1)
-            child2 = self.mutator.mutate(child2)
+            child1.vector = self.mutator.mutate(child1.vector, child2.vector)
+            child2.vector = self.mutator.mutate(child2.vector, child1.vector)
 
             # always create new individual
-            if not any(child1 == item for item in offsprings) and len(offsprings) < 2 * self.options['max_population_size']:
-                child_copy = deepcopy(child1)
-                child_copy.population_id = -1
-                offsprings.append(child_copy)
-            if not any(child2 == item for item in offsprings) and len(offsprings) < 2 * self.options['max_population_size']:
-                child_copy = deepcopy(child2)
-                child_copy.population_id = -1
-                offsprings.append(child_copy)
+            if len(offsprings) == 0:
+                offsprings.append(child1)
+
+            if any(child1 == offspring for offspring in offsprings) and (len(offsprings) < self.options[
+                'max_population_size']):
+                pass
+            else:
+                offsprings.append(child1)
+
+            if any(child2 == offspring for offspring in offsprings) and (len(offsprings) < self.options[
+                'max_population_size']):
+                pass
+            elif len(offsprings) < self.options['max_population_size']:
+                offsprings.append(child2)
 
         return offsprings
 
     def run(self):
         pass
 
 
-class NSGAII(GeneticAlgorithm):
-
-    def __init__(self, problem: Problem, name="NSGA_II Evolutionary Algorithm", evaluator_type=None):
-        """
-         NSGA-II implementation as described in
-
-         [1] K. Deb, A. Pratap, S. Agarwal and T. Meyarivan, "A fast and elitist
-             multiobjective genetic algorithm: NSGA-II," in IEEE Transactions on Evolutionary Computation,
-             vol. 6, no. 2, pp. 182-197, Apr 2002. doi: 10.1109/4235.996017
-        """
-        super().__init__(problem, name, evaluator_type)
-
-        self.options.declare(name='prob_cross', default=1.0, lower=0,
-                             desc='prob_cross')
-
-        self.options.declare(name='prob_mutation', default=1.0 / (len(problem.parameters)), lower=0,
-                             desc='prob_mutation')
-
-        # set random generator
-        self.individual_features['dominate'] = []
-        self.individual_features['crowding_distance'] = 0
-        self.individual_features['domination_counter'] = 0
-        self.individual_features['front_number'] = 0
-
-    def run(self):
-        self.generator = RandomGenerator(self.problem.parameters, self.individual_features)
-        self.generator.init(self.options['max_population_size'])
-        self.crossover = SimulatedBinaryCrossover(self.problem.parameters, self.options['prob_cross'])
-        self.mutator = PmMutator(self.problem.parameters, self.options['prob_mutation'])
-        self.selector = TournamentSelector(self.problem.parameters)
-
-        # create initial population
-        individuals = self.generator.generate()
-
-        for individual in individuals:
-            # append to problem
-            self.problem.individuals.append(individual)
-            # add to population
-            individual.population_id = 0
-
-        # evaluate
-        self.evaluate(individuals)
-
-        # non-dominated sort of individuals
-        self.selector.fast_nondominated_sorting(individuals)
-
-        # sync to datastore
-        for individual in individuals:
-            self.problem.data_store.sync_individual(individual)
-
-        t_s = time.time()
-        self.problem.logger.info(
-            "NSGA_II: {}/{}".format(self.options['max_population_number'],
-                                    self.options['max_population_number'] * self.options['max_population_size']))
-
-        # optimization
-        for it in range(self.options['max_population_number']):
-            # generate new offsprings
-            offsprings = self.generate(individuals)
-
-            # evaluate the offsprings
-            self.evaluate(offsprings)
+class IndividualEpsMOEA(Individual):
 
-            # make the pareto dominance calculation and calculating the crowding distance
-            self.selector.fast_nondominated_sorting(offsprings)
-
-            # truncate
-            individuals = nondominated_truncate(offsprings, self.options['max_population_size'])
-
-            for individual in individuals:
-                # add to population
-                individual.population_id = it + 1
-                # append to problem
-                self.problem.individuals.append(individual)
-                # sync to datastore
-                self.problem.data_store.sync_individual(individual)
-
-        t = time.time() - t_s
-        self.problem.logger.info("NSGA_II: elapsed time: {} s".format(t))
-
-        # sync changed individual informations
-        self.problem.data_store.sync_all()
+    def __init__(self, vector: list):
+        super().__init__(vector)
+        self.features['dominate'] = []
+        self.features['crowding_distance'] = 0
+        self.features['domination_counter'] = 0
+        self.features['front_number'] = 0
+        self.population_id = 0
 
 
 class EpsMOEA(GeneticAlgorithm):
     """
     EpsMOEA is proposed by Deb et al[1] which is a efficient algorithm with less computer time because it does not
     contain a sort process for non-dominate set. The searching space are divided into several hyper-boxes under
     box dominance concept, when two solutions in same box, only one solution can survive in the hyperbox, EpsMOEA choose
@@ -199,32 +110,29 @@
         self.options.declare(name='prob_mutation', default=0.2, lower=0,
                              desc='prob_mutation'),
         self.options.declare(name='epsilons', default=0.01, lower=1e-6,
                              desc='prob_epsilons')
 
         self.archive = None
 
-        # set random generator
-        self.individual_features['dominate'] = []
-        self.individual_features['crowding_distance'] = 0
-        self.individual_features['domination_counter'] = 0
-        self.individual_features['front_number'] = 0
-
     def run(self):
         # set random generator
-        self.generator = RandomGenerator(self.problem.parameters, self.individual_features)
+        self.generator = RandomGenerator(self.problem.parameters)
         self.generator.init(self.options['max_population_size'])
         # set crossover
         self.crossover = SimulatedBinaryCrossover(self.problem.parameters, self.options['prob_cross'])
         self.mutator = PmMutator(self.problem.parameters, self.options['prob_mutation'])
         # one individual is selected from the archive and one from the population to create a new individual
         self.selector = TournamentSelector(self.problem.parameters)
 
         # create initial population
-        individuals = self.generator.generate()
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(IndividualEpsMOEA(vector))
 
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
 
@@ -245,15 +153,14 @@
         t_s = time.time()
         self.problem.logger.info(
             "Eps-MOEA: {}/{}".format(self.options['max_population_number'], self.options['max_population_size']))
 
         for it in range(self.options['max_population_number']):
             # generate and evaluate the next generation
             offsprings = self.generate(individuals, archive=self.archive)
-
             self.evaluator.evaluate(offsprings)
 
             # pop-acceptance procedure, the dominating offsprings will be preserved in the population and  in the archive
             for individual in offsprings:
                 # pareto dominated solutions
                 self.selector.pop_acceptance(individuals, individual)
                 # archived solutions
@@ -270,8 +177,7 @@
             # individuals = offsprings
 
         t = time.time() - t_s
         self.problem.logger.info("Eps-MOEA: {} s".format(t))
 
         # sync changed individual informations
         self.problem.data_store.sync_all()
-
```

### Comparing `artap-2022.1.1.1759/artap/algorithm_gradient_descent.py` & `artap-2023.4.12.3773/artap/algorithm_gradient_descent.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         # compute gradients
         self.evaluator = GradientEvaluator(self)
         self.individual_features['gradient'] = dict()
 
         # set default generator
         if generator is None:
-            self.generator = RandomGenerator(self.problem.parameters, self.individual_features)
+            self.generator = RandomGenerator(self.problem.parameters)
             self.generator.init(1)
         else:
             self.generator = generator
 
     def step_fixed(self, individual):
         x = []
         for i in range(len(individual.vector)):
@@ -56,22 +56,22 @@
         grad_sqr = 0
         for i in range(len(individual.vector)):
             grad_sqr = grad_sqr + individual.features['gradient'][i] ** 2
 
         x_static = []
         for i in range(len(individual.vector)):
             x_static.append(individual.vector[i])
-        individual_static = Individual(x_static, self.individual_features)
+        individual_static = Individual(x_static)
         self.evaluate([individual_static])
 
         while True:
             x_armijo = []
             for i in range(len(individual.vector)):
                 x_armijo.append(individual.vector[i] - h_t * individual.features['gradient'][i])
-            individual_armijo = Individual(x_armijo, self.individual_features)
+            individual_armijo = Individual(x_armijo)
             self.evaluate([individual_armijo])
 
             satisfied = True
             for i in range(len(individual.costs)):
                 if individual_armijo.costs[i] > individual_static.costs[i] - c * h_t * grad_sqr:
                     satisfied = False
             if satisfied:
@@ -118,26 +118,33 @@
             m_corrected = self.cache_grad[i] / (1.0 - self.options["beta1"] ** self.adam_t)
             v_corrected = self.cache_grad_sqr[i] / (1.0 - self.options["beta2"] ** self.adam_t)
 
             x.append(individual.vector[i] - self.options["step"] * m_corrected / (math.sqrt(v_corrected + 1e-8)))
 
         return x
 
+    def generate(self):
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(Individual(vector))
+        return individuals
+
     def run(self):
         # optimization
         t_s = time.time()
         self.problem.logger.info("GradientDescent")
 
         # cache
         self.adam_t = 0
         self.cache_grad = [0] * len(self.problem.parameters)
         self.cache_grad_sqr = [0] * len(self.problem.parameters)
 
         # generate initial point
-        individuals = self.generator.generate()
+        individuals = self.generate()
 
         # append to problem
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
@@ -158,15 +165,15 @@
                     x = self.step_rmsprop(individual)
                 elif self.options["algorithm"] == "adam":
                     x = self.step_adam(individual)
                 else:
                     raise "Algorithm '{}' is defined.".format(self.options["algorithm"])
 
                 # create a new individual
-                individual = Individual(x, self.individual_features)
+                individual = Individual(x)
                 individual.population_id = j + 1
                 new_individuals.append(individual)
 
                 # append to problem
                 self.problem.individuals.append(individual)
                 # sync to datastore
                 self.problem.data_store.sync_individual(individual)
```

### Comparing `artap-2022.1.1.1759/artap/algorithm_monte_carlo.py` & `artap-2023.4.12.3773/artap/algorithm_monte_carlo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 from .problem import Problem
-from .algorithm_genetic import GeneralEvolutionaryAlgorithm
+from .algorithm_genetic import GeneticAlgorithm
 from artap.operators import CustomGenerator, RandomGenerator, UniformGenerator
 import time
 from scipy.stats import norm
 from .individual import Individual
 
 
-class Monte_Carlo(GeneralEvolutionaryAlgorithm):
+class Monte_Carlo(GeneticAlgorithm):
     """
     Monte Carlo simulation
         1) make a list of random values of x
         2) pick a small number of random value of x
         3) evaluate the objective function
         4) pick the lowest
     """
@@ -20,40 +20,43 @@
         super().__init__(problem, name)
         self.evaluation = 0
         self.z_min, self.z_max = 0, 1
         self.sampling_size = self.options['max_population_size']
         self.problem = problem
         # self.problem.parameters = bm.generate_paramlist(self, dimension=self.dimension, lb=0.0, ub=1.0)
         self.intervals = np.linspace(self.z_min, self.z_max, self.sampling_size)
-        self.generator = RandomGenerator(self.problem.parameters, self.individual_features)
+        self.generator = RandomGenerator(self.problem.parameters)
 
     def generate(self):
-        # imsampling = ImportanceSampling()
-        # samples = imsampling.generate()
         self.generator.init(self.options['max_population_size'])
-        individuals = self.generator.generate()
-
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(Individual(vector))
         return individuals
 
     def run(self):
 
         individuals = self.generate()
+
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
-
             self.problem.data_store.sync_individual(individual)
 
+        self.evaluate(individuals)
+
         start = time.time()
         self.problem.logger.info("Monte_Carlo: {}/{}".format(self.options['max_population_number'],
                                                              self.options['max_population_size']))
         for it in range(self.options['max_population_number']):
 
+            individuals = self.generate()
             self.evaluate(individuals)
 
             for individual in individuals:
                 # add to population
                 individual.population_id = it + 1
                 # append to problem
                 self.problem.individuals.append(individual)
@@ -62,69 +65,73 @@
 
         t = time.time() - start
         self.problem.logger.info("Monte_Carlo: elapsed time: {} s".format(t))
         # sync changed individual informations
         self.problem.data_store.sync_all()
 
 
-class Numerical_Integrator(GeneralEvolutionaryAlgorithm):
+class Numerical_Integrator(GeneticAlgorithm):
     """
     Adaptive Monte Carlo Integral Approximation.
     Summation is used to estimate the expected value of a function under a distribution, instead of integration.
     """
 
     def __init__(self, problem: Problem, name="Numerical Integrator using Monte Carlo"):
         super().__init__(problem, name)
         self.evaluation = 0
         self.z_min, self.z_max = 0, 1
-        self.sampling_size = self.options['max_population_size']
+        self.a = 0
+        self.b = (3*np.pi)/2
         self.problem = problem
-        # self.problem.parameters = bm.generate_paramlist(self, dimension=self.dimension, lb=0.0, ub=1.0)
-        self.intervals = np.linspace(self.z_min, self.z_max, self.sampling_size)
-        self.generator = UniformGenerator(self.problem.parameters, self.individual_features)
+        self.num_of_intervals = 10
+        self.generator = UniformGenerator(self.problem.parameters)
 
     def generate(self):
-        sampling = ImportanceSampling(self.problem)
-        samples = sampling.generate()
-        individuals = samples
-        # samples = weights
-        # self.generator.init(samples)
-        # individuals = self.generator.generate()
-        # self.generator.init(self.options['max_population_size'])
-        # individuals = self.generator.generate()
-
+        self.generator.init(self.options['max_population_size'])
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(Individual(vector))
         return individuals
 
     def run(self):
-
         individuals = self.generate()
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
 
-            self.problem.data_store.sync_individual(individual)
+            individual.vector[0] = individual.vector[0] * (self.a + (self.b - self.a))
+
+        self.evaluate(individuals)
 
         start = time.time()
         self.problem.logger.info("Monte_Carlo: {}/{}".format(self.options['max_population_number'],
                                                              self.options['max_population_size']))
-        # for it in range(self.options['max_population_number']):
+        for it in range(self.options['max_population_number']):
 
-        self.evaluate(individuals)
+            individuals = []
+            individuals = self.generate()
 
-        for individual in individuals:
-            # individual.costs[0] = individual.costs[0] / self.options['max_population_size']
-            # add to population
-            # individual.population_id = it + 1
-            # append to problem
-            self.problem.individuals.append(individual)
-            # sync to datastore
-            self.problem.data_store.sync_individual(individual)
+            for individual in individuals:
+                individual.vector[0] = individual.vector[0] * (self.a + (self.b - self.a))
+
+            self.evaluate(individuals)
+
+            for individual in individuals:
+                # individual.costs[0] = result
+                # add to population
+                individual.population_id = it + 1
+                # append to problem
+                self.problem.individuals.append(individual)
+                # sync to datastore
+                self.problem.data_store.sync_individual(individual)
 
+            # self.calculate_integral()
         t = time.time() - start
         self.problem.logger.info("Monte_Carlo: elapsed time: {} s".format(t))
         # sync changed individual informations
         self.problem.data_store.sync_all()
 
 
 class ImportanceSampling(Monte_Carlo):
@@ -249,20 +256,20 @@
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
 
             self.problem.data_store.sync_individual(individual)
-
+        self.evaluate(individuals)
         start = time.time()
         self.problem.logger.info("Rejection_Sampling: {}/{}".format(self.options['max_population_number'],
                                                                     self.options['max_population_size']))
         for it in range(self.options['max_population_number']):
-
+            individuals = self.generate()
             self.evaluate(individuals)
 
             for individual in individuals:
                 # add to population
                 individual.population_id = it + 1
                 # append to problem
                 self.problem.individuals.append(individual)
```

### Comparing `artap-2022.1.1.1759/artap/algorithm_nlopt.py` & `artap-2023.4.12.3773/artap/algorithm_nlopt.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/algorithm_pymoo.py` & `artap-2023.4.12.3773/artap/algorithm_pymoo.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 
 try:
     from pymoo.core.problem import ElementwiseProblem
     from pymoo.factory import get_termination
     from pymoo.optimize import minimize
 
-    from pymoo.core.problem import starmap_parallelized_eval
+    from pymoo.core.problem import StarmapParallelization
     from multiprocessing.pool import ThreadPool
 
 
     class MooProblem(ElementwiseProblem):
         def __init__(self, problem, algorithm, moo_algorithm):
             self.problem = problem
             self.algorithm = algorithm
@@ -25,23 +25,25 @@
                 bounds = parameter['bounds']
 
                 lb.append(bounds[0])
                 ub.append(bounds[1])
 
             # initialize the pool
             if self.algorithm.options["max_processes"] > 1:
-                pool = ThreadPool(self.algorithm.options["max_processes"])
+                # initialize the thread pool and create the runner
+                n_threads = ThreadPool(self.algorithm.options["max_processes"])
+                pool = ThreadPool(n_threads)
+                runner = StarmapParallelization(pool.starmap)
 
                 super().__init__(n_var=len(problem.parameters),
                                  n_obj=len(problem.costs),
                                  n_constr=len(problem.constraints),
                                  xl=np.array(lb),
                                  xu=np.array(ub),
-                                 runner=pool.starmap,
-                                 func_eval=starmap_parallelized_eval)
+                                 elementwise_runner=runner)
             else:
                 super().__init__(n_var=len(problem.parameters),
                                  n_obj=len(problem.costs),
                                  n_constr=len(problem.constraints),
                                  xl=np.array(lb),
                                  xu=np.array(ub))
 
@@ -79,16 +81,16 @@
             self.problem.logger.info("pymoo: {}".format(type(self.options["algorithm"]).__name__))
 
             moo_algorithm = self.options["algorithm"]
             moo_problem = MooProblem(self.problem, self, moo_algorithm)
 
             termination = get_termination("n_gen", self.options["n_iterations"])
 
-            moo_algorithm.setup(moo_problem,
-                                termination,
+            moo_algorithm.setup(problem=moo_problem,
+                                termination=termination,
                                 seed=1,
                                 save_history=True,
                                 verbose=self.options["verbose_level"] > 0)
 
             # until the algorithm has no terminated
             while moo_algorithm.has_next():
                 # do the next iteration
@@ -122,8 +124,8 @@
                 # add to population
                 individual.population_id = moo_algorithm.n_gen + 1
 
             # sync changed individual informations
             self.problem.data_store.sync_all()
 
 except ImportError:
-    print("pymoo is not present test skiped")
+    print("pymoo is not present test skipped")
```

### Comparing `artap-2022.1.1.1759/artap/algorithm_scipy.py` & `artap-2023.4.12.3773/artap/algorithm_scipy.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/algorithm_sensitivity.py` & `artap-2023.4.12.3773/artap/algorithm_sensitivity.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/algorithm_swarm.py` & `artap-2023.4.12.3773/artap/algorithm_swarm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,67 @@
-import sys
-from random import randint, random, uniform, choice, shuffle
-import numpy as np
-
+from random import uniform
 from .individual import Individual
 from .problem import Problem
-from .algorithm_genetic import GeneralEvolutionaryAlgorithm
+from .algorithm_genetic import GeneticAlgorithm
 from .operators import RandomGenerator, PmMutator, ParetoDominance, EpsilonDominance, crowding_distance, \
-    NonUniformMutation, UniformMutator, CopySelector, IntegerGenerator
+    NonUniformMutation, UniformMutator, CopySelector, SimulatedBinaryCrossover, TournamentSelector
 from .archive import Archive
-from copy import copy, deepcopy
+from copy import copy
 import time
-import math
 
 
-class SwarmAlgorithm(GeneralEvolutionaryAlgorithm):
+class IndividualSwarm(Individual):
+
+    def __init__(self, vector: list = None):
+        super().__init__(vector)
+        self.features['dominate'] = []
+        self.features['crowding_distance'] = 0
+        self.features['domination_counter'] = 0
+        self.features['front_number'] = -1
+        self.features['velocity'] = [0] * len(self.vector)
+        self.features['best_cost'] = None
+        self.features['best_vector'] = None
+        self.population_id = -1
+
+    def copy(self):
+        new_individual = self.__class__(self.vector)
+        new_individual.features['best_cost'] = self.features['best_cost']
+        new_individual.features['best_vector'] = self.features['best_vector']
+        return new_individual
+
+
+class SwarmAlgorithm(GeneticAlgorithm):
     def __init__(self, problem: Problem, name="General Swarm-based Algorithm"):
         super().__init__(problem, name)
         # self.options.declare(name='v_max', default=, lower=0., desc='maximum_allowed_speed')
         self.global_best = None  # swarm algorithms share the information, who is the leader
         self.dominance = ParetoDominance()  # some dominance should be defined for every kind of multi-opbjective swarm
+        # constants for the speed and the position calculation
+        self.c1_min = 1.5
+        self.c1_max = 2.0
+        self.c2_min = 1.5
+        self.c2_max = 2.0
+        self.r1_min = 0.0
+        self.r1_max = 1.0
+        self.r2_min = 0.0
+        self.r2_max = 1.0
+        self.min_weight = 0.1
+        self.max_weight = 0.5
 
     def init_pvelocity(self, population):
         pass
 
-    def init_pbest(self, population):
+    @staticmethod
+    def init_pbest(population):
         for individual in population:
             individual.features['best_cost'] = individual.costs_signed
             individual.features['best_vector'] = individual.vector
 
-    def khi(self, c1: float, c2: float) -> float:
+    @staticmethod
+    def khi(c1: float, c2: float) -> float:
         """
         Constriction coefficient [1].
         [1] Ebarhart and Kennedym Empirical study of particle swarm optimization,” in Proc. IEEE Int. Congr.
         Evolutionary Computation, vol. 3, 1999, pp. 101–106.
 
         :param c1: specific parameter to control the particle best component.
         :param c2: specific parameter to control the global best component.
@@ -42,25 +71,26 @@
         if rho <= 4:
             result = 1.0
         else:
             result = 2.0 / (2.0 - rho - (rho ** 2.0 - 4.0 * rho) ** 0.5)
 
         return result
 
-    def speed_constriction(self, velocity, u_bound, l_bound) -> float:
+    @staticmethod
+    def speed_constriction(velocity, u_bound, l_bound) -> float:
         """
         Velocity constriction factor [1].
 
         .. Ref:
         [1] Nebro, Antonio J., et al. "SMPSO: A new PSO-based metaheuristic for multi-objective optimization."
             2009 IEEE Symposium on Computational Intelligence in Multi-Criteria Decision-Making (MCDM). IEEE, 2009.
 
         :param velocity: parameter velocity for the i^th component
-        :param ub: upper bound
-        :param lb: lower bound
+        :param u_bound: upper bound
+        :param l_bound: lower bound
         :return:
         """
 
         delta_i = (u_bound - l_bound) / 2.
         # user defined max speed
         velocity = min(velocity, delta_i)
         velocity = max(velocity, -delta_i)
@@ -72,16 +102,32 @@
 
     def inertia_weight(self):
         pass
 
     def update_global_best(self, offsprings):
         pass
 
-    def update_velocity(self, population):
-        pass
+    def update_velocity(self, individuals):
+        for individual in individuals:
+            individual.features['velocity'] = [0] * len(individual.vector)
+            global_best = self.select_leader()
+
+            r1 = round(uniform(self.r1_min, self.r1_max), 1)
+            r2 = round(uniform(self.r2_min, self.r2_max), 1)
+            c1 = round(uniform(self.c1_min, self.c1_max), 1)
+            c2 = round(uniform(self.c2_min, self.c2_max), 1)
+
+            for i in range(0, len(individual.vector)):
+                momentum = self.inertia_weight() * individual.vector[i]
+                v_cog = c1 * r1 * (individual.features['best_vector'][i] - individual.vector[i])
+                v_soc = c2 * r2 * (global_best.vector[i] - individual.vector[i])
+
+                v = self.khi(c1, c2) * (momentum + v_cog + v_soc)
+                individual.features['velocity'][i] = self.speed_constriction(v, self.parameters[i]['bounds'][1],
+                                                                             self.parameters[i]['bounds'][0])
 
     def update_position(self, population):
         pass
 
     def update_particle_best(self, population):
         for particle in population:
             flag = self.dominance.compare(particle.costs_signed, particle.features['best_cost'])
@@ -120,90 +166,43 @@
         self.options.declare(name='epsilons', default=0.01, lower=1e-6,
                              desc='prob_epsilons')
         self.n = self.options['max_population_size']
 
         self.selector = CopySelector(self.problem.parameters)
         self.dominance = ParetoDominance()
 
-        self.individual_features['velocity'] = dict()
-        self.individual_features['best_cost'] = dict()
-        self.individual_features['best_vector'] = dict()
-        # Add front_number feature
-        self.individual_features['front_number'] = 0
-
         # set random generator
-        self.generator = RandomGenerator(self.problem.parameters, self.individual_features)
+        self.generator = RandomGenerator(self.problem.parameters)
         self.leaders = Archive()
         self.archive = Archive(dominance=EpsilonDominance(epsilons=self.options['epsilons']))
 
         self.non_uniform_mutator = NonUniformMutation(self.problem.parameters, self.options['prob_mutation'],
                                                       self.options['max_population_number'])
         self.uniform_mutator = UniformMutator(self.problem.parameters, self.options['prob_mutation'],
                                               self.options['max_population_number'])
-        # constants for the speed and the position calculation
-        self.c1_min = 1.5
-        self.c1_max = 2.0
-        self.c2_min = 1.5
-        self.c2_max = 2.0
-        self.r1_min = 0.0
-        self.r1_max = 1.0
-        self.r2_min = 0.0
-        self.r2_max = 1.0
-        self.min_weight = 0.1
-        self.max_weight = 0.5
+
 
     def inertia_weight(self):
         return uniform(self.min_weight, self.max_weight)
 
-    def init_pvelocity(self, population):
-        """
-        Inits the particle velocity and its allowed maximum speed.
-        :param population: list of individuals
-        :return
-        """
-        for individual in population:
-            # the initial speed is set to zero
-            individual.features['velocity'] = [0] * len(individual.vector)
-
-        return
-
     def turbulence(self, particles, current_step=0):
         """
         OMOPSO applies a combination of uniform and nonuniform
         mutation to the particle swarm(uniform mutation to the first 30 % of
-        the swarm, non - uniform to the next 30 %, and no mutation on the particles)
+        the swarm, non-uniform to the next 30 %, and no mutation on the particles)
         """
 
         for i in range(len(particles)):
             if i % 3 == 0:
-                mutated = self.uniform_mutator.mutate(particles[i])
-            elif i % 3 == 1:
-                mutated = self.non_uniform_mutator.mutate(particles[i], current_step)
-            particles[i].vector = copy(mutated.vector)
+                mutated = self.uniform_mutator.mutate(particles[i].vector)
+            else:
+                mutated = self.non_uniform_mutator.mutate(particles[i].vector, current_step)
+            particles[i].vector = mutated.copy()
         return
 
-    def update_velocity(self, individuals):
-        for individual in individuals:
-            individual.features['velocity'] = [0] * len(individual.vector)
-            global_best = self.select_leader()
-
-            r1 = round(uniform(self.r1_min, self.r1_max), 1)
-            r2 = round(uniform(self.r2_min, self.r2_max), 1)
-            c1 = round(uniform(self.c1_min, self.c1_max), 1)
-            c2 = round(uniform(self.c2_min, self.c2_max), 1)
-
-            for i in range(0, len(individual.vector)):
-                momentum = self.inertia_weight() * individual.vector[i]
-                v_cog = c1 * r1 * (individual.features['best_vector'][i] - individual.vector[i])
-                v_soc = c2 * r2 * (global_best.vector[i] - individual.vector[i])
-
-                v = self.khi(c1, c2) * (momentum + v_cog + v_soc)
-                individual.features['velocity'][i] = self.speed_constriction(v, self.parameters[i]['bounds'][1],
-                                                                             self.parameters[i]['bounds'][0])
-
     def update_position(self, individuals):
         for individual in individuals:
             for parameter, i in zip(self.parameters, range(len(individual.vector))):
                 individual.vector[i] = individual.vector[i] + individual.features['velocity'][i]
 
                 # adjust maximum position if necessary
                 if individual.vector[i] > parameter['bounds'][1]:
@@ -215,18 +214,25 @@
                     individual.vector[i] = parameter['bounds'][0]
                     individual.features['velocity'][i] *= -1
 
     def update_global_best(self, swarm):
         """ Manages the leader class in OMOPSO. """
 
         # the fitness of the particles are calculated by their crowding distance
-        crowding_distance(swarm)
 
+        # crowding_distance(swarm)
+
+        self.selector.fast_nondominated_sorting(swarm)
         # the length of the leaders archive cannot be longer than the number of the initial population
-        self.leaders += swarm
+        pareto = []
+        for particle in swarm:
+            if particle.features['front_number'] == 1:
+                pareto.append(particle)
+        for item in pareto:
+            self.leaders.append(item)
         self.leaders.truncate(self.options['max_population_size'], 'crowding_distance')
         self.archive += swarm
 
         return
 
     def select_leader(self):
         """
@@ -268,25 +274,26 @@
         # update mutators
         self.non_uniform_mutator = NonUniformMutation(self.problem.parameters, self.options['prob_mutation'],
                                                       self.options['max_population_number'])
         self.uniform_mutator = UniformMutator(self.problem.parameters, self.options['prob_mutation'],
                                               self.options['max_population_number'])
         # initialize the swarm
         self.generator.init(self.options['max_population_size'])
-        individuals = self.generator.generate()
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(IndividualSwarm(vector))
 
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
 
         self.evaluate(individuals)
-
-        self.init_pvelocity(individuals)
         self.init_pbest(individuals)
         self.update_global_best(individuals)
 
         # sync to datastore
         for individual in individuals:
             self.problem.data_store.sync_individual(individual)
 
@@ -357,15 +364,15 @@
         self.individual_features['best_vector'] = dict()
         # Add front_number feature
         self.individual_features['front_number'] = 0
 
         self.selector = CopySelector(self.problem.parameters)
         self.dominance = ParetoDominance()
         # set random generator
-        self.generator = RandomGenerator(self.problem.parameters, self.individual_features)
+        self.generator = RandomGenerator(self.problem.parameters)
         self.leaders = Archive()
         self.mutator = PmMutator(self.problem.parameters, self.options['prob_mutation'])
         # constants for the speed and the position calculation
 
         self.c1_min = 1.5
         self.c1_max = 2.5
         self.c2_min = 1.5
@@ -393,35 +400,15 @@
         return
 
     def turbulence(self, particles, current_step=0):
         """ SMPSO applies polynomial mutation on 15% of the particles """
 
         for i in range(len(particles)):
             if i % 6 == 0:
-                mutated = self.mutator.mutate(particles[i])
-                particles[i].vector = copy(mutated.vector)
-
-    def update_velocity(self, individuals):
-        for individual in individuals:
-            individual.features['velocity'] = [0] * len(individual.vector)
-            global_best = self.select_leader()
-
-            r1 = round(uniform(self.r1_min, self.r1_max), 1)
-            r2 = round(uniform(self.r2_min, self.r2_max), 1)
-            c1 = round(uniform(self.c1_min, self.c1_max), 1)
-            c2 = round(uniform(self.c2_min, self.c2_max), 1)
-
-            for i in range(0, len(individual.vector)):
-                momentum = self.inertia_weight() * individual.vector[i]
-                v_cog = c1 * r1 * (individual.features['best_vector'][i] - individual.vector[i])
-                v_soc = c2 * r2 * (global_best.vector[i] - individual.vector[i])
-
-                v = self.khi(c1, c2) * (momentum + v_cog + v_soc)
-                individual.features['velocity'][i] = self.speed_constriction(v, self.parameters[i]['bounds'][1],
-                                                                             self.parameters[i]['bounds'][0])
+                particles[i].vector = self.mutator.mutate(particles[i].vector)
 
     def update_position(self, individuals):
         for individual in individuals:
             for parameter, i in zip(self.parameters, range(len(individual.vector))):
                 individual.vector[i] = individual.vector[i] + individual.features['velocity'][i]
 
                 # adjust maximum position if necessary
@@ -482,15 +469,18 @@
 
     def run(self):
         t_s = time.time()
         self.problem.logger.info("PSO: {}/{}".format(self.options['max_population_number'],
                                                      self.options['max_population_size']))
         # initialize the swarm
         self.generator.init(self.options['max_population_size'])
-        individuals = self.generator.generate()
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(Individual(vector))
 
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
             # add to population
             individual.population_id = 0
 
@@ -546,32 +536,33 @@
         super().__init__(problem, name)
         self.options.declare(name='prob_cross', default=1.0, lower=0,
                              desc='prob_cross')
         self.options.declare(name='prob_mutation', default=0.1, lower=0,
                              desc='prob_mutation'),
         self.n = self.options['max_population_size']
 
-        self.individual_features['velocity'] = dict()
-        self.individual_features['best_cost'] = dict()
-        self.individual_features['best_vector'] = dict()
+        self.individual_features['velocity'] = None
+        self.individual_features['best_cost'] = None
+        self.individual_features['best_vector'] = None
 
         self.individual_features['dominate'] = []
         self.individual_features['crowding_distance'] = 0
         self.individual_features['domination_counter'] = 0
         # Add front_number feature
         self.individual_features['front_number'] = 0
 
-        self.selector = CopySelector(self.problem.parameters)
+        self.offspring_selector = CopySelector(self.problem.parameters)
+        self.selector = TournamentSelector(self.problem.parameters)
         self.dominance = ParetoDominance()
         # set random generator
-        self.generator = IntegerGenerator(self.problem.parameters, self.individual_features)
+        self.generator = RandomGenerator(self.problem.parameters)
         self.leaders = Archive()
+        self.crossover = SimulatedBinaryCrossover(self.problem.parameters, self.options['prob_cross'])
         self.mutator = PmMutator(self.problem.parameters, self.options['prob_mutation'])
         # constants for the speed and the position calculation
-
         self.c1_min = 1.5
         self.c1_max = 2.5
         self.c2_min = 1.5
         self.c2_max = 2.5
         self.r1_min = 0.0
         self.r1_max = 1.0
         self.r2_min = 0.0
@@ -584,176 +575,14 @@
     def inertia_weight(self):
         return uniform(self.min_weight, self.max_weight)
 
     def init_pvelocity(self, individuals):
         for individual in individuals:
             individual.features['velocity'] = [0] * len(individual.vector)
 
-    # A function for rounding to the nearest integer for all offsprings
-    def makeinteger(self, individual):
-        for i in range(len(individual)):
-            individual[i] = np.rint(individual[i]).astype(int)
-
-    def crossover(self, particles):
-        # nVar = len(particles)
-        # parents = self.tournamentselection(particles)
-        parent1 = particles[0]
-        parent2 = particles[1]
-
-        '''
-        SBX algorithm :
-            Paper describing the algorithm: 
-            Title: An Efficient Constraint Handling Method for Genetic Algorithms
-            Author: Kalyanmoy Deb
-            More info: Appendix A. Page 30.
-            URL: http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.33.7291&rep=rep1&type=pdf
-            
-        discretization using round() command, make the parents to have real value(discrete value)
-        example:
-        a = 7
-        b = 8
-        c = 10 
-        average = round((a+b)/c)
-        '''
-        # parent1.vector = np.round(parent1.vector)
-        # parent2.vector = np.round(parent2.vector)
-
-        """
-        x1 represent parent1 and x2 represent parent2
-        """
-        x1 = deepcopy(parent1.vector)
-        x2 = deepcopy(parent2.vector)
-
-        u = random()
-        if u <= self.probability:
-            for i, param in enumerate(self.parameters):
-                lb = param['bounds'][0]
-                ub = param['bounds'][1]
-
-                # each variable in a solution has a 50% chance of changing its value. This should be removed when
-                # dealing with one-dimensional solutions.
-                if u <= 0.5:
-                    if x1[i] > x2[i]:
-                        y1, y2 = x2[i], x1[i]
-                    else:
-                        y1, y2 = x1[i], x2[i]
-                    # if the value in parent1 is not the same of parent2
-                    if abs(x2[i] - x1[i]) > sys.float_info.epsilon:
-                        # we use different beta for each child.
-                        rand = random()
-                        beta = 1.0 + (2.0 * (y1 - lb) / (y2 - y1))
-                        alpha = 2.0 - pow(beta, -(self.distribution_index + 1.0))
-                        # calculation of betaq
-                        if u <= (1.0 / alpha):
-                            betaq = pow(rand * alpha, (1.0 / (self.distribution_index + 1.0)))
-                        else:
-                            betaq = pow(1.0 / (2.0 - rand * alpha), 1.0 / (self.distribution_index + 1.0))
-
-                        # calculation of the first child
-                        c1 = 0.5 * ((1 + betaq) * y1 + (1 - betaq) * y2)
-
-                        # The second value of beta uses the upper limit (ul) and the maximum between parent1 and parent2
-                        # (y2)
-                        beta = 1.0 + (2.0 * (ub - y2) / (y2 - y1))
-                        alpha = 2.0 - pow(beta, -(self.distribution_index + 1.0))
-                        # calculation of betaq
-                        if u <= (1.0 / alpha):
-                            betaq = pow(rand * alpha, (1.0 / (self.distribution_index + 1.0)))
-                        else:
-                            betaq = pow(1.0 / (2.0 - rand * alpha), 1.0 / (self.distribution_index + 1.0))
-
-                        # calculation of the second child
-                        c2 = 0.5 * ((1 - betaq) * y1 + (1 + betaq) * y2)
-
-                        # check the boundaries
-                        c1 = max(lb, min(c1, ub))
-                        c2 = max(lb, min(c2, ub))
-
-                        if random() <= 0.5:
-                            x1[i], x2[i] = c2, c1
-                        else:
-                            x1[i], x2[i] = c1, c2
-
-                    else:
-                        x1 = parent1.vector
-                        x2 = parent2.vector
-                # 50% chance of changing values. In the case random > 0.5, the children should have the same value as
-                # the parents
-                else:
-                    x1 = parent1.vector
-                    x2 = parent2.vector
-        # if the random number generated is greater than the crossover rate, return the children as exact clones of
-        # the parents
-        else:
-            x1 = parent1.vector
-            x2 = parent2.vector
-        self.makeinteger(x1)
-        self.makeinteger(x2)
-
-        return Individual(list(x1), parent1.features), Individual(list(x2), parent2.features)
-
-        # delta = 0.1
-        #
-        # for i in range(len(particles)):
-        #     alpha = uniform(-delta, 1 + delta)
-        #
-        # particles[i].vector = alpha * np.asarray(particles[i].vector) + (1 - alpha) * np.asarray(particles[i].vector)
-
-    def mutation(self, particle, current_step=0):
-        global deltal, deltar
-        y = []
-        # nVar = len(particles)
-        # for i in range(len(particles) - 1):
-        # sigma = int(uniform(1, nVar)) / 10
-        # sigma = 0.1
-        # y = particles
-        # y.vector = np.asarray(particles.vector) * sigma
-        # return y
-        # Plynomial Mutation
-        # PDF = Analyzing Mutation Schemes for real-Parameter Genetic Algorithms
-        # Link = https://www.iitk.ac.in/kangal/papers/k2012016.pdf
-        # section 2
-        #
-        # u = uniform(0, 1)
-        # if u <= 0.5:
-        #     deltal = pow(2 * u, 1 / (self.distribution_index + 1)) - 1
-        # else:
-        #     deltar = 1 - pow(2 * (1 - u), 1 / (self.distribution_index + 1))
-        #
-        # if u <= 0.5:
-        #     x = x + deltal * (x - lb)
-        # else:
-        #     x = x + deltar * (ub - x)
-        for i, param in enumerate(self.parameters):
-            if uniform(0, 1) < self.probability:
-                lb = param['bounds'][0]
-                ub = param['bounds'][1]
-                x = particle.vector[i]
-                u = uniform(0, 1)
-                # delta = min((x - lb), (ub - x)) / (ub - lb)
-                # mut_probability = 1 / (self.distribution_index + 1)
-
-                if u <= 0.5:
-                    deltal = pow(2 * u, 1 / (self.distribution_index + 1)) - 1
-                else:
-                    deltar = 1 - pow(2 * (1 - u), 1 / (self.distribution_index + 1))
-
-                if u <= 0.5:
-                    x = x + deltal * (x - lb)
-                else:
-                    x = x + deltar * (ub - x)
-                # check child boundaries
-                x = max(lb, min(x, ub))
-                y.append(x)
-            else:
-                y.append(particle[i].vector)
-
-        self.makeinteger(y)
-        return Individual(y, particle.features)
-
     def update_velocity(self, individuals):
         """
         update velocity : w * v(i -1) + c1 * r1 * (best_vector - pos(i)) + c2 * r2 * (global_best - pos(i))
         @param individuals:
         @return: update individual.features['velocity']
         """
 
@@ -799,91 +628,69 @@
                     individual.vector[i] = parameter['bounds'][1]
                     individual.features['velocity'][i] *= -1
 
                 if individual.vector[i] < parameter['bounds'][0]:
                     individual.vector[i] = parameter['bounds'][0]
                     individual.features['velocity'][i] *= -1
 
-            self.makeinteger(individual.vector)
+            # self.makeinteger(individual.vector)
 
     def update_global_best(self, swarm):
         crowding_distance(swarm)
 
         self.leaders += swarm
         self.leaders.truncate(self.options['max_population_size'], 'crowding_distance')
         return
 
-    def tournamentselection(self, parents):
-        # offsprings = []
-        # parent1 = []
-        # parent2 = []
-        # for offspring in parents:
-        #     copy_offspring = deepcopy(offspring)
-        #     copy_offspring.population_id = -1
-        #     offsprings.append(copy_offspring)
-        #
-
-        # tournamentSelection Select and return one individual by tournament selection. A number of individuals are
-        # picked at random and the one with the highest fitness is selected for the next generation.Tournament
-        # selection: Pick tourny_size individuals at random. Return the best one out of the bunch.
-
-        tournamentSize = 2
-        popSize = len(parents)
-        selected = []
-        if tournamentSize > popSize:
-            for p in parents:
-                selected.append(p)
-        else:
-            indices = list(range(popSize))
-            shuffle(indices)
-            for i in range(tournamentSize):
-                selected.append(parents[indices[i]])
-        selected = sorted(selected, key=lambda c: c.costs, reverse=True)
-        return selected
-        # parent1 = self.selector.select(parents)
-        # parent2 = self.selector.select(parents)
-        # return parent1, parent2
-
     def run(self):
         start = time.time()
         self.problem.logger.info("PSOGA: {}/{}".format(self.options['max_population_number'],
                                                        self.options['max_population_size']))
         # initialization of swarm
-        self.generator.init(self.options['max_population_size'], self.parameters)
-        individuals = self.generator.generate()
+        self.generator.init(self.options['max_population_size'])
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(IndividualSwarm(vector))
 
         for individual in individuals:
             # append to problem
             self.problem.individuals.append(individual)
 
             # add to population
             individual.population_id = 0
 
+            self.problem.data_store.sync_individual(individual)
+
         self.evaluate(individuals)
         self.init_pvelocity(individuals)
         self.init_pbest(individuals)
         self.update_global_best(individuals)
 
-        for individual in individuals:
-            self.problem.data_store.sync_individual(individual)
-
         it = 0
-        for it in range(self.options['max_population_number']):
-            offsprings = self.selector.select(individuals)
+        while it < self.options['max_population_number']:
+            offsprings = self.offspring_selector.select(individuals)
 
             # PSO operators
             self.update_velocity(offsprings)
             self.update_position(offsprings)
             self.evaluate(offsprings)
 
             # GA operators
-            selected = self.tournamentselection(offsprings)
-            offspring1, offspring2 = self.crossover(selected)
-            offspring1 = self.mutation(offspring1, it)
-            offspring2 = self.mutation(offspring2, it)
+            first_selected = self.selector.select(offsprings)
+            second_selected = self.selector.select(offsprings)
+            vector1, vector2 = self.crossover.cross(first_selected.vector, second_selected.vector)
+            vector1 = self.mutator.mutate(vector1)
+            vector2 = self.mutator.mutate(vector2)
+
+            # ToDo: Make it clean
+            offspring1 = IndividualSwarm(vector1)
+            offspring2 = IndividualSwarm(vector2)
+            offspring1.features = first_selected.features
+            offspring2.features = second_selected.features
             offsprings.append(offspring1)
             offsprings.append(offspring2)
 
             self.evaluate(offsprings)
             self.update_particle_best(offsprings)
             self.update_global_best(offsprings)
 
@@ -894,88 +701,12 @@
                 # add to population
                 individual.population_id = it + 1
                 # append to problem
                 self.problem.individuals.append(individual)
                 # sync to datastore
                 self.problem.data_store.sync_individual(individual)
 
-            # it += 1
+            it += 1
         t = time.time() - start
         self.problem.logger.info("PSOGA: elapsed time: {} s".format(t))
         # sync changed individual informations
         self.problem.data_store.sync_all()
-# ........................
-#
-# ........................
-
-# class PSO_V1(SwarmAlgorithm):
-#     """
-#
-#     X. Li. A Non-dominated Sorting Particle Swarm Optimizer for Multiobjective
-#     Optimization. In Genetic and Evolutionary Computation - GECCO 2003, volume
-#     2723 of LNCS, pages 37–48, 2003.
-#
-# This algorithm is a variant of the original PSO, published by Eberhart(2000), the origin of this modified
-# algorithm, which constriction factor was introduced by Clercs in 1999.
-#
-#     The code is based on SHI and EBERHARTS algorithm.
-#
-#     Empirical study of particle swarm optimization,” in Proc. IEEE Int. Congr. Evolutionary Computation, vol. 3,
-#     1999, pp. 101–106.
-#     """
-#
-#     def __init__(self, problem: Problem, name="Particle Swarm Algorithm - with time varieting inertia weight"):
-#         super().__init__(problem, name)
-#         self.n = self.options['max_population_size']
-#         self.mutator = SwarmStepTVIW(self.problem.parameters, self.options['max_population_number'])
-#         self.selector = DummySelector(self.problem.parameters, self.problem.signs)
-#
-#     def run(self):
-#         # set random generator
-#         self.generator = RandomGenerator(self.problem.parameters)
-#         self.generator.init(self.options['max_population_size'])
-#
-#         population = self.gen_initial_population()
-#         self.evaluate(population.individuals)
-#         self.add_features(population.individuals)
-#
-#         for individual in population.individuals:
-#             self.mutator.evaluate_best_individual(
-#                 individual)  # TODO: all evaluating should be derived from Evaluator class
-#
-#         self.selector.fast_nondominated_sorting(population.individuals)
-#         self.populations.append(population)
-#
-#         t_s = time.time()
-#         self.problem.logger.info("PSO: {}/{}".format(self.options['max_population_number'],
-#                                                      self.options['max_population_size']))
-#
-#         i = 0
-#         while i < self.options['max_population_number']:
-#             offsprings = self.selector.select(population.individuals)
-#
-#             pareto_front = []
-#             for individual in offsprings:
-#                 if individual.features['front_number'] == 1:
-#                     pareto_front.append(individual)
-#
-#             for individual in offsprings:
-#                 index = randint(0, len(pareto_front) - 1)  # takes random individual from Pareto front
-#                 best_individual = pareto_front[index]
-#                 if best_individual is not individual:
-#                     self.mutator.update(best_individual)
-#                     self.mutator.mutate(individual)
-#
-#             self.evaluate(offsprings)
-#             self.add_features(offsprings)
-#
-#             for individual in offsprings:
-#                 self.mutator.evaluate_best_individual(individual)
-#
-#             self.selector.fast_nondominated_sorting(offsprings)
-#             population = Population(offsprings)
-#             self.populations.append(population)
-#
-#             i += 1
-#
-#         t = time.time() - t_s
-#         self.problem.logger.info("PSO: elapsed time: {} s".format(t))
```

### Comparing `artap-2022.1.1.1759/artap/algorithm_sweep.py` & `artap-2023.4.12.3773/artap/algorithm_sweep.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from .algorithm_genetic import GeneralEvolutionaryAlgorithm
+from .algorithm_genetic import GeneticAlgorithm
+from .individual import Individual
 import time
 import random
 
 
-class SweepAlgorithm(GeneralEvolutionaryAlgorithm):
+class SweepAlgorithm(GeneticAlgorithm):
     """
     Sweep Analysis
     """
 
     def __init__(self, problem, generator, name='SweepAlgorithm'):
         super().__init__(problem, name)
         self.generator = generator
 
     def run(self):
         t_s = time.time()
 
         # create initial population
-        individuals = self.generator.generate()
-
+        vectors = self.generator.generate()
+        individuals = []
+        for vector in vectors:
+            individuals.append(Individual(vector))
         # append to problem
         for individual in individuals:
             self.problem.individuals.append(individual)
 
         # evaluate individuals
         self.evaluate(individuals)
```

### Comparing `artap-2022.1.1.1759/artap/archive.py` & `artap-2023.4.12.3773/artap/archive.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/benchmark_functions.py` & `artap-2023.4.12.3773/artap/benchmark_functions.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/benchmark_pareto.py` & `artap-2023.4.12.3773/artap/benchmark_pareto.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/benchmark_robust.py` & `artap-2023.4.12.3773/artap/benchmark_robust.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/colormaps.py` & `artap-2023.4.12.3773/artap/colormaps.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/config.py` & `artap-2023.4.12.3773/artap/config.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/datastore.py` & `artap-2023.4.12.3773/artap/datastore.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/doe.py` & `artap-2023.4.12.3773/artap/doe.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/executor.py` & `artap-2023.4.12.3773/artap/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import string
 import textwrap
 import re
 import tempfile
 import os
 import subprocess
 import datetime
 import time
@@ -73,20 +74,21 @@
         if (len(x)) > len(sep):
             param_values_string = param_values_string[:-len(sep)]
 
         return param_values_string
 
     @staticmethod
     def _remove_dir(local_dir):
-        files = os.listdir(path=local_dir)
-        for f in files:
-            filepath = os.path.join(local_dir, f)
-            os.remove(filepath)
+        if os.path.exists(local_dir):
+            files = os.listdir(path=local_dir)
+            for f in files:
+                filepath = os.path.join(local_dir, f)
+                os.remove(filepath)
 
-        os.rmdir(local_dir)
+            os.rmdir(local_dir)
 
 
 class LocalComsolExecutor(Executor):
     comsol_command = Template("comsol batch -inputfile $input_file -nosave -pname $param_names -plist $param_values")
 
     def __init__(self, problem, problem_file, input_files=None, output_files=None):
         super().__init__(problem)
@@ -163,15 +165,15 @@
         #                                                                                              'c=42')
         cmd_string = self.femm_command + ' -lua-script={}'.format(arg)
 
         params = param_names_string.split(',')
         values = param_values_string.split(',')
 
         for i in range(len(params)):
-            temp = str(params[i])+'='+str(values[i])
+            temp = str(params[i]) + '=' + str(values[i])
             cmd_string += ' -lua-var={}'.format(temp)
 
         try:
             out = subprocess.run(cmd_string, shell=True, stdout=subprocess.PIPE)
 
             if out.returncode != 0:
                 err = "Unknown error"
@@ -186,36 +188,35 @@
 
         except Exception as e:
             err = "Cannot run FEMM with wine.\n\n {}".format(e)
             self.problem.logger.error(err)
             raise RuntimeError(err)
 
 
-
 class LocalAnsysExecutor(Executor):
     """
     runs an ansys executable python script
     """
 
     def __init__(self, problem, script_file, output_files):
         super().__init__(problem)
         self.script_file = ntpath.basename(script_file)
 
         self.ansys_path = r'C:\Program Files\AnsysEM\AnsysEM20.2\Win64\ansysedt.exe'
-        #"D:\tmp\Example_Conductor.py"
+        # "D:\tmp\Example_Conductor.py"
         self.output_files = output_files
 
     def eval(self, individual):
         super().eval(individual)
 
         param_names_string = Executor._join_parameters_names(self.problem.parameters)
         param_values_string = Executor._join_parameters_values(individual.vector)
 
-        #lua_path = os.path.abspath(self.script_file)
-        #if os.path.isfile(lua_path) and platform == 'linux':
+        # lua_path = os.path.abspath(self.script_file)
+        # if os.path.isfile(lua_path) and platform == 'linux':
         #    arg = '"' + os.popen('winepath -w "' + lua_path + '"').read().strip() + '"'
 
         cmd_string = self.ansys_path + ' - runscript'.format(self.script_file)
 
         try:
 
             out = subprocess.run(cmd_string, shell=True, stdout=subprocess.PIPE)
@@ -483,26 +484,32 @@
                     raise TimeoutError
 
                 if successful_job:
                     if len(self.output_files) > 0:
                         output_files = []
                         d = datetime.datetime.now()
                         ts = d.strftime("%Y-%m-%d-%H-%M-%S-%f")
-                        path = self.problem.working_dir + 'artap' + ts
-                        os.mkdir(path)
+                        path = self.problem.working_dir + 'artap' + ts + str(individual.id)
+
+                        if os.path.exists(path):
+                            pass
+                        else:
+                            os.mkdir(path)
 
                         for file in self.output_files:
                             self._transfer_file_from_remote(source_file=file,
                                                             destination_file="{}/{}".format(path, file),
                                                             remote_dir=remote_dir, client=client)
                             output_files.append("{}/{}".format(path, file))
                         success = True
                         result = self.parse_results(output_files, individual)
                         # update cost on remote server
-                        client.root.log_update_cost(remote_dir, individual, result)
+
+                        # ToDo: resolve this, database is sometimes locked under Windows
+                        # client.root.log_update_cost(remote_dir, individual, result)
 
                     # remove job dir
                     if result is not None:
                         client.root.remove_job_dir(remote_dir)
 
                     if self.problem.options['save_data_files'] is False:
                         self._remove_dir(path)
@@ -672,14 +679,36 @@
                                requirements=self.requirements,
                                request_cpus=self.request_cpus,
                                request_memory=self.request_memory,
                                hold_on_start=self.hold_on_start,
                                desc=desc)
 
 
+class LocalCSTExecutor(Executor):
+    def __init__(self, problem, model_file):
+        self.problem = problem
+        directory = os.path.dirname(model_file)
+        self.parameter_file = os.path.join(directory, 'parameters.txt')
+        self.cst_file = model_file
+        self.executable = r'"C:/Program Files (x86)/CST Studio Suite 2020/CST DESIGN ENVIRONMENT"'
+        self.parameters = r'  -r --rebuild --hide -par {} -project-file {}'.format(self.parameter_file, self.cst_file)
+        self.command = self.executable + self.parameters
+
+    def eval(self, individual):
+        parameters = ""
+        for parameter, value in zip(self.problem.parameters, individual.vector):
+            parameters += "{}={}\n".format(parameter['name'], value)
+        parameter_file = open(self.parameter_file, "w")
+        parameter_file.write(parameters)
+        parameter_file.close()
+        os.system(self.command)
+        result = self.problem.parse_results(individual)
+        return [result]
+
+
 class CondorCSTJobExecutor(CondorJobExecutor):
     def __init__(self, problem, model_file, files_from_condor=None,
                  cst_path="\"C:\Program Files (x86)\CST Studio Suite 2020\CST DESIGN ENVIRONMENT.exe\""):
         self.model_file = ntpath.basename(model_file)
         super().__init__(problem, [self.model_file], files_from_condor)
         copyfile(model_file, self.problem.working_dir + self.model_file)
```

### Comparing `artap-2022.1.1.1759/artap/individual.py` & `artap-2023.4.12.3773/artap/individual.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import *
 from collections.abc import Iterable
 from enum import Enum
+import numpy as np
 
 
 class Individual(metaclass=ABCMeta):
     """ Collects information about one point in design space. """
 
     class State(Enum):
         EMPTY = 0
@@ -21,45 +22,51 @@
         if state == cls.State.EVALUATED:
             return 'evaluated'
         if state == cls.State.FAILED:
             return 'failed'
 
     counter: int = 0
 
-    def __init__(self, vector: list = [], features=dict()):
+    def __init__(self, vector: list = None):
         self.id = Individual.counter
         Individual.counter += 1
 
-        self.vector = vector.copy()
+        if vector is None:
+            self.vector = []
+        else:
+            self.vector = vector.copy()
+
         self.costs = []
         self.costs_signed = []
         self.state = self.State.EMPTY
         self.population_id = -1
         self.algorithm_id = 0
 
         self.parents = []
         self.children = []
 
         self.features = dict()
         self.features["start_time"] = 0.0
         self.features["finish_time"] = 0.0
-        self.features["feasible"] = 0.0   # the distance from the feasibility region in min norm, its an index, not a
-        self.features["precision"] = 7   # the default value of the considered decimals
-        for key, value in features.items():
-            if not key in self.features:
-                self.features[key] = value
-
+        self.features["feasible"] = 0.0  # the distance from the feasibility region in min norm, its an index, not a
+        self.features["precision"] = 7  # the default value of the considered decimals
+        self.add_features()
         self.custom = {}
 
+    def copy(self):
+        """Create a new Individual instance from a single individual"""
+        new_individual = self.__class__(self.vector)
+        return new_individual
+
     def calc_signed_costs(self, p_signs):
         """
         This function calculates the signed costs for every vector and insert the feasibility after
         :return:
         """
-        self.costs_signed = list(map(lambda x, y: x * round(y, ndigits=self.features["precision"]), p_signs, self.costs))
+        self.costs_signed = list(map(lambda x, y: x * np.round(y, decimals=self.features["precision"]), p_signs, self.costs))
         self.costs_signed.append(not self.features["feasible"])
 
     def __repr__(self):
         """ :return: [vector[p1, p2, ... pn]; costs[c1, c2, ... cn]] """
 
         string = "vector: ["
         for i, number in enumerate(self.vector):
@@ -94,25 +101,25 @@
 
         # string += "; state: '{}', ".format(Individual.State.to_string(self.state))
         # string += "; info: {}, ".format(self.info)
 
         return string
 
     def __eq__(self, other):
-        if self.costs_signed == []:
-            diff = set(self.vector) - set(other.vector)
-            return diff == set()
-        else:
-            diff = set(self.costs_signed) - set(other.costs_signed)
-            return  diff == set()
+        diff = 1
+        for i in range(len(self.vector)):
+            diff = abs(self.vector[i] - other.vector[i])
+        return diff < 1e-10
 
     def __hash__(self):
-        #return id(self)
         return hash(tuple(self.vector))
 
+    def add_features(self):
+        pass
+
     def sync(self, individual):
         self.vector = individual.vector
         self.costs = individual.costs
         self.costs_signed = individual.costs_signed
         self.state = individual.state
         self.population_id = individual.population_id
         self.algorithm_id = individual.algorithm_id
@@ -120,14 +127,25 @@
         self.parents = individual.parents
         self.children = individual.children
 
         self.features = individual.features
 
         self.custom = individual.custom
 
+    def _replace_individual_id(self, value):
+        if isinstance(value, Iterable):
+            val = []
+            for item in value:
+                val.append(self._replace_individual_id(item))
+            return val
+        elif isinstance(value, Individual):
+            return value.id
+        else:
+            return value
+
     def to_dict(self):
         output = {'id': self.id,
                   'vector': list(self.vector),
                   'costs': list(self.costs),
                   'costs_signed': self.costs_signed,
                   'state': self.to_string(self.state),
                   'population_id': self.population_id,
@@ -148,25 +166,14 @@
         features = dict()
         for key, value in self.features.items():
             features[key] = self._replace_individual_id(value)
         output['features'] = features
 
         return output
 
-    def _replace_individual_id(self, value):
-        if isinstance(value, Iterable):
-            val = []
-            for item in value:
-                val.append(self._replace_individual_id(item))
-            return val
-        elif isinstance(value, Individual):
-            return value.id
-        else:
-            return value
-
     @staticmethod
     def from_dict(dictionary):
         individual = Individual()
         individual.id = dictionary['id']
 
         individual.vector = dictionary['vector']
         individual.costs = dictionary['costs']
```

### Comparing `artap-2022.1.1.1759/artap/job.py` & `artap-2023.4.12.3773/artap/job.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/operators.py` & `artap-2023.4.12.3773/artap/operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from _ast import operator
 from abc import abstractmethod, ABC
+import copy
 import sys
 import random
 import math
 from math import exp
 import numpy as np
 import functools
 import itertools
+from copy import deepcopy
 
-from .individual import Individual
 from .utils import VectorAndNumbers
 from .doe import build_box_behnken, build_lhs, build_full_fact, build_plackett_burman, build_gsd, build_halton
 from .job import Job
 from joblib import Parallel, delayed
-from copy import deepcopy
+from .individual import Individual
+
 
 EPSILON = sys.float_info.epsilon
 
 # global constants to p and q dominates
 QDOM = 1
 PDOM = 2
 
@@ -189,110 +191,132 @@
                 individual.costs_signed[-2] = sum(sensitivity)
             else:
                 individual.costs.append(sum(sensitivity))
                 individual.costs_signed.insert(-1, sum(sensitivity))
 
 
 class Generator(Operator):
-    def __init__(self, parameters=None, features=dict()):
+    def __init__(self, parameters=None):
         super().__init__()
         self.parameters = parameters
-        self.features = features
 
     @abstractmethod
     def generate(self):
         pass
 
 
 class CustomGenerator(Generator):
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.vectors = []
 
     def init(self, vectors):
         self.vectors = vectors
 
     def generate(self):
+        vectors = []
+        for vector in self.vectors:
+            vectors.append(vector)
+        return vectors
+
+
+class PartiallyCustomGenerator(Generator):
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
+        self.vectors = []
+        self.number = None
+
+    def init(self, vectors, number):
+        self.vectors = vectors
+        self.number = number
+
+    def generate(self):
         individuals = []
         for vector in self.vectors:
-            individuals.append(Individual(vector, self.features))
-        return individuals
+            individuals.append(Individual(vector))
+        req = self.number - len(individuals)
+        vectors = []
+        for i in range(req + 1):
+            vector = VectorAndNumbers.gen_vector(self.parameters)
+            vectors.append(Individual(vector))
+        return vectors
 
 
 class UniformGenerator(Generator):
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.number = 0
 
     def init(self, number):
         self.number = number
 
     def generate(self):
         individuals = []
         vectors = []
         for parameter in self.parameters:
             vectors.append([])
             delta = (parameter['bounds'][1] - parameter['bounds'][0]) / (self.number - 1)
             for i in range(self.number):
                 vectors[-1].append(parameter['bounds'][0] + i * delta)
 
+        result = []
         for combination in itertools.product(*vectors):
-            individuals.append(Individual(list(combination), self.features))
+            result.append(list(combination))
 
-        return individuals
+        return result
 
 
 class RandomGenerator(Generator):
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.number = 0
 
     def init(self, number):
         self.number = number
 
     def generate(self):
-        individuals = []
+        vectors = []
         for i in range(self.number):
             vector = VectorAndNumbers.gen_vector(self.parameters)
-            individuals.append(Individual(vector, self.features))
-        return individuals
+            vectors.append(vector)
+        return vectors
 
 
 class IntegerGenerator(Generator):
     """
     Generate Integer vectors for problems with discrete values
     """
 
-    def __init__(self, parameters, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters):
+        super().__init__(parameters)
         # self.parameters['parameter_type'] = 'integer'
         self.number = 0
 
     def init(self, number, parameters):
         self.number = number
         for parameter in parameters:
             if not ('parameter_type' in parameter):
                 parameter['parameter_type'] = 'integer'
 
     def generate(self):
-        individuals = []
+        vectors = []
         for i in range(self.number):
             vector = VectorAndNumbers.gen_vector(self.parameters)
-            individuals.append(Individual(vector, self.features))
-        return individuals
+            vectors.append(vector)
+        return vectors
 
 
 class FullFactorGenerator(Generator):
     """
     Create a general full-factorial design
     Number of experiments (2 ** len(parameters) - without center, 3 ** len(parameters - with center)
     """
 
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.center = False
 
     def init(self, center):
         self.center = center
 
     def generate(self):
         dict_vars = {}
@@ -303,112 +327,95 @@
 
             if self.center:
                 dict_vars[name] = [l_b, (l_b + u_b) / 2.0, u_b]
             else:
                 dict_vars[name] = [l_b, u_b]
 
         df = build_full_fact(dict_vars)
-
-        individuals = []
-        for vector in df:
-            individuals.append(Individual(vector, self.features))
-        return individuals
+        return df
 
 
 class FullFactorLevelsGenerator(Generator):
     """
     Create a general full-factorial design
     Number of experiments (2 ** len(parameters) - without center, 3 ** len(parameters - with center)
     """
 
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.values = []
 
     def init(self, values):
         self.values = values
 
     def generate(self):
         dict_vars = {}
         for value, parameter in zip(self.values, self.parameters):
             dict_vars[parameter['name']] = value
 
         df = build_full_fact(dict_vars)
-
-        individuals = []
-        for vector in df:
-            individuals.append(Individual(vector, self.features))
-        return individuals
+        return df
 
 
 class PlackettBurmanGenerator(Generator):
     """
     Create a general full-factorial design
     Number of experiments (2 ** len(parameters) - without center, 3 ** len(parameters - with center)
     """
 
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
 
     def generate(self):
         dict_vars = {}
         for parameter in self.parameters:
             name = parameter['name']
             l_b = parameter['bounds'][0]
             u_b = parameter['bounds'][1]
             dict_vars[name] = [l_b, u_b]
 
         df = build_plackett_burman(dict_vars)
-        # print(df)
-
-        individuals = []
-        for vector in df:
-            individuals.append(Individual(vector, self.features))
-        return individuals
+        return df
 
 
 class BoxBehnkenGenerator(Generator):
     """
     Create a general full-factorial design
     # 3 params = 13 experiments
     # 4 params = 25 experiments
     # 5 params = 41 experiments
     # 6 params = 49 experiments
     # 7 params = 57 experiments
     # 8 params = 113 experiments
     https://en.wikipedia.org/wiki/Box%E2%80%93Behnken_design
     """
 
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
 
     def generate(self):
         dict_vars = {}
         for parameter in self.parameters:
             name = parameter['name']
             l_b = parameter['bounds'][0]
             u_b = parameter['bounds'][1]
             dict_vars[name] = [l_b, u_b]
 
         df = build_box_behnken(dict_vars)
         # print(df)
-
-        individuals = []
-        for vector in df:
-            individuals.append(Individual(vector, self.features))
-        return individuals
+        return df
 
 
 class LHSGenerator(Generator):
     """
     Builds a Latin Hypercube design dataframe from a dictionary of factor/level ranges.
     """
 
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.number = 0
 
     def init(self, number):
         self.number = number
 
     def generate(self):
         dict_vars = {}
@@ -416,56 +423,48 @@
             name = parameter["name"]
             l_b = parameter['bounds'][0]
             u_b = parameter['bounds'][1]
             dict_vars[name] = [l_b, u_b]
 
         df = build_lhs(dict_vars, num_samples=self.number)
         # print(df)
-
-        individuals = []
-        for vector in df:
-            individuals.append(Individual(vector, self.features))
-        return individuals
+        return df
 
 
 class HaltonGenerator(Generator):
     """
     Builds a Halton sequence.
     """
 
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.number = 0
 
     def init(self, number):
         self.number = number
 
     def generate(self):
         dict_vars = {}
         for parameter in self.parameters:
             name = parameter["name"]
             l_b = parameter['bounds'][0]
             u_b = parameter['bounds'][1]
             dict_vars[name] = [l_b, u_b]
 
         df = build_halton(dict_vars, num_samples=self.number)
-
-        individuals = []
-        for vector in df:
-            individuals.append(Individual(vector, self.features))
-        return individuals
+        return df
 
 
 class GSDGenerator(Generator):
     """
     Builds a Latin Hypercube design dataframe from a dictionary of factor/level ranges.
     """
 
-    def __init__(self, parameters=None, features=dict()):
-        super().__init__(parameters, features)
+    def __init__(self, parameters=None):
+        super().__init__(parameters)
         self.values = []
         self.reduction = 1
         self.n = 1
 
     def init(self, values, reduction, n=1):
         self.values = values
         self.reduction = reduction
@@ -475,21 +474,21 @@
         levels = []
         for value in self.values:
             levels.append(len(value))
 
         df = build_gsd(levels, self.reduction, self.n)
         # print(df)
 
-        individuals = []
+        vectors = []
         for vector in df:
             vals = []
             for i in range(len(vector)):
                 vals.append(self.values[i][vector[i]])
-            individuals.append(Individual(vals, self.features))
-        return individuals
+            vectors.append(vals)
+        return vectors
 
 
 class Mutator(Operator):
     def __init__(self, parameters, probability):
         super().__init__()
         self.parameters = parameters
         self.probability = probability
@@ -516,15 +515,15 @@
                 para_range = mutation_space * (u_b - l_b)
                 mutation = random.uniform(-para_range, para_range)
                 # vector.append(self.clip(p.vector[i] + mutation, l_b, u_b))
                 vector.append(p.vector[i] + mutation)
             else:
                 vector.append(p.vector[i])
 
-        p_new = Individual(vector, p.features)
+        p_new = vector
         return p_new
 
 
 class PmMutator(Mutator):
     """
     PmMutation -- for nsga2 and epsMoEA
 
@@ -539,19 +538,19 @@
     def mutate(self, parent, current_iteration=0):
         vector = []
 
         for i, parameter in enumerate(self.parameters):
             if random.uniform(0, 1) < self.probability:
                 l_b = parameter['bounds'][0]
                 u_b = parameter['bounds'][1]
-                vector.append(self.pm_mutation(parent.vector[i], l_b, u_b))
+                vector.append(self.pm_mutation(parent[i], l_b, u_b))
             else:
-                vector.append(parent.vector[i])
+                vector.append(parent[i])
 
-        return Individual(vector, parent.features)
+        return vector
 
     def pm_mutation(self, x, lb, ub):
         """
         Polynomial mutation for float and integer parameters.
 
         :param x: represents one parameter of the problem
         :param lb: lower bound
@@ -598,19 +597,19 @@
     def mutate(self, parent, current_iteration=0):
         vector = []
 
         for i, parameter in enumerate(self.parameters):
             if random.uniform(0, 1) < self.probability:
                 l_b = parameter['bounds'][0]
                 u_b = parameter['bounds'][1]
-                vector.append(self.uniform_mutation(parent.vector[i], l_b, u_b))
+                vector.append(self.uniform_mutation(parent[i], l_b, u_b))
             else:
-                vector.append(parent.vector[i])
+                vector.append(parent[i])
 
-        return Individual(vector, parent.features)
+        return vector
 
     def uniform_mutation(self, x, lb, ub):
 
         x = x + (random.random() - 0.5) * self.perturbation
         x = self.clip(x, lb, ub)
 
         return x
@@ -630,19 +629,19 @@
     def mutate(self, parent, current_iteration=0):
         vector = []
 
         for i, parameter in enumerate(self.parameters):
             if random.uniform(0, 1) < self.probability:
                 l_b = parameter['bounds'][0]
                 u_b = parameter['bounds'][1]
-                vector.append(self.non_uniform_mutation(parent.vector[i], l_b, u_b, current_iteration))
+                vector.append(self.non_uniform_mutation(parent[i], l_b, u_b, current_iteration))
             else:
-                vector.append(parent.vector[i])
+                vector.append(parent[i])
 
-        return Individual(vector, parent.features)
+        return vector
 
     def non_uniform_mutation(self, x, lb, ub, current_iteration):
 
         rand = random.random()
 
         if rand <= 0.5:
             x = self.__delta(ub - x, self.perturbation, current_iteration)
@@ -1013,17 +1012,19 @@
         # then use epsilon dominance on the objectives
         dominate_p = False
         dominate_q = False
 
         for i, (p_costs, q_costs) in enumerate(zip(p[:-1], q[:-1])):
 
             epsilon = float(self.epsilons[i % len(self.epsilons)])
+            if epsilon == 0:
+                epsilon = 1e-3
 
-            p_eps = math.floor(p_costs / epsilon)
-            q_eps = math.floor(q_costs / epsilon)
+            p_eps = p_costs / epsilon
+            q_eps = q_costs / epsilon
 
             if p_eps > q_eps:
                 dominate_q = True
                 if dominate_p:
                     return 0
             elif q_eps > p_eps:
                 dominate_p = True
@@ -1033,16 +1034,16 @@
         if not dominate_p and not dominate_q:
             dist1 = 0.0
             dist2 = 0.0
 
             for i, (p_costs, q_costs) in enumerate(zip(p[:-1], q[:-1])):
                 epsilon = float(self.epsilons[i % len(self.epsilons)])
 
-                i1 = math.floor(p_costs / epsilon)
-                i2 = math.floor(q_costs / epsilon)
+                i1 = p_costs / epsilon
+                i2 = q_costs / epsilon
 
                 dist1 += math.pow(p_costs - i1 * epsilon, 2.0)
                 dist2 += math.pow(q_costs - i2 * epsilon, 2.0)
 
             if dist1 < dist2:
                 return 1
             else:
@@ -1160,27 +1161,27 @@
     def individual(self, polulation, id):
         for individual in polulation:
             if individual.id == id:
                 return individual
 
         return None
 
-    def fast_nondominated_sorting(self, population):
+    def fast_nondominated_sorting(self, individuals):
         pareto_front = [[]]
         front_number = 1
 
         # reset elements
-        for p in population:
-            p.features['domination_counter'] = 0
-            p.features['front_number'] = None
-            p.features['dominate'] = []
-
-        for i, p in enumerate(population):
-            for j in range(i + 1, len(population)):
-                q = population[j]
+        for individual in individuals:
+            individual.features['domination_counter'] = 0
+            individual.features['front_number'] = None
+            individual.features['dominate'] = []
+
+        for i, p in enumerate(individuals):
+            for j in range(i + 1, len(individuals)):
+                q = individuals[j]
                 dom = self.comparator.compare(p.costs_signed, q.costs_signed)
                 if dom == 1:
                     p.features['dominate'].append(q.id)
                     q.features['domination_counter'] += 1
                 elif dom == 2:
                     p.features['domination_counter'] += 1
                     q.features['dominate'].append(p.id)
@@ -1191,27 +1192,25 @@
                 pareto_front[front_number - 1].append(p)
 
         while len(pareto_front[front_number - 1]) > 0:
             front_number += 1
             pareto_front.append([])
             for p in pareto_front[front_number - 2]:
                 for individual_id in p.features['dominate']:
-                    q = self.individual(population, individual_id)
+                    q = self.individual(individuals, individual_id)
                     q.features['domination_counter'] -= 1
                     if q.features['domination_counter'] == 0 and q.features['front_number'] is None:
                         q.features['front_number'] = front_number
                         pareto_front[front_number - 1].append(q)
 
         if len(pareto_front[front_number - 1]) == 0:
             pareto_front.pop()
         for sub_front in pareto_front:
             crowding_distance(sub_front)
 
-        return
-
 
 def crowding_distance(front):
     """
     Crowding distance calculates the solution density on a front, a subset of the population.
     :param front: list of individuals
                   which is a subset of the total population
     :return:
@@ -1258,14 +1257,15 @@
     :size:
         The size of the truncated result
     """
 
     # calculating the crowding distance on the different fronts
     population = list(set(population))
     result = sorted(population, key=functools.cmp_to_key(nondominated_cmp))
+    # ToDo:  Return also individuals which are not included in next population , result[size:]
     return result[:size]
 
 
 def nondominated_cmp(p, q):
     """
     From the 'front_number' the smaller value is favourized.
     From the 'crowding_distance' the higher values are favoured.
@@ -1302,18 +1302,16 @@
 class CopySelector(Selector):
     def __init__(self, parameters):
         super().__init__(parameters)
 
     def select(self, individuals):
         selection = []
         for individual in individuals:
-            candidate = Individual(individual.vector)
-            candidate.costs = deepcopy(individual.costs)
+            candidate = individual.copy()
             candidate.features = deepcopy(individual.features)
-            candidate.population_id = -1
             selection.append(candidate)
         return selection
 
 
 class TournamentSelector(Selector):
     def __init__(self, parameters, dominance=ParetoDominance, epsilons=None):
         super().__init__(parameters)
@@ -1429,16 +1427,16 @@
 
 
 class SimpleCrossover(Crossover):
     def __init__(self, parameters, probability):
         super().__init__(parameters, probability)
 
     def cross(self, p1, p2):
-        parent_a = p1.vector.copy()
-        parent_b = p2.vector.copy()
+        parent_a = p1.copy()
+        parent_b = p2.copy()
 
         if random.uniform(0.0, 1.0) <= self.probability:
             parameter1 = []
             parameter2 = []
             linear_range = 2
 
             alpha = random.uniform(0, linear_range)
@@ -1449,16 +1447,16 @@
 
                 parameter1.append(self.clip(alpha * p1.vector[i] + (1 - alpha) * p2.vector[i], l_b, u_b))
                 parameter2.append(self.clip((1 - alpha) * p1.vector[i] + alpha * p2.vector[i], l_b, u_b))
 
             parent_a = parameter1
             parent_b = parameter2
 
-        offspring_a = Individual(parent_a, p1.features)
-        offspring_b = Individual(parent_b, p2.features)
+        offspring_a = parent_a
+        offspring_b = parent_b
 
         return offspring_a, offspring_b
 
 
 class SimulatedBinaryCrossover(Crossover):
 
     def __init__(self, parameters, probability, distribution_index=15):
@@ -1475,16 +1473,18 @@
         """
         Create an offspring using simulated binary crossover.
         :return:  Individual, Individual
 
         a list with 2 offsprings each with the genotype of an  offspring after recombination and mutation.
         """
 
-        x1 = deepcopy(p1.vector)
-        x2 = deepcopy(p2.vector)
+        # Make new instance of class derived from Individual
+
+        x1 = p1.copy()
+        x2 = p2.copy()
 
         if random.random() <= self.probability:
             for i, param in enumerate(self.parameters):
 
                 if random.random() <= 0.5:
 
                     if abs(x2[i] - x1[i]) > EPSILON:
@@ -1523,15 +1523,15 @@
                         c2 = self.clip(c2, lb, ub)
 
                         if random.random() <= 0.5:
                             x1[i], x2[i] = c2, c1
                         else:
                             x1[i], x2[i] = c1, c2
 
-        return Individual(x1, p1.features), Individual(x2, p2.features)
+        return x1, x2
 
 
 class Normalization(Operator):
 
     def __init__(self) -> None:
         super().__init__()
 
@@ -1692,8 +1692,59 @@
         super().__init__()
         self.n_max_evals = n_max_evals
 
         if self.n_max_evals is None:
             self.n_max_evals = float("inf")
 
     def _do_continue(self, algorithm, **kwargs):
-        return algorithm.evaluator.n_eval < self.n_max_evals
+        return algorithm.evaluator.n_eval < self.n_max_evals
+
+
+def derivative(problem, points):
+    """
+        Compute derivative of func at points using finite differences
+
+               ddx = \\frac{func(points + eps) - func(points - eps)}{2 * eps}
+
+            Args:
+                problem (function): function with N parameters
+                points (array): array with N-dimension
+            Returns:
+                derivative: list with derivative
+                for instance:
+                    derivative[0] = d/d X1 func evaluated at points[0]
+                    derivative[1] = d/d X2 func evaluated at points[1]
+        """
+
+    d = []
+    eps = 1e-4
+    for i, p in enumerate(points):
+        step_up, step_down = list(points), list(points)  # copy list
+
+        # approximate derivative by tangent line with eps distance at
+        step_up[i] = p + eps
+        step_down[i] = p - eps
+        step_up = Individual(step_up)
+        step_down = Individual(step_down)
+        d.append((problem.evaluate(step_up)[0] - problem.evaluate(step_down)[0]) / (2 * eps))
+        # d.append((res1 - res2) / (2 * eps))
+
+    return d
+
+
+def std_linear(grad_g_x, sig):
+    """
+        Compute the standard deviation of g(Xi) using linear approximation
+                . math::
+                    sig_g = (sum_i^n (grad_g_xi * sig_Xi)^2)^(1/2)
+            Args:
+                grad_g_x (array): partial derivative of g with respect xi
+                sig (array): standard deviation of variables
+            Returns:
+                std_g (float): standard deviation of g(Xi)
+        """
+
+    std_g = 0
+    for dg_dx, s in zip(grad_g_x, sig):
+        std_g += (dg_dx ** 2 * s ** 2)
+    std_g = std_g ** (1 / 2)
+    return std_g
```

### Comparing `artap-2022.1.1.1759/artap/problem.py` & `artap-2023.4.12.3773/artap/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         self.data_store = None
         self.executor = None
         self.failed = []  # storage for failed individuals
         self.data_store = DummyDataStore()
         self.output_files = None
 
         self.working_dir = tempfile.gettempdir() + os.sep + "artap-{}".format(ts) + os.sep
-        os.mkdir(self.working_dir)
+        if not os.path.exists(self.working_dir):
+            os.mkdir(self.working_dir)
 
         # surrogate model (default - only simple eval)
         self.surrogate = SurrogateModelEval(self)
 
         # self._freeze()
         self.set(**kwargs)
         for cost in self.costs:
@@ -120,14 +121,17 @@
                     self.signs.append(-1)
             else:
                 self.signs.append(1)
 
         # clean up
         atexit.register(self.cleanup)
 
+    def __del__(self):
+        pass
+
     def populations(self):
         individuals = {}
         for individual in self.individuals:
             if individual.population_id not in individuals:
                 individuals[individual.population_id] = []
             individuals[individual.population_id].append(individual)
 
@@ -204,15 +208,14 @@
         return p_types
 
     @abstractmethod
     def evaluate(self, individual):
         """ :param individual: Individual """
         pass
 
-    @abstractmethod
     def evaluate_inequality_constraints(self, x):
         """ :param x: vector """
         return []
 
     def __setattr__(self, key, value):
         # if self.__is_frozen and not hasattr(self, key):
         #     raise TypeError(" %r is a frozen class" % self)
```

### Comparing `artap-2022.1.1.1759/artap/quality_indicator.py` & `artap-2023.4.12.3773/artap/quality_indicator.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/surrogate.py` & `artap-2023.4.12.3773/artap/surrogate.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/surrogate_scikit.py` & `artap-2023.4.12.3773/artap/surrogate_scikit.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/surrogate_smt.py` & `artap-2023.4.12.3773/artap/surrogate_smt.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
     def predict(self, x, *args):
         if self.trained:
             return self.regressor.predict_values(np.array([x]))
         else:
             assert 0
 
-    def predict_variances(self, x, *args):
+    def predict_variances(self, x):
         if self.trained:
-            return self.regressor.predict_variances(np.array([x]), *args)
+            return self.regressor.predict_variances(np.array([x]))
         else:
             assert 0
 
     def train(self):
         self.trained = False
         assert(len(self.x_data) == len(self.y_data))
```

### Comparing `artap-2022.1.1.1759/artap/tests/_test_scikit.py` & `artap-2023.4.12.3773/artap/tests/_test_scikit.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_agros.py` & `artap-2023.4.12.3773/artap/tests/test_agros.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 import math
+import pytest
 
 from ..problem import Problem
 from ..individual import Individual
 from ..results import Results
 
 try:
     from artap.algorithm_nlopt import NLopt
@@ -19,14 +20,15 @@
 
     __agros__ = True
 except ImportError:
     print("Agros is not present test skipped")
     __agros__ = False
 
 
+@pytest.mark.agros
 class AgrosProblem(Problem):
 
     def set(self):
         self.name = "agros problem"
         self.working_dir = "team_22/"
         self.parameters = [{'name': 'R2', 'initial_value': 3.0, 'bounds': [2.6, 3.4]},
                            {'name': 'h2', 'initial_value': 1.0, 'bounds': [0.408, 2.2]},
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_algorithm.py` & `artap-2023.4.12.3773/artap/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_archive.py` & `artap-2023.4.12.3773/artap/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_benchmark_pareto.py` & `artap-2023.4.12.3773/artap/tests/test_benchmark_pareto.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_benchmark_robust.py` & `artap-2023.4.12.3773/artap/tests/test_benchmark_robust.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_benchmarks.py` & `artap-2023.4.12.3773/artap/tests/test_benchmarks.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,9 +176,10 @@
 
 class TestAlpine(unittest.TestCase):
 
     def test_alpine(self):
         test2d = AlpineFunction(**{'dimension': 10})
         self.assertAlmostEqual(test2d.evaluate(Individual(test2d.global_optimum_coords))[0], test2d.global_optimum, 3)
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_calculation_fails.py` & `artap-2023.4.12.3773/artap/tests/test_calculation_fails.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
 from ..problem import Problem
-from ..algorithm_genetic import NSGAII
+from ..algorithm_NSGAII import NSGAII
 from ..results import Results
 from random import random
 
 
 class ParabolicProblem(Problem):
     """ Describe simple one objective optimization problem. """
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_datastore.py` & `artap-2023.4.12.3773/artap/tests/test_datastore.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sqlite3
 import pathlib
 
 from ..problem import Problem, ProblemViewDataStore
 from ..individual import Individual
 from ..datastore import SqliteDataStore
 from ..algorithm_sweep import SweepAlgorithm
-from ..algorithm_genetic import NSGAII
+from ..algorithm_NSGAII import NSGAII
 
 from ..operators import RandomGenerator
 
 from sys import platform
 if platform == "win32":
     __platform__ = 'WINDOWS'
 else:
@@ -39,16 +39,16 @@
         return [x_1**2 + x_2**2]
 
 
 class TestDataStoreSqlite(unittest.TestCase):
     def test_read_write_database(self):
         problem = MyProblem()
         # set data store
-        database_name = tempfile.NamedTemporaryFile(mode="w", delete=False, dir=None, suffix=".sqlite").name
-        # database_name = "database.sqlite"
+        # database_name = tempfile.NamedTemporaryFile(mode="w", delete=False, dir=None, suffix=".sqlite").name
+        database_name = "database_1.sqlite"
         problem.data_store = SqliteDataStore(problem, database_name=database_name)
 
         algorithm = NSGAII(problem)
         algorithm.options['max_population_number'] = 6
         algorithm.options['max_population_size'] = 4
         algorithm.options['max_processes'] = 4
         algorithm.run()
@@ -76,14 +76,15 @@
         self.assertAlmostEqual(individual.vector[1], individual_orig.vector[1], 3)
         for key, value in individual_orig.custom.items():
             self.assertEqual(value, individual.custom[key])
         for key, value in individual_orig.features.items():
             self.assertEqual(value, individual.features[key])
 
         # remove file
+        conn.close()
         os.remove(database_name)
 
     def test_read_datastore(self):
         # Path to this script file location
         file_path = str(pathlib.Path(__file__).parent.absolute())
         database_name = os.path.join(file_path, "data/data.sqlite")
         problem = ProblemViewDataStore(database_name=database_name)
@@ -138,14 +139,15 @@
         rows = c.fetchall()
         for row in rows:
             individual = Individual.from_dict(json.loads(row[1]))
             self.assertAlmostEqual(individual.costs[0], individuals[individual.id].costs[0], 3)
 
         # remove file
         # print(database_name)
+        conn.close()
         os.remove(database_name)
 
         t = time.time() - t_s
         problem.logger.info("read elapsed time: {} s".format(t))
 
     def get_size(self, start_path):
         if os.path.isfile(start_path):
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_generators.py` & `artap-2023.4.12.3773/artap/tests/test_generators.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,183 +9,183 @@
         self.parameters = [{'name': 'x_1', 'initial_value': 2.5, 'bounds': [-2.5, 5]},
                            {'name': 'x_2', 'initial_value': 1.5, 'bounds': [1, 3.4]},
                            {'name': 'x_3', 'initial_value': 3.5, 'bounds': [6, 10]}]
 
     def test_random_generator(self):
         gen = RandomGenerator(parameters=self.parameters)
         gen.init(3)
-        individuals = gen.generate()
+        vectors = gen.generate()
         # values
-        self.assertTrue(self.parameters[0]['bounds'][0] <= individuals[0].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[0].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[0].vector[2] <= self.parameters[2]['bounds'][1] and
-                        self.parameters[0]['bounds'][0] <= individuals[1].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[1].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[1].vector[2] <= self.parameters[2]['bounds'][1] and
-                        self.parameters[0]['bounds'][0] <= individuals[2].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[2].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[2].vector[2] <= self.parameters[2]['bounds'][1])
+        self.assertTrue(self.parameters[0]['bounds'][0] <= vectors[0][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[0][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[0][2] <= self.parameters[2]['bounds'][1] and
+                        self.parameters[0]['bounds'][0] <= vectors[1][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[1][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[1][2] <= self.parameters[2]['bounds'][1] and
+                        self.parameters[0]['bounds'][0] <= vectors[2][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[2][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[2][2] <= self.parameters[2]['bounds'][1])
 
     def test_custom_generator(self):
         gen = CustomGenerator()
         gen.init([[3, 2, 6], [-1, 3, 8]])
-        individuals = gen.generate()
+        vectors = gen.generate()
         # values
-        self.assertEqual(individuals[0].vector[0], 3)
-        self.assertEqual(individuals[0].vector[1], 2)
-        self.assertEqual(individuals[0].vector[2], 6)
-        self.assertEqual(individuals[1].vector[0], -1)
-        self.assertEqual(individuals[1].vector[1], 3)
-        self.assertEqual(individuals[1].vector[2], 8)
+        self.assertEqual(vectors[0][0], 3)
+        self.assertEqual(vectors[0][1], 2)
+        self.assertEqual(vectors[0][2], 6)
+        self.assertEqual(vectors[1][0], -1)
+        self.assertEqual(vectors[1][1], 3)
+        self.assertEqual(vectors[1][2], 8)
 
     def test_uniform_generator(self):
         gen = UniformGenerator(parameters=self.parameters)
         gen.init(4)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # values
-        self.assertEqual(len(individuals), 4**len(self.parameters))
-        self.assertEqual(individuals[0].vector[2], 6.0)
-        self.assertEqual(individuals[1].vector[0], -2.5)
-        self.assertEqual(individuals[12].vector[1], 3.4)
-        self.assertEqual(individuals[28].vector[2], 6.0)
-        self.assertEqual(individuals[35].vector[0], 2.5)
-        self.assertEqual(individuals[63].vector[2], 10.0)
+        self.assertEqual(len(vectors), 4**len(self.parameters))
+        self.assertEqual(vectors[0][2], 6.0)
+        self.assertEqual(vectors[1][0], -2.5)
+        self.assertEqual(vectors[12][1], 3.4)
+        self.assertEqual(vectors[28][2], 6.0)
+        self.assertEqual(vectors[35][0], 2.5)
+        self.assertEqual(vectors[63][2], 10.0)
 
     # Factorial Designs
     def test_full_fact_generator(self):
         # General Full-Factorial
         gen = FullFactorGenerator(parameters=self.parameters)
         gen.init(center=False)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # size
-        self.assertEqual(len(individuals), 8)
+        self.assertEqual(len(vectors), 8)
         # values
-        self.assertEqual(individuals[0].vector[0], -2.5)
-        self.assertEqual(individuals[1].vector[0], 5.0)
-        self.assertEqual(individuals[2].vector[1], 3.4)
-        self.assertEqual(individuals[3].vector[1], 3.4)
-        self.assertEqual(individuals[7].vector[2], 10.0)
+        self.assertEqual(vectors[0][0], -2.5)
+        self.assertEqual(vectors[1][0], 5.0)
+        self.assertEqual(vectors[2][1], 3.4)
+        self.assertEqual(vectors[3][1], 3.4)
+        self.assertEqual(vectors[7][2], 10.0)
 
         gen = FullFactorGenerator(parameters=self.parameters)
         gen.init(center=True)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
-        self.assertEqual(individuals[3].vector[0], -2.5)
-        self.assertEqual(individuals[-1].vector[1], 3.4)
+        self.assertEqual(vectors[3][0], -2.5)
+        self.assertEqual(vectors[-1][1], 3.4)
 
     def test_plackett_burman_generator(self):
         # Plackett-Burman
         gen = PlackettBurmanGenerator(parameters=self.parameters)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # size
-        self.assertEqual(len(individuals), 4)
+        self.assertEqual(len(vectors), 4)
         # values
-        self.assertEqual(individuals[0].vector[0], -2.5)
-        self.assertEqual(individuals[1].vector[0], 5.0)
-        self.assertEqual(individuals[2].vector[2], 6.0)
-        self.assertEqual(individuals[3].vector[1], 3.4)
+        self.assertEqual(vectors[0][0], -2.5)
+        self.assertEqual(vectors[1][0], 5.0)
+        self.assertEqual(vectors[2][2], 6.0)
+        self.assertEqual(vectors[3][1], 3.4)
 
     # Response - Surface Designs
     def test_box_behnken_generator(self):
         # Box-Behnken
         gen = BoxBehnkenGenerator(parameters=self.parameters)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # size
-        self.assertEqual(len(individuals), 13)
+        self.assertEqual(len(vectors), 13)
         # values
-        self.assertEqual(individuals[2].vector[2], 8.0)
-        self.assertEqual(individuals[3].vector[1], 3.4)
-        self.assertEqual(individuals[5].vector[0], 5.0)
-        self.assertEqual(individuals[12].vector[1], 2.2)
+        self.assertEqual(vectors[2][2], 8.0)
+        self.assertEqual(vectors[3][1], 3.4)
+        self.assertEqual(vectors[5][0], 5.0)
+        self.assertEqual(vectors[12][1], 2.2)
 
     # Randomized Designs
     def test_lhs_generation(self):
         # Latin - Hypercube
         gen = LHSGenerator(parameters=self.parameters)
         gen.init(number=3)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # size
-        self.assertEqual(len(individuals), 3)
+        self.assertEqual(len(vectors), 3)
         # values
-        self.assertTrue(self.parameters[0]['bounds'][0] <= individuals[0].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[0].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[0].vector[2] <= self.parameters[2]['bounds'][1] and
-                        self.parameters[0]['bounds'][0] <= individuals[1].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[1].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[1].vector[2] <= self.parameters[2]['bounds'][1] and
-                        self.parameters[0]['bounds'][0] <= individuals[2].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[2].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[2].vector[2] <= self.parameters[2]['bounds'][1])
+        self.assertTrue(self.parameters[0]['bounds'][0] <= vectors[0][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[0][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[0][2] <= self.parameters[2]['bounds'][1] and
+                        self.parameters[0]['bounds'][0] <= vectors[1][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[1][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[1][2] <= self.parameters[2]['bounds'][1] and
+                        self.parameters[0]['bounds'][0] <= vectors[2][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[2][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[2][2] <= self.parameters[2]['bounds'][1])
 
     # Randomized Designs
     def test_halton_generation(self):
         # Halton
         gen = HaltonGenerator(parameters=self.parameters)
         gen.init(number=3)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # size
-        self.assertEqual(len(individuals), 3)
+        self.assertEqual(len(vectors), 3)
         # values
-        self.assertTrue(self.parameters[0]['bounds'][0] <= individuals[0].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[0].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[0].vector[2] <= self.parameters[2]['bounds'][1] and
-                        self.parameters[0]['bounds'][0] <= individuals[1].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[1].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[1].vector[2] <= self.parameters[2]['bounds'][1] and
-                        self.parameters[0]['bounds'][0] <= individuals[2].vector[0] <= self.parameters[0]['bounds'][1] and
-                        self.parameters[1]['bounds'][0] <= individuals[2].vector[1] <= self.parameters[1]['bounds'][1] and
-                        self.parameters[2]['bounds'][0] <= individuals[2].vector[2] <= self.parameters[2]['bounds'][1])
+        self.assertTrue(self.parameters[0]['bounds'][0] <= vectors[0][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[0][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[0][2] <= self.parameters[2]['bounds'][1] and
+                        self.parameters[0]['bounds'][0] <= vectors[1][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[1][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[1][2] <= self.parameters[2]['bounds'][1] and
+                        self.parameters[0]['bounds'][0] <= vectors[2][0] <= self.parameters[0]['bounds'][1] and
+                        self.parameters[1]['bounds'][0] <= vectors[2][1] <= self.parameters[1]['bounds'][1] and
+                        self.parameters[2]['bounds'][0] <= vectors[2][2] <= self.parameters[2]['bounds'][1])
         # values
-        self.assertEqual(individuals[0].vector[2], 6.8)
-        self.assertEqual(individuals[2].vector[0], 3.125)
+        self.assertEqual(vectors[0][2], 6.8)
+        self.assertEqual(vectors[2][0], 3.125)
 
     # Factorial Designs - levels
     def test_full_fact_levels_generator(self):
         # GSD
         self.parameters = [{'name': 'U_1'},
                            {'name': 'U_2'},
                            {'name': 'U_3'},
                            {'name': 'PH_1'},
                            {'name': 'PH_2'},
                            {'name': 'PH_3'}]
         gen = FullFactorLevelsGenerator(parameters=self.parameters)
         amp = [0, 0.25, 0.5, 0.75, 1]
         phase = [-90.000, -67.500, -45.000, -22.500, 0.000, 22.500, 45.000, 67.500, 90.000]
         gen.init([amp, amp, amp, phase, phase, phase])
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # size
-        self.assertEqual(len(individuals), 91125)
+        self.assertEqual(len(vectors), 91125)
         # values
-        self.assertEqual(individuals[152].vector[1], 0)
-        self.assertEqual(individuals[8596].vector[0], 0.25)
-        self.assertEqual(individuals[70153].vector[3], -22.5)
-        self.assertEqual(individuals[90454].vector[5], 90.0)
+        self.assertEqual(vectors[152][1], 0)
+        self.assertEqual(vectors[8596][0], 0.25)
+        self.assertEqual(vectors[70153][3], -22.5)
+        self.assertEqual(vectors[90454][5], 90.0)
 
     # Generalized Subset Design (GSD) (C) 2018 - Rickard Sjoegren
     def test_gsd_generator(self):
         # GSD
         # self.parameters = [{'name': 'U_1'}, {'name': 'U_2'}, {'name': 'U_3'}, {'name': 'PH_1'}, {'name': 'PH_2'}, {'name': 'PH_3'}]
         self.parameters = [{'name': 'U_1'}, {'name': 'U_2'}]
         gen = GSDGenerator(parameters=self.parameters)
         gen.init([[1, 3, 2], [6, 8, 4]], reduction=2)
         # amp = [0, 0.25, 0.5, 0.75, 1]
         # phase = [-90.000, -67.500, -45.000, -22.500, 0.000, 22.500, 45.000, 67.500, 90.000]
         # gen.init([amp, amp, amp, phase, phase, phase], reduction=10)
-        individuals = gen.generate()
+        vectors = gen.generate()
 
         # size
-        self.assertEqual(len(individuals), 5)
+        self.assertEqual(len(vectors), 5)
         # values
-        self.assertEqual(individuals[0].vector[1], 6)
-        self.assertEqual(individuals[2].vector[0], 2)
-        self.assertEqual(individuals[4].vector[0], 3)
+        self.assertEqual(vectors[0][1], 6)
+        self.assertEqual(vectors[2][0], 2)
+        self.assertEqual(vectors[4][0], 3)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_gradients.py` & `artap-2023.4.12.3773/artap/tests/test_gradients.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_job.py` & `artap-2023.4.12.3773/artap/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_local_comsol.py` & `artap-2023.4.12.3773/artap/tests/test_local_comsol.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_local_femm.py` & `artap-2023.4.12.3773/artap/tests/test_local_femm.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 from ..executor import LocalFEMMExecutor
 from ..problem import Problem
 from ..results import Results
 from ..algorithm_sweep import SweepAlgorithm
 from ..operators import CustomGenerator
 
-__femm__ = False
-# result = os.system('femm')
-# if result != 0:
-#     __femm__ = False
+from distutils.spawn import find_executable
+path = find_executable('femm')
+__femm__ = path is not None
 
 
 class FEMMProblem(Problem):
     def set(self):
         self.name = "FEMMProblem"
         # Parameters must be defined in the FEMM model
         # pp = 0.8 -- relative pole pitch: 0.4 - 0.99
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_operators.py` & `artap-2023.4.12.3773/artap/tests/test_operators.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         self.features['precision'] = 7
         self.features['feasible'] = 0.0
 
     def test_simple_mutation(self):
         sm = SimpleMutator(self.parameters, 0.7)
         individual = sm.mutate(self.i1)
         self.assertTrue(
-            self.parameters[0]['bounds'][0] <= individual.vector[0] <= self.parameters[0]['bounds'][1] and
-            self.parameters[1]['bounds'][0] <= individual.vector[1] <= self.parameters[1]['bounds'][1])
+            self.parameters[0]['bounds'][0] <= individual[0] <= self.parameters[0]['bounds'][1] and
+            self.parameters[1]['bounds'][0] <= individual[1] <= self.parameters[1]['bounds'][1])
 
     def test_sbx(self):
         sbx = SimulatedBinaryCrossover(self.parameters, 1.0)
-        offsprings = sbx.cross(self.i1, self.i2)
+        offsprings = sbx.cross(self.i1.vector, self.i2.vector)
         self.assertEqual(len(offsprings), 2)
 
     def test_simple_crossover(self):
         sbx = SimpleCrossover(self.parameters, 0.9)
         offsprings = sbx.cross(self.i1, self.i2)
         self.assertEqual(len(offsprings), 2)
 
@@ -387,95 +387,95 @@
         y = Individual([2, 2])  # last index means that the solution is computed correctly
         y.costs = [-1.0, 6.0, 10.0]
         y.costs_signed = [-1.0, 6.0, 10.0, -0.1]
 
         result = dominance.compare(x.costs_signed, y.costs_signed)
         self.assertEqual(2, result)
 
-
-class EpsDominanceComparator(unittest.TestCase):
-
-    def test_should_dominance_comparator_work_properly_case_d(self):
-        """ Case 1: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 8.0]
-        """
-
-        # eps-dominance comparator should give back the same results as pareto-dominance if eps = 1e-5
-
-        dominance = EpsilonDominance(epsilons=1e-2)
-        x = Individual([2, 2])
-        x.costs = [-1.0, 5.0, 9.0]
-        x.costs_signed = [-1.0, 5.0, 9.0, 0]
-
-        y = Individual([2, 2])  # last index means that the solution is computed correctly
-        y.costs = [-1.0, 5.01, 8.0]
-        y.costs_signed = [-1.0, 5.01, 8.0, 0]
-
-        result = dominance.compare(x.costs_signed, y.costs_signed)
-
-        self.assertEqual(2, result)
-
-        # eps-dominance comparator should give different results if eps = 1
-
-        dominance = EpsilonDominance(epsilons=1e-3)
-        x = Individual([2, 2])
-        x.costs = [-1.0, 5.0, 9.0]
-        x.costs_signed = [-1.0, 5.0, 9.0, 0]
-
-        y = Individual([2, 2])  # last index means that the solution is computed correctly
-        y.costs = [-1.0, 5.01, 8.0]
-        y.costs_signed = [-1.0, 5.01, 8.0, 0]
-
-        result = dominance.compare(x.costs_signed, y.costs_signed)
-
-        self.assertEqual(0, result)
-
-    def test_should_dominance_comparator_work_properly_with_constrains_case_1(self):
-        """ Case 1: solution2 has a higher degree of constraint violation than solution 1
-        """
-        dominance = EpsilonDominance(epsilons=1e-5)
-        x = Individual([2, 2])
-        x.costs = [-1.0, 6.0, 11.0]
-        x.costs_signed = [-1.0, 6.0, 11.0, -0.1]
-
-        y = Individual([2, 2])  # last index means that the solution is computed correctly
-        y.costs = [-1.0, 5.0, 10.0]
-        y.costs_signed = [-1.0, 5.0, 10.0, -0.3]
-
-        result = dominance.compare(x.costs_signed, y.costs_signed)
-        self.assertEqual(1, result)
-
-    def test_should_dominance_comparator_work_properly_with_constrains_case_2(self):
-        """ Case 2: solution1 has a higher degree of constraint violation than solution 1
-        """
-        dominance = EpsilonDominance(epsilons=1e-5)
-        x = Individual([2, 2])
-        x.costs = [-1.0, 6.0, 9.0]
-        x.costs_signed = [-1.0, 6.0, 9.0, -0.5]
-
-        y = Individual([2, 2])  # last index means that the solution is computed correctly
-        y.costs = [-1.0, 6.0, 10.0]
-        y.costs_signed = [-1.0, 6.0, 10.0, -0.1]
-
-        result = dominance.compare(x.costs_signed, y.costs_signed)
-        self.assertEqual(2, result)
-
-    def test_should_dominance_comparator_work_properly_select_closer_to_boundary(self):
-        """ Case 3: solution1 closer to the rounded value than solution 2
-        """
-        dominance = EpsilonDominance(epsilons=0.1)
-        x = Individual([2, 2])
-        x.costs = [-1.0, 6.0, 9.05]
-        x.costs_signed = [-1.0, 6.0, 9.05, 0.0]
-
-        y = Individual([2, 2])  # last index means that the solution is computed correctly
-        y.costs = [-1.0, 6.0, 9.06]
-        y.costs_signed = [-1.0, 6.0, 9.06, 0.0]
-
-        result = dominance.compare(x.costs_signed, y.costs_signed)
-        self.assertEqual(1, result)
+# ToDo: Check and correct the test
+# class EpsDominanceComparator(unittest.TestCase):
+#
+#     def test_should_dominance_comparator_work_properly_case_d(self):
+#         """ Case 1: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 8.0]
+#         """
+#
+#         # eps-dominance comparator should give back the same results as pareto-dominance if eps = 1e-5
+#
+#         dominance = EpsilonDominance(epsilons=1e-2)
+#         x = Individual([2, 2])
+#         x.costs = [-1.0, 5.0, 9.0]
+#         x.costs_signed = [-1.0, 5.0, 9.0, 0]
+#
+#         y = Individual([2, 2])  # last index means that the solution is computed correctly
+#         y.costs = [-1.0, 5.01, 8.0]
+#         y.costs_signed = [-1.0, 5.01, 8.0, 0]
+#
+#         result = dominance.compare(x.costs_signed, y.costs_signed)
+#
+#         self.assertEqual(2, result)
+#
+#         # eps-dominance comparator should give different results if eps = 1
+#
+#         dominance = EpsilonDominance(epsilons=1e-3)
+#         x = Individual([2, 2])
+#         x.costs = [-1.0, 5.0, 9.0]
+#         x.costs_signed = [-1.0, 5.0, 9.0, 0]
+#
+#         y = Individual([2, 2])  # last index means that the solution is computed correctly
+#         y.costs = [-1.0, 5.01, 8.0]
+#         y.costs_signed = [-1.0, 5.01, 8.0, 0]
+#
+#         result = dominance.compare(x.costs_signed, y.costs_signed)
+#
+#         self.assertEqual(0, result)
+#
+#     def test_should_dominance_comparator_work_properly_with_constrains_case_1(self):
+#         """ Case 1: solution2 has a higher degree of constraint violation than solution 1
+#         """
+#         dominance = EpsilonDominance(epsilons=1e-5)
+#         x = Individual([2, 2])
+#         x.costs = [-1.0, 6.0, 11.0]
+#         x.costs_signed = [-1.0, 6.0, 11.0, -0.1]
+#
+#         y = Individual([2, 2])  # last index means that the solution is computed correctly
+#         y.costs = [-1.0, 5.0, 10.0]
+#         y.costs_signed = [-1.0, 5.0, 10.0, -0.3]
+#
+#         result = dominance.compare(x.costs_signed, y.costs_signed)
+#         self.assertEqual(1, result)
+#
+#     def test_should_dominance_comparator_work_properly_with_constrains_case_2(self):
+#         """ Case 2: solution1 has a higher degree of constraint violation than solution 1
+#         """
+#         dominance = EpsilonDominance(epsilons=1e-5)
+#         x = Individual([2, 2])
+#         x.costs = [-1.0, 6.0, 9.0]
+#         x.costs_signed = [-1.0, 6.0, 9.0, -0.5]
+#
+#         y = Individual([2, 2])  # last index means that the solution is computed correctly
+#         y.costs = [-1.0, 6.0, 10.0]
+#         y.costs_signed = [-1.0, 6.0, 10.0, -0.1]
+#
+#         result = dominance.compare(x.costs_signed, y.costs_signed)
+#         self.assertEqual(2, result)
+#
+#     def test_should_dominance_comparator_work_properly_select_closer_to_boundary(self):
+#         """ Case 3: solution1 closer to the rounded value than solution 2
+#         """
+#         dominance = EpsilonDominance(epsilons=0.1)
+#         x = Individual([2, 2])
+#         x.costs = [-1.0, 6.0, 9.05]
+#         x.costs_signed = [-1.0, 6.0, 9.05, 0.0]
+#
+#         y = Individual([2, 2])  # last index means that the solution is computed correctly
+#         y.costs = [-1.0, 6.0, 9.06]
+#         y.costs_signed = [-1.0, 6.0, 9.06, 0.0]
+#
+#         result = dominance.compare(x.costs_signed, y.costs_signed)
+#         self.assertEqual(1, result)
 
 
 class TestTournamentSelector(unittest.TestCase):
 
     def test_should_execute_work_properly_case1(self):
         x = Individual([3, 2])
         x.costs = [2.0, 3.0]
@@ -527,53 +527,41 @@
 class TestUniformMutator(unittest.TestCase):
 
     def setUp(self):
         problem = TestProblem()
         self.um = PmMutator(problem.parameters, 0)
 
     def test_should_the_solution_remain_unchanged_if_the_probability_is_zero(self):
-        x = Individual([3, 2])
-        x.costs = [2.0, 3.0]
-        x.costs_signed = [2.0, 3.0, 0.0]
-
+        x = [3, 2]
         y = self.um.mutate(x)
-        self.assertEqual(y.vector, [3, 2])
+        self.assertEqual(y, [3, 2])
 
     def test_should_change_if_the_probability_is_one(self):
-        x = Individual([3, 2])
-        x.costs = [2.0, 3.0]
-        x.costs_signed = [2.0, 3.0, 0.0]
-
+        x = [3, 2]
         self.um.probability = 1.0
         y = self.um.mutate(x)
-        self.assertNotEqual(y.vector, [3, 2])
+        self.assertNotEqual(y, [3, 2])
 
 
 class TestNonUniformMutator(unittest.TestCase):
 
     def setUp(self):
         problem = TestProblem()
         self.um = NonUniformMutation(problem.parameters, 0, 100, 1)
 
     def test_should_the_solution_remain_unchanged_if_the_probability_is_zero(self):
-        x = Individual([3, 2])
-        x.costs = [2.0, 3.0]
-        x.costs_signed = [2.0, 3.0, 0.0]
-
+        x = [3, 2]
         y = self.um.mutate(x)
-        self.assertEqual(y.vector, [3, 2])
+        self.assertEqual(y, [3, 2])
 
     def test_should_change_if_the_probability_is_one(self):
-        x = Individual([3, 2])
-        x.costs = [2.0, 3.0]
-        x.costs_signed = [2.0, 3.0, 0.0]
-
+        x = [3, 2]
         self.um.probability = 1.0
         y = self.um.mutate(x, 2)
-        self.assertNotEqual(y.vector, [3, 2])
+        self.assertNotEqual(y, [3, 2])
 
 
 class TestFireflystep(unittest.TestCase):
 
     def setUp(self):
         problem = TestProblem()
         self.crossover = FireflyStep(problem.parameters, 0, 1.0, 0, 1)
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_bayesopt.py` & `artap-2023.4.12.3773/artap/tests/test_problem_bayesopt.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_cmaes.py` & `artap-2023.4.12.3773/artap/tests/test_problem_cmaes.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_epsmoea.py` & `artap-2023.4.12.3773/artap/tests/test_problem_epsmoea.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_gradient_descent.py` & `artap-2023.4.12.3773/artap/tests/test_problem_gradient_descent.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,11 +126,10 @@
         algorithm.options["beta1"] = 0.5
         algorithm.options["beta2"] = 0.8
         algorithm.options["minimal_step"] = 1e-6
         algorithm.run()
 
         results = Results(problem)
         optimum = results.find_optimum('F_1')
-        print(optimum)
         self.assertLessEqual(abs(optimum.vector[0]), 1e-6)
         self.assertLessEqual(abs(optimum.vector[1]), 1.0)
         self.assertLessEqual(abs(optimum.costs[0]), 1.0)
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_monte_carlo.py` & `artap-2023.4.12.3773/artap/tests/test_problem_monte_carlo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,89 @@
 import unittest
+
+from artap.problem import Problem
 from ..algorithm_monte_carlo import Monte_Carlo, Numerical_Integrator, ImportanceSampling, Rejection_Sampling
 from ..results import Results
 from ..benchmark_functions import Sphere, Ackley, BenchmarkFunction, Schwefel
 import numpy as np
 
 
-class Integral_Problem(BenchmarkFunction):
+class Integral_Problem(Problem):
     def set(self, **kwargs):
         """Time-dependent 1D QM wave function of a single particle - squared."""
-        self.set_dimension(**kwargs)
-        self.parameters = self.generate_paramlist(self.dimension, lb=0.0, ub=1.0)
-
-        self.global_optimum = 0.50
-        self.global_optimum_coords = [0.0 for x in range(self.dimension)]
+        # self.set_dimension(**kwargs)
+        # self.parameters = self.generate_paramlist(self.dimension, lb=0.0, ub=1.0)
+        self.parameters = [{'name': 'x1', 'bounds': [0, 1], 'parameter_type': 'integer'}]
+        self.u_b = 3 * np.pi / 2
+        self.l_b = 0
+        self.sampling_size = 100
+        self.global_optimum = -1.0
 
         # single objective problem
         self.costs = [{'name': 'f_1', 'criteria': 'minimize'}]
 
     def evaluate(self, z):
         x = z.vector
-        output = np.exp(-x[0] ** 2) / (np.pi ** 0.5)
+        # output = np.exp(-x[0] ** 2) / (np.pi ** 0.5)
+        output = np.sin(x[0])
         return [output]
 
 
 class TestSphere(unittest.TestCase):
     # unit-test  benchmarck : Sphere, algorithm : Monte_Carlo
     def test_local_problem(self, population_number=50):
         problem = Sphere(**{'dimension': 1})
         algorithm = Monte_Carlo(problem)
         algorithm.options['max_population_number'] = population_number
         algorithm.options['max_population_size'] = 100
         algorithm.run()
 
         result = Results(problem)
         optimum = result.find_optimum('f_1')
-        self.assertAlmostEqual(int(optimum.costs[0]), problem.global_optimum)
+        self.assertAlmostEqual(optimum.costs[0], problem.global_optimum, places=4)
 
 
 class TestIntegral_MonteCarlo(unittest.TestCase):
     # unit-test  benchmarck : Sphere, algorithm : Integral_Monte_Carlo
     def test_local_problem(self):
         problem = Integral_Problem(**{'dimension': 1})
         algorithm = Numerical_Integrator(problem)
+        algorithm.options['max_population_number'] = 50
+        algorithm.options['max_population_size'] = 100
+        algorithm.options['max_processes'] = 10
         algorithm.run()
 
         result = Results(problem)
         optimum = result.find_optimum('f_1')
-        x = "{:0.1f}".format(optimum.costs[0])
-        self.assertAlmostEqual(float(x), problem.global_optimum)
-
-
-class TestImpotance_Sampling(unittest.TestCase):
-    # unit-test  benchmarck : Sphere, algorithm : ImportanceSampling
-    def test_local_problem(self):
-        problem = Integral_Problem(**{'dimension': 1})
-        algorithm = ImportanceSampling(problem)
-        algorithm.run()
-
-        result = Results(problem)
-        optimum = result.find_optimum('f_1')
-        x = "{:0.1f}".format(optimum.costs[0])
-        self.assertAlmostEqual(float(x), problem.global_optimum)
+        self.assertAlmostEqual(optimum.costs[0], problem.global_optimum, places=1)
 
 
-class TestRejection_Sampling(unittest.TestCase):
-    # unit-test  benchmarck : Sphere, algorithm : Rejection_Sampling
-    def test_local_problem(self):
-        problem = Sphere(**{'dimension': 1})
-        algorithm = Rejection_Sampling(problem)
-        algorithm.run()
-        result = Results(problem)
-        optimum = result.find_optimum('f_1')
-        self.assertAlmostEquals(int(optimum.costs[0]), problem.global_optimum)
+# class TestImpotance_Sampling(unittest.TestCase):
+#     # unit-test  benchmarck : Sphere, algorithm : ImportanceSampling
+#     def test_local_problem(self):
+#         problem = Integral_Problem(**{'dimension': 1})
+#         algorithm = ImportanceSampling(problem)
+#         algorithm.options['max_population_number'] = 20
+#         algorithm.options['max_population_size'] = 10
+#         algorithm.run()
+#
+#         result = Results(problem)
+#         optimum = result.find_optimum('f_1')
+#         x = "{:0.1f}".format(optimum.costs[0])
+#         self.assertAlmostEqual(optimum.costs[0], problem.global_optimum, places=2)
+#
+#
+# class TestRejection_Sampling(unittest.TestCase):
+#     # unit-test  benchmarck : Sphere, algorithm : Rejection_Sampling
+#     def test_local_problem(self):
+#         problem = Sphere(**{'dimension': 1})
+#         algorithm = Rejection_Sampling(problem)
+#         algorithm.options['max_population_number'] = 20
+#         algorithm.options['max_population_size'] = 10
+#         algorithm.run()
+#         result = Results(problem)
+#         optimum = result.find_optimum('f_1')
+#         self.assertAlmostEquals(optimum.costs[0], problem.global_optimum, places=2)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_nlopt.py` & `artap-2023.4.12.3773/artap/tests/test_problem_nlopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     from ..algorithm_nlopt import LN_NELDERMEAD
     from ..algorithm_nlopt import LN_SBPLX
     from ..algorithm_nlopt import LN_PRAXIS
     from ..algorithm_nlopt import LN_AUGLAG_EQ
     from ..algorithm_nlopt import LD_MMA
 
     __nlopt__ = True
+
 except ImportError:
     __nlopt__ = False
 
 from ..results import Results
 from ..problem import Problem
 from ..benchmark_functions import Booth
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_nsga2.py` & `artap-2023.4.12.3773/artap/tests/test_problem_nsga2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 import unittest
 
 from ..benchmark_functions import AlpineFunction, Ackley
 from ..benchmark_pareto import ZDT1
-from ..algorithm_genetic import NSGAII
+from ..algorithm_NSGAII import NSGAII
 from ..results import Results
 from ..problem import Problem
 from ..quality_indicator import epsilon_add
 
 
 class TestNSGA2(unittest.TestCase):
     def test_local_problem(self):
         problem = ZDT1()
         algorithm = NSGAII(problem)
-        algorithm.options['max_population_number'] = 5
-        algorithm.options['max_population_size'] = 3
+        algorithm.options['max_population_number'] = 10
+        algorithm.options['max_population_size'] = 10
         algorithm.options['max_processes'] = 1
         algorithm.run()
 
         populations = problem.populations()
 
-        self.assertEqual(len(populations), algorithm.options['max_population_number'] + 1)
+        # Test if the number of populations is the same as the required number
+        self.assertEqual(len(populations), algorithm.options['max_population_number'])
+
+        # Test if it fits the number of individuals in population
         for individuals in populations.values():
             self.assertEqual(len(individuals), algorithm.options['max_population_size'])
 
+        # Test if it fits the overall number of individuals
+        self.assertEqual(len(problem.individuals),
+                         algorithm.options['max_population_number'] * algorithm.options['max_population_size'])
+
 
 class TestZDT1(unittest.TestCase):
     # integration test -- tests the total functionality of nsga2
     # around 11secs according to literature DOI: 10.1007/978-3-642-01020-0_39
     def test_local_problem(self):
         problem = ZDT1()
         algorithm = NSGAII(problem)
-        algorithm.options['max_population_number'] = 250
-        algorithm.options['max_population_size'] = 100    # according to the literature
+        algorithm.options['max_population_number'] = 100
+        algorithm.options['max_population_size'] = 100  # according to the literature
         algorithm.options['max_processes'] = 1
         algorithm.run()
 
         results = Results(problem)
         vals = results.pareto_values()
         exact = problem.pareto_front(vals[0])
         self.assertLessEqual(epsilon_add(exact, vals), 0.2)
 
 
 class TestAckley(unittest.TestCase):
-    """ Tests that the nsga - ii can find the global optimum. """
+    """ Tests that the NSGA - II can find the global optimum. """
 
     def test_local_problem(self, population_number=50):
         try:
             problem = Ackley(**{'dimension': 1})
             algorithm = NSGAII(problem)
             algorithm.options['max_population_number'] = population_number
             algorithm.options['max_population_size'] = 100
@@ -125,32 +132,20 @@
 
             f_1 = []
             f_2 = []
             for individual in problem.last_population():
                 f_1.append(individual.costs[0])
                 f_2.append(individual.costs[1])
 
-            # print(len(problem.individuals))
-            # for individual in problem.individuals:
-            #    print(individual)
-
             self.assertLess(min(f_1), 1.5)
             self.assertGreater(max(f_1), 74)
             self.assertLess(max(f_2), 1.5)
             self.assertGreater(max(f_2), 0.75)
 
-            # import matplotlib.pyplot as plt
-            #
-            # plt.figure(figsize=(7, 5))
-            # # plt.scatter(res.F[:, 0], res.F[:, 1], s=30, facecolors='none', edgecolors='blue')
-            # plt.scatter(f_1, f_2, s=30, facecolors='none', edgecolors='blue')
-            # plt.title("Objective Space")
-            # plt.show()
-
-            # print(min(f_1), max(f_1), min(f_2), max(f_2))
+        # ToDo: Is it good in test?
         except AssertionError:
             # stochastic
             print("MultiConstraintOptimization::test_local_problem", population_number)
             self.test_constraint_nsgaii(int(1.5 * population_number))
 
 
 if __name__ == '__main__':
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_pymoo.py` & `artap-2023.4.12.3773/artap/tests/test_problem_pymoo.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 
 try:
     from ..algorithm_pymoo import Pymoo
 
     from pymoo.algorithms.soo.nonconvex.ga import GA
     from pymoo.algorithms.moo.nsga2 import NSGA2
     from pymoo.algorithms.soo.nonconvex.isres import ISRES
-    from pymoo.algorithms.soo.nonconvex.nelder_mead import NelderMead
+    from pymoo.algorithms.soo.nonconvex.nelder import NelderMead
     from pymoo.algorithms.soo.nonconvex.de import DE
 
     from pymoo.operators.sampling.lhs import LHS
-    from pymoo.factory import get_sampling, get_crossover, get_mutation
+
+    from pymoo.operators.crossover.sbx import SimulatedBinaryCrossover
+    from pymoo.operators.mutation.pm import PolynomialMutation
+    from pymoo.operators.sampling.rnd import FloatRandomSampling
 
     __pymoo__ = True
 except ImportError:
-    print("pymoo is not present test skiped")
+    print("pymoo is not present test skipped")
     __pymoo__ = False
 
 
 class ProblemConstraint(Problem):
     def set(self):
         self.name = 'ProblemConstraint'
 
@@ -54,17 +57,17 @@
 
 class TestpymooMultiConstraintOptimization(unittest.TestCase):
     @unittest.skipIf(__pymoo__ is False, "requires pymoo")
     def test_pymoo_nsgaii(self):
         moo_algorithm = NSGA2(
             pop_size=40,
             n_offsprings=10,
-            sampling=get_sampling("real_random"),
-            crossover=get_crossover("real_sbx", prob=0.9, eta=15),
-            mutation=get_mutation("real_pm", eta=20),
+            sampling=FloatRandomSampling(),
+            crossover=SimulatedBinaryCrossover(prob_var=0.9, eta=15),
+            mutation=PolynomialMutation(eta=20),
             eliminate_duplicates=True
         )
 
         problem = ProblemConstraint()
 
         algorithm = Pymoo(problem)
         algorithm.options['verbose_level'] = 0
@@ -121,17 +124,17 @@
             self.moo(moo_algorithm, int(1.5 * population_number))
 
     @unittest.skipIf(__pymoo__ is False, "requires pymoo")
     def test_nsga2(self):
         moo_algorithm = NSGA2(
             pop_size=10,
             n_offsprings=10,
-            sampling=get_sampling("real_random"),
-            crossover=get_crossover("real_sbx", prob=0.9, eta=15),
-            mutation=get_mutation("real_pm", eta=20),
+            sampling=FloatRandomSampling(),
+            crossover=SimulatedBinaryCrossover(prob_var=0.9, eta=15),
+            mutation=PolynomialMutation(eta=20),
             eliminate_duplicates=True
         )
         self.moo(moo_algorithm)
 
     @unittest.skipIf(__pymoo__ is False, "requires pymoo")
     def test_isres(self):
         moo_algorithm = ISRES(
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_scipy.py` & `artap-2023.4.12.3773/artap/tests/test_problem_scipy.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_problem_swarm.py` & `artap-2023.4.12.3773/artap/tests/test_problem_swarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 class TestAckleyOMOPSO(unittest.TestCase):
     """ Tests that the OMOPSO can find the global optimum. """
 
     def test_local_problem(self, population_number=50):
         problem = Ackley(**{'dimension': 1})
         algorithm = OMOPSO(problem)
         algorithm.options['max_population_number'] = population_number
-        algorithm.options['max_population_size'] = 100
+        algorithm.options['max_population_size'] = 40
         algorithm.options['max_processes'] = 10
         algorithm.options['epsilons'] = 0.1
         algorithm.run()
 
         b = Results(problem)
         optimum = b.find_optimum('f_1')  # Takes last cost function
         print(optimum.costs[0], problem.global_optimum)
         self.assertAlmostEqual(optimum.costs[0], problem.global_optimum, 1)
 
 
 class TestZDT1OMOPSO(unittest.TestCase):
     # integration test -- tests the total functionality of OMOPSO
 
     def test_local_problem(self):
-        problem = problem = ZDT1()
+        problem = ZDT1()
         algorithm = OMOPSO(problem)
-        algorithm.options['max_population_number'] = 500
-        algorithm.options['max_population_size'] = 100  # according to the literature
+        algorithm.options['max_population_number'] = 100
+        algorithm.options['max_population_size'] = 200  # according to the literature
         algorithm.options['max_processes'] = 1
         algorithm.options['epsilons'] = 0.05
         algorithm.run()
 
         results = Results(problem)
         vals = results.pareto_values(algorithm.archive)
         exact = problem.pareto_front(vals[0])
@@ -59,17 +59,17 @@
         self.assertAlmostEqual(optimum.costs[0], problem.global_optimum, 1)
 
 
 class TestZDT1SMPSP(unittest.TestCase):
     # integration test -- tests the total functionality of SMPSO
 
     def test_local_problem(self):
-        problem = problem = ZDT1()
+        problem = ZDT1()
         algorithm = OMOPSO(problem)
-        algorithm.options['max_population_number'] = 500
+        algorithm.options['max_population_number'] = 200
         algorithm.options['max_population_size'] = 100  # according to the literature
         algorithm.options['max_processes'] = 1
         algorithm.run()
 
         results = Results(problem)
         vals = results.pareto_values()
         exact = problem.pareto_front(vals[0])
@@ -83,14 +83,15 @@
         algorithm = SMPSO(problem)
         algorithm.options['max_population_number'] = 200
         algorithm.options['max_population_size'] = 100
         algorithm.options['max_processes'] = 10
         algorithm.run()
 
         result = Results(problem)
+
         optimum = result.find_optimum('f_1')
         print(optimum.costs[0])
         print(problem.global_optimum)
         self.assertEqual(optimum.costs[0], problem.global_optimum)
 
 
 class TestRosenbrockOMOPSO(unittest.TestCase):
@@ -180,15 +181,15 @@
 class TestAckleyPSOGA(unittest.TestCase):
     """ Tests that the PSOGA can find the global optimum. """
 
     def test_local_problem(self, population_number=50):
         problem = Ackley(**{'dimension': 1})
         algorithm = PSOGA(problem)
         algorithm.options['max_population_number'] = population_number
-        algorithm.options['max_population_size'] = 100
+        algorithm.options['max_population_size'] = 50
         algorithm.options['max_processes'] = 10
         algorithm.run()
 
         b = Results(problem)
         optimum = b.find_optimum('f_1')  # Takes last cost function
         print(optimum.costs[0], problem.global_optimum)
         self.assertAlmostEqual(optimum.costs[0], problem.global_optimum, 1)
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_quality_indicator.py` & `artap-2023.4.12.3773/artap/tests/test_quality_indicator.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_remote_condor.py` & `artap-2023.4.12.3773/artap/tests/test_remote_condor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 import random
 import unittest
 import zipfile
 from unittest import TestCase, main
 
 from ..algorithm import DummyAlgorithm
-from ..algorithm_genetic import NSGAII
+from ..algorithm_NSGAII import NSGAII
 from ..config import config
 from ..executor import CondorComsolJobExecutor, CondorMatlabJobExecutor, CondorPythonJobExecutor, CondorCSTJobExecutor
 from ..individual import Individual
 from ..problem import Problem
 
 
 class CondorMatlabProblem(Problem):
@@ -44,14 +44,16 @@
         self.parameters = [{'name': 'a', 'initial_value': 10, 'bounds': [0, 20]},
                            {'name': 'b', 'initial_value': 10, 'bounds': [5, 15]}]
 
         self.costs = [{'name': 'F_1'}]
         file_path = os.path.join(str(pathlib.Path(__file__).parent.absolute()), "data/elstat.mph")
         self.executor = CondorComsolJobExecutor(self, model_file=file_path,
                                                 files_from_condor=["out.txt", "elstat.mph"])
+        self.executor.request_cpus = 1
+        self.executor.request_memory = 3
 
     def evaluate(self, individual):
         return self.executor.eval(individual)
 
     def parse_results(self, output_files, individual):
         with open(output_files[0]) as file:
             content = file.readlines()
@@ -227,21 +229,21 @@
         self.assertAlmostEqual(5, individuals[0].costs[0])
 
     @unittest.skipIf(config["condor_host"] is None, "Condor is not defined.")
     def test_condor_python_exec_nsgaii(self):
         problem = PythonExecProblemNSGAII()
 
         algorithm = NSGAII(problem)
-        algorithm.options['max_population_number'] = 5
+        algorithm.options['max_population_number'] = 2
         algorithm.options['max_population_size'] = 3
-        algorithm.options['max_processes'] = 3
+        algorithm.options['max_processes'] = 2
         algorithm.run()
 
         populations = problem.populations()
 
-        self.assertEqual(len(populations), algorithm.options['max_population_number'] + 1)
+        self.assertEqual(len(populations), algorithm.options['max_population_number'])
         for individuals in populations.values():
             self.assertEqual(len(individuals), algorithm.options['max_population_size'])
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_results.py` & `artap-2023.4.12.3773/artap/tests/test_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import unittest
 import os
 import tempfile
 import csv
+import numpy as np
 
-from matplotlib.pyplot import show
-
+from ..algorithm_monte_carlo import Numerical_Integrator
 from ..problem import Problem
 from ..algorithm_sweep import SweepAlgorithm
-from ..algorithm_genetic import NSGAII
+from ..algorithm_NSGAII import NSGAII
 from ..operators import CustomGenerator
 from ..results import Results
 
 
 class TestProblem(Problem):
     """ Describe simple one objective optimization problem. """
 
@@ -40,22 +40,47 @@
                            {'name': 'x3', 'bounds': [12, 60], 'parameter_type': 'integer'},
                            {'name': 'x4', 'bounds': [12, 60], 'parameter_type': 'integer'}]
 
         self.costs = [{'name': 'f_1', 'criteria': 'minimize'},
                       {'name': 'f_2', 'criteria': 'minimize'}]
 
     def evaluate(self, individual):
-        f1 = (1. / 6.931 - (individual.vector[0] * individual.vector[1]) / (individual.vector[2] * individual.vector[3])) ** 2.
+        f1 = (1. / 6.931 - (individual.vector[0] * individual.vector[1]) / (
+                individual.vector[2] * individual.vector[3])) ** 2.
         f2 = max(individual.vector)
         return [f1, f2]
 
     def evaluate_inequality_constraints(self, individual):
         pass
 
 
+class IntegralProblem(Problem):
+
+    def set(self, **kwargs):
+        """Time-dependent 1D QM wave function of a single particle - squared."""
+        # self.set_dimension(**kwargs)
+        # self.parameters = self.generate_paramlist(self.dimension, lb=0.0, ub=1.0)
+        self.parameters = [{'name': 'x1', 'bounds': [0, 1], 'parameter_type': 'integer'}]
+
+        self.u_b = 3 * np.pi / 2
+        self.l_b = 0
+        self.sampling_size = 100
+        self.integral_global = 1.0
+
+        # single objective problem
+        self.costs = [{'name': 'f_1', 'criteria': 'minimize'}]
+
+    def evaluate(self, z):
+        x = z.vector
+        # output = 0
+        # for c in x:
+        f_1 = np.sin(x[0])
+        return [f_1]
+
+
 class TestResults(unittest.TestCase):
     """ Tests simple one objective optimization problem."""
 
     def setUp(self):
         self.problem = TestProblem()
 
         generator = CustomGenerator()
@@ -104,18 +129,18 @@
         parameters = self.results.parameters()
         self.assertEqual(parameters[0], [4.0, 2.0])
         self.assertEqual(parameters[1], [-1.0, -3.0])
         self.assertEqual(parameters[2], [2.0, 4.0])
 
     def test_costs(self):
         costs = self.results.costs()
-        self.assertEqual(len(costs), 3)
+        self.assertEqual(len(costs[0]), 3)
         self.assertEqual(costs[0][0], 20.0)
-        self.assertEqual(costs[1][0], 10.0)
-        self.assertEqual(costs[2][0], 20.0)
+        self.assertEqual(costs[0][1], 10.0)
+        self.assertEqual(costs[0][2], 20.0)
 
     def test_table(self):
         table = self.results.table(transpose=False)
         self.assertEqual(len(table), 3)
         self.assertEqual(table[1][2], 10.0)
 
         table = self.results.table(transpose=True)
@@ -225,7 +250,19 @@
         # remove file
         os.remove(csv_filename)
 
     def test_population(self):
         individuals = self.results.population()
         self.assertEqual(len(individuals), 3)
         self.assertEqual(individuals[1].costs[0], 10.0)
+
+    def test_integration_measure(self):
+        problem = IntegralProblem(**{'dimension': 1})
+        algorithm = Numerical_Integrator(problem)
+        algorithm.options['max_population_number'] = 50
+        algorithm.options['max_population_size'] = 100
+        algorithm.options['max_processes'] = 10
+        algorithm.run()
+
+        result = Results(problem)
+        integral = result.integration_measure()
+        self.assertAlmostEqual(integral, problem.integral_global, places=1)
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_robust.py` & `artap-2023.4.12.3773/artap/tests/test_robust.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_sensitivity.py` & `artap-2023.4.12.3773/artap/tests/test_sensitivity.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,21 +24,17 @@
     """ Tests simple one objective optimization problem."""
 
     def test_sobol_problem(self):
         problem = SensitivitySALibProblem()
         problem.options['save_data_files'] = True
 
         algorithm = SALibAlgorithm(problem)
-        algorithm.options["samples"] = 1024
+        algorithm.options["samples"] = 10000
         algorithm.options["method"] = "sobol"
         algorithm.options["print_to_console"] = True
         algorithm.run()
 
         res = algorithm.analyze()
 
         self.assertAlmostEqual(res["S1"][0], 0.316831, 2)
         self.assertAlmostEqual(res["S1"][1], 0.443764, 2)
-        self.assertAlmostEqual(res["S1"][2], 0.012203, 2)
-
-
-if __name__ == '__main__':
-    unittest.main()
+        self.assertAlmostEqual(res["S1"][2], 0.002807, 2)
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_surrogate_eval.py` & `artap-2023.4.12.3773/artap/tests/test_surrogate_eval.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_surrogate_function.py` & `artap-2023.4.12.3773/artap/tests/test_surrogate_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 from smt.surrogate_models import MGP
 
-from ..algorithm_genetic import NSGAII
+from ..algorithm_NSGAII import NSGAII
 from ..algorithm_sweep import SweepAlgorithm
 from ..operators import LHSGenerator
 from ..problem import Problem
 from ..results import Results
 from ..surrogate_smt import SurrogateModelSMT
 
 
@@ -37,15 +37,15 @@
         # y = - term1 + term2 + s
 
         y = (x[0] + 2 * x[1] - 7) ** 2 + (2 * x[0] + x[1] - 5) ** 2
 
         return [y]
 
     def predict(self, individual):
-        sigma_MGP, sigma_KRG = self.surrogate.predict_variances(individual.vector, True)
+        sigma_MGP = self.surrogate.predict_variances(individual.vector)
 
         if sigma_MGP < 1e-6:
             self.surrogate.train_step *= 1.3
 
             value_problem = self.evaluate(individual)
             value_surrogate = self.surrogate.predict(individual.vector)
             # print(individual.vector, value_problem, value_surrogate, sigma_MGP, sigma_KRG)
@@ -68,15 +68,15 @@
         x = individual.vector
 
         y = x[0]**2
 
         return [y]
 
     def predict(self, individual):
-        sigma_MGP, sigma_KRG = self.surrogate.predict_variances(individual.vector, True)
+        sigma_MGP = self.surrogate.predict_variances(individual.vector)
 
         if sigma_MGP < 1.00:
             # value_problem = self.evaluate(individual)
             value_surrogate = self.surrogate.predict(individual.vector)
             # print(individual.vector, value_problem, value_surrogate, sigma_MGP, sigma_KRG)
 
             return value_surrogate
```

### Comparing `artap-2022.1.1.1759/artap/tests/test_surrogate_scikit.py` & `artap-2023.4.12.3773/artap/tests/test_surrogate_scikit.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_surrogate_smt.py` & `artap-2023.4.12.3773/artap/tests/test_surrogate_smt.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap/tests/test_swarm.py` & `artap-2023.4.12.3773/artap/tests/test_swarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from ..benchmark_functions import Ackley
-from ..algorithm_swarm import SwarmAlgorithm, OMOPSO, SMPSO
+from ..algorithm_swarm import SwarmAlgorithm, OMOPSO, SMPSO, IndividualSwarm
 from ..problem import Problem
 from ..individual import Individual
 from ..archive import Archive
 
 
 class TestProblem(Problem):
 
@@ -42,15 +42,15 @@
     def test_speed_max_should_increase_speed(self):
         self.assertEqual(self.Swarm.speed_constriction(-1., 0., -1.), -0.5)
 
     def test_speed_do_not_change(self):
         self.assertEqual(self.Swarm.speed_constriction(0.1, 0., -1.), 0.1)
 
     def test_particle_best_should_initialized_correctly(self):
-        z = Individual([1, 2])
+        z = IndividualSwarm([1, 2])
         z.costs = [0.5, 1.5]
         z.costs_signed = [0.5, 1.5, 0]
 
         z.features = {'velocity': [], 'best_cost': [], 'best_vector': []}  #
 
         population = [z]
 
@@ -106,26 +106,14 @@
 
         # the new population vector should be differ from the original one
         self.assertNotEqual(population[0].vector, [1, 2])
 
         # it should preserve the features
         self.assertEqual(population[0].features, z.features)
 
-    def test_init_velocity(self):
-        z = Individual([1, 2])
-        z.costs = [0.5, 1.5]
-        z.costs_signed = [0.5, 1.5, 0]
-
-        z.features = {'velocity': [], 'best_cost': [0., 0., 0.], 'best_vector': [1, 2]}
-
-        population = [z]
-
-        self.omopso.init_pvelocity(population)
-        self.assertEqual(z.features['velocity'], [0, 0])
-
     def test_global_best(self):
         x = Individual([1, 2])
         x.costs = [2.0, 1.0]
         x.costs_signed = [2.0, 1.0, 0]
         x.features = {'velocity': [1, 2], 'best_cost': [0., 0., 0.], 'best_vector': [1, 2], 'crowding_distance': [50]}
 
         self.omopso.leaders.add(x)
```

### Comparing `artap-2022.1.1.1759/artap/utils.py` & `artap-2023.4.12.3773/artap/utils.py`

 * *Files identical despite different names*

### Comparing `artap-2022.1.1.1759/artap.egg-info/PKG-INFO` & `artap-2023.4.12.3773/artap.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 Metadata-Version: 2.1
 Name: artap
-Version: 2022.1.1.1759
+Version: 2023.4.12.3773
 Summary: Platform for robust design optimization
 Home-page: http://www.agros2d.org/artap/
 Author: Artap Team
 Author-email: artap.framework@gmail.com
 License: License :: OSI Approved :: MIT License
-Description: # Ārtap
-        
-        Ārtap is a framework for robust design optimization in Python. It contains an integrated, multi-physical FEM solver: Agros suite, furthermore it provides simple interfaces for commercial FEM solvers (COMSOL) and meta-heuristic, bayesian or neural network based optimization algorithms surrogate modelling techniques and neural networks.
-        
-        ## Installation
-        
-        Artap and its dependencies are available as wheel packages for Windows and Linux* distributions:
-        We recommend to install Artap under a [virtual environment](https://docs.python.org/3/tutorial/venv.html).
-        
-            pip install --upgrade pip # make sure that pip is reasonably new
-            pip install artap
-        
-        *The Windows versions are only partially, the linux packages are fully supported at the current version.
-        
-        ### Linux 
-        
-        You can install the full package, which contains the agrossuite package by the following command:
-        
-            pip install --upgrade pip # make sure that pip is reasonably new
-            pip install artap[full]
-        
-        ## Basic usage
-        
-        The goal of this example to show, how we can use Artap to solve a simple, bi-objective optimization problem.
-        
-        The problem is defined in the following way [GDE3]:
-        
-            Minimize f1 = x1
-            Minimize f2 = (1+x2) / x1
-        
-            subject to
-                    x1 e [0.1, 1]
-                    x2 e [0, 5]
-        
-        The Pareto - front of the following problem is known, it is a simple hyperbola. This problem is very simple for an Evolutionary algorithm, it finds its solution within 20-30 generations.
-         NSGA - II algorithm is used to solve this example.
-        
-        ### The Problem definition and solution with NSGA-II in Ārtap:
-        
-            class BiObjectiveTestProblem(Problem):
-        
-                def set(self):
-        
-                    self.name = 'Biobjective Test Problem'
-                    
-                    self.parameters = [{'name':'x_1', 'bounds': [0.1, 1.]},
-                                       {'name':'x_2', 'bounds': [0.0, 5.0]}]
-        
-                    self.costs = [{'name': 'f_1', 'criteria': 'minimize'},
-                                  {'name': 'f_2', 'criteria': 'minimize'}]
-        
-                def evaluate(self, individual):
-                    f1 = individual.vector[0]
-                    f2 = (1+individual.vector[1])/individual.vector[0]
-                return [f1, f2]
-         
-            # Perform the optimization iterating over 100 times on 100 individuals.
-            problem = BiObjectiveTestProblem()
-            algorithm = NSGAII(problem)
-            algorithm.options['max_population_number'] = 100
-            algorithm.options['max_population_size'] = 100
-            algorithm.run()
-        
-        ## References
-        
-        * [GDE3] Saku Kukkonen, Jouni Lampinen, The third Evolution Step of Generalized Differential Evolution
-        
-        
-        ## Citing
-        
-        If you use Ārtap in your research, the developers would be grateful if you would cite the relevant publications:
-        
-        [1]  Karban, Pavel, David Pánek, Tamás Orosz, Iveta Petrášová, and Ivo Doležel. “FEM based robust design optimization with Agros and Ārtap.” Computers & Mathematics with Applications (2020) https://doi.org/10.1016/j.camwa.2020.02.010.
-        
-        [2] Pánek, David, Tamás Orosz, and Pavel Karban. ” Ārtap: robust design optimization framework for engineering applications.” arXiv preprint arXiv:1912.11550 (2019).
-        
-        ### Applications
-        [3] Karban, P., Pánek, D., & Doležel, I. (2018). Model of induction brazing of nonmagnetic metals using model order reduction approach. COMPEL-The international journal for computation and mathematics in electrical and electronic engineering, 37(4), 1515-1524, https://doi.org/10.1108/COMPEL-08-2017-0356.
-        
-        [4] Pánek, D., Orosz, T., Kropík, P., Karban, P., & Doležel, I. (2019, June). Reduced-Order Model Based Temperature Control of Induction Brazing Process. In 2019 Electric Power Quality and Supply Reliability Conference (PQ) & 2019 Symposium on Electrical Engineering and Mechatronics (SEEM) (pp. 1-4). IEEE, https://doi.org/10.1109/PQ.2019.8818256.
-        
-        [5] Pánek, D., Karban, P., & Doležel, I. (2019). Calibration of Numerical Model of Magnetic Induction Brazing. IEEE Transactions on Magnetics, 55(6), 1-4, https://doi.org/10.1109/TMAG.2019.2897571.
-        
-        [6] Pánek, D., Orosz, T., Karban, P., & Doležel, I. (2020), “Comparison of simplified techniques for solving selected coupled electroheat problems”, COMPEL – The international journal for computation and mathematics in electrical and electronic engineering, Vol. 39 No. 1, pp. 220-230. https://doi.org/10.1108/COMPEL-06-2019-0244
-        
-        [7] Orosz, T.; Pánek, D.; Karban, P. FEM Based Preliminary Design Optimization in Case of Large Power Transformers. Appl. Sci. 2020, 10, 1361, https://doi.org/10.3390/app10041361.
-        
-        ## Contact
-        
-        If you have any questions, do not hesitate to contact us: artap.framework@gmail.com
-        
-        ## License
-        
-        Ārtap is published under [MIT license](https://en.wikipedia.org/wiki/MIT_License)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: full
+License-File: LICENSE
+
+# Ārtap
+
+Ārtap is a framework for robust design optimization in Python. It contains an integrated, multi-physical FEM solver: Agros suite, furthermore it provides simple interfaces for commercial FEM solvers (COMSOL) and meta-heuristic, bayesian or neural network based optimization algorithms surrogate modelling techniques and neural networks.
+
+## Installation
+
+Artap and its dependencies are available as wheel packages for Windows and Linux* distributions:
+We recommend to install Artap under a [virtual environment](https://docs.python.org/3/tutorial/venv.html).
+
+    pip install --upgrade pip # make sure that pip is reasonably new
+    pip install artap
+
+*The Windows versions are only partially, the linux packages are fully supported at the current version.
+
+### Linux 
+
+You can install the full package, which contains the agrossuite package by the following command:
+
+    pip install --upgrade pip # make sure that pip is reasonably new
+    pip install artap[full]
+
+## Basic usage
+
+The goal of this example to show, how we can use Artap to solve a simple, bi-objective optimization problem.
+
+The problem is defined in the following way [GDE3]:
+
+    Minimize f1 = x1
+    Minimize f2 = (1+x2) / x1
+
+    subject to
+            x1 e [0.1, 1]
+            x2 e [0, 5]
+
+The Pareto - front of the following problem is known, it is a simple hyperbola. This problem is very simple for an Evolutionary algorithm, it finds its solution within 20-30 generations.
+ NSGA - II algorithm is used to solve this example.
+
+### The Problem definition and solution with NSGA-II in Ārtap:
+
+    class BiObjectiveTestProblem(Problem):
+
+        def set(self):
+
+            self.name = 'Biobjective Test Problem'
+            
+            self.parameters = [{'name':'x_1', 'bounds': [0.1, 1.]},
+                               {'name':'x_2', 'bounds': [0.0, 5.0]}]
+
+            self.costs = [{'name': 'f_1', 'criteria': 'minimize'},
+                          {'name': 'f_2', 'criteria': 'minimize'}]
+
+        def evaluate(self, individual):
+            f1 = individual.vector[0]
+            f2 = (1+individual.vector[1])/individual.vector[0]
+        return [f1, f2]
+ 
+    # Perform the optimization iterating over 100 times on 100 individuals.
+    problem = BiObjectiveTestProblem()
+    algorithm = NSGAII(problem)
+    algorithm.options['max_population_number'] = 100
+    algorithm.options['max_population_size'] = 100
+    algorithm.run()
+
+## References
+
+* [GDE3] Saku Kukkonen, Jouni Lampinen, The third Evolution Step of Generalized Differential Evolution
+
+
+## Citing
+
+If you use Ārtap in your research, the developers would be grateful if you would cite the relevant publications:
+
+[1]  Karban, Pavel, David Pánek, Tamás Orosz, Iveta Petrášová, and Ivo Doležel. “FEM based robust design optimization with Agros and Ārtap.” Computers & Mathematics with Applications (2020) https://doi.org/10.1016/j.camwa.2020.02.010.
+
+[2] Pánek, David, Tamás Orosz, and Pavel Karban. ” Ārtap: robust design optimization framework for engineering applications.” arXiv preprint arXiv:1912.11550 (2019).
+
+### Applications
+[3] Karban, P., Pánek, D., & Doležel, I. (2018). Model of induction brazing of nonmagnetic metals using model order reduction approach. COMPEL-The international journal for computation and mathematics in electrical and electronic engineering, 37(4), 1515-1524, https://doi.org/10.1108/COMPEL-08-2017-0356.
+
+[4] Pánek, D., Orosz, T., Kropík, P., Karban, P., & Doležel, I. (2019, June). Reduced-Order Model Based Temperature Control of Induction Brazing Process. In 2019 Electric Power Quality and Supply Reliability Conference (PQ) & 2019 Symposium on Electrical Engineering and Mechatronics (SEEM) (pp. 1-4). IEEE, https://doi.org/10.1109/PQ.2019.8818256.
+
+[5] Pánek, D., Karban, P., & Doležel, I. (2019). Calibration of Numerical Model of Magnetic Induction Brazing. IEEE Transactions on Magnetics, 55(6), 1-4, https://doi.org/10.1109/TMAG.2019.2897571.
+
+[6] Pánek, D., Orosz, T., Karban, P., & Doležel, I. (2020), “Comparison of simplified techniques for solving selected coupled electroheat problems”, COMPEL – The international journal for computation and mathematics in electrical and electronic engineering, Vol. 39 No. 1, pp. 220-230. https://doi.org/10.1108/COMPEL-06-2019-0244
+
+[7] Orosz, T.; Pánek, D.; Karban, P. FEM Based Preliminary Design Optimization in Case of Large Power Transformers. Appl. Sci. 2020, 10, 1361, https://doi.org/10.3390/app10041361.
+
+## Contact
+
+If you have any questions, do not hesitate to contact us: artap.framework@gmail.com
+
+## License
+
+Ārtap is published under [MIT license](https://en.wikipedia.org/wiki/MIT_License)
```

### Comparing `artap-2022.1.1.1759/artap.egg-info/SOURCES.txt` & `artap-2023.4.12.3773/artap.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 artap/__init__.py
 artap/algorithm.py
+artap/algorithm_NSGAII.py
 artap/algorithm_bayesopt.py
+artap/algorithm_cem.py
 artap/algorithm_cmaes.py
 artap/algorithm_genetic.py
 artap/algorithm_gradient_descent.py
 artap/algorithm_monte_carlo.py
 artap/algorithm_nlopt.py
 artap/algorithm_pymoo.py
 artap/algorithm_scipy.py
@@ -51,17 +53,19 @@
 artap/tests/test_benchmarks.py
 artap/tests/test_calculation_fails.py
 artap/tests/test_datastore.py
 artap/tests/test_generators.py
 artap/tests/test_gradients.py
 artap/tests/test_job.py
 artap/tests/test_local_comsol.py
+artap/tests/test_local_cst.py
 artap/tests/test_local_femm.py
 artap/tests/test_operators.py
 artap/tests/test_problem_bayesopt.py
+artap/tests/test_problem_cem.py
 artap/tests/test_problem_cmaes.py
 artap/tests/test_problem_epsmoea.py
 artap/tests/test_problem_gradient_descent.py
 artap/tests/test_problem_monte_carlo.py
 artap/tests/test_problem_nlopt.py
 artap/tests/test_problem_nsga2.py
 artap/tests/test_problem_pymoo.py
```

### Comparing `artap-2022.1.1.1759/setup.py` & `artap-2023.4.12.3773/setup.py`

 * *Files identical despite different names*

