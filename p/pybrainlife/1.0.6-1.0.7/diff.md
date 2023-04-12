# Comparing `tmp/pybrainlife-1.0.6.tar.gz` & `tmp/pybrainlife-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrainlife-1.0.6.tar", max compression
+gzip compressed data, was "pybrainlife-1.0.7.tar", max compression
```

## Comparing `pybrainlife-1.0.6.tar` & `pybrainlife-1.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.0.6/README.md
--rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.0.6/pybrainlife/__init__.py
--rwxr-xr-x   0        0        0    17760 2023-03-28 20:01:57.016380 pybrainlife-1.0.6/pybrainlife/data/collect.py
--rwxr-xr-x   0        0        0    15541 2023-03-29 19:42:35.746368 pybrainlife-1.0.6/pybrainlife/data/manipulate.py
--rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.0.6/pybrainlife/vis/__pycache__/data.cpython-38.pyc
--rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.0.6/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
--rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.0.6/pybrainlife/vis/plots.py
--rw-r--r--   0        0        0      747 2023-03-29 19:42:43.218350 pybrainlife-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pybrainlife-1.0.6/setup.py
--rw-r--r--   0        0        0     3426 1970-01-01 00:00:00.000000 pybrainlife-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.0.7/README.md
+-rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.0.7/pybrainlife/__init__.py
+-rwxr-xr-x   0        0        0    18100 2023-04-12 18:38:32.639823 pybrainlife-1.0.7/pybrainlife/data/collect.py
+-rwxr-xr-x   0        0        0    16728 2023-04-12 18:38:34.619819 pybrainlife-1.0.7/pybrainlife/data/manipulate.py
+-rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.0.7/pybrainlife/vis/__pycache__/data.cpython-38.pyc
+-rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.0.7/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
+-rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.0.7/pybrainlife/vis/plots.py
+-rw-r--r--   0        0        0      747 2023-04-12 18:38:49.891789 pybrainlife-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pybrainlife-1.0.7/setup.py
+-rw-r--r--   0        0        0     3426 1970-01-01 00:00:00.000000 pybrainlife-1.0.7/PKG-INFO
```

### Comparing `pybrainlife-1.0.6/README.md` & `pybrainlife-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.6/pybrainlife/data/collect.py` & `pybrainlife-1.0.7/pybrainlife/data/collect.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,43 +58,47 @@
     
     return finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags
 
 ## this function will call add_subjects_sessions to add the appropriate columns and will append the object data to a study-wide dataframe
 def compile_data(paths,subjects,sessions,data,dtags,tags):
     # loops through all paths
     for i in range(len(paths)):
-        # if network, load json. if not, load csv
-        if '.json.gz' in paths[i]:
-            tmpdata = pd.read_json(paths[i],orient='index').reset_index(drop=True)
-            tmpdata = add_subjects_sessions(subjects[i],sessions[i],paths[i],tmpdata)
+        # if network, use igraph and pandas. if not, use just pandas
+        if 'network.json.gz' in paths[i]:
+            # tmpdata = pd.read_json(paths[i],orient='index').reset_index(drop=True)
+            tmpdata = pd.DataFrame()
+            tmpdata['igraph'] = jgf.igraph.load(paths[i],compressed=True)
+            # tmpdata = add_subjects_sessions(subjects[i],sessions[i],paths[i],tmpdata)
+            # tmpdata = add_tags_dtags(tags[i],dtags[i],tmpdata) # added 4/12/2023
         else:
             if '.tsv' in paths[i]:
                 sep = '\t'
             else:
                 sep = ','
             tmpdata = pd.read_csv(paths[i],sep=sep)
-            tmpdata = add_subjects_sessions(subjects[i],sessions[i],paths[i],tmpdata)
-            tmpdata = add_tags_dtags(tags[i],dtags[i],tmpdata)
+        tmpdata = add_subjects_sessions(subjects[i],sessions[i],paths[i],tmpdata)
+        tmpdata = add_tags_dtags(tags[i],dtags[i],tmpdata)
 
         #data = data.append(tmpdata,ignore_index=True)
         data = pd.concat([data,tmpdata])
 
     # replace empty spaces with nans
     data = data.replace(r'^\s+$', np.nan, regex=True)
     
     return data
 
+# NO LONGER NECESSARY
 # this function will comile network adjacency matrices into a dictionary structure
-def compile_network_adjacency_matrices(paths,subjects,sessions,data):
+# def compile_network_adjacency_matrices(paths,subjects,sessions,data):
     
-    # loop through paths and append adjacency matrix to dictionary
-    for i in range(len(paths)):
-        data[subjects[i]+'_sess'+sessions[i]] = jgf.conmat.load(paths[i],compressed=True)[0]
+#     # loop through paths and append adjacency matrix to dictionary
+#     for i in range(len(paths)):
+#         data[subjects[i]+'_sess'+sessions[i]] = jgf.conmat.load(paths[i],compressed=True)[0]
 
-    return data
+#     return data
 
 ### load data
 ## this function is useful for identifying duplicate datatypes. if it finds one, it will update the data with the latest finishing dataset.
 def check_for_duplicates(obj,finish_dates,subjects,sessions,paths,obj_tags,obj_datatype_tags):
     
     # first checks if there is a session id available in the keys of the object. if finds one, then checks if the subject and session ID 
     # were already looped over. if so, will delete position in list and update with appropriate path. if it doesn't find a session ID, it
@@ -164,15 +168,16 @@
     for i in tags:
         if i in obj['output'][tagOrDatatypeTag]:
             ctr=ctr+1
     
     return ctr
 
 ## this function is the wrapper function that calls all the prevouis functions to generate a dataframe for the entire project of the appropriate datatype
-def collect_data(datatype,datatype_tags,tags,filename,outPath,net_adj):
+# def collect_data(datatype,datatype_tags,tags,filename,outPath,net_adj): # net_adj no longer necessary
+def collect_data(datatype,datatype_tags,tags,filename,outPath):
 
     # grab path and data objects
     objects = requests.get('https://brainlife.io/api/warehouse/secondary/list/%s'%os.environ['PROJECT_ID']).json()
 
     # subjects and paths
     subjects = []
     sessions = []
@@ -248,25 +253,25 @@
     # check if tab separated or comma separated by looking at input filename
     if '.tsv' in filename:
         sep = '\t'
     else:
         sep = ','
 
     # compile data
-    if net_adj:
-        data = {}
-        data = compile_network_adjacency_matrices(paths,subjects,sessions,data)
-        if outPath:
-            np.save(outPath,data)
-    else:
-        data = compile_data(paths,subjects,sessions,data,obj_datatype_tags,obj_tags)
-
-        # output data structure for records and any further analyses
-        if outPath:
-            data.to_csv(outPath,sep=sep,index=False)
+    # if net_adj:
+    #     data = {}
+    #     data = compile_network_adjacency_matrices(paths,subjects,sessions,data)
+    #     if outPath:
+    #         np.save(outPath,data)
+    # else:
+    data = compile_data(paths,subjects,sessions,data,obj_datatype_tags,obj_tags)
+
+    # output data structure for records and any further analyses
+    if outPath:
+        data.to_csv(outPath,sep=sep,index=False)
 
     return data, obj_tags, obj_datatype_tags
 
 # ## this function is the wrapper function that calls all the prevouis functions to generate a dataframe for the entire project of the appropriate datatype
 # def collect_data(datatype,datatype_tags=[],tags=[],filename='',outPath='',net_adj=False):
 
 #     if datatype in ['cortex_example','tractmeasures_example']:
```

### Comparing `pybrainlife-1.0.6/pybrainlife/data/manipulate.py` & `pybrainlife-1.0.7/pybrainlife/data/manipulate.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,14 +289,45 @@
         merged = [{**structural[0],**diffusion[0]}]
 
         if outPath:
             with open(outPath+'_'+i+'.json','w') as out_f:
                 json.dump(merged,out_f)
 
 ### adjacency-matrix related fuctions for computing network values locally
+# this function creates a datframe for the connectivity matrix from a network.igraph object
+def build_connectivity_matrix(network,output_array=False):
+    if 'weight' in network.attributes():
+        conn_mat = pd.DataFrame(network.get_adjacency(attribute='weight').data)
+    else:
+        conn_mat = pd.DataFrame(network.get_adjacency().data)
+            
+    labels = network.get_vertex_dataframe()
+    conn_mat = conn_mat.rename(columns=labels.name,index=labels.name)
+
+    if output_array:
+        conn_mat = conn_mat.values
+
+    return conn_mat
+
+# this function will build a dataframe of the LOCAL network measures computed from a network.igraph object
+def build_local_measures_df(network):
+    local_measurements = network.get_vertex_dataframe().reset_index() #local
+    # labels = network.get_vertex_dataframe()
+    # local_measurements['name'] = labels['name']
+
+    return local_measurements
+
+# this function will build a dataframe of the GLOBAL network measures computed from a network.igraph object
+def build_global_measures_df(network):
+	global_measurements = pd.DataFrame()
+	for i in network.attributes():
+		global_measurements[i] = [network[i]]
+
+	return global_measurements
+
 # this function will binarize an adjacency matrix
 def binarize_matrices(data):
     
     # use brain connectivity toolbox to binarize data
     bin_data = [ bct.utils.binarize(data[f]) for f in data.keys() ]
     
     return bin_data
```

### Comparing `pybrainlife-1.0.6/pybrainlife/vis/__pycache__/data.cpython-38.pyc` & `pybrainlife-1.0.7/pybrainlife/vis/__pycache__/data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.6/pybrainlife/vis/__pycache__/plots.cpython-38.pyc` & `pybrainlife-1.0.7/pybrainlife/vis/__pycache__/plots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.6/pybrainlife/vis/plots.py` & `pybrainlife-1.0.7/pybrainlife/vis/plots.py`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.6/pyproject.toml` & `pybrainlife-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybrainlife"
-version = "1.0.6"
+version = "1.0.7"
 description = "This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io"
 authors = ["Brad Caron <bacaron245@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/brainlife/pybrainlife"
 repository = "https://github.com/brainlife/pybrainlife"
 keywords = ["brainlife"]
```

### Comparing `pybrainlife-1.0.6/setup.py` & `pybrainlife-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2.28.1,<3.0.0',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'seaborn>=0.12.2,<0.13.0']
 
 setup_kwargs = {
     'name': 'pybrainlife',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io',
     'long_description': '[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/soichih/abcd-spec)\n\n# pybrainlife\nThis repository contains the python package for collecting, collating, manipulating, analyzing, and visualizing MRI data generated on brainlife.io. Designed to used within the brainlife.io Analysis tab Jupyter notebooks, can be installed as a pypi package to your local machine.\n\n### Authors\n- Brad Caron (bacaron@iu.edu)\n\n### Contributors\n- Soichi Hayashi (hayashi@iu.edu)\n- Franco Pestilli (franpest@indiana.edu)\n\n### Funding\n[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)\n[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)\n\n### Citations\n\nPlease cite the following articles when publishing papers that used data, code or other resources created by the brainlife.io community.\n\n1. Avesani, P., McPherson, B., Hayashi, S. et al. The open diffusion data derivatives, brain data upcycling via integrated publishing of derivatives and reproducible open cloud services. Sci Data 6, 69 (2019). https://doi.org/10.1038/s41597-019-0073-y\n\n### Directory structure\n```\npybrainlife\n├── dist\n│\xa0\xa0 ├── pybrainlife-1.0.0-py3-none-any.whl\n│\xa0\xa0 └── pybrainlife-1.0.0.tar.gz\n├── poetry.lock\n├── pybrainlife\n│\xa0\xa0 ├── data\n│\xa0\xa0 │\xa0\xa0 ├── collect.py\n│\xa0\xa0 │\xa0\xa0 └── manipulate.py\n│\xa0\xa0 ├── __init__.py\n│\xa0\xa0 └── vis\n│\xa0\xa0     ├── plots.py\n│\xa0\xa0     └── __pycache__\n│\xa0\xa0         ├── data.cpython-38.pyc\n│\xa0\xa0         └── plots.cpython-38.pyc\n├── pyproject.toml\n├── README.md\n└── tests\n    ├── __init__.py\n    └── test_pybrainlife.py\n```\n\n### Installing locally\nThis package can be installed locally via PyPi using the following command:\n\n```\npip install pybrainlife\n```\n\n### Dependencies\n\nThis package requires the following libraries.\n  - python = "3.8"\n  - numpy = "^1.9.3"\n  - bctpy = "^0.5.2"\n  - seaborn = "^0.11.2"\n  - jgf = "^0.2.2"\n  - scikit-learn = "^1.0.2"\n  - pandas = "^1.4.2"\n  - scipy = "^1.8.0"\n  - requests = "^2.27.1"\n\nLibrary of Modules for Loading Data and Analyzing Data from brainlife.io\n\n2022 The University of Texas at Austin\n',
     'author': 'Brad Caron',
     'author_email': 'bacaron245@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/brainlife/pybrainlife',
```

### Comparing `pybrainlife-1.0.6/PKG-INFO` & `pybrainlife-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybrainlife
-Version: 1.0.6
+Version: 1.0.7
 Summary: This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io
 Home-page: https://github.com/brainlife/pybrainlife
 Keywords: brainlife
 Author: Brad Caron
 Author-email: bacaron245@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

