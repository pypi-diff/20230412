# Comparing `tmp/gmltools-0.0.41.tar.gz` & `tmp/gmltools-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.41.tar", last modified: Tue Apr 11 09:53:19 2023, max compression
+gzip compressed data, was "gmltools-0.0.42.tar", last modified: Wed Apr 12 10:45:05 2023, max compression
```

## Comparing `gmltools-0.0.41.tar` & `gmltools-0.0.42.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.528497 gmltools-0.0.41/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.41/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.41/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-11 09:53:19.528497 gmltools-0.0.41/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.41/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.507324 gmltools-0.0.41/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.41/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.41/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.41/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.41/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.41/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.41/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-11 09:52:11.000000 gmltools-0.0.41/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 09:53:19.528497 gmltools-0.0.41/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-11 09:51:56.000000 gmltools-0.0.41/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.495361 gmltools-0.0.41/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.509317 gmltools-0.0.41/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.41/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.41/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.517330 gmltools-0.0.41/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.41/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.41/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.521601 gmltools-0.0.41/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.41/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.41/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.41/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0    88338 2023-04-11 09:50:45.000000 gmltools-0.0.41/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.41/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.41/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.525077 gmltools-0.0.41/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.41/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73495 2023-04-11 09:50:48.000000 gmltools-0.0.41/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.41/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.527460 gmltools-0.0.41/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.41/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.41/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.41/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.41/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.514805 gmltools-0.0.41/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.907029 gmltools-0.0.42/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.42/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.42/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-12 10:45:05.906077 gmltools-0.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.42/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.707172 gmltools-0.0.42/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.42/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.42/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.42/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.42/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.42/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.42/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-12 10:44:04.000000 gmltools-0.0.42/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:45:05.907029 gmltools-0.0.42/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-12 10:43:53.000000 gmltools-0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.631458 gmltools-0.0.42/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.726798 gmltools-0.0.42/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.42/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.42/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.770934 gmltools-0.0.42/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.42/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.42/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.824852 gmltools-0.0.42/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.42/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.42/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.42/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0   118550 2023-04-12 10:42:43.000000 gmltools-0.0.42/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.42/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.42/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.860878 gmltools-0.0.42/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.42/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 10:42:46.000000 gmltools-0.0.42/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.42/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.904142 gmltools-0.0.42/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.42/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.42/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.42/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.42/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:45:05.758885 gmltools-0.0.42/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-12 10:45:05.000000 gmltools-0.0.42/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-12 10:45:05.000000 gmltools-0.0.42/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:45:05.000000 gmltools-0.0.42/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-12 10:45:05.000000 gmltools-0.0.42/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 10:45:05.000000 gmltools-0.0.42/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.41/LICENSE` & `gmltools-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/Models.ipynb` & `gmltools-0.0.42/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/PKG-INFO` & `gmltools-0.0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.41
+Version: 0.0.42
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.41/README.md` & `gmltools-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.42/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.42/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.42/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.42/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/gmltools.yml` & `gmltools-0.0.42/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/mltools.yml` & `gmltools-0.0.42/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/pyproject.toml` & `gmltools-0.0.42/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.41"
+version = "0.0.42"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.41/setup.py` & `gmltools-0.0.42/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.41',
+    'version': '0.0.42',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.41/src/gmltools/To_Do.txt` & `gmltools-0.0.42/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/eda/eda.py` & `gmltools-0.0.42/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/models/bayes.py` & `gmltools-0.0.42/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.42/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/models/model.py` & `gmltools-0.0.42/src/gmltools/models/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,160 +44,309 @@
     dt_default_params_reg
 )
 #import compute_sample_weight
 from sklearn.utils.class_weight import compute_sample_weight
 import joblib
 import os
 from openpyxl import load_workbook
+import time
+from typing import Union, List, Dict, Any, Optional
 
 
 
 #---------------------------------------------------------------------------
 
-def automatic_preprocessor(X_train,ordinal_cat_cols):
-    #Arguments assertion not needed because they are already checked in the model method of the classes that are the ones that call this function
-    """
-    This function performs a preprocessor for the data. It automatically detects the categorical and numeric variables and performs the following steps:
-        - Numeric variables: imputation by scaling. STANDARD SCALER
-        - Categorical variables: imputation by encoding. ONE HOT ENCODER
-        - Ordinal categorical variables: imputation by encoding. ORDINAL ENCODER
-
-    Parameters
-    ----------
-    X_train : pandas dataframe
-        Training data.
-    ordinal_cat_cols : list, optional
-        List of categorical variables that are ordinal.
-
-    Returns
-    -------
-    preprocessor : sklearn preprocessor
-        Preprocessor for the data. Used fo the pipelines for every model.
 
+class SelectSearchCV:
+
+    """
+    This class is used to perform a grid search, random search or bayesian search for a model. It is used in the model method of the classes that are the ones that call this function
     """
-    num_cols = X_train.select_dtypes(include=np.number).columns.values.tolist() #Detects the numeric variables
-    cat_cols = X_train.select_dtypes(include=['category']).columns.values.tolist() #detects the categorical variables
 
-    if ordinal_cat_cols is None:
-        cat_cols_onehot = cat_cols
-        ordinal_cat_cols = []
-    else:
-        for col in ordinal_cat_cols:
-            cat_cols.remove(col)
-        cat_cols_onehot = cat_cols
-
-    # Prepare the categorical variables by encoding the categories    
-    categorical_transformer_onehot = Pipeline(steps=[('onehot', OneHotEncoder(handle_unknown='ignore', drop='first'))])
-    categorical_transformer_ordinal = Pipeline(steps=[('ordinal', OrdinalEncoder())])
-    # Prepare the numeric variables by imputing by scaling
-    numeric_transformer = Pipeline(steps=[('scaler', StandardScaler())])
-
-    preprocessor = ColumnTransformer(transformers=[
-        ('num', numeric_transformer, num_cols), #numeric variables
-        ('cat_onehot', categorical_transformer_onehot, cat_cols_onehot), #categorical variables
-        ('cat_ordinal', categorical_transformer_ordinal, ordinal_cat_cols)]) #ordinal categorical variables
-    return preprocessor
+    def __init__(self, X_train, y_train, pipe, scoring, sample_weight=None,cv:int=10,n_jobs:int=-1):
+        """
+        Parameters
+        ----------
+        X_train : pandas dataframe
+            Training data.
+        y_train : pandas series
+            Training labels.
+        pipe : sklearn pipeline
+            Pipeline for the model.
+        scoring : str
+            Scoring metric for the model.
+        sample_weight : str, optional
+            If the sample weight is balanced. The default is None.
+        cv : int, optional
+            Number of folds for the cross validation. The default is 10.
+        n_jobs : int, optional
+            Number of jobs for the cross validation. The default is -1.
+        """
+        self.X_train = X_train
+        self.y_train = y_train
+        self.pipe = pipe
+        self.scoring = scoring
+        self.cv = cv
+        self.n_jobs = n_jobs
+        self._model=""
+        if sample_weight=='balanced' : #If the sample weight is balanced
+            self.weight = compute_sample_weight(
+            class_weight='balanced',
+            y=y_train)
+        else:
+            self.sample_weight = sample_weight
 
 
-def train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=None,cv=10,random_n_iter=10, X_prev=None, columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
+    #grid search
+    def _grid_search(self,grid_params:dict):
+        """
+        This method performs a grid search for a model.
 
-    #Arguments assertion not needed because they are already checked in the model method of the classes that are the ones that call this function
-    """
-    This function performs a grid search or a bayesian search for the hyperparameters of the model. It is used in the for the deployment 
-    of the model in ecah model method of the model classes.
+        Parameters
+        ----------
+        grid_params : dict
+            Dictionary with the parameters for the grid search.
 
-    Parameters
-    ----------
-    X_train : pandas
-        Training data.
-    y_train : pandas
-        Training labels.
-    bayes_pbounds : dict, optional
-        Dictionary with the bounds for the bayesian search. The default is None.
-    grid_params : dict, optional
-        Dictionary with the grid search parameters. The default is None.
-    random_params : dict, optional
-        Dictionary with the random search parameters. The default is None.
-    n_jobs : int, optional
-        Number of jobs for the grid search. The default is -1.
-    pipe : sklearn pipeline
-        Pipeline for the model.
-    scoring : str
-        Scoring metric for the grid search.
-    bayes_int_params : list, optional
-        List of parameters that are integers. The default is None.
-    bayes_n_iter : int, optional
-        Number of iterations for the bayesian search. The default is 10.
-    sample_weight : pandas, optional
-        Sample weights for the grid search. The default is None.
-    cv : int, optional
-        Number of folds for the grid search. The default is 10.
-        For time series use TimeSeriesSplit or BlockTimeSeriesSplit
-    random_n_iter : int, optional
-        Number of iterations for the random search. The default is 10.
-    """
-    #For Grid Search optimizartion,its done when the bayes_pbounds and random_params are None
-    if bayes_pbounds is None and random_params is None : 
+        Limitations
+        ----------
+        grid_params = {MODEL__parameter: [list of values],...}
+
+        """
         print("Grid search is running")
-    #apply the grid search
-        model_ = GridSearchCV(
-            estimator = pipe, 
+        self._model = GridSearchCV(
+            estimator = self.pipe, 
             param_grid = grid_params, 
-            cv = cv, 
-            n_jobs = n_jobs, 
-            scoring = scoring,
+            cv = self.cv, 
+            n_jobs = self.n_jobs, 
+            scoring = self.scoring,
             verbose=2
         )
-    #For Bayesian Search optimization, its done when the bayes_pbounds is not None and random_params is None
-    elif bayes_pbounds is not None and random_params is None: 
-        print("Bayesian search is running")
-        optimizer = ModelOptimizer(scoring=scoring,cv=cv)
-        params_bayes = optimizer.optimize_model(pbounds=bayes_pbounds, X_train_scale=X_train, 
-                                    y_train=y_train, model=pipe, 
-                                    int_params=bayes_int_params,n_iter=bayes_n_iter)
-        hyper_params = { (k):(int(np.round(v, 0)) if k in bayes_int_params else round(v, 2)) for k, v in params_bayes.items()}
-        model_ = pipe.set_params(**hyper_params)
-    #For Random Search optimization, its done when the bayes_pbounds is None and random_params is not None
-    else: 
+    #random search
+    def _random_search(self,random_params:dict,n_iter:int):
+        """
+        This method performs a random search for a model.
+
+        Parameters
+        ----------
+        random_params : dict
+            Dictionary with the parameters for the random search.
+        n_iter : int
+            Number of iterations for the random search.
+        
+        Limitations
+        ----------
+        random_params = {MODEL__parameter: [list of values],...}
+
+        """
         print("Random search is running")
-        model_ = RandomizedSearchCV(
-            estimator = pipe, 
+        self._model = RandomizedSearchCV(
+            estimator = self.pipe, 
             param_distributions = random_params, 
-            cv = cv, 
-            n_jobs = n_jobs, 
-            scoring = scoring,
+            cv = self.cv, 
+            n_jobs = self.n_jobs, 
+            scoring = self.scoring,
             verbose=2,
-            return_train_score=True,
-            n_iter=random_n_iter
+            n_iter = n_iter
         )
+    #bayes search
+    def _bayes_search(self,bayes_pbounds:dict,bayes_int_params:List[int],bayes_n_iter:int):
+        """
+        This method performs a bayesian search for a model.
 
-    if sample_weight is not None : #Sample weight are for XGBoost ando some other models but not fo all
-        if sample_weight=='balanced' : #If the sample weight is balanced
-            sample_weights = compute_sample_weight(
-            class_weight='balanced',
-            y=y_train)
+        Parameters
+        ----------
+        bayes_pbounds : dict
+            Dictionary with the parameters for the bayesian search.
+            bayes_pbounds = {MODEL__parameter: (min, max),...}
+        bayes_int_params : list
+            List of parameters that are integer.
+            bayes_int_params = [...,...]
+        """
+        print("Bayesian search is running")
+        optimizer = ModelOptimizer(scoring=self.scoring,cv=self.cv)
+        params_bayes = optimizer.optimize_model(pbounds=bayes_pbounds, X_train_scale=self.X_train, 
+                                    y_train=self.y_train, model=self.pipe, 
+                                    int_params=bayes_int_params,n_iter=bayes_n_iter)
+        hyper_params = { (k):(int(np.round(v, 0)) if k in bayes_int_params else round(v, 2)) for k, v in params_bayes.items()}
+        self._model = self.pipe.set_params(**hyper_params)
+
+    def select_automatic(self, grid_params:dict, random_params:dict, random_n_iter:int, bayes_pbounds:dict, bayes_int_params:List[str], bayes_n_iter:int):
+        """
+        This method selects the search method to be used
+
+        Parameters
+        ----------
+        grid_params : dict, optional
+            Dictionary with the parameters to be used in the grid search. The default is None.
+        random_params : dict, optional
+            Dictionary with the parameters to be used in the random search. The default is None.
+        random_n_iter : int, optional
+            Number of iterations to be used in the random search. The default is None.
+        bayes_pbounds : dict, optional
+            Dictionary with the parameters to be used in the bayesian search. The default is None.
+        bayes_int_params : list, optional
+            List of parameters to be used in the bayesian search. The default is None.
+        bayes_n_iter : int, optional
+            Number of iterations to be used in the bayesian search. The default is None.
+        
+        """
+        if grid_params is not None:
+            self.grid_search(grid_params)
+        elif random_params is not None:
+            self.random_search(random_params,random_n_iter)
+        elif bayes_pbounds is not None:
+            self.bayes_search(bayes_pbounds,bayes_int_params,bayes_n_iter)
+    
+
+    def fit(self, X_prev=None,columns_lags:List[int]=None, column_rolled_lags:List[int]=None,lags:List[int]=None,rolled_lags:List[int]=None, rolled_metrics:List[int]=None, column_rolled_lags_initial:List[int]=None):
+        """
+        This method fits the model when previously the search has been performed with the grid_search, random_search or bayes_search methods
+
+        Parameters
+        ----------
+        X_prev : pandas dataframe, optional
+            DataFrame con previsiones. The default is None.
+        columns_lags : list, optional
+            List of columns to lag. The default is None.
+        column_rolled_lags : list, optional
+            List of columns to lag. The default is None. 
+            The position column of the lags   
+        lags : list, optional
+            List of lags. The default is None.
+            Is used in autoregressive models
+        rolled_lags : list, optional
+            List of lags. The default is None.
+        rolled_metrics : list, optional
+            List of metrics. The default is None.
+            "mean","std","max","min"
+        column_rolled_lags_initial : list, optional
+            List of columns to lag. The default is None.
+            The initial lag where the rolling window starts/finish. The default is None.
+
+        """
+        if self.sample_weight is not None:
+            if self.pipe.steps[-1][0]=='XGB':
+                self._model.fit(self.X_train, self.y_train, XGB__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            elif self.pipe.steps[-1][0]=='LGBM':
+                self._model.fit(self.X_train, self.y_train, LGBM__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            elif self.pipe.steps[-1][0]=='RF':
+                self._model.fit(self.X_train, self.y_train, RF__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            elif self.pipe.steps[-1][0] == 'KNN':
+                self._model.fit(self.X_train, self.y_train, KNN__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            elif self.pipe.steps[-1][0] == 'LR':
+                self._model.fit(self.X_train, self.y_train, LR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            elif self.pipe.steps[-1][0] == 'MLP':
+                self._model.fit(self.X_train, self.y_train, MLP__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            elif self.pipe.steps[-1][0] == 'DT':
+                self._model.fit(self.X_train, self.y_train, DT__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
         else:
-            sample_weights=sample_weight
-        if pipe.steps[-1][0]=='XGB':
-            model_.fit(X_train, y_train, XGB__sample_weight=sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-        elif pipe.steps[-1][0]=='LGBM':
-            model_.fit(X_train, y_train, LGBM__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-        elif pipe.steps[-1][0]=='RF':
-            model_.fit(X_train, y_train, RF__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-        elif pipe.steps[-1][0] == 'KNN':
-            model_.fit(X_train, y_train, KNN__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-        elif pipe.steps[-1][0] == 'LR':
-            model_.fit(X_train, y_train, LR__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-        elif pipe.steps[-1][0] == 'MLP':
-            model_.fit(X_train, y_train, MLP__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-        elif pipe.steps[-1][0] == 'DT':
-            model_.fit(X_train, y_train, DT__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-    else :
-        model_.fit(X_train, y_train, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-    return model_
+            self._model.fit(self.X_train, self.y_train, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+
+        return self._model
+
+
+    
+    
+    
+# def train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=None,cv=10,random_n_iter=10, X_prev=None, columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
+
+#     #Arguments assertion not needed because they are already checked in the model method of the classes that are the ones that call this function
+#     """
+#     This function performs a grid search or a bayesian search for the hyperparameters of the model. It is used in the for the deployment 
+#     of the model in ecah model method of the model classes.
+
+#     Parameters
+#     ----------
+#     X_train : pandas
+#         Training data.
+#     y_train : pandas
+#         Training labels.
+#     bayes_pbounds : dict, optional
+#         Dictionary with the bounds for the bayesian search. The default is None.
+#     grid_params : dict, optional
+#         Dictionary with the grid search parameters. The default is None.
+#     random_params : dict, optional
+#         Dictionary with the random search parameters. The default is None.
+#     n_jobs : int, optional
+#         Number of jobs for the grid search. The default is -1.
+#     pipe : sklearn pipeline
+#         Pipeline for the model.
+#     scoring : str
+#         Scoring metric for the grid search.
+#     bayes_int_params : list, optional
+#         List of parameters that are integers. The default is None.
+#     bayes_n_iter : int, optional
+#         Number of iterations for the bayesian search. The default is 10.
+#     sample_weight : pandas, optional
+#         Sample weights for the grid search. The default is None.
+#     cv : int, optional
+#         Number of folds for the grid search. The default is 10.
+#         For time series use TimeSeriesSplit or BlockTimeSeriesSplit
+#     random_n_iter : int, optional
+#         Number of iterations for the random search. The default is 10.
+#     """
+#     #For Grid Search optimizartion,its done when the bayes_pbounds and random_params are None
+#     if bayes_pbounds is None and random_params is None : 
+#         print("Grid search is running")
+#     #apply the grid search
+#         model_ = GridSearchCV(
+#             estimator = pipe, 
+#             param_grid = grid_params, 
+#             cv = cv, 
+#             n_jobs = n_jobs, 
+#             scoring = scoring,
+#             verbose=2
+#         )
+#     #For Bayesian Search optimization, its done when the bayes_pbounds is not None and random_params is None
+#     elif bayes_pbounds is not None and random_params is None: 
+#         print("Bayesian search is running")
+#         optimizer = ModelOptimizer(scoring=scoring,cv=cv)
+#         params_bayes = optimizer.optimize_model(pbounds=bayes_pbounds, X_train_scale=X_train, 
+#                                     y_train=y_train, model=pipe, 
+#                                     int_params=bayes_int_params,n_iter=bayes_n_iter)
+#         hyper_params = { (k):(int(np.round(v, 0)) if k in bayes_int_params else round(v, 2)) for k, v in params_bayes.items()}
+#         model_ = pipe.set_params(**hyper_params)
+#     #For Random Search optimization, its done when the bayes_pbounds is None and random_params is not None
+#     else: 
+#         print("Random search is running")
+#         model_ = RandomizedSearchCV(
+#             estimator = pipe, 
+#             param_distributions = random_params, 
+#             cv = cv, 
+#             n_jobs = n_jobs, 
+#             scoring = scoring,
+#             verbose=2,
+#             return_train_score=True,
+#             n_iter=random_n_iter
+#         )
+
+#     if sample_weight is not None : #Sample weight are for XGBoost ando some other models but not fo all
+#         if sample_weight=='balanced' : #If the sample weight is balanced
+#             sample_weights = compute_sample_weight(
+#             class_weight='balanced',
+#             y=y_train)
+#         else:
+#             sample_weights=sample_weight
+#         if pipe.steps[-1][0]=='XGB':
+#             model_.fit(X_train, y_train, XGB__sample_weight=sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#         elif pipe.steps[-1][0]=='LGBM':
+#             model_.fit(X_train, y_train, LGBM__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#         elif pipe.steps[-1][0]=='RF':
+#             model_.fit(X_train, y_train, RF__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#         elif pipe.steps[-1][0] == 'KNN':
+#             model_.fit(X_train, y_train, KNN__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#         elif pipe.steps[-1][0] == 'LR':
+#             model_.fit(X_train, y_train, LR__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#         elif pipe.steps[-1][0] == 'MLP':
+#             model_.fit(X_train, y_train, MLP__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#         elif pipe.steps[-1][0] == 'DT':
+#             model_.fit(X_train, y_train, DT__sample_weight=sample_weights, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#     else :
+#         model_.fit(X_train, y_train, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+#     return model_
 
 
 class Classification:
     """
     This class contains all the classification models. Consideres relevant.
     Its up to suggestions for other models to be added.
     """
@@ -205,34 +354,35 @@
     RandomForest_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     XGBoost_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     LogisticRegression_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     DecisionTree_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     KNN_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     MLP_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
 
-    def __init__(self, model_name):
+    def __init__(self, model_name, X_train=None, y_train=None):
         self.model = None
         self.model_name = model_name
-
-    def RandomForest_Classifier(self, X_train, y_train, ordinal_cat_cols=None,
+        self.X_train = X_train
+        self.y_train = y_train
+    def RandomForest_Classifier(self, ordinal_cat_cols:List[str]=None,
                                 scoring='accuracy', class_weight=None,
-                                grid_params={'RFC__n_estimators': [100, 200],
+                                grid_params:dict={'RFC__n_estimators': [100, 200],
                                             'RFC__max_depth': [None, 10, 20],
                                             'RFC__min_samples_split': [2, 5],
                                             'RFC__max_features': ['sqrt', None]},
                                 cv=10,
-                                random_params=None,
-                                random_n_iter=10,
-                                bayes_pbounds=None,
-                                bayes_int_params=None, 
-                                bayes_n_iter=30,
+                                random_params:dict=None,
+                                random_n_iter:int=10,
+                                bayes_pbounds:dict=None,
+                                bayes_int_params:List[str]=None, 
+                                bayes_n_iter:int=30,
                                 criterion='gini',
                                 sample_weight=None,
-                                random_state=None,
-                                n_jobs=-1):
+                                random_state:int=None,
+                                n_jobs:int=-1):
         """
         This function performs a Random Forest classification model with grid search or bayesian optimization.
 
 
         Parameters
         ----------
         X_train : pandas dataframe
@@ -276,51 +426,55 @@
         model : sklearn model
             Trained model with grid seach
         """
         print(" INFO: Agurments params must start as 'RF__param'" + '\n' "INFO: Default params in Documentation for Random Forest are: ", rf_default_params_clf)
         print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}', f'criterion = {criterion}',
             f'bayes_n_iter = {bayes_n_iter}', f'class_weigth = {class_weight}', f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}',
             f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+        assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
         assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
         assert class_weight is None or class_weight is 'balanced' , "In case of balanced class weights, balanced must be 'balanced'"
         assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameters"
         assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameters"
         assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
         assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
         #RFC should be in every key of grid_param_grid
         if grid_params is not None and random_params is None and bayes_pbounds is None:
             assert all('RF__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'RF__'"
         elif random_params is not None:
             assert all('RF__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'RF__'"
         elif bayes_pbounds is not None:
             assert all('RF__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'RF__'"
             assert all('RF__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'RF__'"
-        # Inputs of the model. Change accordingly to perform variable selection
     
-        preprocessor = automatic_preprocessor(X_train, ordinal_cat_cols)
-        pipe = Pipeline([
-            ('preprocessor', preprocessor),
-            ('RF', RandomForestClassifier(
-                criterion = criterion,
-                bootstrap = True,
-                n_jobs = n_jobs,
-                random_state = random_state,
-                class_weight = class_weight))])
-
-        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        #Preprocess the data automatically
+        preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+        pipe = Pipeline(steps=[('Prep', preprocessor),
+                            ('RF', RandomForestRegressor(criterion=criterion,random_state=random_state,n_jobs=n_jobs,class_weight=class_weight))]) # Model always the last step
+        #Select Grid Search, Random Search or Bayesian Optimization
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        self.model=select_searchcv.fit()
+        
+        #generate a dictionary with all the parameters used in the model
+        self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        
+        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), "Class_Weights":str(class_weight), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                    'scoring':str(scoring), 'cv':str(cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight)}
         
 
         return self.model
     
-    def XGBoost_Classifier( self, X_train, y_train, ordinal_cat_cols=None,
+    def XGBoost_Classifier( self, ordinal_cat_cols:list=None,
                             scoring='accuracy', eval_metric='merror',
-                            objective='multi:softmax', grid_params={},
-                            cv=10, random_params=None, random_n_iter=10,
-                            bayes_pbounds=None,bayes_int_params=None, 
-                            bayes_n_iter=30, random_state=None,
+                            objective='multi:softmax', grid_params:dict={},
+                            cv=10, random_params:dict=None, random_n_iter:int=10,
+                            bayes_pbounds:dict=None,bayes_int_params:List[str]=None, 
+                            bayes_n_iter:int=30, random_state:int=None,
                             sample_weight=None, n_jobs=-1):  
         """
         This method performs a XGBoost classification model with grid search or bayesian optimization.
 
 
         Parameters
         ----------
@@ -369,14 +523,15 @@
             Trained model with grid seach or bayesian optimization
 
         """
         print(" INFO: Agurments params must start as 'XGB__param'" + '\n' "INFO: Default params for XGBoost in Documentation are: ", xgb_default_params_clf)
         print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}', f'eval_metric = {eval_metric}',f'objective = {objective}',
             f'bayes_n_iter = {bayes_n_iter}', f'sample_weigth = {sample_weight}', f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}',
             f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+        assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
         assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
         assert sample_weight is None or sample_weight is 'balanced' or isinstance(sample_weight, compute_sample_weight) , "In case of balanced class weights, balanced must be 'balanced'"
         assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameters"
         assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameters"
         assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
         assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
         #XGB__ is the prefix for every hyperparameter of this model
@@ -384,38 +539,45 @@
             assert all('XGB__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'XGB__'"
         elif random_params is not None:
             assert all('XGB__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'XGB__'"
         elif bayes_pbounds is not None:
             assert all('XGB__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'XGB__'"
             assert all('XGB__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'XGB__'"
 
-        preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
 
-        pipe = Pipeline([
-            ('preprocessor', preprocessor),
-            ('XGB', XGBClassifier(
+        preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+        pipe = Pipeline(steps=[('Prep', preprocessor),
+                            ('XGB', XGBClassifier(
                                 random_state=random_state,
                                 n_jobs=n_jobs, 
                                 verbosity=0,
                                 eval_metric=eval_metric,
-                                objective=objective))])
-                                
-        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+                                objective=objective))]) # Model always the last step
+        #Select Grid Search, Random Search or Bayesian Optimization
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        self.model=select_searchcv.fit()
+        
+        #generate a dictionary with all the parameters used in the model
+        self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        
+        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
+                                    'scoring':str(scoring), 'cv':str(cv), 'eval_metric':str(eval_metric), 'sample_weight':str(sample_weight), "objective":str(objective)}
         return self.model
     
-    def LogisticRegression_Classifier(self, X_train, y_train,  
-                                      ordinal_cat_cols=None, scoring='accuracy',
+    def LogisticRegression_Classifier(self,  ordinal_cat_cols:List[str]=None, scoring='accuracy',
                                     grid_params = {'LR__C': [0.1, 1, 10],
                                     'LR__penalty': ['l1', 'l2', 'elasticnet'],
                                     'LR__multi_class': ['ovr', 'multinomial'],   
                                     'LR__solver': ['newton-cg', 'lbfgs', 'liblinear', 'sag', 'saga']},
-                                    cv=10, random_params=None, random_n_iter=10,
-                                    bayes_pbounds=None, bayes_int_params=None, 
-                                    bayes_n_iter=30, random_state=None, class_weight=None, sample_weight=None,
-                                    n_jobs=-1 , tol=0.0001, max_iter=1000):
+                                    cv=10, random_params:dict=None, random_n_iter:int=10,
+                                    bayes_pbounds:dict=None, bayes_int_params:List[str]=None, 
+                                    bayes_n_iter:int=30, random_state:int=None, class_weight=None, sample_weight=None,
+                                    n_jobs:int=-1 , tol:float=0.0001, max_iter:int=1000):
         """
         This method performs a Logistic Regression classification model with grid search or bayesian optimization.
 
         Parameters
         ----------
         X_train : pandas dataframe
             Training set.
@@ -474,50 +636,58 @@
 
         """
 
         print(" INFO: Agurments params must start as 'LR__param'" + '\n' "INFO: Default params in Documentaction for Logistic Regression are: ", lr_default_params_clf)
         print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}', f'bayes_n_iter = {bayes_n_iter}',
             f'class_weigth = {class_weight}', f'max_iter = {max_iter}' f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}',
             f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+        assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
         assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
         assert class_weight is None or class_weight is 'balanced' , "In case of balanced class weights, balanced must be 'balanced'"
         assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter values"
         assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter values"
         assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
         assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
         #LR__ is the prefix for every hyperparameter in this model
         if grid_params is not None and random_params is None and bayes_pbounds is None:
             assert all('LR__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'LR__'"
         elif random_params is not None:
             assert all('LR__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'LR__'"
         elif bayes_pbounds is not None:
             assert all('LR__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LR__'"
             assert all('LR__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LR__'"
-
-        preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
-
-        pipe = Pipeline([
-            ('preprocessor', preprocessor),
-            ('LR', LogisticRegression(
+        #Preprocessing
+        preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+        pipe = Pipeline(steps=[('Prep', preprocessor),
+                            ('LR', LogisticRegression(
                                     max_iter=max_iter,
                                     tol=tol, #default 1e-4
                                     class_weight=class_weight, #is used to handle the imbalance dataset
                                     random_state=random_state,
                                     n_jobs=n_jobs, 
                                     verbose=0,
                                     warm_start=False,
                                     fit_intercept=True,
                                     intercept_scaling=1,
-                                    dual=False))])
-
-        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,cv=cv,random_n_iter=random_n_iter,sample_weight=sample_weight)
-        
+                                    dual=False))]) # Model always the last step
+        #Select Grid Search, Random Search or Bayesian Optimization
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        self.model=select_searchcv.fit()
+        
+        #generate a dictionary with all the parameters used in the model
+        self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        
+        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Class Weight":str(class_weight), 'random_state':str(random_state),
+                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
+                                    'scoring':str(scoring), 'cv':str(cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter)}
         return self.model
+        
     
-    def MLP_Classifier(self,X_train,y_train,ordinal_cat_cols=None, scoring='accuracy',
+    def MLP_Classifier(self,ordinal_cat_cols=None, scoring='accuracy',
                        grid_params={'MLP__alpha': [1e-9,1e-7,1e-5,0.001,0.01],
                         'MLP__hidden_layer_sizes':[(5,),(10,),(15,),(20,),(25,)]},
                         cv=10, random_params=None, random_n_iter=10,
                         bayes_pbounds=None, bayes_int_params=None, bayes_n_iter=30, 
                         random_state=None, n_jobs=-1, solver='lbfgs',
                         activation='logistic', tol=1e-4, max_iter=450, early_stopping=False,
                        learning_rate='constant',learning_rate_init=0.001,verbose=True, sample_weight=None):
@@ -600,14 +770,15 @@
         """
 
         print(" INFO: Agurments params must start as 'MLP__param'" + '\n' "INFO: Default params in Documentation for MultiLayer Perceptron are: ", mlp_default_params_clf)
         print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}', f'solver = {solver}',f'activation = {activation}',
         f'bayes_n_iter = {bayes_n_iter}', f'tol = {tol}', f'max_iter = {max_iter}' , f'learning_rate = {learning_rate}', f'learning_rate_init = {learning_rate_init}',
         f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}',
         f'random_state = {random_state}', f'n_jobs = {n_jobs}', f'early_stopping = {early_stopping}', f'verbose = {verbose}')
+        assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
         assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
         assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_params must be a dictionary of parameter values"
         assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter values"
         assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
         assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
         assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
         #MLP__ is the prefix for every hyperparameter in MLPClassifier
@@ -615,35 +786,44 @@
             assert all('MLP__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'MLP__'"
         elif random_params is not None:
             assert all('MLP__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'MLP__'"
         elif bayes_pbounds is not None:
             assert all('MLP__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'MLP__'"
             assert all('MLP__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'MLP__'"
 
-        preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
-        pipe = Pipeline(steps=[('Prep', preprocessor), 
+        preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+        pipe = Pipeline(steps=[('Prep', preprocessor),
                             ('MLP', MLPClassifier(solver=solver, # Update function
                                                     activation=activation, # Logistic sigmoid activation function
                                                     max_iter=max_iter, # Maximum number of iterations
                                                     tol=tol, # Tolerance for the optimization
                                                     random_state=random_state,
                                                     verbose = verbose,
                                                     early_stopping=early_stopping,
                                                     learning_rate=learning_rate,
                                                     learning_rate_init=learning_rate_init
-                                                    ))]) # For replication
-
-
-        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+                                                    ))]) # Model always the last step
+        #Select Grid Search, Random Search or Bayesian Optimization
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        self.model=select_searchcv.fit()
+        
+        #generate a dictionary with all the parameters used in the model
+        self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        
+        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Early Stopping":str(early_stopping), 'random_state':str(random_state),
+                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape),
+                                    'scoring':str(scoring), 'cv':str(cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter), "Learning Rate":str(learning_rate), "Learning Rate Init":str(learning_rate_init)}
+        
         return self.model
         
 
 
     #do the same for knn_classifier
-    def KNN_Classifier(self,X_train,y_train,ordinal_cat_cols=None, scoring='accuracy',
+    def KNN_Classifier(self,ordinal_cat_cols=None, scoring='accuracy',
                         grid_params={'KNN__n_neighbors': [3,10,25,60]},
                         cv=10, random_params=None, random_n_iter=10,  bayes_pbounds=None,
                         bayes_int_params=None, bayes_n_iter=30, sample_weight=None,
                         random_state=None, n_jobs=-1):
           
         """
         This method performs a K-Nearest Neighbors classification model with grid search or bayesian optimization.
@@ -702,42 +882,52 @@
             Trained model.
 
         """
 
         print(" INFO: Agurments params must start as 'KNN__param'" + '\n' "INFO: Default params in Documentation for Random Forest are: ", knn_default_params_clf)
         print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}', f'bayes_n_iter = {bayes_n_iter}',
                f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+        assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
         assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
         assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter values"
         assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter values"
         assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
         assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
         assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
         #KNN_ is the prefix for every hyperparameter in the KNN model
         if grid_params is not None and random_params is None and bayes_pbounds is None:
             assert all('KNN__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'KNN__'"
         elif random_params is not None:
             assert all('KNN__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'KNN__'"
         elif bayes_pbounds is not None:
             assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
             assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
-
-        preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
-        pipe = Pipeline(steps=[('Prep', preprocessor),
-                            ('KNN', KNeighborsClassifier(n_jobs=n_jobs, random_state=random_state))])
         
-        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+        pipe = Pipeline(steps=[('Prep', preprocessor),
+                            ('KNN', KNeighborsClassifier(n_jobs=n_jobs, random_state=random_state))]) # Model always the last step
+        #Select Grid Search, Random Search or Bayesian Optimization
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        self.model=select_searchcv.fit()
+        
+        #generate a dictionary with all the parameters used in the model
+        self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        
+        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
+                                    'scoring':str(scoring), 'cv':str(cv),  'sample_weight':str(sample_weight)}
 
         return self.model
 
 
     
 
     #do the same for a decision tree
-    def DecisionTree_Classifier(self,X_train,y_train, ordinal_cat_cols=None, scoring='accuracy',
+    def DecisionTree_Classifier(self, ordinal_cat_cols=None, scoring='accuracy',
                             grid_params={'DT__max_depth': [3,5,7,10],
                                 'DT__min_samples_split': [2,3,4],
                                 'DT__min_samples_leaf': [4,5,6],
                                 'DT__max_features': ['auto','sqrt','log2',None]},
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None, 
                             bayes_int_params=None, bayes_n_iter=30, class_weight=None, sample_weight=None, random_state=None, n_jobs=-1):
             
@@ -792,14 +982,15 @@
         
         """
 
         print(" INFO: Agurments params must start as 'DT__param'" + '\n' "INFO: Default params in Documentation for Decision Tree are: ", dt_default_params_clf)
         print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
         f'bayes_n_iter = {bayes_n_iter}', f'class_weigth = {class_weight}', f'bayes_pbounds = {bayes_pbounds}', 
         f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+        assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
         assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
         assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter values"
         assert random_params is None or isinstance(random_params, dict), "In case of random search, random_param_grid must be a dictionary of parameter values"
         assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
         assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
         assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
         #DT__ is the prefix for every hyperparameter in the Decision Tree model
@@ -807,97 +998,185 @@
             assert all('DT__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'DT__'"
         elif random_params is not None:
             assert all('DT__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'DT__'"
         elif bayes_pbounds is not None:
             assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
             assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
 
-        preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
+        preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
         pipe = Pipeline(steps=[('Prep', preprocessor),
-                            ('DT', DecisionTreeClassifier(random_state=random_state,class_weight=class_weight))])
-        
-        self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params,n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+                            ('DT', DecisionTreeClassifier(random_state=random_state,class_weight=class_weight))]) # Model always the last step
+        #Select Grid Search, Random Search or Bayesian Optimization
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        self.model=select_searchcv.fit()
+        
+        #generate a dictionary with all the parameters used in the model
+        self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+        
+        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Class Weight": class_weight, 'random_state':str(random_state),
+                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape),
+                                    'scoring':str(scoring), 'cv':str(cv),  'sample_weight':str(sample_weight)}
 
         return self.model
     #save model
-    def save(self):
+    def save(self, return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
         Parameters
         ----------
         model_name : str
             Name of the model.
             The model is stored in the models folder. with the model name provided
 
         Returns
         -------
         None.
 
         """
-        assert self._model is not None , "Model not trained yet"
+        assert self.model is not None , "Model not trained yet"
         #create folder if not exists where the model will be saved
         path = f'./models/{self.model_name}'
         if not os.path.exists(path):
             os.makedirs(path)
 
-        joblib.dump(self._model, os.path.join(path, self.model_name+'.joblib'))
+        joblib.dump(self.model, os.path.join(path, self.model_name+'.joblib'))
         #save cv results if exists grid search or random search
-        if hasattr(self._model, 'cv_results_'):
-            df = pd.DataFrame(self._model.cv_results_)
+        if hasattr(self.model, 'cv_results_'):
+            df = pd.DataFrame(self.model.cv_results_)
             df.sort_values('rank_test_score', inplace=True)
             df.to_excel(os.path.join(path, self.model_name+'_cv_results.xlsx'), index=False)
-    #load model
+
+            #save the best register of the cv_results in a second sheet of excel file called summary_models.xlsx
+            df_best = pd.DataFrame(df.iloc[0]).T
+            df_best["Search conditions"]=str(self._overall_dict_params)
+            df_best['model_name'] = self.model_name
+            #set model_name the firts column and Search conditions the second column
+            cols = df_best.columns.tolist()
+            cols = cols[-1:] + cols[:-1]
+            df_best = df_best[cols]
+
+            # save in the second sheet
+            file_path = './models/summary_models.xlsx'
+            if os.path.isfile(file_path):
+                df_summary = pd.read_excel(file_path, sheet_name='Sheet2')
+                df_summary = pd.concat([df_summary, df_best], axis=0, ignore_index=True)
+                df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
+            else:
+                df_best.to_excel(file_path, index=False, sheet_name='Sheet2')
+            if return_best_metrics:
+                return df_best
+
     def load(self):
 
         """
         Loads a model from a file.
 
         Parameters
         ----------
         model_name : str
             Name of the model.
-            The model is stored in the models folder. with the model name provided
+            The model is stored in the models folder. with the model name provided.
+            To load a model, the model must be saved before. And when instantiating the class, 
+            its not mandatory to pass the X_train and y_train arguments.
 
         Returns
         -------
         None.
 
         """
         assert self.model_name+'.joblib' in os.listdir('./models'), "Model not found"
         path = f'./models/{self.model_name}/{self.model_name}'+'.joblib'
         self.model = joblib.load(path)
         return self.model
     
+    def _automatic_preprocessor(self, X_train, ordinal_cat_cols:List[str]=None):
+        #Arguments assertion not needed because they are already checked in the model method of the classes that are the ones that call this function
+        """
+        This function performs a preprocessor for the data. It automatically detects the categorical and numeric variables and performs the following steps:
+            - Numeric variables: imputation by scaling. STANDARD SCALER
+            - Categorical variables: imputation by encoding. ONE HOT ENCODER
+            - Ordinal categorical variables: imputation by encoding. ORDINAL ENCODER
+
+        Parameters
+        ----------
+        X_train : pandas dataframe
+            Training data.
+        ordinal_cat_cols : list, optional
+            List of categorical variables that are ordinal.
+
+        Returns
+        -------
+        preprocessor : sklearn preprocessor
+            Preprocessor for the data. Used fo the pipelines for every model.
+
+        """
+        num_cols = X_train.select_dtypes(include=np.number).columns.values.tolist() #Detects the numeric variables
+        cat_cols = X_train.select_dtypes(include=['category']).columns.values.tolist() #detects the categorical variables
+
+        if ordinal_cat_cols is None:
+            cat_cols_onehot = cat_cols
+            ordinal_cat_cols = []
+        else:
+            for col in ordinal_cat_cols:
+                cat_cols.remove(col)
+            cat_cols_onehot = cat_cols
+
+        # Prepare the categorical variables by encoding the categories    
+        categorical_transformer_onehot = Pipeline(steps=[('onehot', OneHotEncoder(handle_unknown='ignore', drop='first'))])
+        categorical_transformer_ordinal = Pipeline(steps=[('ordinal', OrdinalEncoder())])
+        # Prepare the numeric variables by imputing by scaling
+        numeric_transformer = Pipeline(steps=[('scaler', StandardScaler())])
+
+        preprocessor = ColumnTransformer(transformers=[
+            ('num', numeric_transformer, num_cols), #numeric variables
+            ('cat_onehot', categorical_transformer_onehot, cat_cols_onehot), #categorical variables
+            ('cat_ordinal', categorical_transformer_ordinal, ordinal_cat_cols)]) #ordinal categorical variables
+        
+        return preprocessor
+    
+    @staticmethod
+    def _not_none_search(*args):
+        """
+        This function returns a list of the arguments that are not None. Is used to store the not none parameters of the seleted search  of the model in the dictionary self._overall_dict
+        """
+        search_list=['grid_params', 'random_params', 'random_n_iter', 'bayes_pbounds', 'bayes_int_params', 'bayes_n_iter']
+        return [(search_list[i],value_var) for i, value_var in enumerate(args) if value_var is not None]
+        #add the variable name to the value
+    
 #-------------------------------------------------------------------------------------------------------------------REGRESSION-------------------------------------------------------------------------------------------------------------#
 class Regression:
     """
     This class contains all regression models that are considered relevant.
     Its up to add more models in the future thta could be suggested by the user.
     """
 
     RandomForest_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     XGBoost_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     LogisticRegression_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     DecisionTree_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     KNN_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     MLP_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
 
-    def __init__(self,model_name:str):
+    def __init__(self,model_name:str, X_train=None, y_train=None, X_prev=None):
         self.model = None
         self.model_name = model_name
+        self.X_train = X_train
+        self.y_train = y_train
+        self.X_prev = X_prev
 
-    def RandomForest_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error', criterion="friedman_mse",
+    def RandomForest_Regressor(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error', criterion="friedman_mse",
                             grid_params={'RF__n_estimators': [100, 200, 300, 400, 500],
                                 'RF__max_depth': [3,5,7,10],
                                 'RF__min_samples_split': [2,3,4],
                                 'RF__min_samples_leaf': [4,5,6],
                                 'RF__max_features': ['auto','sqrt','log2',None]}, 
                             cv=10, random_params=None, random_n_iter = 10, bayes_pbounds=None, 
-                            bayes_int_params=None, bayes_n_iter = 30, sample_weight=None, random_state=None, n_jobs=-1,X_prev=None,
+                            bayes_int_params=None, bayes_n_iter = 30, sample_weight=None, random_state=None, n_jobs=-1, 
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a Random Forest regression model with grid search or bayesian optimization.
     
             Parameters
             ----------
@@ -949,14 +1228,15 @@
             """
             
 
             print(" INFO: Agurments params must start as 'RF__param'" + '\n' "INFO: Default params in Documentation for Random Forest are: ", rf_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
             f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}', 
             f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
             assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
             assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameters"
             assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameters"
             assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
             assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
             assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
             #RF__ is the prefix for every hyperparameter in the model
@@ -964,32 +1244,42 @@
                 assert all('RF__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'RF__'"
             elif random_params is not None:
                 assert all('RF__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'RF__'"
             elif bayes_pbounds is not None:
                 assert all('RF__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'RF__'"
                 assert all('RF__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'RF__'"
 
-            preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
+            #Preprocess the data automatically
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
-                                ('RF', RandomForestRegressor(criterion=criterion,random_state=random_state,n_jobs=n_jobs))])
-            
-            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter, X_prev=X_prev
-                                              ,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+                                ('RF', RandomForestRegressor(criterion=criterion,random_state=random_state,n_jobs=n_jobs))]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+            
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
 
             return self.model
     
-    def XGB_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def XGB_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'XGB__n_estimators': [100, 200, 300, 400, 500],
                                 'XGB__max_depth': [3,5,7,10],
                                 'XGB__learning_rate': [0.01,0.05,0.1,0.15,0.2],
                                 'XGB__min_child_weight': [1,3,5,7],
                                 'XGB__gamma': [0.0,0.1,0.2,0.3,0.4],
                                 'XGB__colsample_bytree': [0.3,0.4,0.5,0.7]}, 
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
-                            bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1, X_prev=None,
+                            bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a XGBoost regression model with grid search or bayesian optimization.
     
             Parameters
             ----------
@@ -1040,14 +1330,15 @@
             
             """
 
             print(" INFO: Agurments params must start as 'XGB__param'" + '\n' "INFO: Default params in Documentation for XGBoost are: ", xgb_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
             f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
             f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
             assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
             assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary"
             assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary"
             assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
             assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
             assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
             # XGB__ is the prefix for every hyperparameters
@@ -1055,29 +1346,41 @@
                 assert all('XGB__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'XGB__'"
             elif random_params is not None:
                 assert all('XGB__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'XGB__'"
             elif bayes_pbounds is not None:
                 assert all('XGB__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'XGB__'"
                 assert all('XGB__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'XGB__'"
             
-            preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
+
+            #Preprocess the data automatically
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
-                                ('XGB', XGBRegressor(random_state=random_state,n_jobs=n_jobs))])
-            
-            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter, X_prev=X_prev,
-                                              columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+                                ('XGB', XGBRegressor(random_state=random_state,n_jobs=n_jobs))]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+            
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
 
             return self.model
+
     
-    def Linear_Regression(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def Linear_Regression(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'LR__fit_intercept': [True, False],
                                 'LR__normalize': [True, False],
                                 'LR__copy_X': [True, False]}, 
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None,
-                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1, X_prev=None,
+                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a Linear Regression model with grid search or bayesian optimization.
     
             Parameters
             ----------
@@ -1128,14 +1431,15 @@
             
             """
 
             print(" INFO: Agurments params must start as 'LR__param'" + '\n' "INFO: Default params in Documentation for Linear Regression are: ", lr_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
             f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
             f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
             assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
             assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameters"
             assert random_params is None or isinstance(random_params, dict), "In case of random search, random_param_grid must be a dictionary of parameters"
             assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
             assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
             assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
             #LR is the prefix for every hyperparameter of the Linear Regression
@@ -1143,31 +1447,40 @@
                 assert all('LR__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'LR__'"
             elif random_params is not None:
                 assert all('LR__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'LR__'"
             elif bayes_pbounds is not None:
                 assert all('LR__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LR__'"
                 assert all('LR__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LR__'"
             
-            preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
-                                ('LR', LinearRegression())])
-            
-            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight, cv=cv, random_n_iter=random_n_iter,
-                                              X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
-
-            self.model
+                                ('LR', LinearRegression())]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+            
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
     
-    def KNN_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+            return self.model
+    
+    def KNN_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'KNN__n_neighbors': [3,5,7,9,11,13,15,17,19,21,23,25,27,29,31,33,35,37,39,41,43,45,47,49,51,53,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,87,89,91,93,95,97,99],
                                 'KNN__weights': ['uniform', 'distance'],
                                 'KNN__algorithm': ['auto', 'ball_tree', 'kd_tree', 'brute'],
                                 'KNN__leaf_size': [10,20,30,40,50,60,70,80,90,100],
                                 'KNN__p': [1,2]}, 
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
-                            bayes_n_iter=30, sample_weight=None ,random_state=None, n_jobs=-1, X_prev=None,
+                            bayes_n_iter=30, sample_weight=None ,random_state=None, n_jobs=-1, 
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a KNN Regressor model with grid search or bayesian optimization.
     
             Parameters
             ----------
@@ -1218,14 +1531,15 @@
             
             """
 
             print(" INFO: Agurments params must start as 'KNN__param'" + '\n' "INFO: Default params in Documentation for KNN Regressor are: ", knn_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
             f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
             f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
             assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
             assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter bounds"
             assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
             assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter bounds"
             assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
             assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
             #KNN_ is the prefix for every hyperparameter in KNN
@@ -1233,31 +1547,42 @@
                 assert all('KNN__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'KNN__'"
             elif random_params is not None:
                 assert all('KNN__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'KNN__'"
             elif bayes_pbounds is not None:
                 assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
                 assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
 
-            preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
-                                ('KNN', KNeighborsRegressor())])
-            
-            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight, cv=cv, random_n_iter=random_n_iter,
-                                              X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+                                ('KNN', KNeighborsRegressor())]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+            
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+    
+            return self.model
+
 
-            self.model
     
-    def DecisionTree_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def DecisionTree_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'DT__criterion': ["squared_error", "friedman_mse", "absolute_error", "poisson"],
                                 'DT__max_depth': [None,2,3,4,5],
                                 'DT__min_samples_split': [2,3,4,],
                                 'DT__max_features': ['auto', 'sqrt', 'log2'],
                                 'DT__min_impurity_decrease': [0.0,0.1,0.2]}, 
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None,
-                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1, X_prev=None,
+                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a Decision Tree Regressor model with grid search or bayesian optimization.
     
             Parameters
             ----------
@@ -1308,14 +1633,15 @@
             
             """
 
             print(" INFO: Agurments params must start as 'DT__param'" + '\n' "INFO: Default params in Documentation for Decision Tree Regressor are: ", dt_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
             f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
             f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
             assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
             assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter bounds"
             assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
             assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter bounds"
             assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
             assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
             # DT__ is the prefix for every hyperparameter in the Decision Tree Regressor
@@ -1323,31 +1649,40 @@
                 assert all('DT__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'DT__'"
             elif random_params is not None:
                 assert all('DT__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'DT__'"
             elif bayes_pbounds is not None:
                 assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
                 assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
             
-            preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
-                                ('DT', DecisionTreeRegressor(random_state=random_state))])
-            
-            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv, random_n_iter=random_n_iter,
-                                              X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+                                ('DT', DecisionTreeRegressor(random_state=random_state))]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+            
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
 
-            self.model
+            return self.model
     
-    def MLP_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def MLP_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'MLP__hidden_layer_sizes': [(3,),(5,)],
                                 'MLP__activation': ['identity', 'logistic', 'tanh', 'relu'],
                                 'MLP__solver': ['lbfgs', 'sgd', 'adam'],
                                 'MLP__alpha': [0.0001,0.001,0.01,0.1,1,10,100],
                                 'MLP__max_iter': [200]},
                             cv=10, random_params=None, random_n_iter=10,bayes_pbounds=None,
-                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None,random_state=None, n_jobs=-1, X_prev=None,
+                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None,random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             """
             Trains a MLP Regressor model.
 
             Parameters
             ----------
             X_train : pandas dataframe
@@ -1402,14 +1737,15 @@
             """
             
 
             print(" INFO: Agurments params must start as 'MLP__param'" + '\n' "INFO: Default params in Documentation for MultiLayer Perceptron are: ", mlp_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}', f'bayes_n_iter = {bayes_n_iter}' ,
             f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}',
             f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
             assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
             assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
             assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter bounds"
             assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
             assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter bounds"
             assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
             assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
@@ -1418,26 +1754,33 @@
                 assert all('MLP__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'MLP__'"
             elif random_params is not None:
                 assert all('MLP__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'MLP__'"
             elif bayes_pbounds is not None:
                 assert all('MLP__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'MLP__'"
                 assert all('MLP__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'MLP__'"
 
-            
-            preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
-            pipe = Pipeline(steps=[('Prep', preprocessor), 
-                                      ('MLP', MLPRegressor(random_state=random_state))])
-            
-
-            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv, random_n_iter=random_n_iter,
-                                              X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            pipe = Pipeline(steps=[('Prep', preprocessor),
+                                ('MLP', MLPRegressor(random_state=random_state))]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+            
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             return self.model
     
 
-    def save(self):
+    def save(self,return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
         Parameters
         ----------
         model_name : str
             Name of the model.
@@ -1459,50 +1802,118 @@
         if hasattr(self.model, 'cv_results_'):
             df = pd.DataFrame(self.model.cv_results_)
             df.sort_values('rank_test_score', inplace=True)
             df.to_excel(os.path.join(path, self.model_name+'_cv_results.xlsx'), index=False)
 
             #save the best register of the cv_results in a second sheet of excel file called summary_models.xlsx
             df_best = pd.DataFrame(df.iloc[0]).T
+            df_best["Search conditions"]=str(self._overall_dict_params)
             df_best['model_name'] = self.model_name
-            #set the model_name as the firts column
-            cols = df_summary.columns.tolist()
+            #set model_name the firts column and Search conditions the second column
+            cols = df_best.columns.tolist()
             cols = cols[-1:] + cols[:-1]
             df_best = df_best[cols]
 
             # save in the second sheet
             file_path = './models/summary_models.xlsx'
             if os.path.exists(file_path):
                 df_summary = pd.read_excel(file_path, sheet_name='Sheet2')
                 df_summary = pd.concat([df_summary, df_best], axis=0,ignore_index=True)
                 df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
             else:
                 df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
-
+            if return_best_metrics:
+                return df_best
 
     def load(self):
 
         """
         Loads a model from a file.
 
         Parameters
         ----------
         model_name : str
             Name of the model.
             The model is stored in the models folder. with the model name provided
+            To load a model, the model must be saved before. And when instantiating the class, 
+            its not mandatory to pass the X_train and y_train arguments.
 
         Returns
         -------
         None.
 
         """
         assert self.model_name+'.joblib' in os.listdir('./models'), "Model not found"
         path = f'./models/{self.model_name}/{self.model_name}'+'.joblib'
         self.model = joblib.load(path)
         return self.model
+    
+    def _automatic_preprocessor(self, X_train, ordinal_cat_cols:List[str]=None):
+        #Arguments assertion not needed because they are already checked in the model method of the classes that are the ones that call this function
+        """
+        This function performs a preprocessor for the data. It automatically detects the categorical and numeric variables and performs the following steps:
+            - Numeric variables: imputation by scaling. STANDARD SCALER
+            - Categorical variables: imputation by encoding. ONE HOT ENCODER
+            - Ordinal categorical variables: imputation by encoding. ORDINAL ENCODER
+
+        Parameters
+        ----------
+        X_train : pandas dataframe
+            Training data.
+        ordinal_cat_cols : list, optional
+            List of categorical variables that are ordinal.
+
+        Returns
+        -------
+        preprocessor : sklearn preprocessor
+            Preprocessor for the data. Used fo the pipelines for every model.
+
+        """
+        num_cols = X_train.select_dtypes(include=np.number).columns.values.tolist() #Detects the numeric variables
+        cat_cols = X_train.select_dtypes(include=['category']).columns.values.tolist() #detects the categorical variables
+
+        if ordinal_cat_cols is None:
+            cat_cols_onehot = cat_cols
+            ordinal_cat_cols = []
+        else:
+            for col in ordinal_cat_cols:
+                cat_cols.remove(col)
+            cat_cols_onehot = cat_cols
+
+        # Prepare the categorical variables by encoding the categories    
+        categorical_transformer_onehot = Pipeline(steps=[('onehot', OneHotEncoder(handle_unknown='ignore', drop='first'))])
+        categorical_transformer_ordinal = Pipeline(steps=[('ordinal', OrdinalEncoder())])
+        # Prepare the numeric variables by imputing by scaling
+        numeric_transformer = Pipeline(steps=[('scaler', StandardScaler())])
+
+        preprocessor = ColumnTransformer(transformers=[
+            ('num', numeric_transformer, num_cols), #numeric variables
+            ('cat_onehot', categorical_transformer_onehot, cat_cols_onehot), #categorical variables
+            ('cat_ordinal', categorical_transformer_ordinal, ordinal_cat_cols)]) #ordinal categorical variables
+        
+        return preprocessor
+    
+    @staticmethod
+    def _not_none_search(*args):
+        """
+        This function returns a list of the arguments that are not None. Is used to store the not none parameters of the seleted search  of the model in the dictionary self._overall_dict
+        """
+        search_list=['grid_params', 'random_params', 'random_n_iter', 'bayes_pbounds', 'bayes_int_params', 'bayes_n_iter']
+        return [(search_list[i],value_var) for i, value_var in enumerate(args) if value_var is not None]
+        #add the variable name to the value
+    @staticmethod
+    def _not_none_recursive(*args):
+        """
+        This function returns a list of the arguments that are not None. Is used to store the not none parameters of the  the recursive parameters of the model in the dictionary self._overall_dict
+        """
+        recursive_list=['columns_lags', 'column_rolled_lags','lags,rolled_lags', 'rolled_metrics', 'column_rolled_lags_initial']
+        return [(recursive_list[i],value_var) for i, value_var in enumerate(args) if value_var is not None]
+            
+        
+
```

### Comparing `gmltools-0.0.41/src/gmltools/models/models_info.py` & `gmltools-0.0.42/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.42/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.42/src/gmltools/models_analysis/classification_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1423,14 +1423,16 @@
         metrics_dict["CV"] = self.model.cv
         try:
             metrics_dict["best_params"] = str(self.model.best_params_)
             if "GridSearchCV" in str(self.model.__getattribute__):
                 metrics_dict["Search"] = 'Grid' + str(self.model.param_grid)
             elif "RandomizedSearchCV" in str(self.model.__getattribute__):
                 metrics_dict["Search"] = 'Random' + str(self.model.param_distributions)
+            else:
+                metrics_dict["Search"] = None
 
         except:
             metrics_dict["best_params"] = None
             metrics_dict["Search"] = None
         
         # Return the metrics as a DataFrame
         summary=pd.DataFrame(metrics_dict,index=[0])
@@ -1439,19 +1441,20 @@
         if save:
             if not os.path.exists('./models'):
                 os.makedirs('./models')
 
             if not os.path.isfile('./models/summary_models.xlsx'):
                 df=pd.DataFrame(columns=summary.columns)
                 #save the summary data to the excel
-                df.to_excel('./models/summary_models.xlsx',index=False)
+                df.to_excel('./models/summary_models.xlsx',index=False,sheet_name='Sheet1')
             else:
-                df=pd.read_excel('./models/summary_models.xlsx')
+                df=pd.read_excel('./models/summary_models.xlsx',sheet_name='Sheet1')
                 #concat the summary data to the excel
                 df=pd.concat([df,summary],axis=0,ignore_index=True)
+                df.to_excel('./models/summary_models.xlsx',index=False,sheet_name='Sheet1')
     
         return  self.metrics_summary
```

### Comparing `gmltools-0.0.41/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.42/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.42/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.42/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.42/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.41/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.42/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.41
+Version: 0.0.42
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.41/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.42/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

