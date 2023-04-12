# Comparing `tmp/portbt-0.1.3.tar.gz` & `tmp/portbt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portbt-0.1.3.tar", max compression
+gzip compressed data, was "portbt-0.1.4.tar", max compression
```

## Comparing `portbt-0.1.3.tar` & `portbt-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.3/portbt/__init__.py
--rw-r--r--   0        0        0     3139 2023-04-12 03:01:01.868034 portbt-0.1.3/portbt/backtest_functions.py
--rw-r--r--   0        0        0     1663 2023-04-12 03:03:15.656462 portbt-0.1.3/portbt/portfolio.py
--rw-r--r--   0        0        0      658 2023-04-11 22:15:59.356410 portbt-0.1.3/portbt/utils.py
--rw-r--r--   0        0        0      575 2023-04-12 03:08:12.542581 portbt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3747 2023-04-12 03:07:27.269246 portbt-0.1.3/README.md
--rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 portbt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.4/portbt/__init__.py
+-rw-r--r--   0        0        0     3139 2023-04-12 03:01:01.868034 portbt-0.1.4/portbt/backtest_functions.py
+-rw-r--r--   0        0        0     1663 2023-04-12 03:03:15.656462 portbt-0.1.4/portbt/portfolio.py
+-rw-r--r--   0        0        0      658 2023-04-11 22:15:59.356410 portbt-0.1.4/portbt/utils.py
+-rw-r--r--   0        0        0      575 2023-04-12 03:09:55.339039 portbt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3755 2023-04-12 03:09:19.187519 portbt-0.1.4/README.md
+-rw-r--r--   0        0        0     4368 1970-01-01 00:00:00.000000 portbt-0.1.4/PKG-INFO
```

### Comparing `portbt-0.1.3/LICENSE.txt` & `portbt-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `portbt-0.1.3/portbt/backtest_functions.py` & `portbt-0.1.4/portbt/backtest_functions.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.3/portbt/portfolio.py` & `portbt-0.1.4/portbt/portfolio.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.3/portbt/utils.py` & `portbt-0.1.4/portbt/utils.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.3/pyproject.toml` & `portbt-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "portbt"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python library designed to make portfolio backtesting easy and intuitive"
 authors = ["renanmoretto <himynameisrenan@outlook.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/renanmoretto/portbt"
 
 [tool.poetry.dependencies]
```

### Comparing `portbt-0.1.3/README.md` & `portbt-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -70,20 +70,20 @@
 2023-04-05  0.258185  0.102898  0.145396  0.130913  0.139037  0.223571
 2023-04-06  0.258177  0.103195  0.145399  0.129457  0.139871  0.223901
 2023-04-10  0.255589  0.103228  0.145400  0.130815  0.139155  0.225814
 ```
 
 ## Portfolio functions
 ```
-Portfolio.backtest_with_rebalance() -> dict
+Portfolio.backtest_with_rebalance() -> Backtest
     Optional parameters:
         rebal_weights: dict | str,
         rebal_freq: str,
 
-Portfolio.backtest_without_rebalance() -> dict
+Portfolio.backtest_without_rebalance() -> Backtest
     Optional parameters:
         start_weights: dict | str,
 ```
 
 ## TODO
 - Performance metrics and visualizations
 - Reports
```

### Comparing `portbt-0.1.3/PKG-INFO` & `portbt-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portbt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library designed to make portfolio backtesting easy and intuitive
 Home-page: https://github.com/renanmoretto/portbt
 License: MIT
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -89,20 +89,20 @@
 2023-04-05  0.258185  0.102898  0.145396  0.130913  0.139037  0.223571
 2023-04-06  0.258177  0.103195  0.145399  0.129457  0.139871  0.223901
 2023-04-10  0.255589  0.103228  0.145400  0.130815  0.139155  0.225814
 ```
 
 ## Portfolio functions
 ```
-Portfolio.backtest_with_rebalance() -> dict
+Portfolio.backtest_with_rebalance() -> Backtest
     Optional parameters:
         rebal_weights: dict | str,
         rebal_freq: str,
 
-Portfolio.backtest_without_rebalance() -> dict
+Portfolio.backtest_without_rebalance() -> Backtest
     Optional parameters:
         start_weights: dict | str,
 ```
 
 ## TODO
 - Performance metrics and visualizations
 - Reports
```

