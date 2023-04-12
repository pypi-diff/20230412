# Comparing `tmp/portbt-0.1.2.tar.gz` & `tmp/portbt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portbt-0.1.2.tar", max compression
+gzip compressed data, was "portbt-0.1.3.tar", max compression
```

## Comparing `portbt-0.1.2.tar` & `portbt-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.2/portbt/__init__.py
--rw-r--r--   0        0        0     3139 2023-04-11 22:35:26.638321 portbt-0.1.2/portbt/backtest_functions.py
--rw-r--r--   0        0        0     1643 2023-04-12 02:22:47.006848 portbt-0.1.2/portbt/portfolio.py
--rw-r--r--   0        0        0      658 2023-04-11 22:15:59.356410 portbt-0.1.2/portbt/utils.py
--rw-r--r--   0        0        0      575 2023-04-12 02:38:04.522063 portbt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-12 02:39:37.960111 portbt-0.1.2/README.md
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 portbt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.3/portbt/__init__.py
+-rw-r--r--   0        0        0     3139 2023-04-12 03:01:01.868034 portbt-0.1.3/portbt/backtest_functions.py
+-rw-r--r--   0        0        0     1663 2023-04-12 03:03:15.656462 portbt-0.1.3/portbt/portfolio.py
+-rw-r--r--   0        0        0      658 2023-04-11 22:15:59.356410 portbt-0.1.3/portbt/utils.py
+-rw-r--r--   0        0        0      575 2023-04-12 03:08:12.542581 portbt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3747 2023-04-12 03:07:27.269246 portbt-0.1.3/README.md
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 portbt-0.1.3/PKG-INFO
```

### Comparing `portbt-0.1.2/LICENSE.txt` & `portbt-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `portbt-0.1.2/portbt/backtest_functions.py` & `portbt-0.1.3/portbt/backtest_functions.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.2/portbt/portfolio.py` & `portbt-0.1.3/portbt/portfolio.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pandas import DataFrame, Series
 
 from .backtest_functions import backtest_with_rebalance, backtest_without_rebalance
 
 
 class Backtest:
     def __init__(self):
-        self.prices: DataFrame | Series = pd.DataFrame()
+        # self.prices: DataFrame | Series = pd.DataFrame() # can delete this
         self.values: DataFrame | Series = pd.DataFrame()
         self.exposure: DataFrame | Series = pd.DataFrame()
         self.result: DataFrame | Series = pd.DataFrame()
         self.all_dates: list = []
         self.rebal_dates: list = []
 
     def set_parameters(self, backtest):
```

### Comparing `portbt-0.1.2/portbt/utils.py` & `portbt-0.1.3/portbt/utils.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.2/pyproject.toml` & `portbt-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "portbt"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python library designed to make portfolio backtesting easy and intuitive"
 authors = ["renanmoretto <himynameisrenan@outlook.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/renanmoretto/portbt"
 
 [tool.poetry.dependencies]
```

