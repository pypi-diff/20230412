# Comparing `tmp/quantfreedom-0.0.3.tar.gz` & `tmp/quantfreedom-0.0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfreedom-0.0.3.tar", last modified: Wed Apr 12 01:24:19 2023, max compression
+gzip compressed data, was "quantfreedom-0.0.3.post1.tar", last modified: Wed Apr 12 13:48:15 2023, max compression
```

## Comparing `quantfreedom-0.0.3.tar` & `quantfreedom-0.0.3.post1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.391476 quantfreedom-0.0.3/
--rw-rw-rw-   0        0        0    11558 2023-03-29 16:20:45.000000 quantfreedom-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9399 2023-04-12 01:24:19.390475 quantfreedom-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8179 2023-03-31 02:51:25.000000 quantfreedom-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.354789 quantfreedom-0.0.3/quantfreedom/
--rw-rw-rw-   0        0        0      701 2023-04-11 17:50:38.000000 quantfreedom-0.0.3/quantfreedom/__init__.py
--rw-rw-rw-   0        0        0    15199 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/_doc_test.py
--rw-rw-rw-   0        0        0    10209 2023-04-11 17:59:26.000000 quantfreedom-0.0.3/quantfreedom/_testing.py
--rw-rw-rw-   0        0        0      946 2023-04-09 19:14:42.000000 quantfreedom-0.0.3/quantfreedom/_typing.py
--rw-rw-rw-   0        0        0       24 2023-04-12 01:20:01.000000 quantfreedom-0.0.3/quantfreedom/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.374563 quantfreedom-0.0.3/quantfreedom/base/
--rw-rw-rw-   0        0        0       38 2023-03-30 14:02:24.000000 quantfreedom-0.0.3/quantfreedom/base/__init__.py
--rw-rw-rw-   0        0        0    12170 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/base/base.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.375552 quantfreedom-0.0.3/quantfreedom/data/
--rw-rw-rw-   0        0        0       31 2023-04-11 19:21:38.000000 quantfreedom-0.0.3/quantfreedom/data/__init__.py
--rw-rw-rw-   0        0        0     7417 2023-04-11 19:13:23.000000 quantfreedom-0.0.3/quantfreedom/data/data_dl.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.377552 quantfreedom-0.0.3/quantfreedom/enums/
--rw-rw-rw-   0        0        0       40 2023-03-30 14:02:24.000000 quantfreedom-0.0.3/quantfreedom/enums/__init__.py
--rw-rw-rw-   0        0        0     8082 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/enums/enums.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.378553 quantfreedom-0.0.3/quantfreedom/evaluators/
--rw-rw-rw-   0        0        0       50 2023-03-30 14:02:24.000000 quantfreedom-0.0.3/quantfreedom/evaluators/__init__.py
--rw-rw-rw-   0        0        0    31974 2023-04-11 19:23:01.000000 quantfreedom-0.0.3/quantfreedom/evaluators/evaluators.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.380554 quantfreedom-0.0.3/quantfreedom/indicators/
--rw-rw-rw-   0        0        0       49 2023-04-11 19:23:10.000000 quantfreedom-0.0.3/quantfreedom/indicators/__init__.py
--rw-rw-rw-   0        0        0    15760 2023-04-11 18:18:08.000000 quantfreedom-0.0.3/quantfreedom/indicators/talib_ind.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.384478 quantfreedom-0.0.3/quantfreedom/nb/
--rw-rw-rw-   0        0        0      212 2023-03-30 14:02:23.000000 quantfreedom-0.0.3/quantfreedom/nb/__init__.py
--rw-rw-rw-   0        0        0    16293 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/buy_funcs.py
--rw-rw-rw-   0        0        0    12476 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/execute_funcs.py
--rw-rw-rw-   0        0        0    28820 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/helper_funcs.py
--rw-rw-rw-   0        0        0    16308 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/sell_funcs.py
--rw-rw-rw-   0        0        0    27311 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/simulate.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.388475 quantfreedom-0.0.3/quantfreedom/plotting/
--rw-rw-rw-   0        0        0       49 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/__init__.py
--rw-rw-rw-   0        0        0    10761 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/plot_helper_functions.py
--rw-rw-rw-   0        0        0     8294 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/plotting_main.py
--rw-rw-rw-   0        0        0    13294 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/replay.py
--rw-rw-rw-   0        0        0        0 2023-04-02 21:46:09.000000 quantfreedom-0.0.3/quantfreedom/plotting/temp.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.389475 quantfreedom-0.0.3/quantfreedom/utils/
--rw-rw-rw-   0        0        0      117 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/utils/__init__.py
--rw-rw-rw-   0        0        0     3012 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/utils/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.372549 quantfreedom-0.0.3/quantfreedom.egg-info/
--rw-rw-rw-   0        0        0     9399 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      606 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 01:24:19.391476 quantfreedom-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2784 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.467898 quantfreedom-0.0.3.post1/
+-rw-rw-rw-   0        0        0    11558 2023-03-29 16:20:45.000000 quantfreedom-0.0.3.post1/LICENSE
+-rw-rw-rw-   0        0        0     9405 2023-04-12 13:48:15.467898 quantfreedom-0.0.3.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     8179 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.440553 quantfreedom-0.0.3.post1/quantfreedom/
+-rw-rw-rw-   0        0        0      701 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/__init__.py
+-rw-rw-rw-   0        0        0    15199 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/_doc_test.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/_testing.py
+-rw-rw-rw-   0        0        0      946 2023-04-09 19:14:42.000000 quantfreedom-0.0.3.post1/quantfreedom/_typing.py
+-rw-rw-rw-   0        0        0       28 2023-04-12 13:47:55.000000 quantfreedom-0.0.3.post1/quantfreedom/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.452367 quantfreedom-0.0.3.post1/quantfreedom/base/
+-rw-rw-rw-   0        0        0       38 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/base/__init__.py
+-rw-rw-rw-   0        0        0    12170 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/base/base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.454383 quantfreedom-0.0.3.post1/quantfreedom/data/
+-rw-rw-rw-   0        0        0       31 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/data/__init__.py
+-rw-rw-rw-   0        0        0     7417 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/data/data_dl.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.455368 quantfreedom-0.0.3.post1/quantfreedom/enums/
+-rw-rw-rw-   0        0        0       40 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/enums/__init__.py
+-rw-rw-rw-   0        0        0     8082 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/enums/enums.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.456368 quantfreedom-0.0.3.post1/quantfreedom/evaluators/
+-rw-rw-rw-   0        0        0       50 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/evaluators/__init__.py
+-rw-rw-rw-   0        0        0    31974 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/evaluators/evaluators.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.458378 quantfreedom-0.0.3.post1/quantfreedom/indicators/
+-rw-rw-rw-   0        0        0       49 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/indicators/__init__.py
+-rw-rw-rw-   0        0        0    15760 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/indicators/talib_ind.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.462196 quantfreedom-0.0.3.post1/quantfreedom/nb/
+-rw-rw-rw-   0        0        0      212 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/nb/__init__.py
+-rw-rw-rw-   0        0        0    16293 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/nb/buy_funcs.py
+-rw-rw-rw-   0        0        0    12476 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/nb/execute_funcs.py
+-rw-rw-rw-   0        0        0    28820 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/nb/helper_funcs.py
+-rw-rw-rw-   0        0        0    16308 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/nb/sell_funcs.py
+-rw-rw-rw-   0        0        0    27311 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/nb/simulate.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.465197 quantfreedom-0.0.3.post1/quantfreedom/plotting/
+-rw-rw-rw-   0        0        0       49 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/plotting/__init__.py
+-rw-rw-rw-   0        0        0    10761 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/plotting/plot_helper_functions.py
+-rw-rw-rw-   0        0        0     8294 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/plotting/plotting_main.py
+-rw-rw-rw-   0        0        0    13294 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/plotting/replay.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/plotting/temp.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.467197 quantfreedom-0.0.3.post1/quantfreedom/utils/
+-rw-rw-rw-   0        0        0      117 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/utils/__init__.py
+-rw-rw-rw-   0        0        0     3012 2023-04-12 13:30:57.000000 quantfreedom-0.0.3.post1/quantfreedom/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:48:15.451367 quantfreedom-0.0.3.post1/quantfreedom.egg-info/
+-rw-rw-rw-   0        0        0     9405 2023-04-12 13:48:15.000000 quantfreedom-0.0.3.post1/quantfreedom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-04-12 13:48:15.000000 quantfreedom-0.0.3.post1/quantfreedom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:48:15.000000 quantfreedom-0.0.3.post1/quantfreedom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      600 2023-04-12 13:48:15.000000 quantfreedom-0.0.3.post1/quantfreedom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 13:48:15.000000 quantfreedom-0.0.3.post1/quantfreedom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 13:48:15.467898 quantfreedom-0.0.3.post1/setup.cfg
+-rw-rw-rw-   0        0        0     2766 2023-04-12 13:35:49.000000 quantfreedom-0.0.3.post1/setup.py
```

### Comparing `quantfreedom-0.0.3/LICENSE` & `quantfreedom-0.0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/PKG-INFO` & `quantfreedom-0.0.3.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfreedom
-Version: 0.0.3
+Version: 0.0.3.post1
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/QuantFreedom1022/quantfreedom
 Author: Quant Freedom
 Author-email: QuantFreedom1022@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quantfreedom-0.0.3/README.md` & `quantfreedom-0.0.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/__init__.py` & `quantfreedom-0.0.3.post1/quantfreedom/__init__.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/_doc_test.py` & `quantfreedom-0.0.3.post1/quantfreedom/_doc_test.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/_typing.py` & `quantfreedom-0.0.3.post1/quantfreedom/_typing.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/base/base.py` & `quantfreedom-0.0.3.post1/quantfreedom/base/base.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/data/data_dl.py` & `quantfreedom-0.0.3.post1/quantfreedom/data/data_dl.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/enums/enums.py` & `quantfreedom-0.0.3.post1/quantfreedom/enums/enums.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/evaluators/evaluators.py` & `quantfreedom-0.0.3.post1/quantfreedom/evaluators/evaluators.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/indicators/talib_ind.py` & `quantfreedom-0.0.3.post1/quantfreedom/indicators/talib_ind.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/nb/buy_funcs.py` & `quantfreedom-0.0.3.post1/quantfreedom/nb/buy_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/nb/execute_funcs.py` & `quantfreedom-0.0.3.post1/quantfreedom/nb/execute_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/nb/helper_funcs.py` & `quantfreedom-0.0.3.post1/quantfreedom/nb/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/nb/sell_funcs.py` & `quantfreedom-0.0.3.post1/quantfreedom/nb/sell_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/nb/simulate.py` & `quantfreedom-0.0.3.post1/quantfreedom/nb/simulate.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/plotting/plot_helper_functions.py` & `quantfreedom-0.0.3.post1/quantfreedom/plotting/plot_helper_functions.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/plotting/plotting_main.py` & `quantfreedom-0.0.3.post1/quantfreedom/plotting/plotting_main.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/plotting/replay.py` & `quantfreedom-0.0.3.post1/quantfreedom/plotting/replay.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom/utils/helpers.py` & `quantfreedom-0.0.3.post1/quantfreedom/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom.egg-info/PKG-INFO` & `quantfreedom-0.0.3.post1/quantfreedom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfreedom
-Version: 0.0.3
+Version: 0.0.3.post1
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/QuantFreedom1022/quantfreedom
 Author: Quant Freedom
 Author-email: QuantFreedom1022@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quantfreedom-0.0.3/quantfreedom.egg-info/SOURCES.txt` & `quantfreedom-0.0.3.post1/quantfreedom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.3/quantfreedom.egg-info/requires.txt` & `quantfreedom-0.0.3.post1/quantfreedom.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 mypy_extensions
 notebook
 tqdm
 numpy>=1.16.5
 pandas
 polars
 pyarrow
-pybit
 tables
 
 [:python_version < "3.10"]
 numba>=0.53.1
 
 [:python_version < "3.8"]
 typing_extensions
```

### Comparing `quantfreedom-0.0.3/setup.py` & `quantfreedom-0.0.3.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         "tqdm",
         'numba>=0.53.1; python_version < "3.10"',
         'numba>=0.56.0; python_version >= "3.10"',
         "numpy>=1.16.5",
         "pandas",
         "polars",
         "pyarrow",
-        "pybit",
         "tables",
         'typing_extensions; python_version < "3.8"',
     ],
     extras_require={
         "web": [
             "Markdown",
             "PyYAML",
```

