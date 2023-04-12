# Comparing `tmp/gmltools-0.0.43.tar.gz` & `tmp/gmltools-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.43.tar", last modified: Wed Apr 12 10:52:26 2023, max compression
+gzip compressed data, was "gmltools-0.0.44.tar", last modified: Wed Apr 12 10:56:44 2023, max compression
```

## Comparing `gmltools-0.0.43.tar` & `gmltools-0.0.44.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.847082 gmltools-0.0.43/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.43/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.43/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-12 10:52:26.847082 gmltools-0.0.43/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.43/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.757871 gmltools-0.0.43/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.43/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.43/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.43/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.43/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.43/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.43/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-12 10:51:38.000000 gmltools-0.0.43/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 10:52:26.847082 gmltools-0.0.43/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-12 10:51:29.000000 gmltools-0.0.43/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.729393 gmltools-0.0.43/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.765313 gmltools-0.0.43/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.43/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.43/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.807028 gmltools-0.0.43/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.43/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.43/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.834570 gmltools-0.0.43/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.43/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.43/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.43/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0   118553 2023-04-12 10:51:56.000000 gmltools-0.0.43/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.43/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.43/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.840069 gmltools-0.0.43/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.43/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 10:42:46.000000 gmltools-0.0.43/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.43/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.846076 gmltools-0.0.43/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.43/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.43/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.43/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.43/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:52:26.804301 gmltools-0.0.43/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-12 10:52:26.000000 gmltools-0.0.43/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-12 10:52:26.000000 gmltools-0.0.43/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:52:26.000000 gmltools-0.0.43/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-12 10:52:26.000000 gmltools-0.0.43/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 10:52:26.000000 gmltools-0.0.43/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.377689 gmltools-0.0.44/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.44/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.44/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-12 10:56:44.377689 gmltools-0.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.44/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.311135 gmltools-0.0.44/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.44/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.44/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.44/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.44/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.44/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.44/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-12 10:56:21.000000 gmltools-0.0.44/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:56:44.378693 gmltools-0.0.44/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-12 10:56:12.000000 gmltools-0.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.276741 gmltools-0.0.44/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.313456 gmltools-0.0.44/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.44/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.44/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.337925 gmltools-0.0.44/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.44/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.44/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.365909 gmltools-0.0.44/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.44/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.44/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.44/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0   118555 2023-04-12 10:56:02.000000 gmltools-0.0.44/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.44/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.44/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.369946 gmltools-0.0.44/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.44/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 10:42:46.000000 gmltools-0.0.44/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.44/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.376656 gmltools-0.0.44/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.44/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.44/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.44/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.44/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:56:44.334408 gmltools-0.0.44/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-12 10:56:44.000000 gmltools-0.0.44/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 10:56:43.000000 gmltools-0.0.44/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.43/LICENSE` & `gmltools-0.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/Models.ipynb` & `gmltools-0.0.44/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/PKG-INFO` & `gmltools-0.0.44/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.43
+Version: 0.0.44
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.43/README.md` & `gmltools-0.0.44/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.44/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.44/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.44/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.44/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/gmltools.yml` & `gmltools-0.0.44/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/mltools.yml` & `gmltools-0.0.44/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/pyproject.toml` & `gmltools-0.0.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.43"
+version = "0.0.44"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.43/setup.py` & `gmltools-0.0.44/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.43',
+    'version': '0.0.44',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.43/src/gmltools/To_Do.txt` & `gmltools-0.0.44/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/eda/eda.py` & `gmltools-0.0.44/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/models/bayes.py` & `gmltools-0.0.44/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.44/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/models/model.py` & `gmltools-0.0.44/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1901,15 +1901,15 @@
         return [(search_list[i],value_var) for i, value_var in enumerate(args) if value_var is not None]
         #add the variable name to the value
     @staticmethod
     def _not_none_recursive(*args):
         """
         This function returns a list of the arguments that are not None. Is used to store the not none parameters of the  the recursive parameters of the model in the dictionary self._overall_dict
         """
-        recursive_list=['columns_lags', 'column_rolled_lags','lags,rolled_lags', 'rolled_metrics', 'column_rolled_lags_initial']
+        recursive_list=['columns_lags', 'column_rolled_lags','lags','rolled_lags', 'rolled_metrics', 'column_rolled_lags_initial']
         return [(recursive_list[i],value_var) for i, value_var in enumerate(args) if value_var is not None]
```

### Comparing `gmltools-0.0.43/src/gmltools/models/models_info.py` & `gmltools-0.0.44/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.44/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.44/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.44/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.44/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.44/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.44/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.43/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.44/src/gmltools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.43
+Version: 0.0.44
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.43/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.44/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

