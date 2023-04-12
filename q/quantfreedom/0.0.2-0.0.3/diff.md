# Comparing `tmp/quantfreedom-0.0.2.tar.gz` & `tmp/quantfreedom-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfreedom-0.0.2.tar", last modified: Tue Apr 11 16:07:01 2023, max compression
+gzip compressed data, was "quantfreedom-0.0.3.tar", last modified: Wed Apr 12 01:24:19 2023, max compression
```

## Comparing `quantfreedom-0.0.2.tar` & `quantfreedom-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.263799 quantfreedom-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-03-29 16:20:45.000000 quantfreedom-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     9399 2023-04-11 16:07:01.263799 quantfreedom-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8179 2023-03-31 02:51:25.000000 quantfreedom-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.230474 quantfreedom-0.0.2/quantfreedom/
--rw-rw-rw-   0        0        0      701 2023-04-06 12:23:09.000000 quantfreedom-0.0.2/quantfreedom/__init__.py
--rw-rw-rw-   0        0        0    15199 2023-04-11 15:51:19.000000 quantfreedom-0.0.2/quantfreedom/_doc_test.py
--rw-rw-rw-   0        0        0    10211 2023-04-11 14:49:54.000000 quantfreedom-0.0.2/quantfreedom/_testing.py
--rw-rw-rw-   0        0        0      946 2023-04-09 19:14:42.000000 quantfreedom-0.0.2/quantfreedom/_typing.py
--rw-rw-rw-   0        0        0       24 2023-03-29 16:20:45.000000 quantfreedom-0.0.2/quantfreedom/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.248990 quantfreedom-0.0.2/quantfreedom/base/
--rw-rw-rw-   0        0        0       38 2023-03-30 14:02:24.000000 quantfreedom-0.0.2/quantfreedom/base/__init__.py
--rw-rw-rw-   0        0        0    12170 2023-04-11 14:16:02.000000 quantfreedom-0.0.2/quantfreedom/base/base.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.250985 quantfreedom-0.0.2/quantfreedom/data/
--rw-rw-rw-   0        0        0      115 2023-04-04 16:06:19.000000 quantfreedom-0.0.2/quantfreedom/data/__init__.py
--rw-rw-rw-   0        0        0     8126 2023-04-11 14:25:03.000000 quantfreedom-0.0.2/quantfreedom/data/ccxtdata.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.251986 quantfreedom-0.0.2/quantfreedom/enums/
--rw-rw-rw-   0        0        0       40 2023-03-30 14:02:24.000000 quantfreedom-0.0.2/quantfreedom/enums/__init__.py
--rw-rw-rw-   0        0        0     8082 2023-04-09 18:54:20.000000 quantfreedom-0.0.2/quantfreedom/enums/enums.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.252985 quantfreedom-0.0.2/quantfreedom/evaluators/
--rw-rw-rw-   0        0        0       50 2023-03-30 14:02:24.000000 quantfreedom-0.0.2/quantfreedom/evaluators/__init__.py
--rw-rw-rw-   0        0        0    31984 2023-04-10 04:39:02.000000 quantfreedom-0.0.2/quantfreedom/evaluators/evaluators.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.254986 quantfreedom-0.0.2/quantfreedom/indicators/
--rw-rw-rw-   0        0        0       49 2023-03-30 14:02:24.000000 quantfreedom-0.0.2/quantfreedom/indicators/__init__.py
--rw-rw-rw-   0        0        0    15263 2023-04-06 19:44:29.000000 quantfreedom-0.0.2/quantfreedom/indicators/talib_ind.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.258803 quantfreedom-0.0.2/quantfreedom/nb/
--rw-rw-rw-   0        0        0      212 2023-03-30 14:02:23.000000 quantfreedom-0.0.2/quantfreedom/nb/__init__.py
--rw-rw-rw-   0        0        0    16293 2023-04-09 18:49:08.000000 quantfreedom-0.0.2/quantfreedom/nb/buy_funcs.py
--rw-rw-rw-   0        0        0    12476 2023-04-07 13:57:33.000000 quantfreedom-0.0.2/quantfreedom/nb/execute_funcs.py
--rw-rw-rw-   0        0        0    28820 2023-04-09 18:49:24.000000 quantfreedom-0.0.2/quantfreedom/nb/helper_funcs.py
--rw-rw-rw-   0        0        0    16308 2023-04-09 18:49:28.000000 quantfreedom-0.0.2/quantfreedom/nb/sell_funcs.py
--rw-rw-rw-   0        0        0    27311 2023-04-09 18:49:32.000000 quantfreedom-0.0.2/quantfreedom/nb/simulate.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.261799 quantfreedom-0.0.2/quantfreedom/plotting/
--rw-rw-rw-   0        0        0       49 2023-04-08 20:59:59.000000 quantfreedom-0.0.2/quantfreedom/plotting/__init__.py
--rw-rw-rw-   0        0        0    10761 2023-04-08 21:45:05.000000 quantfreedom-0.0.2/quantfreedom/plotting/plot_helper_functions.py
--rw-rw-rw-   0        0        0     8294 2023-04-09 16:03:12.000000 quantfreedom-0.0.2/quantfreedom/plotting/plotting_main.py
--rw-rw-rw-   0        0        0    13294 2023-04-08 20:47:24.000000 quantfreedom-0.0.2/quantfreedom/plotting/replay.py
--rw-rw-rw-   0        0        0        0 2023-04-02 21:46:09.000000 quantfreedom-0.0.2/quantfreedom/plotting/temp.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.262798 quantfreedom-0.0.2/quantfreedom/utils/
--rw-rw-rw-   0        0        0      117 2023-04-08 04:16:16.000000 quantfreedom-0.0.2/quantfreedom/utils/__init__.py
--rw-rw-rw-   0        0        0     3012 2023-04-08 20:10:04.000000 quantfreedom-0.0.2/quantfreedom/utils/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:07:01.248228 quantfreedom-0.0.2/quantfreedom.egg-info/
--rw-rw-rw-   0        0        0     9399 2023-04-11 16:07:01.000000 quantfreedom-0.0.2/quantfreedom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2023-04-11 16:07:01.000000 quantfreedom-0.0.2/quantfreedom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 16:07:01.000000 quantfreedom-0.0.2/quantfreedom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      606 2023-04-11 16:07:01.000000 quantfreedom-0.0.2/quantfreedom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 16:07:01.000000 quantfreedom-0.0.2/quantfreedom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 16:07:01.263799 quantfreedom-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2784 2023-04-11 16:05:24.000000 quantfreedom-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.391476 quantfreedom-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-03-29 16:20:45.000000 quantfreedom-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     9399 2023-04-12 01:24:19.390475 quantfreedom-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8179 2023-03-31 02:51:25.000000 quantfreedom-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.354789 quantfreedom-0.0.3/quantfreedom/
+-rw-rw-rw-   0        0        0      701 2023-04-11 17:50:38.000000 quantfreedom-0.0.3/quantfreedom/__init__.py
+-rw-rw-rw-   0        0        0    15199 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/_doc_test.py
+-rw-rw-rw-   0        0        0    10209 2023-04-11 17:59:26.000000 quantfreedom-0.0.3/quantfreedom/_testing.py
+-rw-rw-rw-   0        0        0      946 2023-04-09 19:14:42.000000 quantfreedom-0.0.3/quantfreedom/_typing.py
+-rw-rw-rw-   0        0        0       24 2023-04-12 01:20:01.000000 quantfreedom-0.0.3/quantfreedom/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.374563 quantfreedom-0.0.3/quantfreedom/base/
+-rw-rw-rw-   0        0        0       38 2023-03-30 14:02:24.000000 quantfreedom-0.0.3/quantfreedom/base/__init__.py
+-rw-rw-rw-   0        0        0    12170 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/base/base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.375552 quantfreedom-0.0.3/quantfreedom/data/
+-rw-rw-rw-   0        0        0       31 2023-04-11 19:21:38.000000 quantfreedom-0.0.3/quantfreedom/data/__init__.py
+-rw-rw-rw-   0        0        0     7417 2023-04-11 19:13:23.000000 quantfreedom-0.0.3/quantfreedom/data/data_dl.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.377552 quantfreedom-0.0.3/quantfreedom/enums/
+-rw-rw-rw-   0        0        0       40 2023-03-30 14:02:24.000000 quantfreedom-0.0.3/quantfreedom/enums/__init__.py
+-rw-rw-rw-   0        0        0     8082 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/enums/enums.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.378553 quantfreedom-0.0.3/quantfreedom/evaluators/
+-rw-rw-rw-   0        0        0       50 2023-03-30 14:02:24.000000 quantfreedom-0.0.3/quantfreedom/evaluators/__init__.py
+-rw-rw-rw-   0        0        0    31974 2023-04-11 19:23:01.000000 quantfreedom-0.0.3/quantfreedom/evaluators/evaluators.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.380554 quantfreedom-0.0.3/quantfreedom/indicators/
+-rw-rw-rw-   0        0        0       49 2023-04-11 19:23:10.000000 quantfreedom-0.0.3/quantfreedom/indicators/__init__.py
+-rw-rw-rw-   0        0        0    15760 2023-04-11 18:18:08.000000 quantfreedom-0.0.3/quantfreedom/indicators/talib_ind.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.384478 quantfreedom-0.0.3/quantfreedom/nb/
+-rw-rw-rw-   0        0        0      212 2023-03-30 14:02:23.000000 quantfreedom-0.0.3/quantfreedom/nb/__init__.py
+-rw-rw-rw-   0        0        0    16293 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/buy_funcs.py
+-rw-rw-rw-   0        0        0    12476 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/execute_funcs.py
+-rw-rw-rw-   0        0        0    28820 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/helper_funcs.py
+-rw-rw-rw-   0        0        0    16308 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/sell_funcs.py
+-rw-rw-rw-   0        0        0    27311 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/nb/simulate.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.388475 quantfreedom-0.0.3/quantfreedom/plotting/
+-rw-rw-rw-   0        0        0       49 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/__init__.py
+-rw-rw-rw-   0        0        0    10761 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/plot_helper_functions.py
+-rw-rw-rw-   0        0        0     8294 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/plotting_main.py
+-rw-rw-rw-   0        0        0    13294 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/plotting/replay.py
+-rw-rw-rw-   0        0        0        0 2023-04-02 21:46:09.000000 quantfreedom-0.0.3/quantfreedom/plotting/temp.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.389475 quantfreedom-0.0.3/quantfreedom/utils/
+-rw-rw-rw-   0        0        0      117 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/utils/__init__.py
+-rw-rw-rw-   0        0        0     3012 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/quantfreedom/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:24:19.372549 quantfreedom-0.0.3/quantfreedom.egg-info/
+-rw-rw-rw-   0        0        0     9399 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      606 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 01:24:19.000000 quantfreedom-0.0.3/quantfreedom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 01:24:19.391476 quantfreedom-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2784 2023-04-11 17:47:14.000000 quantfreedom-0.0.3/setup.py
```

### Comparing `quantfreedom-0.0.2/LICENSE` & `quantfreedom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/PKG-INFO` & `quantfreedom-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfreedom
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/QuantFreedom1022/quantfreedom
 Author: Quant Freedom
 Author-email: QuantFreedom1022@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quantfreedom-0.0.2/README.md` & `quantfreedom-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/__init__.py` & `quantfreedom-0.0.3/quantfreedom/__init__.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/_doc_test.py` & `quantfreedom-0.0.3/quantfreedom/_doc_test.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/_testing.py` & `quantfreedom-0.0.3/quantfreedom/_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Notes
 -----
     This is an example of an indented section. It's like any other section,
     but the body is indented to help it stand out from surrounding text.
 
 If a section is indented, then a section break is created by
-resuming unindented text.
+resuming unindent text.
 
 Attributes
 ----------
 module_level_variable1 : int
     Module level variables may be documented in either the ``Attributes``
     section of the module docstring, or in an inline docstring immediately
     following the variable.
```

### Comparing `quantfreedom-0.0.2/quantfreedom/_typing.py` & `quantfreedom-0.0.3/quantfreedom/_typing.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/base/base.py` & `quantfreedom-0.0.3/quantfreedom/base/base.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/data/ccxtdata.py` & `quantfreedom-0.0.3/quantfreedom/data/data_dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,188 +1,184 @@
 import ccxt
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 from quantfreedom._typing import Union
 from re import sub
 
-
-class CCXTData:
-    @classmethod
-    def data_download(
-        cls,
-        exchange: str,
-        start: str,
-        end: str,
-        symbols: Union[str, list],
-        timeframe: str,
-        drop_volume: bool = True,
-        remove_rate_limit: bool = False,
-        bars_per_loop: int = 200,
-    ):
-        """
-        Function Name
-        -------------
-        data_download
-
-        Quick Summary
-        -------------
-        Download Data using CCXT. Go here to find a list of exchanges http://docs.ccxt.com/#/README?id=exchanges
-
-        Explainer Video
-        ---------------
-        https://youtu.be/yDNPhgO-450
-
-        Parameters
-        ----------
-        cls: self
-            passing all the information from the created class
-        exchange : str
-            'bybit' or 'binance' or whatever exchange works with ccxt
-        start : str
-            needs to be in this format '2022-01-01T00:00:00Z'
-        end : str
-            needs to be in this format '2022-01-01T00:00:00Z'
-        symbol : list or str
-            This will depend on the exchange for bybit it would be 'BTCUSDT' you will have to look this up on ccxt if you need to know.
-            You can send this as a list of symbols or just one symbol.
-            Here is an example of how to get the symbols list from bybit.
-            ```python
-            import ccxt
-            exh = ccxt.bybit()
-            exh.load_markets()
-            exh.symbols
-            ```
-        timeframe : str
-            '1m', '5m', '1h' '4h' '1d' '1w'
-        drop_volume: bool = True
-            Set this to False if you want to keep volume data.
-        remove_rate_limit: bool = False
-            This is the default rate limit the exchange asks for. If you remove it then its possible that if you are trying to get tons and tons of data from the exchange they could ban you or time you out.
-        bars_per_loop: int = 200
-            How many bars you want to grab at a time. Some exchanges let you grab more info per loop and some don't. I don't think grabbing more would make anything faster but you can try if the exchange allows for more. You would have to do your research and figure out how man bars but i know bybit says you can grab a max of 200 and apparently binance lets you grab up to 1000.
-
-        Returns
-        -------
-            Pandas dataframe of prices
-        """
-        if remove_rate_limit:
-            exchange = getattr(ccxt, exchange)()
-        else:
-            exchange = getattr(ccxt, exchange)({"enableRateLimit": True})
-        print("Loading exchange data")
-        exchange.load_markets()
-        # exchange.verbose = True  # uncomment for debugging purposes if necessary
-        start = exchange.parse8601(start)
-        end = exchange.parse8601(end)
-        timeframe = timeframe.lower()
-        if not isinstance(symbols, list):
-            symbols = [symbols]
-        if not all(isinstance(x, str) for x in symbols):
-            raise ValueError("your symbols must be strings")
-
-        symbols = sorted(symbols)
-        timeframe_int = int(sub(r"\D", "", timeframe))
-        timeframe_str = sub(r"\d", "", timeframe)
-        len_symbols = len(symbols)
-        if timeframe_str == "m":
-            time_in = 1000 * 60
-        elif timeframe_str == "h":
-            time_in = 1000 * 60 * 60
-        elif timeframe_str == "d":
-            time_in = 1000 * 60 * 60 * 24
-        elif timeframe_str == "w":
-            time_in = 1000 * 60 * 60 * 24 * 7
-        elif timeframe_str == "m":
-            time_in = 1000 * 60 * 60 * 24 * 7 * 12
-        else:
-            raise ValueError("something wrong with your timeframe")
-
-        x = start
-        timelist = [x]
-        while x < end:
-            x += time_in * timeframe_int
-            timelist.append(x)
-
-        final_df = pd.DataFrame(
-            columns=pd.MultiIndex.from_tuples(
-                tuples=[],
-                name=["symbol", "candle_info"],
-            ),
-            index=pd.Index(
-                data=pd.to_datetime(timelist, unit="ms"),
-                name="open_time",
-            ),
-        )
-        # Example if you selected your timeframe as 30 minute candles
-
-        # Get the distance between the end date and start date in miliseconds
-        # Divide that by the amount of miliseconds in what ever timeframe you set ex: there are 60,000 miliseconds in one minute.
-        # Then you divide that by the number for the timeframe you set like 30 for 30 minutes to get the amount of 30 min bars in that distance of time
-        # Then divide by limit because that is the amount of rows of data you can return
-        # Then add one because that is the amount of loops we will have to do
-        # then multiple by the amount of symbols so if we have to do 2 loops per symbol and we have 2 symbols we have to do a total of 4 loops
-        # Then last we do + len of symbols because we will do an extra pbar update after we create the dataframe
-        num_candles_per_coin = ((end - start) / time_in) / timeframe_int
-        total_tqdm = (
-            (int(num_candles_per_coin / bars_per_loop) + 1) * len_symbols
-        ) + len_symbols
-        print(
-            f"Total possible rows of data to be download: {int(num_candles_per_coin)}\n"
-            f"Total possible candles to be download: {int(num_candles_per_coin) * len_symbols}\n"
-            f"It could finish earlier than expected because maybe not all coins have data starting from the start date selected."
-        )
-        with tqdm(total=total_tqdm) as pbar:
-            # with tqdm(total=96*2) as pbar:
-            for symbol in symbols:
-                all_ohlcvs = []
-                temp_end = end
-                pbar.set_description(f"Downloading {symbol}")
-                while True:
-                    try:
-                        ohlcvs = exchange.fetch_ohlcv(
-                            symbol=symbol,
-                            timeframe=timeframe,
-                            since=start,
-                            limit=bars_per_loop,
-                            params={"end": temp_end},
-                        )
-                        all_ohlcvs += ohlcvs
-                        if len(ohlcvs):
-                            temp_end = ohlcvs[0][0] - 1
-                            pbar.update(1)
-                        else:
-                            break
-
-                    except Exception as e:
-                        print(type(e).__name__, str(e))
-
-                if all_ohlcvs:
-                    all_ohlcvs = np.array(all_ohlcvs)
-                    data_columns = pd.MultiIndex.from_tuples(
-                        [
-                            (symbol, "open"),
-                            (symbol, "high"),
-                            (symbol, "low"),
-                            (symbol, "close"),
-                            (symbol, "volume"),
-                        ],
-                        name=["symbol", "candle_info"],
-                    )
-                    data_index = pd.Index(
-                        data=pd.to_datetime(all_ohlcvs[:, 0].flatten(), unit="ms"),
-                        name="open_time",
-                    )
-                    data = pd.DataFrame(
-                        all_ohlcvs[:, 1:],
-                        columns=data_columns,
-                        index=data_index,
+def data_download_from_ccxt(
+    exchange: str,
+    start: str,
+    end: str,
+    symbols: Union[str, list],
+    timeframe: str,
+    drop_volume: bool = True,
+    remove_rate_limit: bool = False,
+    bars_per_loop: int = 200,
+):
+    """
+    Function Name
+    -------------
+    data_download
+
+    Quick Summary
+    -------------
+    Download Data using CCXT. Go here to find a list of exchanges http://docs.ccxt.com/#/README?id=exchanges
+
+    Explainer Video
+    ---------------
+    https://youtu.be/yDNPhgO-450
+
+    Parameters
+    ----------
+    cls: self
+        passing all the information from the created class
+    exchange : str
+        'bybit' or 'binance' or whatever exchange works with ccxt
+    start : str
+        needs to be in this format '2022-01-01T00:00:00Z'
+    end : str
+        needs to be in this format '2022-01-01T00:00:00Z'
+    symbol : list or str
+        This will depend on the exchange for bybit it would be 'BTCUSDT' you will have to look this up on ccxt if you need to know.
+        You can send this as a list of symbols or just one symbol.
+        Here is an example of how to get the symbols list from bybit.
+        ```python
+        import ccxt
+        exh = ccxt.bybit()
+        exh.load_markets()
+        exh.symbols
+        ```
+    timeframe : str
+        '1m', '5m', '1h' '4h' '1d' '1w'
+    drop_volume: bool = True
+        Set this to False if you want to keep volume data.
+    remove_rate_limit: bool = False
+        This is the default rate limit the exchange asks for. If you remove it then its possible that if you are trying to get tons and tons of data from the exchange they could ban you or time you out.
+    bars_per_loop: int = 200
+        How many bars you want to grab at a time. Some exchanges let you grab more info per loop and some don't. I don't think grabbing more would make anything faster but you can try if the exchange allows for more. You would have to do your research and figure out how man bars but i know bybit says you can grab a max of 200 and apparently binance lets you grab up to 1000.
+
+    Returns
+    -------
+        Pandas dataframe of prices
+    """
+    if remove_rate_limit:
+        exchange = getattr(ccxt, exchange)()
+    else:
+        exchange = getattr(ccxt, exchange)({"enableRateLimit": True})
+    print("Loading exchange data")
+    exchange.load_markets()
+    # exchange.verbose = True  # uncomment for debugging purposes if necessary
+    start = exchange.parse8601(start)
+    end = exchange.parse8601(end)
+    timeframe = timeframe.lower()
+    if not isinstance(symbols, list):
+        symbols = [symbols]
+    if not all(isinstance(x, str) for x in symbols):
+        raise ValueError("your symbols must be strings")
+
+    symbols = sorted(symbols)
+    timeframe_int = int(sub(r"\D", "", timeframe))
+    timeframe_str = sub(r"\d", "", timeframe)
+    len_symbols = len(symbols)
+    if timeframe_str == "m":
+        time_in = 1000 * 60
+    elif timeframe_str == "h":
+        time_in = 1000 * 60 * 60
+    elif timeframe_str == "d":
+        time_in = 1000 * 60 * 60 * 24
+    elif timeframe_str == "w":
+        time_in = 1000 * 60 * 60 * 24 * 7
+    elif timeframe_str == "m":
+        time_in = 1000 * 60 * 60 * 24 * 7 * 12
+    else:
+        raise ValueError("something wrong with your timeframe")
+
+    x = start
+    timelist = [x]
+    while x < end:
+        x += time_in * timeframe_int
+        timelist.append(x)
+
+    final_df = pd.DataFrame(
+        columns=pd.MultiIndex.from_tuples(
+            tuples=[],
+            name=["symbol", "candle_info"],
+        ),
+        index=pd.Index(
+            data=pd.to_datetime(timelist, unit="ms"),
+            name="open_time",
+        ),
+    )
+    # Example if you selected your timeframe as 30 minute candles
+
+    # Get the distance between the end date and start date in miliseconds
+    # Divide that by the amount of miliseconds in what ever timeframe you set ex: there are 60,000 miliseconds in one minute.
+    # Then you divide that by the number for the timeframe you set like 30 for 30 minutes to get the amount of 30 min bars in that distance of time
+    # Then divide by limit because that is the amount of rows of data you can return
+    # Then add one because that is the amount of loops we will have to do
+    # then multiple by the amount of symbols so if we have to do 2 loops per symbol and we have 2 symbols we have to do a total of 4 loops
+    # Then last we do + len of symbols because we will do an extra pbar update after we create the dataframe
+    num_candles_per_coin = ((end - start) / time_in) / timeframe_int
+    total_tqdm = (
+        (int(num_candles_per_coin / bars_per_loop) + 1) * len_symbols
+    ) + len_symbols
+    print(
+        f"Total possible rows of data to be download: {int(num_candles_per_coin)}\n"
+        f"Total possible candles to be download: {int(num_candles_per_coin) * len_symbols}\n"
+        f"It could finish earlier than expected because maybe not all coins have data starting from the start date selected."
+    )
+    with tqdm(total=total_tqdm) as pbar:
+        # with tqdm(total=96*2) as pbar:
+        for symbol in symbols:
+            all_ohlcvs = []
+            temp_end = end
+            pbar.set_description(f"Downloading {symbol}")
+            while True:
+                try:
+                    ohlcvs = exchange.fetch_ohlcv(
+                        symbol=symbol,
+                        timeframe=timeframe,
+                        since=start,
+                        limit=bars_per_loop,
+                        params={"end": temp_end},
                     )
-                    if drop_volume:
-                        data.drop(columns=(symbol, "volume"), inplace=True, axis=1)
-                    final_df = final_df.join(data)
-                pbar.update(1)
-        final_df.sort_index(ascending=True, inplace=True)
-        final_df.sort_index(axis=1, level=0, sort_remaining=False)
-        final_df.dropna(how="all", inplace=True)
-        final_df.drop(final_df.tail(1).index, inplace=True)
-        return final_df
+                    all_ohlcvs += ohlcvs
+                    if len(ohlcvs):
+                        temp_end = ohlcvs[0][0] - 1
+                        pbar.update(1)
+                    else:
+                        break
+
+                except Exception as e:
+                    print(type(e).__name__, str(e))
+
+            if all_ohlcvs:
+                all_ohlcvs = np.array(all_ohlcvs)
+                data_columns = pd.MultiIndex.from_tuples(
+                    [
+                        (symbol, "open"),
+                        (symbol, "high"),
+                        (symbol, "low"),
+                        (symbol, "close"),
+                        (symbol, "volume"),
+                    ],
+                    name=["symbol", "candle_info"],
+                )
+                data_index = pd.Index(
+                    data=pd.to_datetime(all_ohlcvs[:, 0].flatten(), unit="ms"),
+                    name="open_time",
+                )
+                data = pd.DataFrame(
+                    all_ohlcvs[:, 1:],
+                    columns=data_columns,
+                    index=data_index,
+                )
+                if drop_volume:
+                    data.drop(columns=(symbol, "volume"), inplace=True, axis=1)
+                final_df = final_df.join(data)
+            pbar.update(1)
+    final_df.sort_index(ascending=True, inplace=True)
+    final_df.sort_index(axis=1, level=0, sort_remaining=False)
+    final_df.dropna(how="all", inplace=True)
+    final_df.drop(final_df.tail(1).index, inplace=True)
+    return final_df
```

### Comparing `quantfreedom-0.0.2/quantfreedom/enums/enums.py` & `quantfreedom-0.0.3/quantfreedom/enums/enums.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/evaluators/evaluators.py` & `quantfreedom-0.0.3/quantfreedom/evaluators/evaluators.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         columns=pd.MultiIndex.from_tuples(
             tuples=list(pd_multind_tuples),
             names=pd_col_names,
         ),
     )
 
 
-def eval_is_above(
+def is_above(
     want_to_evaluate: pdFrame,
     user_args: Union[list[int, float], int, float, Array1d] = None,
     indicator_data: pdFrame = None,
     prices: pdFrame = None,
     cand_ohlc: str = None,
     plot_results: bool = False,
 ) -> pdFrame:
@@ -564,15 +564,15 @@
         columns=pd.MultiIndex.from_tuples(
             tuples=list(pd_multind_tuples),
             names=pd_col_names,
         ),
     )
 
 
-def eval_is_below(
+def is_below(
     want_to_evaluate: pdFrame,
     user_args: Union[list[int, float], int, float, Array1d] = None,
     indicator_data: pdFrame = None,
     prices: pdFrame = None,
     cand_ohlc: str = None,
     plot_results: bool = False,
 ) -> pdFrame:
```

### Comparing `quantfreedom-0.0.2/quantfreedom/indicators/talib_ind.py` & `quantfreedom-0.0.3/quantfreedom/indicators/talib_ind.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,47 @@
 from talib import get_functions
 from itertools import product
 from quantfreedom._typing import pdFrame, Array1d
 
 
 def from_talib(
     func_name: str,
-    cart_product: bool,
-    combos: bool,
     prices: pdFrame = None,
     indicator_data: pdFrame = None,
+    cart_product: bool = False,
+    combos: bool = False,
     **kwargs,
 ) -> pdFrame:
-
+    """
+    Function Name
+    -------------
+    from_talib
+    
+    Summary
+    -------
+    _summary_
+    
+    Parameters
+    ----------
+    func_name : str
+        _description_
+    prices : pdFrame, None
+        _description_
+    indicator_data : pdFrame, None
+        _description_
+    cart_product : bool, False
+        _description_
+    combos : bool, False
+        _description_
+    
+    Returns
+    -------
+    pdFrame
+        _description_
+    """
     if all(x is None for x in (prices, indicator_data)):
         raise ValueError(
             f"You need to send either prices = pdFrame or indicator_data = pdFrame"
         )
     elif all(x is not None for x in (prices, indicator_data)):
         raise ValueError(
             f"You can't send both prices and values ... please pick one or the other"
```

### Comparing `quantfreedom-0.0.2/quantfreedom/nb/buy_funcs.py` & `quantfreedom-0.0.3/quantfreedom/nb/buy_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/nb/execute_funcs.py` & `quantfreedom-0.0.3/quantfreedom/nb/execute_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/nb/helper_funcs.py` & `quantfreedom-0.0.3/quantfreedom/nb/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/nb/sell_funcs.py` & `quantfreedom-0.0.3/quantfreedom/nb/sell_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/nb/simulate.py` & `quantfreedom-0.0.3/quantfreedom/nb/simulate.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/plotting/plot_helper_functions.py` & `quantfreedom-0.0.3/quantfreedom/plotting/plot_helper_functions.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/plotting/plotting_main.py` & `quantfreedom-0.0.3/quantfreedom/plotting/plotting_main.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/plotting/replay.py` & `quantfreedom-0.0.3/quantfreedom/plotting/replay.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom/utils/helpers.py` & `quantfreedom-0.0.3/quantfreedom/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/quantfreedom.egg-info/PKG-INFO` & `quantfreedom-0.0.3/quantfreedom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfreedom
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/QuantFreedom1022/quantfreedom
 Author: Quant Freedom
 Author-email: QuantFreedom1022@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quantfreedom-0.0.2/quantfreedom.egg-info/SOURCES.txt` & `quantfreedom-0.0.3/quantfreedom.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 quantfreedom.egg-info/SOURCES.txt
 quantfreedom.egg-info/dependency_links.txt
 quantfreedom.egg-info/requires.txt
 quantfreedom.egg-info/top_level.txt
 quantfreedom/base/__init__.py
 quantfreedom/base/base.py
 quantfreedom/data/__init__.py
-quantfreedom/data/ccxtdata.py
+quantfreedom/data/data_dl.py
 quantfreedom/enums/__init__.py
 quantfreedom/enums/enums.py
 quantfreedom/evaluators/__init__.py
 quantfreedom/evaluators/evaluators.py
 quantfreedom/indicators/__init__.py
 quantfreedom/indicators/talib_ind.py
 quantfreedom/nb/__init__.py
```

### Comparing `quantfreedom-0.0.2/quantfreedom.egg-info/requires.txt` & `quantfreedom-0.0.3/quantfreedom.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.0.2/setup.py` & `quantfreedom-0.0.3/setup.py`

 * *Files identical despite different names*

