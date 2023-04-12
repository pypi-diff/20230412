# Comparing `tmp/graphomaly-0.2.6.tar.gz` & `tmp/graphomaly-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphomaly-0.2.6.tar", last modified: Mon Oct 17 13:14:43 2022, max compression
+gzip compressed data, was "graphomaly-0.2.7.tar", last modified: Wed Apr 12 15:04:12 2023, max compression
```

## Comparing `graphomaly-0.2.6.tar` & `graphomaly-0.2.7.tar`

### file list

```diff
@@ -1,41 +1,52 @@
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-10-17 13:14:43.375513 graphomaly-0.2.6/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      718 2022-02-25 22:45:24.000000 graphomaly-0.2.6/LICENSE
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2022-10-17 13:14:43.375513 graphomaly-0.2.6/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1955 2022-04-22 17:59:40.000000 graphomaly-0.2.6/README.md
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-10-17 13:14:43.372180 graphomaly-0.2.6/graphomaly/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       43 2022-03-11 07:59:51.000000 graphomaly-0.2.6/graphomaly/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    19445 2022-10-17 13:13:51.000000 graphomaly-0.2.6/graphomaly/estimator.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    21471 2022-10-17 13:13:51.000000 graphomaly-0.2.6/graphomaly/grid_search.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-10-17 13:14:43.372180 graphomaly-0.2.6/graphomaly/models/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       46 2022-03-11 07:59:51.000000 graphomaly-0.2.6/graphomaly/models/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    16596 2022-10-17 13:13:51.000000 graphomaly-0.2.6/graphomaly/models/autoencoder.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2684 2022-05-12 09:04:41.000000 graphomaly-0.2.6/graphomaly/models/base_model.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6718 2022-03-25 16:11:16.000000 graphomaly-0.2.6/graphomaly/models/dictlearn.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7111 2022-05-12 09:04:41.000000 graphomaly-0.2.6/graphomaly/models/models.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      731 2022-03-11 07:59:51.000000 graphomaly-0.2.6/graphomaly/models/sklearn.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    14903 2022-03-21 11:50:08.000000 graphomaly-0.2.6/graphomaly/models/vae.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-10-17 13:14:43.375513 graphomaly-0.2.6/graphomaly/preprocessing/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-03-11 07:59:51.000000 graphomaly-0.2.6/graphomaly/preprocessing/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8556 2022-04-22 17:59:40.000000 graphomaly-0.2.6/graphomaly/preprocessing/egonet.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-10-17 13:14:43.375513 graphomaly-0.2.6/graphomaly/preprocessing/fe_base/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-04-29 11:18:06.000000 graphomaly-0.2.6/graphomaly/preprocessing/fe_base/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4642 2022-05-02 09:08:18.000000 graphomaly-0.2.6/graphomaly/preprocessing/fe_base/historical_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    18634 2022-04-29 11:18:06.000000 graphomaly-0.2.6/graphomaly/preprocessing/fe_base/statistical_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12728 2022-04-29 11:18:06.000000 graphomaly-0.2.6/graphomaly/preprocessing/fe_base/time_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5112 2022-05-02 09:08:18.000000 graphomaly-0.2.6/graphomaly/preprocessing/fe_difference_transformer.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8427 2022-04-29 11:18:06.000000 graphomaly-0.2.6/graphomaly/preprocessing/fe_statistical_transformer.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9538 2022-04-29 11:18:06.000000 graphomaly-0.2.6/graphomaly/preprocessing/fe_time_transformers.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    33228 2022-09-28 08:52:43.000000 graphomaly-0.2.6/graphomaly/preprocessing/graph_to_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9095 2022-04-22 17:59:40.000000 graphomaly-0.2.6/graphomaly/preprocessing/graph_to_spectrum_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7204 2022-04-22 17:59:40.000000 graphomaly-0.2.6/graphomaly/preprocessing/rwalk.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6850 2022-04-22 17:59:40.000000 graphomaly-0.2.6/graphomaly/preprocessing/spectrum.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6129 2022-09-28 12:40:51.000000 graphomaly-0.2.6/graphomaly/preprocessing/transactions_to_graph.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8499 2022-09-27 13:57:22.000000 graphomaly-0.2.6/graphomaly/voting.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-10-17 13:14:43.375513 graphomaly-0.2.6/graphomaly.egg-info/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2022-10-17 13:14:43.000000 graphomaly-0.2.6/graphomaly.egg-info/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1223 2022-10-17 13:14:43.000000 graphomaly-0.2.6/graphomaly.egg-info/SOURCES.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2022-10-17 13:14:43.000000 graphomaly-0.2.6/graphomaly.egg-info/dependency_links.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      144 2022-10-17 13:14:43.000000 graphomaly-0.2.6/graphomaly.egg-info/requires.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       11 2022-10-17 13:14:43.000000 graphomaly-0.2.6/graphomaly.egg-info/top_level.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       99 2022-02-25 22:45:24.000000 graphomaly-0.2.6/pyproject.toml
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1155 2022-10-17 13:14:43.375513 graphomaly-0.2.6/setup.cfg
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.261259 graphomaly-0.2.7/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      718 2021-10-11 19:50:38.000000 graphomaly-0.2.7/LICENSE
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-12 15:04:12.261259 graphomaly-0.2.7/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1955 2022-05-03 07:20:54.000000 graphomaly-0.2.7/README.md
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.254592 graphomaly-0.2.7/graphomaly/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       43 2022-03-01 20:47:00.000000 graphomaly-0.2.7/graphomaly/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    31674 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/estimator.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    25465 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/grid_search.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.254592 graphomaly-0.2.7/graphomaly/models/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       46 2022-02-27 21:19:37.000000 graphomaly-0.2.7/graphomaly/models/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    24065 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/models/autoencoder.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2684 2022-02-27 21:07:58.000000 graphomaly-0.2.7/graphomaly/models/base_model.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7950 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/models/dictlearn.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7111 2022-05-03 07:25:03.000000 graphomaly-0.2.7/graphomaly/models/models.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      731 2022-02-27 21:06:44.000000 graphomaly-0.2.7/graphomaly/models/sklearn.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    26574 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/models/vae.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4813 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/normalizations.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.257926 graphomaly-0.2.7/graphomaly/preprocessing/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-02-27 22:16:17.000000 graphomaly-0.2.7/graphomaly/preprocessing/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8556 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/egonet.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.257926 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4642 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/historical_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    18634 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/statistical_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12728 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/time_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5112 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_difference_transformer.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8427 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_statistical_transformer.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9538 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_time_transformers.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    33228 2022-09-27 19:49:32.000000 graphomaly-0.2.7/graphomaly/preprocessing/graph_to_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9095 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/graph_to_spectrum_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7204 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/rwalk.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6850 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/spectrum.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6129 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/preprocessing/transactions_to_graph.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    36401 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/voting.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.257926 graphomaly-0.2.7/graphomaly.egg-info/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1494 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/SOURCES.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/dependency_links.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      168 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/requires.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       11 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/top_level.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       99 2021-10-11 19:50:38.000000 graphomaly-0.2.7/pyproject.toml
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1180 2023-04-12 15:04:12.261259 graphomaly-0.2.7/setup.cfg
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.261259 graphomaly-0.2.7/tests/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1619 2022-03-31 19:27:11.000000 graphomaly-0.2.7/tests/test_dl.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1501 2022-05-03 07:20:54.000000 graphomaly-0.2.7/tests/test_fe_time.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1991 2022-04-02 17:39:48.000000 graphomaly-0.2.7/tests/test_graphomaly_ctor.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1035 2022-04-02 17:24:08.000000 graphomaly-0.2.7/tests/test_synthetic.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1023 2022-04-02 17:10:58.000000 graphomaly-0.2.7/tests/test_synthetic_gridsearch.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3264 2022-05-03 07:20:54.000000 graphomaly-0.2.7/tests/test_synthetic_preprocessing.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1084 2022-04-02 15:48:52.000000 graphomaly-0.2.7/tests/test_synthetic_voting.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1722 2022-03-15 18:50:57.000000 graphomaly-0.2.7/tests/test_tf_save.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1535 2022-03-01 23:27:25.000000 graphomaly-0.2.7/tests/test_voting.py
```

### Comparing `graphomaly-0.2.6/LICENSE` & `graphomaly-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/PKG-INFO` & `graphomaly-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphomaly
-Version: 0.2.6
+Version: 0.2.7
 Summary: software package for anomaly detection in graphs modeling financial transactions
 Home-page: https://gitlab.com/unibuc/graphomaly/graphomaly
 Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
 Author-email: graphomaly@fmi.unibuc.ro
 Project-URL: Bug Tracker, https://gitlab.com/unibuc/graphomaly/graphomaly/-/issues
 Keywords: anomaly detection,graphs,financial transactions,machine learning,security
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphomaly-0.2.6/README.md` & `graphomaly-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/grid_search.py` & `graphomaly-0.2.7/graphomaly/grid_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
 import numpy as np
 from sklearn.base import clone
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import ParameterGrid
 from tensorflow.keras.models import load_model
 
+from wrapt_timeout_decorator import timeout
+
 from .models import ModelsLoader
 
 class GridSearch:
     """Grid Search routine.
 
     Grid search expects an estimator and a set of multiple parameters values
     for each possible parameter of the estimator on which to `fit` the provided
@@ -207,26 +209,29 @@
         n_cpus=1,
         clf_type="sklearn",
         get_results=None,
         compare_metric=None,
         refit=False,
         clf_algorithm = '',
         clf_model_kwargs={},
-        params_generators = []
+        params_generators = [],
+        timeout_fit=None
 
     ):
         self.base_clf = clf
         self.clf_algorithm = clf_algorithm
         self.clf_model_kwargs = clf_model_kwargs
         self.datadir = datadir
         self.n_cpus = n_cpus
         self.clf_type = clf_type
+        self.timeout_fit = timeout_fit
 
         self.params = params        # Dictionary with params settings
         self.params_grid = []       # Will hold the actual parameter configurations returned by ParameterGrid
+        self.params_grid_noremove = []  # All the params for the current session, including the cached ones from the datadir
         self.refit = refit
 
         self.clf_name = clf.__class__.__name__
 
         self.get_results = get_results
         if self.get_results is None:
             self.get_results = _fpfn
@@ -263,14 +268,17 @@
             self.best_estimator_ = clf
 
     def _test_clf(self, params):
         X = params.pop("samples")
         y = params.pop("targets")
         start = time.time()
 
+        experiment_file_params = self._experiment_file_params(params)
+        logger.info(f"Fitting {experiment_file_params}")
+
         if self.clf_type == "tensorflow":  # tf has no clone
             clf = self.base_clf
         else:
             clf = clone(self.base_clf)
         clf = clf.set_params(**params)
         y_pred = clf.fit_predict(X)
 
@@ -301,93 +309,14 @@
                 open(
                     fname,
                     "wb",
                 ),
             )
         return metrics
 
-    @staticmethod
-    def _test_clf_static(params):
-        """Static version of _test_clf(). Instantiates tensorflow models internally.
-
-        Args:
-            params (dict): Dictionary with all necessary parameters. Includes parameters for instantiating a tensorflow model.
-
-        Returns:
-            dict: Metrics dict
-        """
-        X = params.pop("samples")
-        y = params.pop("targets")
-        clf_algorithm = params.pop("clf_algorithm")
-        clf_model_kwargs = params.pop("clf_model_kwargs")
-        clf_type = params.pop("clf_type")
-        datadir = params.pop("datadir")
-        clf_name = params.pop("clf_name")
-        experiment_file_params = params.pop("experiment_file_params")
-        start = time.time()
-
-        logger.info(f"Running {experiment_file_params}")
-
-        # Assume self.clf_type == "tensorflow"
-        clf = ModelsLoader.get(clf_algorithm, **clf_model_kwargs)
-
-        clf = clf.set_params(**params)
-        y_pred = clf.fit_predict(X)
-
-        metrics = _fpfn(None, None, y_pred, y)
-        end = time.time()
-        duration = end - start
-        metrics["duration"] = duration
-
-        logger.debug(metrics)
-
-        fname = f"{datadir}/{clf_name}" + experiment_file_params
-
-        if clf_type == "tensorflow":  # tf is not pickle compatible
-
-            # Save model
-            clf.metrics_ = metrics
-            clf.save(fname)
-
-            # Manually pickle attributes in a separate file
-            attrs_to_pickle = clf.get_config()
-            attrs_to_pickle['optimizer'] = params['optimizer']
-            attrs_to_pickle['loss'] = params['loss']
-            pickle.dump(attrs_to_pickle, open(os.path.join(fname, 'autoencoder_attrs'),'wb'))
-
-            # Pickle metrics
-            pickle.dump(
-                # [ba, tpr, tnr, duration, tn, fp, fn, tp],
-                metrics,
-                open(
-                    fname + "/metrics",
-                    "wb",
-                ),
-            )
-
-            # Save metrics also as a text file
-            with open(os.path.join(fname, 'metrics.txt'), "w") as external_file:
-                pprint.pprint(metrics, stream=external_file)
-
-            # Save config to a text file
-            with open(os.path.join(fname, 'config.txt'), "w") as external_file:
-                pprint.pprint(clf.get_config(), stream=external_file)
-
-        else:
-            metrics["clf"] = clf
-            pickle.dump(
-                # [clf, ba, tpr, tnr, duration, tn, fp, fn, tp],
-                metrics,
-                open(
-                    fname,
-                    "wb",
-                ),
-            )
-        return metrics
-
     def _grid_make_iterable(self):
         for k, v in self.params.items():
             if not isinstance(self.params[k], Iterable):
                 self.params[k] = [v]
             if isinstance(self.params[k], str):
                 self.params[k] = [v]
 
@@ -408,30 +337,37 @@
                 d.update(t)
             return d
 
         # Combine `self.params` with the parameters defined by the additional generators
         # Generators can overwrite values defined in self.params
         self.params_grid = [_merge_dict_tuple(tup) for tup in itertools.product(self.params_grid, *self.params_generators)]
 
+        # Make a copy of the full list
+        # Cached estimators found in the save folder will be removed from params_grid, but are kept in params_grid_all
+        self.params_grid_noremove = self.params_grid
+
     def _experiment_get_path(self, prefix, p):
         return prefix + self._experiment_file_params(p)
 
     def _experiment_exists(self, prefix, p):
         experiment = self._experiment_get_path(prefix, p)
         return os.path.exists(experiment)
 
     def _experiment_remove_if_exists(self, prefix, p):
         experiment = self._experiment_get_path(prefix, p)
         if os.path.exists(experiment):
-            shutil.rmtree(experiment)            
+            if os.path.isfile(experiment):
+                os.remove(experiment)
+            else:
+                shutil.rmtree(experiment)
 
     def _experiment_file_params(self, p):
         str_params = ""
         for k, v in p.items():
-            if k == "samples" or k == "targets" or k == "savename_key_len":
+            if k == "samples" or k == "targets" or k == "savename_key_len" or k == "timeout_fit":
                 continue
             if type(v) == np.ndarray:
                 v = self._params_array_subsample_hash(v)
             keylen = p['savename_key_len'] if 'savename_key_len' in p else math.inf
             str_params += f"-{k[:min(keylen,len(k))]}_{v}"    # Restrict key length to first keylen characters
         str_params = str_params.replace('[','_').replace(']','_').replace(',','_') 
         return str_params
@@ -465,57 +401,85 @@
         # p = Path(self.datadir)
         # experiments = list(p.glob(f"{self.clf_name}-*"))
         prefix = f"{self.datadir}/{self.clf_name}"
         experiments = [
             prefix + self._experiment_file_params(p) for p in self.params_in_
         ]
         for i, experiment in enumerate(experiments):
-            logging.info(f"{experiment}")
-            if os.path.isdir(experiment):  # tf
-                clf = load_model(experiment)
-
-                # Restore model, including the manually saved attributes
-                with open(os.path.join(str(experiment), "autoencoder_attrs"), "rb") as fp:
-                    clf_attrs = pickle.load(fp)
-                # Change object's class to actual Autoencoder, so methods are available. Weird but works.
-                clf.__class__ = ModelsLoader.get_constructor(self.clf_algorithm)
-                # Update with the manually pickled attributes
-                clf.set_params(**clf_attrs)
-
-                with open(str(experiment) + "/metrics", "rb") as fp:
-                    metrics = pickle.load(fp)
-            else:
-                with open(experiment, "rb") as fp:
-                    metrics = pickle.load(fp)
-                clf = metrics["clf"]
-            self._compare_results(experiment, clf, metrics)
+            if os.path.exists(experiment):
+                logging.info(f"{experiment}")
+                if os.path.isdir(experiment):  # tf
+                    clf = load_model(experiment)
+
+                    # Restore model, including the manually saved attributes
+                    with open(os.path.join(str(experiment), "autoencoder_attrs"), "rb") as fp:
+                        clf_attrs = pickle.load(fp)
+                    # Change object's class to actual Autoencoder, so methods are available. Weird but works.
+                    clf.__class__ = ModelsLoader.get_constructor(self.clf_algorithm)
+                    # Update with the manually pickled attributes
+                    clf.set_params(**clf_attrs)
+
+                    with open(str(experiment) + "/metrics", "rb") as fp:
+                        metrics = pickle.load(fp)
+                else:
+                    with open(experiment, "rb") as fp:
+                        metrics = pickle.load(fp)
+                    clf = metrics["clf"]
+                self._compare_results(experiment, clf, metrics)
 
         params = str(self.best_experiment_).split("-")[1:]
         params = ",".join(params)
+        durationstr = f"{self.best_duration_:.2f}" if self.best_duration_ else f"{self.best_duration_}"
         logging.info(
-            f"{self.clf_name.upper()} BEST [{self.best_duration_:.2f}s]"
+            f"{self.clf_name.upper()} BEST [" + durationstr +"s]"  
             f"({params}): "
             f"{self.best_score_}"
         )
 
         if hasattr(self.best_estimator_, "get_params"):  # sklearn
             self.best_params_ = self.best_estimator_.get_params()
             self.labels_ = self.best_estimator_.labels_
 
     def _grid_get_estimators(self):
         p = Path(self.datadir)
+        
+        # Read saved estimators from folder
         experiments = list(p.glob(f"{self.clf_name}-*"))
+
+        # Keep only the experiments from the current session, match by path name
+        exp_names_current_session = [ os.path.join(p, f"{self.clf_name}") + self._experiment_file_params(e) for e in self.params_grid_noremove]
+        experiments = [e for e in experiments if str(e) in exp_names_current_session]
+
         for experiment in experiments:
-            with open(experiment, "rb") as fp:
-                # [clf, ba, tpr, tnr, duration, tn, fp, fn, tp] = pickle.load(fp)
-                metrics = pickle.load(fp)
-                clf = metrics["clf"]
+            logging.info(f"{experiment}")
+
+            if os.path.isdir(experiment):  # tf
+                clf = load_model(experiment)
+
+                # Restore model, including the manually saved attributes
+                with open(os.path.join(str(experiment), "autoencoder_attrs"), "rb") as fp:
+                    clf_attrs = pickle.load(fp)
+                # Change object's class to actual Autoencoder, so methods are available. Weird but works.
+                clf.__class__ = ModelsLoader.get_constructor(self.clf_algorithm)
+                # Update with the manually pickled attributes
+                clf.set_params(**clf_attrs)
+
+                with open(str(experiment) + "/metrics", "rb") as fp:
+                    metrics = pickle.load(fp)
+
                 self.estimators_.append(clf)
-                print(experiment)
-                print(clf)
+
+            else:
+                with open(experiment, "rb") as fp:
+                    # [clf, ba, tpr, tnr, duration, tn, fp, fn, tp] = pickle.load(fp)
+                    metrics = pickle.load(fp)
+                    clf = metrics["clf"]
+                    self.estimators_.append(clf)
+                    print(experiment)
+                    print(clf)
 
     def _grid_find_mean_std(self):
         bas = []
         p = Path(self.datadir)
         params = "-".join(str(e[0]) for e in self.params[:-1])  # skip round parameter
         experiments = list(p.glob(f"{self.clf_name}-{params}*"))
         for experiment in experiments:
@@ -528,49 +492,58 @@
         std = np.std(bas)
         logging.info(
             f"{self.clf_name.upper()} {len(experiments)} rounds ({params}): "
             f"max {max:.4f}, mean {mean:.4f}, std {std:.4f}"
         )
 
     def _grid_search(self, X, y):
-        self._grid_generate_search_space(X, y)
-        if self.refit:
-            self._grid_remove_existing_experiments()
-        else:
-            self._grid_remove_existing_tests()
 
-        if self.n_cpus == 1:
-            for p in self.params_grid:
-                self._test_clf(p)
+        # Try to retrieve a timeout for trainning each estimator
+        # Individual algorithm value (self.params), if specified, has precedence over global value self.timeout_fit)
+        timeout_fit = self.params['timeout_fit'][0] if 'timeout_fit' in self.params else self.timeout_fit
+
+        # Append new parameters so that _test_clf_static() can instantiate the model internally
+        new_params = {  "clf_algorithm": self.clf_algorithm,
+                        "clf_model_kwargs": self.clf_model_kwargs,
+                        "clf_type": self.clf_type,
+                        "datadir": self.datadir,
+                        "clf_name": self.clf_name,
+                        "timeout_fit": timeout_fit
+        }
+        # Merge new params with each set in the existing list
+        params_grid_augmented = []
+        for p in self.params_grid:
+            p_clone = p.copy()  # Make a clone of the parameters dict. In case of timeout error, added params are not popped, and pollute the original params list
+            p_clone.update({"experiment_file_params": self._experiment_file_params(p)})
+            p_clone.update(new_params)
+            params_grid_augmented.append(p_clone)
 
+        # For tf-based models, call _test_clf_static() instead of _test_clf
         # tf incompatible with mp according to tf issue #46316
-        elif self.clf_type == "tensorflow":
+        if self.clf_type == "tensorflow":
+            for p in params_grid_augmented:
 
-            # Append new parameters so that _test_clf_static() can instantiate the model internally
-            new_params = {  "clf_algorithm": self.clf_algorithm,
-                            "clf_model_kwargs": self.clf_model_kwargs,
-                            "clf_type": self.clf_type,
-                            "datadir": self.datadir,
-                            "clf_name": self.clf_name,
-            }
-            for p in self.params_grid:
-                p.update({"experiment_file_params": self._experiment_file_params(p)})
-                p.update(new_params)
+                # tf-based models cannot be run with timeout, because of incompatibility with mp
+                del p['timeout_fit']
 
-                self._test_clf_static(p)    
+                _test_clf_static(p)    
 
             # Still can't parallelize, models get instantiated but hang when fitting()
             # pool_obj = multiprocessing.Pool(self.n_cpus)
-            # pool_obj.map(self._test_clf_static, self.params_grid)
+            # pool_obj.map(_test_clf_static, params_grid_augmented)
+
+        elif self.n_cpus == 1:
+            for p in params_grid_augmented:
+                _test_clf_static(p)    
 
         else:
             pool_obj = multiprocessing.Pool(self.n_cpus)
-            pool_obj.map(self._test_clf, self.params_grid)
+            pool_obj.map(_test_clf_static, params_grid_augmented)
 
-    def fit(self, X, y=None):
+    def fit(self, X, y=None, only_cached=False):
         """Perform grid search on samples in `X` with the selected `clf`.
 
         Parameters
         ----------
         X: array-like of shape (n_samples, n_features)
             samples on which to fit the methods in `models_list`
 
@@ -580,25 +553,44 @@
 
         Returns
         -------
         self: object
             Fitted estimator.
         """
 
-        self._grid_search(X, y)
+        # Generate parameters
+        self._grid_generate_search_space(X, y)
+        if self.refit:
+            self._grid_remove_existing_experiments()
+        else:
+            self._grid_remove_existing_tests()
+
+        # Actual search
+        if not only_cached:
+            self._grid_search(X, y)
+
         if y is None:
             self._grid_get_estimators()
         else:
             self._grid_find_best_result()
+        #self.load(find_best=(y is not None))
 
     # def _test_rounds(self, X, y):
     #     self._grid_search(X, y)
     #     self._grid_find_mean_std()
 
 
+    # def load(self, find_best=False):
+    #     """Only loads existing (cached) estimators from disk
+    #     """
+    #     if find_best:
+    #         self._grid_find_best_result()
+    #     else:
+    #         self._grid_get_estimators()
+
 def _fpfn(cls, clf, y_pred, y_true):
     if y_true is None:
         metrics = {
             "ba": None,
             "tpr": None,
             "tnr": None,
             "tn": None,
@@ -628,7 +620,105 @@
     return metrics
 
 
 def _compare_metric_balanced_accuracy(cls, experiment, clf, metrics):
     if metrics["ba"] > cls.best_score_["ba"]:
         return True
     return False
+
+def _test_clf_static(params):
+    """Function version of _test_clf(), outside of class definition. Internally instantiates models from scratch.
+
+    Args:
+        params (dict): Dictionary with all necessary parameters, including the ones for instantiating models.
+
+    Returns:
+        dict: Metrics dict
+    """
+    X = params.pop("samples")
+    y = params.pop("targets")
+    clf_algorithm = params.pop("clf_algorithm")
+    clf_model_kwargs = params.pop("clf_model_kwargs")
+    clf_type = params.pop("clf_type")
+    datadir = params.pop("datadir")
+    clf_name = params.pop("clf_name")
+    experiment_file_params = params.pop("experiment_file_params")
+    if 'timeout_fit' in params:
+        timeout_fit = params.pop('timeout_fit')
+    else:
+        timeout_fit = None
+    
+    start = time.time()
+    logger.info(f"Fitting {clf_algorithm} with timeout={timeout_fit}: {experiment_file_params}")
+
+    # Create model from scratch and parameterize
+    clf = ModelsLoader.get(clf_algorithm, **clf_model_kwargs)
+    clf = clf.set_params(**params)
+
+    if timeout_fit is not None:
+
+        # Local function to replace clf.fit_predict()
+        # because we can't apply timeout() decorator directly to a function with side-effects
+        def clf_fit_predict(clf, X):
+            y_pred = clf.fit_predict(X)
+            return y_pred, clf
+
+        # Fit and catch a possible TimeoutError
+        try:
+            y_pred, clf = timeout(dec_timeout=timeout_fit, use_signals=False)(clf_fit_predict)(clf, X)
+        except TimeoutError as e:
+            logger.info(f"Timeout exceeded! : {experiment_file_params}")
+            return None
+    else:
+        y_pred = clf.fit_predict(X)
+    logger.info(f"Finished {clf_algorithm} {experiment_file_params}")
+
+    metrics = _fpfn(None, None, y_pred, y)
+    end = time.time()
+    duration = end - start
+    metrics["duration"] = duration
+
+    logger.debug(metrics)
+
+    fname = f"{datadir}/{clf_name}" + experiment_file_params
+
+    if clf_type == "tensorflow":  # tf is not pickle compatible
+
+        # Save model
+        clf.metrics_ = metrics
+        clf.save(fname)
+
+        # Manually pickle attributes in a separate file
+        attrs_to_pickle = clf.get_config()
+        attrs_to_pickle['optimizer'] = params['optimizer']
+        attrs_to_pickle['loss'] = params['loss']
+        pickle.dump(attrs_to_pickle, open(os.path.join(fname, 'autoencoder_attrs'),'wb'))
+
+        # Pickle metrics
+        pickle.dump(
+            # [ba, tpr, tnr, duration, tn, fp, fn, tp],
+            metrics,
+            open(
+                fname + "/metrics",
+                "wb",
+            ),
+        )
+
+        # Save metrics also as a text file
+        with open(os.path.join(fname, 'metrics.txt'), "w") as external_file:
+            pprint.pprint(metrics, stream=external_file)
+
+        # Save config to a text file
+        with open(os.path.join(fname, 'config.txt'), "w") as external_file:
+            pprint.pprint(clf.get_config(), stream=external_file)
+
+    else:
+        metrics["clf"] = clf
+        pickle.dump(
+            # [clf, ba, tpr, tnr, duration, tn, fp, fn, tp],
+            metrics,
+            open(
+                fname,
+                "wb",
+            ),
+        )
+    return metrics
```

### Comparing `graphomaly-0.2.6/graphomaly/models/autoencoder.py` & `graphomaly-0.2.7/graphomaly/models/autoencoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
+import logging
+logger = logging.getLogger(__name__)
+
 import numpy as np
 import tensorflow as tf
 from sklearn.preprocessing import MinMaxScaler
 from tensorflow.keras import activations, layers
 from tensorflow.keras.regularizers import L2
 from tensorflow.keras.callbacks import EarlyStopping, ReduceLROnPlateau
 
@@ -25,18 +28,20 @@
 @tf.keras.utils.register_keras_serializable()
 class Autoencoder(tf.keras.Model):
     """Autoencoder model introduced by Aggarwal C. [1]_
 
     Parameters
     ----------
     encoder_neurons : list
-        The number of neurons per encoder layers.
+        The number of neurons per encoder layers. 
+        Values > 1 are absolute, values <= 1 are relative to input size (e.g. [0.8, 0.4])
 
     decoder_neurons : list
-        The number of neurons per decoder layers.
+        The number of neurons per decoder layers. 
+        Values > 1 are absolute, values <= 1 are relative to input size (e.g. [0.8, 0.4])
 
     activation_function : str or callable, default='tanh'
         The activation function for all layers.
         See `Keras doc <https://keras.io/api/layers/activations/>`_.
 
     l2_regularizer : float in (0., 1), default=0.1
         The regularization factor for L2 regularizer for all layers.
@@ -48,117 +53,229 @@
         The threshold used for anomalies selection. If None, the
         contamination is used to compute the threshold.
 
     contamination : float, default=0.1
         The contamination rate used for computing the reconstruction error
         threshold. Used if threshold is not set.
 
+    optimizer: str or callable, default='adam'
+        The optimizer algorithm of the neural network.
+        See `Keras doc <https://keras.io/api/optimizers/>`_.
+
+    loss: str or callable, default='mse'
+        The loss function of the neural network.
+        See `Keras doc <https://keras.io/api/losses/>`_.
+
+    epochs: int, default=1000
+        Maximum number of epochs for network training.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        
+    batch_size: int, default=10000
+        Batch size used for training.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+
+    shuffle: boolean, default=True
+        Shuffle data before each epoch during training.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+
+    validation_size: float, default==0.1
+        Amount of training set used for validation.
+        See `validation_split` argument of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+
+    learning_rate : float, default==0.001
+        Gradient step size used in training.
+        Depends on the optimizer used.
+
+    verbose: int or str, default='auto'
+        Print training progress. Can be 0, 1, or 'auto'
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+
+    es_monitor: str or None, default='val_loss'
+        Quantity to monitor for early stopping of training.
+        Use None to disable EarlyStopping.
+        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`_.
+
+    es_patience: int, default=50
+        Early Stopping: how many epochs to wait before stop.
+        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`_.
+
+    redlr_monitor: str or None, default='val_loss'                  
+        Quantity to monitor for "Reduce Learning Rate on Plateau" during training.
+        Use None to disable ReduceLROnPlateau.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+
+    redlr_learning_rate_reduce_factor: float, default=0.2
+        Factor for reducing learning rate when plateau is detected. Must be < 1. 
+        Use None to disable ReduceLROnPlateau.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+
+    redlr_learning_rate_min: float, default=0.00001
+        Minimum learning rate allowed when reducing learning rate on plateau.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+
+    redlr_patience: int, default=10
+        How many epochs to wait before reducing learning rate on plateau.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+
+    savename_key_len: int, default=3
+        When saving the model, restrict key length in the name to this many characters.
+
     Attributes
     ----------
-    reconstruction_errors_ : array-like of shape (n_samples,)
-        The raw outlier scores for the training data. The anomalies have
-        a larger error score.
+    decision_scores_ : array-like of shape (n_samples,)
+        The raw outlier scores for the training data, i.e. the reconstruction errors. 
+        The anomalies have a larger error score.
 
     history_ : Keras Object
         The training history of the model.
 
     labels_ : list of int (0 or 1)
         The binary labels for the training data. 0 means inliers and 1 means
         outliers.
 
     threshold_ : float
         The threshold for the raw outliers scores.
 
+    encoder_neurons_ : list
+        The actual number of neurons per encoder layers, if decoder_neurons is relative
+
+    decoder_neurons_ : list
+        The actual number of neurons per decoder layers, if decoder_neurons is relative
+
     References
     ----------
     .. [1] Aggarwal C. (2015) Outlier Analysis. In: Data Mining. Springer,
         Cham. https://doi.org/10.1007/978-3-319-14142-8_8
     """
 
     def __init__(
         self,
-        encoder_neurons=None,
-        decoder_neurons=None,
-        activation_function="tanh",
-        l2_regularizer=0.1,
-        dropout=0.2,
-        threshold=None,
-        contamination=0.1,
-        optimizer=None,
-        loss=None,
-        epochs=None,
-        batch_size=None,
-        shuffle=None,
-        validation_size=None,
+        encoder_neurons = None,
+        decoder_neurons = None,
+        activation_function = "relu",
+        l2_regularizer = 0.1,
+        dropout = 0.5,
+        threshold = None,
+        contamination = 0.1,
+        optimizer = 'adam',
+        loss = "mse",
+        epochs = 1000,
+        batch_size = 10000,
+        shuffle = True,
+        validation_size = 0.1,
+        learning_rate = 0.001,
+        verbose = 1,
+        es_monitor = 'val_loss',                       # What to monitor. Required. Comment-out to disable EarlyStopping
+        es_patience = 50,                              # How many epochs to wait before stop. Defaults to 0.
+        redlr_monitor = 'val_loss',                    # What to monitor. Required. Comment-out to disable ReduceLROnPlateau
+        redlr_learning_rate_reduce_factor = 0.2,       # Reduce factor. Must be < 1. Required. Comment-out to disable ReduceLROnPlateau
+        redlr_learning_rate_min = 0.00001,             # Minimum learning rate. Defaults to 0.
+        redlr_patience = 10,                           # How many epochs to wait before reducing. Defaults to 10.
+        savename_key_len = 3                           # When saving, restrict key length in the name to this many characters
     ):
         super(Autoencoder, self).__init__()
 
+        # Fixed parameters, passed via __init__()
         self.encoder_neurons = encoder_neurons
         self.decoder_neurons = decoder_neurons
         self.activation_function = activation_function
         self.l2_regularizer = l2_regularizer
         self.dropout = dropout
+        self.threshold = threshold              # Fixed threshold parameter specified at instantiation, while threshold_ is the actual threshold to use
         self.contamination = contamination
-        self.threshold = threshold
-        self.classes = 2
-        self.reconstruction_errors_ = None
-        self.history_ = None
-        self.labels_ = None
-
         self.optimizer = optimizer
         self.loss = loss
         self.epochs = epochs
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.validation_size = validation_size
+        self.learning_rate = learning_rate
+        self.verbose = verbose
+        self.es_monitor = es_monitor
+        self.es_patience = es_patience
+        self.redlr_monitor = redlr_monitor
+        self.redlr_learning_rate_reduce_factor = redlr_learning_rate_reduce_factor
+        self.redlr_learning_rate_min = redlr_learning_rate_min
+        self.redlr_patience = redlr_patience
+        self.savename_key_len = savename_key_len
 
-        self._check_parameters()
-        self._build_model()
+        # Fixed parameters, internal
+        self.classes = 2
+
+        # Attributes estimated from data, ending with `_`
+        # See here for a general discussion: https://scikit-learn.org/stable/developers/develop.html
+        self.threshold_ = None                  # Threshold set based on contamination level, if self.threshold is None, else equal to threshold.
+        self.decision_scores_ = None
+        self.history_ = None
+        self.labels_ = None
+        self.encoder_neurons_ = None    # Actual layer sizes, if case encoder_neurons contains relative values
+        self.decoder_neurons_ = None    # Actual layer sizes, if case decoder_neurons contains relative values
+
+        # sk-learn: nothing should be done in constructor, not even validation
+        # validation and building the Keras model is done in fit(), after set_params()
 
     # See here: https://www.tensorflow.org/api_docs/python/tf/keras/utils/register_keras_serializable
     # "To be serialized and deserialized, classes must implement the get_config() method."
     def get_config(self):
-        return {"encoder_neurons": self.encoder_neurons,
-                "decoder_neurons": self.decoder_neurons,
-                "activation_function": self.activation_function,
-                "l2_regularizer": self.l2_regularizer,
-                "dropout": self.dropout,
-                "threshold": self.threshold,
-                "contamination": self.contamination,
-                "classes": self.classes,
-                "reconstruction_errors_": self.reconstruction_errors_,
-                "history_": self.history_,
-                "labels_": self.labels_,
-                "optimizer": self.optimizer,
-                "loss": self.loss,
-                "epochs": self.epochs,
-                "batch_size": self.batch_size,
-                "shuffle": self.shuffle,
-                "validation_size": self.validation_size
-        }
+        """Returns all data members of the object, i.e. both the parameters and the attributes (ending in `_`)
+
+        Needed for serialization / deserialization.
+        """
+        # Get object attributes
+        attributes = {  "classes": self.classes,
+                        "threshold_": self.threshold_,
+                        "decision_scores_": self.decision_scores_,
+                        "history_": self.history_,
+                        "labels_": self.labels_
+            }
+
+        # Join the parameters with the attributes in a single dict
+        params = self.get_params()
+        params.update(attributes)
+        return params
+
+    @classmethod
+    def from_config(cls, config):
+        """Instantiates an object based on a config dict returned by get_config()
+        """
+        
+        # Extract attributes from `config` and set later, they cannot be passed to __init__()
+        attrs = ["classes", "threshold_", "decision_scores_", "history_", "labels_"]
+        attrs_dict = {attr: config.pop(attr) for attr in attrs}
+
+        # Instantiate with the remaining keys        
+        instance = cls(**config)
+
+        # Set attributes
+        for attr, value in attrs_dict.items():
+            setattr(instance, attr, value)
+
+        return instance
 
     def _build_model(self):
+
         encoder_layers = []
-        for neurons in self.encoder_neurons:
+
+        for neurons in self.encoder_neurons_:
             linear_layer = layers.Dense(
                 neurons,
                 activation=self.activation_function,
                 activity_regularizer=L2(self.l2_regularizer),
             )
             dropout_layer = layers.Dropout(self.dropout)
 
             encoder_layers.append(linear_layer)
             encoder_layers.append(dropout_layer)
 
         decoder_layers = []
-        for ilayer, neurons in enumerate(self.decoder_neurons):
+        for ilayer, neurons in enumerate(self.decoder_neurons_):
 
             # The last layer should have no activation function
             activation = self.activation_function
-            if ilayer == len(self.decoder_neurons)-1:
+            if ilayer == len(self.decoder_neurons_)-1:
                 activation = 'linear'
 
             linear_layer = layers.Dense(
                 neurons,
                 activation=activation,
                 activity_regularizer=L2(self.l2_regularizer),
             )
@@ -167,34 +284,34 @@
             decoder_layers.append(linear_layer)
             decoder_layers.append(dropout_layer)
 
         self.encoder = tf.keras.Sequential(encoder_layers, name="encoder")
         self.decoder = tf.keras.Sequential(decoder_layers[:-1], name="decoder")
 
     def call(self, inputs):
-        if inputs.shape[1] != self.decoder_neurons[-1]:
+        if inputs.shape[1] != self.decoder_neurons_[-1]:
             raise ValueError(
                 "Expected the number of features to be equal to "
                 "the number of neurons on the last decoder layer. "
                 f"But found: {inputs.shape[1]} features and "
-                f"{self.decoder_neurons[-1]} neurons."
+                f"{self.decoder_neurons_[-1]} neurons."
             )
 
         encoded = self.encoder(inputs)
         decoded = self.decoder(encoded)
 
         return decoded
 
     def summary(self):
         """Print Autoencoder architecture on components."""
         print(self.encoder.summary())
         print(self.decoder.summary())
 
-    def predict_reconstruction_error(self, X):
-        """Predict the reconstruction errors for some samples.
+    def decision_function(self, X):
+        """Compute the reconstruction errors for some samples.
         The anomalies have a larger error score.
 
         This does not modify the object. Use for prediction, not fitting.
 
         Parameters
         ----------
         X : array-like of shape (num_samples, num_features)
@@ -206,60 +323,57 @@
             The reconstruction error scores.
         """
         preds = super().predict(X)
         return Autoencoder._compute_scores(X, preds)
 
     def predict_proba(self, X=None, method="linear", thresh=None):
         """Compute a distribution probability on the reconstuction errors
-        predicted for the samples passed as parameter. The scores as
-        normalized using a scaler fitted on the train scores, so the method
-        predict_decision_scores() must be called after training the model
-        in order to be able to compute the probabilities.
+        predicted for the samples passed as parameter. 
 
         This does not modify the object. Use for prediction, not fitting.
 
         If X is not None, the errors are computed for the data in X
-        If X is None, assume the erorrs are already available in self.reconstruction_errors_
+        If X is None, assume the erorrs are already available in self.decision_scores_
 
         Parameters
         ----------
         X : array-like of shape (num_samples, num_features)
             The samples for which to compute the probabilities.
 
         method : {'linear', 'hard', 'quantile'}, default='linear'
             The method used for score normalization. 
-            'linear': scale scores to [0, 1] range
-            'hard': hard thresholding with a given threshold `thresh`, return binary scores. If `thresh` is None, use self.threshold instead.
+            'linear': scale scores to [0, 1] range. Default.
+            'hard': hard thresholding with a given threshold `thresh`, return binary scores. If `thresh` is None, use self.threshold_ instead.
             'quantile': hard thresholding using the given quantile in `thresh`, 
                         e.g. thresh=0.1 assigns 0 to the smallest 10% errors, and 1 to the largest 90% errors.
 
         Returns
         -------
         ndarray of shape (num_samples, )
             The probabilities for each class (normal prob on dimension 0,
             anomaly prob on dimension 1).
         """
 
-        # If X is None, we process the error values stored in self.reconstruction_errors_
-        if X is None and self.reconstruction_errors_ is None:
+        # If X is None, we process the error values stored in self.decision_scores_
+        if X is None and self.decision_scores_ is None:
             raise Exception(
                 "Reconstruction errors on train set are not available."
             )
 
-        rec_errors = self.predict_reconstruction_error(X) if X is not None else self.reconstruction_errors_
+        rec_errors = self.decision_function(X) if X is not None else self.decision_scores_
 
         probs = np.zeros([rec_errors.shape[0], self.classes])
 
         if method == "linear":
             scaler = MinMaxScaler()
             probs[:, 1] = scaler.fit_transform(rec_errors.reshape(-1, 1)).squeeze()
             probs[:, 0] = 1 - probs[:, 1]
 
-        elif method == "hard" and (thresh is not None or self.threshold is not None):
-            thresh_local = thresh if thresh is not None else self.threshold   # given threshold, or fitted one
+        elif method == "hard" and (thresh is not None or self.threshold_ is not None):
+            thresh_local = thresh if thresh is not None else self.threshold_   # given threshold, or fitted one
             probs[:, 1] = (rec_errors > thresh_local).astype("int")
 
         elif method == "quantile" and thresh is not None:
             q_thresh = np.quantile(rec_errors, thresh)
             probs[:, 1] = (rec_errors > q_thresh).astype("int")
 
         else:
@@ -271,36 +385,62 @@
 
     def set_params(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
         return self
 
     def get_params(self, deep=True):
+        """Returns all parameters of the estimator. Needed for Scikit-learn compatibility
+        """
+
+        # Don't return the attributes (ending in `_``)
         return {
             "encoder_neurons": self.encoder_neurons,
             "decoder_neurons": self.decoder_neurons,
             "activation_function": self.activation_function,
             "l2_regularizer": self.l2_regularizer,
             "dropout": self.dropout,
             "contamination": self.contamination,
             "threshold": self.threshold,
             "optimizer": self.optimizer,
             "loss": self.loss,
             "epochs": self.epochs,
             "batch_size": self.batch_size,
             "shuffle": self.shuffle,
             "validation_size": self.validation_size,
-            #reconstruction_errors_?
-            #history_?
-            #labels_?
+            "learning_rate": self.learning_rate,
+            "verbose": self.verbose,
+            "es_monitor": self.es_monitor,
+            "es_patience": self.es_patience,
+            "redlr_monitor": self.redlr_monitor,
+            "redlr_learning_rate_reduce_factor": self.redlr_learning_rate_reduce_factor,
+            "redlr_learning_rate_min": self.redlr_learning_rate_min,
+            "redlr_patience": self.redlr_patience,
+            "savename_key_len": self.savename_key_len
         }
 
     def fit(self, X, y=None, **kwargs):
+
         self.set_params(**kwargs)
 
+        # When the last decoder layer has size 1, the values are relative. 
+        # Scale the numbers by input size.
+        # Note the trailing underscore_!
+        input_size = X.shape[1]
+        if round(self.decoder_neurons[-1]) == 1:
+            self.encoder_neurons_ = [round(v * input_size) for v in self.encoder_neurons]
+            self.decoder_neurons_ = [round(v * input_size) for v in self.decoder_neurons]
+            logger.info(f'Layer size was relative, actual sizes are: encoder: {self.encoder_neurons_}, decoder: {self.decoder_neurons_}')
+        else:
+            self.encoder_neurons_ = self.encoder_neurons
+            self.decoder_neurons_ = self.decoder_neurons
+
+        self._check_parameters()
+        self._build_model()
+
         self.compile(optimizer=self.optimizer, loss=self.loss)
 
         # Overwrite learning rate, if specified
         if hasattr(self, 'learning_rate'):
             self.optimizer.learning_rate = self.learning_rate
 
         # Add callbacks
@@ -332,20 +472,22 @@
                 verbose=self.verbose,
                 callbacks=callbacks
             )
             .history
         )
 
         # Fit the threshold, based on the reconstruction errors on the training set
-        self.reconstruction_errors_ = self.predict_reconstruction_error(X)
+        self.decision_scores_ = self.decision_function(X)
         if self.threshold is None:
-            self.threshold = np.quantile(self.reconstruction_errors_, 1 - self.contamination)
+            self.threshold_ = np.quantile(self.decision_scores_, 1 - self.contamination)
+        else:
+            self.threshold_ = self.threshold
 
         # Compute the labels on the training set
-        self.labels_ = self.predict_proba(method='hard', thresh=self.threshold)[:,1]
+        self.labels_ = self.predict_proba(method='hard', thresh=self.threshold_)[:,1]
 
         return self
 
     def predict(self, X):
         """Predict binary labels for the samples passed as parameter.
 
         This does not modify the object. Use for prediction, not fitting.
@@ -357,20 +499,20 @@
 
         Returns
         -------
         ndarray of shape (num_samples, )
             The predicted labels for all input.
         """
 
-        pred_score = self.predict_reconstruction_error(X)
-        labels = (pred_score > self.threshold).astype("int")
+        pred_score = self.decision_function(X)
+        labels = (pred_score > self.threshold_).astype("int")
         return labels
 
     def fit_predict(self, X, y=None):
-        #return self.fit(X, y).predict(X)
+        # Fit already does prediction internally, and the labels are in labels_
         return self.fit(X, y).labels_
 
     def _check_parameters(self):
         if not isinstance(self.encoder_neurons, list):
             raise TypeError(
                 "Expected encoder_neurons to have type list, but "
                 f"received {type(self.encoder_neurons)}"
@@ -378,19 +520,26 @@
 
         if not isinstance(self.decoder_neurons, list):
             raise TypeError(
                 "Expected decoder_neurons to have type list, but "
                 f"received {type(self.encoder_neurons)}"
             )
 
-        if not all(map(lambda x: isinstance(x, int), self.encoder_neurons)):
-            raise TypeError("Not all elements from encoder_neurons have int " "type")
+        if not all(map(lambda x: isinstance(x, int), self.encoder_neurons_)):
+            raise TypeError("Not all elements from encoder_neurons_ have int " "type")
+
+        if not all(map(lambda x: isinstance(x, int), self.decoder_neurons_)):
+            raise TypeError("Not all elements from decoder_neurons_ have int " "type")
+
+        # Check layers size is not 0
+        if any (map(lambda x: x == 0, self.encoder_neurons_)):
+            raise ValueError("Some layer size from encoder_neurons_ is 0")
 
-        if not all(map(lambda x: isinstance(x, int), self.decoder_neurons)):
-            raise TypeError("Not all elements from decoder_neurons have int " "type")
+        if any (map(lambda x: x == 0, self.decoder_neurons_)):
+            raise ValueError("Some layer size from decoder_neurons_ is 0")
 
         # Check regularizer type and value
         if not isinstance(self.l2_regularizer, float):
             raise TypeError(
                 "Expected l2_regularizer to have type float, but "
                 f"received {type(self.l2_regularizer)}"
             )
```

### Comparing `graphomaly-0.2.6/graphomaly/models/base_model.py` & `graphomaly-0.2.7/graphomaly/models/base_model.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/models/dictlearn.py` & `graphomaly-0.2.7/graphomaly/models/dictlearn.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import numpy as np
 import pandas as pd
 from dictlearn import DictionaryLearning
 from sklearn.preprocessing import MinMaxScaler
 
 
 class AnomalyDL(DictionaryLearning):
-    """Dictionary Learning [1]_ model for Unsupervised Anomaly Detection [2]_
+    """Dictionary Learning [DL1]_ model for Unsupervised Anomaly Detection [DL2]_
 
     Parameters
     ----------
     threshold : float, default=None
         The threshold used for anomalies selection. If None, the
         contamination is used to compute the threshold.
 
@@ -42,31 +42,37 @@
         outliers.
 
     threshold_ : float
         The threshold for the raw outliers scores.
 
     References
     ----------
-    .. [1] B. Dumitrescu and P. Irofti, Dictionary Learning Algorithms and
+    .. [DL1] B. Dumitrescu and P. Irofti, Dictionary Learning Algorithms and
            Applications, Springer, 2018. http://dx.doi.org/10.1007/978-3-319-78674-2
-    .. [2] P. Irofti and A. Băltoiu,Unsupervised Dictionary Learning for
+    .. [DL2] P. Irofti and A. Băltoiu,Unsupervised Dictionary Learning for
            Anomaly Detection, in International Traveling Workshop on Interactions
            Between Sparse Models and Technology, 2020, pp. 1--3
     """
 
     def __init__(
         self,
         threshold=None,
         contamination=None,
         **pparams,
     ):
         super().__init__(**pparams)
 
+        # Fixed parameters 
         self.contamination = contamination
-        self.threshold_ = threshold
+        self.threshold = threshold      # Fixed threshold parameter specified at instantiation, while threshold_ is the actual threshold to use
+        self.classes = 2
+
+        # Attributes estimated from data, ending with `_`
+        # See here for a general discussion: https://scikit-learn.org/stable/developers/develop.html
+        self.threshold_ = None          # Threshold set based on contamination level, if self.threshold is None, else equal to threshold.
         self.decision_scores_ = None
         self.labels_ = None
 
     def _estimate(self, X):
         codes = self.transform(X)
         preds = (self.D_.T @ codes.T).T
         return preds
@@ -90,23 +96,25 @@
         """
         preds = self._estimate(X_train)
 
         self.decision_scores_ = self._compute_scores(X_train, preds)
         self.scaler = MinMaxScaler()
         self.scaler.fit(self.decision_scores_.reshape(-1, 1))
 
-        if self.threshold_ is None:
+        if self.threshold is None:
             if self.contamination is None:
                 self.threshold_ = np.mean(self.decision_scores_) + np.std(
                     self.decision_scores_
                 )
             else:
                 self.threshold_ = pd.Series(self.decision_scores_).quantile(
                     1 - self.contamination
                 )
+        else:
+            self.threshold_ = self.threshold
 
         self.labels_ = (self.decision_scores_ > self.threshold_).astype("int")
 
         return self.decision_scores_
 
     def decision_function(self, X):
         """Predict the reconstruction errors for some samples.
@@ -190,9 +198,26 @@
         pred_score = self.decision_function(X)
         self.labels_ = (pred_score > self.threshold_).astype("int")
         return self.labels_
 
     def fit_predict(self, X, y=None):
         return self.fit(X, y).predict(X)
 
-    def _compute_scores(cls, X, Y):
+    @staticmethod
+    def _compute_scores(X, Y):
         return np.sqrt(np.sum(np.square(Y - X), axis=1))
+
+    # We need to get the params of both AnomalyDL and its parent, Dictionary Learning
+    # Not done automatically, see: https://github.com/scikit-learn/scikit-learn/issues/13555
+    def get_params(self, deep=True):
+
+        # Get params of current class (AnomalyDL) using the built-in get_params()
+        params = super(AnomalyDL, self).get_params()
+
+        # Get params of parent class (DictionaryLearning) by temporarily instantiating a parent object
+        all = vars(self)
+        parent_keys = DictionaryLearning().get_params(self).keys()
+        parent_params = {k: all[k] for k in parent_keys}
+
+        # Return their union
+        params.update(parent_params)
+        return params
```

### Comparing `graphomaly-0.2.6/graphomaly/models/models.py` & `graphomaly-0.2.7/graphomaly/models/models.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/models/sklearn.py` & `graphomaly-0.2.7/graphomaly/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/egonet.py` & `graphomaly-0.2.7/graphomaly/preprocessing/egonet.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/fe_base/historical_features.py` & `graphomaly-0.2.7/graphomaly/preprocessing/fe_base/historical_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/fe_base/statistical_features.py` & `graphomaly-0.2.7/graphomaly/preprocessing/fe_base/statistical_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/fe_base/time_features.py` & `graphomaly-0.2.7/graphomaly/preprocessing/fe_base/time_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/fe_difference_transformer.py` & `graphomaly-0.2.7/graphomaly/preprocessing/fe_difference_transformer.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/fe_statistical_transformer.py` & `graphomaly-0.2.7/graphomaly/preprocessing/fe_statistical_transformer.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/fe_time_transformers.py` & `graphomaly-0.2.7/graphomaly/preprocessing/fe_time_transformers.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/graph_to_features.py` & `graphomaly-0.2.7/graphomaly/preprocessing/graph_to_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/graph_to_spectrum_features.py` & `graphomaly-0.2.7/graphomaly/preprocessing/graph_to_spectrum_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/rwalk.py` & `graphomaly-0.2.7/graphomaly/preprocessing/rwalk.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/spectrum.py` & `graphomaly-0.2.7/graphomaly/preprocessing/spectrum.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly/preprocessing/transactions_to_graph.py` & `graphomaly-0.2.7/graphomaly/preprocessing/transactions_to_graph.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.6/graphomaly.egg-info/PKG-INFO` & `graphomaly-0.2.7/graphomaly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphomaly
-Version: 0.2.6
+Version: 0.2.7
 Summary: software package for anomaly detection in graphs modeling financial transactions
 Home-page: https://gitlab.com/unibuc/graphomaly/graphomaly
 Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
 Author-email: graphomaly@fmi.unibuc.ro
 Project-URL: Bug Tracker, https://gitlab.com/unibuc/graphomaly/graphomaly/-/issues
 Keywords: anomaly detection,graphs,financial transactions,machine learning,security
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphomaly-0.2.6/setup.cfg` & `graphomaly-0.2.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graphomaly
-version = 0.2.6
+version = 0.2.7
 author = Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
 author_email = graphomaly@fmi.unibuc.ro
 description = software package for anomaly detection in graphs modeling financial transactions
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = anomaly detection, graphs, financial transactions, machine learning, security
 url = https://gitlab.com/unibuc/graphomaly/graphomaly
@@ -33,14 +33,15 @@
 	pyod
 	python-louvain
 	PyYAML
 	scikit-learn
 	scipy
 	tensorflow
 	wheel
+	wrapt-timeout-decorator
 
 [options.packages.find]
 where = .
 exclude = tests
 
 [flake8]
 max-line-length = 88
```

