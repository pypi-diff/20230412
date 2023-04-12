# Comparing `tmp/python-okx-0.1.8.tar.gz` & `tmp/python-okx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-okx-0.1.8.tar", last modified: Tue Mar 28 03:21:44 2023, max compression
+gzip compressed data, was "python-okx-0.1.9.tar", last modified: Wed Apr 12 06:43:15 2023, max compression
```

## Comparing `python-okx-0.1.8.tar` & `python-okx-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-03-28 03:21:44.819306 python-okx-0.1.8/
--rw-r--r--   0 oker       (501) staff       (20)     2934 2023-03-28 03:21:44.819028 python-okx-0.1.8/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)     2586 2023-02-16 06:55:25.000000 python-okx-0.1.8/README.md
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-03-28 03:21:44.810874 python-okx-0.1.8/okx/
--rw-r--r--   0 oker       (501) staff       (20)     7099 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/Account.py
--rw-r--r--   0 oker       (501) staff       (20)     3699 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/BlockTrading.py
--rw-r--r--   0 oker       (501) staff       (20)     1542 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/Convert.py
--rw-r--r--   0 oker       (501) staff       (20)     2139 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/Earning.py
--rw-r--r--   0 oker       (501) staff       (20)      756 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/FDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     5035 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/Funding.py
--rw-r--r--   0 oker       (501) staff       (20)     4248 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/Grid.py
--rw-r--r--   0 oker       (501) staff       (20)     4476 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/MarketData.py
--rw-r--r--   0 oker       (501) staff       (20)     5031 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/NDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     5056 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/PublicData.py
--rw-r--r--   0 oker       (501) staff       (20)      463 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/Status.py
--rw-r--r--   0 oker       (501) staff       (20)     2660 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/SubAccount.py
--rw-r--r--   0 oker       (501) staff       (20)     8218 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/Trade.py
--rw-r--r--   0 oker       (501) staff       (20)     2299 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/TradingData.py
--rw-r--r--   0 oker       (501) staff       (20)       58 2023-03-28 03:21:02.000000 python-okx-0.1.8/okx/__init__.py
--rw-r--r--   0 oker       (501) staff       (20)     2233 2023-03-28 03:20:42.000000 python-okx-0.1.8/okx/client.py
--rw-r--r--   0 oker       (501) staff       (20)    10930 2023-03-28 03:20:01.000000 python-okx-0.1.8/okx/consts.py
--rw-r--r--   0 oker       (501) staff       (20)     1246 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/exceptions.py
--rw-r--r--   0 oker       (501) staff       (20)     1826 2022-12-12 02:06:58.000000 python-okx-0.1.8/okx/utils.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-03-28 03:21:44.816791 python-okx-0.1.8/okx/websocket/
--rw-r--r--   0 oker       (501) staff       (20)     2070 2022-12-16 08:49:53.000000 python-okx-0.1.8/okx/websocket/WsClientFactory.py
--rw-r--r--   0 oker       (501) staff       (20)     1712 2022-12-05 07:37:01.000000 python-okx-0.1.8/okx/websocket/WsClientProtocol.py
--rw-r--r--   0 oker       (501) staff       (20)     5393 2022-12-15 13:01:18.000000 python-okx-0.1.8/okx/websocket/WsConnectManager.py
--rw-r--r--   0 oker       (501) staff       (20)     2672 2022-12-04 06:10:10.000000 python-okx-0.1.8/okx/websocket/WsLoginFactory.py
--rw-r--r--   0 oker       (501) staff       (20)      924 2022-12-15 13:06:35.000000 python-okx-0.1.8/okx/websocket/WsPrivate.py
--rw-r--r--   0 oker       (501) staff       (20)      498 2022-12-15 12:59:40.000000 python-okx-0.1.8/okx/websocket/WsPublic.py
--rw-r--r--   0 oker       (501) staff       (20)     2234 2022-12-05 08:05:32.000000 python-okx-0.1.8/okx/websocket/WsUtils.py
--rw-r--r--   0 oker       (501) staff       (20)        0 2022-12-15 12:47:25.000000 python-okx-0.1.8/okx/websocket/__init__.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-03-28 03:21:44.818578 python-okx-0.1.8/python_okx.egg-info/
--rw-r--r--   0 oker       (501) staff       (20)     2934 2023-03-28 03:21:44.000000 python-okx-0.1.8/python_okx.egg-info/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)      723 2023-03-28 03:21:44.000000 python-okx-0.1.8/python_okx.egg-info/SOURCES.txt
--rw-r--r--   0 oker       (501) staff       (20)        1 2023-03-28 03:21:44.000000 python-okx-0.1.8/python_okx.egg-info/dependency_links.txt
--rw-r--r--   0 oker       (501) staff       (20)       67 2023-03-28 03:21:44.000000 python-okx-0.1.8/python_okx.egg-info/requires.txt
--rw-r--r--   0 oker       (501) staff       (20)        4 2023-03-28 03:21:44.000000 python-okx-0.1.8/python_okx.egg-info/top_level.txt
--rw-r--r--   0 oker       (501) staff       (20)       38 2023-03-28 03:21:44.819413 python-okx-0.1.8/setup.cfg
--rw-r--r--   0 oker       (501) staff       (20)      758 2023-03-28 03:15:08.000000 python-okx-0.1.8/setup.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.071591 python-okx-0.1.9/
+-rw-r--r--   0 oker       (501) staff       (20)     2934 2023-04-12 06:43:15.071277 python-okx-0.1.9/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)     2586 2023-02-16 06:55:25.000000 python-okx-0.1.9/README.md
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.061478 python-okx-0.1.9/okx/
+-rw-r--r--   0 oker       (501) staff       (20)     7099 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Account.py
+-rw-r--r--   0 oker       (501) staff       (20)     3699 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/BlockTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)     1542 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Convert.py
+-rw-r--r--   0 oker       (501) staff       (20)     2139 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Earning.py
+-rw-r--r--   0 oker       (501) staff       (20)      756 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/FDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     5058 2023-04-12 06:41:59.000000 python-okx-0.1.9/okx/Funding.py
+-rw-r--r--   0 oker       (501) staff       (20)     4248 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Grid.py
+-rw-r--r--   0 oker       (501) staff       (20)     4476 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/MarketData.py
+-rw-r--r--   0 oker       (501) staff       (20)     5031 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/NDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     5056 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/PublicData.py
+-rw-r--r--   0 oker       (501) staff       (20)      463 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Status.py
+-rw-r--r--   0 oker       (501) staff       (20)     2660 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/SubAccount.py
+-rw-r--r--   0 oker       (501) staff       (20)     8218 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Trade.py
+-rw-r--r--   0 oker       (501) staff       (20)     2299 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/TradingData.py
+-rw-r--r--   0 oker       (501) staff       (20)       58 2023-04-12 06:42:27.000000 python-okx-0.1.9/okx/__init__.py
+-rw-r--r--   0 oker       (501) staff       (20)     2233 2023-03-28 03:20:42.000000 python-okx-0.1.9/okx/client.py
+-rw-r--r--   0 oker       (501) staff       (20)    10930 2023-03-28 03:20:01.000000 python-okx-0.1.9/okx/consts.py
+-rw-r--r--   0 oker       (501) staff       (20)     1246 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/exceptions.py
+-rw-r--r--   0 oker       (501) staff       (20)     1826 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/utils.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.068356 python-okx-0.1.9/okx/websocket/
+-rw-r--r--   0 oker       (501) staff       (20)     2070 2022-12-16 08:49:53.000000 python-okx-0.1.9/okx/websocket/WsClientFactory.py
+-rw-r--r--   0 oker       (501) staff       (20)     1712 2022-12-05 07:37:01.000000 python-okx-0.1.9/okx/websocket/WsClientProtocol.py
+-rw-r--r--   0 oker       (501) staff       (20)     5393 2022-12-15 13:01:18.000000 python-okx-0.1.9/okx/websocket/WsConnectManager.py
+-rw-r--r--   0 oker       (501) staff       (20)     2672 2022-12-04 06:10:10.000000 python-okx-0.1.9/okx/websocket/WsLoginFactory.py
+-rw-r--r--   0 oker       (501) staff       (20)      924 2022-12-15 13:06:35.000000 python-okx-0.1.9/okx/websocket/WsPrivate.py
+-rw-r--r--   0 oker       (501) staff       (20)      498 2022-12-15 12:59:40.000000 python-okx-0.1.9/okx/websocket/WsPublic.py
+-rw-r--r--   0 oker       (501) staff       (20)     2234 2022-12-05 08:05:32.000000 python-okx-0.1.9/okx/websocket/WsUtils.py
+-rw-r--r--   0 oker       (501) staff       (20)        0 2022-12-15 12:47:25.000000 python-okx-0.1.9/okx/websocket/__init__.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.070707 python-okx-0.1.9/python_okx.egg-info/
+-rw-r--r--   0 oker       (501) staff       (20)     2934 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)      723 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/SOURCES.txt
+-rw-r--r--   0 oker       (501) staff       (20)        1 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/dependency_links.txt
+-rw-r--r--   0 oker       (501) staff       (20)       67 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/requires.txt
+-rw-r--r--   0 oker       (501) staff       (20)        4 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/top_level.txt
+-rw-r--r--   0 oker       (501) staff       (20)       38 2023-04-12 06:43:15.071721 python-okx-0.1.9/setup.cfg
+-rw-r--r--   0 oker       (501) staff       (20)      758 2023-03-28 03:15:08.000000 python-okx-0.1.9/setup.py
```

### Comparing `python-okx-0.1.8/PKG-INFO` & `python-okx-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.1.8/README.md` & `python-okx-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/Account.py` & `python-okx-0.1.9/okx/Account.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/BlockTrading.py` & `python-okx-0.1.9/okx/BlockTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/Convert.py` & `python-okx-0.1.9/okx/Convert.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/Earning.py` & `python-okx-0.1.9/okx/Earning.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/FDBroker.py` & `python-okx-0.1.9/okx/FDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/Funding.py` & `python-okx-0.1.9/okx/Funding.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
     # Get Deposit History
     def get_deposit_history(self, ccy='', state='', after='', before='', limit='',txId='',depId=''):
         params = {'ccy': ccy, 'state': state, 'after': after, 'before': before, 'limit': limit,'txId':txId,'depId':depId}
         return self._request_with_params(GET, DEPOSIT_HISTORIY, params)
 
     # Get Withdrawal History
-    def get_withdrawal_history(self, ccy='', state='', after='', before='', limit='',txId=''):
-        params = {'ccy': ccy, 'state': state, 'after': after, 'before': before, 'limit': limit,'txId':txId}
+    def get_withdrawal_history(self, ccy='', wdId='', state='', after='', before='', limit='',txId=''):
+        params = {'ccy': ccy, 'wdId': wdId, 'state': state, 'after': after, 'before': before, 'limit': limit,'txId':txId}
         return self._request_with_params(GET, WITHDRAWAL_HISTORIY, params)
 
     # Get Currencies
     def get_currencies(self, ccy=''):
         params = {'ccy': ccy}
         return self._request_with_params(GET, CURRENCY_INFO, params)
```

### Comparing `python-okx-0.1.8/okx/Grid.py` & `python-okx-0.1.9/okx/Grid.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/MarketData.py` & `python-okx-0.1.9/okx/MarketData.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/NDBroker.py` & `python-okx-0.1.9/okx/NDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/PublicData.py` & `python-okx-0.1.9/okx/PublicData.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/SubAccount.py` & `python-okx-0.1.9/okx/SubAccount.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/Trade.py` & `python-okx-0.1.9/okx/Trade.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/TradingData.py` & `python-okx-0.1.9/okx/TradingData.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/client.py` & `python-okx-0.1.9/okx/client.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/consts.py` & `python-okx-0.1.9/okx/consts.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/exceptions.py` & `python-okx-0.1.9/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/utils.py` & `python-okx-0.1.9/okx/utils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/websocket/WsClientFactory.py` & `python-okx-0.1.9/okx/websocket/WsClientFactory.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/websocket/WsClientProtocol.py` & `python-okx-0.1.9/okx/websocket/WsClientProtocol.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/websocket/WsConnectManager.py` & `python-okx-0.1.9/okx/websocket/WsConnectManager.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/websocket/WsLoginFactory.py` & `python-okx-0.1.9/okx/websocket/WsLoginFactory.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/websocket/WsPrivate.py` & `python-okx-0.1.9/okx/websocket/WsPrivate.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/okx/websocket/WsUtils.py` & `python-okx-0.1.9/okx/websocket/WsUtils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/python_okx.egg-info/PKG-INFO` & `python-okx-0.1.9/python_okx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.1.8/python_okx.egg-info/SOURCES.txt` & `python-okx-0.1.9/python_okx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.8/setup.py` & `python-okx-0.1.9/setup.py`

 * *Files identical despite different names*

