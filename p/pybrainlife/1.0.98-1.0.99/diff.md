# Comparing `tmp/pybrainlife-1.0.98.tar.gz` & `tmp/pybrainlife-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrainlife-1.0.98.tar", max compression
+gzip compressed data, was "pybrainlife-1.0.99.tar", max compression
```

## Comparing `pybrainlife-1.0.98.tar` & `pybrainlife-1.0.99.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.0.98/README.md
--rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.0.98/pybrainlife/__init__.py
--rwxr-xr-x   0        0        0    18114 2023-04-12 18:47:32.386736 pybrainlife-1.0.98/pybrainlife/data/collect.py
--rwxr-xr-x   0        0        0    18783 2023-04-12 20:05:01.240314 pybrainlife-1.0.98/pybrainlife/data/manipulate.py
--rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.0.98/pybrainlife/vis/__pycache__/data.cpython-38.pyc
--rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.0.98/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
--rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.0.98/pybrainlife/vis/plots.py
--rw-r--r--   0        0        0      748 2023-04-12 20:05:14.648282 pybrainlife-1.0.98/pyproject.toml
--rw-r--r--   0        0        0     3489 1970-01-01 00:00:00.000000 pybrainlife-1.0.98/setup.py
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pybrainlife-1.0.98/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.0.99/README.md
+-rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.0.99/pybrainlife/__init__.py
+-rwxr-xr-x   0        0        0    18114 2023-04-12 18:47:32.386736 pybrainlife-1.0.99/pybrainlife/data/collect.py
+-rwxr-xr-x   0        0        0    19287 2023-04-12 21:52:50.584436 pybrainlife-1.0.99/pybrainlife/data/manipulate.py
+-rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.0.99/pybrainlife/vis/__pycache__/data.cpython-38.pyc
+-rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.0.99/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
+-rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.0.99/pybrainlife/vis/plots.py
+-rw-r--r--   0        0        0      748 2023-04-12 21:52:58.620415 pybrainlife-1.0.99/pyproject.toml
+-rw-r--r--   0        0        0     3489 1970-01-01 00:00:00.000000 pybrainlife-1.0.99/setup.py
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pybrainlife-1.0.99/PKG-INFO
```

### Comparing `pybrainlife-1.0.98/README.md` & `pybrainlife-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.98/pybrainlife/data/collect.py` & `pybrainlife-1.0.99/pybrainlife/data/collect.py`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.98/pybrainlife/data/manipulate.py` & `pybrainlife-1.0.99/pybrainlife/data/manipulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,41 +328,44 @@
 def build_global_measures_df(network):
 	global_measurements = pd.DataFrame()
 	for i in network.attributes():
 		global_measurements[i] = [network[i]]
 
 	return global_measurements
 
-def build_temporary_network_dataframe(network,function_name,subjectID):
+def build_temporary_network_dataframe(network,function_name,subjectID,sessionID,tags,datatype_tags):
 
     if function_name == 'connectivity':
         tmp = build_connectivity_matrix(network)
     elif function_name == 'local':
         tmp = build_local_measures_df(network)
     else:
         tmp = build_global_measures_df(network)
 
     tmp['subjectID'] = [ subjectID for f in range(len(tmp)) ]
+    tmp['sessionID'] = [ sessionID for f in range(len(tmp)) ]
+    tmp['tags'] = [ tags for f in range(len(tmp)) ]
+    tmp['datatype_tags'] = [ datatype_tags for f in range(len(tmp)) ]
 
     return tmp
 
 def parse_networks(network_df):
 
     connectivity_matrices = pd.DataFrame()
     global_measures = pd.DataFrame()
     local_measures = pd.DataFrame()
 
     for i in range(len(network_df)):
-        connectivity_matrices = pd.concat([connectivity_matrices,build_temporary_network_dataframe(network_df.iloc[i]['igraph'],'connectivity',network_df.iloc[i]['subjectID'])])
-        global_measures = pd.concat([global_measures,build_temporary_network_dataframe(network_df.iloc[i]['igraph'],'global',network_df.iloc[i]['subjectID'])])
-        local_measures = pd.concat([local_measures,build_temporary_network_dataframe(network_df.iloc[i]['igraph'],'local',network_df.iloc[i]['subjectID'])])
-
-    connectivity_matrices = connectivity_matrices.reset_index().merge(network_df[['subjectID','sessionID','tags','datatype_tags']],on='subjectID').set_index('index')
-    global_measures = global_measures.merge(network_df[['subjectID','sessionID','tags','datatype_tags']],on='subjectID')
-    local_measures = local_measures.merge(network_df[['subjectID','sessionID','tags','datatype_tags']],on='subjectID')
+        connectivity_matrices = pd.concat([connectivity_matrices,build_temporary_network_dataframe(network_df.iloc[i]['igraph'],'connectivity',network_df.iloc[i]['subjectID'],network_df.iloc[i]['sessionID'],network_df.iloc[i]['tags'],network_df.iloc[i]['datatype_tags'])])
+        global_measures = pd.concat([global_measures,build_temporary_network_dataframe(network_df.iloc[i]['igraph'],'global',network_df.iloc[i]['subjectID'],network_df.iloc[i]['sessionID'],network_df.iloc[i]['tags'],network_df.iloc[i]['datatype_tags'])])
+        local_measures = pd.concat([local_measures,build_temporary_network_dataframe(network_df.iloc[i]['igraph'],'local',network_df.iloc[i]['subjectID'],network_df.iloc[i]['sessionID'],network_df.iloc[i]['tags'],network_df.iloc[i]['datatype_tags'])])
+
+    # connectivity_matrices = connectivity_matrices.reset_index().merge(network_df[['subjectID','sessionID','tags','datatype_tags']],on='subjectID').set_index('index')
+    # global_measures = global_measures.merge(network_df[['subjectID','sessionID','tags','datatype_tags']],on='subjectID')
+    # local_measures = local_measures.merge(network_df[['subjectID','sessionID','tags','datatype_tags']],on='subjectID')
 
     return connectivity_matrices, global_measures, local_measures
 
 # this function will binarize an adjacency matrix
 def binarize_matrices(data):
     
     # use brain connectivity toolbox to binarize data
```

### Comparing `pybrainlife-1.0.98/pybrainlife/vis/__pycache__/data.cpython-38.pyc` & `pybrainlife-1.0.99/pybrainlife/vis/__pycache__/data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.98/pybrainlife/vis/__pycache__/plots.cpython-38.pyc` & `pybrainlife-1.0.99/pybrainlife/vis/__pycache__/plots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.98/pybrainlife/vis/plots.py` & `pybrainlife-1.0.99/pybrainlife/vis/plots.py`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.98/pyproject.toml` & `pybrainlife-1.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybrainlife"
-version = "1.0.98"
+version = "1.0.99"
 description = "This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io"
 authors = ["Brad Caron <bacaron245@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/brainlife/pybrainlife"
 repository = "https://github.com/brainlife/pybrainlife"
 keywords = ["brainlife"]
```

### Comparing `pybrainlife-1.0.98/setup.py` & `pybrainlife-1.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2.28.1,<3.0.0',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'seaborn>=0.12.2,<0.13.0']
 
 setup_kwargs = {
     'name': 'pybrainlife',
-    'version': '1.0.98',
+    'version': '1.0.99',
     'description': 'This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io',
     'long_description': '[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/soichih/abcd-spec)\n\n# pybrainlife\nThis repository contains the python package for collecting, collating, manipulating, analyzing, and visualizing MRI data generated on brainlife.io. Designed to used within the brainlife.io Analysis tab Jupyter notebooks, can be installed as a pypi package to your local machine.\n\n### Authors\n- Brad Caron (bacaron@iu.edu)\n\n### Contributors\n- Soichi Hayashi (hayashi@iu.edu)\n- Franco Pestilli (franpest@indiana.edu)\n\n### Funding\n[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)\n[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)\n\n### Citations\n\nPlease cite the following articles when publishing papers that used data, code or other resources created by the brainlife.io community.\n\n1. Avesani, P., McPherson, B., Hayashi, S. et al. The open diffusion data derivatives, brain data upcycling via integrated publishing of derivatives and reproducible open cloud services. Sci Data 6, 69 (2019). https://doi.org/10.1038/s41597-019-0073-y\n\n### Directory structure\n```\npybrainlife\n├── dist\n│\xa0\xa0 ├── pybrainlife-1.0.0-py3-none-any.whl\n│\xa0\xa0 └── pybrainlife-1.0.0.tar.gz\n├── poetry.lock\n├── pybrainlife\n│\xa0\xa0 ├── data\n│\xa0\xa0 │\xa0\xa0 ├── collect.py\n│\xa0\xa0 │\xa0\xa0 └── manipulate.py\n│\xa0\xa0 ├── __init__.py\n│\xa0\xa0 └── vis\n│\xa0\xa0     ├── plots.py\n│\xa0\xa0     └── __pycache__\n│\xa0\xa0         ├── data.cpython-38.pyc\n│\xa0\xa0         └── plots.cpython-38.pyc\n├── pyproject.toml\n├── README.md\n└── tests\n    ├── __init__.py\n    └── test_pybrainlife.py\n```\n\n### Installing locally\nThis package can be installed locally via PyPi using the following command:\n\n```\npip install pybrainlife\n```\n\n### Dependencies\n\nThis package requires the following libraries.\n  - python = "3.8"\n  - numpy = "^1.9.3"\n  - bctpy = "^0.5.2"\n  - seaborn = "^0.11.2"\n  - jgf = "^0.2.2"\n  - scikit-learn = "^1.0.2"\n  - pandas = "^1.4.2"\n  - scipy = "^1.8.0"\n  - requests = "^2.27.1"\n\nLibrary of Modules for Loading Data and Analyzing Data from brainlife.io\n\n2022 The University of Texas at Austin\n',
     'author': 'Brad Caron',
     'author_email': 'bacaron245@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/brainlife/pybrainlife',
```

### Comparing `pybrainlife-1.0.98/PKG-INFO` & `pybrainlife-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybrainlife
-Version: 1.0.98
+Version: 1.0.99
 Summary: This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io
 Home-page: https://github.com/brainlife/pybrainlife
 Keywords: brainlife
 Author: Brad Caron
 Author-email: bacaron245@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

