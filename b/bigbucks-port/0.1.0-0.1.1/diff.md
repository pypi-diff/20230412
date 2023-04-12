# Comparing `tmp/bigbucks_port-0.1.0.tar.gz` & `tmp/bigbucks_port-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigbucks_port-0.1.0.tar", last modified: Tue Apr 11 05:30:58 2023, max compression
+gzip compressed data, was "bigbucks_port-0.1.1.tar", last modified: Wed Apr 12 02:18:46 2023, max compression
```

## Comparing `bigbucks_port-0.1.0.tar` & `bigbucks_port-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 05:30:58.591722 bigbucks_port-0.1.0/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     1065 2023-04-03 00:48:13.000000 bigbucks_port-0.1.0/LICENSE
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 05:30:58.591560 bigbucks_port-0.1.0/PKG-INFO
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3264 2023-04-06 03:40:05.000000 bigbucks_port-0.1.0/README.md
--rw-r--r--   0 cuiwenjie   (501) staff       (20)       38 2023-04-11 05:30:58.591764 bigbucks_port-0.1.0/setup.cfg
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      346 2023-04-11 05:29:39.000000 bigbucks_port-0.1.0/setup.py
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 05:30:58.589428 bigbucks_port-0.1.0/src/
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 05:30:58.590459 bigbucks_port-0.1.0/src/bigbucks_port/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)        0 2023-04-02 23:17:45.000000 bigbucks_port-0.1.0/src/bigbucks_port/__init__.py
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     8999 2023-04-11 05:11:22.000000 bigbucks_port-0.1.0/src/bigbucks_port/portfolio.py
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 05:30:58.591162 bigbucks_port-0.1.0/src/bigbucks_port.egg-info/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 05:30:58.000000 bigbucks_port-0.1.0/src/bigbucks_port.egg-info/PKG-INFO
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      275 2023-04-11 05:30:58.000000 bigbucks_port-0.1.0/src/bigbucks_port.egg-info/SOURCES.txt
--rw-r--r--   0 cuiwenjie   (501) staff       (20)        1 2023-04-11 05:30:58.000000 bigbucks_port-0.1.0/src/bigbucks_port.egg-info/dependency_links.txt
--rw-r--r--   0 cuiwenjie   (501) staff       (20)       14 2023-04-11 05:30:58.000000 bigbucks_port-0.1.0/src/bigbucks_port.egg-info/top_level.txt
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 05:30:58.591363 bigbucks_port-0.1.0/tests/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      783 2023-04-11 05:18:27.000000 bigbucks_port-0.1.0/tests/test_portfolio.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-12 02:18:46.745536 bigbucks_port-0.1.1/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     1065 2023-04-03 00:48:13.000000 bigbucks_port-0.1.1/LICENSE
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-12 02:18:46.745346 bigbucks_port-0.1.1/PKG-INFO
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3264 2023-04-06 03:40:05.000000 bigbucks_port-0.1.1/README.md
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)       38 2023-04-12 02:18:46.745582 bigbucks_port-0.1.1/setup.cfg
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      346 2023-04-12 02:18:37.000000 bigbucks_port-0.1.1/setup.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-12 02:18:46.741805 bigbucks_port-0.1.1/src/
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-12 02:18:46.742901 bigbucks_port-0.1.1/src/bigbucks_port/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)        0 2023-04-02 23:17:45.000000 bigbucks_port-0.1.1/src/bigbucks_port/__init__.py
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     9167 2023-04-12 02:12:18.000000 bigbucks_port-0.1.1/src/bigbucks_port/portfolio.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-12 02:18:46.744519 bigbucks_port-0.1.1/src/bigbucks_port.egg-info/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-12 02:18:46.000000 bigbucks_port-0.1.1/src/bigbucks_port.egg-info/PKG-INFO
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      275 2023-04-12 02:18:46.000000 bigbucks_port-0.1.1/src/bigbucks_port.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)        1 2023-04-12 02:18:46.000000 bigbucks_port-0.1.1/src/bigbucks_port.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)       14 2023-04-12 02:18:46.000000 bigbucks_port-0.1.1/src/bigbucks_port.egg-info/top_level.txt
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-12 02:18:46.745012 bigbucks_port-0.1.1/tests/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      615 2023-04-12 02:15:29.000000 bigbucks_port-0.1.1/tests/test_portfolio.py
```

### Comparing `bigbucks_port-0.1.0/LICENSE` & `bigbucks_port-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bigbucks_port-0.1.0/PKG-INFO` & `bigbucks_port-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbucks_port
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package used for portfolio analysis in Fintech512
 Author: Wenjie Cui
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
```

### Comparing `bigbucks_port-0.1.0/README.md` & `bigbucks_port-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bigbucks_port-0.1.0/src/bigbucks_port/portfolio.py` & `bigbucks_port-0.1.1/src/bigbucks_port/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,29 +52,33 @@
 # Calculate the daily returns for the stocks in the portfolio
 def cal_returns(objs,id):
     # Get the symbols in the holding
     holdings = current_holding(objs,id)
     symbols = holdings.index.to_numpy()
     if len(symbols) ==0:
         raise Exception("This user has no holding")
-    stockreturns = pd.DataFrame(columns=symbols)
+    # stockreturns = pd.DataFrame(columns=symbols)
+    stockreturns = []
     # Get the daily prices for the given symbol
     for s in symbols:
         data = objs.view_symbol_price_data(s)
         if len(data) == 0:
             raise Exception("This symbol has no historical price data")
         stockprice = pd.json_normalize(data)
         # Sort prices by date
         stockprice.sort_values(by='date',inplace=True)
         # calculate the daily returns
-        returns = np.log(stockprice['adjusted_close']/stockprice['adjusted_close'].shift(1))
-        stockreturns[s]=returns.to_numpy()
-    stockreturns.index = stockprice['date']
-    stockreturns.dropna(inplace=True)
-    return stockreturns
+        returns = pd.DataFrame(np.log(stockprice['adjusted_close']/stockprice['adjusted_close'].shift(1)))
+        returns.columns = [s]
+        returns.index = stockprice['date']
+        # stockreturns[s]=returns.to_numpy()
+        stockreturns.append(returns)
+    returns = pd.concat(stockreturns,axis=1)
+    returns.dropna(inplace=True)
+    return returns
 
 # Calculate the daily returns for SPY
 def spy_returns(objs):
     spy_price = pd.json_normalize(objs.view_table_data("SP500_Index"))
     spy_price['return'] = np.log(spy_price['close']/spy_price['close'].shift(1))
     spy_price.dropna(inplace=True)
     return spy_price[['date','return']]
@@ -184,16 +188,16 @@
 # risk and return for efficient frontier json format
 def frontier_json(objs,id,num):
     returns,risk = frontier(objs,id,num)
     # A list of json objects 
     js_list =[]
     labels_list = []
     for i in range(len(returns)):
-        dict_obj = {'std': risk[i], 'mean': returns[i]}
-        labels_list.append(risk[i])
+        dict_obj = {'std': round(risk[i],3), 'mean': round(returns[i],3)}
+        labels_list.append(round(risk[i],3))
         js_list.append(dict_obj)
     return json.dumps({"data":js_list,"labels":labels_list})
 
 # optimal portfolio with max sharpe
 def optimize_port(rf,objs,id):
     er = er_covar(objs,id)[0].to_numpy()
     covar = er_covar(objs,id)[2].to_numpy()
```

### Comparing `bigbucks_port-0.1.0/src/bigbucks_port.egg-info/PKG-INFO` & `bigbucks_port-0.1.1/src/bigbucks_port.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbucks-port
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package used for portfolio analysis in Fintech512
 Author: Wenjie Cui
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
```

