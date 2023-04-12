# Comparing `tmp/GPyReg-1.0.0.tar.gz` & `tmp/GPyReg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPyReg-1.0.0.tar", last modified: Thu Mar 16 12:34:47 2023, max compression
+gzip compressed data, was "GPyReg-1.0.1.tar", last modified: Wed Apr 12 20:22:10 2023, max compression
```

## Comparing `GPyReg-1.0.0.tar` & `GPyReg-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:34:47.167924 GPyReg-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:34:47.147924 GPyReg-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:34:47.155924 GPyReg-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.github/workflows/merge-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-16 12:34:36.000000 GPyReg-1.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:34:47.155924 GPyReg-1.0.0/GPyReg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-03-16 12:34:47.000000 GPyReg-1.0.0/GPyReg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-16 12:34:47.000000 GPyReg-1.0.0/GPyReg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 12:34:47.000000 GPyReg-1.0.0/GPyReg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-16 12:34:47.000000 GPyReg-1.0.0/GPyReg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 12:34:47.000000 GPyReg-1.0.0/GPyReg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-16 12:34:36.000000 GPyReg-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-16 12:34:36.000000 GPyReg-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-03-16 12:34:47.163924 GPyReg-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-03-16 12:34:36.000000 GPyReg-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-16 12:34:36.000000 GPyReg-1.0.0/coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-16 12:34:36.000000 GPyReg-1.0.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-16 12:34:36.000000 GPyReg-1.0.0/environment_pure_conda.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:34:47.159924 GPyReg-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-16 12:34:36.000000 GPyReg-1.0.0/examples/example_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-03-16 12:34:36.000000 GPyReg-1.0.0/examples/example_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:34:47.163924 GPyReg-1.0.0/gpyreg/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/covariance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/f_min_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    92330 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/noise_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30718 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/slice_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:34:47.163924 GPyReg-1.0.0/gpyreg/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/test_covariance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35700 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/test_gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/test_mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/test_noise_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/test_slice_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/test_smoothbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-16 12:34:36.000000 GPyReg-1.0.0/gpyreg/testing/test_smoothbox_student_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    19388 2023-03-16 12:34:36.000000 GPyReg-1.0.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-16 12:34:36.000000 GPyReg-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 12:34:47.167924 GPyReg-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-16 12:34:36.000000 GPyReg-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.716208 GPyReg-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.708208 GPyReg-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/merge-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 20:22:00.000000 GPyReg-1.0.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/GPyReg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 20:22:10.000000 GPyReg-1.0.1/GPyReg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 20:22:00.000000 GPyReg-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 20:22:00.000000 GPyReg-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 20:22:10.712208 GPyReg-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-12 20:22:00.000000 GPyReg-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-12 20:22:00.000000 GPyReg-1.0.1/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 20:22:00.000000 GPyReg-1.0.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 20:22:00.000000 GPyReg-1.0.1/environment_pure_conda.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 20:22:00.000000 GPyReg-1.0.1/examples/example_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 20:22:00.000000 GPyReg-1.0.1/examples/example_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/gpyreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/f_min_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92330 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/isotropic_covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/noise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30718 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/slice_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:22:10.712208 GPyReg-1.0.1/gpyreg/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35700 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_gaussian_process_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_isotropic_covariance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_noise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_slice_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_smoothbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-12 20:22:00.000000 GPyReg-1.0.1/gpyreg/testing/test_smoothbox_student_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19388 2023-04-12 20:22:00.000000 GPyReg-1.0.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-12 20:22:00.000000 GPyReg-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:22:10.716208 GPyReg-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 20:22:00.000000 GPyReg-1.0.1/setup.py
```

### Comparing `GPyReg-1.0.0/.github/workflows/docs.yml` & `GPyReg-1.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/.github/workflows/merge-tests.yml` & `GPyReg-1.0.1/.github/workflows/merge-tests.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/.github/workflows/release.yml` & `GPyReg-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/.github/workflows/tests.yml` & `GPyReg-1.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/.gitignore` & `GPyReg-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/.pre-commit-config.yaml` & `GPyReg-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/GPyReg.egg-info/PKG-INFO` & `GPyReg-1.0.1/GPyReg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyReg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lightweight package for Gaussian process regression.
 License: BSD 3-Clause License
         
         Copyright (c) 2021, GPyReg Developers and their Assignees
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `GPyReg-1.0.0/GPyReg.egg-info/SOURCES.txt` & `GPyReg-1.0.1/GPyReg.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,21 @@
 examples/example_1.py
 examples/example_2.py
 gpyreg/__init__.py
 gpyreg/covariance_functions.py
 gpyreg/f_min_fill.py
 gpyreg/formatting.py
 gpyreg/gaussian_process.py
+gpyreg/isotropic_covariance_functions.py
 gpyreg/mean_functions.py
 gpyreg/noise_functions.py
 gpyreg/slice_sample.py
 gpyreg/testing/__init__.py
 gpyreg/testing/test_covariance_functions.py
 gpyreg/testing/test_gaussian_process.py
+gpyreg/testing/test_gaussian_process_isotropic.py
+gpyreg/testing/test_isotropic_covariance_functions.py
 gpyreg/testing/test_mean_functions.py
 gpyreg/testing/test_noise_functions.py
 gpyreg/testing/test_slice_sample.py
 gpyreg/testing/test_smoothbox.py
 gpyreg/testing/test_smoothbox_student_t.py
```

### Comparing `GPyReg-1.0.0/LICENSE` & `GPyReg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/PKG-INFO` & `GPyReg-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyReg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lightweight package for Gaussian process regression.
 License: BSD 3-Clause License
         
         Copyright (c) 2021, GPyReg Developers and their Assignees
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `GPyReg-1.0.0/README.md` & `GPyReg-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/examples/example_1.py` & `GPyReg-1.0.1/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/examples/example_2.py` & `GPyReg-1.0.1/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/covariance_functions.py` & `GPyReg-1.0.1/gpyreg/covariance_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,14 +165,16 @@
                 tmp = squareform(pdist(X / ell, "sqeuclidean"))
         else:
             tmp = cdist(X / ell, X_star / ell, "sqeuclidean")
 
         K = sf2 * np.exp(-tmp / 2)
 
         if compute_grad:
+            if X_star is not None:
+                raise ValueError("X_star should be None when compute_grad is True.")
             dK = np.zeros((cov_N, N, N))
             for i in range(0, D):
                 # Gradient of cov length scales
                 dK[i, :, :] = K * squareform(
                     pdist(np.reshape(X[:, i] / ell[i], (-1, 1)), "sqeuclidean")
                 )
             # Gradient of cov output scale.
@@ -251,14 +253,16 @@
             a = X @ np.diag(np.sqrt(self.degree) / ell)
             b = X_star @ np.diag(np.sqrt(self.degree) / ell)
             tmp = cdist(a, b)
 
         K = sf2 * self.f(tmp) * np.exp(-tmp)
 
         if compute_grad:
+            if X_star is not None:
+                raise ValueError("X_star should be None when compute_grad is True.")
             dK = np.zeros((cov_N, N, N))
             for i in range(0, D):
                 Ki = squareform(
                     pdist(
                         np.reshape(
                             np.sqrt(self.degree) / ell[i] * X[:, i], (-1, 1)
                         ),
@@ -327,14 +331,16 @@
             b = X_star @ np.diag(1.0 / ell)
             tmp = cdist(a, b, "sqeuclidean")
 
         M = 1 + 0.5 * tmp / alpha
         K = sf2 * M ** (-alpha)
 
         if compute_grad:
+            if X_star is not None:
+                raise ValueError("X_star should be None when compute_grad is True.")
             dK = np.zeros((cov_N, N, N))
 
             # Gradient respect of lenght scale.
             for i in range(0, D):
                 Ki = squareform(
                     pdist(
                         np.reshape(1.0 / ell[i] * X[:, i], (-1, 1)),
```

### Comparing `GPyReg-1.0.0/gpyreg/f_min_fill.py` & `GPyReg-1.0.1/gpyreg/f_min_fill.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/formatting.py` & `GPyReg-1.0.1/gpyreg/formatting.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/gaussian_process.py` & `GPyReg-1.0.1/gpyreg/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/mean_functions.py` & `GPyReg-1.0.1/gpyreg/mean_functions.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/noise_functions.py` & `GPyReg-1.0.1/gpyreg/noise_functions.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/slice_sample.py` & `GPyReg-1.0.1/gpyreg/slice_sample.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/testing/test_covariance_functions.py` & `GPyReg-1.0.1/gpyreg/testing/test_covariance_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 def test_squared_exponential_compute_sanity_checks():
     squared_expontential = SquaredExponential()
     D = 3
     N = 20
     X = np.ones((N, D))
+    X_star = np.zeros((N, D))
 
     with pytest.raises(ValueError) as execinfo:
         hyp = np.ones(D + 2)
         squared_expontential.compute(hyp, X)
     assert (
         "Expected 4 covariance function hyperparameters"
         in execinfo.value.args[0]
@@ -25,14 +26,21 @@
     with pytest.raises(ValueError) as execinfo:
         hyp = np.ones((D + 1, 1))
         squared_expontential.compute(hyp, X)
     assert (
         "Covariance function output is available only for"
         in execinfo.value.args[0]
     )
+    with pytest.raises(ValueError) as execinfo:
+        hyp = np.ones(D + 1)
+        squared_expontential.compute(hyp, X, X_star, compute_grad=True)
+    assert (
+        "X_star should be None when compute_grad is True."
+        in execinfo.value.args[0]
+    )
 
 
 def test_sqr_exp_kernel_gradient():
     sqr_exp = SquaredExponential()
     D = 3
     N = 20
     diag_cov = np.eye(N) * (0.2)
@@ -44,14 +52,15 @@
 
 
 def test_matern_compute_sanity_checks():
     matern = Matern(3)
     D = 3
     N = 20
     X = np.ones((N, D))
+    X_star = np.zeros((N, D))
 
     with pytest.raises(ValueError) as execinfo:
         hyp = np.ones(D + 2)
         matern.compute(hyp, X)
     assert (
         "Expected 4 covariance function hyperparameters"
         in execinfo.value.args[0]
@@ -59,14 +68,21 @@
     with pytest.raises(ValueError) as execinfo:
         hyp = np.ones((D + 1, 1))
         matern.compute(hyp, X)
     assert (
         "Covariance function output is available only for"
         in execinfo.value.args[0]
     )
+    with pytest.raises(ValueError) as execinfo:
+        hyp = np.ones(D + 1)
+        matern.compute(hyp, X, X_star, compute_grad=True)
+    assert (
+        "X_star should be None when compute_grad is True."
+        in execinfo.value.args[0]
+    )
 
 
 def test_matern_invalid_degree():
     for degree in [0, 2, 4, 6]:
         with pytest.raises(ValueError) as execinfo:
             Matern(degree)
         assert (
```

### Comparing `GPyReg-1.0.0/gpyreg/testing/test_gaussian_process.py` & `GPyReg-1.0.1/gpyreg/testing/test_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/testing/test_mean_functions.py` & `GPyReg-1.0.1/gpyreg/testing/test_mean_functions.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/testing/test_noise_functions.py` & `GPyReg-1.0.1/gpyreg/testing/test_noise_functions.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/testing/test_slice_sample.py` & `GPyReg-1.0.1/gpyreg/testing/test_slice_sample.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/testing/test_smoothbox.py` & `GPyReg-1.0.1/gpyreg/testing/test_smoothbox.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/gpyreg/testing/test_smoothbox_student_t.py` & `GPyReg-1.0.1/gpyreg/testing/test_smoothbox_student_t.py`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/pylintrc` & `GPyReg-1.0.1/pylintrc`

 * *Files identical despite different names*

### Comparing `GPyReg-1.0.0/pyproject.toml` & `GPyReg-1.0.1/pyproject.toml`

 * *Files identical despite different names*

