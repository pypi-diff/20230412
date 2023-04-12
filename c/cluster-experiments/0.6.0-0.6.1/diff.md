# Comparing `tmp/cluster_experiments-0.6.0.tar.gz` & `tmp/cluster_experiments-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.6.0.tar", last modified: Thu Mar  9 14:22:40 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.6.1.tar", last modified: Wed Apr 12 09:19:36 2023, max compression
```

## Comparing `cluster_experiments-0.6.0.tar` & `cluster_experiments-0.6.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:40.087331 cluster_experiments-0.6.0/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.0/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.0/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-03-09 14:22:40.086502 cluster_experiments-0.6.0/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-03-09 14:09:53.000000 cluster_experiments-0.6.0/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:39.991264 cluster_experiments-0.6.0/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-03-09 14:09:53.000000 cluster_experiments-0.6.0/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7301 2022-12-19 15:58:12.000000 cluster_experiments-0.6.0/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17228 2023-03-01 11:45:41.000000 cluster_experiments-0.6.0/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-03-01 11:31:23.000000 cluster_experiments-0.6.0/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    16733 2023-03-09 13:53:44.000000 cluster_experiments-0.6.0/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.0/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17759 2023-03-09 14:22:29.000000 cluster_experiments-0.6.0/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.0/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5915 2023-03-09 14:22:29.000000 cluster_experiments-0.6.0/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:39.999120 cluster_experiments-0.6.0/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-03-09 14:22:39.000000 cluster_experiments-0.6.0/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1409 2023-03-09 14:22:39.000000 cluster_experiments-0.6.0/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-03-09 14:22:39.000000 cluster_experiments-0.6.0/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)      945 2023-03-09 14:22:39.000000 cluster_experiments-0.6.0/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-03-09 14:22:39.000000 cluster_experiments-0.6.0/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-03-09 14:22:40.087484 cluster_experiments-0.6.0/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1077 2023-03-09 14:22:29.000000 cluster_experiments-0.6.0/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:40.009934 cluster_experiments-0.6.0/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.0/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:40.030144 cluster_experiments-0.6.0/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.0/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.0/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2022-12-23 16:22:32.000000 cluster_experiments-0.6.0/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:40.047143 cluster_experiments-0.6.0/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.0/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2022-12-30 09:27:02.000000 cluster_experiments-0.6.0/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2141 2022-12-30 09:27:02.000000 cluster_experiments-0.6.0/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.0/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:40.053125 cluster_experiments-0.6.0/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.0/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2022-12-23 16:22:32.000000 cluster_experiments-0.6.0/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:40.072306 cluster_experiments-0.6.0/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.0/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.0/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.0/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.0/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5291 2023-03-01 11:45:41.000000 cluster_experiments-0.6.0/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.0/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-02-10 16:31:12.000000 cluster_experiments-0.6.0/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-03-09 14:22:40.084717 cluster_experiments-0.6.0/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.0/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5743 2023-03-09 14:09:53.000000 cluster_experiments-0.6.0/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.0/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.0/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.0/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-03-09 14:22:29.000000 cluster_experiments-0.6.0/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-03-09 14:09:53.000000 cluster_experiments-0.6.0/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.0/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.0/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1324 2022-10-21 09:42:28.000000 cluster_experiments-0.6.0/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.739387 cluster_experiments-0.6.1/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.1/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.1/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-12 09:19:36.738271 cluster_experiments-0.6.1/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.647365 cluster_experiments-0.6.1/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7301 2022-12-19 15:58:12.000000 cluster_experiments-0.6.1/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17228 2023-03-01 11:45:41.000000 cluster_experiments-0.6.1/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-03-01 11:31:23.000000 cluster_experiments-0.6.1/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17759 2023-04-12 08:53:42.000000 cluster_experiments-0.6.1/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.1/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.655499 cluster_experiments-0.6.1/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1071 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-04-12 09:19:36.739717 cluster_experiments-0.6.1/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1133 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.668180 cluster_experiments-0.6.1/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.1/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.674312 cluster_experiments-0.6.1/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.1/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.680215 cluster_experiments-0.6.1/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2141 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.1/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.683447 cluster_experiments-0.6.1/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.700360 cluster_experiments-0.6.1/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5239 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.1/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.736675 cluster_experiments-0.6.1/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5743 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.1/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.1/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.1/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.1/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1324 2022-10-21 09:42:28.000000 cluster_experiments-0.6.1/tests/utils.py
```

### Comparing `cluster_experiments-0.6.0/LICENSE` & `cluster_experiments-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/README.md` & `cluster_experiments-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/cluster_experiments/__init__.py` & `cluster_experiments-0.6.1/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/cluster_experiments/cupac.py` & `cluster_experiments-0.6.1/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.6.1/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/cluster_experiments/perturbator.py` & `cluster_experiments-0.6.1/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/cluster_experiments/power_analysis.py` & `cluster_experiments-0.6.1/cluster_experiments/power_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Dict, Generator, Iterable, List, Optional
+from typing import Dict, Generator, Iterable, List, Optional, Tuple
 
 import pandas as pd
 from sklearn.base import BaseEstimator
 from tqdm import tqdm
 
 from cluster_experiments.cupac import CupacHandler
 from cluster_experiments.experiment_analysis import ExperimentAnalysis
@@ -124,33 +124,18 @@
         pre_experiment_df: Optional[pd.DataFrame] = None,
         verbose: bool = False,
         average_effect: Optional[float] = None,
         n_simulations: int = 100,
     ) -> Generator[pd.DataFrame, None, None]:
         """Yields splitted + perturbated dataframe for each iteration of the simulation."""
         df = df.copy()
-
         df = self.cupac_handler.add_covariates(df, pre_experiment_df)
 
         for _ in tqdm(range(n_simulations), disable=not verbose):
-            treatment_df = self.splitter.assign_treatment_df(df)
-            self.log_nulls(treatment_df)
-            # The second query allows as to do power analysis for multivariate testing
-            # It assumes that we give, to each treatment value, the same number of samples
-            # If this is not the case, several PowerAnalysis should be run with different weights
-            treatment_df = treatment_df.query(
-                f"{self.treatment_col}.notnull()", engine="python"
-            ).query(
-                f"{self.treatment_col}.isin(['{self.treatment}', '{self.control}'])",
-                engine="python",
-            )
-            perturbed_df = self.perturbator.perturbate(
-                treatment_df, average_effect=average_effect
-            )
-            yield perturbed_df
+            yield self._split_and_perturbate(df, average_effect)
 
     def simulate_pvalue(
         self,
         df: pd.DataFrame,
         pre_experiment_df: Optional[pd.DataFrame] = None,
         verbose: bool = False,
         average_effect: Optional[float] = None,
@@ -211,70 +196,158 @@
         self,
         df: pd.DataFrame,
         pre_experiment_df: Optional[pd.DataFrame] = None,
         verbose: bool = False,
         average_effect: Optional[float] = None,
         n_simulations: Optional[int] = None,
         alpha: Optional[float] = None,
+        n_jobs: int = 1,
     ) -> float:
         """
         Run power analysis by simulation
         Args:
             df: Dataframe with outcome and treatment variables.
             pre_experiment_df: Dataframe with pre-experiment data.
             verbose: Whether to show progress bar.
             average_effect: Average effect of treatment. If None, it will use the perturbator average effect.
             n_simulations: Number of simulations to run.
             alpha: Significance level.
+            n_jobs: Number of jobs to run in parallel. If 1, it will run in serial.
         """
         n_simulations = self.n_simulations if n_simulations is None else n_simulations
         alpha = self.alpha if alpha is None else alpha
 
+        df = df.copy()
+        df = self.cupac_handler.add_covariates(df, pre_experiment_df)
+
+        if n_jobs == 1:
+            return self._non_parallel_loop(
+                df, average_effect, n_simulations, alpha, verbose
+            )
+        elif n_jobs > 1 or n_jobs == -1:
+            return self._parallel_loop(
+                df, average_effect, n_simulations, alpha, verbose, n_jobs
+            )
+        else:
+            raise ValueError("n_jobs must be greater than 0, or -1.")
+
+    def _split_and_perturbate(
+        self, df: pd.DataFrame, average_effect: Optional[float]
+    ) -> pd.DataFrame:
+        """
+        Split and perturbate dataframe.
+        Args:
+            df: Dataframe with outcome variable
+            average_effect: Average effect of treatment. If None, it will use the perturbator average effect.
+        """
+        treatment_df = self.splitter.assign_treatment_df(df)
+        self.log_nulls(treatment_df)
+        treatment_df = treatment_df.query(
+            f"{self.treatment_col}.notnull()", engine="python"
+        ).query(
+            f"{self.treatment_col}.isin(['{self.treatment}', '{self.control}'])",
+            engine="python",
+        )
+        perturbed_df = self.perturbator.perturbate(
+            treatment_df, average_effect=average_effect
+        )
+        return perturbed_df
+
+    def _run_simulation(self, args: Tuple[pd.DataFrame, Optional[float]]) -> float:
+        df, average_effect = args
+        perturbed_df = self._split_and_perturbate(df, average_effect)
+        return self.analysis.get_pvalue(perturbed_df)
+
+    def _non_parallel_loop(
+        self,
+        df: pd.DataFrame,
+        average_effect: Optional[float],
+        n_simulations: int,
+        alpha: float,
+        verbose: bool,
+    ) -> float:
+        """
+        Run power analysis by simulation in serial
+        Args:
+            df: Dataframe with outcome and treatment variables.
+            average_effect: Average effect of treatment. If None, it will use the perturbator average effect.
+            n_simulations: Number of simulations to run.
+            alpha: Significance level.
+        """
         n_detected_mde = 0
-        for p_value in self.simulate_pvalue(
-            df=df,
-            pre_experiment_df=pre_experiment_df,
-            verbose=verbose,
-            average_effect=average_effect,
-            n_simulations=n_simulations,
-        ):
+        for _ in tqdm(range(n_simulations), disable=not verbose):
+            p_value = self._run_simulation((df, average_effect))
             n_detected_mde += p_value < alpha
 
         return n_detected_mde / n_simulations
 
+    def _parallel_loop(
+        self,
+        df: pd.DataFrame,
+        average_effect: Optional[float],
+        n_simulations: int,
+        alpha: float,
+        verbose: bool,
+        n_jobs: int,
+    ) -> float:
+        """
+        Run power analysis by simulation in parallel
+        Args:
+            df: Dataframe with outcome and treatment variables.
+            average_effect: Average effect of treatment. If None, it will use the perturbator average effect.
+            n_simulations: Number of simulations to run.
+            alpha: Significance level.
+            n_jobs: Number of jobs to run in parallel.
+        """
+        from multiprocessing import Pool, cpu_count
+
+        n_jobs = n_jobs if n_jobs != -1 else cpu_count()
+
+        n_detected_mde = 0
+        with Pool(processes=n_jobs) as pool:
+            args = [(df, average_effect) for _ in range(n_simulations)]
+            results = pool.imap_unordered(self._run_simulation, args)
+            for p_value in tqdm(results, total=n_simulations, disable=not verbose):
+                n_detected_mde += p_value < alpha
+
+        return n_detected_mde / n_simulations
+
     def power_line(
         self,
         df: pd.DataFrame,
         pre_experiment_df: Optional[pd.DataFrame] = None,
         verbose: bool = False,
         average_effects: Iterable[float] = (),
         n_simulations: Optional[int] = None,
         alpha: Optional[float] = None,
+        n_jobs: int = 1,
     ) -> Dict[float, float]:
         """Runs power analysis with multiple average effects
 
         Args:
             df: Dataframe with outcome and treatment variables.
             pre_experiment_df: Dataframe with pre-experiment data.
             verbose: Whether to show progress bar.
             average_effects: Average effects to test.
             n_simulations: Number of simulations to run.
             alpha: Significance level.
+            n_jobs: Number of jobs to run in parallel.
 
         Returns:
             Dictionary with average effects as keys and power as values.
         """
         return {
             effect: self.power_analysis(
                 df=df,
                 pre_experiment_df=pre_experiment_df,
                 verbose=verbose,
                 average_effect=effect,
                 n_simulations=n_simulations,
                 alpha=alpha,
+                n_jobs=n_jobs,
             )
             for effect in tqdm(
                 list(average_effects), disable=not verbose, desc="Effects loop"
             )
         }
 
     def log_nulls(self, df: pd.DataFrame) -> None:
```

### Comparing `cluster_experiments-0.6.0/cluster_experiments/power_config.py` & `cluster_experiments-0.6.1/cluster_experiments/power_config.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/cluster_experiments/random_splitter.py` & `cluster_experiments-0.6.1/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/cluster_experiments/washover.py` & `cluster_experiments-0.6.1/cluster_experiments/washover.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,18 @@
         cluster_cols: List[str],
         original_time_col: Optional[str] = None,
     ) -> pd.DataFrame:
         """No washover - returns the same dataframe as input.
 
         Args:
             df (pd.DataFrame): Input dataframe.
-            time_col (str): Name of the time column.
+            truncated_time_col (str): Name of the truncated time column.
             treatment_col (str): Name of the treatment column.
             cluster_cols (List[str]): List of clusters of experiment.
+            original_time_col (Optional[str], optional): Name of the original time column.
 
         Returns:
             pd.DataFrame: Same dataframe as input.
 
         Usage:
         ```python
         from cluster_experiments import SwitchbackSplitter
@@ -96,17 +97,18 @@
         cluster_cols: List[str],
         original_time_col: Optional[str] = None,
     ) -> pd.DataFrame:
         """No washover - returns the same dataframe as input.
 
         Args:
             df (pd.DataFrame): Input dataframe.
-            time_col (str): Name of the time column.
+            truncated_time_col (str): Name of the truncated time column.
             treatment_col (str): Name of the treatment column.
             cluster_cols (List[str]): List of clusters of experiment.
+            original_time_col (Optional[str], optional): Name of the original time column.
 
         Returns:
             pd.DataFrame: Same dataframe as input.
 
         Usage:
         ```python
         from cluster_experiments import SwitchbackSplitter
```

### Comparing `cluster_experiments-0.6.0/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.6.1/cluster_experiments.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 tests/cupac/test_cupac_handler.py
 tests/perturbator/__init__.py
 tests/perturbator/test_perturbator.py
 tests/power_analysis/__init__.py
 tests/power_analysis/conftest.py
 tests/power_analysis/test_cupac_power.py
 tests/power_analysis/test_multivariate.py
+tests/power_analysis/test_parallel.py
 tests/power_analysis/test_power_analysis.py
 tests/power_analysis/test_power_raises.py
 tests/power_analysis/test_switchback_power.py
 tests/splitter/__init__.py
 tests/splitter/conftest.py
 tests/splitter/test_splitter.py
 tests/splitter/test_switchback_splitter.py
```

### Comparing `cluster_experiments-0.6.0/setup.py` & `cluster_experiments-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     "black==22.12.0",
     "flake8>=3.8.3",
     "mktestdocs>=0.2.0",
     "pytest-cov>=2.10.1",
     "pytest-sugar>=0.9.4",
     "pytest-slow-last>=0.1.3",
     "coverage",
+    "pytest-reportlog",
+    "pytest-duration-insights",
 ]
 test_packages = only_test_packages + base_packages
 
 util_packages = [
     "pre-commit>=2.6.0",
     "ipykernel>=6.15.1",
     "twine",
@@ -36,15 +38,15 @@
     "mkdocs-jupyter==0.22.0",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.6.0",
+    version="0.6.1",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.6.0/tests/analysis/test_analysis.py` & `cluster_experiments-0.6.1/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/cupac/test_aggregator.py` & `cluster_experiments-0.6.1/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.6.1/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/examples.py` & `cluster_experiments-0.6.1/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.6.1/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/power_analysis/conftest.py` & `cluster_experiments-0.6.1/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.6.1/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.6.1/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.6.1/tests/power_analysis/test_power_analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,18 +47,17 @@
     power = pw.power_analysis(df, average_effect=0.0)
     assert power >= 0
     assert power <= 1
 
 
 def test_power_analysis_dict(df):
     config = dict(
-        cluster_cols=["cluster", "date"],
-        analysis="gee",
+        analysis="ols_non_clustered",
         perturbator="uniform",
-        splitter="clustered",
+        splitter="non_clustered",
         n_simulations=4,
     )
     pw = PowerAnalysis.from_dict(config)
     power = pw.power_analysis(df, average_effect=0.0)
     assert power >= 0
     assert power <= 1
 
@@ -73,15 +72,15 @@
             "cluster": "cluster_0",
             "target": "target_0",
             "date": "date_0",
         }
     )
     config = dict(
         cluster_cols=["cluster_0", "date_0"],
-        analysis="gee",
+        analysis="ols_clustered",
         perturbator="uniform",
         splitter="clustered",
         n_simulations=4,
         treatment_col="treatment_0",
         target_col="target_0",
     )
     pw = PowerAnalysis.from_dict(config)
@@ -130,33 +129,32 @@
     power_verbose = pw.power_analysis(df, verbose=True, average_effect=0.0)
     assert power_verbose >= 0
     assert power_verbose <= 1
 
 
 def test_power_alpha(df):
     config = PowerConfig(
-        cluster_cols=["cluster", "date"],
-        analysis="gee",
+        analysis="ols_non_clustered",
         perturbator="uniform",
-        splitter="clustered",
+        splitter="non_clustered",
         n_simulations=10,
         average_effect=0.0,
         alpha=0.05,
     )
     pw = PowerAnalysis.from_config(config)
     power_50 = pw.power_analysis(df, alpha=0.5, verbose=True)
     power_01 = pw.power_analysis(df, alpha=0.01)
 
     assert power_50 > power_01
 
 
 def test_length_simulation(df):
     config = PowerConfig(
         cluster_cols=["cluster", "date"],
-        analysis="gee",
+        analysis="ols_clustered",
         perturbator="uniform",
         splitter="clustered",
         n_simulations=10,
         average_effect=0.0,
         alpha=0.05,
     )
     pw = PowerAnalysis.from_config(config)
@@ -179,18 +177,17 @@
     pw = PowerAnalysis.from_config(config)
     for point_estimate in pw.simulate_point_estimate(df, n_simulations=5):
         assert point_estimate > 0.0
 
 
 def test_power_line(df):
     config = PowerConfig(
-        cluster_cols=["cluster", "date"],
-        analysis="gee",
+        analysis="ols_non_clustered",
         perturbator="uniform",
-        splitter="clustered",
+        splitter="non_clustered",
         n_simulations=10,
         average_effect=0.0,
         alpha=0.05,
     )
     pw = PowerAnalysis.from_config(config)
 
     power_line = pw.power_line(df, average_effects=[0.0, 1.0], n_simulations=10)
```

### Comparing `cluster_experiments-0.6.0/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.6.1/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.6.1/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/splitter/conftest.py` & `cluster_experiments-0.6.1/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/splitter/test_splitter.py` & `cluster_experiments-0.6.1/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.6.1/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/splitter/test_time_col.py` & `cluster_experiments-0.6.1/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/splitter/test_washover.py` & `cluster_experiments-0.6.1/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/test_docs.py` & `cluster_experiments-0.6.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/test_non_clustered.py` & `cluster_experiments-0.6.1/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.0/tests/utils.py` & `cluster_experiments-0.6.1/tests/utils.py`

 * *Files identical despite different names*

