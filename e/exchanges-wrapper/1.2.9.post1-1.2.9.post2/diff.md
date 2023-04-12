# Comparing `tmp/exchanges-wrapper-1.2.9.post1.tar.gz` & `tmp/exchanges-wrapper-1.2.9.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges-wrapper-1.2.9.post1.tar", last modified: Mon Jan 23 15:59:55 2023, max compression
+gzip compressed data, was "exchanges-wrapper-1.2.9.post2.tar", last modified: Sat Feb  4 17:01:11 2023, max compression
```

## Comparing `exchanges-wrapper-1.2.9.post1.tar` & `exchanges-wrapper-1.2.9.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.2.9.post1/.deepsource.toml
--rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.2.9.post1/.dockerignore
--rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.2.9.post1/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.2.9.post1/.github/dependabot.yml
--rwxr-xr-x   0        0        0     4417 2023-01-23 15:46:26.467237 exchanges-wrapper-1.2.9.post1/CHANGELOG.md
--rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.2.9.post1/Dockerfile
--rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.2.9.post1/LICENSE.md
--rw-r--r--   0        0        0     6667 2023-01-08 11:24:31.823555 exchanges-wrapper-1.2.9.post1/README.md
--rw-r--r--   0        0        0    14151 2022-09-18 14:15:05.822876 exchanges-wrapper-1.2.9.post1/example/exch_client.py
--rwxr-xr-x   0        0        0      227 2022-06-05 17:07:32.203624 exchanges-wrapper-1.2.9.post1/example/ms_cfg.toml
--rw-r--r--   0        0        0     1276 2023-01-23 15:46:26.471237 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45676 2022-12-15 14:07:38.807179 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    41250 2022-12-15 10:25:18.509000 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19558 2022-11-11 12:14:58.168172 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     3415 2022-11-11 12:14:55.292269 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    60579 2023-01-23 15:58:14.804443 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2645 2022-08-27 14:25:03.637572 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      840 2022-11-13 15:51:33.933962 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12538 2023-01-08 11:24:31.783555 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    43618 2023-01-23 15:46:26.471237 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     3673 2023-01-08 11:24:31.803555 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10514 2023-01-22 17:50:40.429785 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15766 2022-11-11 12:14:42.520683 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    18454 2022-12-04 12:13:18.586813 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12171 2022-12-15 14:07:38.807179 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    24619 2023-01-08 11:24:31.823555 exchanges-wrapper-1.2.9.post1/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0      940 2022-09-20 08:03:52.893747 exchanges-wrapper-1.2.9.post1/pyproject.toml
--rw-r--r--   0        0        0       74 2022-09-20 08:03:52.885747 exchanges-wrapper-1.2.9.post1/requirements.txt
--rw-r--r--   0        0        0     7511 1970-01-01 00:00:00.000000 exchanges-wrapper-1.2.9.post1/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.2.9.post2/.deepsource.toml
+-rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.2.9.post2/.dockerignore
+-rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.2.9.post2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.2.9.post2/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     4533 2023-02-04 15:12:03.486985 exchanges-wrapper-1.2.9.post2/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.2.9.post2/Dockerfile
+-rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.2.9.post2/LICENSE.md
+-rw-r--r--   0        0        0     6633 2023-02-04 16:54:49.040299 exchanges-wrapper-1.2.9.post2/README.md
+-rw-r--r--   0        0        0    14153 2023-02-04 15:12:03.486985 exchanges-wrapper-1.2.9.post2/example/exch_client.py
+-rwxr-xr-x   0        0        0      227 2022-06-05 17:07:32.203624 exchanges-wrapper-1.2.9.post2/example/ms_cfg.toml
+-rw-r--r--   0        0        0     1289 2023-02-04 15:12:03.486985 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    45676 2022-12-15 14:07:38.807179 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    41250 2022-12-15 10:25:18.509000 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19515 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     5737 2023-02-04 16:52:19.854578 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    59837 2023-02-04 16:52:30.821726 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2601 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12494 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    43622 2023-02-04 16:47:28.918272 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     3673 2023-01-08 11:24:31.803555 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10470 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    18411 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12171 2022-12-15 14:07:38.807179 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    24576 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0      940 2022-09-20 08:03:52.893747 exchanges-wrapper-1.2.9.post2/pyproject.toml
+-rw-r--r--   0        0        0       74 2022-09-20 08:03:52.885747 exchanges-wrapper-1.2.9.post2/requirements.txt
+-rw-r--r--   0        0        0     7456 1970-01-01 00:00:00.000000 exchanges-wrapper-1.2.9.post2/PKG-INFO
```

### Comparing `exchanges-wrapper-1.2.9.post1/CHANGELOG.md` & `exchanges-wrapper-1.2.9.post2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## v1.2.9-2 - 2023-02-04
+### Fixed
+* Fix DogsTailFarmer/martin-binance#50
+
+### Update
+* Remove unnecessary shebang
+
 ## v1.2.9-1 - 2023-01-23
 ### Update
 * Additional check for order status if its can't place during timeout period for avoid place duplicate order
 
 ## v1.2.9 - 2023-01-08
 ### Update
 * Removing FTX smell
```

### Comparing `exchanges-wrapper-1.2.9.post1/Dockerfile` & `exchanges-wrapper-1.2.9.post2/Dockerfile`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post1/LICENSE.md` & `exchanges-wrapper-1.2.9.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post1/README.md` & `exchanges-wrapper-1.2.9.post2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
 ***
 
 ## exchanges-wrapper vs binance.py
-The main difference is the development of the project for trading with many exchanges, including DeFi platforms shortly.
+The main difference is the development of the project for trading with many exchanges.
 
 Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction for many accounts
 and many trading pairs through one connection. It's powered by [gRPC](https://grpc.io/about/)
 Remote Procedure Call framework.
 
 Warning. Coverage of overridden binance.py packages is significant but not complete.
 Served methods describes into ```example/exch_client.py```
```

#### html2text {}

```diff
@@ -4,36 +4,36 @@
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** *** ##
 exchanges-wrapper vs binance.py The main difference is the development of the
-project for trading with many exchanges, including DeFi platforms shortly. Next
-is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer
-layer, providing simultaneous async interaction for many accounts and many
-trading pairs through one connection. It's powered by [gRPC](https://grpc.io/
-about/) Remote Procedure Call framework. Warning. Coverage of overridden
-binance.py packages is significant but not complete. Served methods describes
-into ```example/exch_client.py``` ### Initial capabilities (inherited from
-binance.py) - Covers general endpoints (test connectivity and get exchange
-information's) - Covers market data endpoints - Covers Account endpoints
-(create and manage orders) - Covers user data stream (receive real time user
-updates) - Covers web socket streams (receive real time market updates) - Async
-support - Auto reconnect after exchanges API or network failure - Completely
-free and without limitations ### Added Features - Multi exchanges support -
-Adaptive algorithm to ensure maximum performance and avoid exceeding the rates
-limits - Passthrough logging ## Extra exchanges implementation features -
-Binance REST API and WSS are accepted as basic, connection of other exchanges
-wrapped their API to Binance compatible - For other, some data cannot be
-obtained by directly calling one method, it is generated by a synthetic or
-calculation method - Some exchanges have not any testing or "paper trading"
-features, therefore, application development and testing is possible only at
-real bidding. First, run applications on the [Binance Spot Test Network](https:
-//testnet.binance.vision/) or Bitfinex test account. ## Get started ### Prepare
+project for trading with many exchanges. Next is adding a new module
+```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing
+simultaneous async interaction for many accounts and many trading pairs through
+one connection. It's powered by [gRPC](https://grpc.io/about/) Remote Procedure
+Call framework. Warning. Coverage of overridden binance.py packages is
+significant but not complete. Served methods describes into ```example/
+exch_client.py``` ### Initial capabilities (inherited from binance.py) - Covers
+general endpoints (test connectivity and get exchange information's) - Covers
+market data endpoints - Covers Account endpoints (create and manage orders) -
+Covers user data stream (receive real time user updates) - Covers web socket
+streams (receive real time market updates) - Async support - Auto reconnect
+after exchanges API or network failure - Completely free and without
+limitations ### Added Features - Multi exchanges support - Adaptive algorithm
+to ensure maximum performance and avoid exceeding the rates limits -
+Passthrough logging ## Extra exchanges implementation features - Binance REST
+API and WSS are accepted as basic, connection of other exchanges wrapped their
+API to Binance compatible - For other, some data cannot be obtained by directly
+calling one method, it is generated by a synthetic or calculation method - Some
+exchanges have not any testing or "paper trading" features, therefore,
+application development and testing is possible only at real bidding. First,
+run applications on the [Binance Spot Test Network](https://
+testnet.binance.vision/) or Bitfinex test account. ## Get started ### Prepare
 exchange account * Create account on [Binance](https://accounts.binance.com/en/
 register?ref=QCS4OGWR) and get 10% discount on all trading fee * Create account
 on [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
 rebate fee * Create account on [HUOBI](https://www.huobi.com/en-us/topic/
 double-reward/?invite_code=9uaw3223) and get 10% cashback on all trading fee *
 Create account on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes
 worth up to $10,000 * For test purpose log in at [Binance Spot Test Network]
```

### Comparing `exchanges-wrapper-1.2.9.post1/example/exch_client.py` & `exchanges-wrapper-1.2.9.post2/example/exch_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3.8
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Client example for exchanges-wrapper, examples of use of server methods are given
 """
 
 import asyncio
 import toml
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/__init__.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-REST API and WebSocket asyncio wrapper with grpc powered multiplexer server for crypto exchanges
- (Binance, FTX, Bitfinex,)
-Utilizes one connection for many accounts and trading pairs.
-For SPOT market only
+REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
+ for crypto exchanges (Binance, Bitfinex, OKX, Huobi,)
+ Utilizes one connection for many accounts and trading pairs.
+ For SPOT market only
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.2.9-1"
+__version__ = "1.2.9-2"
 
 from pathlib import Path
 import shutil
 #
 import platform
 print(f"Python {platform.python_version()}")
 #
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/api_pb2.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/api_pb2_grpc.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/bitfinex_parser.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/bitfinex_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
 """
 Parser for convert Bitfinex REST API/WSS response to Binance like result
 """
 import time
 from decimal import Decimal
 import logging
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/client.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-
 import aiohttp
 from enum import Enum
 from typing import Union
 import decimal
 import math
 import asyncio
 import logging
@@ -811,33 +808,19 @@
             params = {"symbol": symbol}
             if order_id:
                 params["orderId"] = order_id
             else:
                 params["origClientOrderId"] = origin_client_order_id
             if receive_window:
                 params["recvWindow"] = receive_window
-            res = await self.http.send_api_call(
+            binance_res = await self.http.send_api_call(
                 "/api/v3/order",
                 params=params,
                 signed=True,
             )
-            binance_res = {
-                "symbol": res.get('symbol'),
-                "orderId": res.get('orderId'),
-                "orderListId": res.get('orderListId'),
-                "clientOrderId": res.get('clientOrderId'),
-                "price": res.get('price'),
-                "origQty": res.get('origQty'),
-                "executedQty": res.get('executedQty'),
-                "cummulativeQuoteQty": res.get('cummulativeQuoteQty'),
-                "status": res.get('status'),
-                "timeInForce": res.get('timeInForce'),
-                "type": res.get('type'),
-                "side": res.get('side'),
-            }
         elif self.exchange == 'bitfinex':
             params = {'id': [order_id]}
             res = await self.http.send_api_call(
                 f"v2/auth/r/orders/{self.symbol_to_bfx(symbol)}",
                 method="POST",
                 signed=True,
                 **params
@@ -845,15 +828,14 @@
             if not res:
                 res = await self.http.send_api_call(
                     f"v2/auth/r/orders/{self.symbol_to_bfx(symbol)}/hist",
                     method="POST",
                     signed=True,
                     **params
                 )
-            logger.debug(f"fetch_order(closed).res: {res}")
             if res:
                 binance_res = bfx.order(res[0], response_type=response_type)
         elif self.exchange == 'huobi':
             if origin_client_order_id:
                 params = {'clientOrderId': str(origin_client_order_id)}
                 res = await self.http.send_api_call("/v1/order/orders/getClientOrder", signed=True, **params)
             else:
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/definitions.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-
 # Enum definitions of the exchanges_wrapper REST API
 # see: https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#enum-definitions
 
 from enum import Enum
 
 
 # Symbol status (status)
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/errors.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-
 class ExchangePyError(Exception):
     pass
 
 
 class UnknownEventType(ExchangePyError):
     message = "ExchangePy doesn't handle this event type"
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/events.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-
 import asyncio
 import functools
 from collections import defaultdict
 import logging
 
 from exchanges_wrapper.errors import UnknownEventType
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/exch_srv.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from exchanges_wrapper import __version__
 
 import time
 import weakref
 import gc
 import traceback
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/http_client.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-
 import json
 from urllib.parse import urlencode, urlparse
 from exchanges_wrapper import __version__
 import logging
 import time
 from datetime import datetime
 from exchanges_wrapper.c_structures import generate_signature
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/huobi_parser.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/huobi_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
 """
 Parser for convert Huobi REST API/WSS response to Binance like result
 """
 import time
 from decimal import Decimal
 import logging
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/okx_parser.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/okx_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
 """
 Parser for convert OKX REST API/WSS response to Binance like result
 """
 import time
 from decimal import Decimal
 import logging
```

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post1/exchanges_wrapper/web_sockets.py` & `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/web_sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
 # __version__ = "1.2.6b4"
 
 from exchanges_wrapper import __version__
 
 import aiohttp
 import asyncio
 import json
```

### Comparing `exchanges-wrapper-1.2.9.post1/pyproject.toml` & `exchanges-wrapper-1.2.9.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post1/PKG-INFO` & `exchanges-wrapper-1.2.9.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.2.9.post1
-Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server for crypto exchanges
+Version: 1.2.9.post2
+Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -35,15 +35,15 @@
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
 ***
 
 ## exchanges-wrapper vs binance.py
-The main difference is the development of the project for trading with many exchanges, including DeFi platforms shortly.
+The main difference is the development of the project for trading with many exchanges.
 
 Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction for many accounts
 and many trading pairs through one connection. It's powered by [gRPC](https://grpc.io/about/)
 Remote Procedure Call framework.
 
 Warning. Coverage of overridden binance.py packages is significant but not complete.
 Served methods describes into ```example/exch_client.py```
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.2.9.post1 Summary:
-REST API and WebSocket asyncio wrapper with grpc powered multiplexer server for
-crypto exchanges Author-email: Thomas Marchand
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.2.9.post2 Summary:
+REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
+Author-email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: aiohttp==3.8.1 Requires-Dist: grpcio==1.48.1 Requires-Dist: grpcio-
@@ -16,36 +16,36 @@
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** *** ##
 exchanges-wrapper vs binance.py The main difference is the development of the
-project for trading with many exchanges, including DeFi platforms shortly. Next
-is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer
-layer, providing simultaneous async interaction for many accounts and many
-trading pairs through one connection. It's powered by [gRPC](https://grpc.io/
-about/) Remote Procedure Call framework. Warning. Coverage of overridden
-binance.py packages is significant but not complete. Served methods describes
-into ```example/exch_client.py``` ### Initial capabilities (inherited from
-binance.py) - Covers general endpoints (test connectivity and get exchange
-information's) - Covers market data endpoints - Covers Account endpoints
-(create and manage orders) - Covers user data stream (receive real time user
-updates) - Covers web socket streams (receive real time market updates) - Async
-support - Auto reconnect after exchanges API or network failure - Completely
-free and without limitations ### Added Features - Multi exchanges support -
-Adaptive algorithm to ensure maximum performance and avoid exceeding the rates
-limits - Passthrough logging ## Extra exchanges implementation features -
-Binance REST API and WSS are accepted as basic, connection of other exchanges
-wrapped their API to Binance compatible - For other, some data cannot be
-obtained by directly calling one method, it is generated by a synthetic or
-calculation method - Some exchanges have not any testing or "paper trading"
-features, therefore, application development and testing is possible only at
-real bidding. First, run applications on the [Binance Spot Test Network](https:
-//testnet.binance.vision/) or Bitfinex test account. ## Get started ### Prepare
+project for trading with many exchanges. Next is adding a new module
+```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing
+simultaneous async interaction for many accounts and many trading pairs through
+one connection. It's powered by [gRPC](https://grpc.io/about/) Remote Procedure
+Call framework. Warning. Coverage of overridden binance.py packages is
+significant but not complete. Served methods describes into ```example/
+exch_client.py``` ### Initial capabilities (inherited from binance.py) - Covers
+general endpoints (test connectivity and get exchange information's) - Covers
+market data endpoints - Covers Account endpoints (create and manage orders) -
+Covers user data stream (receive real time user updates) - Covers web socket
+streams (receive real time market updates) - Async support - Auto reconnect
+after exchanges API or network failure - Completely free and without
+limitations ### Added Features - Multi exchanges support - Adaptive algorithm
+to ensure maximum performance and avoid exceeding the rates limits -
+Passthrough logging ## Extra exchanges implementation features - Binance REST
+API and WSS are accepted as basic, connection of other exchanges wrapped their
+API to Binance compatible - For other, some data cannot be obtained by directly
+calling one method, it is generated by a synthetic or calculation method - Some
+exchanges have not any testing or "paper trading" features, therefore,
+application development and testing is possible only at real bidding. First,
+run applications on the [Binance Spot Test Network](https://
+testnet.binance.vision/) or Bitfinex test account. ## Get started ### Prepare
 exchange account * Create account on [Binance](https://accounts.binance.com/en/
 register?ref=QCS4OGWR) and get 10% discount on all trading fee * Create account
 on [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
 rebate fee * Create account on [HUOBI](https://www.huobi.com/en-us/topic/
 double-reward/?invite_code=9uaw3223) and get 10% cashback on all trading fee *
 Create account on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes
 worth up to $10,000 * For test purpose log in at [Binance Spot Test Network]
```

