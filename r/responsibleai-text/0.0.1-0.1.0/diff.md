# Comparing `tmp/responsibleai_text-0.0.1.tar.gz` & `tmp/responsibleai_text-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_text-0.0.1.tar", last modified: Fri Apr  7 21:47:56 2023, max compression
+gzip compressed data, was "dist/responsibleai_text-0.1.0.tar", last modified: Wed Apr 12 20:55:46 2023, max compression
```

## Comparing `responsibleai_text-0.0.1.tar` & `responsibleai_text-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.287187 responsibleai_text-0.0.1/
--rw-rw-rw-   0        0        0     1410 2023-04-07 21:47:56.285961 responsibleai_text-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-02-24 21:18:43.000000 responsibleai_text-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.225944 responsibleai_text-0.0.1/responsibleai_text/
--rw-rw-rw-   0        0        0      355 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/responsibleai_text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.256948 responsibleai_text-0.0.1/responsibleai_text/common/
--rw-rw-rw-   0        0        0      127 2023-02-24 21:18:43.000000 responsibleai_text-0.0.1/responsibleai_text/common/__init__.py
--rw-rw-rw-   0        0        0      906 2023-02-24 21:18:43.000000 responsibleai_text-0.0.1/responsibleai_text/common/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.264952 responsibleai_text-0.0.1/responsibleai_text/managers/
--rw-rw-rw-   0        0        0      109 2023-02-24 21:18:43.000000 responsibleai_text-0.0.1/responsibleai_text/managers/__init__.py
--rw-rw-rw-   0        0        0    11935 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/responsibleai_text/managers/error_analysis_manager.py
--rw-rw-rw-   0        0        0    14509 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/responsibleai_text/managers/explainer_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.270944 responsibleai_text-0.0.1/responsibleai_text/rai_text_insights/
--rw-rw-rw-   0        0        0      241 2023-02-24 21:18:43.000000 responsibleai_text-0.0.1/responsibleai_text/rai_text_insights/__init__.py
--rw-rw-rw-   0        0        0    27523 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/responsibleai_text/rai_text_insights/rai_text_insights.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.278951 responsibleai_text-0.0.1/responsibleai_text/utils/
--rw-rw-rw-   0        0        0      128 2023-02-24 21:18:43.000000 responsibleai_text-0.0.1/responsibleai_text/utils/__init__.py
--rw-rw-rw-   0        0        0     3963 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/responsibleai_text/utils/feature_extractors.py
--rw-rw-rw-   0        0        0     2365 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/responsibleai_text/utils/question_answering.py
--rw-rw-rw-   0        0        0      192 2023-04-07 21:47:43.000000 responsibleai_text-0.0.1/responsibleai_text/version.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.250946 responsibleai_text-0.0.1/responsibleai_text.egg-info/
--rw-rw-rw-   0        0        0     1410 2023-04-07 21:47:55.000000 responsibleai_text-0.0.1/responsibleai_text.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      834 2023-04-07 21:47:55.000000 responsibleai_text-0.0.1/responsibleai_text.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 21:47:55.000000 responsibleai_text-0.0.1/responsibleai_text.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-04-07 21:47:55.000000 responsibleai_text-0.0.1/responsibleai_text.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-07 21:47:55.000000 responsibleai_text-0.0.1/responsibleai_text.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 21:47:56.287187 responsibleai_text-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1412 2023-02-28 22:07:46.000000 responsibleai_text-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:47:56.282951 responsibleai_text-0.0.1/tests/
--rw-rw-rw-   0        0        0     2053 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/tests/test_rai_text_insights.py
--rw-rw-rw-   0        0        0     5731 2023-04-07 21:45:23.000000 responsibleai_text-0.0.1/tests/test_rai_text_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25718 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/rai_text_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/utils/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/responsibleai_text/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/responsibleai_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:55:46.000000 responsibleai_text-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/tests/test_rai_text_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-12 20:53:15.000000 responsibleai_text-0.1.0/tests/test_rai_text_insights_save_and_load_scenarios.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `responsibleai_text-0.0.1/PKG-INFO` & `responsibleai_text-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: responsibleai_text
-Version: 0.0.1
-Summary: SDK API to assess text Machine Learning models.
-Home-page: https://github.com/microsoft/responsible-ai-toolbox
-Author: Roman Lutz, Ilya Matiach, Ke Xu
-Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Responsible AI Text SDK for Python
-
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
-
-The Responsible AI Text sdk enables users to analyze their machine learning models for text data in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
-
-Highlights of the package include:
-
-- `explainer.add()` explains the model
-
-### Supported scenarios, models and datasets
-
-The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
-
-The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-widgets
+Metadata-Version: 2.1
+Name: responsibleai_text
+Version: 0.1.0
+Summary: SDK API to assess text Machine Learning models.
+Home-page: https://github.com/microsoft/responsible-ai-toolbox
+Author: Roman Lutz, Ilya Matiach, Ke Xu
+Author-email: raiwidgets-maintain@microsoft.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# Responsible AI Text SDK for Python
+
+### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+
+The Responsible AI Text sdk enables users to analyze their machine learning models for text data in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
+
+Highlights of the package include:
+
+- `explainer.add()` explains the model
+
+### Supported scenarios, models and datasets
+
+The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
+
+The open source code for the visualization dashboard can be found here:
+https://github.com/microsoft/responsible-ai-widgets
```

### Comparing `responsibleai_text-0.0.1/README.md` & `responsibleai_text-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.0.1/responsibleai_text/common/constants.py` & `responsibleai_text-0.1.0/responsibleai_text/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.0.1/responsibleai_text/managers/error_analysis_manager.py` & `responsibleai_text-0.1.0/responsibleai_text/managers/error_analysis_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,18 @@
             dataset.drop(columns=target_column, inplace=True)
             ext_dataset.drop(columns=target_column, inplace=True)
             target_column = LABELS
             is_multilabel = True
         index_predictor = ErrorAnalysisManager._create_index_predictor(
             model, dataset, target_column, is_multilabel, task_type,
             index_classes)
-        categorical_features = []
+        if task_type == ModelTask.QUESTION_ANSWERING:
+            categorical_features = ['question_type']
+        else:
+            categorical_features = []
         super(ErrorAnalysisManager, self).__init__(
             index_predictor, ext_dataset, target_column,
             classes, categorical_features)
 
     @staticmethod
     def _create_index_predictor(model, dataset, target_column,
                                 is_multilabel, task_type, classes=None):
@@ -263,14 +266,15 @@
                                            index_classes)
             index_dataset.drop(columns=target_column, inplace=True)
             index_dataset[LABELS] = labels
             target_column = LABELS
             is_multilabel = True
             true_y = index_dataset[target_column]
         inst.__dict__['_true_y'] = true_y
+        inst.__dict__['_task_type'] = rai_insights.task_type
         index_predictor = ErrorAnalysisManager._create_index_predictor(
             wrapped_model, index_dataset, target_column, is_multilabel,
             rai_insights.task_type, index_classes)
         inst.__dict__['_analyzer'] = ModelAnalyzer(index_predictor,
                                                    dataset,
                                                    true_y,
                                                    feature_names,
```

### Comparing `responsibleai_text-0.0.1/responsibleai_text/managers/explainer_manager.py` & `responsibleai_text-0.1.0/responsibleai_text/managers/explainer_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,42 +32,36 @@
 CONTEXT = QuestionAnsweringFields.CONTEXT
 QUESTIONS = QuestionAnsweringFields.QUESTIONS
 SEP = Tokens.SEP
 SPARSE_NUM_FEATURES_THRESHOLD = 1000
 IS_RUN = 'is_run'
 IS_ADDED = 'is_added'
 CLASSES = 'classes'
-U_INITIALIZATION_EXAMPLES = '_initialization_examples'
 U_EVALUATION_EXAMPLES = '_evaluation_examples'
 FEATURES = 'features'
 META_JSON = Metadata.META_JSON
 MODEL = Metadata.MODEL
 EXPLANATION = '_explanation'
 TASK_TYPE = '_task_type'
 
 
 class ExplainerManager(BaseManager):
 
     """Defines the ExplainerManager for explaining a text-based model."""
 
-    def __init__(self, model: Any, initialization_examples: pd.DataFrame,
-                 evaluation_examples: pd.DataFrame,
+    def __init__(self, model: Any, evaluation_examples: pd.DataFrame,
                  target_column: str,
                  task_type: str,
                  classes: Optional[List] = None):
         """Creates an ExplainerManager object.
 
         :param model: The model to explain.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
-        :param initialization_examples: A matrix of feature vector
-            examples (# examples x # features) for initializing the explainer,
-            with an additional label column.
-        :type initialization_examples: pandas.DataFrame
         :param evaluation_examples: A matrix of feature vector
             examples (# examples x # features) on which to explain the
             model's output, with an additional label column.
         :type evaluation_examples: pandas.DataFrame
         :param target_column: The name of the label column or list of columns.
             This is a list of columns for multilabel models.
         :type target_column: str or list[str]
@@ -78,21 +72,19 @@
             output.  Only required if explaining classifier.
         :type classes: list
         """
         self._model = model
         self._target_column = target_column
         if not isinstance(target_column, list):
             target_column = [target_column]
-        self._initialization_examples = \
-            initialization_examples.drop(columns=target_column)
         self._evaluation_examples = \
             evaluation_examples.drop(columns=target_column)
         self._is_run = False
         self._is_added = False
-        self._features = list(self._initialization_examples.columns)
+        self._features = list(self._evaluation_examples.columns)
         self._classes = classes
         self._explanation = None
         self._task_type = task_type
 
     def add(self):
         """Add an explainer to be computed later."""
         if self._model is None:
@@ -347,15 +339,13 @@
             inst.__dict__[EXPLANATION] = None
 
         inst.__dict__['_' + MODEL] = rai_insights.model
         inst.__dict__['_' + CLASSES] = rai_insights._classes
         target_column = rai_insights.target_column
         if not isinstance(target_column, list):
             target_column = [target_column]
-        train = rai_insights.train.drop(columns=target_column)
         test = rai_insights.test.drop(columns=target_column)
-        inst.__dict__[U_INITIALIZATION_EXAMPLES] = train
         inst.__dict__[U_EVALUATION_EXAMPLES] = test
-        inst.__dict__['_' + FEATURES] = list(train.columns)
+        inst.__dict__['_' + FEATURES] = list(test.columns)
         inst.__dict__[TASK_TYPE] = rai_insights.task_type
 
         return inst
```

### Comparing `responsibleai_text-0.0.1/responsibleai_text/rai_text_insights/rai_text_insights.py` & `responsibleai_text-0.1.0/responsibleai_text/rai_text_insights/rai_text_insights.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,47 +27,44 @@
 from responsibleai_text.managers.error_analysis_manager import \
     ErrorAnalysisManager
 from responsibleai_text.managers.explainer_manager import ExplainerManager
 from responsibleai_text.utils.feature_extractors import extract_features
 
 _PREDICTIONS = 'predictions'
 _PREDICT_OUTPUT = 'predict_output'
-_TRAIN = 'train'
+_TEST = 'test'
 _TARGET_COLUMN = 'target_column'
 _TASK_TYPE = 'task_type'
 _CLASSES = 'classes'
 _META_JSON = Metadata.META_JSON
-_TRAIN_LABELS = 'train_labels'
 _JSON_EXTENSION = '.json'
 _PREDICT = 'predict'
 _PREDICT_PROBA = 'predict_proba'
 _EXT_TEST = '_ext_test'
 _EXT_FEATURES = '_ext_features'
 
 
 class RAITextInsights(RAIBaseInsights):
     """Defines the top-level RAITextInsights API.
 
     Use RAITextInsights to assess text machine learning models in a
     single API.
     """
 
-    def __init__(self, model: Any, train: pd.DataFrame, test: pd.DataFrame,
+    def __init__(self, model: Any, test: pd.DataFrame,
                  target_column: str, task_type: str,
                  classes: Optional[np.ndarray] = None,
                  serializer: Optional[Any] = None,
                  maximum_rows_for_test: int = 5000):
         """Creates an RAITextInsights object.
 
         :param model: The model to compute RAI insights for.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
-        :param train: The training dataset including the label column.
-        :type train: pandas.DataFrame
         :param test: The test dataset including the label column.
         :type test: pandas.DataFrame
         :param target_column: The name of the label column or list of columns.
             This is a list of columns for multilabel models.
         :type target_column: str or list[str]
         :param task_type: The task to run.
         :type task_type: str
@@ -81,64 +78,64 @@
         :type serializer: object
         :param maximum_rows_for_test: Limit on size of test data
             (for performance reasons)
         :type maximum_rows_for_test: int
         """
         # drop index as this can cause issues later like when copying
         # target column below from test dataset to _ext_test_df
-        train = train.reset_index(drop=True)
         test = test.reset_index(drop=True)
         self._wrapped_model = wrap_model(model, test, task_type)
         self._validate_rai_insights_input_parameters(
-            model=self._wrapped_model, train=train, test=test,
+            model=self._wrapped_model, test=test,
             target_column=target_column, task_type=task_type,
             classes=classes,
             serializer=serializer,
             maximum_rows_for_test=maximum_rows_for_test)
         self._classes = RAITextInsights._get_classes(
             task_type=task_type,
-            train=train,
+            test=test,
             target_column=target_column,
             classes=classes
         )
         ext_test, ext_features = extract_features(test,
                                                   target_column,
                                                   task_type)
         self._ext_test = ext_test
         self._ext_features = ext_features
         self._ext_test_df = pd.DataFrame(ext_test, columns=ext_features)
         self._ext_test_df[target_column] = test[target_column]
         self.predict_output = None
 
+        # TODO: on next responsibleai package upgrade pass None for train
         super(RAITextInsights, self).__init__(
-            model, train, test, target_column, task_type,
+            model, test, test, target_column, task_type,
             serializer)
         self._initialize_managers()
 
     def _initialize_managers(self):
         """Initializes the managers.
 
         Initializes the explainer and error analysis managers.
         """
         self._explainer_manager = ExplainerManager(
-            self.model, self.train, self.test,
+            self.model, self.test,
             self.target_column,
             self.task_type,
             self._classes)
         self._error_analysis_manager = ErrorAnalysisManager(
             self._wrapped_model, self.test, self._ext_test_df,
             self.target_column, self.task_type, self._classes)
         self._managers = [self._explainer_manager,
                           self._error_analysis_manager]
 
     @staticmethod
-    def _get_classes(task_type, train, target_column, classes):
+    def _get_classes(task_type, test, target_column, classes):
         if task_type == ModelTask.TEXT_CLASSIFICATION:
             if classes is None:
-                classes = train[target_column].unique()
+                classes = test[target_column].unique()
                 # sort the classes after calling unique in numeric case
                 classes.sort()
                 return classes
             else:
                 return classes
         elif task_type == ModelTask.MULTILABEL_TEXT_CLASSIFICATION:
             if classes is None:
@@ -164,65 +161,57 @@
 
         try:
             pickle.dumps(serializer)
         except Exception:
             raise UserConfigValidationException(
                 'The serializer should be serializable via pickle')
 
-    def _validate_model(self, model: Any, train: pd.DataFrame, test: pd.DataFrame,
+    def _validate_model(self, model: Any, test: pd.DataFrame,
                         target_column: Union[str, List], task_type: str):
         """Validate the model.
 
         :param model: The model to validate.
         :type model: object
-        :param train: The training dataset including the label column.
-        :type train: pandas.DataFrame
         :param test: The test dataset including the label column.
         :type test: pandas.DataFrame
         :param target_column: The name of the label column or list of columns.
             This is a list of columns for multilabel models.
         :type target_column: str or list[str]
         :param task_type: The task to run, can be `classification` or
             `regression`.
         :type task_type: str
         """
         if not isinstance(target_column, list):
             target_column = [target_column]
-        # Pick one row from train and test data
-        small_train_data = train.iloc[0:1].drop(
-            target_column, axis=1).iloc[0]
+        # Pick one row from test data
         small_test_data = test.iloc[0:1].drop(
             target_column, axis=1).iloc[0]
         if task_type != ModelTask.QUESTION_ANSWERING:
-            small_train_data = small_train_data.tolist()
             small_test_data = small_test_data.tolist()
         # Call the model
         try:
-            model.predict(small_train_data)
             model.predict(small_test_data)
         except Exception:
             raise UserConfigValidationException(
                 'The model passed cannot be used for'
                 ' getting predictions via predict()'
             )
 
     def _validate_rai_insights_input_parameters(
-            self, model: Any, train: pd.DataFrame, test: pd.DataFrame,
+            self, model: Any, test: pd.DataFrame,
             target_column: Union[str, List], task_type: str,
             classes: np.ndarray,
             serializer,
             maximum_rows_for_test: int):
         """Validate the inputs for the RAITextInsights constructor.
 
         :param model: The model to compute RAI insights for.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
-        :param train: The training dataset including the label column.
-        :type train: pandas.DataFrame
         :param test: The test dataset including the label column.
         :type test: pandas.DataFrame
         :param target_column: The name of the label column or list of columns.
             This is a list of columns for multilabel models.
         :type target_column: str or list[str]
         :param task_type: The task to run, can be `classification` or
             `regression`.
@@ -257,76 +246,57 @@
             warnings.warn(
                 'INVALID-MODEL-WARNING: No valid model is supplied. '
                 'Explanations will not work')
 
         if serializer is not None:
             self._validate_serializer(serializer)
 
-        train_is_pd = isinstance(train, pd.DataFrame)
         test_is_pd = isinstance(test, pd.DataFrame)
-        if not train_is_pd or not test_is_pd:
+        if not test_is_pd:
             raise UserConfigValidationException(
-                "Unsupported data type for either train or test. "
-                "Expecting pandas DataFrame for train and test."
+                "Unsupported data type for test dataset. "
+                "Expecting pandas DataFrame."
             )
 
         if test.shape[0] > maximum_rows_for_test:
             msg_fmt = 'The test data has {0} rows, ' +\
                 'but limit is set to {1} rows. ' +\
                 'Please resample the test data or ' +\
                 'adjust maximum_rows_for_test'
             raise UserConfigValidationException(
                 msg_fmt.format(
                     test.shape[0], maximum_rows_for_test)
             )
 
-        if len(set(train.columns) - set(test.columns)) != 0 or \
-                len(set(test.columns) - set(train.columns)):
-            raise UserConfigValidationException(
-                'The features in train and test data do not match')
-
         if task_type == ModelTask.MULTILABEL_TEXT_CLASSIFICATION.value:
             if not isinstance(target_column, list):
                 raise UserConfigValidationException(
                     'The target_column should be a list for multilabel '
                     'classification')
-            # check all target columns are present in train and test
+            # check all target columns are present in test
             target_columns_set = set(target_column)
-            if not target_columns_set.issubset(set(train.columns)):
-                raise UserConfigValidationException(
-                    'The list of target_column(s) should be in train data')
             if not target_columns_set.issubset(set(test.columns)):
                 raise UserConfigValidationException(
                     'The list of target_column(s) should be in test data')
         else:
-            if target_column not in list(train.columns) or \
-                    target_column not in list(test.columns):
+            if target_column not in list(test.columns):
                 raise UserConfigValidationException(
-                    'Target name {0} not present in train/test data'.format(
+                    'Target name {0} not present in test data'.format(
                         target_column)
                 )
 
-        if classes is not None and task_type == \
-                ModelTask.TEXT_CLASSIFICATION:
-            if len(set(train[target_column].unique()) -
-                    set(classes)) != 0 or \
-                    len(set(classes) -
-                        set(train[target_column].unique())) != 0:
-                raise UserConfigValidationException(
-                    'The train labels and distinct values in '
-                    'target (train data) do not match')
-
+        if classes is not None and task_type == ModelTask.TEXT_CLASSIFICATION:
             if len(set(test[target_column].unique()) -
                     set(classes)) != 0:
                 raise UserConfigValidationException(
                     'The test labels are not a subset of the '
                     'distinct values in target (test data)')
 
         if model is not None:
-            self._validate_model(model, train, test, target_column,
+            self._validate_model(model, test, target_column,
                                  task_type)
 
     def get_filtered_test_data(self, filters, composite_filters,
                                include_original_columns_only=False,
                                use_entire_test_data=False):
         """Get the filtered test data based on cohort filters.
 
@@ -409,16 +379,15 @@
         :type path: str
         """
         super(RAITextInsights, self).save(path)
         # Save extracted features data
         self._save_ext_data(path)
 
     def _save_ext_data(self, path):
-        """Save the copy of raw data (train and test sets) and
-           their related metadata.
+        """Save the copy of raw data and their related metadata.
 
         :param path: The directory path to save the RAIBaseInsights to.
         :type path: str
         """
         data_directory = Path(path) / SerializationAttributes.DATA_DIRECTORY
         ext_path = data_directory / (_EXT_TEST + _JSON_EXTENSION)
         ext_features_path = data_directory / (_EXT_FEATURES + _JSON_EXTENSION)
@@ -605,23 +574,19 @@
         top_dir = Path(path)
         with open(top_dir / _META_JSON, 'r') as meta_file:
             meta = meta_file.read()
         meta = json.loads(meta)
         inst.__dict__[_TARGET_COLUMN] = meta[_TARGET_COLUMN]
         inst.__dict__[_TASK_TYPE] = meta[_TASK_TYPE]
         inst.__dict__[_PREDICT_OUTPUT] = None
-        classes = None
-        if _TRAIN_LABELS in meta:
-            classes = meta[_TRAIN_LABELS]
-        else:
-            classes = meta[_CLASSES]
+        classes = meta[_CLASSES]
 
         inst.__dict__['_' + _CLASSES] = RAITextInsights._get_classes(
             task_type=meta[_TASK_TYPE],
-            train=inst.__dict__[_TRAIN],
+            test=inst.__dict__[_TEST],
             target_column=meta[_TARGET_COLUMN],
             classes=classes
         )
         # load the extracted features as part of metadata
         RAITextInsights._load_ext_data(inst, path)
 
     @staticmethod
```

### Comparing `responsibleai_text-0.0.1/responsibleai_text/utils/question_answering.py` & `responsibleai_text-0.1.0/responsibleai_text/utils/question_answering.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.0.1/responsibleai_text.egg-info/PKG-INFO` & `responsibleai_text-0.1.0/responsibleai_text.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: responsibleai-text
-Version: 0.0.1
-Summary: SDK API to assess text Machine Learning models.
-Home-page: https://github.com/microsoft/responsible-ai-toolbox
-Author: Roman Lutz, Ilya Matiach, Ke Xu
-Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Responsible AI Text SDK for Python
-
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
-
-The Responsible AI Text sdk enables users to analyze their machine learning models for text data in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
-
-Highlights of the package include:
-
-- `explainer.add()` explains the model
-
-### Supported scenarios, models and datasets
-
-The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
-
-The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-widgets
+Metadata-Version: 2.1
+Name: responsibleai-text
+Version: 0.1.0
+Summary: SDK API to assess text Machine Learning models.
+Home-page: https://github.com/microsoft/responsible-ai-toolbox
+Author: Roman Lutz, Ilya Matiach, Ke Xu
+Author-email: raiwidgets-maintain@microsoft.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# Responsible AI Text SDK for Python
+
+### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+
+The Responsible AI Text sdk enables users to analyze their machine learning models for text data in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
+
+Highlights of the package include:
+
+- `explainer.add()` explains the model
+
+### Supported scenarios, models and datasets
+
+The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
+
+The open source code for the visualization dashboard can be found here:
+https://github.com/microsoft/responsible-ai-widgets
```

### Comparing `responsibleai_text-0.0.1/responsibleai_text.egg-info/SOURCES.txt` & `responsibleai_text-0.1.0/responsibleai_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.0.1/setup.py` & `responsibleai_text-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.0.1/tests/test_rai_text_insights.py` & `responsibleai_text-0.1.0/tests/test_rai_text_insights.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,19 +32,25 @@
         task_type = ModelTask.MULTILABEL_TEXT_CLASSIFICATION
         labels = COVID19_EVENTS_LABELS
         run_rai_insights(pred, data, data[:5], labels, task_type)
 
 
 def run_rai_insights(model, train_data, test_data,
                      target_column, task_type):
-    rai_insights = RAITextInsights(model, train_data, test_data,
+    if task_type == ModelTask.TEXT_CLASSIFICATION:
+        classes = train_data[target_column].unique()
+        classes.sort()
+    else:
+        classes = None
+    rai_insights = RAITextInsights(model, test_data,
                                    target_column,
-                                   task_type=task_type)
+                                   task_type=task_type,
+                                   classes=classes)
     rai_insights.explainer.add()
     if task_type != ModelTask.QUESTION_ANSWERING:
         rai_insights.error_analysis.add()
     rai_insights.compute()
     rai_insights.get_data()
     # Validate
     validate_rai_text_insights(
-        rai_insights, train_data, test_data,
+        rai_insights, classes, test_data,
         target_column, task_type)
```

### Comparing `responsibleai_text-0.0.1/tests/test_rai_text_insights_save_and_load_scenarios.py` & `responsibleai_text-0.1.0/tests/test_rai_text_insights_save_and_load_scenarios.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 class TestRAITextInsightsSaveAndLoadScenarios(object):
 
     def test_rai_insights_empty_save_load_save(self):
         data = load_emotion_dataset()
         pred = create_text_classification_pipeline()
         train = data
         test = data[:3]
+        classes = train[EMOTION].unique()
+        classes.sort()
 
         rai_insights = RAITextInsights(
-            pred, train, test, EMOTION,
+            pred, test, EMOTION,
             task_type=ModelTask.TEXT_CLASSIFICATION,
-            serializer=TextClassificationPipelineSerializer())
+            serializer=TextClassificationPipelineSerializer(),
+            classes=classes)
 
         with TemporaryDirectory() as tmpdir:
             save_1 = Path(tmpdir) / "first_save"
             save_2 = Path(tmpdir) / "second_save"
 
             # Save it
             rai_insights.save(save_1)
@@ -39,34 +42,37 @@
             assert len(os.listdir(save_1 / ManagerNames.ERROR_ANALYSIS)) == 0
 
             # Load
             rai_2 = RAITextInsights.load(save_1)
 
             # Validate
             validate_rai_text_insights(
-                rai_2, train, test,
+                rai_2, classes, test,
                 EMOTION, ModelTask.TEXT_CLASSIFICATION)
 
             # Save again
             rai_2.save(save_2)
             assert len(os.listdir(save_2 / ManagerNames.EXPLAINER)) == 0
             assert len(os.listdir(save_2 / ManagerNames.ERROR_ANALYSIS)) == 0
 
     @pytest.mark.parametrize('manager_type', [ManagerNames.EXPLAINER,
                                               ManagerNames.ERROR_ANALYSIS])
     def test_rai_insights_save_load_add_save(self, manager_type):
         data = load_emotion_dataset()
         pred = create_text_classification_pipeline()
         train = data
         test = data[:3]
+        classes = train[EMOTION].unique()
+        classes.sort()
 
         rai_insights = RAITextInsights(
-            pred, train, test, EMOTION,
+            pred, test, EMOTION,
             task_type=ModelTask.TEXT_CLASSIFICATION,
-            serializer=TextClassificationPipelineSerializer())
+            serializer=TextClassificationPipelineSerializer(),
+            classes=classes)
 
         with TemporaryDirectory() as tmpdir:
             save_1 = Path(tmpdir) / "first_save"
             save_2 = Path(tmpdir) / "second_save"
 
             # Save it
             rai_insights.save(save_1)
@@ -83,30 +89,33 @@
                 raise ValueError(
                     "Bad manager_type: {0}".format(manager_type))
 
             rai_2.compute()
 
             # Validate
             validate_rai_text_insights(
-                rai_2, train, test,
+                rai_2, classes, test,
                 EMOTION, ModelTask.TEXT_CLASSIFICATION)
 
             # Save again
             rai_2.save(save_2)
 
     def test_loading_rai_insights_without_model_file(self):
         data = load_emotion_dataset()
         pred = create_text_classification_pipeline()
         train = data
         test = data[:3]
+        classes = train[EMOTION].unique()
+        classes.sort()
 
         rai_insights = RAITextInsights(
-            pred, train, test, EMOTION,
+            pred, test, EMOTION,
             task_type=ModelTask.TEXT_CLASSIFICATION,
-            serializer=TextClassificationPipelineSerializer())
+            serializer=TextClassificationPipelineSerializer(),
+            classes=classes)
 
         with TemporaryDirectory() as tmpdir:
             assert rai_insights.model is not None
             save_path = Path(tmpdir) / "rai_insights"
             rai_insights.save(save_path)
 
             # Remove the model.pkl file to cause an exception to occur
@@ -122,19 +131,22 @@
     @pytest.mark.parametrize('manager_type', [ManagerNames.EXPLAINER,
                                               ManagerNames.ERROR_ANALYSIS])
     def test_rai_insights_add_save_load_save(self, manager_type):
         data = load_emotion_dataset()
         pred = create_text_classification_pipeline()
         train = data
         test = data[:3]
+        classes = train[EMOTION].unique()
+        classes.sort()
 
         rai_insights = RAITextInsights(
-            pred, train, test, EMOTION,
+            pred, test, EMOTION,
             task_type=ModelTask.TEXT_CLASSIFICATION,
-            serializer=TextClassificationPipelineSerializer())
+            serializer=TextClassificationPipelineSerializer(),
+            classes=classes)
 
         # Call a single manager
         if manager_type == ManagerNames.EXPLAINER:
             rai_insights.explainer.add()
         elif manager_type == ManagerNames.ERROR_ANALYSIS:
             rai_insights.error_analysis.add()
         else:
@@ -151,12 +163,12 @@
             rai_insights.save(save_1)
 
             # Load
             rai_2 = RAITextInsights.load(save_1)
 
             # Validate
             validate_rai_text_insights(
-                rai_2, train, test,
+                rai_2, classes, test,
                 EMOTION, ModelTask.TEXT_CLASSIFICATION)
 
             # Save again
             rai_2.save(save_2)
```

