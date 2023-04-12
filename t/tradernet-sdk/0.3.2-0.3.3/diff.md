# Comparing `tmp/tradernet_sdk-0.3.2.tar.gz` & `tmp/tradernet_sdk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradernet_sdk-0.3.2.tar", max compression
+gzip compressed data, was "tradernet_sdk-0.3.3.tar", max compression
```

## Comparing `tradernet_sdk-0.3.2.tar` & `tradernet_sdk-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1131 2023-03-13 19:06:10.633456 tradernet_sdk-0.3.2/LICENSE
--rw-r--r--   0        0        0     4024 2023-03-13 19:06:10.633456 tradernet_sdk-0.3.2/README.md
--rw-r--r--   0        0        0      975 2023-03-14 18:52:55.304097 tradernet_sdk-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/PublicApiClient.py
--rw-r--r--   0        0        0      583 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/__init__.py
--rw-r--r--   0        0        0    32929 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/client.py
--rw-r--r--   0        0        0    11656 2023-03-13 19:12:40.869617 tradernet_sdk-0.3.2/tradernet/core.py
--rw-r--r--   0        0        0     2231 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/netutils.py
--rw-r--r--   0        0        0     7877 2023-03-13 19:12:40.869617 tradernet_sdk-0.3.2/tradernet/string_utils.py
--rw-r--r--   0        0        0        0 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/symbols/__init__.py
--rw-r--r--   0        0        0     6329 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/symbols/base_market_symbol.py
--rw-r--r--   0        0        0     4151 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/symbols/base_option_symbol.py
--rw-r--r--   0        0        0     2836 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/symbols/das_option.py
--rw-r--r--   0        0        0      290 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/symbols/option_properties.py
--rw-r--r--   0        0        0     2132 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/symbols/tradernet_option.py
--rw-r--r--   0        0        0     2336 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/symbols/tradernet_symbol.py
--rw-r--r--   0        0        0     3052 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/tradernet_wsapi.py
--rw-r--r--   0        0        0     6414 2023-03-14 18:52:55.304097 tradernet_sdk-0.3.2/tradernet/trading.py
--rw-r--r--   0        0        0     2858 2023-03-13 19:06:10.637456 tradernet_sdk-0.3.2/tradernet/ws_utils.py
--rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4024 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/README.md
+-rw-r--r--   0        0        0      978 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1305 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/PublicApiClient.py
+-rw-r--r--   0        0        0      583 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/__init__.py
+-rw-r--r--   0        0        0    32929 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/client.py
+-rw-r--r--   0        0        0    11656 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/core.py
+-rw-r--r--   0        0        0     2231 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/netutils.py
+-rw-r--r--   0        0        0     7877 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/string_utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:01:58.087196 tradernet_sdk-0.3.3/tradernet/symbols/__init__.py
+-rw-r--r--   0        0        0     6329 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/base_market_symbol.py
+-rw-r--r--   0        0        0     4151 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/base_option_symbol.py
+-rw-r--r--   0        0        0     2836 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/das_option.py
+-rw-r--r--   0        0        0      290 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/option_properties.py
+-rw-r--r--   0        0        0     2132 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/tradernet_option.py
+-rw-r--r--   0        0        0     2336 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/tradernet_symbol.py
+-rw-r--r--   0        0        0     3052 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/tradernet_wsapi.py
+-rw-r--r--   0        0        0     6414 2023-04-12 18:30:40.754961 tradernet_sdk-0.3.3/tradernet/trading.py
+-rw-r--r--   0        0        0     2858 2023-04-12 18:30:40.754961 tradernet_sdk-0.3.3/tradernet/ws_utils.py
+-rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.3/PKG-INFO
```

### Comparing `tradernet_sdk-0.3.2/LICENSE` & `tradernet_sdk-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/README.md` & `tradernet_sdk-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/pyproject.toml` & `tradernet_sdk-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "tradernet-sdk"
-version = "0.3.2"
+version = "0.3.3"
 description = "Public API for TraderNet"
 authors = ["Anton Kudelin <a.kudelin@freedomfinance.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://tradernet.com/tradernet-api/"
 packages = [
     {include = "tradernet"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 lxml = "^4.9.2"
-pandas = "^1.5.3"
+pandas = "^2.0.0"
 requests = "^2.28.2"
-aiohttp = "^3.8.3"
+aiohttp = "^3.8.4"
 mypy-extensions = "^1.0.0"
 certifi = "^2022.12.7"
 tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.1.1"
-pylint = "^2.15.10"
-types-requests = "^2.28.7"
+mypy = "^1.2.0"
+pylint = "^2.17.2"
+types-requests = "^2.28.11.17"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 strict = true
```

### Comparing `tradernet_sdk-0.3.2/tradernet/PublicApiClient.py` & `tradernet_sdk-0.3.3/tradernet/PublicApiClient.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/__init__.py` & `tradernet_sdk-0.3.3/tradernet/__init__.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/client.py` & `tradernet_sdk-0.3.3/tradernet/client.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/core.py` & `tradernet_sdk-0.3.3/tradernet/core.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/netutils.py` & `tradernet_sdk-0.3.3/tradernet/netutils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/string_utils.py` & `tradernet_sdk-0.3.3/tradernet/string_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/symbols/base_market_symbol.py` & `tradernet_sdk-0.3.3/tradernet/symbols/base_market_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/symbols/base_option_symbol.py` & `tradernet_sdk-0.3.3/tradernet/symbols/base_option_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/symbols/das_option.py` & `tradernet_sdk-0.3.3/tradernet/symbols/das_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/symbols/tradernet_option.py` & `tradernet_sdk-0.3.3/tradernet/symbols/tradernet_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/symbols/tradernet_symbol.py` & `tradernet_sdk-0.3.3/tradernet/symbols/tradernet_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/tradernet_wsapi.py` & `tradernet_sdk-0.3.3/tradernet/tradernet_wsapi.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/trading.py` & `tradernet_sdk-0.3.3/tradernet/trading.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/tradernet/ws_utils.py` & `tradernet_sdk-0.3.3/tradernet/ws_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.2/PKG-INFO` & `tradernet_sdk-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: tradernet-sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Public API for TraderNet
 Home-page: https://tradernet.com/tradernet-api/
 License: MIT
 Author: Anton Kudelin
 Author-email: a.kudelin@freedomfinance.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: mypy-extensions (>=1.0.0,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # tradernet-sdk
 
 Public Python API for TraderNet
```

