# Comparing `tmp/qudi_hira_analysis-1.3.4.tar.gz` & `tmp/qudi_hira_analysis-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qudi_hira_analysis-1.3.4.tar", max compression
+gzip compressed data, was "qudi_hira_analysis-1.3.5.tar", max compression
```

## Comparing `qudi_hira_analysis-1.3.4.tar` & `qudi_hira_analysis-1.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.3.4/LICENSE
--rw-r--r--   0        0        0     9531 2023-04-12 17:44:20.350633 qudi_hira_analysis-1.3.4/README.md
--rw-r--r--   0        0        0      868 2023-04-12 17:46:50.500495 qudi_hira_analysis-1.3.4/pyproject.toml
--rw-r--r--   0        0        0      171 2023-03-05 21:19:20.709702 qudi_hira_analysis-1.3.4/qudi_hira_analysis/__init__.py
--rw-r--r--   0        0        0    10745 2023-03-05 21:19:20.709832 qudi_hira_analysis-1.3.4/qudi_hira_analysis/analysis_logic.py
--rw-r--r--   0        0        0    13322 2023-03-09 12:03:13.046866 qudi_hira_analysis-1.3.4/qudi_hira_analysis/data_handler.py
--rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/antibunchingmethods.py
--rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/decaylikemethods.py
--rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
--rw-r--r--   0        0        0    23150 2023-03-05 21:19:20.711989 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/generalmethods.py
--rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
--rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/linearmethods.py
--rw-r--r--   0        0        0    41457 2023-03-05 21:19:20.712635 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
--rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
--rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/sinemethods.py
--rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.3.4/qudi_hira_analysis/helper_functions.py
--rw-r--r--   0        0        0    12696 2023-04-12 17:43:42.063710 qudi_hira_analysis-1.3.4/qudi_hira_analysis/io_handler.py
--rw-r--r--   0        0        0     6758 2023-04-12 17:43:42.063880 qudi_hira_analysis-1.3.4/qudi_hira_analysis/measurement_dataclass.py
--rw-r--r--   0        0        0    18729 2023-03-05 21:19:20.714069 qudi_hira_analysis-1.3.4/qudi_hira_analysis/qudi_fit_logic.py
--rw-r--r--   0        0        0    10570 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.3.5/LICENSE
+-rw-r--r--   0        0        0     9531 2023-04-12 17:44:20.350633 qudi_hira_analysis-1.3.5/README.md
+-rw-r--r--   0        0        0      868 2023-04-12 17:54:57.241605 qudi_hira_analysis-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-03-05 21:19:20.709702 qudi_hira_analysis-1.3.5/qudi_hira_analysis/__init__.py
+-rw-r--r--   0        0        0    10745 2023-03-05 21:19:20.709832 qudi_hira_analysis-1.3.5/qudi_hira_analysis/analysis_logic.py
+-rw-r--r--   0        0        0    13322 2023-03-09 12:03:13.046866 qudi_hira_analysis-1.3.5/qudi_hira_analysis/data_handler.py
+-rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/__init__.py
+-rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/antibunchingmethods.py
+-rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/decaylikemethods.py
+-rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
+-rw-r--r--   0        0        0    23150 2023-03-05 21:19:20.711989 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/generalmethods.py
+-rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
+-rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/linearmethods.py
+-rw-r--r--   0        0        0    41457 2023-03-05 21:19:20.712635 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
+-rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
+-rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/sinemethods.py
+-rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.3.5/qudi_hira_analysis/helper_functions.py
+-rw-r--r--   0        0        0    12696 2023-04-12 17:43:42.063710 qudi_hira_analysis-1.3.5/qudi_hira_analysis/io_handler.py
+-rw-r--r--   0        0        0     6758 2023-04-12 17:43:42.063880 qudi_hira_analysis-1.3.5/qudi_hira_analysis/measurement_dataclass.py
+-rw-r--r--   0        0        0    18729 2023-03-05 21:19:20.714069 qudi_hira_analysis-1.3.5/qudi_hira_analysis/qudi_fit_logic.py
+-rw-r--r--   0        0        0    10529 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.3.5/PKG-INFO
```

### Comparing `qudi_hira_analysis-1.3.4/LICENSE` & `qudi_hira_analysis-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/README.md` & `qudi_hira_analysis-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/pyproject.toml` & `qudi_hira_analysis-1.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qudi-hira-analysis"
-version = "1.3.4"
+version = "1.3.5"
 repository = "https://github.com/dineshpinto/qudi-hira-analysis"
 homepage = "https://github.com/dineshpinto/qudi-hira-analysis"
 keywords = ["python", "qubit", "analysis", "nv centers", "photon timetrace"]
 description = "A Python toolkit to analzye photon timetrace data from qubit sensors"
 authors = ["dineshpinto <annual.fallout_0z@icloud.com>"]
 license = "MIT"
 readme = "README.md"
@@ -15,17 +15,17 @@
 lmfit = "^1.1.0"
 matplotlib = "^3.6.2"
 numpy = "^1.24.0"
 pandas = "^2.0.0"
 xlrd = "^2.0.1"
 openpyxl = "^3.0.10"
 tqdm = "^4.64.1"
-notebook = "^6.5.3"
 pyspm = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 seaborn = "^0.12.2"
 jupyterlab = "^3.6.2"
+notebook = "^6.5.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/analysis_logic.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/analysis_logic.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/data_handler.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/data_handler.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/antibunchingmethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/antibunchingmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/decaylikemethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/decaylikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/gaussianlikemethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/gaussianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/generalmethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/generalmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/linearmethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/linearmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/poissonianlikemethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/poissonianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/fitmethods/sinemethods.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/sinemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/helper_functions.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/io_handler.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/io_handler.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/measurement_dataclass.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/measurement_dataclass.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/qudi_hira_analysis/qudi_fit_logic.py` & `qudi_hira_analysis-1.3.5/qudi_hira_analysis/qudi_fit_logic.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.4/PKG-INFO` & `qudi_hira_analysis-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: qudi-hira-analysis
-Version: 1.3.4
+Version: 1.3.5
 Summary: A Python toolkit to analzye photon timetrace data from qubit sensors
 Home-page: https://github.com/dineshpinto/qudi-hira-analysis
 License: MIT
 Keywords: python,qubit,analysis,nv centers,photon timetrace
 Author: dineshpinto
 Author-email: annual.fallout_0z@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lmfit (>=1.1.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: notebook (>=6.5.3,<7.0.0)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pyspm (>=0.3.0,<0.4.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/dineshpinto/qudi-hira-analysis
```

