# Comparing `tmp/unicorn-binance-websocket-api-1.45.2.tar.gz` & `tmp/unicorn-binance-websocket-api-1.46.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicorn-binance-websocket-api-1.45.2.tar", last modified: Mon Apr 10 01:47:18 2023, max compression
+gzip compressed data, was "unicorn-binance-websocket-api-1.46.0.tar", last modified: Wed Apr 12 21:37:44 2023, max compression
```

## Comparing `unicorn-binance-websocket-api-1.45.2.tar` & `unicorn-binance-websocket-api-1.46.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-10 01:47:18.508813 unicorn-binance-websocket-api-1.45.2/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1215 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/LICENSE
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    44007 2023-04-10 01:47:18.504819 unicorn-binance-websocket-api-1.45.2/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    42159 2023-04-09 23:44:27.000000 unicorn-binance-websocket-api-1.45.2/README.md
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-10 01:47:18.510814 unicorn-binance-websocket-api-1.45.2/setup.cfg
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4925 2023-04-10 01:41:32.000000 unicorn-binance-websocket-api-1.45.2/setup.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-10 01:47:18.311409 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      498 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/__init__.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    47042 2023-04-07 22:03:52.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/api.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    26452 2023-04-06 12:13:20.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2836 2023-04-10 01:34:45.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection_settings.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2168 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/exceptions.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)   208184 2023-04-10 01:46:50.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/manager.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    14327 2023-04-04 08:52:30.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restclient.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3673 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restserver.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    16540 2023-04-07 16:36:46.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/sockets.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-10 01:47:18.473240 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    44007 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      680 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      162 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/requires.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       30 2023-04-10 01:47:17.000000 unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/top_level.txt
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 21:37:44.612731 unicorn-binance-websocket-api-1.46.0/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1215 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.0/LICENSE
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    43944 2023-04-12 21:37:44.607577 unicorn-binance-websocket-api-1.46.0/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    42105 2023-04-12 19:43:57.000000 unicorn-binance-websocket-api-1.46.0/README.md
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-12 21:37:44.613907 unicorn-binance-websocket-api-1.46.0/setup.cfg
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4920 2023-04-12 19:43:57.000000 unicorn-binance-websocket-api-1.46.0/setup.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 21:37:44.423591 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      498 2023-04-10 02:58:46.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/__init__.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    86185 2023-04-12 21:14:34.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/api.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    26452 2023-04-06 12:13:20.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2744 2023-04-12 11:58:02.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection_settings.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2168 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/exceptions.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)   209597 2023-04-12 21:37:26.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/manager.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    17375 2023-04-12 13:37:19.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restclient.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3673 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restserver.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    18629 2023-04-12 12:04:53.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/sockets.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 21:37:44.575566 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    43944 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      680 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      162 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/requires.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       30 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/top_level.txt
```

### Comparing `unicorn-binance-websocket-api-1.45.2/LICENSE` & `unicorn-binance-websocket-api-1.46.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.2/PKG-INFO` & `unicorn-binance-websocket-api-1.46.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-websocket-api
-Version: 1.45.2
-Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, jex, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
+Version: 1.46.0
+Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-websocket-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-websocket-api.docs.lucit.tech
 Project-URL: Wiki, https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki
@@ -61,27 +61,28 @@
 
 [Description](#description) | [Live Demo](#live-demo) | [Installation](#installation-and-upgrade) | [How To](#howto) |
 [Documentation](#documentation) | [Examples](#examples) | [Change Log](#change-log) | [Wiki](#wiki) | [Social](#social) |
 [Notifications](#receive-notifications) | [Bugs](#how-to-report-bugs-or-suggest-improvements) | 
 [Contributing](#contributing) | [Leave a review](#you-want-to-say-thank-you) | [Disclaimer](#disclaimer) | [Commercial Support](#commercial-support)
 
 An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, 
-com-isolated_margin+testnet, com-futures+testnet, com-coin_futures, us, tr, jex, dex/chain+testnet) 
+com-isolated_margin+testnet, com-futures+testnet, com-coin_futures, us, tr, dex/chain+testnet) 
 in a easy, fast, flexible, robust and fully-featured way. 
 
 Part of ['UNICORN Binance Suite'](https://www.lucit.tech/unicorn-binance-suite.html).
 
+## Receive Data from Binance WebSockets
 ### [Create a multiplex websocket connection](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.create_stream) to Binance with a [`stream_buffer`](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/%60stream_buffer%60) with just 3 lines of code:
 
 ```
 import unicorn_binance_websocket_api
 
 
 ubwa = unicorn_binance_websocket_api.BinanceWebSocketApiManager(exchange="binance.com")
-ubwa.create_stream(['trade', 'kline_1m'], ['btcusdt', 'bnbbtc', 'ethbtc'])
+ubwa.create_stream(channels=['trade', 'kline_1m'], markets=['btcusdt', 'bnbbtc', 'ethbtc'])
 ```
 
 #### And 4 more lines to print the receives:
 ```
 while True:
     oldest_data_from_stream_buffer = ubwa.pop_stream_data_from_stream_buffer()
     if oldest_data_from_stream_buffer:
@@ -94,15 +95,16 @@
 
 
 def process_new_receives(stream_data):
     print(str(stream_data))
 
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
-ubwa.create_stream(['trade', 'kline_1m'], ['btcusdt', 'bnbbtc', 'ethbtc'], process_stream_data=process_new_receives)
+ubwa.create_stream(channels=['trade', 'kline_1m'], markets=['btcusdt', 'bnbbtc', 'ethbtc'], 
+                   process_stream_data=process_new_receives)
 ```
 
 Basically that's it, but there are more options.
 
 ### Convert received raw webstream data into well-formed Python dictionaries with [UnicornFy](https://www.lucit.tech/unicorn-fy.html):
 ```
 unicorn_fied_stream_data = UnicornFy.binance_com_websocket(oldest_data_from_stream_buffer)
@@ -115,22 +117,23 @@
 ```
 
 ### [Subscribe](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.subscribe_to_stream) / [unsubscribe](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.unsubscribe_from_stream) new markets and channels:
 ```
 markets = ['engbtc', 'zileth']
 channels = ['kline_5m', 'kline_15m', 'kline_30m', 'kline_1h', 'kline_12h', 'depth5']
 
-ubwa.subscribe_to_stream(stream_id, channels=channels, markets=markets)
+ubwa.subscribe_to_stream(stream_id=stream_id, channels=channels, markets=markets)
 
-ubwa.unsubscribe_from_stream(stream_id, markets=markets)
+ubwa.unsubscribe_from_stream(stream_id=stream_id, markets=markets)
 
-ubwa.unsubscribe_from_stream(stream_id, channels=channels)
+ubwa.unsubscribe_from_stream(stream_id=stream_id, channels=channels)
 ```
 
-### [Place orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.create_order), [cancel orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.cancel_order) or [send other requests](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#module-unicorn_binance_websocket_api.api) via WebSocket.
+## Send Requests to Binance WebSocket API
+### [Place orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.create_order), [cancel orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.cancel_order) or [send other requests](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#module-unicorn_binance_websocket_api.api) via WebSocket:
 ```
 from unicorn_binance_websocket_api.manager import BinanceWebSocketApiManager
 
 
 def process_api_responses(stream_data):
     print(str(stream_data))
 
@@ -138,19 +141,23 @@
 api_key = "YOUR BINANCE API KEY"
 api_secret = "YOUR BINANCE API SECRET"
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
 api_stream = ubwa.create_stream(api=True, api_key=api_key, api_secret=api_secret,
                                 process_stream_data=process_api_responses)
                                 
-orig_client_order_id = ubwa.api.create_order(stream_id=api_stream, price=1.1, order_type="LIMIT",
+orig_client_order_id = ubwa.api.create_order(order_type="LIMIT", price=1.1, 
                                              quantity=15.0, side="SELL", symbol="BUSDUSDT")
-ubwa.api.cancel_order(stream_id=api_stream, symbol="BUSDUSDT", orig_client_order_id=orig_client_order_id)                                             
+ubwa.api.cancel_order(orig_client_order_id=orig_client_order_id, symbol="BUSDUSDT")                                             
 ```
 
+[Here](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404) you can find a complete 
+guide on 
+[how to process requests via the Binance WebSocket API](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404)!
+
 ### Get the right [logger](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/Logging):
 ```
 logging.getLogger("unicorn_binance_websocket_api")
 ```
 
 [Discover even more possibilities](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html)
 or [use this script](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_stream_everything.py) 
@@ -171,24 +178,22 @@
 [Binance Isolated Margin](https://binance-docs.github.io/apidocs/spot/en/#listen-key-isolated-margin)
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Futures](https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams) 
 ([+Testnet](https://testnet.binancefuture.com)), 
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
 [Binance US](https://github.com/binance-us/binance-official-api-docs), 
 [Binance TR](https://www.trbinance.com/apidocs), 
-[Binance JEX](https://jexapi.github.io/api-doc/spot.html#web-socket-streams), 
 [Binance DEX](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and 
 [Binance DEX Testnet](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and supports sending requests 
 to the [Binance Websocket API](https://developers.binance.com/docs/binance-trading-api/websocket_api) and the streaming 
 of all public streams like trade, kline, ticker, depth, bookTicker, forceOrder, compositeIndex, blockheight etc. and 
 also all private userData streams which needs to be used with a valid api_key and api_secret from the Binance Exchange 
 [www.binance.com](https://www.binance.com/userCenter/createApi.html), 
-[testnet.binance.vision](https://testnet.binance.vision/), 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) or 
-[www.jex.com](https://www.jex.com/userCenter/createApi.html) - for the DEX you need a user address from 
+[testnet.binance.vision](https://testnet.binance.vision/) or 
+[www.binance.us](https://www.binance.us/userCenter/createApi.html) - for the DEX you need a user address from 
 [www.binance.org](https://www.binance.org/en/create) or [testnet.binance.org](https://testnet.binance.org/en/create) 
 and you can [get funds](https://www.binance.vision/tutorials/binance-dex-funding-your-testnet-account) for the testnet.
 
 Use the [UNICORN Binance REST API](https://www.lucit.tech/unicorn-binance-rest-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance WebSocket API?
 - Fully managed websockets and 100% auto-reconnect! Also handles maintenance windows!
@@ -209,15 +214,14 @@
 | [Binance Isolated Margin](https://www.binance.com)                 | `binance.com-isolated_margin`         |
 | [Binance Isolated Margin Testnet](https://testnet.binance.vision/) | `binance.com-isolated_margin-testnet` |
 | [Binance USD-M Futures](https://www.binance.com)                   | `binance.com-futures`                 |
 | [Binance USD-M Futures Testnet](https://testnet.binancefuture.com) | `binance.com-futures-testnet`         |
 | [Binance Coin-M Futures](https://www.binance.com)                  | `binance.com-coin_futures`            |
 | [Binance US](https://www.binance.us)                               | `binance.us`                          |
 | [Binance TR](https://www.trbinance.com)                            | `trbinance.com`                       |
-| [Binance JEX](https://www.jex.com)                                 | `jex.com`                             |
 | [Binance DEX](https://www.binance.org)                             | `binance.org`                         |
 | [Binance DEX Testnet](https://testnet.binance.org)                 | `binance.org-testnet`                 |
 
 - Streams are processing asynchronous/concurrent (Python asyncio) and each stream is started in a separate thread, so 
 you dont need to deal with asyncio in your code!
 
 - Supports 
@@ -295,17 +299,19 @@
 [![icinga2-demo](https://raw.githubusercontent.com/lucit-systems-and-development/unicorn-binance-websocket-api/master/images/misc/icinga.png)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/UNICORN-Monitoring-API-Service)
 
 - Integration of [test cases](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml) and [examples](#examples).
 
 - Customizable base URL.
 
 - *Socks5 Proxy* support:
+
   ```
   ubwa = BinanceWebSocketApiManager(exchange="binance.com", socks5_proxy_server="127.0.0.1:9050") 
   ```
+  
   Read the [docs](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager)
   or this [how to](https://medium.com/@oliverzehentleitner/how-to-connect-to-binance-com-websockets-using-python-via-a-socks5-proxy-3c5a3e063f12) 
   for more information or try 
   [example_socks5_proxy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_socks5_proxy.py).
 
 - Excessively tested on Linux, Mac and Windows
 
@@ -342,18 +348,18 @@
 ### From source of the latest release with PIP from [Github](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 #### Linux, macOS, ...
 Run in bash:
 
 `pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/$(curl -s https://api.github.com/repos/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest | grep -oP '"tag_name": "\K(.*)(?=")').tar.gz --upgrade`
 
 #### Windows
-Use the below command with the version (such as 1.43.3) you determined 
+Use the below command with the version (such as 1.46.0) you determined 
 [here](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest):
 
-`pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/1.43.3.tar.gz --upgrade`
+`pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/1.46.0.tar.gz --upgrade`
 ### From the latest source (dev-stage) with PIP from [Github](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 This is not a release version and can not be considered to be stable!
 
 `pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/tarball/master --upgrade`
 
 ### [Conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), [Virtualenv](https://virtualenv.pypa.io/en/latest/) or plain [Python](https://www.python.org)
 Download the [latest release](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest) 
@@ -372,15 +378,14 @@
 - [Modules](https://unicorn-binance-websocket-api.docs.lucit.tech/modules.html)
 
 ## Examples
 - [example_binance_coin_futures.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_coin_futures.py)
 - [example_binance_dex.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_dex.py)
 - [example_binance_futures.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_futures.py)
 - [example_binance_futures_1s.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_futures_1s.py)
-- [example_binance_jex.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_jex.py)
 - [example_binance_us.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_us.py)
 - [example_bookticker.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_bookticker.py)
 - [example_ctrl-c.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_ctrl-c.py)
 - [example_demo.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_demo.py)
 - [example_easy_migration_from_python-binance.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_easy_migration_from_python-binance.py)
 - [example_interactive_mode.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_interactive_mode.py)
 - [example_kline_1m_with_unicorn_fy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_kline_1m_with_unicorn_fy.py)
@@ -438,15 +443,14 @@
 
 Follow us on [Twitter](https://twitter.com/LUCIT_SysDev) or on [Facebook](https://www.facebook.com/lucit.systems.and.development) for general news about the [unicorn-binance-suite](https://www.lucit.tech/unicorn-binance-suite.html)!
 
 To receive news (like inspection windows/maintenance) about the Binance API`s subscribe to their telegram groups: 
 
 - [https://t.me/binance_api_announcements](https://t.me/binance_api_announcements)
 - [https://t.me/binance_api_english](https://t.me/binance_api_english)
-- [https://t.me/Binance_JEX_EN](https://t.me/Binance_JEX_EN)
 - [https://t.me/Binance_USA](https://t.me/Binance_USA)
 - [https://t.me/TRBinanceTR](https://t.me/TRBinanceTR)
 - [https://t.me/BinanceDEXchange](https://t.me/BinanceDEXchange)
 - [https://t.me/BinanceExchange](https://t.me/BinanceExchange)
 
 ## How to report Bugs or suggest Improvements?
 [List of planned features](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement) - 
@@ -478,15 +482,15 @@
 ## Disclaimer
 This project is for informational purposes only. You should not construe this information or any other material as 
 legal, tax, investment, financial or other advice. Nothing contained herein constitutes a solicitation, recommendation, 
 endorsement or offer by us or any third party provider to buy or sell any securities or other financial instruments in 
 this or any other jurisdiction in which such solicitation or offer would be unlawful under the securities laws of such 
 jurisdiction.
 
-***If you intend to use real money, use it at your own risk.***
+### If you intend to use real money, use it at your own risk!
 
 Under no circumstances will we be responsible or liable for any claims, damages, losses, expenses, costs or liabilities 
 of any kind, including but not limited to direct or indirect damages for loss of profits.
 
 ### SOCKS5 Proxy / Geoblocking
 We would like to explicitly point out that in our opinion US citizens are exclusively authorized to trade on Binance.US 
 and that this restriction must not be circumvented!
```

### Comparing `unicorn-binance-websocket-api-1.45.2/README.md` & `unicorn-binance-websocket-api-1.46.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,27 +24,28 @@
 
 [Description](#description) | [Live Demo](#live-demo) | [Installation](#installation-and-upgrade) | [How To](#howto) |
 [Documentation](#documentation) | [Examples](#examples) | [Change Log](#change-log) | [Wiki](#wiki) | [Social](#social) |
 [Notifications](#receive-notifications) | [Bugs](#how-to-report-bugs-or-suggest-improvements) | 
 [Contributing](#contributing) | [Leave a review](#you-want-to-say-thank-you) | [Disclaimer](#disclaimer) | [Commercial Support](#commercial-support)
 
 An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, 
-com-isolated_margin+testnet, com-futures+testnet, com-coin_futures, us, tr, jex, dex/chain+testnet) 
+com-isolated_margin+testnet, com-futures+testnet, com-coin_futures, us, tr, dex/chain+testnet) 
 in a easy, fast, flexible, robust and fully-featured way. 
 
 Part of ['UNICORN Binance Suite'](https://www.lucit.tech/unicorn-binance-suite.html).
 
+## Receive Data from Binance WebSockets
 ### [Create a multiplex websocket connection](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.create_stream) to Binance with a [`stream_buffer`](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/%60stream_buffer%60) with just 3 lines of code:
 
 ```
 import unicorn_binance_websocket_api
 
 
 ubwa = unicorn_binance_websocket_api.BinanceWebSocketApiManager(exchange="binance.com")
-ubwa.create_stream(['trade', 'kline_1m'], ['btcusdt', 'bnbbtc', 'ethbtc'])
+ubwa.create_stream(channels=['trade', 'kline_1m'], markets=['btcusdt', 'bnbbtc', 'ethbtc'])
 ```
 
 #### And 4 more lines to print the receives:
 ```
 while True:
     oldest_data_from_stream_buffer = ubwa.pop_stream_data_from_stream_buffer()
     if oldest_data_from_stream_buffer:
@@ -57,15 +58,16 @@
 
 
 def process_new_receives(stream_data):
     print(str(stream_data))
 
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
-ubwa.create_stream(['trade', 'kline_1m'], ['btcusdt', 'bnbbtc', 'ethbtc'], process_stream_data=process_new_receives)
+ubwa.create_stream(channels=['trade', 'kline_1m'], markets=['btcusdt', 'bnbbtc', 'ethbtc'], 
+                   process_stream_data=process_new_receives)
 ```
 
 Basically that's it, but there are more options.
 
 ### Convert received raw webstream data into well-formed Python dictionaries with [UnicornFy](https://www.lucit.tech/unicorn-fy.html):
 ```
 unicorn_fied_stream_data = UnicornFy.binance_com_websocket(oldest_data_from_stream_buffer)
@@ -78,22 +80,23 @@
 ```
 
 ### [Subscribe](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.subscribe_to_stream) / [unsubscribe](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.unsubscribe_from_stream) new markets and channels:
 ```
 markets = ['engbtc', 'zileth']
 channels = ['kline_5m', 'kline_15m', 'kline_30m', 'kline_1h', 'kline_12h', 'depth5']
 
-ubwa.subscribe_to_stream(stream_id, channels=channels, markets=markets)
+ubwa.subscribe_to_stream(stream_id=stream_id, channels=channels, markets=markets)
 
-ubwa.unsubscribe_from_stream(stream_id, markets=markets)
+ubwa.unsubscribe_from_stream(stream_id=stream_id, markets=markets)
 
-ubwa.unsubscribe_from_stream(stream_id, channels=channels)
+ubwa.unsubscribe_from_stream(stream_id=stream_id, channels=channels)
 ```
 
-### [Place orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.create_order), [cancel orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.cancel_order) or [send other requests](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#module-unicorn_binance_websocket_api.api) via WebSocket.
+## Send Requests to Binance WebSocket API
+### [Place orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.create_order), [cancel orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.cancel_order) or [send other requests](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#module-unicorn_binance_websocket_api.api) via WebSocket:
 ```
 from unicorn_binance_websocket_api.manager import BinanceWebSocketApiManager
 
 
 def process_api_responses(stream_data):
     print(str(stream_data))
 
@@ -101,19 +104,23 @@
 api_key = "YOUR BINANCE API KEY"
 api_secret = "YOUR BINANCE API SECRET"
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
 api_stream = ubwa.create_stream(api=True, api_key=api_key, api_secret=api_secret,
                                 process_stream_data=process_api_responses)
                                 
-orig_client_order_id = ubwa.api.create_order(stream_id=api_stream, price=1.1, order_type="LIMIT",
+orig_client_order_id = ubwa.api.create_order(order_type="LIMIT", price=1.1, 
                                              quantity=15.0, side="SELL", symbol="BUSDUSDT")
-ubwa.api.cancel_order(stream_id=api_stream, symbol="BUSDUSDT", orig_client_order_id=orig_client_order_id)                                             
+ubwa.api.cancel_order(orig_client_order_id=orig_client_order_id, symbol="BUSDUSDT")                                             
 ```
 
+[Here](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404) you can find a complete 
+guide on 
+[how to process requests via the Binance WebSocket API](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404)!
+
 ### Get the right [logger](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/Logging):
 ```
 logging.getLogger("unicorn_binance_websocket_api")
 ```
 
 [Discover even more possibilities](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html)
 or [use this script](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_stream_everything.py) 
@@ -134,24 +141,22 @@
 [Binance Isolated Margin](https://binance-docs.github.io/apidocs/spot/en/#listen-key-isolated-margin)
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Futures](https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams) 
 ([+Testnet](https://testnet.binancefuture.com)), 
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
 [Binance US](https://github.com/binance-us/binance-official-api-docs), 
 [Binance TR](https://www.trbinance.com/apidocs), 
-[Binance JEX](https://jexapi.github.io/api-doc/spot.html#web-socket-streams), 
 [Binance DEX](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and 
 [Binance DEX Testnet](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and supports sending requests 
 to the [Binance Websocket API](https://developers.binance.com/docs/binance-trading-api/websocket_api) and the streaming 
 of all public streams like trade, kline, ticker, depth, bookTicker, forceOrder, compositeIndex, blockheight etc. and 
 also all private userData streams which needs to be used with a valid api_key and api_secret from the Binance Exchange 
 [www.binance.com](https://www.binance.com/userCenter/createApi.html), 
-[testnet.binance.vision](https://testnet.binance.vision/), 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) or 
-[www.jex.com](https://www.jex.com/userCenter/createApi.html) - for the DEX you need a user address from 
+[testnet.binance.vision](https://testnet.binance.vision/) or 
+[www.binance.us](https://www.binance.us/userCenter/createApi.html) - for the DEX you need a user address from 
 [www.binance.org](https://www.binance.org/en/create) or [testnet.binance.org](https://testnet.binance.org/en/create) 
 and you can [get funds](https://www.binance.vision/tutorials/binance-dex-funding-your-testnet-account) for the testnet.
 
 Use the [UNICORN Binance REST API](https://www.lucit.tech/unicorn-binance-rest-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance WebSocket API?
 - Fully managed websockets and 100% auto-reconnect! Also handles maintenance windows!
@@ -172,15 +177,14 @@
 | [Binance Isolated Margin](https://www.binance.com)                 | `binance.com-isolated_margin`         |
 | [Binance Isolated Margin Testnet](https://testnet.binance.vision/) | `binance.com-isolated_margin-testnet` |
 | [Binance USD-M Futures](https://www.binance.com)                   | `binance.com-futures`                 |
 | [Binance USD-M Futures Testnet](https://testnet.binancefuture.com) | `binance.com-futures-testnet`         |
 | [Binance Coin-M Futures](https://www.binance.com)                  | `binance.com-coin_futures`            |
 | [Binance US](https://www.binance.us)                               | `binance.us`                          |
 | [Binance TR](https://www.trbinance.com)                            | `trbinance.com`                       |
-| [Binance JEX](https://www.jex.com)                                 | `jex.com`                             |
 | [Binance DEX](https://www.binance.org)                             | `binance.org`                         |
 | [Binance DEX Testnet](https://testnet.binance.org)                 | `binance.org-testnet`                 |
 
 - Streams are processing asynchronous/concurrent (Python asyncio) and each stream is started in a separate thread, so 
 you dont need to deal with asyncio in your code!
 
 - Supports 
@@ -258,17 +262,19 @@
 [![icinga2-demo](https://raw.githubusercontent.com/lucit-systems-and-development/unicorn-binance-websocket-api/master/images/misc/icinga.png)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/UNICORN-Monitoring-API-Service)
 
 - Integration of [test cases](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml) and [examples](#examples).
 
 - Customizable base URL.
 
 - *Socks5 Proxy* support:
+
   ```
   ubwa = BinanceWebSocketApiManager(exchange="binance.com", socks5_proxy_server="127.0.0.1:9050") 
   ```
+  
   Read the [docs](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager)
   or this [how to](https://medium.com/@oliverzehentleitner/how-to-connect-to-binance-com-websockets-using-python-via-a-socks5-proxy-3c5a3e063f12) 
   for more information or try 
   [example_socks5_proxy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_socks5_proxy.py).
 
 - Excessively tested on Linux, Mac and Windows
 
@@ -305,18 +311,18 @@
 ### From source of the latest release with PIP from [Github](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 #### Linux, macOS, ...
 Run in bash:
 
 `pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/$(curl -s https://api.github.com/repos/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest | grep -oP '"tag_name": "\K(.*)(?=")').tar.gz --upgrade`
 
 #### Windows
-Use the below command with the version (such as 1.43.3) you determined 
+Use the below command with the version (such as 1.46.0) you determined 
 [here](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest):
 
-`pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/1.43.3.tar.gz --upgrade`
+`pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/1.46.0.tar.gz --upgrade`
 ### From the latest source (dev-stage) with PIP from [Github](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 This is not a release version and can not be considered to be stable!
 
 `pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/tarball/master --upgrade`
 
 ### [Conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), [Virtualenv](https://virtualenv.pypa.io/en/latest/) or plain [Python](https://www.python.org)
 Download the [latest release](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest) 
@@ -335,15 +341,14 @@
 - [Modules](https://unicorn-binance-websocket-api.docs.lucit.tech/modules.html)
 
 ## Examples
 - [example_binance_coin_futures.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_coin_futures.py)
 - [example_binance_dex.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_dex.py)
 - [example_binance_futures.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_futures.py)
 - [example_binance_futures_1s.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_futures_1s.py)
-- [example_binance_jex.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_jex.py)
 - [example_binance_us.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_us.py)
 - [example_bookticker.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_bookticker.py)
 - [example_ctrl-c.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_ctrl-c.py)
 - [example_demo.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_demo.py)
 - [example_easy_migration_from_python-binance.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_easy_migration_from_python-binance.py)
 - [example_interactive_mode.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_interactive_mode.py)
 - [example_kline_1m_with_unicorn_fy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_kline_1m_with_unicorn_fy.py)
@@ -401,15 +406,14 @@
 
 Follow us on [Twitter](https://twitter.com/LUCIT_SysDev) or on [Facebook](https://www.facebook.com/lucit.systems.and.development) for general news about the [unicorn-binance-suite](https://www.lucit.tech/unicorn-binance-suite.html)!
 
 To receive news (like inspection windows/maintenance) about the Binance API`s subscribe to their telegram groups: 
 
 - [https://t.me/binance_api_announcements](https://t.me/binance_api_announcements)
 - [https://t.me/binance_api_english](https://t.me/binance_api_english)
-- [https://t.me/Binance_JEX_EN](https://t.me/Binance_JEX_EN)
 - [https://t.me/Binance_USA](https://t.me/Binance_USA)
 - [https://t.me/TRBinanceTR](https://t.me/TRBinanceTR)
 - [https://t.me/BinanceDEXchange](https://t.me/BinanceDEXchange)
 - [https://t.me/BinanceExchange](https://t.me/BinanceExchange)
 
 ## How to report Bugs or suggest Improvements?
 [List of planned features](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement) - 
@@ -441,15 +445,15 @@
 ## Disclaimer
 This project is for informational purposes only. You should not construe this information or any other material as 
 legal, tax, investment, financial or other advice. Nothing contained herein constitutes a solicitation, recommendation, 
 endorsement or offer by us or any third party provider to buy or sell any securities or other financial instruments in 
 this or any other jurisdiction in which such solicitation or offer would be unlawful under the securities laws of such 
 jurisdiction.
 
-***If you intend to use real money, use it at your own risk.***
+### If you intend to use real money, use it at your own risk!
 
 Under no circumstances will we be responsible or liable for any claims, damages, losses, expenses, costs or liabilities 
 of any kind, including but not limited to direct or indirect damages for loss of profits.
 
 ### SOCKS5 Proxy / Geoblocking
 We would like to explicitly point out that in our opinion US citizens are exclusively authorized to trade on Binance.US 
 and that this restriction must not be circumvented!
```

### Comparing `unicorn-binance-websocket-api-1.45.2/setup.py` & `unicorn-binance-websocket-api-1.46.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 setuptools.setup(
      name='unicorn-binance-websocket-api',
      version=str(ubwa.get_version()),
      author="LUCIT Systems and Development",
      author_email='info@lucit.tech',
      url="https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api",
      description="An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, "
-                 "com-isolated_margin+testnet, com-futures+testnet, jersey, us, jex, dex/chain+testnet) in a easy, fast"
+                 "com-isolated_margin+testnet, com-futures+testnet, jersey, us, dex/chain+testnet) in a easy, fast"
                  ", flexible, robust and fully-featured way.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      license='MIT License',
      install_requires=['colorama', 'requests', 'websocket-client', 'websockets==10.4', 'flask_restful',
                        'cheroot', 'flask', 'ujson', 'psutil', 'PySocks', 'unicorn-fy',
-                       'unicorn-binance-rest-api>=1.8.1', 'typing_extensions'],
+                       'unicorn-binance-rest-api>=1.9.0', 'typing_extensions'],
      keywords='binance, asyncio, async, asynchronous, concurrent, websocket-api, webstream-api, '
               'binance-websocket, binance-webstream, webstream, websocket, api, binance-jersey, binance-dex, '
               'binance-futures, binance-margin, binance-us',
      project_urls={
          'Howto': 'https://www.lucit.tech/unicorn-binance-websocket-api.html#howto',
          'Documentation': 'https://unicorn-binance-websocket-api.docs.lucit.tech',
          'Wiki': 'https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki',
```

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection.py` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/connection_settings.py` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     BINANCE_ISOLATED_MARGIN = "binance.com-isolated_margin"
     BINANCE_ISOLATED_MARGIN_TESTNET = "binance.com-isolated_margin-testnet"
     BINANCE_FUTURES = "binance.com-futures"
     BINANCE_COIN_FUTURES = "binance.com-coin_futures"
     BINANCE_FUTURES_TESTNET = "binance.com-futures-testnet"
     BINANCE_US = "binance.us"
     TRBINANCE = "trbinance.com"
-    JEX = "jex.com"
     BINANCE_ORG = "binance.org"
     BINANCE_ORG_TESTNET = "binance.org-testnet"
 
 
 DEX_EXCHANGES = [Exchanges.BINANCE_ORG, Exchanges.BINANCE_ORG_TESTNET]
 CEX_EXCHANGES = [
     Exchanges.BINANCE,
@@ -38,15 +37,14 @@
     Exchanges.BINANCE_ISOLATED_MARGIN,
     Exchanges.BINANCE_ISOLATED_MARGIN_TESTNET,
     Exchanges.BINANCE_FUTURES,
     Exchanges.BINANCE_COIN_FUTURES,
     Exchanges.BINANCE_FUTURES_TESTNET,
     Exchanges.BINANCE_US,
     Exchanges.TRBINANCE,
-    Exchanges.JEX,
 ]
 
 # only python 3.9+
 # CONNECTION_SETTINGS: dict[str, Tuple[MAX_SUBSCRIPTIONS_PER_STREAM, WEBSOCKET_BASE_URI, WEBSOCKET_API_BASE_URI]] = {
 
 CONNECTION_SETTINGS = {
     Exchanges.BINANCE: (1024, "wss://stream.binance.com:9443/", "wss://ws-api.binance.com/ws-api/v3"),
@@ -56,11 +54,10 @@
     Exchanges.BINANCE_ISOLATED_MARGIN: (1024, "wss://stream.binance.com:9443/", ""),
     Exchanges.BINANCE_ISOLATED_MARGIN_TESTNET: (1024, "wss://testnet.binance.vision/", ""),
     Exchanges.BINANCE_FUTURES: (200, "wss://fstream.binance.com/", ""),
     Exchanges.BINANCE_FUTURES_TESTNET: (200, "wss://stream.binancefuture.com/", ""),
     Exchanges.BINANCE_COIN_FUTURES: (200, "wss://dstream.binance.com/", ""),
     Exchanges.BINANCE_US: (1024, "wss://stream.binance.us:9443/", ""),
     Exchanges.TRBINANCE: (1024, "wss://stream-cloud.trbinance.com/", ""),
-    Exchanges.JEX: (10, "wss://ws.jex.com/", ""),
     Exchanges.BINANCE_ORG: (1024, "wss://dex.binance.org/api/", ""),
     Exchanges.BINANCE_ORG_TESTNET: (1024, "wss://testnet-dex.binance.org/api/", ""),
 }
```

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/exceptions.py` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/manager.py` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
 
 logger = logging.getLogger("unicorn_binance_websocket_api")
 
 
 class BinanceWebSocketApiManager(threading.Thread):
     """
     An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet,
-    com-isolated_margin+testnet, com-futures+testnet, us, jex, dex/chain+testnet) in a easy, fast, flexible,
+    com-isolated_margin+testnet, com-futures+testnet, us, dex/chain+testnet) in a easy, fast, flexible,
     robust and fully-featured way.
 
     This library supports two different kind of websocket endpoints:
 
-        - CEX (Centralized exchange): binance.com, binance.vision, binance.je, binance.us, trbinance.com, jex.com
+        - CEX (Centralized exchange): binance.com, binance.vision, binance.je, binance.us, trbinance.com
 
         - DEX (Decentralized exchange): binance.org
 
     Binance.com websocket API documentation:
 
         - https://github.com/binance/binance-spot-api-docs/blob/master/web-socket-streams.md
 
@@ -102,20 +102,14 @@
 
         - https://docs.binance.us/#introduction
 
     TRBinance.com websocket API documentation:
 
         - https://www.trbinance.com/apidocs/#general-wss-information
 
-    Jex.com websocket API documentation:
-
-        - https://jexapi.github.io/api-doc/option.html#web-socket-streams
-
-        - https://jexapi.github.io/api-doc/option.html#user-data-streams
-
     Binance.org websocket API documentation:
 
         - https://docs.binance.org/api-reference/dex-api/ws-connection.html
 
     :param process_stream_data: Provide a function/method to process the received webstream data (callback). The function
                                 will be called instead of
                                 `add_to_stream_buffer() <unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.add_to_stream_buffer>`_
@@ -124,15 +118,15 @@
                                 get stored in the stream_buffer or provided to a specific callback function of
                                 `create_stream()`! `How to read from stream_buffer!
                                 <https://unicorn-binance-websocket-api.docs.lucit.tech/README.html#and-4-more-lines-to-print-the-receives>`_
     :type process_stream_data: function
     :param exchange: Select binance.com, binance.com-testnet, binance.com-margin, binance.com-margin-testnet,
                      binance.com-isolated_margin, binance.com-isolated_margin-testnet, binance.com-futures,
                      binance.com-futures-testnet, binance.com-coin_futures, binance.us, trbinance.com,
-                     jex.com, binance.org, binance.org-testnet (default: binance.com)
+                     binance.org, binance.org-testnet (default: binance.com)
     :type exchange: str
     :param warn_on_update: set to `False` to disable the update warning of UBWA and also in UBRA used as submodule.
     :type warn_on_update: bool
     :param throw_exception_if_unrepairable: set to `True` to activate exceptions if a crashed stream is unrepairable
                                             (invalid API key, exceeded subscription limit) or an unknown exchange is
                                             used
     :type throw_exception_if_unrepairable: bool
@@ -232,15 +226,15 @@
                  exchange_type: Optional[Literal['cex', 'dex']] = None,
                  socks5_proxy_server: Optional[str] = None,
                  socks5_proxy_user: Optional[str] = None,
                  socks5_proxy_pass: Optional[str] = None,
                  socks5_proxy_ssl_verification: Optional[bool] = True,):
         threading.Thread.__init__(self)
         self.name = "unicorn-binance-websocket-api"
-        self.version = "1.45.2"
+        self.version = "1.46.0"
         logger.info(f"New instance of {self.get_user_agent()} on "
                     f"{str(platform.system())} {str(platform.release())} for exchange {exchange} started ...")
         self.debug = debug
         logger.info(f"Debug is {self.debug}")
         if disable_colorama is not True:
             logger.info(f"Initiating `colorama_{colorama.__version__}`")
             colorama.init()
@@ -335,20 +329,24 @@
         self.max_send_messages_per_second = 5
         self.max_send_messages_per_second_reserve = 2
         self.most_receives_per_second = 0
         self.monitoring_api_server = False
         self.monitoring_total_received_bytes = 0
         self.monitoring_total_receives = 0
         self.output_default = output_default
+        self.process_response = {}
+        self.process_response_lock = threading.Lock()
         self.reconnects = 0
         self.reconnects_lock = threading.Lock()
         self.request_id = 0
         self.request_id_lock = threading.Lock()
         self.restart_requests = {}
         self.restart_timeout = restart_timeout
+        self.return_response = {}
+        self.return_response_lock = threading.Lock()
         self.ringbuffer_error = []
         self.ringbuffer_error_max_size = 500
         self.ringbuffer_result = []
         self.ringbuffer_result_max_size = 500
         self.show_secrets_in_logs = show_secrets_in_logs
         self.start_time = time.time()
         self.stream_buffer_maxlen = stream_buffer_maxlen
@@ -747,15 +745,15 @@
                 if last_second_receiving_speed > self.receiving_speed_peak['value']:
                     self.receiving_speed_peak['value'] = last_second_receiving_speed
                     self.receiving_speed_peak['timestamp'] = time.time()
                     logger.info(f"BinanceWebSocketApiManager._frequent_checks() - reached new "
                                 f"`highest_receiving_speed` "
                                 f"{str(self.get_human_bytesize(self.receiving_speed_peak['value'], '/s'))} at "
                                 f"{self.get_date_of_timestamp(self.receiving_speed_peak['timestamp'])}")
-            except TypeError as error_msg:
+            except TypeError:
                 pass
             # send keepalive for `!userData` streams every 30 minutes
             if active_stream_list:
                 for stream_id in active_stream_list:
                     if isinstance(active_stream_list[stream_id]['markets'], str):
                         active_stream_list[stream_id]['markets'] = [active_stream_list[stream_id]['markets'], ]
                     if isinstance(active_stream_list[stream_id]['channels'], str):
@@ -815,15 +813,15 @@
             except RuntimeError as error_msg:
                 if "dictionary changed size during iteration" in error_msg:
                     continue
                 else:
                     raise RuntimeError(error_msg)
             for stream_id in temp_restart_requests:
                 try:
-                    # find restarts that didnt work
+                    # find restarts that didn't work
                     if self.restart_requests[stream_id]['status'] == "restarted" and \
                             self.restart_requests[stream_id]['last_restart_time']+self.restart_timeout < time.time():
                         self.restart_requests[stream_id] = {'status': "new",
                                                             'initiated': None}
                     # restart streams with requests
                     if self.restart_requests[stream_id]['status'] == "new" or \
                             self.stream_list[stream_id]['kill_request'] is not None:
@@ -1476,15 +1474,15 @@
         :param api: Setting this to `True` activates the creation of a Websocket API stream to send API requests via Websocket.
                     Needs `api_key` and `api_secret` in combination. This type of stream can not be combined with a UserData
                     stream or an other public endpoint. (Default is `False`)
         :type api: bool
         """
         if api is True:
             logger.info("BinanceWebSocketApiManager.create_websocket_uri(" + str(channels) + ", " +
-                        str(markets) + ", " + ", " + str(symbols) + ", " + str(api) + " - Created websocket URI for "
+                        str(markets) + ", " + ", " + str(symbols) + ", " + str(api) + ") - Created websocket URI for "
                         "stream_id=" + str(stream_id) + " is " + self.websocket_api_base_uri)
             return self.websocket_api_base_uri
         if isinstance(channels, bool):
             logger.error(f"BinanceWebSocketApiManager.create_websocket_uri({str(channels)}, {str(markets)}"
                          f", {str(symbols)}) - error_msg: Parameter `channels` must be str, tuple, list "
                          f"or a set!")
             return False
@@ -2482,15 +2480,19 @@
         :param stream_label: stream_label of the stream you search
         :type stream_label: str
         :return: stream_id or False
         """
         if stream_label:
             for stream_id in self.stream_list:
                 if self.stream_list[stream_id]['stream_label'] == stream_label:
+                    logger.debug(f"BinanceWebSocketApiManager.get_stream_id_by_label() - Found `stream_id` via `stream_label` "
+                                 f"`{stream_label}`")
                     return stream_id
+        logger.error(f"BinanceWebSocketApiManager.get_stream_id_by_label() - No `stream_id` found via `stream_label` "
+                     f"`{stream_label}`")
         return False
 
     def get_stream_info(self, stream_id):
         """
         Get all infos about a specific stream
 
         :param stream_id: id of a stream
@@ -2661,14 +2663,38 @@
             stream_statistic['stream_receives_per_day'] = stream_receives_per_second * 60 * 60 * 24
         if stream_statistic['uptime'] > 60 * 60 * 24 * 30:
             stream_statistic['stream_receives_per_month'] = stream_receives_per_second * 60 * 60 * 24 * 30
         if stream_statistic['uptime'] > 60 * 60 * 24 * 30 * 12:
             stream_statistic['stream_receives_per_year'] = stream_receives_per_second * 60 * 60 * 24 * 30 * 12
         return stream_statistic
 
+    def get_the_one_active_websocket_api(self):
+        """
+        This function is needed to simplify the access to the websocket API, if only one API stream exists it is clear
+        that only this stream can be used for the requests and therefore will be used.
+
+        :return: stream_id or False
+        """
+        found_entries = 0
+        found_stream_id = None
+        for stream_id in self.stream_list:
+            if self.stream_list[stream_id]['api'] is True:
+                found_entries += 1
+                found_stream_id = stream_id
+
+        if found_entries == 1:
+            # Its clear, there is only one valid connection to use, so we can take it!
+            logger.debug(f"BinanceWebSocketApiManager.get_the_one_active_websocket_api() - Found `stream_id` "
+                         f"`{found_stream_id}`")
+            return found_stream_id
+        else:
+            logger.error(f"BinanceWebSocketApiManager.get_the_one_active_websocket_api() - No valid `stream_id` found! "
+                         f"- `found_entries` = {found_entries}")
+            return False
+
     def get_total_received_bytes(self):
         """
         Get number of total received bytes
 
         :return: int
         """
         # how much bytes did we receive till now?
```

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restclient.py` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restclient.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,21 +29,18 @@
 # OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABIL-
 # ITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
 # SHALL THE AUTHOR BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
-import json
+from unicorn_binance_rest_api import BinanceRestApiManager
 import logging
-import requests
-import socket
 import threading
 import time
-from unicorn_binance_rest_api import BinanceRestApiManager
 
 logger = logging.getLogger("unicorn_binance_websocket_api")
 
 
 class BinanceWebSocketApiRestclient(object):
     def __init__(self, manager):
         """
@@ -160,24 +157,46 @@
                             ubra.MARGIN_API_URL = self.manager.restful_base_uri
                         response = ubra.isolated_margin_stream_get_listen_key(symbol=str(self.symbol), output="raw_data",
                                                                               throw_exception=False)
                     except AttributeError as error_msg:
                         logger.critical(f"BinanceWebSocketApiRestclient.get_listen_key() - error: 8 - "
                                         f"error_msg: {error_msg} - Can not acquire listen_key for isolated_margin!")
                         return False
+            elif self.manager.exchange == "binance.com-futures":
+                try:
+                    if self.manager.restful_base_uri is not None:
+                        ubra.FUTURES_URL = self.manager.restful_base_uri
+                    response = ubra.futures_stream_get_listen_key(output="raw_data", throw_exception=False)
+                except AttributeError as error_msg:
+                    logger.critical(f"BinanceWebSocketApiRestclient.get_listen_key() - error: 8 - "
+                                    f"error_msg: {error_msg} - Can not acquire listen_key for futures!!")
+                    return False
+            elif self.manager.exchange == "binance.com-coin_futures":
+                try:
+                    if self.manager.restful_base_uri is not None:
+                        ubra.FUTURES_COIN_URL = self.manager.restful_base_uri
+                    response = ubra.futures_coin_stream_get_listen_key(output="raw_data", throw_exception=False)
+                except AttributeError as error_msg:
+                    logger.critical(f"BinanceWebSocketApiRestclient.get_listen_key() - error: 8 - "
+                                    f"error_msg: {error_msg} - Can not acquire listen_key for coin futures!!")
+                    return False
             else:
                 try:
                     if self.manager.restful_base_uri is not None:
                         ubra.API_URL = self.manager.restful_base_uri
                     response = ubra.stream_get_listen_key(output="raw_data", throw_exception=False)
                 except AttributeError as error_msg:
                     logger.critical(f"BinanceWebSocketApiRestclient.get_listen_key() - error: 8 - "
-                                    f"error_msg: {error_msg} - Can not acquire listen_key!")
+                                    f"error_msg: {error_msg} - Can not acquire listen_key for exchange='"
+                                    f"{self.manager.exchange}'!")
                     return False
+            # used weight:
             self.manager.binance_api_status = ubra.get_used_weight()
+            weight = self.manager.binance_api_status['weight']
+            self.manager.binance_api_status['weight'] = 0 if weight is None else weight
             self.manager.binance_api_status['timestamp'] = time.time()
             try:
                 self.listen_key = response['listenKey']
                 self.last_static_ping_listen_key = time.time()
                 return response
             except KeyError:
                 return response
@@ -217,20 +236,31 @@
             if self.manager.exchange == "binance.com-isolated_margin" or \
                     self.manager.exchange == "binance.com-isolated_margin-testnet":
                 if self.manager.restful_base_uri is not None:
                     ubra.MARGIN_API_URL = self.manager.restful_base_uri
                 result = ubra.isolated_margin_stream_close(symbol=str(self.symbol), listenKey=str(self.listen_key),
                                                            throw_exception=False)
                 self.symbol = False
+            elif self.manager.exchange == "binance.com-futures":
+                if self.manager.restful_base_uri is not None:
+                    ubra.FUTURES_URL = self.manager.restful_base_uri
+                result = ubra.futures_stream_close(listenKey=str(self.listen_key), throw_exception=False)
+            elif self.manager.exchange == "binance.com-coin_futures":
+                if self.manager.restful_base_uri is not None:
+                    ubra.FUTURES_COIN_URL = self.manager.restful_base_uri
+                result = ubra.futures_coin_stream_close(listenKey=str(self.listen_key), throw_exception=False)
             else:
                 if self.manager.restful_base_uri is not None:
                     ubra.API_URL = self.manager.restful_base_uri
                 result = ubra.stream_close(listenKey=str(self.listen_key), throw_exception=False)
             self.listen_key = False
+            # used weight:
             self.manager.binance_api_status = ubra.get_used_weight()
+            weight = self.manager.binance_api_status['weight']
+            self.manager.binance_api_status['weight'] = 0 if weight is None else weight
             self.manager.binance_api_status['timestamp'] = time.time()
             return result
 
     def keepalive_listen_key(self,
                              stream_id=False,
                              api_key=False,
                              api_secret=False,
@@ -266,16 +296,26 @@
                                          warn_on_update=self.manager.warn_on_update)
             if self.manager.exchange == "binance.com-isolated_margin" or \
                     self.manager.exchange == "binance.com-isolated_margin-testnet":
                 if self.manager.restful_base_uri is not None:
                     ubra.MARGIN_API_URL = self.manager.restful_base_uri
                 result = ubra.isolated_margin_stream_keepalive(symbol=str(self.symbol), listenKey=str(self.listen_key),
                                                                throw_exception=False)
-                self.last_static_ping_listen_key = time.time()
+            elif self.manager.exchange == "binance.com-futures":
+                if self.manager.restful_base_uri is not None:
+                    ubra.FUTURES_URL = self.manager.restful_base_uri
+                result = ubra.futures_stream_keepalive(listenKey=str(self.listen_key), throw_exception=False)
+            elif self.manager.exchange == "binance.com-coin_futures":
+                if self.manager.restful_base_uri is not None:
+                    ubra.FUTURES_URL = self.manager.restful_base_uri
+                result = ubra.futures_stream_keepalive(listenKey=str(self.listen_key), throw_exception=False)
             else:
                 if self.manager.restful_base_uri is not None:
                     ubra.API_URL = self.manager.restful_base_uri
                 result = ubra.stream_keepalive(listenKey=str(self.listen_key), throw_exception=False)
-                self.last_static_ping_listen_key = time.time()
+            self.last_static_ping_listen_key = time.time()
+            # used weight:
             self.manager.binance_api_status = ubra.get_used_weight()
+            weight = self.manager.binance_api_status['weight']
+            self.manager.binance_api_status['weight'] = 0 if weight is None else weight
             self.manager.binance_api_status['timestamp'] = time.time()
             return result
```

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/restserver.py` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restserver.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api/sockets.py` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/sockets.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 from unicorn_fy.unicorn_fy import UnicornFy
 import asyncio
 import ujson as json
 import logging
 import sys
 import uuid
 import websockets
-# import websockets.speedups
 
 logger = logging.getLogger("unicorn_binance_websocket_api")
 
 
 class BinanceWebSocketApiSocket(object):
     def __init__(self, manager, stream_id, channels, markets):
         self.manager = manager
@@ -114,62 +113,89 @@
                                                            self.manager.max_send_messages_per_second_reserve
                             idle_time = 1/max_subscriptions_per_second
                             await asyncio.sleep(idle_time)
                     try:
                         try:
                             received_stream_data_json = await websocket.receive()
                         except asyncio.TimeoutError:
-                            # Timeout from `asyncio.wait_for()` which we use to keep the loop running even if we dont
+                            # Timeout from `asyncio.wait_for()` which we use to keep the loop running even if we don't
                             # receive new records via websocket.
                             logger.debug(f"BinanceWebSocketApiSocket.start_socket({str(self.stream_id)}, "
                                          f"{str(self.channels)}, {str(self.markets)} - Received inner "
-                                         f"asyncio.TimeoutError")
+                                         f"asyncio.TimeoutError (This is no ERROR, its exactly what we want!)")
                             continue
                         if self.manager.is_stop_request(self.stream_id):
                             self.manager.stream_is_stopping(self.stream_id)
                             await websocket.close()
                             sys.exit(0)
                         if received_stream_data_json is not None:
                             if self.output == "UnicornFy":
-                                if self.exchange == "binance.com":
-                                    received_stream_data = self.unicorn_fy.binance_com_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-testnet":
-                                    received_stream_data = self.unicorn_fy.binance_com_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-margin":
-                                    received_stream_data = self.unicorn_fy.binance_com_margin_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-margin-testnet":
-                                    received_stream_data = self.unicorn_fy.binance_com_margin_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-isolated_margin":
-                                    received_stream_data = self.unicorn_fy.binance_com_isolated_margin_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-isolated_margin-testnet":
-                                    received_stream_data = self.unicorn_fy.binance_com_isolated_margin_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-futures":
-                                    received_stream_data = self.unicorn_fy.binance_com_futures_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-futures-testnet":
-                                    received_stream_data = self.unicorn_fy.binance_com_futures_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.com-coin-futures" or self.exchange == "binance.com-coin_futures":
-                                    received_stream_data = self.unicorn_fy.binance_com_coin_futures_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.je":
-                                    received_stream_data = self.unicorn_fy.binance_je_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.us":
-                                    received_stream_data = self.unicorn_fy.binance_us_websocket(received_stream_data_json)
-                                elif self.exchange == "trbinance.com":
-                                    received_stream_data = self.unicorn_fy.trbinance_com_websocket(received_stream_data_json)
-                                elif self.exchange == "jex.com":
-                                    received_stream_data = self.unicorn_fy.jex_com_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.org":
-                                    received_stream_data = self.unicorn_fy.binance_org_websocket(received_stream_data_json)
-                                elif self.exchange == "binance.org-testnet":
-                                    received_stream_data = self.unicorn_fy.binance_org_websocket(received_stream_data_json)
+                                if self.manager.stream_list[self.stream_id]['api'] is False:
+                                    if self.exchange == "binance.com":
+                                        received_stream_data = self.unicorn_fy.binance_com_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-testnet":
+                                        received_stream_data = self.unicorn_fy.binance_com_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-margin":
+                                        received_stream_data = self.unicorn_fy.binance_com_margin_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-margin-testnet":
+                                        received_stream_data = self.unicorn_fy.binance_com_margin_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-isolated_margin":
+                                        received_stream_data = self.unicorn_fy.binance_com_isolated_margin_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-isolated_margin-testnet":
+                                        received_stream_data = self.unicorn_fy.binance_com_isolated_margin_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-futures":
+                                        received_stream_data = self.unicorn_fy.binance_com_futures_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-futures-testnet":
+                                        received_stream_data = self.unicorn_fy.binance_com_futures_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.com-coin-futures" or self.exchange == "binance.com-coin_futures":
+                                        received_stream_data = self.unicorn_fy.binance_com_coin_futures_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.je":
+                                        received_stream_data = self.unicorn_fy.binance_je_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.us":
+                                        received_stream_data = self.unicorn_fy.binance_us_websocket(received_stream_data_json)
+                                    elif self.exchange == "trbinance.com":
+                                        received_stream_data = self.unicorn_fy.trbinance_com_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.org":
+                                        received_stream_data = self.unicorn_fy.binance_org_websocket(received_stream_data_json)
+                                    elif self.exchange == "binance.org-testnet":
+                                        received_stream_data = self.unicorn_fy.binance_org_websocket(received_stream_data_json)
+                                    else:
+                                        received_stream_data = received_stream_data_json
                                 else:
-                                    received_stream_data = received_stream_data_json
+                                    # WS API does not need to get unicornfied, just turn it into a dict:
+                                    received_stream_data = json.loads(received_stream_data_json)
                             elif self.output == "dict":
                                 received_stream_data = json.loads(received_stream_data_json)
                             else:
                                 received_stream_data = received_stream_data_json
+
+                            if self.manager.stream_list[self.stream_id]['api'] is True:
+                                return_response_by_request_id = None
+                                with self.manager.return_response_lock:
+                                    for request_id in self.manager.return_response:
+                                        if request_id in received_stream_data_json:
+                                            return_response_by_request_id = request_id
+                                            break
+                                if return_response_by_request_id is not None:
+                                    self.manager.return_response[return_response_by_request_id]['response_value'] = received_stream_data
+                                    self.manager.return_response[return_response_by_request_id]['event_return_response'].set()
+                                    continue
+
+                                process_by_request_id = None
+                                with self.manager.process_response_lock:
+                                    for request_id in self.manager.process_response:
+                                        if request_id in received_stream_data_json:
+                                            process_by_request_id = request_id
+                                            break
+                                if process_by_request_id is not None:
+                                    self.manager.process_response[process_by_request_id]['callback_function'](received_stream_data)
+                                    with self.manager.process_response_lock:
+                                        del self.manager.process_response[process_by_request_id]
+                                    continue
+
                             try:
                                 stream_buffer_name = self.manager.stream_list[self.stream_id]['stream_buffer_name']
                             except KeyError:
                                 stream_buffer_name = False
                             if stream_buffer_name:
                                 # if create_stream() got a stram_buffer_name -> use it
                                 self.manager.add_to_stream_buffer(received_stream_data,
```

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/PKG-INFO` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-websocket-api
-Version: 1.45.2
-Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, jex, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
+Version: 1.46.0
+Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-websocket-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-websocket-api.docs.lucit.tech
 Project-URL: Wiki, https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki
@@ -61,27 +61,28 @@
 
 [Description](#description) | [Live Demo](#live-demo) | [Installation](#installation-and-upgrade) | [How To](#howto) |
 [Documentation](#documentation) | [Examples](#examples) | [Change Log](#change-log) | [Wiki](#wiki) | [Social](#social) |
 [Notifications](#receive-notifications) | [Bugs](#how-to-report-bugs-or-suggest-improvements) | 
 [Contributing](#contributing) | [Leave a review](#you-want-to-say-thank-you) | [Disclaimer](#disclaimer) | [Commercial Support](#commercial-support)
 
 An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, 
-com-isolated_margin+testnet, com-futures+testnet, com-coin_futures, us, tr, jex, dex/chain+testnet) 
+com-isolated_margin+testnet, com-futures+testnet, com-coin_futures, us, tr, dex/chain+testnet) 
 in a easy, fast, flexible, robust and fully-featured way. 
 
 Part of ['UNICORN Binance Suite'](https://www.lucit.tech/unicorn-binance-suite.html).
 
+## Receive Data from Binance WebSockets
 ### [Create a multiplex websocket connection](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.create_stream) to Binance with a [`stream_buffer`](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/%60stream_buffer%60) with just 3 lines of code:
 
 ```
 import unicorn_binance_websocket_api
 
 
 ubwa = unicorn_binance_websocket_api.BinanceWebSocketApiManager(exchange="binance.com")
-ubwa.create_stream(['trade', 'kline_1m'], ['btcusdt', 'bnbbtc', 'ethbtc'])
+ubwa.create_stream(channels=['trade', 'kline_1m'], markets=['btcusdt', 'bnbbtc', 'ethbtc'])
 ```
 
 #### And 4 more lines to print the receives:
 ```
 while True:
     oldest_data_from_stream_buffer = ubwa.pop_stream_data_from_stream_buffer()
     if oldest_data_from_stream_buffer:
@@ -94,15 +95,16 @@
 
 
 def process_new_receives(stream_data):
     print(str(stream_data))
 
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
-ubwa.create_stream(['trade', 'kline_1m'], ['btcusdt', 'bnbbtc', 'ethbtc'], process_stream_data=process_new_receives)
+ubwa.create_stream(channels=['trade', 'kline_1m'], markets=['btcusdt', 'bnbbtc', 'ethbtc'], 
+                   process_stream_data=process_new_receives)
 ```
 
 Basically that's it, but there are more options.
 
 ### Convert received raw webstream data into well-formed Python dictionaries with [UnicornFy](https://www.lucit.tech/unicorn-fy.html):
 ```
 unicorn_fied_stream_data = UnicornFy.binance_com_websocket(oldest_data_from_stream_buffer)
@@ -115,22 +117,23 @@
 ```
 
 ### [Subscribe](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.subscribe_to_stream) / [unsubscribe](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.unsubscribe_from_stream) new markets and channels:
 ```
 markets = ['engbtc', 'zileth']
 channels = ['kline_5m', 'kline_15m', 'kline_30m', 'kline_1h', 'kline_12h', 'depth5']
 
-ubwa.subscribe_to_stream(stream_id, channels=channels, markets=markets)
+ubwa.subscribe_to_stream(stream_id=stream_id, channels=channels, markets=markets)
 
-ubwa.unsubscribe_from_stream(stream_id, markets=markets)
+ubwa.unsubscribe_from_stream(stream_id=stream_id, markets=markets)
 
-ubwa.unsubscribe_from_stream(stream_id, channels=channels)
+ubwa.unsubscribe_from_stream(stream_id=stream_id, channels=channels)
 ```
 
-### [Place orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.create_order), [cancel orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.cancel_order) or [send other requests](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#module-unicorn_binance_websocket_api.api) via WebSocket.
+## Send Requests to Binance WebSocket API
+### [Place orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.create_order), [cancel orders](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.api.BinanceWebSocketApiApi.cancel_order) or [send other requests](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#module-unicorn_binance_websocket_api.api) via WebSocket:
 ```
 from unicorn_binance_websocket_api.manager import BinanceWebSocketApiManager
 
 
 def process_api_responses(stream_data):
     print(str(stream_data))
 
@@ -138,19 +141,23 @@
 api_key = "YOUR BINANCE API KEY"
 api_secret = "YOUR BINANCE API SECRET"
 
 ubwa = BinanceWebSocketApiManager(exchange="binance.com")
 api_stream = ubwa.create_stream(api=True, api_key=api_key, api_secret=api_secret,
                                 process_stream_data=process_api_responses)
                                 
-orig_client_order_id = ubwa.api.create_order(stream_id=api_stream, price=1.1, order_type="LIMIT",
+orig_client_order_id = ubwa.api.create_order(order_type="LIMIT", price=1.1, 
                                              quantity=15.0, side="SELL", symbol="BUSDUSDT")
-ubwa.api.cancel_order(stream_id=api_stream, symbol="BUSDUSDT", orig_client_order_id=orig_client_order_id)                                             
+ubwa.api.cancel_order(orig_client_order_id=orig_client_order_id, symbol="BUSDUSDT")                                             
 ```
 
+[Here](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404) you can find a complete 
+guide on 
+[how to process requests via the Binance WebSocket API](https://medium.lucit.tech/create-and-cancel-orders-via-websocket-on-binance-7f828831404)!
+
 ### Get the right [logger](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/Logging):
 ```
 logging.getLogger("unicorn_binance_websocket_api")
 ```
 
 [Discover even more possibilities](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html)
 or [use this script](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_stream_everything.py) 
@@ -171,24 +178,22 @@
 [Binance Isolated Margin](https://binance-docs.github.io/apidocs/spot/en/#listen-key-isolated-margin)
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Futures](https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams) 
 ([+Testnet](https://testnet.binancefuture.com)), 
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
 [Binance US](https://github.com/binance-us/binance-official-api-docs), 
 [Binance TR](https://www.trbinance.com/apidocs), 
-[Binance JEX](https://jexapi.github.io/api-doc/spot.html#web-socket-streams), 
 [Binance DEX](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and 
 [Binance DEX Testnet](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and supports sending requests 
 to the [Binance Websocket API](https://developers.binance.com/docs/binance-trading-api/websocket_api) and the streaming 
 of all public streams like trade, kline, ticker, depth, bookTicker, forceOrder, compositeIndex, blockheight etc. and 
 also all private userData streams which needs to be used with a valid api_key and api_secret from the Binance Exchange 
 [www.binance.com](https://www.binance.com/userCenter/createApi.html), 
-[testnet.binance.vision](https://testnet.binance.vision/), 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) or 
-[www.jex.com](https://www.jex.com/userCenter/createApi.html) - for the DEX you need a user address from 
+[testnet.binance.vision](https://testnet.binance.vision/) or 
+[www.binance.us](https://www.binance.us/userCenter/createApi.html) - for the DEX you need a user address from 
 [www.binance.org](https://www.binance.org/en/create) or [testnet.binance.org](https://testnet.binance.org/en/create) 
 and you can [get funds](https://www.binance.vision/tutorials/binance-dex-funding-your-testnet-account) for the testnet.
 
 Use the [UNICORN Binance REST API](https://www.lucit.tech/unicorn-binance-rest-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance WebSocket API?
 - Fully managed websockets and 100% auto-reconnect! Also handles maintenance windows!
@@ -209,15 +214,14 @@
 | [Binance Isolated Margin](https://www.binance.com)                 | `binance.com-isolated_margin`         |
 | [Binance Isolated Margin Testnet](https://testnet.binance.vision/) | `binance.com-isolated_margin-testnet` |
 | [Binance USD-M Futures](https://www.binance.com)                   | `binance.com-futures`                 |
 | [Binance USD-M Futures Testnet](https://testnet.binancefuture.com) | `binance.com-futures-testnet`         |
 | [Binance Coin-M Futures](https://www.binance.com)                  | `binance.com-coin_futures`            |
 | [Binance US](https://www.binance.us)                               | `binance.us`                          |
 | [Binance TR](https://www.trbinance.com)                            | `trbinance.com`                       |
-| [Binance JEX](https://www.jex.com)                                 | `jex.com`                             |
 | [Binance DEX](https://www.binance.org)                             | `binance.org`                         |
 | [Binance DEX Testnet](https://testnet.binance.org)                 | `binance.org-testnet`                 |
 
 - Streams are processing asynchronous/concurrent (Python asyncio) and each stream is started in a separate thread, so 
 you dont need to deal with asyncio in your code!
 
 - Supports 
@@ -295,17 +299,19 @@
 [![icinga2-demo](https://raw.githubusercontent.com/lucit-systems-and-development/unicorn-binance-websocket-api/master/images/misc/icinga.png)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/wiki/UNICORN-Monitoring-API-Service)
 
 - Integration of [test cases](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml) and [examples](#examples).
 
 - Customizable base URL.
 
 - *Socks5 Proxy* support:
+
   ```
   ubwa = BinanceWebSocketApiManager(exchange="binance.com", socks5_proxy_server="127.0.0.1:9050") 
   ```
+  
   Read the [docs](https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager)
   or this [how to](https://medium.com/@oliverzehentleitner/how-to-connect-to-binance-com-websockets-using-python-via-a-socks5-proxy-3c5a3e063f12) 
   for more information or try 
   [example_socks5_proxy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_socks5_proxy.py).
 
 - Excessively tested on Linux, Mac and Windows
 
@@ -342,18 +348,18 @@
 ### From source of the latest release with PIP from [Github](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 #### Linux, macOS, ...
 Run in bash:
 
 `pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/$(curl -s https://api.github.com/repos/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest | grep -oP '"tag_name": "\K(.*)(?=")').tar.gz --upgrade`
 
 #### Windows
-Use the below command with the version (such as 1.43.3) you determined 
+Use the below command with the version (such as 1.46.0) you determined 
 [here](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest):
 
-`pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/1.43.3.tar.gz --upgrade`
+`pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/archive/1.46.0.tar.gz --upgrade`
 ### From the latest source (dev-stage) with PIP from [Github](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 This is not a release version and can not be considered to be stable!
 
 `pip install https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/tarball/master --upgrade`
 
 ### [Conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html), [Virtualenv](https://virtualenv.pypa.io/en/latest/) or plain [Python](https://www.python.org)
 Download the [latest release](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases/latest) 
@@ -372,15 +378,14 @@
 - [Modules](https://unicorn-binance-websocket-api.docs.lucit.tech/modules.html)
 
 ## Examples
 - [example_binance_coin_futures.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_coin_futures.py)
 - [example_binance_dex.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_dex.py)
 - [example_binance_futures.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_futures.py)
 - [example_binance_futures_1s.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_futures_1s.py)
-- [example_binance_jex.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_jex.py)
 - [example_binance_us.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_binance_us.py)
 - [example_bookticker.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_bookticker.py)
 - [example_ctrl-c.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_ctrl-c.py)
 - [example_demo.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_demo.py)
 - [example_easy_migration_from_python-binance.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_easy_migration_from_python-binance.py)
 - [example_interactive_mode.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_interactive_mode.py)
 - [example_kline_1m_with_unicorn_fy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_kline_1m_with_unicorn_fy.py)
@@ -438,15 +443,14 @@
 
 Follow us on [Twitter](https://twitter.com/LUCIT_SysDev) or on [Facebook](https://www.facebook.com/lucit.systems.and.development) for general news about the [unicorn-binance-suite](https://www.lucit.tech/unicorn-binance-suite.html)!
 
 To receive news (like inspection windows/maintenance) about the Binance API`s subscribe to their telegram groups: 
 
 - [https://t.me/binance_api_announcements](https://t.me/binance_api_announcements)
 - [https://t.me/binance_api_english](https://t.me/binance_api_english)
-- [https://t.me/Binance_JEX_EN](https://t.me/Binance_JEX_EN)
 - [https://t.me/Binance_USA](https://t.me/Binance_USA)
 - [https://t.me/TRBinanceTR](https://t.me/TRBinanceTR)
 - [https://t.me/BinanceDEXchange](https://t.me/BinanceDEXchange)
 - [https://t.me/BinanceExchange](https://t.me/BinanceExchange)
 
 ## How to report Bugs or suggest Improvements?
 [List of planned features](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement) - 
@@ -478,15 +482,15 @@
 ## Disclaimer
 This project is for informational purposes only. You should not construe this information or any other material as 
 legal, tax, investment, financial or other advice. Nothing contained herein constitutes a solicitation, recommendation, 
 endorsement or offer by us or any third party provider to buy or sell any securities or other financial instruments in 
 this or any other jurisdiction in which such solicitation or offer would be unlawful under the securities laws of such 
 jurisdiction.
 
-***If you intend to use real money, use it at your own risk.***
+### If you intend to use real money, use it at your own risk!
 
 Under no circumstances will we be responsible or liable for any claims, damages, losses, expenses, costs or liabilities 
 of any kind, including but not limited to direct or indirect damages for loss of profits.
 
 ### SOCKS5 Proxy / Geoblocking
 We would like to explicitly point out that in our opinion US citizens are exclusively authorized to trade on Binance.US 
 and that this restriction must not be circumvented!
```

### Comparing `unicorn-binance-websocket-api-1.45.2/unicorn_binance_websocket_api.egg-info/SOURCES.txt` & `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

