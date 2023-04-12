# Comparing `tmp/goated-0.0.5.tar.gz` & `tmp/goated-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goated-0.0.5.tar", last modified: Wed Apr  5 23:21:59 2023, max compression
+gzip compressed data, was "goated-0.0.6.tar", last modified: Wed Apr 12 10:15:14 2023, max compression
```

## Comparing `goated-0.0.5.tar` & `goated-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.228206 goated-0.0.5/
--rw-r--r--   0 Cian       (502) staff       (20)     1055 2023-03-29 01:31:01.000000 goated-0.0.5/LICENSE.txt
--rw-r--r--   0 Cian       (502) staff       (20)     1121 2023-03-30 06:12:25.000000 goated-0.0.5/MANIFEST.in
--rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-05 23:21:59.228319 goated-0.0.5/PKG-INFO
--rw-r--r--   0 Cian       (502) staff       (20)     2397 2023-04-01 01:28:07.000000 goated-0.0.5/README.md
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.216035 goated-0.0.5/goated/
--rw-r--r--   0 Cian       (502) staff       (20)      396 2023-04-05 23:04:51.000000 goated-0.0.5/goated/__init__.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.218853 goated-0.0.5/goated/client/
--rw-r--r--   0 Cian       (502) staff       (20)      436 2023-04-05 23:03:02.000000 goated-0.0.5/goated/client/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)     6116 2023-04-01 01:41:05.000000 goated-0.0.5/goated/client/base_client.py
--rw-r--r--   0 Cian       (502) staff       (20)      344 2023-03-30 23:10:14.000000 goated-0.0.5/goated/client/exceptions.py
--rw-r--r--   0 Cian       (502) staff       (20)    19380 2023-03-27 20:32:17.000000 goated-0.0.5/goated/client/trading_client.py
--rw-r--r--   0 Cian       (502) staff       (20)     2535 2023-04-01 01:28:00.000000 goated-0.0.5/goated/example.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.220907 goated-0.0.5/goated/instructions/
--rw-r--r--   0 Cian       (502) staff       (20)      674 2023-04-05 23:15:12.000000 goated-0.0.5/goated/instructions/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)      866 2023-03-16 05:12:07.000000 goated-0.0.5/goated/instructions/cancel_order.py
--rw-r--r--   0 Cian       (502) staff       (20)      617 2023-03-20 04:18:46.000000 goated-0.0.5/goated/instructions/enums.py
--rw-r--r--   0 Cian       (502) staff       (20)     2046 2023-03-16 05:12:03.000000 goated-0.0.5/goated/instructions/new_order.py
--rw-r--r--   0 Cian       (502) staff       (20)     1159 2023-03-16 05:12:11.000000 goated-0.0.5/goated/instructions/reduce_order.py
--rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:12:14.000000 goated-0.0.5/goated/instructions/update_persistence.py
--rw-r--r--   0 Cian       (502) staff       (20)       49 2022-12-19 05:08:12.000000 goated-0.0.5/goated/main.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.224436 goated-0.0.5/goated/state/
--rw-r--r--   0 Cian       (502) staff       (20)      934 2023-04-05 23:17:45.000000 goated-0.0.5/goated/state/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)     6188 2023-03-27 00:10:44.000000 goated-0.0.5/goated/state/container.py
--rw-r--r--   0 Cian       (502) staff       (20)     5314 2023-03-27 19:57:02.000000 goated-0.0.5/goated/state/market.py
--rw-r--r--   0 Cian       (502) staff       (20)     8233 2023-03-27 19:54:58.000000 goated-0.0.5/goated/state/order.py
--rw-r--r--   0 Cian       (502) staff       (20)     8866 2023-03-27 20:01:29.000000 goated-0.0.5/goated/state/pool.py
--rw-r--r--   0 Cian       (502) staff       (20)     3140 2023-03-26 23:45:50.000000 goated-0.0.5/goated/state/position.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.226239 goated-0.0.5/goated/state/profiles/
--rw-r--r--   0 Cian       (502) staff       (20)      214 2023-03-27 20:01:28.000000 goated-0.0.5/goated/state/profiles/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)     6252 2023-03-27 20:01:28.000000 goated-0.0.5/goated/state/profiles/current_liquidity_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)     8955 2023-03-27 20:01:28.000000 goated-0.0.5/goated/state/profiles/pool_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)     1887 2023-03-27 20:01:28.000000 goated-0.0.5/goated/state/profiles/position_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)      874 2023-03-27 20:01:28.000000 goated-0.0.5/goated/state/profiles/target_liquidity_profile.py
--rw-r--r--   0 Cian       (502) staff       (20)     2785 2023-03-27 19:59:42.000000 goated-0.0.5/goated/state/selection.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.227920 goated-0.0.5/goated/utils/
--rw-r--r--   0 Cian       (502) staff       (20)      305 2023-04-05 23:06:59.000000 goated-0.0.5/goated/utils/__init__.py
--rw-r--r--   0 Cian       (502) staff       (20)    11984 2023-03-30 21:25:55.000000 goated-0.0.5/goated/utils/bucketing.py
--rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:18:05.000000 goated-0.0.5/goated/utils/converter.py
--rw-r--r--   0 Cian       (502) staff       (20)      764 2023-03-29 01:15:50.000000 goated-0.0.5/goated/utils/encoder.py
--rw-r--r--   0 Cian       (502) staff       (20)     7426 2023-03-29 01:15:53.000000 goated-0.0.5/goated/utils/payoff_signature.py
--rw-r--r--   0 Cian       (502) staff       (20)       21 2023-04-05 23:21:38.000000 goated-0.0.5/goated/version.py
-drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-05 23:21:59.217381 goated-0.0.5/goated.egg-info/
--rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-05 23:21:59.000000 goated-0.0.5/goated.egg-info/PKG-INFO
--rw-r--r--   0 Cian       (502) staff       (20)     1126 2023-04-05 23:21:59.000000 goated-0.0.5/goated.egg-info/SOURCES.txt
--rw-r--r--   0 Cian       (502) staff       (20)        1 2023-04-05 23:21:59.000000 goated-0.0.5/goated.egg-info/dependency_links.txt
--rw-r--r--   0 Cian       (502) staff       (20)       31 2023-04-05 23:21:59.000000 goated-0.0.5/goated.egg-info/requires.txt
--rw-r--r--   0 Cian       (502) staff       (20)        7 2023-04-05 23:21:59.000000 goated-0.0.5/goated.egg-info/top_level.txt
--rw-r--r--   0 Cian       (502) staff       (20)       59 2023-03-29 01:31:01.000000 goated-0.0.5/pyproject.toml
--rw-r--r--   0 Cian       (502) staff       (20)     1017 2023-04-05 23:21:59.228726 goated-0.0.5/setup.cfg
--rw-r--r--   0 Cian       (502) staff       (20)       87 2023-03-29 01:31:02.000000 goated-0.0.5/setup.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.435852 goated-0.0.6/
+-rw-r--r--   0 Cian       (502) staff       (20)     1055 2023-03-29 01:31:01.000000 goated-0.0.6/LICENSE.txt
+-rw-r--r--   0 Cian       (502) staff       (20)     1121 2023-03-30 06:12:25.000000 goated-0.0.6/MANIFEST.in
+-rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-12 10:15:14.435948 goated-0.0.6/PKG-INFO
+-rw-r--r--   0 Cian       (502) staff       (20)     2397 2023-04-01 01:28:07.000000 goated-0.0.6/README.md
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.426411 goated-0.0.6/goated/
+-rw-r--r--   0 Cian       (502) staff       (20)      396 2023-04-05 23:04:51.000000 goated-0.0.6/goated/__init__.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.428615 goated-0.0.6/goated/client/
+-rw-r--r--   0 Cian       (502) staff       (20)      435 2023-04-06 02:23:23.000000 goated-0.0.6/goated/client/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)     6116 2023-04-01 01:41:05.000000 goated-0.0.6/goated/client/base_client.py
+-rw-r--r--   0 Cian       (502) staff       (20)      344 2023-03-30 23:10:14.000000 goated-0.0.6/goated/client/exceptions.py
+-rw-r--r--   0 Cian       (502) staff       (20)    19380 2023-03-27 20:32:17.000000 goated-0.0.6/goated/client/trading_client.py
+-rw-r--r--   0 Cian       (502) staff       (20)     2535 2023-04-01 01:28:00.000000 goated-0.0.6/goated/example.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.430452 goated-0.0.6/goated/instructions/
+-rw-r--r--   0 Cian       (502) staff       (20)      752 2023-04-07 05:15:12.000000 goated-0.0.6/goated/instructions/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)      866 2023-03-16 05:12:07.000000 goated-0.0.6/goated/instructions/cancel_order.py
+-rw-r--r--   0 Cian       (502) staff       (20)      617 2023-03-20 04:18:46.000000 goated-0.0.6/goated/instructions/enums.py
+-rw-r--r--   0 Cian       (502) staff       (20)     2046 2023-03-16 05:12:03.000000 goated-0.0.6/goated/instructions/new_order.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1159 2023-03-16 05:12:11.000000 goated-0.0.6/goated/instructions/reduce_order.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:12:14.000000 goated-0.0.6/goated/instructions/update_persistence.py
+-rw-r--r--   0 Cian       (502) staff       (20)       49 2022-12-19 05:08:12.000000 goated-0.0.6/goated/main.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.432670 goated-0.0.6/goated/state/
+-rw-r--r--   0 Cian       (502) staff       (20)      934 2023-04-05 23:17:45.000000 goated-0.0.6/goated/state/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)     6550 2023-04-11 05:07:54.000000 goated-0.0.6/goated/state/container.py
+-rw-r--r--   0 Cian       (502) staff       (20)     7300 2023-04-11 07:18:12.000000 goated-0.0.6/goated/state/market.py
+-rw-r--r--   0 Cian       (502) staff       (20)    11919 2023-04-11 07:18:02.000000 goated-0.0.6/goated/state/order.py
+-rw-r--r--   0 Cian       (502) staff       (20)    10120 2023-04-11 07:18:09.000000 goated-0.0.6/goated/state/pool.py
+-rw-r--r--   0 Cian       (502) staff       (20)     4759 2023-04-11 07:17:49.000000 goated-0.0.6/goated/state/position.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.434285 goated-0.0.6/goated/state/profiles/
+-rw-r--r--   0 Cian       (502) staff       (20)      214 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)     6252 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/current_liquidity_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)     8955 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/pool_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1887 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/position_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)      874 2023-03-27 20:01:28.000000 goated-0.0.6/goated/state/profiles/target_liquidity_profile.py
+-rw-r--r--   0 Cian       (502) staff       (20)     3869 2023-04-11 07:17:53.000000 goated-0.0.6/goated/state/selection.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.435586 goated-0.0.6/goated/utils/
+-rw-r--r--   0 Cian       (502) staff       (20)      305 2023-04-05 23:06:59.000000 goated-0.0.6/goated/utils/__init__.py
+-rw-r--r--   0 Cian       (502) staff       (20)    11984 2023-03-30 21:25:55.000000 goated-0.0.6/goated/utils/bucketing.py
+-rw-r--r--   0 Cian       (502) staff       (20)     1037 2023-03-16 05:18:05.000000 goated-0.0.6/goated/utils/converter.py
+-rw-r--r--   0 Cian       (502) staff       (20)      764 2023-03-29 01:15:50.000000 goated-0.0.6/goated/utils/encoder.py
+-rw-r--r--   0 Cian       (502) staff       (20)     7426 2023-03-29 01:15:53.000000 goated-0.0.6/goated/utils/payoff_signature.py
+-rw-r--r--   0 Cian       (502) staff       (20)       21 2023-04-12 10:15:11.000000 goated-0.0.6/goated/version.py
+drwxr-xr-x   0 Cian       (502) staff       (20)        0 2023-04-12 10:15:14.427327 goated-0.0.6/goated.egg-info/
+-rw-r--r--   0 Cian       (502) staff       (20)     3280 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/PKG-INFO
+-rw-r--r--   0 Cian       (502) staff       (20)     1126 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/SOURCES.txt
+-rw-r--r--   0 Cian       (502) staff       (20)        1 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/dependency_links.txt
+-rw-r--r--   0 Cian       (502) staff       (20)       31 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/requires.txt
+-rw-r--r--   0 Cian       (502) staff       (20)        7 2023-04-12 10:15:14.000000 goated-0.0.6/goated.egg-info/top_level.txt
+-rw-r--r--   0 Cian       (502) staff       (20)       59 2023-03-29 01:31:01.000000 goated-0.0.6/pyproject.toml
+-rw-r--r--   0 Cian       (502) staff       (20)     1017 2023-04-12 10:15:14.436279 goated-0.0.6/setup.cfg
+-rw-r--r--   0 Cian       (502) staff       (20)       87 2023-03-29 01:31:02.000000 goated-0.0.6/setup.py
```

### Comparing `goated-0.0.5/LICENSE.txt` & `goated-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/MANIFEST.in` & `goated-0.0.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/PKG-INFO` & `goated-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goated
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for interacting with the Goated Exchange API.
 Home-page: https://github.com/goatedsports/python-sdk
 Download-URL: https://github.com/goatedsports/python-sdk/archive/refs/heads/main.zip
 Author: Goated Core Team
 Author-email: cian@goated.com
 License: MIT
 Keywords: goated,betting,trading,sports,sportsbetting,exchange,bet,prediction,market
```

### Comparing `goated-0.0.5/README.md` & `goated-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/client/base_client.py` & `goated-0.0.6/goated/client/base_client.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/client/trading_client.py` & `goated-0.0.6/goated/client/trading_client.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/example.py` & `goated-0.0.6/goated/example.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/instructions/cancel_order.py` & `goated-0.0.6/goated/instructions/cancel_order.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/instructions/enums.py` & `goated-0.0.6/goated/instructions/enums.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/instructions/new_order.py` & `goated-0.0.6/goated/instructions/new_order.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/instructions/reduce_order.py` & `goated-0.0.6/goated/instructions/reduce_order.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/instructions/update_persistence.py` & `goated-0.0.6/goated/instructions/update_persistence.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/state/__init__.py` & `goated-0.0.6/goated/state/__init__.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/state/container.py` & `goated-0.0.6/goated/state/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import datetime
 import json
+from this import d
 from typing import Union, List
 from .order import Order
 from .position import SelectionPosition
 from .pool import Pool
 from .market import Market
 from .selection import Selection
 
@@ -25,20 +27,21 @@
         if type(data) == str:
             data = json.loads(data)
         if type(data) != list:
             data = [data]
         for balance in data:
             self.balances[balance.get('currency')] = balance
 
+
     def remove_balance(
         self,
         currency: str
     ):
         if currency in self.balances.keys():
-            self.orders.pop(str(currency))
+            self.balances.pop(str(currency))
         else:
             print('No balance found for this currency')
 
 
     def update_orders(
         self,
         data: Union[dict, str, list]
@@ -201,25 +204,46 @@
         selection_id: int
     ):
         if selection_id in self.selections.keys():
             selection = self.selections.pop(int(selection_id))
         else:
             print('No selection found for this id')
 
-  
+    
+    @property
+    def balance_tickers(
+        self,
+    ): 
+        return list(self.balances.keys())
+
+    @property
+    def position_selection_ids(
+        self,
+    ): 
+        return list(self.positions.keys()) 
+
+    @property
+    def order_ids(
+        self,
+    ): 
+        return list(self.orders.keys())
+
+    @property
+    def pool_ids(
+        self,
+    ): 
+        return list(self.pools.keys())
+    
     @property
     def market_ids(
         self,
     ): 
         return list(self.markets.keys())
     
     @property
     def selection_ids(
         self,
     ): 
         return list(self.selections.keys())
     
-    @property
-    def order_ids(
-        self,
-    ): 
-        return list(self.orders.keys())
+
+
```

### Comparing `goated-0.0.5/goated/state/pool.py` & `goated-0.0.6/goated/state/pool.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .profiles import CurrentLiquidityProfile
 from .profiles import MatchedPositionProfile
 from decimal import Decimal
 import numpy as np
 from ..utils.converter import convert_to_probability
 from ..utils.bucketing import DEFAULT_AMERICAN_SCHEMA, DEFAULT_DECIMAL_SCHEMA, DEFAULT_PROBABILITY_SCHEMA
 import time
+from datetime import datetime
 
 class Pool():
 
     def __init__(
         self,
         state,
         id: int,
@@ -22,38 +23,40 @@
         price_schema: str,
         status: str,
         min_residual_quantity: Decimal,
         min_post_quantity: Decimal,
         supports_in_play: bool,
         in_play_delay_seconds: Decimal,
         event_id: int,
+        _update_timestamp: datetime = None
     ):
         self.state = state
         self.id = id
         self.scenario_space = scenario_space
         self.currency = currency
         self.payoff_signature_length = payoff_signature_length
         self._price_schema = price_schema
         self.status = status
         self.min_residual_quantity = min_residual_quantity
         self.min_post_quantity = min_post_quantity
         self.supports_in_play = supports_in_play
         self.in_play_delay_seconds = in_play_delay_seconds
         self.event_id = event_id
-        self._update_timestamp = time.time()
 
         # Profiles
         self.refresh_profiles(perform_regardless=True)
 
         # Checks on whether profile refreshes are required
         self._orders_updated = False
         self._positions_updated = False
         self._selections_updated = False
         self._markets_updated = False
         
+        self._update_timestamp = _update_timestamp if _update_timestamp else datetime.utcnow()
+
 
 
     @property
     def is_frozen(
         self,
     ):
         if self._frozen == False:
@@ -133,15 +136,45 @@
             payoff_signature_length = data.get('payoff_signature_length'),
             price_schema = data.get('price_schema'),
             status = data.get('status'),
             min_residual_quantity = Decimal(data.get('min_residual_quantity')),
             min_post_quantity = Decimal(data.get('min_post_quantity')),
             supports_in_play = data.get('supports_in_play'),
             in_play_delay_seconds = Decimal(data.get('in_play_delay_seconds')),
-            event_id = data.get('event')
+            event_id = data.get('event'),
+            _update_timestamp = datetime.strptime(data.get('_update_timestamp'), "%Y-%m-%dT%H:%M:%SZ") if data.get('_update_timestamp') != None else None,
+        )
+        
+    def serialize_to_dict(
+        self,
+    ):
+        d = {
+            'id': self.id,
+            'scenario_space': self.scenario_space,
+            'currency': self.currency,
+            'payoff_signature_length': self.payoff_signature_length,
+            'price_schema': self._price_schema,
+            'status': self.status,
+            'min_residual_quantity': f'{self.min_residual_quantity:.18f}',
+            'min_post_quantity': f'{self.min_post_quantity:.18f}',
+            'in_play_delay_seconds': f'{self.in_play_delay_seconds:.18f}',
+            'supports_in_play': self.supports_in_play,
+            'event': self.event_id,
+            '_update_timestamp': self._update_timestamp.strftime("%Y-%m-%dT%H:%M:%SZ") if self._update_timestamp else None,
+        }
+        return d
+
+
+    def serialize_to_json(
+        self,
+        indent: int = 0
+    ):
+        return json.dumps(
+            self.serialize_to_dict(),
+            indent=indent
         )
     
 
     def update_from_json(
         self,
         data: Union[str, dict]
     ):
```

### Comparing `goated-0.0.5/goated/state/profiles/current_liquidity_profile.py` & `goated-0.0.6/goated/state/profiles/current_liquidity_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/state/profiles/pool_profile.py` & `goated-0.0.6/goated/state/profiles/pool_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/state/profiles/position_profile.py` & `goated-0.0.6/goated/state/profiles/position_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/state/profiles/target_liquidity_profile.py` & `goated-0.0.6/goated/state/profiles/target_liquidity_profile.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/state/selection.py` & `goated-0.0.6/goated/state/selection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from typing import Union, List
 import json
 from ..utils.payoff_signature import PayoffSignature
 from decimal import Decimal
 import time
+from datetime import datetime
 
 class Selection():
 
     def __init__(
         self,
         state,
         id: int,
         market_id: int,
         name: str,
         competitor: Union[dict, None],
         resolution_status: Union[str, None],
         payoff_signature: str,
         display_order: int,
         status: str,
-        price_probability: str
+        price_probability: str,
+        _update_timestamp: datetime = None
     ):
         self.state = state
         self.id = id
         self.market_id = market_id
         self.name = name
         self.competitor = competitor
         self.resolution_status = resolution_status
         self.payoff_signature = PayoffSignature.from_string(payoff_signature)
         self.display_order = display_order
         self.status = status
         self.price_probability = Decimal(price_probability) if price_probability else Decimal(1)
-        self._update_timestamp = time.time()
+        self._update_timestamp = _update_timestamp if _update_timestamp else datetime.utcnow()
 
     @classmethod
     def load_from_json(
         cls,
         state,
         data: Union[str, dict]
     ):
@@ -46,16 +48,44 @@
             name = data.get('name'),
             competitor = data.get('competitor'),
             resolution_status = data.get('resolution_status'),
             payoff_signature = data.get('payoff_signature'),
             display_order = data.get('display_order'),
             status =data.get('status'),
             price_probability = data.get('price_probability'),
+            _update_timestamp = datetime.strptime(data.get('_update_timestamp'), "%Y-%m-%dT%H:%M:%SZ") if data.get('_update_timestamp') != None else None,
         )
         
+    def serialize_to_dict(
+        self,
+    ):
+        d = {
+            'id': self.id,
+            'market': self.market_id,
+            'name': self.name,
+            'competitor': self.competitor,
+            'resolution_status': self.resolution_status,
+            'payoff_signature': self.payoff_signature.to_string(),
+            'display_order': self.display_order,
+            'status': self.status,
+            'price_probability': self.price_probability,
+            '_update_timestamp': self._update_timestamp.strftime("%Y-%m-%dT%H:%M:%SZ") if self._update_timestamp else None,
+        }
+        return d
+
+    def serialize_to_json(
+        self,
+        indent: int = 0
+    ):
+        return json.dumps(
+            self.serialize_to_dict(),
+            indent=indent
+        )
+    
+        
     @classmethod
     def load_from_client(
         cls,
         state,
         id: int
     ):
         selection_data = state.client.get_selections(
```

### Comparing `goated-0.0.5/goated/utils/bucketing.py` & `goated-0.0.6/goated/utils/bucketing.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/utils/converter.py` & `goated-0.0.6/goated/utils/converter.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/utils/encoder.py` & `goated-0.0.6/goated/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated/utils/payoff_signature.py` & `goated-0.0.6/goated/utils/payoff_signature.py`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/goated.egg-info/PKG-INFO` & `goated-0.0.6/goated.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goated
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for interacting with the Goated Exchange API.
 Home-page: https://github.com/goatedsports/python-sdk
 Download-URL: https://github.com/goatedsports/python-sdk/archive/refs/heads/main.zip
 Author: Goated Core Team
 Author-email: cian@goated.com
 License: MIT
 Keywords: goated,betting,trading,sports,sportsbetting,exchange,bet,prediction,market
```

### Comparing `goated-0.0.5/goated.egg-info/SOURCES.txt` & `goated-0.0.6/goated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goated-0.0.5/setup.cfg` & `goated-0.0.6/setup.cfg`

 * *Files identical despite different names*

