# Comparing `tmp/qpsolvers-3.3.0.tar.gz` & `tmp/qpsolvers-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpsolvers-3.3.0.tar", last modified: Tue Apr 11 12:21:12 2023, max compression
+gzip compressed data, was "qpsolvers-3.3.1.tar", last modified: Wed Apr 12 09:43:49 2023, max compression
```

## Comparing `qpsolvers-3.3.0.tar` & `qpsolvers-3.3.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1590 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2529 2023-03-29 16:03:40.695119 qpsolvers-3.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      128 2023-03-03 11:09:52.358283 qpsolvers-3.3.0/.gitignore
--rw-r--r--   0        0        0    15793 2023-04-11 12:17:50.779162 qpsolvers-3.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      916 2023-02-28 14:28:36.811176 qpsolvers-3.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     7652 2021-03-24 14:54:52.923152 qpsolvers-3.3.0/LICENSE
--rw-r--r--   0        0        0     9754 2023-04-11 09:57:38.987082 qpsolvers-3.3.0/README.md
--rw-r--r--   0        0        0      832 2023-02-28 13:41:23.525818 qpsolvers-3.3.0/THANKS
--rw-r--r--   0        0        0     2740 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_dense_problem.py
--rw-r--r--   0        0        0     2077 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_model_predictive_control.py
--rw-r--r--   0        0        0     3471 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_random_problems.py
--rw-r--r--   0        0        0     3017 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_sparse_problem.py
--rw-r--r--   0        0        0     9656 2023-03-03 11:09:52.358283 qpsolvers-3.3.0/doc/conf.py
--rw-r--r--   0        0        0     2924 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/developer-notes.rst
--rw-r--r--   0        0        0      265 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/environment.yml
--rw-r--r--   0        0        0      931 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/doc/index.rst
--rw-r--r--   0        0        0     3707 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/doc/installation.rst
--rw-r--r--   0        0        0     1006 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/doc/least-squares.rst
--rw-r--r--   0        0        0     5559 2023-03-03 15:29:30.344114 qpsolvers-3.3.0/doc/quadratic-programming.rst
--rw-r--r--   0        0        0     2521 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/references.rst
--rw-r--r--   0        0        0      968 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/supported-solvers.rst
--rw-r--r--   0        0        0      473 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/doc/unsupported-solvers.rst
--rw-r--r--   0        0        0      636 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/README.md
--rw-r--r--   0        0        0     2030 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/box_inequalities.py
--rw-r--r--   0        0        0     1601 2023-02-23 09:14:02.683958 qpsolvers-3.3.0/examples/constrained_linear_regression.py
--rw-r--r--   0        0        0     2790 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/dual_multipliers.py
--rw-r--r--   0        0        0     1867 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/least_squares.py
--rw-r--r--   0        0        0     8297 2023-02-23 09:14:02.683958 qpsolvers-3.3.0/examples/model_predictive_control.py
--rw-r--r--   0        0        0     2045 2023-03-03 11:01:10.969238 qpsolvers-3.3.0/examples/quadratic_program.py
--rw-r--r--   0        0        0     2656 2023-03-28 08:42:54.624660 qpsolvers-3.3.0/examples/sparse_least_squares.py
--rw-r--r--   0        0        0     2100 2023-04-11 09:56:47.503891 qpsolvers-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     2295 2023-04-11 12:18:06.354909 qpsolvers-3.3.0/qpsolvers/__init__.py
--rw-r--r--   0        0        0     1317 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/qpsolvers/_internals.py
--rw-r--r--   0        0        0     1216 2023-02-23 09:14:02.687958 qpsolvers-3.3.0/qpsolvers/conversions/__init__.py
--rw-r--r--   0        0        0     2317 2023-02-23 09:14:02.687958 qpsolvers-3.3.0/qpsolvers/conversions/ensure_sparse_matrices.py
--rw-r--r--   0        0        0     3561 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/qpsolvers/conversions/linear_from_box_inequalities.py
--rw-r--r--   0        0        0     3762 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/qpsolvers/conversions/socp_from_qp.py
--rw-r--r--   0        0        0     2284 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/conversions/split_dual_linear_box.py
--rw-r--r--   0        0        0     1677 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/qpsolvers/exceptions.py
--rw-r--r--   0        0        0     8531 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/qpsolvers/problem.py
--rw-r--r--   0        0        0     6610 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/problems.py
--rw-r--r--   0        0        0     7795 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solution.py
--rw-r--r--   0        0        0     7412 2023-03-28 08:42:54.624660 qpsolvers-3.3.0/qpsolvers/solve_ls.py
--rw-r--r--   0        0        0     3437 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/qpsolvers/solve_problem.py
--rw-r--r--   0        0        0     4698 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solve_qp.py
--rw-r--r--   0        0        0     1743 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solve_unconstrained.py
--rw-r--r--   0        0        0    12032 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/qpsolvers/solvers/__init__.py
--rw-r--r--   0        0        0     6665 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/clarabel_.py
--rw-r--r--   0        0        0     9089 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/cvxopt_.py
--rw-r--r--   0        0        0     6441 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/daqp_.py
--rw-r--r--   0        0        0     8434 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/ecos_.py
--rw-r--r--   0        0        0     7813 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/gurobi_.py
--rw-r--r--   0        0        0     9571 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/highs_.py
--rw-r--r--   0        0        0     9733 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/osqp_.py
--rw-r--r--   0        0        0     9807 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/proxqp_.py
--rw-r--r--   0        0        0    13544 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/qpoases_.py
--rw-r--r--   0        0        0    10619 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/qpswift_.py
--rw-r--r--   0        0        0     6046 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/quadprog_.py
--rw-r--r--   0        0        0     9904 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/scs_.py
--rw-r--r--   0        0        0     2808 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/qpsolvers/unsupported/__init__.py
--rw-r--r--   0        0        0     4274 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/unsupported/mosek_.py
--rw-r--r--   0        0        0     6453 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/unsupported/nppro_.py
--rw-r--r--   0        0        0     2390 2023-02-28 13:27:49.518364 qpsolvers-3.3.0/qpsolvers/utils.py
--rw-r--r--   0        0        0       59 2021-04-09 11:14:24.912320 qpsolvers-3.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2612 2023-03-28 08:42:54.628660 qpsolvers-3.3.0/tests/problems.py
--rw-r--r--   0        0        0     2214 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/tests/test_clarabel.py
--rw-r--r--   0        0        0     3681 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_conversions.py
--rw-r--r--   0        0        0     3940 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/tests/test_cvxopt.py
--rw-r--r--   0        0        0     1370 2023-03-31 12:30:36.615914 qpsolvers-3.3.0/tests/test_ecos.py
--rw-r--r--   0        0        0     1527 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_gurobi.py
--rw-r--r--   0        0        0     1773 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_highs.py
--rw-r--r--   0        0        0     1377 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_mosek.py
--rw-r--r--   0        0        0     1348 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/tests/test_nppro.py
--rw-r--r--   0        0        0     1370 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_osqp.py
--rw-r--r--   0        0        0     3584 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/tests/test_problem.py
--rw-r--r--   0        0        0     3570 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_proxqp.py
--rw-r--r--   0        0        0     3191 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_qpoases.py
--rw-r--r--   0        0        0     1733 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_qpswift.py
--rw-r--r--   0        0        0     2332 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_quadprog.py
--rw-r--r--   0        0        0     1695 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_scs.py
--rw-r--r--   0        0        0     2640 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_solution.py
--rw-r--r--   0        0        0     9194 2023-03-28 08:42:54.628660 qpsolvers-3.3.0/tests/test_solve_ls.py
--rw-r--r--   0        0        0    11123 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/tests/test_solve_problem.py
--rw-r--r--   0        0        0    25373 2023-03-31 12:28:59.113529 qpsolvers-3.3.0/tests/test_solve_qp.py
--rw-r--r--   0        0        0     3012 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_unfeasible_problem.py
--rw-r--r--   0        0        0     1865 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     2426 2023-04-11 09:56:47.503891 qpsolvers-3.3.0/tox.ini
--rw-r--r--   0        0        0    11721 1970-01-01 00:00:00.000000 qpsolvers-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1590 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2529 2023-03-29 16:03:40.695119 qpsolvers-3.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      128 2023-03-03 11:09:52.358283 qpsolvers-3.3.1/.gitignore
+-rw-r--r--   0        0        0    15890 2023-04-12 09:43:12.950561 qpsolvers-3.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      916 2023-02-28 14:28:36.811176 qpsolvers-3.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     7652 2021-03-24 14:54:52.923152 qpsolvers-3.3.1/LICENSE
+-rw-r--r--   0        0        0     9754 2023-04-11 09:57:38.987082 qpsolvers-3.3.1/README.md
+-rw-r--r--   0        0        0      832 2023-02-28 13:41:23.525818 qpsolvers-3.3.1/THANKS
+-rw-r--r--   0        0        0     2740 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_dense_problem.py
+-rw-r--r--   0        0        0     2077 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_model_predictive_control.py
+-rw-r--r--   0        0        0     3471 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_random_problems.py
+-rw-r--r--   0        0        0     3017 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_sparse_problem.py
+-rw-r--r--   0        0        0     9656 2023-03-03 11:09:52.358283 qpsolvers-3.3.1/doc/conf.py
+-rw-r--r--   0        0        0     2924 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/developer-notes.rst
+-rw-r--r--   0        0        0      265 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/environment.yml
+-rw-r--r--   0        0        0      931 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/doc/index.rst
+-rw-r--r--   0        0        0     3707 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/doc/installation.rst
+-rw-r--r--   0        0        0     1006 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/doc/least-squares.rst
+-rw-r--r--   0        0        0     5559 2023-03-03 15:29:30.344114 qpsolvers-3.3.1/doc/quadratic-programming.rst
+-rw-r--r--   0        0        0     2521 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/references.rst
+-rw-r--r--   0        0        0      968 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/supported-solvers.rst
+-rw-r--r--   0        0        0      473 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/doc/unsupported-solvers.rst
+-rw-r--r--   0        0        0      636 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/README.md
+-rw-r--r--   0        0        0     2030 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/box_inequalities.py
+-rw-r--r--   0        0        0     1601 2023-02-23 09:14:02.683958 qpsolvers-3.3.1/examples/constrained_linear_regression.py
+-rw-r--r--   0        0        0     2790 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/dual_multipliers.py
+-rw-r--r--   0        0        0     1867 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/least_squares.py
+-rw-r--r--   0        0        0     8297 2023-02-23 09:14:02.683958 qpsolvers-3.3.1/examples/model_predictive_control.py
+-rw-r--r--   0        0        0     2045 2023-03-03 11:01:10.969238 qpsolvers-3.3.1/examples/quadratic_program.py
+-rw-r--r--   0        0        0     2656 2023-03-28 08:42:54.624660 qpsolvers-3.3.1/examples/sparse_least_squares.py
+-rw-r--r--   0        0        0     2100 2023-04-12 09:42:35.095945 qpsolvers-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2295 2023-04-12 09:43:22.815073 qpsolvers-3.3.1/qpsolvers/__init__.py
+-rw-r--r--   0        0        0     1317 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/qpsolvers/_internals.py
+-rw-r--r--   0        0        0     1216 2023-02-23 09:14:02.687958 qpsolvers-3.3.1/qpsolvers/conversions/__init__.py
+-rw-r--r--   0        0        0     2317 2023-02-23 09:14:02.687958 qpsolvers-3.3.1/qpsolvers/conversions/ensure_sparse_matrices.py
+-rw-r--r--   0        0        0     3561 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/qpsolvers/conversions/linear_from_box_inequalities.py
+-rw-r--r--   0        0        0     3762 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/qpsolvers/conversions/socp_from_qp.py
+-rw-r--r--   0        0        0     2284 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/conversions/split_dual_linear_box.py
+-rw-r--r--   0        0        0     1677 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/qpsolvers/exceptions.py
+-rw-r--r--   0        0        0     8531 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/qpsolvers/problem.py
+-rw-r--r--   0        0        0     6610 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/problems.py
+-rw-r--r--   0        0        0     7795 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solution.py
+-rw-r--r--   0        0        0     7412 2023-03-28 08:42:54.624660 qpsolvers-3.3.1/qpsolvers/solve_ls.py
+-rw-r--r--   0        0        0     3437 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/qpsolvers/solve_problem.py
+-rw-r--r--   0        0        0     4698 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solve_qp.py
+-rw-r--r--   0        0        0     1743 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solve_unconstrained.py
+-rw-r--r--   0        0        0    12032 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/qpsolvers/solvers/__init__.py
+-rw-r--r--   0        0        0     6665 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/clarabel_.py
+-rw-r--r--   0        0        0     9089 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/cvxopt_.py
+-rw-r--r--   0        0        0     6441 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/daqp_.py
+-rw-r--r--   0        0        0     8434 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/ecos_.py
+-rw-r--r--   0        0        0     7813 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/gurobi_.py
+-rw-r--r--   0        0        0     9571 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/highs_.py
+-rw-r--r--   0        0        0     9733 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/osqp_.py
+-rw-r--r--   0        0        0     9807 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/proxqp_.py
+-rw-r--r--   0        0        0    13544 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/qpoases_.py
+-rw-r--r--   0        0        0    10619 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/qpswift_.py
+-rw-r--r--   0        0        0     6046 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/quadprog_.py
+-rw-r--r--   0        0        0     9904 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/scs_.py
+-rw-r--r--   0        0        0     2808 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/qpsolvers/unsupported/__init__.py
+-rw-r--r--   0        0        0     4274 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/unsupported/mosek_.py
+-rw-r--r--   0        0        0     6453 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/unsupported/nppro_.py
+-rw-r--r--   0        0        0     2390 2023-02-28 13:27:49.518364 qpsolvers-3.3.1/qpsolvers/utils.py
+-rw-r--r--   0        0        0       59 2021-04-09 11:14:24.912320 qpsolvers-3.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2612 2023-03-28 08:42:54.628660 qpsolvers-3.3.1/tests/problems.py
+-rw-r--r--   0        0        0     2214 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/tests/test_clarabel.py
+-rw-r--r--   0        0        0     3681 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_conversions.py
+-rw-r--r--   0        0        0     3940 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/tests/test_cvxopt.py
+-rw-r--r--   0        0        0     1370 2023-03-31 12:30:36.615914 qpsolvers-3.3.1/tests/test_ecos.py
+-rw-r--r--   0        0        0     1527 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_gurobi.py
+-rw-r--r--   0        0        0     1773 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_highs.py
+-rw-r--r--   0        0        0     1377 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_mosek.py
+-rw-r--r--   0        0        0     1348 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/tests/test_nppro.py
+-rw-r--r--   0        0        0     1370 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_osqp.py
+-rw-r--r--   0        0        0     3584 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/tests/test_problem.py
+-rw-r--r--   0        0        0     3570 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_proxqp.py
+-rw-r--r--   0        0        0     3191 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_qpoases.py
+-rw-r--r--   0        0        0     1733 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_qpswift.py
+-rw-r--r--   0        0        0     2332 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_quadprog.py
+-rw-r--r--   0        0        0     1695 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_scs.py
+-rw-r--r--   0        0        0     2640 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_solution.py
+-rw-r--r--   0        0        0     9194 2023-03-28 08:42:54.628660 qpsolvers-3.3.1/tests/test_solve_ls.py
+-rw-r--r--   0        0        0    11123 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/tests/test_solve_problem.py
+-rw-r--r--   0        0        0    25373 2023-03-31 12:28:59.113529 qpsolvers-3.3.1/tests/test_solve_qp.py
+-rw-r--r--   0        0        0     3012 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_unfeasible_problem.py
+-rw-r--r--   0        0        0     1865 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2426 2023-04-12 09:42:35.095945 qpsolvers-3.3.1/tox.ini
+-rw-r--r--   0        0        0    11721 1970-01-01 00:00:00.000000 qpsolvers-3.3.1/PKG-INFO
```

### Comparing `qpsolvers-3.3.0/.github/workflows/docs.yml` & `qpsolvers-3.3.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/.github/workflows/test.yml` & `qpsolvers-3.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/CHANGELOG.md` & `qpsolvers-3.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [3.3.1] - 2023/04/12
+
+### Fixed
+
+- DAQP: Update to 0.5.1 to fix installation of arm64 wheels
+
 ## [3.3.0] - 2023/04/11
 
 ### Added
 
 - New sample problems in ``qpsolvers.problems``
 - New solver: [DAQP](https://darnstrom.github.io/daqp/) (thanks to @darnstrom)
```

### Comparing `qpsolvers-3.3.0/CONTRIBUTING.md` & `qpsolvers-3.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/LICENSE` & `qpsolvers-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/README.md` & `qpsolvers-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/THANKS` & `qpsolvers-3.3.1/THANKS`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/benchmark/benchmark_dense_problem.py` & `qpsolvers-3.3.1/benchmark/benchmark_dense_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/benchmark/benchmark_model_predictive_control.py` & `qpsolvers-3.3.1/benchmark/benchmark_model_predictive_control.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/benchmark/benchmark_random_problems.py` & `qpsolvers-3.3.1/benchmark/benchmark_random_problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/benchmark/benchmark_sparse_problem.py` & `qpsolvers-3.3.1/benchmark/benchmark_sparse_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/conf.py` & `qpsolvers-3.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/developer-notes.rst` & `qpsolvers-3.3.1/doc/developer-notes.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/index.rst` & `qpsolvers-3.3.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/installation.rst` & `qpsolvers-3.3.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/least-squares.rst` & `qpsolvers-3.3.1/doc/least-squares.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/quadratic-programming.rst` & `qpsolvers-3.3.1/doc/quadratic-programming.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/references.rst` & `qpsolvers-3.3.1/doc/references.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/doc/supported-solvers.rst` & `qpsolvers-3.3.1/doc/supported-solvers.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/README.md` & `qpsolvers-3.3.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/box_inequalities.py` & `qpsolvers-3.3.1/examples/box_inequalities.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/constrained_linear_regression.py` & `qpsolvers-3.3.1/examples/constrained_linear_regression.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/dual_multipliers.py` & `qpsolvers-3.3.1/examples/dual_multipliers.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/least_squares.py` & `qpsolvers-3.3.1/examples/least_squares.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/model_predictive_control.py` & `qpsolvers-3.3.1/examples/model_predictive_control.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/quadratic_program.py` & `qpsolvers-3.3.1/examples/quadratic_program.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/examples/sparse_least_squares.py` & `qpsolvers-3.3.1/examples/sparse_least_squares.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/pyproject.toml` & `qpsolvers-3.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
-    "daqp >=0.5.0",
+    "daqp >=0.5.1",
     "ecos >=2.0.8",
     "numpy >=1.15.4",
     "osqp >=0.6.2",
     "scipy >=1.2.0",
     "scs >=3.2.0",
 ]
 keywords = ["quadratic programming", "solver", "numerical optimization"]
```

### Comparing `qpsolvers-3.3.0/qpsolvers/__init__.py` & `qpsolvers-3.3.1/qpsolvers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     quadprog_solve_qp,
     scs_solve_qp,
     sparse_solvers,
 )
 from .unsupported import mosek_solve_qp, nppro_solve_qp
 from .utils import print_matrix_vector
 
-__version__ = "3.3.0"
+__version__ = "3.3.1"
 
 __all__ = [
     "NoSolverSelected",
     "ParamError",
     "Problem",
     "ProblemError",
     "QPError",
```

### Comparing `qpsolvers-3.3.0/qpsolvers/_internals.py` & `qpsolvers-3.3.1/qpsolvers/_internals.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/conversions/__init__.py` & `qpsolvers-3.3.1/qpsolvers/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/conversions/ensure_sparse_matrices.py` & `qpsolvers-3.3.1/qpsolvers/conversions/ensure_sparse_matrices.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/conversions/linear_from_box_inequalities.py` & `qpsolvers-3.3.1/qpsolvers/conversions/linear_from_box_inequalities.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/conversions/socp_from_qp.py` & `qpsolvers-3.3.1/qpsolvers/conversions/socp_from_qp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/conversions/split_dual_linear_box.py` & `qpsolvers-3.3.1/qpsolvers/conversions/split_dual_linear_box.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/exceptions.py` & `qpsolvers-3.3.1/qpsolvers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/problem.py` & `qpsolvers-3.3.1/qpsolvers/problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/problems.py` & `qpsolvers-3.3.1/qpsolvers/problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solution.py` & `qpsolvers-3.3.1/qpsolvers/solution.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solve_ls.py` & `qpsolvers-3.3.1/qpsolvers/solve_ls.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solve_problem.py` & `qpsolvers-3.3.1/qpsolvers/solve_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solve_qp.py` & `qpsolvers-3.3.1/qpsolvers/solve_qp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solve_unconstrained.py` & `qpsolvers-3.3.1/qpsolvers/solve_unconstrained.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/__init__.py` & `qpsolvers-3.3.1/qpsolvers/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/clarabel_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/clarabel_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/cvxopt_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/cvxopt_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/daqp_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/daqp_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/ecos_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/ecos_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/gurobi_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/gurobi_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/highs_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/highs_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/osqp_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/osqp_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/proxqp_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/proxqp_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/qpoases_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/qpoases_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/qpswift_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/qpswift_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/quadprog_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/quadprog_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/solvers/scs_.py` & `qpsolvers-3.3.1/qpsolvers/solvers/scs_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/unsupported/__init__.py` & `qpsolvers-3.3.1/qpsolvers/unsupported/__init__.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/unsupported/mosek_.py` & `qpsolvers-3.3.1/qpsolvers/unsupported/mosek_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/unsupported/nppro_.py` & `qpsolvers-3.3.1/qpsolvers/unsupported/nppro_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/qpsolvers/utils.py` & `qpsolvers-3.3.1/qpsolvers/utils.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/problems.py` & `qpsolvers-3.3.1/tests/problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_clarabel.py` & `qpsolvers-3.3.1/tests/test_clarabel.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_conversions.py` & `qpsolvers-3.3.1/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_cvxopt.py` & `qpsolvers-3.3.1/tests/test_cvxopt.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_ecos.py` & `qpsolvers-3.3.1/tests/test_ecos.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_gurobi.py` & `qpsolvers-3.3.1/tests/test_gurobi.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_highs.py` & `qpsolvers-3.3.1/tests/test_highs.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_mosek.py` & `qpsolvers-3.3.1/tests/test_mosek.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_nppro.py` & `qpsolvers-3.3.1/tests/test_nppro.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_osqp.py` & `qpsolvers-3.3.1/tests/test_osqp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_problem.py` & `qpsolvers-3.3.1/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_proxqp.py` & `qpsolvers-3.3.1/tests/test_proxqp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_qpoases.py` & `qpsolvers-3.3.1/tests/test_qpoases.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_qpswift.py` & `qpsolvers-3.3.1/tests/test_qpswift.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_quadprog.py` & `qpsolvers-3.3.1/tests/test_quadprog.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_scs.py` & `qpsolvers-3.3.1/tests/test_scs.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_solution.py` & `qpsolvers-3.3.1/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_solve_ls.py` & `qpsolvers-3.3.1/tests/test_solve_ls.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_solve_problem.py` & `qpsolvers-3.3.1/tests/test_solve_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_solve_qp.py` & `qpsolvers-3.3.1/tests/test_solve_qp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_unfeasible_problem.py` & `qpsolvers-3.3.1/tests/test_unfeasible_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tests/test_utils.py` & `qpsolvers-3.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.0/tox.ini` & `qpsolvers-3.3.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     macos-latest: macos
     windows-latest: windows
 
 [testenv]
 deps =
     clarabel >=0.4.1
     cvxopt >=1.2.6
-    daqp >=0.5.0
+    daqp >=0.5.1
     ecos >=2.0.8
     gurobipy >=9.5.2
     numpy <1.24.0
     osqp >=0.6.2
     quadprog >=0.1.11
     scipy >=1.2.0
     scs >=3.2.0
@@ -35,15 +35,15 @@
     python -m unittest discover
 
 [testenv:coverage]
 deps =
     clarabel >=0.4.1
     coverage >=5.5
     cvxopt >=1.2.6
-    daqp >=0.5.0
+    daqp >=0.5.1
     ecos >=2.0.8
     gurobipy >=9.5.2
     highspy >=1.1.2.dev3
     numpy <1.24.0
     osqp >=0.6.2
     proxsuite >=0.3.1
     quadprog >=0.1.11
```

### Comparing `qpsolvers-3.3.0/PKG-INFO` & `qpsolvers-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpsolvers
-Version: 3.3.0
+Version: 3.3.1
 Summary: Quadratic programming solvers in Python with a unified API.
 Keywords: quadratic programming,solver,numerical optimization
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Dist: daqp >=0.5.0
+Requires-Dist: daqp >=0.5.1
 Requires-Dist: ecos >=2.0.8
 Requires-Dist: numpy >=1.15.4
 Requires-Dist: osqp >=0.6.2
 Requires-Dist: scipy >=1.2.0
 Requires-Dist: scs >=3.2.0
 Requires-Dist: clarabel >=0.4.1 ; extra == "open_source_solvers"
 Requires-Dist: cvxopt >=1.2.6 ; extra == "open_source_solvers"
```

