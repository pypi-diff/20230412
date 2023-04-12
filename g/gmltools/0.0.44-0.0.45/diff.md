# Comparing `tmp/gmltools-0.0.44.tar.gz` & `tmp/gmltools-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.44.tar", last modified: Wed Apr 12 10:56:44 2023, max compression
+gzip compressed data, was "gmltools-0.0.45.tar", last modified: Wed Apr 12 11:03:49 2023, max compression
```

## Comparing `gmltools-0.0.44.tar` & `gmltools-0.0.45.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.377689 gmltools-0.0.44/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.44/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.44/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-12 10:56:44.377689 gmltools-0.0.44/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.44/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.311135 gmltools-0.0.44/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.44/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.44/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.44/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.44/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.44/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.44/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-12 10:56:21.000000 gmltools-0.0.44/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 10:56:44.378693 gmltools-0.0.44/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-12 10:56:12.000000 gmltools-0.0.44/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.276741 gmltools-0.0.44/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.313456 gmltools-0.0.44/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.44/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.44/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.337925 gmltools-0.0.44/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.44/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.44/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.365909 gmltools-0.0.44/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.44/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.44/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.44/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0   118555 2023-04-12 10:56:02.000000 gmltools-0.0.44/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.44/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.44/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.369946 gmltools-0.0.44/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.44/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 10:42:46.000000 gmltools-0.0.44/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.44/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.376656 gmltools-0.0.44/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.44/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.44/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.44/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.44/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.334408 gmltools-0.0.44/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-12 10:56:44.000000 gmltools-0.0.44/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.181303 gmltools-0.0.45/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.45/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.45/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-12 11:03:49.180306 gmltools-0.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.45/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.116741 gmltools-0.0.45/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.45/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.45/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.45/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.45/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.45/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.45/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-12 11:03:23.000000 gmltools-0.0.45/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 11:03:49.181303 gmltools-0.0.45/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-12 11:03:15.000000 gmltools-0.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.084575 gmltools-0.0.45/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.120075 gmltools-0.0.45/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.45/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.45/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.140220 gmltools-0.0.45/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.45/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.45/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.169383 gmltools-0.0.45/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.45/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.45/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.45/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0   118211 2023-04-12 11:03:07.000000 gmltools-0.0.45/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.45/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.45/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.173330 gmltools-0.0.45/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.45/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 10:42:46.000000 gmltools-0.0.45/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.45/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.179310 gmltools-0.0.45/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.45/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.45/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.45/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.45/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:03:49.137893 gmltools-0.0.45/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-12 11:03:48.000000 gmltools-0.0.45/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-12 11:03:48.000000 gmltools-0.0.45/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 11:03:48.000000 gmltools-0.0.45/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-12 11:03:48.000000 gmltools-0.0.45/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 11:03:48.000000 gmltools-0.0.45/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.44/LICENSE` & `gmltools-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/Models.ipynb` & `gmltools-0.0.45/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/PKG-INFO` & `gmltools-0.0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.44
+Version: 0.0.45
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.44/README.md` & `gmltools-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.45/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.45/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.45/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.45/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/gmltools.yml` & `gmltools-0.0.45/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/mltools.yml` & `gmltools-0.0.45/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/pyproject.toml` & `gmltools-0.0.45/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.44"
+version = "0.0.45"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.44/setup.py` & `gmltools-0.0.45/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.44',
+    'version': '0.0.45',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.44/src/gmltools/To_Do.txt` & `gmltools-0.0.45/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/eda/eda.py` & `gmltools-0.0.45/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/models/bayes.py` & `gmltools-0.0.45/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.45/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/models/model.py` & `gmltools-0.0.45/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,14 @@
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), "Class_Weights":str(class_weight), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                     'scoring':str(scoring), 'cv':str(cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight)}
         
 
-        return self.model
     
     def XGBoost_Classifier( self, ordinal_cat_cols:list=None,
                             scoring='accuracy', eval_metric='merror',
                             objective='multi:softmax', grid_params:dict={},
                             cv=10, random_params:dict=None, random_n_iter:int=10,
                             bayes_pbounds:dict=None,bayes_int_params:List[str]=None, 
                             bayes_n_iter:int=30, random_state:int=None,
@@ -559,15 +558,15 @@
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
                                     'scoring':str(scoring), 'cv':str(cv), 'eval_metric':str(eval_metric), 'sample_weight':str(sample_weight), "objective":str(objective)}
-        return self.model
+
     
     def LogisticRegression_Classifier(self,  ordinal_cat_cols:List[str]=None, scoring='accuracy',
                                     grid_params = {'LR__C': [0.1, 1, 10],
                                     'LR__penalty': ['l1', 'l2', 'elasticnet'],
                                     'LR__multi_class': ['ovr', 'multinomial'],   
                                     'LR__solver': ['newton-cg', 'lbfgs', 'liblinear', 'sag', 'saga']},
                                     cv=10, random_params:dict=None, random_n_iter:int=10,
@@ -676,15 +675,15 @@
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Class Weight":str(class_weight), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
                                     'scoring':str(scoring), 'cv':str(cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter)}
-        return self.model
+  
         
     
     def MLP_Classifier(self,ordinal_cat_cols=None, scoring='accuracy',
                        grid_params={'MLP__alpha': [1e-9,1e-7,1e-5,0.001,0.01],
                         'MLP__hidden_layer_sizes':[(5,),(10,),(15,),(20,),(25,)]},
                         cv=10, random_params=None, random_n_iter=10,
                         bayes_pbounds=None, bayes_int_params=None, bayes_n_iter=30, 
@@ -810,15 +809,14 @@
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Early Stopping":str(early_stopping), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape),
                                     'scoring':str(scoring), 'cv':str(cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter), "Learning Rate":str(learning_rate), "Learning Rate Init":str(learning_rate_init)}
         
-        return self.model
         
 
 
     #do the same for knn_classifier
     def KNN_Classifier(self,ordinal_cat_cols=None, scoring='accuracy',
                         grid_params={'KNN__n_neighbors': [3,10,25,60]},
                         cv=10, random_params=None, random_n_iter=10,  bayes_pbounds=None,
@@ -913,15 +911,14 @@
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
                                     'scoring':str(scoring), 'cv':str(cv),  'sample_weight':str(sample_weight)}
 
-        return self.model
 
 
     
 
     #do the same for a decision tree
     def DecisionTree_Classifier(self, ordinal_cat_cols=None, scoring='accuracy',
                             grid_params={'DT__max_depth': [3,5,7,10],
@@ -1013,15 +1010,14 @@
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Class Weight": class_weight, 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape),
                                     'scoring':str(scoring), 'cv':str(cv),  'sample_weight':str(sample_weight)}
 
-        return self.model
     #save model
     def save(self, return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
         Parameters
         ----------
@@ -1261,15 +1257,14 @@
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
 
-            return self.model
     
     def XGB_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'XGB__n_estimators': [100, 200, 300, 400, 500],
                                 'XGB__max_depth': [3,5,7,10],
                                 'XGB__learning_rate': [0.01,0.05,0.1,0.15,0.2],
                                 'XGB__min_child_weight': [1,3,5,7],
                                 'XGB__gamma': [0.0,0.1,0.2,0.3,0.4],
@@ -1364,15 +1359,14 @@
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
 
-            return self.model
 
     
     def Linear_Regression(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'LR__fit_intercept': [True, False],
                                 'LR__normalize': [True, False],
                                 'LR__copy_X': [True, False]}, 
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None,
@@ -1462,16 +1456,15 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
-    
-            return self.model
+
     
     def KNN_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'KNN__n_neighbors': [3,5,7,9,11,13,15,17,19,21,23,25,27,29,31,33,35,37,39,41,43,45,47,49,51,53,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,87,89,91,93,95,97,99],
                                 'KNN__weights': ['uniform', 'distance'],
                                 'KNN__algorithm': ['auto', 'ball_tree', 'kd_tree', 'brute'],
                                 'KNN__leaf_size': [10,20,30,40,50,60,70,80,90,100],
                                 'KNN__p': [1,2]}, 
@@ -1563,15 +1556,14 @@
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
     
-            return self.model
 
 
     
     def DecisionTree_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'DT__criterion': ["squared_error", "friedman_mse", "absolute_error", "poisson"],
                                 'DT__max_depth': [None,2,3,4,5],
                                 'DT__min_samples_split': [2,3,4,],
@@ -1665,15 +1657,14 @@
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
 
-            return self.model
     
     def MLP_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'MLP__hidden_layer_sizes': [(3,),(5,)],
                                 'MLP__activation': ['identity', 'logistic', 'tanh', 'relu'],
                                 'MLP__solver': ['lbfgs', 'sgd', 'adam'],
                                 'MLP__alpha': [0.0001,0.001,0.01,0.1,1,10,100],
                                 'MLP__max_iter': [200]},
@@ -1769,15 +1760,15 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
-            return self.model
+
     
 
     def save(self,return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
         Parameters
@@ -1811,15 +1802,15 @@
             #set model_name the firts column and Search conditions the second column
             cols = df_best.columns.tolist()
             cols = cols[-1:] + cols[:-1]
             df_best = df_best[cols]
 
             # save in the second sheet
             file_path = './models/summary_models.xlsx'
-            if os.path.exists(file_path):
+            if os.path.isfile(file_path):
                 df_summary = pd.read_excel(file_path, sheet_name='Sheet2')
                 df_summary = pd.concat([df_summary, df_best], axis=0,ignore_index=True)
                 df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
             else:
                 df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
             if return_best_metrics:
                 return df_best
```

### Comparing `gmltools-0.0.44/src/gmltools/models/models_info.py` & `gmltools-0.0.45/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.45/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.45/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.45/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.45/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.45/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.45/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.44/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.45/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.44
+Version: 0.0.45
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.44/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.45/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

