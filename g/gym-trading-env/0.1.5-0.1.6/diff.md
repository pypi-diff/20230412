# Comparing `tmp/gym-trading-env-0.1.5.tar.gz` & `tmp/gym-trading-env-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.1.5.tar", last modified: Tue Apr 11 10:12:22 2023, max compression
+gzip compressed data, was "gym-trading-env-0.1.6.tar", last modified: Wed Apr 12 05:48:48 2023, max compression
```

## Comparing `gym-trading-env-0.1.5.tar` & `gym-trading-env-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 10:12:22.697621 gym-trading-env-0.1.5/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0    14011 2023-04-11 10:12:22.696623 gym-trading-env-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    12149 2023-04-11 09:31:03.000000 gym-trading-env-0.1.5/README.md
--rw-rw-rw-   0        0        0      854 2023-04-11 10:09:30.000000 gym-trading-env-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 10:12:22.697621 gym-trading-env-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 10:12:22.606096 gym-trading-env-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 10:12:22.640775 gym-trading-env-0.1.5/src/gym_trading_env/
--rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.5/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     3986 2023-04-11 10:11:51.000000 gym-trading-env-0.1.5/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.5/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.5/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:12:22.693633 gym-trading-env-0.1.5/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.5/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.5/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.5/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.5/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:12:22.683690 gym-trading-env-0.1.5/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0    14011 2023-04-11 10:12:22.000000 gym-trading-env-0.1.5/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-04-11 10:12:22.000000 gym-trading-env-0.1.5/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 10:12:22.000000 gym-trading-env-0.1.5/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-04-11 10:12:22.000000 gym-trading-env-0.1.5/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 10:12:22.000000 gym-trading-env-0.1.5/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.774973 gym-trading-env-0.1.6/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    14011 2023-04-12 05:48:48.773975 gym-trading-env-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12149 2023-04-11 09:31:03.000000 gym-trading-env-0.1.6/README.md
+-rw-rw-rw-   0        0        0      870 2023-04-12 05:33:10.000000 gym-trading-env-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 05:48:48.774973 gym-trading-env-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.612408 gym-trading-env-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.665269 gym-trading-env-0.1.6/src/gym_trading_env/
+-rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.6/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4029 2023-04-12 05:32:37.000000 gym-trading-env-0.1.6/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.6/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.6/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.770983 gym-trading-env-0.1.6/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.718124 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0    14011 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.1.5/LICENSE.txt` & `gym-trading-env-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.5/PKG-INFO` & `gym-trading-env-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.5/README.md` & `gym-trading-env-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.5/pyproject.toml` & `gym-trading-env-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.1.5"
+version = "0.1.6"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["pandas>=1.5.3", "numpy>=1.23.1", "gymnasium>=0.28.1", "flask>=2.2.3", "pyecharts>=2.0.2", "ccxt==3.0.59", "numpy>=1.24.2"]
+dependencies = ["pandas>=1.5.3", "numpy>=1.23.1", "gymnasium>=0.28.1", "flask>=2.2.3", "pyecharts>=2.0.2", "ccxt==3.0.59", "numpy>=1.24.2", "nest_asyncio"]
 
 [project.urls]
 "Homepage" = "https://github.com/ClementPerroud/Gym-Trading-Env"
 "Bug Tracker" = "https://github.com/ClementPerroud/Gym-Trading-Env/issues"
```

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env/downloader.py` & `gym-trading-env-0.1.6/src/gym_trading_env/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import ccxt.async_support as ccxt
 import pandas as pd
 import datetime
 import numpy as np
+import nest_asyncio
+nest_asyncio.apply()
 
 EXCHANGE_LIMIT_RATES = {
     "bitfinex2": {
         "limit":10_000,
         "pause_every": 1,
         "pause" : 3, #seconds
     },
```

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env/environments.py` & `gym-trading-env-0.1.6/src/gym_trading_env/environments.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env/renderer.py` & `gym-trading-env-0.1.6/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.1.6/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.1.6/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.1.6/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.1.6/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.5/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.1.6/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

