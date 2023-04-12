# Comparing `tmp/intelligraphs-0.1.0.tar.gz` & `tmp/intelligraphs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelligraphs-0.1.0.tar", last modified: Wed Apr 12 13:16:35 2023, max compression
+gzip compressed data, was "intelligraphs-0.1.1.tar", last modified: Wed Apr 12 13:40:39 2023, max compression
```

## Comparing `intelligraphs-0.1.0.tar` & `intelligraphs-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 thiviyan   (501) staff       (20)        0 2023-04-12 13:16:35.054207 intelligraphs-0.1.0/
--rw-r--r--   0 thiviyan   (501) staff       (20)     1081 2023-04-06 11:58:00.000000 intelligraphs-0.1.0/LICENSE
--rw-r--r--   0 thiviyan   (501) staff       (20)     6040 2023-04-12 13:16:35.053203 intelligraphs-0.1.0/PKG-INFO
--rw-r--r--   0 thiviyan   (501) staff       (20)     5301 2023-04-11 13:09:32.000000 intelligraphs-0.1.0/README.md
-drwxr-xr-x   0 thiviyan   (501) staff       (20)        0 2023-04-12 13:16:35.051587 intelligraphs-0.1.0/intelligraphs.egg-info/
--rw-r--r--   0 thiviyan   (501) staff       (20)     6040 2023-04-12 13:16:34.000000 intelligraphs-0.1.0/intelligraphs.egg-info/PKG-INFO
--rw-r--r--   0 thiviyan   (501) staff       (20)      210 2023-04-12 13:16:34.000000 intelligraphs-0.1.0/intelligraphs.egg-info/SOURCES.txt
--rw-r--r--   0 thiviyan   (501) staff       (20)        1 2023-04-12 13:16:34.000000 intelligraphs-0.1.0/intelligraphs.egg-info/dependency_links.txt
--rw-r--r--   0 thiviyan   (501) staff       (20)       20 2023-04-12 13:16:34.000000 intelligraphs-0.1.0/intelligraphs.egg-info/requires.txt
--rw-r--r--   0 thiviyan   (501) staff       (20)        1 2023-04-12 13:16:34.000000 intelligraphs-0.1.0/intelligraphs.egg-info/top_level.txt
--rw-r--r--   0 thiviyan   (501) staff       (20)       38 2023-04-12 13:16:35.054603 intelligraphs-0.1.0/setup.cfg
--rw-r--r--   0 thiviyan   (501) staff       (20)      977 2023-04-08 22:32:51.000000 intelligraphs-0.1.0/setup.py
+drwxr-xr-x   0 thiviyan   (501) staff       (20)        0 2023-04-12 13:40:39.797900 intelligraphs-0.1.1/
+-rw-r--r--   0 thiviyan   (501) staff       (20)     1081 2023-04-06 11:58:00.000000 intelligraphs-0.1.1/LICENSE
+-rw-r--r--   0 thiviyan   (501) staff       (20)     6356 2023-04-12 13:40:39.797531 intelligraphs-0.1.1/PKG-INFO
+-rw-r--r--   0 thiviyan   (501) staff       (20)     5617 2023-04-12 13:33:47.000000 intelligraphs-0.1.1/README.md
+drwxr-xr-x   0 thiviyan   (501) staff       (20)        0 2023-04-12 13:40:39.797109 intelligraphs-0.1.1/intelligraphs.egg-info/
+-rw-r--r--   0 thiviyan   (501) staff       (20)     6356 2023-04-12 13:40:39.000000 intelligraphs-0.1.1/intelligraphs.egg-info/PKG-INFO
+-rw-r--r--   0 thiviyan   (501) staff       (20)      210 2023-04-12 13:40:39.000000 intelligraphs-0.1.1/intelligraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 thiviyan   (501) staff       (20)        1 2023-04-12 13:40:39.000000 intelligraphs-0.1.1/intelligraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 thiviyan   (501) staff       (20)       20 2023-04-12 13:40:39.000000 intelligraphs-0.1.1/intelligraphs.egg-info/requires.txt
+-rw-r--r--   0 thiviyan   (501) staff       (20)        1 2023-04-12 13:40:39.000000 intelligraphs-0.1.1/intelligraphs.egg-info/top_level.txt
+-rw-r--r--   0 thiviyan   (501) staff       (20)       38 2023-04-12 13:40:39.797997 intelligraphs-0.1.1/setup.cfg
+-rw-r--r--   0 thiviyan   (501) staff       (20)      977 2023-04-12 13:40:20.000000 intelligraphs-0.1.1/setup.py
```

### Comparing `intelligraphs-0.1.0/LICENSE` & `intelligraphs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `intelligraphs-0.1.0/PKG-INFO` & `intelligraphs-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelligraphs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library to generate synthetic Knowledge Graphs using random triples.
 Home-page: https://github.com/thiviyanT/intelligraphs
 Author: Thiviyan Thanapalasingam
 Author-email: thiviyan.t@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,90 +14,52 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p  align="center">
-    <img src="images/IntelliGraph-logo.png" width="450px;" style="max-width: 100%;  margin-right:10px;">
+    <img src="https://raw.githubusercontent.com/thiviyanT/IntelliGraphs/main/images/IntelliGraph-logo.png?token=GHSAT0AAAAAAB5H4DZTLA4DT3TVAZXVWXPCZBWYCDA" width="450px;" style="max-width: 100%;  margin-right:10px;">
 <p>
 
 ---
 
-IntelliGraphs is a library that generates a collection of datasets for benchmarking generative models for knowledge
-graphs. These are graphs that are generated according to first order logic rules. These datasets are intended to be used
+[![PyPI Latest Release](https://img.shields.io/pypi/v/intelligraphs.svg)]([https://pypi.org/project/pandas/](https://pypi.org/project/intelligraphs/))
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+IntelliGraphs is a Python package that generates a collection of benchmark datasets. These datasets are intended to be used
 for benchmarking machine learning models under transductive settings. It can also be used as a testbed for developing
-new generative models. This library was designed to be extendable to create new synthetic datasets with other custom 
-First-Order Logical (FOL) constraints.
+new generative models. This library was designed to be extendable to create new synthetic datasets with custom 
+First-Order Logical (FOL) rules.
 
 ### TODO
 
 * Ask Paul: Do we want to register this with Zenodo. If so, add DOI badge here.
 * Ask Paul: How to generate dataset metadata? Is it needed?
 * Ask Paul: When to register dataset? Before or after publication?
 * Ask Paul: Where to put the dataset so that it lasts? (Zenodo, GitHub, etc.)
 * Ask Peter/Paul: Do we want to make it available on PyPI? If so, add badge here.
 * Make GitHub repo anonymous before submission
 
+## Installation
+
+To install IntelliGraphs locally, simply:
+
+```bash
+pip install intelligraphs
+```
+
 ## Advantages
 
 * Easy to use: Generate and manipulate Knowledge Graphs with a simple and clean Python API.
 * Flexible: Customize the number of graphs, triples, and data splits.
 * Extendable: Create more graphs according to custom FOL rules.
 * Efficient: Fast and memory-efficient graph generation and manipulation using native Python data structures.
 * Visualization: Visualize Knowledge Graphs.
 
-## Datasets
-
-Here is a description of the datasets:
-
-| Dataset | Rules | # Nodes | # Edges | # Relations | # Classes | # Train | # Valid | # Test |
-|---------|-------------|---------|---------|-------------|-----------|---------|---------|--------|
-|syn-paths|-|-|-|-| - |-|-|-|
-|syn-tipr|-|-|-|-|-|-|-|-|
-|syn-type|-|-|-|-|-|-|-|-|
-|syn-nl|-|-|-|-|-|-|-|-|
-|wd-movies|-|-|-|-|-|-|-|-|
-|wd-articles|-|-|-|-|-|-|-|-|
-
-## Example
-
-<table>
-  <tr>
-    <th>Dataset</th>
-    <th>Knowledge Graph</th>
-  </tr>
-  <tr>
-    <td>syn-paths</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-  <tr>
-    <td>syn-tipr</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-  <tr>
-    <td>syn-types</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-</table>
-
-## Installation
-
-To install IntelliGraphs locally, simply:
-
-```bash
-pip install -e .
-```
-
 ## Usage
 
 Here's a brief example of how to use various features of the IntelliGraphs library:
 
 ```python
 from intelligraphs import IntelliGraphs
 
@@ -144,14 +106,62 @@
 intelligraph.save_splits(filename='example', file_path='output', zip_compression=False)
 
 # Save the graphs and splits to zip compressed text files
 intelligraph.save_graphs(filename='example', file_path='output', zip_compression=True)
 intelligraph.save_splits(filename='example', file_path='output', zip_compression=True)
 ```
 
+## Datasets
+
+Here is a description of the datasets:
+
+| Dataset | Rules | # Nodes | # Edges | # Relations | # Classes | # Train | # Valid | # Test |
+|---------|-------------|---------|---------|-------------|-----------|---------|---------|--------|
+|syn-paths|-|-|-|-| - |-|-|-|
+|syn-tipr|-|-|-|-|-|-|-|-|
+|syn-type|-|-|-|-|-|-|-|-|
+|syn-nl|-|-|-|-|-|-|-|-|
+|wd-movies|-|-|-|-|-|-|-|-|
+|wd-articles|-|-|-|-|-|-|-|-|
+
+## Example
+
+<table>
+  <tr>
+    <th>Dataset</th>
+    <th>Knowledge Graph</th>
+  </tr>
+  <tr>
+    <td>syn-paths</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>syn-tipr</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>syn-types</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>wd-movies</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>wd-articles</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+</table>
+    
+    
 ## First-Order Logic
 
 First-order logic (FOL) is a logic system that is used to describe the world around us. It is a formal language that
 allows us to make statements about the world.
 
 Statements in FOL are made up of two parts: the subject and the predicate. The subject is the thing that is being
 described, and the predicate is the property of the subject. For example, the statement "John is a student" has the
```

### Comparing `intelligraphs-0.1.0/README.md` & `intelligraphs-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,46 @@
 <p  align="center">
-    <img src="images/IntelliGraph-logo.png" width="450px;" style="max-width: 100%;  margin-right:10px;">
+    <img src="https://raw.githubusercontent.com/thiviyanT/IntelliGraphs/main/images/IntelliGraph-logo.png?token=GHSAT0AAAAAAB5H4DZTLA4DT3TVAZXVWXPCZBWYCDA" width="450px;" style="max-width: 100%;  margin-right:10px;">
 <p>
 
 ---
 
-IntelliGraphs is a library that generates a collection of datasets for benchmarking generative models for knowledge
-graphs. These are graphs that are generated according to first order logic rules. These datasets are intended to be used
+[![PyPI Latest Release](https://img.shields.io/pypi/v/intelligraphs.svg)]([https://pypi.org/project/pandas/](https://pypi.org/project/intelligraphs/))
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+IntelliGraphs is a Python package that generates a collection of benchmark datasets. These datasets are intended to be used
 for benchmarking machine learning models under transductive settings. It can also be used as a testbed for developing
-new generative models. This library was designed to be extendable to create new synthetic datasets with other custom 
-First-Order Logical (FOL) constraints.
+new generative models. This library was designed to be extendable to create new synthetic datasets with custom 
+First-Order Logical (FOL) rules.
 
 ### TODO
 
 * Ask Paul: Do we want to register this with Zenodo. If so, add DOI badge here.
 * Ask Paul: How to generate dataset metadata? Is it needed?
 * Ask Paul: When to register dataset? Before or after publication?
 * Ask Paul: Where to put the dataset so that it lasts? (Zenodo, GitHub, etc.)
 * Ask Peter/Paul: Do we want to make it available on PyPI? If so, add badge here.
 * Make GitHub repo anonymous before submission
 
+## Installation
+
+To install IntelliGraphs locally, simply:
+
+```bash
+pip install intelligraphs
+```
+
 ## Advantages
 
 * Easy to use: Generate and manipulate Knowledge Graphs with a simple and clean Python API.
 * Flexible: Customize the number of graphs, triples, and data splits.
 * Extendable: Create more graphs according to custom FOL rules.
 * Efficient: Fast and memory-efficient graph generation and manipulation using native Python data structures.
 * Visualization: Visualize Knowledge Graphs.
 
-## Datasets
-
-Here is a description of the datasets:
-
-| Dataset | Rules | # Nodes | # Edges | # Relations | # Classes | # Train | # Valid | # Test |
-|---------|-------------|---------|---------|-------------|-----------|---------|---------|--------|
-|syn-paths|-|-|-|-| - |-|-|-|
-|syn-tipr|-|-|-|-|-|-|-|-|
-|syn-type|-|-|-|-|-|-|-|-|
-|syn-nl|-|-|-|-|-|-|-|-|
-|wd-movies|-|-|-|-|-|-|-|-|
-|wd-articles|-|-|-|-|-|-|-|-|
-
-## Example
-
-<table>
-  <tr>
-    <th>Dataset</th>
-    <th>Knowledge Graph</th>
-  </tr>
-  <tr>
-    <td>syn-paths</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-  <tr>
-    <td>syn-tipr</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-  <tr>
-    <td>syn-types</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-</table>
-
-## Installation
-
-To install IntelliGraphs locally, simply:
-
-```bash
-pip install -e .
-```
-
 ## Usage
 
 Here's a brief example of how to use various features of the IntelliGraphs library:
 
 ```python
 from intelligraphs import IntelliGraphs
 
@@ -125,14 +87,62 @@
 intelligraph.save_splits(filename='example', file_path='output', zip_compression=False)
 
 # Save the graphs and splits to zip compressed text files
 intelligraph.save_graphs(filename='example', file_path='output', zip_compression=True)
 intelligraph.save_splits(filename='example', file_path='output', zip_compression=True)
 ```
 
+## Datasets
+
+Here is a description of the datasets:
+
+| Dataset | Rules | # Nodes | # Edges | # Relations | # Classes | # Train | # Valid | # Test |
+|---------|-------------|---------|---------|-------------|-----------|---------|---------|--------|
+|syn-paths|-|-|-|-| - |-|-|-|
+|syn-tipr|-|-|-|-|-|-|-|-|
+|syn-type|-|-|-|-|-|-|-|-|
+|syn-nl|-|-|-|-|-|-|-|-|
+|wd-movies|-|-|-|-|-|-|-|-|
+|wd-articles|-|-|-|-|-|-|-|-|
+
+## Example
+
+<table>
+  <tr>
+    <th>Dataset</th>
+    <th>Knowledge Graph</th>
+  </tr>
+  <tr>
+    <td>syn-paths</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>syn-tipr</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>syn-types</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>wd-movies</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>wd-articles</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+</table>
+    
+    
 ## First-Order Logic
 
 First-order logic (FOL) is a logic system that is used to describe the world around us. It is a formal language that
 allows us to make statements about the world.
 
 Statements in FOL are made up of two parts: the subject and the predicate. The subject is the thing that is being
 described, and the predicate is the property of the subject. For example, the statement "John is a student" has the
```

### Comparing `intelligraphs-0.1.0/intelligraphs.egg-info/PKG-INFO` & `intelligraphs-0.1.1/intelligraphs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelligraphs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library to generate synthetic Knowledge Graphs using random triples.
 Home-page: https://github.com/thiviyanT/intelligraphs
 Author: Thiviyan Thanapalasingam
 Author-email: thiviyan.t@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,90 +14,52 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p  align="center">
-    <img src="images/IntelliGraph-logo.png" width="450px;" style="max-width: 100%;  margin-right:10px;">
+    <img src="https://raw.githubusercontent.com/thiviyanT/IntelliGraphs/main/images/IntelliGraph-logo.png?token=GHSAT0AAAAAAB5H4DZTLA4DT3TVAZXVWXPCZBWYCDA" width="450px;" style="max-width: 100%;  margin-right:10px;">
 <p>
 
 ---
 
-IntelliGraphs is a library that generates a collection of datasets for benchmarking generative models for knowledge
-graphs. These are graphs that are generated according to first order logic rules. These datasets are intended to be used
+[![PyPI Latest Release](https://img.shields.io/pypi/v/intelligraphs.svg)]([https://pypi.org/project/pandas/](https://pypi.org/project/intelligraphs/))
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+IntelliGraphs is a Python package that generates a collection of benchmark datasets. These datasets are intended to be used
 for benchmarking machine learning models under transductive settings. It can also be used as a testbed for developing
-new generative models. This library was designed to be extendable to create new synthetic datasets with other custom 
-First-Order Logical (FOL) constraints.
+new generative models. This library was designed to be extendable to create new synthetic datasets with custom 
+First-Order Logical (FOL) rules.
 
 ### TODO
 
 * Ask Paul: Do we want to register this with Zenodo. If so, add DOI badge here.
 * Ask Paul: How to generate dataset metadata? Is it needed?
 * Ask Paul: When to register dataset? Before or after publication?
 * Ask Paul: Where to put the dataset so that it lasts? (Zenodo, GitHub, etc.)
 * Ask Peter/Paul: Do we want to make it available on PyPI? If so, add badge here.
 * Make GitHub repo anonymous before submission
 
+## Installation
+
+To install IntelliGraphs locally, simply:
+
+```bash
+pip install intelligraphs
+```
+
 ## Advantages
 
 * Easy to use: Generate and manipulate Knowledge Graphs with a simple and clean Python API.
 * Flexible: Customize the number of graphs, triples, and data splits.
 * Extendable: Create more graphs according to custom FOL rules.
 * Efficient: Fast and memory-efficient graph generation and manipulation using native Python data structures.
 * Visualization: Visualize Knowledge Graphs.
 
-## Datasets
-
-Here is a description of the datasets:
-
-| Dataset | Rules | # Nodes | # Edges | # Relations | # Classes | # Train | # Valid | # Test |
-|---------|-------------|---------|---------|-------------|-----------|---------|---------|--------|
-|syn-paths|-|-|-|-| - |-|-|-|
-|syn-tipr|-|-|-|-|-|-|-|-|
-|syn-type|-|-|-|-|-|-|-|-|
-|syn-nl|-|-|-|-|-|-|-|-|
-|wd-movies|-|-|-|-|-|-|-|-|
-|wd-articles|-|-|-|-|-|-|-|-|
-
-## Example
-
-<table>
-  <tr>
-    <th>Dataset</th>
-    <th>Knowledge Graph</th>
-  </tr>
-  <tr>
-    <td>syn-paths</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-  <tr>
-    <td>syn-tipr</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-  <tr>
-    <td>syn-types</td>
-    <td><pre>
-Element_1 has_shape octagon.
-    </pre></td>
-  </tr>
-</table>
-
-## Installation
-
-To install IntelliGraphs locally, simply:
-
-```bash
-pip install -e .
-```
-
 ## Usage
 
 Here's a brief example of how to use various features of the IntelliGraphs library:
 
 ```python
 from intelligraphs import IntelliGraphs
 
@@ -144,14 +106,62 @@
 intelligraph.save_splits(filename='example', file_path='output', zip_compression=False)
 
 # Save the graphs and splits to zip compressed text files
 intelligraph.save_graphs(filename='example', file_path='output', zip_compression=True)
 intelligraph.save_splits(filename='example', file_path='output', zip_compression=True)
 ```
 
+## Datasets
+
+Here is a description of the datasets:
+
+| Dataset | Rules | # Nodes | # Edges | # Relations | # Classes | # Train | # Valid | # Test |
+|---------|-------------|---------|---------|-------------|-----------|---------|---------|--------|
+|syn-paths|-|-|-|-| - |-|-|-|
+|syn-tipr|-|-|-|-|-|-|-|-|
+|syn-type|-|-|-|-|-|-|-|-|
+|syn-nl|-|-|-|-|-|-|-|-|
+|wd-movies|-|-|-|-|-|-|-|-|
+|wd-articles|-|-|-|-|-|-|-|-|
+
+## Example
+
+<table>
+  <tr>
+    <th>Dataset</th>
+    <th>Knowledge Graph</th>
+  </tr>
+  <tr>
+    <td>syn-paths</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>syn-tipr</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>syn-types</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>wd-movies</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+  <tr>
+    <td>wd-articles</td>
+    <td><pre>
+    </pre></td>
+  </tr>
+</table>
+    
+    
 ## First-Order Logic
 
 First-order logic (FOL) is a logic system that is used to describe the world around us. It is a formal language that
 allows us to make statements about the world.
 
 Statements in FOL are made up of two parts: the subject and the predicate. The subject is the thing that is being
 described, and the predicate is the property of the subject. For example, the statement "John is a student" has the
```

### Comparing `intelligraphs-0.1.0/setup.py` & `intelligraphs-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="intelligraphs",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         'tqdm',
         'bokeh',
         'graphviz',
     ],
     author="Thiviyan Thanapalasingam",
```

