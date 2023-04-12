# Comparing `tmp/pykrack-0.0.1.tar.gz` & `tmp/pykrack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrack-0.0.1.tar", last modified: Wed Apr 12 12:53:09 2023, max compression
+gzip compressed data, was "pykrack-0.0.2.tar", last modified: Wed Apr 12 14:09:59 2023, max compression
```

## Comparing `pykrack-0.0.1.tar` & `pykrack-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 12:53:09.805880 pykrack-0.0.1/
--rw-rw-r--   0 ferran    (1000) ferran    (1000)    11337 2023-01-20 02:50:04.000000 pykrack-0.0.1/LICENSE
--rw-rw-r--   0 ferran    (1000) ferran    (1000)      111 2023-01-20 02:50:04.000000 pykrack-0.0.1/MANIFEST.in
--rw-r--r--   0 ferran    (1000) ferran    (1000)     3479 2023-04-12 12:53:09.805880 pykrack-0.0.1/PKG-INFO
--rw-r--r--   0 ferran    (1000) ferran    (1000)     2687 2023-04-12 12:16:46.000000 pykrack-0.0.1/README.md
-drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 12:53:09.803880 pykrack-0.0.1/pykrack/
--rw-r--r--   0 ferran    (1000) ferran    (1000)       22 2023-04-12 12:48:08.000000 pykrack-0.0.1/pykrack/__init__.py
--rw-r--r--   0 ferran    (1000) ferran    (1000)      524 2023-04-12 12:48:08.000000 pykrack-0.0.1/pykrack/_modidx.py
--rw-r--r--   0 ferran    (1000) ferran    (1000)      800 2023-04-12 12:48:08.000000 pykrack-0.0.1/pykrack/core.py
--rw-r--r--   0 ferran    (1000) ferran    (1000)     2721 2023-04-12 12:48:08.000000 pykrack-0.0.1/pykrack/hierarchy.py
-drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 12:53:09.804880 pykrack-0.0.1/pykrack.egg-info/
--rw-r--r--   0 ferran    (1000) ferran    (1000)     3479 2023-04-12 12:53:09.000000 pykrack-0.0.1/pykrack.egg-info/PKG-INFO
--rw-r--r--   0 ferran    (1000) ferran    (1000)      345 2023-04-12 12:53:09.000000 pykrack-0.0.1/pykrack.egg-info/SOURCES.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)        1 2023-04-12 12:53:09.000000 pykrack-0.0.1/pykrack.egg-info/dependency_links.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)       36 2023-04-12 12:53:09.000000 pykrack-0.0.1/pykrack.egg-info/entry_points.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)        1 2023-04-04 13:10:52.000000 pykrack-0.0.1/pykrack.egg-info/not-zip-safe
--rw-r--r--   0 ferran    (1000) ferran    (1000)       65 2023-04-12 12:53:09.000000 pykrack-0.0.1/pykrack.egg-info/requires.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)        8 2023-04-12 12:53:09.000000 pykrack-0.0.1/pykrack.egg-info/top_level.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)     1316 2023-04-04 13:32:05.000000 pykrack-0.0.1/settings.ini
--rw-r--r--   0 ferran    (1000) ferran    (1000)       38 2023-04-12 12:53:09.805880 pykrack-0.0.1/setup.cfg
--rw-rw-r--   0 ferran    (1000) ferran    (1000)     2560 2023-01-20 02:50:04.000000 pykrack-0.0.1/setup.py
+drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 14:09:59.191664 pykrack-0.0.2/
+-rw-rw-r--   0 ferran    (1000) ferran    (1000)    11337 2023-01-20 02:50:04.000000 pykrack-0.0.2/LICENSE
+-rw-rw-r--   0 ferran    (1000) ferran    (1000)      111 2023-01-20 02:50:04.000000 pykrack-0.0.2/MANIFEST.in
+-rw-r--r--   0 ferran    (1000) ferran    (1000)     3615 2023-04-12 14:09:59.190664 pykrack-0.0.2/PKG-INFO
+-rw-r--r--   0 ferran    (1000) ferran    (1000)     2823 2023-04-12 14:02:23.000000 pykrack-0.0.2/README.md
+drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 14:09:59.189664 pykrack-0.0.2/pykrack/
+-rw-r--r--   0 ferran    (1000) ferran    (1000)       22 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/__init__.py
+-rw-r--r--   0 ferran    (1000) ferran    (1000)      524 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/_modidx.py
+-rw-r--r--   0 ferran    (1000) ferran    (1000)      800 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/core.py
+-rw-r--r--   0 ferran    (1000) ferran    (1000)     2721 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/hierarchy.py
+drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 14:09:59.190664 pykrack-0.0.2/pykrack.egg-info/
+-rw-r--r--   0 ferran    (1000) ferran    (1000)     3615 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/PKG-INFO
+-rw-r--r--   0 ferran    (1000) ferran    (1000)      345 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/SOURCES.txt
+-rw-r--r--   0 ferran    (1000) ferran    (1000)        1 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/dependency_links.txt
+-rw-r--r--   0 ferran    (1000) ferran    (1000)       36 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/entry_points.txt
+-rw-r--r--   0 ferran    (1000) ferran    (1000)        1 2023-04-04 13:10:52.000000 pykrack-0.0.2/pykrack.egg-info/not-zip-safe
+-rw-r--r--   0 ferran    (1000) ferran    (1000)       34 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/requires.txt
+-rw-r--r--   0 ferran    (1000) ferran    (1000)        8 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/top_level.txt
+-rw-r--r--   0 ferran    (1000) ferran    (1000)      846 2023-04-12 14:06:42.000000 pykrack-0.0.2/settings.ini
+-rw-r--r--   0 ferran    (1000) ferran    (1000)       38 2023-04-12 14:09:59.191664 pykrack-0.0.2/setup.cfg
+-rw-rw-r--   0 ferran    (1000) ferran    (1000)     2560 2023-01-20 02:50:04.000000 pykrack-0.0.2/setup.py
```

### Comparing `pykrack-0.0.1/LICENSE` & `pykrack-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykrack-0.0.1/PKG-INFO` & `pykrack-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,34 @@
-Metadata-Version: 2.1
-Name: pykrack
-Version: 0.0.1
-Summary: Computing Krackhardt hierarchy score on netowrkX graphs
-Home-page: https://github.com/FerranC96/pykrack
-Author: FerranC96
-Author-email: ferricaro@hotmail.com
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # pyKrack
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
+## Install
+
+Due to the comparisons with the R package `sna` we recommend using conda
+to manage your environment.
 
-THIS IS CLEARLY STILL A WORK IN PROGRESS PROJECT
+1.  First create the pykrack conda environment from the environment.yml
+    file:
 
-## Install
+``` sh
+conda (or mamba) env create -f environment.yml
+```
+
+2.  Then load the conda environment with:
 
-Due to the comparisons with the r package sna We recommend using conda.
-Create an environment using the environment.yml file, load it and
-install/run the package.
+``` sh
+conda activate pykrack
+```
+
+3.  And finally install the package from pip via the following command:
+
+``` sh
+pip install pyKrack
+```
 
 Alternatively pyKrack can also be isntalled using pip via the following
 command
 
 ``` sh
 pip install pyKrack
 ```
```

#### html2text {}

```diff
@@ -1,34 +1,25 @@
-Metadata-Version: 2.1 Name: pykrack Version: 0.0.1 Summary: Computing
-Krackhardt hierarchy score on netowrkX graphs Home-page: https://github.com/
-FerranC96/pykrack Author: FerranC96 Author-email: ferricaro@hotmail.com
-License: Apache Software License 2.0 Keywords: nbdev jupyter notebook python
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
-Software License Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE # pyKrack  This file will become your
-README and also the index of your documentation. THIS IS CLEARLY STILL A WORK
-IN PROGRESS PROJECT ## Install Due to the comparisons with the r package sna We
-recommend using conda. Create an environment using the environment.yml file,
-load it and install/run the package. Alternatively pyKrack can also be
-isntalled using pip via the following command ``` sh pip install pyKrack ```
-Then install the R dependencies listed in the conda environmnet.yml manually.
-## How to use Please see the core and hierarchy notebooks for more detailed
-explanations. **pyKrack** consists of one main function, [`compute_hierarchy`]
-(https://FerranC96.github.io/pykrack/hierarchy.html#compute_hierarchy). -------
------------------------------------------------------------------ source ###
-compute_hierarchy > compute_hierarchy (G, metric='pykrack') Compute one of the
-possible hierarchy scores | | **Type** | **Default** | **Details** | |---------
-----|-----------|-------------|------------------------------------------------
+# pyKrack  ## Install Due to the comparisons with the R package `sna` we
+recommend using conda to manage your environment. 1. First create the pykrack
+conda environment from the environment.yml file: ``` sh conda (or mamba) env
+create -f environment.yml ``` 2. Then load the conda environment with: ``` sh
+conda activate pykrack ``` 3. And finally install the package from pip via the
+following command: ``` sh pip install pyKrack ``` Alternatively pyKrack can
+also be isntalled using pip via the following command ``` sh pip install
+pyKrack ``` Then install the R dependencies listed in the conda environmnet.yml
+manually. ## How to use Please see the core and hierarchy notebooks for more
+detailed explanations. **pyKrack** consists of one main function,
+[`compute_hierarchy`](https://FerranC96.github.io/pykrack/
+hierarchy.html#compute_hierarchy). --------------------------------------------
+---------------------------- source ### compute_hierarchy > compute_hierarchy
+(G, metric='pykrack') Compute one of the possible hierarchy scores | | **Type**
+| **Default** | **Details** | |-------------|-----------|-------------|--------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------| | G | | | Directed
-NetworkX graph | | metric | str | pykrack | Type of hierarchy metric to
-compute. Accepted types are:
+-------------------------------------------------------------------------------
+-------------------| | G | | | Directed NetworkX graph | | metric | str |
+pykrack | Type of hierarchy metric to compute. Accepted types are:
 âpykrackâ for this moduleâs implementation of the Krackhardt score.
 ârsnakrackâ for the sna implementation in R.
 âhierarchy_flowâ for the Luo and Magee 2011 as implemented in the NetworkX
 package. | | **Returns** | **float** | | **One of the possible hierarchy
 scores** |
```

### Comparing `pykrack-0.0.1/README.md` & `pykrack-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,56 @@
+Metadata-Version: 2.1
+Name: pykrack
+Version: 0.0.2
+Summary: Computing Krackhardt hierarchy score on netowrkX graphs
+Home-page: https://github.com/FerranC96/pykrack
+Author: FerranC96
+Author-email: ferricaro@hotmail.com
+License: Apache Software License 2.0
+Keywords: nbdev jupyter notebook python
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # pyKrack
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
+## Install
+
+Due to the comparisons with the R package `sna` we recommend using conda
+to manage your environment.
 
-THIS IS CLEARLY STILL A WORK IN PROGRESS PROJECT
+1.  First create the pykrack conda environment from the environment.yml
+    file:
 
-## Install
+``` sh
+conda (or mamba) env create -f environment.yml
+```
+
+2.  Then load the conda environment with:
 
-Due to the comparisons with the r package sna We recommend using conda.
-Create an environment using the environment.yml file, load it and
-install/run the package.
+``` sh
+conda activate pykrack
+```
+
+3.  And finally install the package from pip via the following command:
+
+``` sh
+pip install pyKrack
+```
 
 Alternatively pyKrack can also be isntalled using pip via the following
 command
 
 ``` sh
 pip install pyKrack
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,25 @@
-# pyKrack  This file will become your README and also the index of your
-documentation. THIS IS CLEARLY STILL A WORK IN PROGRESS PROJECT ## Install Due
-to the comparisons with the r package sna We recommend using conda. Create an
-environment using the environment.yml file, load it and install/run the
-package. Alternatively pyKrack can also be isntalled using pip via the
-following command ``` sh pip install pyKrack ``` Then install the R
+Metadata-Version: 2.1 Name: pykrack Version: 0.0.2 Summary: Computing
+Krackhardt hierarchy score on netowrkX graphs Home-page: https://github.com/
+FerranC96/pykrack Author: FerranC96 Author-email: ferricaro@hotmail.com
+License: Apache Software License 2.0 Keywords: nbdev jupyter notebook python
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Developers Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev License-File: LICENSE # pyKrack  ## Install Due to the
+comparisons with the R package `sna` we recommend using conda to manage your
+environment. 1. First create the pykrack conda environment from the
+environment.yml file: ``` sh conda (or mamba) env create -f environment.yml ```
+2. Then load the conda environment with: ``` sh conda activate pykrack ``` 3.
+And finally install the package from pip via the following command: ``` sh pip
+install pyKrack ``` Alternatively pyKrack can also be isntalled using pip via
+the following command ``` sh pip install pyKrack ``` Then install the R
 dependencies listed in the conda environmnet.yml manually. ## How to use Please
 see the core and hierarchy notebooks for more detailed explanations.
 **pyKrack** consists of one main function, [`compute_hierarchy`](https://
 FerranC96.github.io/pykrack/hierarchy.html#compute_hierarchy). ----------------
 -------------------------------------------------------- source ###
 compute_hierarchy > compute_hierarchy (G, metric='pykrack') Compute one of the
 possible hierarchy scores | | **Type** | **Default** | **Details** | |---------
```

### Comparing `pykrack-0.0.1/pykrack/_modidx.py` & `pykrack-0.0.2/pykrack/_modidx.py`

 * *Files identical despite different names*

### Comparing `pykrack-0.0.1/pykrack/core.py` & `pykrack-0.0.2/pykrack/core.py`

 * *Files identical despite different names*

### Comparing `pykrack-0.0.1/pykrack/hierarchy.py` & `pykrack-0.0.2/pykrack/hierarchy.py`

 * *Files identical despite different names*

### Comparing `pykrack-0.0.1/pykrack.egg-info/PKG-INFO` & `pykrack-0.0.2/pykrack.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykrack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Computing Krackhardt hierarchy score on netowrkX graphs
 Home-page: https://github.com/FerranC96/pykrack
 Author: FerranC96
 Author-email: ferricaro@hotmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -20,24 +20,37 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyKrack
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
+## Install
 
-THIS IS CLEARLY STILL A WORK IN PROGRESS PROJECT
+Due to the comparisons with the R package `sna` we recommend using conda
+to manage your environment.
 
-## Install
+1.  First create the pykrack conda environment from the environment.yml
+    file:
 
-Due to the comparisons with the r package sna We recommend using conda.
-Create an environment using the environment.yml file, load it and
-install/run the package.
+``` sh
+conda (or mamba) env create -f environment.yml
+```
+
+2.  Then load the conda environment with:
+
+``` sh
+conda activate pykrack
+```
+
+3.  And finally install the package from pip via the following command:
+
+``` sh
+pip install pyKrack
+```
 
 Alternatively pyKrack can also be isntalled using pip via the following
 command
 
 ``` sh
 pip install pyKrack
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 2.1 Name: pykrack Version: 0.0.1 Summary: Computing
+Metadata-Version: 2.1 Name: pykrack Version: 0.0.2 Summary: Computing
 Krackhardt hierarchy score on netowrkX graphs Home-page: https://github.com/
 FerranC96/pykrack Author: FerranC96 Author-email: ferricaro@hotmail.com
 License: Apache Software License 2.0 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE # pyKrack  This file will become your
-README and also the index of your documentation. THIS IS CLEARLY STILL A WORK
-IN PROGRESS PROJECT ## Install Due to the comparisons with the r package sna We
-recommend using conda. Create an environment using the environment.yml file,
-load it and install/run the package. Alternatively pyKrack can also be
-isntalled using pip via the following command ``` sh pip install pyKrack ```
-Then install the R dependencies listed in the conda environmnet.yml manually.
-## How to use Please see the core and hierarchy notebooks for more detailed
-explanations. **pyKrack** consists of one main function, [`compute_hierarchy`]
-(https://FerranC96.github.io/pykrack/hierarchy.html#compute_hierarchy). -------
------------------------------------------------------------------ source ###
+Provides-Extra: dev License-File: LICENSE # pyKrack  ## Install Due to the
+comparisons with the R package `sna` we recommend using conda to manage your
+environment. 1. First create the pykrack conda environment from the
+environment.yml file: ``` sh conda (or mamba) env create -f environment.yml ```
+2. Then load the conda environment with: ``` sh conda activate pykrack ``` 3.
+And finally install the package from pip via the following command: ``` sh pip
+install pyKrack ``` Alternatively pyKrack can also be isntalled using pip via
+the following command ``` sh pip install pyKrack ``` Then install the R
+dependencies listed in the conda environmnet.yml manually. ## How to use Please
+see the core and hierarchy notebooks for more detailed explanations.
+**pyKrack** consists of one main function, [`compute_hierarchy`](https://
+FerranC96.github.io/pykrack/hierarchy.html#compute_hierarchy). ----------------
+-------------------------------------------------------- source ###
 compute_hierarchy > compute_hierarchy (G, metric='pykrack') Compute one of the
 possible hierarchy scores | | **Type** | **Default** | **Details** | |---------
 ----|-----------|-------------|------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ----------------------------------------------------------| | G | | | Directed
 NetworkX graph | | metric | str | pykrack | Type of hierarchy metric to
```

### Comparing `pykrack-0.0.1/setup.py` & `pykrack-0.0.2/setup.py`

 * *Files identical despite different names*

