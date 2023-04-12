# Comparing `tmp/claspy-0.1.6.tar.gz` & `tmp/claspy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claspy-0.1.6.tar", last modified: Sat Mar 18 16:33:42 2023, max compression
+gzip compressed data, was "claspy-0.1.7.tar", last modified: Wed Apr 12 08:02:33 2023, max compression
```

## Comparing `claspy-0.1.6.tar` & `claspy-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-03-18 16:33:42.172392 claspy-0.1.6/
--rw-r--r--   0 ermshaua   (501) staff       (20)     1500 2023-02-18 10:38:44.000000 claspy-0.1.6/LICENSE
--rw-r--r--   0 ermshaua   (501) staff       (20)     6713 2023-03-18 16:33:42.172615 claspy-0.1.6/PKG-INFO
--rw-r--r--   0 ermshaua   (501) staff       (20)     3917 2023-03-06 20:15:55.000000 claspy-0.1.6/README.md
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-03-18 16:33:42.160922 claspy-0.1.6/claspy/
--rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-18 10:41:51.000000 claspy-0.1.6/claspy/__init__.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    14597 2023-03-05 16:49:44.000000 claspy-0.1.6/claspy/clasp.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     4495 2023-02-26 13:47:51.000000 claspy-0.1.6/claspy/data_loader.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6456 2023-03-05 16:43:36.000000 claspy-0.1.6/claspy/distance.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    12481 2023-03-06 07:43:49.000000 claspy-0.1.6/claspy/nearest_neighbour.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6099 2023-02-25 09:43:02.000000 claspy-0.1.6/claspy/scoring.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    14640 2023-03-05 16:49:50.000000 claspy-0.1.6/claspy/segmentation.py
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-03-18 16:33:42.171666 claspy-0.1.6/claspy/tests/
--rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-20 16:05:58.000000 claspy-0.1.6/claspy/tests/__init__.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2432 2023-03-05 17:32:09.000000 claspy-0.1.6/claspy/tests/clasp_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6600 2023-02-24 12:09:02.000000 claspy-0.1.6/claspy/tests/evaluation.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2515 2023-03-05 17:28:16.000000 claspy-0.1.6/claspy/tests/nearest_neighbour_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2747 2023-03-05 17:32:09.000000 claspy-0.1.6/claspy/tests/segmentation_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     1683 2023-02-28 15:56:43.000000 claspy-0.1.6/claspy/utils.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2905 2023-02-25 10:32:45.000000 claspy-0.1.6/claspy/validation.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6991 2023-02-28 19:59:17.000000 claspy-0.1.6/claspy/window_size.py
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-03-18 16:33:42.168156 claspy-0.1.6/claspy.egg-info/
--rw-r--r--   0 ermshaua   (501) staff       (20)     6713 2023-03-18 16:33:42.000000 claspy-0.1.6/claspy.egg-info/PKG-INFO
--rw-r--r--   0 ermshaua   (501) staff       (20)      585 2023-03-18 16:33:42.000000 claspy-0.1.6/claspy.egg-info/SOURCES.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-03-18 16:33:42.000000 claspy-0.1.6/claspy.egg-info/dependency_links.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-03-18 16:33:42.000000 claspy-0.1.6/claspy.egg-info/not-zip-safe
--rw-r--r--   0 ermshaua   (501) staff       (20)      137 2023-03-18 16:33:42.000000 claspy-0.1.6/claspy.egg-info/requires.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        7 2023-03-18 16:33:42.000000 claspy-0.1.6/claspy.egg-info/top_level.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)     1560 2023-03-18 16:30:06.000000 claspy-0.1.6/pyproject.toml
--rw-r--r--   0 ermshaua   (501) staff       (20)       79 2023-03-18 16:33:42.173560 claspy-0.1.6/setup.cfg
--rw-r--r--   0 ermshaua   (501) staff       (20)     1375 2023-03-04 15:50:17.000000 claspy-0.1.6/setup.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.903123 claspy-0.1.7/
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1500 2023-02-18 10:38:44.000000 claspy-0.1.7/LICENSE
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:02:33.903329 claspy-0.1.7/PKG-INFO
+-rw-r--r--   0 ermshaua   (501) staff       (20)     4084 2023-03-29 19:08:59.000000 claspy-0.1.7/README.md
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.894555 claspy-0.1.7/claspy/
+-rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-18 10:41:51.000000 claspy-0.1.7/claspy/__init__.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    16928 2023-04-11 17:01:12.000000 claspy-0.1.7/claspy/clasp.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     4495 2023-02-26 13:47:51.000000 claspy-0.1.7/claspy/data_loader.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6456 2023-03-05 16:43:36.000000 claspy-0.1.7/claspy/distance.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    15830 2023-04-12 07:38:40.000000 claspy-0.1.7/claspy/nearest_neighbour.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6099 2023-02-25 09:43:02.000000 claspy-0.1.7/claspy/scoring.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    14897 2023-04-12 07:43:17.000000 claspy-0.1.7/claspy/segmentation.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.902375 claspy-0.1.7/claspy/tests/
+-rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-20 16:05:58.000000 claspy-0.1.7/claspy/tests/__init__.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2560 2023-04-12 07:27:07.000000 claspy-0.1.7/claspy/tests/clasp_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6600 2023-02-24 12:09:02.000000 claspy-0.1.7/claspy/tests/evaluation.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2569 2023-04-12 07:25:30.000000 claspy-0.1.7/claspy/tests/nearest_neighbour_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2937 2023-04-12 07:43:17.000000 claspy-0.1.7/claspy/tests/segmentation_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1683 2023-02-28 15:56:43.000000 claspy-0.1.7/claspy/utils.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2918 2023-04-03 15:59:10.000000 claspy-0.1.7/claspy/validation.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6991 2023-02-28 19:59:17.000000 claspy-0.1.7/claspy/window_size.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.898413 claspy-0.1.7/claspy.egg-info/
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/PKG-INFO
+-rw-r--r--   0 ermshaua   (501) staff       (20)      585 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/SOURCES.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/dependency_links.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/not-zip-safe
+-rw-r--r--   0 ermshaua   (501) staff       (20)      137 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/requires.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        7 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/top_level.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1560 2023-04-12 07:45:54.000000 claspy-0.1.7/pyproject.toml
+-rw-r--r--   0 ermshaua   (501) staff       (20)       79 2023-04-12 08:02:33.904149 claspy-0.1.7/setup.cfg
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1376 2023-04-12 07:43:17.000000 claspy-0.1.7/setup.py
```

### Comparing `claspy-0.1.6/LICENSE` & `claspy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/PKG-INFO` & `claspy-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claspy
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/ermshaua/claspy
 Author: Arik Ermshaus
 Author-email: Arik Ermshaus <ermshaua@informatik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Arik Ermshaus
         
@@ -92,14 +92,15 @@
 
 ## Examples
 
 Checkout the following Jupyter notebooks that show applications of the ClaSPy package:
 
 - <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/tssb_evaluation.ipynb">ClaSP evaluation on the "Time Series Segmentation Benchmark" (TSSB)</a>
 - <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/clasp_configuration.ipynb">Hyper-parameter Tuning and Configuration of ClaSP</a>
+- <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/window_size_selection.ipynb">Window Size Selection for Unsupervised Time Series Analytics</a>
 
 ## Citation
 
 The ClaSPy package is actively maintained, updated and intended for application. If you use ClaSP in your scientific publication, we would appreciate the following <a href="https://doi.org/10.1007/s10618-023-00923-x" target="_blank">citation</a>:
 
 ```
 @article{clasp2023,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: claspy Version: 0.1.6 Home-page: https://
+Metadata-Version: 2.1 Name: claspy Version: 0.1.7 Home-page: https://
 github.com/ermshaua/claspy Author: Arik Ermshaus Author-email: Arik Ermshaus
 informatik.hu-berlin.de> License: BSD 3-Clause License Copyright (c) 2023, Arik
 Ermshaus Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -61,17 +61,18 @@
 accurately detects the number and location of changes in the motion sequence
 (compare green vs red lines) that infer its segmentation (the different-
 coloured subsequences). It is carefully designed to do this fully autonomously.
 However, if you have domain-specific knowledge, you can utilize it to guide and
 improve the segmentation. See its parameters for more information. ## Examples
 Checkout the following Jupyter notebooks that show applications of the ClaSPy
 package: - ClaSP_evaluation_on_the_"Time_Series_Segmentation_Benchmark"_(TSSB)
-- Hyper-parameter_Tuning_and_Configuration_of_ClaSP ## Citation The ClaSPy
-package is actively maintained, updated and intended for application. If you
-use ClaSP in your scientific publication, we would appreciate the following
-citation: ``` @article{clasp2023, title={ClaSP: parameter-free time series
-segmentation}, author={Arik Ermshaus and Patrick Sch{\"a}fer and Ulf Leser},
-journal={Data Mining and Knowledge Discovery}, year={2023}, } ``` ## Todos Here
-are some of the things we would like to add to ClaSPy in the future: - Future
-research related to ClaSP - Example and application Jupyter notebooks - More
+- Hyper-parameter_Tuning_and_Configuration_of_ClaSP - Window_Size_Selection_for
+Unsupervised_Time_Series_Analytics ## Citation The ClaSPy package is actively
+maintained, updated and intended for application. If you use ClaSP in your
+scientific publication, we would appreciate the following citation: ```
+@article{clasp2023, title={ClaSP: parameter-free time series segmentation},
+author={Arik Ermshaus and Patrick Sch{\"a}fer and Ulf Leser}, journal={Data
+Mining and Knowledge Discovery}, year={2023}, } ``` ## Todos Here are some of
+the things we would like to add to ClaSPy in the future: - Future research
+related to ClaSP - Example and application Jupyter notebooks - More
 documentation and tests If you want to contribute, report bugs, or need help
 applying ClaSP for your application, feel free to reach out.
```

### Comparing `claspy-0.1.6/README.md` & `claspy-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 ## Examples
 
 Checkout the following Jupyter notebooks that show applications of the ClaSPy package:
 
 - <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/tssb_evaluation.ipynb">ClaSP evaluation on the "Time Series Segmentation Benchmark" (TSSB)</a>
 - <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/clasp_configuration.ipynb">Hyper-parameter Tuning and Configuration of ClaSP</a>
+- <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/window_size_selection.ipynb">Window Size Selection for Unsupervised Time Series Analytics</a>
 
 ## Citation
 
 The ClaSPy package is actively maintained, updated and intended for application. If you use ClaSP in your scientific publication, we would appreciate the following <a href="https://doi.org/10.1007/s10618-023-00923-x" target="_blank">citation</a>:
 
 ```
 @article{clasp2023,
```

#### html2text {}

```diff
@@ -28,17 +28,18 @@
 number and location of changes in the motion sequence (compare green vs red
 lines) that infer its segmentation (the different-coloured subsequences). It is
 carefully designed to do this fully autonomously. However, if you have domain-
 specific knowledge, you can utilize it to guide and improve the segmentation.
 See its parameters for more information. ## Examples Checkout the following
 Jupyter notebooks that show applications of the ClaSPy package: - ClaSP
 evaluation_on_the_"Time_Series_Segmentation_Benchmark"_(TSSB) - Hyper-parameter
-Tuning_and_Configuration_of_ClaSP ## Citation The ClaSPy package is actively
-maintained, updated and intended for application. If you use ClaSP in your
-scientific publication, we would appreciate the following citation: ```
-@article{clasp2023, title={ClaSP: parameter-free time series segmentation},
-author={Arik Ermshaus and Patrick Sch{\"a}fer and Ulf Leser}, journal={Data
-Mining and Knowledge Discovery}, year={2023}, } ``` ## Todos Here are some of
-the things we would like to add to ClaSPy in the future: - Future research
-related to ClaSP - Example and application Jupyter notebooks - More
-documentation and tests If you want to contribute, report bugs, or need help
-applying ClaSP for your application, feel free to reach out.
+Tuning_and_Configuration_of_ClaSP - Window_Size_Selection_for_Unsupervised_Time
+Series_Analytics ## Citation The ClaSPy package is actively maintained, updated
+and intended for application. If you use ClaSP in your scientific publication,
+we would appreciate the following citation: ``` @article{clasp2023, title=
+{ClaSP: parameter-free time series segmentation}, author={Arik Ermshaus and
+Patrick Sch{\"a}fer and Ulf Leser}, journal={Data Mining and Knowledge
+Discovery}, year={2023}, } ``` ## Todos Here are some of the things we would
+like to add to ClaSPy in the future: - Future research related to ClaSP -
+Example and application Jupyter notebooks - More documentation and tests If you
+want to contribute, report bugs, or need help applying ClaSP for your
+application, feel free to reach out.
```

### Comparing `claspy-0.1.6/claspy/clasp.py` & `claspy-0.1.7/claspy/clasp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,86 @@
+import os
+
 import numpy as np
-from numba import njit
+from numba import njit, prange
+from numba.typed.typedlist import List
 from sklearn.exceptions import NotFittedError
 
 from claspy.nearest_neighbour import KSubsequenceNeighbours
 from claspy.nearest_neighbour import cross_val_labels
 from claspy.scoring import map_scores
 from claspy.utils import check_input_time_series, check_excl_radius
 from claspy.validation import map_validation_tests
 
 
 @njit(fastmath=True, cache=False)
-def _profile(offsets, window_size, score, min_seg_size):
+def _profile(offsets, start, end, window_size, score):
     """
     Computes the classification score profile given nearest neighbour offsets.
 
     Parameters
     ----------
     offsets : np.ndarray
         An array of shape (n_timepoints, k_neighbors) containing the offsets of the k nearest
         neighbors for each timepoint.
+    start : int
+        The first index to consider (inclusive).
+    end : int
+        The last index to consider (exclusive).
     window_size : int
         The size of the window used to calculate nearest neighbours.
     score : callable
         A callable that computes the score of a segmentation given the true and predicted labels.
         The callable must accept two arguments: y_true and y_pred, which are arrays of binary labels
         indicating whether each timepoint belongs to the first or second segment of the segmentation.
-    min_seg_size : int
-        The minimum length of a segment. Segments shorter than this will be ignored.
 
     Returns
     -------
     np.ndarray
-        An array of shape (n_timepoints,) containing the classification score profile.
+        An array of shape (end-start,) containing the classification score profile.
     """
-    n_timepoints, _ = offsets.shape
-    profile = np.full(shape=n_timepoints, fill_value=-np.inf, dtype=np.float64)
+    profile = np.full(shape=end - start, fill_value=-np.inf, dtype=np.float64)
 
-    for split_idx in range(min_seg_size, n_timepoints - min_seg_size):
+    for split_idx in range(start, end):
         y_true, y_pred = cross_val_labels(offsets, split_idx, window_size)
-        profile[split_idx] = score(y_true, y_pred)
+        profile[split_idx - start] = score(y_true, y_pred)
+
+    return profile
+
+
+@njit(fastmath=True, cache=True, parallel=True)
+def _parallel_profile(offsets, pranges, window_size, score):
+    """
+    Computes the classification score profile given nearest neighbour offsets in parallel
+    with n_jobs threads.
+
+    Parameters
+    ----------
+    offsets : np.ndarray
+        An array of shape (n_timepoints, k_neighbors) containing the offsets of the k nearest
+        neighbors for each timepoint.
+    pranges : ndarray of shape (m, 2), where each row is (start, end)
+        Ranges in which the profile scpres are calculated per thread. Infers the number of threads.
+    window_size : int
+        The size of the window used to calculate nearest neighbours.
+    score : callable
+        A callable that computes the score of a segmentation given the true and predicted labels.
+        The callable must accept two arguments: y_true and y_pred, which are arrays of binary labels
+        indicating whether each timepoint belongs to the first or second segment of the segmentation.
+
+    Returns
+    -------
+    np.ndarray
+        An array of shape (n_timepoints,) containing the classification score profile.
+    """
+    profile = np.full(shape=offsets.shape[0], fill_value=-np.inf, dtype=np.float64)
+
+    for idx in prange(len(pranges)):
+        start, end = pranges[idx]
+        profile[start:end] = _profile(offsets, start, end, window_size, score)
 
     return profile
 
 
 class ClaSP:
     """
     An implementation of the ClaSP algorithm for detecting change points in time series data.
@@ -57,35 +95,38 @@
         The name of the distance function to be computed for determining the k-NNs. Available options are
         "znormed_euclidean_distance" and "euclidean_distance".
     score : str or callable, optional
         The name of the classification score to use.
         Available options are "roc_auc", "f1", by default "roc_auc".
     excl_radius : int, optional
         The radius of the exclusion zone around the detected change point, by default 5*window_size.
+    n_jobs : int, optional (default=1)
+        Amount of threads used in the ClaSP computation.
 
     Methods
     -------
     fit(time_series)
         Create a ClaSP for the input time series data.
     predict()
         Return the ClaSP for the input time series data.
     fit_predict(time_series)
         Create and return a ClaSP for the input time series data.
     split()
         Split ClaSP into two segments.
     """
 
     def __init__(self, window_size=10, k_neighbours=3, distance="znormed_euclidean_distance", score="roc_auc",
-                 excl_radius=5):
+                 excl_radius=5, n_jobs=-1):
         self.window_size = window_size
         self.k_neighbours = k_neighbours
         self.distance = distance
         self.score_name = score
         self.score = map_scores(score)
         self.excl_radius = excl_radius
+        self.n_jobs = os.cpu_count() if n_jobs < 1 else n_jobs
         self.is_fitted = False
 
         check_excl_radius(k_neighbours, excl_radius)
 
     def _check_is_fitted(self):
         """
         Checks if the ClaSP object is fitted.
@@ -124,30 +165,45 @@
         Raises
         ------
         ValueError
             If the input time series has less than 2*min_seg_size data points.
         """
         check_input_time_series(time_series)
         self.min_seg_size = self.window_size * self.excl_radius
+        self.lbound, self.ubound = 0, time_series.shape[0]
 
         if time_series.shape[0] < 2 * self.min_seg_size:
             raise ValueError("Time series must at least have 2*min_seg_size data points.")
 
         self.time_series = time_series
 
         if knn is None:
             self.knn = KSubsequenceNeighbours(
                 window_size=self.window_size,
                 k_neighbours=self.k_neighbours,
-                distance=self.distance
+                distance=self.distance,
+                n_jobs=self.n_jobs
             ).fit(time_series)
         else:
             self.knn = knn
 
-        self.profile = _profile(self.knn.offsets, self.window_size, self.score, self.min_seg_size)
+        pranges = List()
+        n_jobs = self.n_jobs
+
+        while self.knn.offsets.shape[0] // n_jobs < self.min_seg_size and n_jobs != 1:
+            n_jobs -= 1
+
+        bin_size = self.knn.offsets.shape[0] // n_jobs
+
+        for idx in range(n_jobs):
+            start = max(idx * bin_size, self.min_seg_size)
+            end = min((idx + 1) * bin_size, self.knn.offsets.shape[0] - self.min_seg_size + self.window_size - 1)
+            if end > start: pranges.append((start, end))
+
+        self.profile = _parallel_profile(self.knn.offsets, pranges, self.window_size, self.score)
 
         self.is_fitted = True
         return self
 
     def transform(self):
         """
         Transform the input time series into a ClaSP profile.
@@ -244,32 +300,32 @@
         The scoring method to use in the profile scoring. Must be a string ("f1" "roc_auc",).
         Default is "roc_auc".
     early_stopping : bool
         Determines if ensembling is stopped, once a validated change point is found or
         the ClaSP models do not improve anymore. Default is True.
     excl_radius : int, optional
         The radius of the exclusion zone in the profile scoring. Default is 5*window_size.
+    n_jobs : int, optional (default=1)
+        Amount of threads used in the ClaSP computation.
     random_state : int or RandomState, optional
         Seed for the random number generator. Default is 2357.
 
     Methods
     -------
     fit(time_series)
         Create a ClaSP ensemble for the input time series data.
     predict()
         Return the ClaSP ensemble for the input time series data.
     fit_predict(time_series)
         Create and return a ClaSP ensemble for the input time series data.
     """
 
     def __init__(self, n_estimators=10, window_size=10, k_neighbours=3, distance="znormed_euclidean_distance",
-                 score="roc_auc", early_stopping=True,
-                 excl_radius=5,
-                 random_state=2357):
-        super().__init__(window_size, k_neighbours, distance, score, excl_radius)
+                 score="roc_auc", early_stopping=True, excl_radius=5, n_jobs=-1, random_state=2357):
+        super().__init__(window_size, k_neighbours, distance, score, excl_radius, n_jobs)
         self.n_estimators = n_estimators
         self.early_stopping = early_stopping
         self.random_state = random_state
 
     def _calculate_temporal_constraints(self):
         """
         Calculates a set of random temporal constraints for each ClaSP in the ensemble.
@@ -336,25 +392,27 @@
         self.time_series = time_series
         tcs = self._calculate_temporal_constraints()
 
         if knn is None:
             knn = KSubsequenceNeighbours(
                 window_size=self.window_size,
                 k_neighbours=self.k_neighbours,
-                distance=self.distance
+                distance=self.distance,
+                n_jobs=self.n_jobs
             ).fit(time_series, temporal_constraints=tcs)
 
         best_score, best_tc, best_clasp = -np.inf, None, None
 
         for idx, (lbound, ubound) in enumerate(tcs):
             clasp = ClaSP(
                 window_size=self.window_size,
                 k_neighbours=self.k_neighbours,
                 score=self.score_name,
-                excl_radius=self.excl_radius
+                excl_radius=self.excl_radius,
+                n_jobs=self.n_jobs
             ).fit(time_series[lbound:ubound], knn=knn.constrain(lbound, ubound))
 
             clasp.profile = (clasp.profile + (ubound - lbound) / time_series.shape[0]) / 2
 
             if clasp.profile.max() > best_score or best_clasp is None and idx == tcs.shape[0] - 1:
                 best_score = clasp.profile.max()
                 best_tc = (lbound, ubound)
@@ -362,14 +420,13 @@
             else:
                 if self.early_stopping is True: break
 
             if self.early_stopping is True and best_clasp.split(validation=validation, threshold=threshold) is not None:
                 break
 
         self.knn = best_clasp.knn
+        self.lbound, self.ubound = best_tc
         self.profile = np.full(shape=time_series.shape[0] - self.window_size + 1, fill_value=-np.inf, dtype=np.float64)
-
-        lbound, ubound = best_tc
-        self.profile[lbound:ubound - self.window_size + 1] = best_clasp.profile
+        self.profile[self.lbound:self.ubound - self.window_size + 1] = best_clasp.profile
 
         self.is_fitted = True
         return self
```

### Comparing `claspy-0.1.6/claspy/data_loader.py` & `claspy-0.1.7/claspy/data_loader.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/claspy/distance.py` & `claspy-0.1.7/claspy/distance.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/claspy/nearest_neighbour.py` & `claspy-0.1.7/claspy/nearest_neighbour.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import os
+
 import numpy as np
 import numpy.fft as fft
-from numba import njit
+from numba import njit, prange
+from numba.typed.typedlist import List
 
 from claspy.distance import map_distances
 from claspy.utils import check_input_time_series
 
 
 def _sliding_dot(query, time_series):
     """
@@ -117,31 +120,37 @@
         dist[min_arg] = np.inf
 
     dist[args] = vals
     return args
 
 
 @njit(fastmath=True, cache=True)
-def _knn(time_series, window_size, k_neighbours, tcs, dot_first, distance, distance_preprocessing):
+def _knn(time_series, start, end, window_size, k_neighbours, tcs, dot_first, dot_ref, distance, distance_preprocessing):
     """
     Perform k-nearest neighbors search between all pairs of subsequences of `time_series`
     of length `window_size`, based on their Euclidean distance after normalization by mean and
     standard deviation. Uses a dot product method for fast calculation.
 
     Parameters
     ----------
     time_series : ndarray of shape (n,)
         The time series to search over.
+    start : int
+        The first index to consider (inclusive).
+    end : int
+        The last index to consider (exclusive).
     window_size : int
         The length of the sliding window for comparison.
     k_neighbours : int
         The number of nearest neighbors to return for each query.
     tcs : ndarray of shape (m, 2), where each row is (start, end)
         Temporal constraints to consider.
     dot_first : ndarray of shape (n - window_size + 1,)
+        Dot product of the sliding window at start with itself.
+    dot_ref : ndarray of shape (n - window_size + 1,)
         Dot product of the first sliding window with itself.
     distance: callable
         The distance function to be computed.
     distance_preprocessing: callable
         The distance preprocessing function to be computed.
 
     Returns
@@ -150,52 +159,105 @@
         Array of distances between subsequences, sorted in increasing order.
     knns : ndarray of shape (l, m * k_neighbours)
         Array of indices of k nearest neighbors for each subsequence.
     """
     l = len(time_series) - window_size + 1
     exclusion_radius = np.int64(window_size / 2)
 
-    knns = np.zeros(shape=(l, len(tcs) * k_neighbours), dtype=np.int64)
-    dists = np.zeros(shape=(l, len(tcs) * k_neighbours), dtype=np.float64)
+    knns = np.zeros(shape=(end-start, len(tcs) * k_neighbours), dtype=np.int64)
+    dists = np.zeros(shape=(end-start, len(tcs) * k_neighbours), dtype=np.float64)
 
     dot_prev = None
     preprocessing = distance_preprocessing(time_series, window_size)
 
-    for order in range(0, l):
-        if order == 0:
+    for order in range(start, end):
+        if order == start:
             dot_rolled = dot_first
         else:
-            dot_rolled = np.roll(dot_prev, 1) + time_series[order + window_size - 1] * time_series[
-                                                                                       window_size - 1:l + window_size] - \
-                         time_series[order - 1] * np.roll(time_series[:l], 1)
-            dot_rolled[0] = dot_first[order]
+            dot_rolled = np.roll(dot_prev, 1) \
+                         + time_series[order + window_size - 1] * time_series[window_size - 1:l + window_size] \
+                         - time_series[order - 1] * np.roll(time_series[:l], 1)
+            dot_rolled[0] = dot_ref[order]
 
         dist = distance(order, dot_rolled, window_size, preprocessing)
 
         # self-join: exclusion zone
         trivialMatchRange = (
             int(max(0, order - np.round(exclusion_radius, 0))),
             int(min(order + np.round(exclusion_radius + 1, 0), l))
         )
 
         dist[trivialMatchRange[0]:trivialMatchRange[1]] = np.max(dist)
 
         for kdx, (lbound, ubound) in enumerate(tcs):
             if order < lbound or order >= ubound: continue
-
             tc_nn = lbound + _argkmin(dist[lbound:ubound - window_size + 1], k_neighbours)
 
-            knns[order, kdx * k_neighbours:(kdx + 1) * k_neighbours] = tc_nn
-            dists[order, kdx * k_neighbours:(kdx + 1) * k_neighbours] = dist[tc_nn]
+            knns[order-start, kdx * k_neighbours:(kdx + 1) * k_neighbours] = tc_nn
+            dists[order-start, kdx * k_neighbours:(kdx + 1) * k_neighbours] = dist[tc_nn]
 
         dot_prev = dot_rolled
 
     return dists, knns
 
 
+@njit(fastmath=True, cache=True, parallel=True)
+def _parallel_knn(time_series, window_size, k_neighbours, pranges, tcs, dot_firsts, distance, distance_preprocessing):
+    """
+    Perform k-nearest neighbors search between all pairs of subsequences of `time_series`
+    of length `window_size` in parallel with n_jobs threads.
+
+    Parameters
+    ----------
+    time_series : ndarray of shape (n,)
+        The time series to search over.
+    window_size : int
+        The length of the sliding window for comparison.
+    k_neighbours : int
+        The number of nearest neighbors to return for each query.
+    pranges : ndarray of shape (m, 2), where each row is (start, end)
+        Ranges in which the k-NNs are calculated per thread. Infers the number of threads.
+    tcs : ndarray of shape (m, 2), where each row is (start, end)
+        Temporal constraints to consider.
+    dot_firsts : ndarray of shape (n - window_size + 1,)
+        Dot product of the first sliding window with itself.
+    distance: callable
+        The distance function to be computed.
+    distance_preprocessing: callable
+        The distance preprocessing function to be computed.
+
+    Returns
+    -------
+    dists : ndarray of shape (l, m * k_neighbours)
+        Array of distances between subsequences, sorted in increasing order.
+    knns : ndarray of shape (l, m * k_neighbours)
+        Array of indices of k nearest neighbors for each subsequence.
+    """
+    knns = np.zeros(shape=(len(time_series) - window_size + 1, len(tcs) * k_neighbours), dtype=np.int64)
+    dists = np.zeros(shape=(len(time_series) - window_size + 1, len(tcs) * k_neighbours), dtype=np.float64)
+
+    for idx in prange(len(pranges)):
+        start, end = pranges[idx]
+
+        dists[start:end, :], knns[start:end, :] = _knn(
+            time_series.copy(),
+            start,
+            end,
+            window_size,
+            k_neighbours,
+            tcs,
+            dot_firsts[idx],
+            dot_firsts[0],
+            distance,
+            distance_preprocessing
+        )
+
+    return dists, knns
+
+
 @njit(fastmath=True, cache=True)
 def cross_val_labels(offsets, split_idx, window_size):
     """
     Generate predicted and true labels for cross-validation based on nearest neighbour distances.
 
     Parameters
     ----------
@@ -247,28 +309,31 @@
     window_size : int, optional (default=10)
         Length of subsequence window.
     k_neighbours : int, optional (default=3)
         Number of nearest neighbors to return for each time series subsequence.
     distance: str
         The name of the distance function to be computed. Available options are "znormed_euclidean_distance"
         and "euclidean_distance".
+    n_jobs : int, optional (default=1)
+        Amount of threads used in the k-nearest neighbour calculation.
 
     Methods
     -------
     fit(time_series)
         Fit the KSN model to the input time series data.
     constrain(self, lbound, ubound)
         Return a constrained KSN model for the given temporal constraint.
     """
 
-    def __init__(self, window_size=10, k_neighbours=3, distance="znormed_euclidean_distance"):
+    def __init__(self, window_size=10, k_neighbours=3, distance="znormed_euclidean_distance", n_jobs=-1):
         self.window_size = window_size
         self.k_neighbours = k_neighbours
         self.distance_name = distance
         self.distance_preprocessing, self.distance = map_distances(distance)
+        self.n_jobs = os.cpu_count() if n_jobs < 1 else n_jobs
 
     def fit(self, time_series, temporal_constraints=None):
         """
         Fits the k-subsequence neighbors model to the provided time series.
 
         Parameters
         ----------
@@ -283,24 +348,47 @@
 
         Returns
         -------
         self : KSubsequenceNeighbours
             A reference to the fitted model.
         """
         check_input_time_series(time_series)
+
+        if time_series.shape[0] < self.window_size * self.k_neighbours:
+            raise ValueError("Time series must at least have k_neighbours*window_size data points.")
+
         self.time_series = time_series
 
         if temporal_constraints is None:
             self.temporal_constraints = np.asarray([(0, time_series.shape[0])], dtype=np.int64)
         else:
             self.temporal_constraints = temporal_constraints
 
-        dot_first = _sliding_dot(time_series[:self.window_size], time_series)
-        self.distances, self.offsets = _knn(time_series, self.window_size, self.k_neighbours, self.temporal_constraints,
-                                            dot_first, self.distance, self.distance_preprocessing)
+        pranges, dot_firsts = List(), List()
+        n_jobs = self.n_jobs
+
+        while time_series.shape[0] // n_jobs < self.window_size * self.k_neighbours and n_jobs != 1:
+            n_jobs -= 1
+
+        bin_size = time_series.shape[0] // n_jobs
+
+        for idx in range(n_jobs):
+            start = idx * bin_size
+
+            end = min((idx + 1) * bin_size, len(time_series)-self.window_size+1)
+            dot_first = _sliding_dot(time_series[start:start+self.window_size], time_series)
+
+            if end > start:
+                pranges.append((start, end))
+                dot_firsts.append(dot_first)
+
+        self.distances, self.offsets = _parallel_knn(time_series, self.window_size, self.k_neighbours,
+                                                     pranges, List(self.temporal_constraints), dot_firsts,
+                                                     self.distance, self.distance_preprocessing)
+
         return self
 
     def constrain(self, lbound, ubound):
         """
         Constrain the k-nearest neighbours search to a specific range.
 
         Parameters
```

### Comparing `claspy-0.1.6/claspy/scoring.py` & `claspy-0.1.7/claspy/scoring.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/claspy/segmentation.py` & `claspy-0.1.7/claspy/segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import warnings
 from queue import PriorityQueue
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from sklearn.exceptions import NotFittedError
@@ -53,14 +54,17 @@
         null hypothesis. If the validation method is "score_threshold", this value represents
         the threshold score for accepting the change point. Default is 1e-15.
 
     excl_radius : int, default=5*window_size
         The radius (in multiples of the window size) around each point in the time series to exclude
         when searching for change points.
 
+    n_jobs : int, optional (default=max_cores)
+        Amount of threads used in the ClaSP computation.
+
     random_state : int, default=2357
         Seed for the random number generator. Default is 2357.
 
     Methods
     -------
     fit(time_series)
         Fit the BinaryClaSPSegmentation model to the input time series.
@@ -71,25 +75,26 @@
     plot()
         Visualize the segmentation for the input time series.
     """
 
     def __init__(self, n_segments="learn", n_estimators=10, window_size="suss", k_neighbours=3,
                  distance="znormed_euclidean_distance", score="roc_auc",
                  early_stopping=True, validation="significance_test", threshold=1e-15, excl_radius=5,
-                 random_state=2357):
+                 n_jobs=-1, random_state=2357):
         self.n_segments = n_segments
         self.n_estimators = n_estimators
         self.window_size = window_size
         self.k_neighbours = k_neighbours
         self.distance = distance
         self.validation = validation
         self.threshold = threshold
         self.score = score
         self.early_stopping = early_stopping
         self.excl_radius = excl_radius
+        self.n_jobs = os.cpu_count() if n_jobs < 1 else n_jobs
         self.random_state = random_state
         self.is_fitted = False
 
         check_excl_radius(k_neighbours, excl_radius)
 
     def _cp_is_valid(self, candidate, change_points):
         """
@@ -137,14 +142,15 @@
             n_estimators=self.n_estimators,
             window_size=self.window_size,
             k_neighbours=self.k_neighbours,
             distance=self.distance,
             score=self.score,
             early_stopping=self.early_stopping,
             excl_radius=self.excl_radius,
+            n_jobs=self.n_jobs,
             random_state=self.random_state
         ).fit(self.time_series[lbound:ubound], validation=self.validation, threshold=self.threshold)
 
         cp = clasp.split(validation=self.validation, threshold=self.threshold)
         if cp is None: return
         score = clasp.profile[cp]
 
@@ -217,14 +223,15 @@
                 n_estimators=self.n_estimators,
                 window_size=self.window_size,
                 k_neighbours=self.k_neighbours,
                 distance=self.distance,
                 score=self.score,
                 early_stopping=self.early_stopping,
                 excl_radius=self.excl_radius,
+                n_jobs=self.n_jobs,
                 random_state=self.random_state
             ).fit(time_series, validation=self.validation, threshold=self.threshold)
 
             cp = clasp.split(validation=self.validation, threshold=self.threshold)
 
             if cp is not None:
                 self.clasp_tree.append((prange, clasp))
```

### Comparing `claspy-0.1.6/claspy/tests/clasp_test.py` & `claspy-0.1.7/claspy/tests/clasp_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,19 +22,20 @@
     def test_param_configs(self):
         tssb = load_tssb_dataset()
         np.random.seed(2357)
         tssb = tssb.sample(3)
 
         window_sizes = (10, 50, 100)
         scores = ("f1", "roc_auc")
+        n_jobs = (1, -1)
 
         for _, (dataset, window_size, cps, time_series) in tssb.iterrows():
-            for window_size, score in product(window_sizes, scores):
+            for window_size, score, n_job in product(window_sizes, scores, n_jobs):
                 if time_series.shape[0] < 2 * 5 * window_size: continue
-                clasp = ClaSP(window_size=window_size, score=score)
+                clasp = ClaSP(window_size=window_size, score=score, n_jobs=n_job)
                 clasp.fit(time_series)
                 assert clasp.profile.shape[0] == time_series.shape[0] - clasp.window_size + 1
 
 
 class ClaSPEnsembleTest(unittest.TestCase):
 
     def test_tssb_benchmark(self):
@@ -51,18 +52,20 @@
         tssb = load_tssb_dataset()
         np.random.seed(2357)
         tssb = tssb.sample(3)
 
         window_sizes = (10, 50, 100)
         scores = ("f1", "roc_auc")
         early_stopping = (True, False)
+        n_jobs = (1, -1)
 
         for _, (dataset, window_size, cps, time_series) in tssb.iterrows():
-            for window_size, score, stop in product(window_sizes, scores, early_stopping):
+            for window_size, score, stop, n_job in product(window_sizes, scores, early_stopping, n_jobs):
                 if time_series.shape[0] < 2 * 5 * window_size: continue
                 clasp = ClaSPEnsemble(
                     window_size=window_size,
                     score=score,
-                    early_stopping=stop
+                    early_stopping=stop,
+                    n_jobs=n_job
                 )
                 clasp.fit(time_series)
                 assert clasp.profile.shape[0] == time_series.shape[0] - clasp.window_size + 1
```

### Comparing `claspy-0.1.6/claspy/tests/evaluation.py` & `claspy-0.1.7/claspy/tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/claspy/tests/nearest_neighbour_test.py` & `claspy-0.1.7/claspy/tests/nearest_neighbour_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,18 +26,19 @@
         tssb = load_tssb_dataset()
         np.random.seed(2357)
         tssb = tssb.sample(3)
 
         window_sizes = (10, 50, 100)
         k_neighbours = (1, 3, 5)
         distances = ("znormed_euclidean_distance", "euclidean_distance")
+        n_jobs = (1, -1)
 
         for _, (dataset, window_size, cps, time_series) in tssb.iterrows():
-            for window_size, k, dist in product(window_sizes, k_neighbours, distances):
-                knn = KSubsequenceNeighbours(window_size=window_size)
+            for window_size, k, dist, n_job in product(window_sizes, k_neighbours, distances, n_jobs):
+                knn = KSubsequenceNeighbours(window_size=window_size, n_jobs=n_job)
                 knn.fit(time_series)
 
                 for arr in (knn.distances, knn.offsets):
                     assert arr.shape[0] == time_series.shape[0] - knn.window_size + 1
                     assert arr.shape[1] == knn.k_neighbours
 
     def test_constraints(self):
```

### Comparing `claspy-0.1.6/claspy/tests/segmentation_test.py` & `claspy-0.1.7/claspy/tests/segmentation_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import os
 import time
 import unittest
 from itertools import product
 
 import numpy as np
 
 from claspy.data_loader import load_tssb_dataset
 from claspy.segmentation import BinaryClaSPSegmentation
 from claspy.tests.evaluation import covering
 
+ABS_PATH = os.path.dirname(os.path.abspath(__file__))
+
 # tssb data sets, with recurring segments
 REC_SEG_DS = [
     "Crop",
     "EOGHorizontalSignal",
     "EOGVerticalSignal",
     "FreezerRegularTrain",
     "Ham",
@@ -46,32 +49,38 @@
         np.random.seed(2357)
         tssb = tssb.sample(1)
 
         n_segments = (1, "learn")
         window_sizes = (10, "suss", "fft", "acf")
         validations = (None, "significance_test", "score_threshold")
         thresholds = {"significance_test": 1e-15, "score_threshold": .75}
+        n_jobs = (1, -1)
 
         for idx, (dataset, window_size, cps, time_series) in list(tssb.iterrows()):
-            for n_seg, window_size, val in product(n_segments, window_sizes, validations):
+            for n_seg, window_size, val, n_job in product(n_segments, window_sizes, validations, n_jobs):
                 BinaryClaSPSegmentation(
                     n_segments=n_seg,
                     window_size=window_size,
                     validation=val,
-                    threshold=thresholds[val] if val is not None else None
+                    threshold=thresholds[val] if val is not None else None,
+                    n_jobs=n_job
                 ).fit(time_series)
 
     def test_readme(self):
         dataset, window_size, true_cps, time_series = load_tssb_dataset(names=("CricketX",)).iloc[0, :]
 
         clasp = BinaryClaSPSegmentation()
         change_points = clasp.fit_predict(time_series)
         assert np.array_equal(change_points, np.array([712, 1281, 1933, 2581]))
-        clasp.plot(gt_cps=true_cps, heading="Segmentation of different umpire cricket signals", ts_name="ACC",
-                   file_path="../../segmentation_example.png")
+        clasp.plot(
+            gt_cps=true_cps,
+            heading="Segmentation of different umpire cricket signals",
+            ts_name="ACC",
+            file_path=f"{ABS_PATH}/../../segmentation_example.png"
+        )
 
     def test_very_small_ts(self):
         time_series = np.zeros(0)
         clasp = BinaryClaSPSegmentation()
         clasp.fit_predict(time_series)
 
         time_series = np.zeros(1)
```

### Comparing `claspy-0.1.6/claspy/utils.py` & `claspy-0.1.7/claspy/utils.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/claspy/validation.py` & `claspy-0.1.7/claspy/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     -----
     This method uses a two-sample rank-sum test with a p-value threshold to determine if a candidate change point
     is statistically significant. The test is performed using the classification labels for the candidate change point.
     If the resulting p-value is less than or equal to the specified threshold, the change point is considered significant
     and the method returns True. Otherwise, the change point is considered not significant and the method returns False.
 
     """
-    _, y_pred = cross_val_labels(clasp.knn.offsets, change_point, clasp.window_size)
+    _, y_pred = cross_val_labels(clasp.knn.offsets, change_point-clasp.lbound, clasp.window_size)
     _, p = ranksums(y_pred[:change_point], y_pred[change_point:])
     return p <= threshold
 
 
 def score_threshold(clasp, change_point, threshold=0.75):
     """
     Returns whether the ClaSP score at the given change point exceeds the specified threshold.
```

### Comparing `claspy-0.1.6/claspy/window_size.py` & `claspy-0.1.7/claspy/window_size.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/claspy.egg-info/PKG-INFO` & `claspy-0.1.7/claspy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claspy
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/ermshaua/claspy
 Author: Arik Ermshaus
 Author-email: Arik Ermshaus <ermshaua@informatik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Arik Ermshaus
         
@@ -92,14 +92,15 @@
 
 ## Examples
 
 Checkout the following Jupyter notebooks that show applications of the ClaSPy package:
 
 - <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/tssb_evaluation.ipynb">ClaSP evaluation on the "Time Series Segmentation Benchmark" (TSSB)</a>
 - <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/clasp_configuration.ipynb">Hyper-parameter Tuning and Configuration of ClaSP</a>
+- <a href="https://github.com/ermshaua/claspy/blob/main/claspy/notebooks/window_size_selection.ipynb">Window Size Selection for Unsupervised Time Series Analytics</a>
 
 ## Citation
 
 The ClaSPy package is actively maintained, updated and intended for application. If you use ClaSP in your scientific publication, we would appreciate the following <a href="https://doi.org/10.1007/s10618-023-00923-x" target="_blank">citation</a>:
 
 ```
 @article{clasp2023,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: claspy Version: 0.1.6 Home-page: https://
+Metadata-Version: 2.1 Name: claspy Version: 0.1.7 Home-page: https://
 github.com/ermshaua/claspy Author: Arik Ermshaus Author-email: Arik Ermshaus
 informatik.hu-berlin.de> License: BSD 3-Clause License Copyright (c) 2023, Arik
 Ermshaus Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -61,17 +61,18 @@
 accurately detects the number and location of changes in the motion sequence
 (compare green vs red lines) that infer its segmentation (the different-
 coloured subsequences). It is carefully designed to do this fully autonomously.
 However, if you have domain-specific knowledge, you can utilize it to guide and
 improve the segmentation. See its parameters for more information. ## Examples
 Checkout the following Jupyter notebooks that show applications of the ClaSPy
 package: - ClaSP_evaluation_on_the_"Time_Series_Segmentation_Benchmark"_(TSSB)
-- Hyper-parameter_Tuning_and_Configuration_of_ClaSP ## Citation The ClaSPy
-package is actively maintained, updated and intended for application. If you
-use ClaSP in your scientific publication, we would appreciate the following
-citation: ``` @article{clasp2023, title={ClaSP: parameter-free time series
-segmentation}, author={Arik Ermshaus and Patrick Sch{\"a}fer and Ulf Leser},
-journal={Data Mining and Knowledge Discovery}, year={2023}, } ``` ## Todos Here
-are some of the things we would like to add to ClaSPy in the future: - Future
-research related to ClaSP - Example and application Jupyter notebooks - More
+- Hyper-parameter_Tuning_and_Configuration_of_ClaSP - Window_Size_Selection_for
+Unsupervised_Time_Series_Analytics ## Citation The ClaSPy package is actively
+maintained, updated and intended for application. If you use ClaSP in your
+scientific publication, we would appreciate the following citation: ```
+@article{clasp2023, title={ClaSP: parameter-free time series segmentation},
+author={Arik Ermshaus and Patrick Sch{\"a}fer and Ulf Leser}, journal={Data
+Mining and Knowledge Discovery}, year={2023}, } ``` ## Todos Here are some of
+the things we would like to add to ClaSPy in the future: - Future research
+related to ClaSP - Example and application Jupyter notebooks - More
 documentation and tests If you want to contribute, report bugs, or need help
 applying ClaSP for your application, feel free to reach out.
```

### Comparing `claspy-0.1.6/claspy.egg-info/SOURCES.txt` & `claspy-0.1.7/claspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claspy-0.1.6/pyproject.toml` & `claspy-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "claspy"
 
-version = "0.1.6"
+version = "0.1.7"
 
 description = ""
 readme = "README.md"
 authors = [
     {name = "Arik Ermshaus", email = "ermshaua@informatik.hu-berlin.de"}
 ]
 keywords = [
```

### Comparing `claspy-0.1.6/setup.py` & `claspy-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 
 __author__ = ["ermshaua"]
 
+from pathlib import Path
+
 import toml
 from setuptools import find_packages, setup
-from pathlib import Path
 
 pyproject = toml.load("pyproject.toml")
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
     
 """Set up package."""
```

