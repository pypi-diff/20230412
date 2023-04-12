# Comparing `tmp/gym-trading-env-0.1.6.tar.gz` & `tmp/gym-trading-env-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.1.6.tar", last modified: Wed Apr 12 05:48:48 2023, max compression
+gzip compressed data, was "gym-trading-env-0.1.7.tar", last modified: Wed Apr 12 06:40:44 2023, max compression
```

## Comparing `gym-trading-env-0.1.6.tar` & `gym-trading-env-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.774973 gym-trading-env-0.1.6/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0    14011 2023-04-12 05:48:48.773975 gym-trading-env-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    12149 2023-04-11 09:31:03.000000 gym-trading-env-0.1.6/README.md
--rw-rw-rw-   0        0        0      870 2023-04-12 05:33:10.000000 gym-trading-env-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 05:48:48.774973 gym-trading-env-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.612408 gym-trading-env-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.665269 gym-trading-env-0.1.6/src/gym_trading_env/
--rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.6/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4029 2023-04-12 05:32:37.000000 gym-trading-env-0.1.6/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.6/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.6/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.770983 gym-trading-env-0.1.6/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.6/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:48:48.718124 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0    14011 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-12 05:48:48.000000 gym-trading-env-0.1.6/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.190187 gym-trading-env-0.1.7/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    14258 2023-04-12 06:40:44.188192 gym-trading-env-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    12396 2023-04-12 06:38:12.000000 gym-trading-env-0.1.7/README.md
+-rw-rw-rw-   0        0        0      870 2023-04-12 06:40:24.000000 gym-trading-env-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 06:40:44.190187 gym-trading-env-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.123367 gym-trading-env-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.139323 gym-trading-env-0.1.7/src/gym_trading_env/
+-rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.7/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4126 2023-04-12 06:37:36.000000 gym-trading-env-0.1.7/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.7/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.7/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.185201 gym-trading-env-0.1.7/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.175227 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0    14258 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.1.6/LICENSE.txt` & `gym-trading-env-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.6/PKG-INFO` & `gym-trading-env-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,37 +74,40 @@
 This environment supports more complex positions such as:
 - ```-1``` : Bet 100% of the portfolio value on the decline of asset Y (=SHORT). To perform this action, the environment borrows 100% of the portfolio valuation as stock Y to an imaginary person, and immediately sells it. When the agent closes this position, the environment buys the owed amount of stock Y and repays the imaginary person with it. If the price has fallen during the operation, we buy cheaper than we sold what we need to repay : the difference is our gain. The imaginary person is paid a small rent (parameter : ```borrow_interest_rate```)
 - ```+2``` : Bet 100% of the portfolio value of the rise of asset Y. We use the same mechanism explained above, but we borrow currency and buy stock Y.
 - ```-10``` ? : We can BUT ...  We need to borrow 1000% of the portfolio valuation as asset Y. You need to understand that such a "leverage" is very risky. As if the stock price rise by 10%, you need to repay the original 1000% of your portfolio valuation at 1100% (1000%*1.10) of your current portfolio valuation. Well, 100% (1100% - 1000%) of your portfolio is used to repay your debt. **GAME OVER, you have 0$ left**. The leverage is very useful but also risky, as it increases your **gains** AND your **losses**. Always keep in mind that you can lose everything.
 
 ### How to use ?
 
-**1 - Import and clean your data**. They need to be ordered by ascending date. Index must be a date. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
+**1 - Import and clean your data**. They need to be ordered by ascending date. Index must be DatetimeIndex. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
 ```python
 # Available in the github repo : test/data/BTC_USD-Hourly.csv
 df = pd.read_csv("data/BTC_USD-Hourly.csv", parse_dates=["date"], index_col= "date")
 df.sort_index(inplace= True)
 df.dropna(inplace= True)
 df.drop_duplicates(inplace=True)
 ```
-**1.1 (Optional) Download data** : The package provide a easy way to download data (works with CCTX ans use asyncio to get FAST) :
+**1.1 (Optional) Download data** : The package provides an easy way to download data (works with CCTX and uses asyncio for FAST download) :
+
+Indeed, data is KING. To train RL Agent, you will need a big amount of good quality data. 
 ```python
 from gym_trading_env.downloader import download
 import datetime
 
 download(
     exchange_names = ["binance", "bitfinex2", "huobi"],
     symbols= ["BTC/USDT", "ETH/USDT"],
     timeframe= "30m",
     dir = "test/data",
     since= datetime.datetime(year= 2019, month= 1, day=1),
     until = datetime.datetime(year= 2023, month= 1, day=1),
 )
+# It will download and save in folder 'test/data' both 'BTC/USDT' and 'ETH/USDT' historical data from all the exchanges mentionned.
 ```
-This function use pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```.
+This function uses pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```. 
 
 
 **2 - Create your features**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
 **The feature column names need to contain the keyword 'feature'. The environment will automatically detect them !**
 
 ```python
 df["feature_close"] = df["close"].pct_change()
@@ -127,15 +130,15 @@
 
 
 Accessible columns of history object :
 >- ```step``` : Step = t.
 >- ```date``` : Date at step t, datetime.
 >- ```reward``` : Reward at step t.
 >- ```position_index``` : Index of the position at step t amoung your position argument.
-v- ```position``` : Portfolio position at step t.
+>- ```position``` : Portfolio position at step t.
 >- ```portfolio_valuation```: Global valuation of the portfolio.
 >- It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :```data_close```, ```data_open```,  ```data_high```....
 >- It stores the distribution of the portfolio : ```portfolio_distribution_asset``` the amount of owned asset (stock), ```portfolio_distribution_fiat``` the amount of owned fiat currency, ```portfolio_distribution_borrowed_asset``` amount of borrowed asset, ```portfolio_distribution_borrowed_fiat``` the amount of borrowed fiat currency, ```portfolio_distribution_interest_asset``` the total of cumalated interest generated by the borrowed asset, ```portfolio_distribution_interest_fiat``` the total of cumalated interest generated by the borrowed fiat currency.
 
 
 **4 - Initiate the environment**
 
@@ -190,15 +193,15 @@
 
 ```python
 ...
 # At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
 ```
 
-Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
+Then in the separated render script. You can import and initiate a renderer object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
 renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
 #### Custom render
```

### Comparing `gym-trading-env-0.1.6/README.md` & `gym-trading-env-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,37 +39,40 @@
 This environment supports more complex positions such as:
 - ```-1``` : Bet 100% of the portfolio value on the decline of asset Y (=SHORT). To perform this action, the environment borrows 100% of the portfolio valuation as stock Y to an imaginary person, and immediately sells it. When the agent closes this position, the environment buys the owed amount of stock Y and repays the imaginary person with it. If the price has fallen during the operation, we buy cheaper than we sold what we need to repay : the difference is our gain. The imaginary person is paid a small rent (parameter : ```borrow_interest_rate```)
 - ```+2``` : Bet 100% of the portfolio value of the rise of asset Y. We use the same mechanism explained above, but we borrow currency and buy stock Y.
 - ```-10``` ? : We can BUT ...  We need to borrow 1000% of the portfolio valuation as asset Y. You need to understand that such a "leverage" is very risky. As if the stock price rise by 10%, you need to repay the original 1000% of your portfolio valuation at 1100% (1000%*1.10) of your current portfolio valuation. Well, 100% (1100% - 1000%) of your portfolio is used to repay your debt. **GAME OVER, you have 0$ left**. The leverage is very useful but also risky, as it increases your **gains** AND your **losses**. Always keep in mind that you can lose everything.
 
 ### How to use ?
 
-**1 - Import and clean your data**. They need to be ordered by ascending date. Index must be a date. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
+**1 - Import and clean your data**. They need to be ordered by ascending date. Index must be DatetimeIndex. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
 ```python
 # Available in the github repo : test/data/BTC_USD-Hourly.csv
 df = pd.read_csv("data/BTC_USD-Hourly.csv", parse_dates=["date"], index_col= "date")
 df.sort_index(inplace= True)
 df.dropna(inplace= True)
 df.drop_duplicates(inplace=True)
 ```
-**1.1 (Optional) Download data** : The package provide a easy way to download data (works with CCTX ans use asyncio to get FAST) :
+**1.1 (Optional) Download data** : The package provides an easy way to download data (works with CCTX and uses asyncio for FAST download) :
+
+Indeed, data is KING. To train RL Agent, you will need a big amount of good quality data. 
 ```python
 from gym_trading_env.downloader import download
 import datetime
 
 download(
     exchange_names = ["binance", "bitfinex2", "huobi"],
     symbols= ["BTC/USDT", "ETH/USDT"],
     timeframe= "30m",
     dir = "test/data",
     since= datetime.datetime(year= 2019, month= 1, day=1),
     until = datetime.datetime(year= 2023, month= 1, day=1),
 )
+# It will download and save in folder 'test/data' both 'BTC/USDT' and 'ETH/USDT' historical data from all the exchanges mentionned.
 ```
-This function use pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```.
+This function uses pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```. 
 
 
 **2 - Create your features**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
 **The feature column names need to contain the keyword 'feature'. The environment will automatically detect them !**
 
 ```python
 df["feature_close"] = df["close"].pct_change()
@@ -92,15 +95,15 @@
 
 
 Accessible columns of history object :
 >- ```step``` : Step = t.
 >- ```date``` : Date at step t, datetime.
 >- ```reward``` : Reward at step t.
 >- ```position_index``` : Index of the position at step t amoung your position argument.
-v- ```position``` : Portfolio position at step t.
+>- ```position``` : Portfolio position at step t.
 >- ```portfolio_valuation```: Global valuation of the portfolio.
 >- It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :```data_close```, ```data_open```,  ```data_high```....
 >- It stores the distribution of the portfolio : ```portfolio_distribution_asset``` the amount of owned asset (stock), ```portfolio_distribution_fiat``` the amount of owned fiat currency, ```portfolio_distribution_borrowed_asset``` amount of borrowed asset, ```portfolio_distribution_borrowed_fiat``` the amount of borrowed fiat currency, ```portfolio_distribution_interest_asset``` the total of cumalated interest generated by the borrowed asset, ```portfolio_distribution_interest_fiat``` the total of cumalated interest generated by the borrowed fiat currency.
 
 
 **4 - Initiate the environment**
 
@@ -155,15 +158,15 @@
 
 ```python
 ...
 # At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
 ```
 
-Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
+Then in the separated render script. You can import and initiate a renderer object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
 renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
 #### Custom render
```

### Comparing `gym-trading-env-0.1.6/pyproject.toml` & `gym-trading-env-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.1.6"
+version = "0.1.7"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env/downloader.py` & `gym-trading-env-0.1.7/src/gym_trading_env/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,17 @@
         "pause_every": 10,
         "pause" : 1, #seconds
     }
 }
 
 async def _ohlcv(exchange, symbol, timeframe, limit, step_since, timedelta):
     result = await exchange.fetch_ohlcv(symbol = symbol, timeframe= timeframe, limit= limit, since=step_since)
-    result_df = pd.DataFrame(result, columns=["timestamp_open", "open", "high", "low", "close", "volume"], dtype= np.float32)
+    result_df = pd.DataFrame(result, columns=["timestamp_open", "open", "high", "low", "close", "volume"])
+    for col in ["open", "high", "low", "close", "volume"]:
+        result_df[col] = pd.to_numeric(result_df[col])
     result_df["date_open"] = pd.to_datetime(result_df["timestamp_open"], unit= "ms")
     result_df["date_close"] = pd.to_datetime(result_df["timestamp_open"] + timedelta, unit= "ms")
     return result_df
 
 async def _download_symbol(exchange, symbol, timeframe = '5m', since = int(datetime.datetime(year=2020, month= 1, day= 1).timestamp()*1E3), until = int(datetime.datetime.now().timestamp()*1E3), limit = 1000, pause_every = 10, pause = 1):
     timedelta = int(pd.Timedelta(timeframe).to_timedelta64()/1E6)
     tasks = []
```

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env/environments.py` & `gym-trading-env-0.1.7/src/gym_trading_env/environments.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env/renderer.py` & `gym-trading-env-0.1.7/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.1.7/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.1.7/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.1.7/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.1.7/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,37 +74,40 @@
 This environment supports more complex positions such as:
 - ```-1``` : Bet 100% of the portfolio value on the decline of asset Y (=SHORT). To perform this action, the environment borrows 100% of the portfolio valuation as stock Y to an imaginary person, and immediately sells it. When the agent closes this position, the environment buys the owed amount of stock Y and repays the imaginary person with it. If the price has fallen during the operation, we buy cheaper than we sold what we need to repay : the difference is our gain. The imaginary person is paid a small rent (parameter : ```borrow_interest_rate```)
 - ```+2``` : Bet 100% of the portfolio value of the rise of asset Y. We use the same mechanism explained above, but we borrow currency and buy stock Y.
 - ```-10``` ? : We can BUT ...  We need to borrow 1000% of the portfolio valuation as asset Y. You need to understand that such a "leverage" is very risky. As if the stock price rise by 10%, you need to repay the original 1000% of your portfolio valuation at 1100% (1000%*1.10) of your current portfolio valuation. Well, 100% (1100% - 1000%) of your portfolio is used to repay your debt. **GAME OVER, you have 0$ left**. The leverage is very useful but also risky, as it increases your **gains** AND your **losses**. Always keep in mind that you can lose everything.
 
 ### How to use ?
 
-**1 - Import and clean your data**. They need to be ordered by ascending date. Index must be a date. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
+**1 - Import and clean your data**. They need to be ordered by ascending date. Index must be DatetimeIndex. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
 ```python
 # Available in the github repo : test/data/BTC_USD-Hourly.csv
 df = pd.read_csv("data/BTC_USD-Hourly.csv", parse_dates=["date"], index_col= "date")
 df.sort_index(inplace= True)
 df.dropna(inplace= True)
 df.drop_duplicates(inplace=True)
 ```
-**1.1 (Optional) Download data** : The package provide a easy way to download data (works with CCTX ans use asyncio to get FAST) :
+**1.1 (Optional) Download data** : The package provides an easy way to download data (works with CCTX and uses asyncio for FAST download) :
+
+Indeed, data is KING. To train RL Agent, you will need a big amount of good quality data. 
 ```python
 from gym_trading_env.downloader import download
 import datetime
 
 download(
     exchange_names = ["binance", "bitfinex2", "huobi"],
     symbols= ["BTC/USDT", "ETH/USDT"],
     timeframe= "30m",
     dir = "test/data",
     since= datetime.datetime(year= 2019, month= 1, day=1),
     until = datetime.datetime(year= 2023, month= 1, day=1),
 )
+# It will download and save in folder 'test/data' both 'BTC/USDT' and 'ETH/USDT' historical data from all the exchanges mentionned.
 ```
-This function use pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```.
+This function uses pickle format to save the OHLCV data. You will need to import the dataset with ```pd.read_pickle('... .pkl', ...)```. The function supports exchange_names ```binance```, ```biftfinex2``` (API v2) and ```huobi```. 
 
 
 **2 - Create your features**. Your RL-agent will need some good, preprocessed features. It is your job to make sure it has everything it needs.
 **The feature column names need to contain the keyword 'feature'. The environment will automatically detect them !**
 
 ```python
 df["feature_close"] = df["close"].pct_change()
@@ -127,15 +130,15 @@
 
 
 Accessible columns of history object :
 >- ```step``` : Step = t.
 >- ```date``` : Date at step t, datetime.
 >- ```reward``` : Reward at step t.
 >- ```position_index``` : Index of the position at step t amoung your position argument.
-v- ```position``` : Portfolio position at step t.
+>- ```position``` : Portfolio position at step t.
 >- ```portfolio_valuation```: Global valuation of the portfolio.
 >- It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :```data_close```, ```data_open```,  ```data_high```....
 >- It stores the distribution of the portfolio : ```portfolio_distribution_asset``` the amount of owned asset (stock), ```portfolio_distribution_fiat``` the amount of owned fiat currency, ```portfolio_distribution_borrowed_asset``` amount of borrowed asset, ```portfolio_distribution_borrowed_fiat``` the amount of borrowed fiat currency, ```portfolio_distribution_interest_asset``` the total of cumalated interest generated by the borrowed asset, ```portfolio_distribution_interest_fiat``` the total of cumalated interest generated by the borrowed fiat currency.
 
 
 **4 - Initiate the environment**
 
@@ -190,15 +193,15 @@
 
 ```python
 ...
 # At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
 ```
 
-Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
+Then in the separated render script. You can import and initiate a renderer object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
 renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
 #### Custom render
```

### Comparing `gym-trading-env-0.1.6/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.1.7/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

