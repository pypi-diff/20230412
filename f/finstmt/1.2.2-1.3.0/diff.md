# Comparing `tmp/finstmt-1.2.2.tar.gz` & `tmp/finstmt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finstmt-1.2.2.tar", max compression
+gzip compressed data, was "finstmt-1.3.0.tar", max compression
```

## Comparing `finstmt-1.2.2.tar` & `finstmt-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
--rw-r--r--   0        0        0     1082 2023-02-22 11:52:15.345106 finstmt-1.2.2/LICENSE.md
--rw-r--r--   0        0        0     2107 2023-02-22 11:52:15.345106 finstmt-1.2.2/README.md
--rw-r--r--   0        0        0     1532 2023-02-22 11:52:15.345106 finstmt-1.2.2/conf.py
--rw-r--r--   0        0        0      386 2023-02-22 11:52:51.509596 finstmt-1.2.2/finstmt/__init__.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/bs/__init__.py
--rw-r--r--   0        0        0    38293 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/bs/config.py
--rw-r--r--   0        0        0     1840 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/bs/data.py
--rw-r--r--   0        0        0      672 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/bs/main.py
--rw-r--r--   0        0        0      197 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/check.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/clean/__init__.py
--rw-r--r--   0        0        0      946 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/clean/name.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/combined/__init__.py
--rw-r--r--   0        0        0     5947 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/combined/combinator.py
--rw-r--r--   0        0        0    12737 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/combined/statements.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/config_manage/__init__.py
--rw-r--r--   0        0        0     8245 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/config_manage/base.py
--rw-r--r--   0        0        0     2189 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/config_manage/data.py
--rw-r--r--   0        0        0      872 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/config_manage/global_.py
--rw-r--r--   0        0        0     2935 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/config_manage/statement.py
--rw-r--r--   0        0        0     4483 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/config_manage/statements.py
--rw-r--r--   0        0        0      926 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/exc.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/findata/__init__.py
--rw-r--r--   0        0        0     5867 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/findata/database.py
--rw-r--r--   0        0        0    12405 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/findata/statementsbase.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/__init__.py
--rw-r--r--   0        0        0     4896 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/config.py
--rw-r--r--   0        0        0      304 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/dataframe.py
--rw-r--r--   0        0        0     6764 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/main.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/__init__.py
--rw-r--r--   0        0        0     1028 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/average.py
--rw-r--r--   0        0        0     3486 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/base.py
--rw-r--r--   0        0        0     3392 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/cagr.py
--rw-r--r--   0        0        0     1316 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/chooser.py
--rw-r--r--   0        0        0     2469 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/manual.py
--rw-r--r--   0        0        0     3007 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/prophet.py
--rw-r--r--   0        0        0      803 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/recent.py
--rw-r--r--   0        0        0     1651 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/models/trend.py
--rw-r--r--   0        0        0     1529 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/plot.py
--rw-r--r--   0        0        0     4339 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/forecast/statements.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/inc/__init__.py
--rw-r--r--   0        0        0    11984 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/inc/config.py
--rw-r--r--   0        0        0     1363 2023-02-22 11:52:15.345106 finstmt-1.2.2/finstmt/inc/data.py
--rw-r--r--   0        0        0      702 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/inc/main.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/items/__init__.py
--rw-r--r--   0        0        0     2345 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/items/config.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/loaders/__init__.py
--rw-r--r--   0        0        0     1378 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/loaders/capiq.py
--rw-r--r--   0        0        0      278 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/logger.py
--rw-r--r--   0        0        0        0 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/resolver/__init__.py
--rw-r--r--   0        0        0     1140 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/resolver/base.py
--rw-r--r--   0        0        0    25053 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/resolver/forecast.py
--rw-r--r--   0        0        0     3238 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/resolver/history.py
--rw-r--r--   0        0        0     5900 2023-02-22 11:52:15.349106 finstmt-1.2.2/finstmt/resolver/solve.py
--rw-r--r--   0        0        0     1703 2023-02-22 11:52:51.401595 finstmt-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      474 2023-02-22 11:52:15.417107 finstmt-1.2.2/version.py
--rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 finstmt-1.2.2/setup.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 finstmt-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-12 00:08:44.972746 finstmt-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2107 2023-04-12 00:08:44.972746 finstmt-1.3.0/README.md
+-rw-r--r--   0        0        0     1532 2023-04-12 00:08:44.976745 finstmt-1.3.0/conf.py
+-rw-r--r--   0        0        0      386 2023-04-12 00:09:23.265073 finstmt-1.3.0/finstmt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/bs/__init__.py
+-rw-r--r--   0        0        0    38597 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/bs/config.py
+-rw-r--r--   0        0        0      742 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/bs/main.py
+-rw-r--r--   0        0        0      197 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/check.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/clean/__init__.py
+-rw-r--r--   0        0        0      946 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/clean/name.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/combined/__init__.py
+-rw-r--r--   0        0        0     5947 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/combined/combinator.py
+-rw-r--r--   0        0        0    12737 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/combined/statements.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/__init__.py
+-rw-r--r--   0        0        0     8245 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/base.py
+-rw-r--r--   0        0        0     2189 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/data.py
+-rw-r--r--   0        0        0      872 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/global_.py
+-rw-r--r--   0        0        0     2935 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/statement.py
+-rw-r--r--   0        0        0     4483 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/statements.py
+-rw-r--r--   0        0        0      926 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/exc.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/__init__.py
+-rw-r--r--   0        0        0     6233 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/period_data.py
+-rw-r--r--   0        0        0     1505 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/statement_item.py
+-rw-r--r--   0        0        0    11904 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/statementsbase.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/__init__.py
+-rw-r--r--   0        0        0     4896 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/config.py
+-rw-r--r--   0        0        0      304 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/dataframe.py
+-rw-r--r--   0        0        0     6764 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/main.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/__init__.py
+-rw-r--r--   0        0        0     1028 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/average.py
+-rw-r--r--   0        0        0     3486 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/base.py
+-rw-r--r--   0        0        0     3392 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/cagr.py
+-rw-r--r--   0        0        0     1316 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/chooser.py
+-rw-r--r--   0        0        0     2469 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/manual.py
+-rw-r--r--   0        0        0     3007 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/prophet.py
+-rw-r--r--   0        0        0      803 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/recent.py
+-rw-r--r--   0        0        0     1651 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/trend.py
+-rw-r--r--   0        0        0     1529 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/plot.py
+-rw-r--r--   0        0        0     4339 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/statements.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/inc/__init__.py
+-rw-r--r--   0        0        0    12013 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/inc/config.py
+-rw-r--r--   0        0        0      769 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/inc/main.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/items/__init__.py
+-rw-r--r--   0        0        0     2614 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/items/config.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/loaders/__init__.py
+-rw-r--r--   0        0        0     1378 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/loaders/capiq.py
+-rw-r--r--   0        0        0      278 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/logger.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/__init__.py
+-rw-r--r--   0        0        0     1140 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/base.py
+-rw-r--r--   0        0        0    25053 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/forecast.py
+-rw-r--r--   0        0        0     3238 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/history.py
+-rw-r--r--   0        0        0     5900 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/solve.py
+-rw-r--r--   0        0        0     1794 2023-04-12 00:09:23.161073 finstmt-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-12 00:08:45.036746 finstmt-1.3.0/version.py
+-rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 finstmt-1.3.0/setup.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 finstmt-1.3.0/PKG-INFO
```

### Comparing `finstmt-1.2.2/LICENSE.md` & `finstmt-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/README.md` & `finstmt-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/conf.py` & `finstmt-1.3.0/conf.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/bs/config.py` & `finstmt-1.3.0/finstmt/bs/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,60 +33,38 @@
             "st investments",
             "shortterm invest",
             "short term invest",
             "st invest",
         ],
     ),
     ItemConfig(
-        "cash_and_st_invest",
-        "Cash and Short-Term Investments",
-        extract_names=[
-            "total cash st investments",
-            "total cash and st investments",
-            "total cash and shortterm investments",
-            "total cash and short term investments",
-            "total cash shortterm investments",
-            "total cash short term investments",
-            "total cash st invest",
-            "total cash and st invest",
-            "total cash and shortterm invest",
-            "total cash and short term invest",
-            "total cash shortterm invest",
-            "total cash short term invest",
-            "cash st investments",
-            "cash and st investments",
-            "cash and shortterm investments",
-            "cash and short term investments",
-            "cash shortterm investments",
-            "cash short term investments",
-            "cash st invest",
-            "cash and st invest",
-            "cash and shortterm invest",
-            "cash and short term invest",
-            "cash shortterm invest",
-            "cash short term invest",
-        ],
-        expr_str="cash[t] + st_invest[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
         "receivables",
         "Receivables",
         extract_names=["receivables", "rec", "accounts receivable", "ar"],
         forecast_config=ForecastItemConfig(pct_of="revenue"),
     ),
     ItemConfig(
         "inventory",
         "Inventory",
         extract_names=["inv", "inventory", "inventories"],
         forecast_config=ForecastItemConfig(pct_of="revenue"),
     ),
     ItemConfig(
+        "lt_invest",
+        "Long-Term Investments",
+        extract_names=[
+            "lt invest",
+            "lt investments",
+            "long term invest",
+            "long term investments",
+            "longterm invest",
+            "longterm investments",
+        ],
+    ),
+    ItemConfig(
         "def_tax_st",
         "Deferred Tax Assets, Current",
         extract_names=[
             "def tax asset curr",
             "deferred tax asset curr",
             "tax asset curr",
             "def tax assets curr",
@@ -126,26 +104,14 @@
             "other current asset",
             "other curr assets",
             "other curr asset",
             "oca",
         ],
     ),
     ItemConfig(
-        "total_current_assets",
-        "Total Current Assets",
-        extract_names=[
-            "total current assets",
-            "tca",
-        ],
-        expr_str="cash_and_st_invest[t] + receivables[t] + inventory[t] + def_tax_st[t] + other_current_assets[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
         "gross_ppe",
         "Gross Property, Plant & Equipment",
         extract_names=[
             "gross ppe",
             "gross property plant equipment",
             "gross property plant and equipment",
             "ppe gross",
@@ -170,33 +136,14 @@
             "acc depreciation",
             "accum depreciation",
             "acc dep",
             "accum dep",
         ],
     ),
     ItemConfig(
-        "net_ppe",
-        "Net Property, Plant & Equipment",
-        extract_names=[
-            "ppe",
-            "property plant equipment",
-            "property plant and equipment",
-            "ppe net",
-            "property plant equipment net",
-            "property plant and equipment net",
-            "net ppe",
-            "net property plant equipment",
-            "net property plant and equipment",
-        ],
-        expr_str="gross_ppe[t] - dep[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
         "goodwill",
         "Goodwill and Intangible Assets",
         extract_names=[
             "goodwill",
             "goodwill and intangible assets",
             "goodwill and intangibles",
             "goodwill intangible assets",
@@ -209,26 +156,14 @@
         ]
         # TODO [#50]: need to be able to extract from multiple items at once
         #
         # Morningstar financial statements have Goodwill and then Intangibles other than Goodwill,
         # both of those should be coming into the Goodwill and Intagible Assets variable.
     ),
     ItemConfig(
-        "lt_invest",
-        "Long-Term Investments",
-        extract_names=[
-            "lt invest",
-            "lt investments",
-            "long term invest",
-            "long term investments",
-            "longterm invest",
-            "longterm investments",
-        ],
-    ),
-    ItemConfig(
         "def_tax_lt",
         "Deferred Tax Assets, Long-Term",
         extract_names=[
             "def tax asset long term",
             "deferred tax asset long term",
             "tax asset long term",
             "def tax assets long term",
@@ -277,39 +212,14 @@
             "longterm assets other",
             "longterm asset other",
             "long term assets other",
             "long term asset other",
         ],
     ),
     ItemConfig(
-        "total_non_current_assets",
-        "Total Non-Current Assets",
-        extract_names=[
-            "total non current assets",
-            "total noncurrent assets",
-            "total lt assets",
-            "total longterm assets",
-            "total long term assets",
-        ],
-        expr_str="net_ppe[t] + goodwill[t] + lt_invest[t] + def_tax_lt[t] + other_lt_assets[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_assets",
-        "Total Assets",
-        extract_names=["total assets", "total asset", "assets", "asset"],
-        expr_str="total_current_assets[t] + total_non_current_assets[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-            balance_with="total_liab_and_equity",
-        ),
-    ),
-    ItemConfig(
         "payables",
         "Payables",
         extract_names=[
             "payables",
             "accounts payable",
             "ap",
             "payables and accrued expenses",
@@ -328,29 +238,14 @@
             "payables and acc exp",
             "payable and acc exps",
             "payable and acc exp",
         ],
         forecast_config=ForecastItemConfig(pct_of="revenue"),
     ),
     ItemConfig(
-        "st_debt",
-        "Short-Term Debt",
-        extract_names=[
-            "st debt",
-            "short term debt",
-            "shortterm debt",
-            "st borrow",
-            "short term borrow",
-            "shortterm borrow" "st borrowings",
-            "short term borrowings",
-            "shortterm borrowings",
-        ],
-        forecast_config=ForecastItemConfig(pct_of="total_debt"),
-    ),
-    ItemConfig(
         "current_lt_debt",
         "Current Portion of Long-Term Debt",
         extract_names=[
             "curr port of lt debt",
             "curr port lt debt",
             "current port of lt debt",
             "current port lt debt",
@@ -398,14 +293,158 @@
             "curr part debt",
             "current part of debt",
             "current part debt",
         ],
         forecast_config=ForecastItemConfig(pct_of="total_debt"),
     ),
     ItemConfig(
+        "st_debt",
+        "Short-Term Debt",
+        extract_names=[
+            "st debt",
+            "short term debt",
+            "shortterm debt",
+            "st borrow",
+            "short term borrow",
+            "shortterm borrow" "st borrowings",
+            "short term borrowings",
+            "shortterm borrowings",
+        ],
+        forecast_config=ForecastItemConfig(pct_of="total_debt"),
+    ),
+    ItemConfig(
+        "lt_debt",
+        "Long-Term Debt",
+        extract_names=[
+            "lt debt",
+            "long term debt",
+            "longterm debt",
+            "lt borrow",
+            "long term borrow",
+            "longterm borrow",
+            "lt borrowings",
+            "long term borrowings",
+            "longterm borrowings",
+            "lt debt total",
+            "long term debt total",
+            "longterm debt total",
+            "lt borrow total",
+            "long term borrow total",
+            "longterm borrow total",
+            "lt borrowings total",
+            "long term borrowings total",
+            "longterm borrowings total",
+        ],
+        forecast_config=ForecastItemConfig(plug=True),
+    ),
+    ItemConfig(
+        "deferred_rev",
+        "Deferred Revenue",
+        extract_names=[
+            "deferred revenue",
+            "deferred sales",
+            "def revenue",
+            "def sales" "non current revenue",
+            "non current sales",
+            "non current revenue def",
+            "non current sales def",
+            "non current revenue deferred",
+            "non current sales deferred",
+            "revenue non current",
+            "sales non current",
+            "revenue def non current",
+            "sales def non current",
+            "revenue deferred non current",
+            "sales deferred non current",
+            "def revenue non current",
+            "def sales non current",
+            "def revenue def non current",
+            "def sales def non current",
+            "def revenue deferred non current",
+            "def sales deferred non current",
+            "deferred revenue non current",
+            "deferred sales non current",
+            "deferred revenue def non current",
+            "deferred sales def non current",
+            "deferred revenue deferred non current",
+            "deferred sales deferred non current",
+            "non curr revenue",
+            "non curr sales",
+            "non curr revenue def",
+            "non curr sales def",
+            "non curr revenue deferred",
+            "non curr sales deferred",
+            "revenue non curr",
+            "sales non curr",
+            "revenue def non curr",
+            "sales def non curr",
+            "revenue deferred non curr",
+            "sales deferred non curr",
+            "def revenue non curr",
+            "def sales non curr",
+            "def revenue def non curr",
+            "def sales def non curr",
+            "def revenue deferred non curr",
+            "def sales deferred non curr",
+            "deferred revenue non curr",
+            "deferred sales non curr",
+            "deferred revenue def non curr",
+            "deferred sales def non curr",
+            "deferred revenue deferred non curr",
+            "deferred sales deferred non curr" "noncurrent revenue",
+            "noncurrent sales",
+            "noncurrent revenue def",
+            "noncurrent sales def",
+            "noncurrent revenue deferred",
+            "noncurrent sales deferred",
+            "revenue noncurrent",
+            "sales noncurrent",
+            "revenue def noncurrent",
+            "sales def noncurrent",
+            "revenue deferred noncurrent",
+            "sales deferred noncurrent",
+            "def revenue noncurrent",
+            "def sales noncurrent",
+            "def revenue def noncurrent",
+            "def sales def noncurrent",
+            "def revenue deferred noncurrent",
+            "def sales deferred noncurrent",
+            "deferred revenue noncurrent",
+            "deferred sales noncurrent",
+            "deferred revenue def noncurrent",
+            "deferred sales def noncurrent",
+            "deferred revenue deferred noncurrent",
+            "deferred sales deferred noncurrent",
+            "noncurr revenue",
+            "noncurr sales",
+            "noncurr revenue def",
+            "noncurr sales def",
+            "noncurr revenue deferred",
+            "noncurr sales deferred",
+            "revenue noncurr",
+            "sales noncurr",
+            "revenue def noncurr",
+            "sales def noncurr",
+            "revenue deferred noncurr",
+            "sales deferred noncurr",
+            "def revenue noncurr",
+            "def sales noncurr",
+            "def revenue def noncurr",
+            "def sales def noncurr",
+            "def revenue deferred noncurr",
+            "def sales deferred noncurr",
+            "deferred revenue noncurr",
+            "deferred sales noncurr",
+            "deferred revenue def noncurr",
+            "deferred sales def noncurr",
+            "deferred revenue deferred noncurr",
+            "deferred sales deferred noncurr",
+        ],
+    ),
+    ItemConfig(
         "tax_liab_st",
         "Tax Liabilities, Short-Term",
         extract_names=[
             "tax liab shortterm",
             "tax liability shortterm",
             "tax liabilities shortterm",
             "tax liab short term",
@@ -544,163 +583,14 @@
             "other liabilities current",
             "other liab current",
             "other liabilities curr",
             "other liab curr",
         ],
     ),
     ItemConfig(
-        "total_current_liab",
-        "Total Current Liabilities",
-        extract_names=[
-            "total current liabilities",
-        ],
-        expr_str="payables[t] + st_debt[t] + tax_liab_st[t] + current_lt_debt[t] + other_current_liab[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "lt_debt",
-        "Long-Term Debt",
-        extract_names=[
-            "lt debt",
-            "long term debt",
-            "longterm debt",
-            "lt borrow",
-            "long term borrow",
-            "longterm borrow",
-            "lt borrowings",
-            "long term borrowings",
-            "longterm borrowings",
-            "lt debt total",
-            "long term debt total",
-            "longterm debt total",
-            "lt borrow total",
-            "long term borrow total",
-            "longterm borrow total",
-            "lt borrowings total",
-            "long term borrowings total",
-            "longterm borrowings total",
-        ],
-        forecast_config=ForecastItemConfig(plug=True),
-    ),
-    ItemConfig(
-        "total_debt",
-        "Total Debt",
-        extract_names=["total debt"],
-        expr_str="st_debt[t] + lt_debt[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "deferred_rev",
-        "Deferred Revenue",
-        extract_names=[
-            "deferred revenue",
-            "deferred sales",
-            "def revenue",
-            "def sales" "non current revenue",
-            "non current sales",
-            "non current revenue def",
-            "non current sales def",
-            "non current revenue deferred",
-            "non current sales deferred",
-            "revenue non current",
-            "sales non current",
-            "revenue def non current",
-            "sales def non current",
-            "revenue deferred non current",
-            "sales deferred non current",
-            "def revenue non current",
-            "def sales non current",
-            "def revenue def non current",
-            "def sales def non current",
-            "def revenue deferred non current",
-            "def sales deferred non current",
-            "deferred revenue non current",
-            "deferred sales non current",
-            "deferred revenue def non current",
-            "deferred sales def non current",
-            "deferred revenue deferred non current",
-            "deferred sales deferred non current",
-            "non curr revenue",
-            "non curr sales",
-            "non curr revenue def",
-            "non curr sales def",
-            "non curr revenue deferred",
-            "non curr sales deferred",
-            "revenue non curr",
-            "sales non curr",
-            "revenue def non curr",
-            "sales def non curr",
-            "revenue deferred non curr",
-            "sales deferred non curr",
-            "def revenue non curr",
-            "def sales non curr",
-            "def revenue def non curr",
-            "def sales def non curr",
-            "def revenue deferred non curr",
-            "def sales deferred non curr",
-            "deferred revenue non curr",
-            "deferred sales non curr",
-            "deferred revenue def non curr",
-            "deferred sales def non curr",
-            "deferred revenue deferred non curr",
-            "deferred sales deferred non curr" "noncurrent revenue",
-            "noncurrent sales",
-            "noncurrent revenue def",
-            "noncurrent sales def",
-            "noncurrent revenue deferred",
-            "noncurrent sales deferred",
-            "revenue noncurrent",
-            "sales noncurrent",
-            "revenue def noncurrent",
-            "sales def noncurrent",
-            "revenue deferred noncurrent",
-            "sales deferred noncurrent",
-            "def revenue noncurrent",
-            "def sales noncurrent",
-            "def revenue def noncurrent",
-            "def sales def noncurrent",
-            "def revenue deferred noncurrent",
-            "def sales deferred noncurrent",
-            "deferred revenue noncurrent",
-            "deferred sales noncurrent",
-            "deferred revenue def noncurrent",
-            "deferred sales def noncurrent",
-            "deferred revenue deferred noncurrent",
-            "deferred sales deferred noncurrent",
-            "noncurr revenue",
-            "noncurr sales",
-            "noncurr revenue def",
-            "noncurr sales def",
-            "noncurr revenue deferred",
-            "noncurr sales deferred",
-            "revenue noncurr",
-            "sales noncurr",
-            "revenue def noncurr",
-            "sales def noncurr",
-            "revenue deferred noncurr",
-            "sales deferred noncurr",
-            "def revenue noncurr",
-            "def sales noncurr",
-            "def revenue def noncurr",
-            "def sales def noncurr",
-            "def revenue deferred noncurr",
-            "def sales deferred noncurr",
-            "deferred revenue noncurr",
-            "deferred sales noncurr",
-            "deferred revenue def noncurr",
-            "deferred sales def noncurr",
-            "deferred revenue deferred noncurr",
-            "deferred sales deferred noncurr",
-        ],
-    ),
-    ItemConfig(
         "tax_liab_lt",
         "Tax Liabilities, Long-Term",
         extract_names=[
             "tax liab longterm",
             "tax liability longterm",
             "tax liabilities longterm",
             "tax liab long term",
@@ -935,43 +825,14 @@
             "liab noncurrent other",
             "liab non current other",
             "liab noncurr other",
             "liab non curr other",
         ],
     ),
     ItemConfig(
-        "total_non_current_liab",
-        "Total Non-Current Liabilities",
-        extract_names=[
-            "total non current liabilities",
-            "total noncurrent liabilities",
-            "total non current liability",
-            "total noncurrent liability",
-            "total non current liab",
-            "total noncurrent liab",
-        ],
-        expr_str="lt_debt[t] + deferred_rev[t] + tax_liab_lt[t] + deposit_liab[t] + other_lt_liab[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_liab",
-        "Total Liabilities",
-        extract_names=[
-            "total liab",
-            "total liability",
-            "total liabilities",
-        ],
-        expr_str="total_non_current_liab[t] + total_current_liab[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
         "common_stock",
         "Common Stock",
         extract_names=[
             "total common stock",
             "total stock",
             "total common shares",
             "total shares",
@@ -991,14 +852,24 @@
             "total shares net",
             "common stock net",
             "stock net" "common shares net",
             "shares net",
         ],
     ),
     ItemConfig(
+        "minority_interest",
+        "Minority Interest",
+        extract_names=[
+            "minority interest",
+            "minority int",
+            "min int",
+            "min interest",
+        ],
+    ),
+    ItemConfig(
         "other_income",
         "Other Comprehensive Income",
         extract_names=[
             "other income",
             "other comprehensive income",
             "other comp income",
             "comp income",
@@ -1025,22 +896,151 @@
         ],
         force_positive=False,
         # TODO [#4]: forecast of retained earnings should be calculated
         #
         # Should be a calculation of retained_earnings[t-1] + net income[t] - dividends[t]
     ),
     ItemConfig(
-        "minority_interest",
-        "Minority Interest",
+        "cash_and_st_invest",
+        "Cash and Short-Term Investments",
         extract_names=[
-            "minority interest",
-            "minority int",
-            "min int",
-            "min interest",
+            "total cash st investments",
+            "total cash and st investments",
+            "total cash and shortterm investments",
+            "total cash and short term investments",
+            "total cash shortterm investments",
+            "total cash short term investments",
+            "total cash st invest",
+            "total cash and st invest",
+            "total cash and shortterm invest",
+            "total cash and short term invest",
+            "total cash shortterm invest",
+            "total cash short term invest",
+            "cash st investments",
+            "cash and st investments",
+            "cash and shortterm investments",
+            "cash and short term investments",
+            "cash shortterm investments",
+            "cash short term investments",
+            "cash st invest",
+            "cash and st invest",
+            "cash and shortterm invest",
+            "cash and short term invest",
+            "cash shortterm invest",
+            "cash short term invest",
+        ],
+        expr_str="cash[t] + st_invest[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_current_assets",
+        "Total Current Assets",
+        extract_names=[
+            "total current assets",
+            "tca",
+        ],
+        expr_str="cash_and_st_invest[t] + receivables[t] + inventory[t] + def_tax_st[t] + other_current_assets[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "net_ppe",
+        "Net Property, Plant & Equipment",
+        extract_names=[
+            "ppe",
+            "property plant equipment",
+            "property plant and equipment",
+            "ppe net",
+            "property plant equipment net",
+            "property plant and equipment net",
+            "net ppe",
+            "net property plant equipment",
+            "net property plant and equipment",
+        ],
+        expr_str="gross_ppe[t] - dep[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_non_current_assets",
+        "Total Non-Current Assets",
+        extract_names=[
+            "total non current assets",
+            "total noncurrent assets",
+            "total lt assets",
+            "total longterm assets",
+            "total long term assets",
+        ],
+        expr_str="net_ppe[t] + goodwill[t] + lt_invest[t] + def_tax_lt[t] + other_lt_assets[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_assets",
+        "Total Assets",
+        extract_names=["total assets", "total asset", "assets", "asset"],
+        expr_str="total_current_assets[t] + total_non_current_assets[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+            balance_with="total_liab_and_equity",
+        ),
+    ),
+    ItemConfig(
+        "total_current_liab",
+        "Total Current Liabilities",
+        extract_names=[
+            "total current liabilities",
+        ],
+        expr_str="payables[t] + st_debt[t] + tax_liab_st[t] + current_lt_debt[t] + other_current_liab[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_debt",
+        "Total Debt",
+        extract_names=["total debt"],
+        expr_str="st_debt[t] + lt_debt[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_non_current_liab",
+        "Total Non-Current Liabilities",
+        extract_names=[
+            "total non current liabilities",
+            "total noncurrent liabilities",
+            "total non current liability",
+            "total noncurrent liability",
+            "total non current liab",
+            "total noncurrent liab",
+        ],
+        expr_str="lt_debt[t] + deferred_rev[t] + tax_liab_lt[t] + deposit_liab[t] + other_lt_liab[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_liab",
+        "Total Liabilities",
+        extract_names=[
+            "total liab",
+            "total liability",
+            "total liabilities",
         ],
+        expr_str="total_non_current_liab[t] + total_current_liab[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
     ),
     ItemConfig(
         "total_equity",
         "Total Stockholder's Equity",
         extract_names=[
             "total equity",
             "total shareholders equity",
@@ -1072,8 +1072,20 @@
         ],
         expr_str="total_liab[t] + total_equity[t]",
         forecast_config=ForecastItemConfig(
             make_forecast=False,
             balance_with="total_assets",
         ),
     ),
+    ItemConfig(
+        "nwc",
+        "Net Working Capital",
+        extract_names=[
+            "nwc",
+        ],
+        expr_str="receivables[t] + inventory[t] - payables[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+        display_verbosity=2,
+    ),
 ]
```

### Comparing `finstmt-1.2.2/finstmt/clean/name.py` & `finstmt-1.3.0/finstmt/clean/name.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/combined/combinator.py` & `finstmt-1.3.0/finstmt/combined/combinator.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/combined/statements.py` & `finstmt-1.3.0/finstmt/combined/statements.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/config_manage/base.py` & `finstmt-1.3.0/finstmt/config_manage/base.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/config_manage/data.py` & `finstmt-1.3.0/finstmt/config_manage/data.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/config_manage/global_.py` & `finstmt-1.3.0/finstmt/config_manage/global_.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/config_manage/statement.py` & `finstmt-1.3.0/finstmt/config_manage/statement.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/config_manage/statements.py` & `finstmt-1.3.0/finstmt/config_manage/statements.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/exc.py` & `finstmt-1.3.0/finstmt/exc.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/findata/database.py` & `finstmt-1.3.0/finstmt/findata/period_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,114 @@
+import json
 import warnings
 from copy import deepcopy
-from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Sequence, Union, cast
+from typing import Dict, List, Optional, cast
 
+import numpy as np
 import pandas as pd
-from sympy import IndexedBase
 
 from finstmt.clean.name import standardize_names_in_series_index
 from finstmt.config_manage.data import DataConfigManager
 from finstmt.exc import CouldNotParseException
-from finstmt.items.config import ItemConfig
+from finstmt.findata.statement_item import StatementItem
 
 
-@dataclass
-class FinDataBase:
+class PeriodFinancialData:
     """
     Base class for financial statement data. Should not be used directly.
     """
 
-    items_config: Union[List[ItemConfig], DataConfigManager] = field(repr=False)
-    prior_statement: Optional["FinDataBase"] = field(default=None, repr=False)
-    unextracted_names: List[str] = field(default_factory=lambda: [], repr=False)
-
-    def __init__(self, *args, **kwargs):
-        raise NotImplementedError
-
-    def __post_init__(self):
-        self.items_config = DataConfigManager(deepcopy(self.items_config))
-        for item in self.items_config:
-            if item.force_positive and item.extract_names is not None:
-                # If extracted and need to force positive, take absolute value
-                value = getattr(self, item.key)
-                if value is None:
-                    continue
-                positive_value = abs(value)
-                setattr(self, item.key, positive_value)
+    config_manager: DataConfigManager
+    prior_statement: Optional["PeriodFinancialData"]
+    unextracted_names: List[str]
+    statement_items: Dict[str, StatementItem]
+
+    # TODO: Set this via user config
+    maximum_display_verbosity = 1
+
+    def __init__(
+        self,
+        data_dict: Dict[str, float],
+        config_manager: DataConfigManager,
+        unextracted_names: List[str],
+        prior_statement: Optional["PeriodFinancialData"] = None,
+    ):
+        self.config_manager = DataConfigManager(deepcopy(config_manager.configs))
+        self.prior_statement = prior_statement
+        self.unextracted_names = unextracted_names
+
+        self.statement_items = {}
+        for item in self.config_manager:
+            self.statement_items[item.key] = StatementItem(
+                item_config=deepcopy(item),
+                value=data_dict.get(item.key, None),
+            )
 
     def _repr_html_(self):
         series = self.to_series()
         df = pd.DataFrame(series)
         return df.applymap(
             lambda x: f"${x:,.0f}" if not x == 0 else " - "
         )._repr_html_()
 
+    def __repr__(self) -> str:
+        statement_items: dict = cast(dict, self.statement_items)
+        results = {}
+        for k, v in statement_items.items():
+            val = v.get_value(self)
+            # Some properties, e.g., nwc and effective tax rate, may be associated with a statements, but we don't
+            # necessarily want to display it on the print-out
+            if (val != 0) and (
+                v.item_config.display_verbosity <= self.maximum_display_verbosity
+            ):
+                results[k] = val
+
+        return json.dumps(results, indent=2)
+
+    def __dir__(self):
+        normal_attrs = [
+            "config_manager",
+            "prior_statement",
+            "unextracted_names",
+            "statement_items",
+            "from_series",
+            "to_series",
+            "dict",
+        ]
+        return normal_attrs + list(self.statement_items.keys())
+
     @classmethod
     def from_series(
         cls,
         series: pd.Series,
-        prior_statement: Optional["FinDataBase"] = None,
-        items_config: Optional[Sequence[ItemConfig]] = None,
+        config_manager: DataConfigManager,
+        prior_statement: Optional["PeriodFinancialData"] = None,
     ):
-        if items_config is None:
-            items_config = cast(Sequence[ItemConfig], cls.items_config)
-
         for_lookup = deepcopy(series)
         standardize_names_in_series_index(for_lookup)
-        data_dict: Dict[str, Union[float, "FinDataBase"]] = {}
+        data_dict: Dict[str, float] = {}
         extracted_name_dict: Dict[str, str] = {}
         original_name_dict: Dict[str, str] = {}
         unextracted_names: List[str] = []
 
-        if prior_statement is not None:
-            data_dict["prior_statement"] = prior_statement
-
         for i, name in enumerate(for_lookup.index):
             orig_name = series.index[i]
-            for item_config in items_config:
+            for item_config in config_manager:
                 if item_config.extract_names is None:
                     # Not an extractable item, must be a calculated item
                     continue
                 if name in item_config.extract_names:
                     # Got a match for series name to allowed names
                     if item_config.key in data_dict:
                         # Multiple matches for data item.
                         # First see if data is the same, then just skip
                         if for_lookup[name] == data_dict[item_config.key]:
                             continue
-                        # Data is not the same, so take the one which is earliest in extract_names
+                        # Data is not the same, so take the one which is
+                        # earliest in extract_names
                         current_match_idx = item_config.extract_names.index(name)
                         existing_match_idx = item_config.extract_names.index(
                             extracted_name_dict[item_config.key]
                         )
                         current_match_is_preferred = (
                             current_match_idx < existing_match_idx
                         )
@@ -106,31 +134,25 @@
         if not data_dict:
             raise CouldNotParseException(
                 "Passed Series did not have any statement items in the index. "
                 "Got index:",
                 series.index,
             )
         return cls(
-            **data_dict, items_config=items_config, unextracted_names=unextracted_names
+            data_dict=data_dict,
+            config_manager=config_manager,
+            unextracted_names=unextracted_names,
+            prior_statement=prior_statement,
         )
 
     def to_series(self) -> pd.Series:
         data_dict = {}
-        for item_config in self.items_config:
+        for item_config in self.config_manager:
             data_dict[item_config.display_name] = getattr(self, item_config.key)
         return pd.Series(data_dict).fillna(0)
 
-    def as_dict(self) -> Dict[str, float]:
-        remove_keys = ["items_config"]
-
-        all_dict = deepcopy(self.__dict__)
-        [all_dict.pop(key) for key in remove_keys]
-        return all_dict
-
-    def get_sympy_subs_dict(self, t_offset: int = 0) -> Dict[IndexedBase, float]:
-        subs_dict = self.items_config.eq_subs_dict(self.as_dict(), t_offset=t_offset)  # type: ignore
-        if self.prior_statement is not None:
-            # Recursively look up prior statements to fill out historical values
-            subs_dict.update(
-                self.prior_statement.get_sympy_subs_dict(t_offset=t_offset - 1)
-            )
-        return subs_dict
+    def __getattr__(self, key: str):
+        try:
+            statement_item = self.statement_items[key]
+        except KeyError:
+            raise AttributeError(key)
+        return np.float64(statement_item.get_value(self))
```

### Comparing `finstmt-1.2.2/finstmt/findata/statementsbase.py` & `finstmt-1.3.0/finstmt/findata/statementsbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 import operator
-from typing import Callable, Dict, List, Optional, Sequence, Tuple
+from typing import Callable, Dict, List, Optional, Tuple
 
 import pandas as pd
 from tqdm import tqdm
 
 from finstmt.check import item_series_is_empty
-from finstmt.config_manage.data import _key_pct_of_key
+from finstmt.config_manage.data import DataConfigManager, _key_pct_of_key
 from finstmt.config_manage.statement import StatementConfigManager
 from finstmt.exc import (
     CouldNotParseException,
     MixedFrequencyException,
     NoSuchItemException,
 )
-from finstmt.findata.database import FinDataBase
+from finstmt.findata.period_data import PeriodFinancialData
 from finstmt.forecast.config import ForecastConfig
 from finstmt.forecast.main import Forecast
 from finstmt.items.config import ItemConfig
 from finstmt.logger import logger
 
 
 class FinStatementsBase:
-    # TODO [#9]: rethink typing for FinStatementsBase considering invariant types
-    #
-    # Was trying to set generic base types in the base class FinStatementsBase
-    # and then in the subclasses, set them to the specific types. But this seems to not
-    # work correctly with mutable collections of the types.
-    #
-    # Currently I have set type ignore for all the subclass typing
-    #
-    # See https://github.com/python/mypy/issues/2984#issuecomment-285721489 for more details
-    statement_cls = FinDataBase  # to be overridden with individual class
-    statements: Dict[pd.Timestamp, FinDataBase]
+    statements: Dict[pd.Timestamp, PeriodFinancialData]
     statement_name: str = "Base"
+    items_config_list: List[ItemConfig]
 
     def __init__(self, *args, **kwargs):
         raise NotImplementedError
 
     def __post_init__(self):
         self.df = self.to_df()
 
@@ -47,36 +38,37 @@
             if i != 0:
                 self.statements[date].prior_statement = self.statements[prior_date]
             prior_date = date
 
         # Create dictionary of individual time period configs to construct the entire statement config
         configs_dict = {}
         for date, statement in self.statements.items():
-            configs_dict[date] = statement.items_config
+            configs_dict[date] = statement.config_manager
         self.config = StatementConfigManager(configs_dict)
 
     def _repr_html_(self):
         return self._formatted_df._repr_html_()
 
+    # Get longitudenal series for a statement item
     def __getattr__(self, item):
         data_dict = {}
-        for date, statement in super().__getattribute__("statements").items():
+        for (
+            date,
+            statement,
+        ) in self.statements.items():
             try:
                 statement_value = getattr(statement, item)
             except AttributeError:
-                # Should hit here on the first loop if this is an invalid item. Raise attribute error like normal.
+                # Should hit here on the first loop if this is an invalid item
+                # Raise attribute error like normal.
                 raise AttributeError(item)
             if pd.isnull(statement_value):
                 statement_value = 0
             data_dict[date] = statement_value
         item_config: Optional[ItemConfig] = None
-        # TODO: Proper names in series for calculated items
-        #  As nwc is calculated only, it does not have a corresponding config item and so the best
-        #  we can do is use the item key as the name. We can solve this by moving everything to
-        #  config items rather than properties.
         try:
             item_config = self.config.get(item)
         except NoSuchItemException:
             pass
         return pd.Series(
             data_dict, name=item_config.display_name if item_config else item
         )
@@ -106,27 +98,33 @@
         item_attrs = dir(list(self.statements.values())[0])
         return normal_attrs + item_attrs
 
     @classmethod
     def from_df(
         cls,
         df: pd.DataFrame,
-        items_config: Optional[Sequence[ItemConfig]] = None,
+        items_config_list: Optional[List[ItemConfig]] = None,
         disp_unextracted: bool = True,
     ):
         """
         DataFrame must have columns as dates and index as names of financial statement items
         """
         statements_dict = {}
         dates = list(df.columns)
         dates.sort(key=lambda t: pd.to_datetime(t))
+
+        if items_config_list is None:
+            config_manager = DataConfigManager(cls.items_config_list.copy())
+        else:
+            config_manager = DataConfigManager(items_config_list.copy())
+
         for col in dates:
             try:
-                statement = cls.statement_cls.from_series(
-                    df[col], items_config=items_config
+                statement = PeriodFinancialData.from_series(
+                    df[col], config_manager=config_manager
                 )
             except CouldNotParseException:
                 raise CouldNotParseException(
                     "Passed DataFrame did not have any statement items in the index. "
                     "Did you set the column with statement items to the index? Got index:",
                     df.index,
                 )
```

### Comparing `finstmt-1.2.2/finstmt/forecast/config.py` & `finstmt-1.3.0/finstmt/forecast/config.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/main.py` & `finstmt-1.3.0/finstmt/forecast/main.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/average.py` & `finstmt-1.3.0/finstmt/forecast/models/average.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/base.py` & `finstmt-1.3.0/finstmt/forecast/models/base.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/cagr.py` & `finstmt-1.3.0/finstmt/forecast/models/cagr.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/chooser.py` & `finstmt-1.3.0/finstmt/forecast/models/chooser.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/manual.py` & `finstmt-1.3.0/finstmt/forecast/models/manual.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/prophet.py` & `finstmt-1.3.0/finstmt/forecast/models/prophet.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/recent.py` & `finstmt-1.3.0/finstmt/forecast/models/recent.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/models/trend.py` & `finstmt-1.3.0/finstmt/forecast/models/trend.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/plot.py` & `finstmt-1.3.0/finstmt/forecast/plot.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/forecast/statements.py` & `finstmt-1.3.0/finstmt/forecast/statements.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/inc/config.py` & `finstmt-1.3.0/finstmt/inc/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,28 +34,15 @@
         "gross_profit",
         "Gross Profit",
         force_positive=False,
         expr_str="revenue[t] - cogs[t]",
         forecast_config=ForecastItemConfig(
             make_forecast=False,
         ),
-    ),
-    ItemConfig(
-        "rd_exp",
-        "R&D Expense",
-        extract_names=[
-            "rd expenses",
-            "rd expense",
-            "rd exp",
-            "rd",
-            "research and development expenses",
-            "research and development expense",
-            "research and development exp",
-            "research and development",
-        ],
+        display_verbosity=2,
     ),
     ItemConfig(
         "sga",
         "SG&A Expense",
         extract_names=[
             "sga",
             "sga expense",
@@ -76,14 +63,68 @@
             "selling general admin",
             "selling general admin expense",
             "selling general admin expenses",
             "selling general admin exp",
         ],
     ),
     ItemConfig(
+        "int_exp",
+        "Interest Expense",
+        extract_names=[
+            "int",
+            "int expense",
+            "int expenses",
+            "int exp",
+            "interest",
+            "interest expense",
+            "interest expenses",
+            "interest exp",
+        ],
+        forecast_config=ForecastItemConfig(pct_of="total_debt"),
+    ),
+    ItemConfig(
+        "tax_exp",
+        "Income Tax Expense",
+        extract_names=[
+            "taxes",
+            "tax",
+            "tax provision",
+            "tax expense",
+            "tax expenses",
+            "tax exp",
+            "income tax",
+            "income tax provision",
+            "income tax expense",
+            "income tax expenses",
+            "income tax exp",
+        ],
+        # TODO [#51]: better handling for income tax expense sign
+        #
+        # This item can be reported as a negative for a positive expense, so previously
+        # had it as forcing positive. But also there can truly be negative expenses if
+        # EBT is negative. Handle determination of whether should be forced positive
+        # based on the EBT value.
+        force_positive=False,
+        forecast_config=ForecastItemConfig(pct_of="ebt"),
+    ),
+    ItemConfig(
+        "rd_exp",
+        "R&D Expense",
+        extract_names=[
+            "rd expenses",
+            "rd expense",
+            "rd exp",
+            "rd",
+            "research and development expenses",
+            "research and development expense",
+            "research and development exp",
+            "research and development",
+        ],
+    ),
+    ItemConfig(
         "dep_exp",
         "Depreciation & Amortization Expense",
         extract_names=[
             "da",
             "dep amort",
             "dep and amort",
             "dep",
@@ -145,73 +186,14 @@
             "other expenses inc",
             "other expense inc",
             "other exps inc",
             "other exp inc",
         ],
     ),
     ItemConfig(
-        "op_exp",
-        "Operating Expense",
-        extract_names=[
-            "op expense",
-            "op expenses",
-            "op exp",
-            "operating expense",
-            "operating expenses",
-            "operating exp",
-        ],
-        forecast_config=ForecastItemConfig(make_forecast=False),
-        expr_str="rd_exp[t] + dep_exp[t] + sga[t] + other_op_exp[t]",
-    ),
-    ItemConfig(
-        "ebit",
-        "Earnings Before Interest and Taxes",
-        extract_names=[
-            "ebit",
-            "earnings before interest and taxes",
-            "earnings before int and taxes",
-            "earnings before interest and tax",
-            "earnings before int and tax",
-            "earn before interest and taxes",
-            "earn before int and taxes",
-            "earn before interest and tax",
-            "earn before int and tax",
-            "earnings before interest taxes",
-            "earnings before int taxes",
-            "earnings before interest tax",
-            "earnings before int tax",
-            "earn before interest taxes",
-            "earn before int taxes",
-            "earn before interest tax",
-            "earn before int tax",
-            "operating income",
-            "op income",
-            "op inc",
-            "operating inc",
-        ],
-        force_positive=False,
-        forecast_config=ForecastItemConfig(make_forecast=False),
-        expr_str="gross_profit[t] - op_exp[t]",
-    ),
-    ItemConfig(
-        "int_exp",
-        "Interest Expense",
-        extract_names=[
-            "int",
-            "int expense",
-            "int expenses",
-            "int exp",
-            "interest",
-            "interest expense",
-            "interest expenses",
-            "interest exp",
-        ],
-        forecast_config=ForecastItemConfig(pct_of="total_debt"),
-    ),
-    ItemConfig(
         "gain_on_sale_invest",
         "Gain on Sale of Investments",
         extract_names=[
             "gain loss on sale of invest",
             "gain loss sale of invest",
             "gain loss sale invest",
             "gain on sale of invest",
@@ -285,14 +267,58 @@
             "asset writedown",
             "assets writedown",
             "asset write down",
             "assets write down",
         ],
     ),
     ItemConfig(
+        "op_exp",
+        "Operating Expense",
+        extract_names=[
+            "op expense",
+            "op expenses",
+            "op exp",
+            "operating expense",
+            "operating expenses",
+            "operating exp",
+        ],
+        forecast_config=ForecastItemConfig(make_forecast=False),
+        expr_str="rd_exp[t] + dep_exp[t] + sga[t] + other_op_exp[t]",
+    ),
+    ItemConfig(
+        "ebit",
+        "Earnings Before Interest and Taxes",
+        extract_names=[
+            "ebit",
+            "earnings before interest and taxes",
+            "earnings before int and taxes",
+            "earnings before interest and tax",
+            "earnings before int and tax",
+            "earn before interest and taxes",
+            "earn before int and taxes",
+            "earn before interest and tax",
+            "earn before int and tax",
+            "earnings before interest taxes",
+            "earnings before int taxes",
+            "earnings before interest tax",
+            "earnings before int tax",
+            "earn before interest taxes",
+            "earn before int taxes",
+            "earn before interest tax",
+            "earn before int tax",
+            "operating income",
+            "op income",
+            "op inc",
+            "operating inc",
+        ],
+        force_positive=False,
+        forecast_config=ForecastItemConfig(make_forecast=False),
+        expr_str="gross_profit[t] - op_exp[t]",
+    ),
+    ItemConfig(
         "ebt",
         "Earnings Before Tax",
         extract_names=[
             "ebt",
             "earnings before taxes",
             "earnings before tax",
             "earn before tax",
@@ -318,39 +344,14 @@
             "income pre tax",
         ],
         force_positive=False,
         forecast_config=ForecastItemConfig(make_forecast=False),
         expr_str="ebit[t] - int_exp[t]",
     ),
     ItemConfig(
-        "tax_exp",
-        "Income Tax Expense",
-        extract_names=[
-            "taxes",
-            "tax",
-            "tax provision",
-            "tax expense",
-            "tax expenses",
-            "tax exp",
-            "income tax",
-            "income tax provision",
-            "income tax expense",
-            "income tax expenses",
-            "income tax exp",
-        ],
-        # TODO [#51]: better handling for income tax expense sign
-        #
-        # This item can be reported as a negative for a positive expense, so previously
-        # had it as forcing positive. But also there can truly be negative expenses if
-        # EBT is negative. Handle determination of whether should be forced positive
-        # based on the EBT value.
-        force_positive=False,
-        forecast_config=ForecastItemConfig(pct_of="ebt"),
-    ),
-    ItemConfig(
         "net_income",
         "Net Income",
         extract_names=[
             "net income",
             "net inc",
             "earnings",
             "earn",
```

### Comparing `finstmt-1.2.2/finstmt/inc/main.py` & `finstmt-1.3.0/finstmt/inc/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dataclasses import dataclass
 from typing import Dict
 
 import pandas as pd
 
+from finstmt.findata.period_data import PeriodFinancialData
 from finstmt.findata.statementsbase import FinStatementsBase
-from finstmt.inc.data import IncomeStatementData
+from finstmt.inc.config import INCOME_STATEMENT_INPUT_ITEMS
 
 
 @dataclass
 class IncomeStatements(FinStatementsBase):
     """
     Main class for holding income statement data. Usual way to construct is with the .from_df method.
 
     Examples:
         >>> inc_path = r'WMT Income Statement.xlsx'
         >>> inc_df = pd.read_excel(inc_path)
         >>> inc_data = IncomeStatements.from_df(inc_df)
     """
 
-    statements: Dict[pd.Timestamp, IncomeStatementData]  # type: ignore
-
-    statement_cls = IncomeStatementData  # type: ignore
+    statements: Dict[pd.Timestamp, PeriodFinancialData]  # type: ignore
     statement_name = "Income Statement"
+    items_config_list = INCOME_STATEMENT_INPUT_ITEMS
```

### Comparing `finstmt-1.2.2/finstmt/items/config.py` & `finstmt-1.3.0/finstmt/items/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,14 +18,22 @@
     extract_names: Optional[Sequence[str]] = None
     force_positive: bool = True
     forecast_config: ForecastItemConfig = field(
         default_factory=lambda: ForecastItemConfig()
     )
     expr_str: Optional[str] = None
 
+    # The required verbosity level to display this item in the output
+    # 0: always display
+    # 1: display in the default output
+    # 2: display in verbose output
+    # 3: display in very verbose output
+    # ... and so on
+    display_verbosity: int = 1
+
     # TODO [#19]: add config and logic for whether to take highest priority or add all of matching names
     #
     # When extracting impairment, in Capital IQ data it has Impairment of Goodwill and Asset Writedown,
     # both of which should be included. This is in contrast to most others where only the highest priority
     # key should be selected
 
     @property
@@ -60,15 +68,16 @@
 def _apply_operation_to_item_config(
     item_config: ItemConfig,
     other: T,
     func: Callable[[ItemConfigOperationData, T], ItemConfigOperationData],
 ) -> ItemConfig:
     updates: Dict[str, Any] = {}
     updates["forecast_config"] = func(
-        item_config.forecast_config, _get_attr_if_needed(other, "forecast_config")
+        item_config.forecast_config,
+        _get_attr_if_needed(other, "forecast_config"),
     )
     return item_config.copy(**updates)
 
 
 def _get_attr_if_needed(other: Any, attr: str) -> Any:
     if isinstance(other, ItemConfig):
         return getattr(other, attr)
```

### Comparing `finstmt-1.2.2/finstmt/loaders/capiq.py` & `finstmt-1.3.0/finstmt/loaders/capiq.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/resolver/base.py` & `finstmt-1.3.0/finstmt/resolver/base.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/resolver/forecast.py` & `finstmt-1.3.0/finstmt/resolver/forecast.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/resolver/history.py` & `finstmt-1.3.0/finstmt/resolver/history.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/finstmt/resolver/solve.py` & `finstmt-1.3.0/finstmt/resolver/solve.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.2.2/pyproject.toml` & `finstmt-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
-[tool.poetry]
+[project]
 name = "finstmt"
 version = "1.2.2"
+
+[tool.setuptools]
+py-modules = ['finstmt']
+
+[tool.poetry]
+name = "finstmt"
+version = "1.3.0"
 description = "Contains classes to work with financial statement data. Can calculate free cash flows and help project financial statements."
 authors = ["Nick DeRobertis <whoopnip@gmail.com>"]
 readme = "README.md"
 packages = [{include = "finstmt"}]
 license = "MIT"
 classifiers = [
     # How mature is this project? Common values are
@@ -52,7 +59,8 @@
 
 [tool.black]
 include = 'finstmt.*\.pyi?$|tests.*\.pyi?$'
 
 [tool.isort]
 profile = "black"
 skip = ['.bzr', '.direnv', '.eggs', '.git', '.hg', '.mypy_cache', '.pants.d', '.svn', '.tox', '.venv', '__pypackages__', '_build', 'buck-out', 'build', 'dist', 'node_modules', '.venvs']
+
```

### Comparing `finstmt-1.2.2/setup.py` & `finstmt-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'xlrd']
 
 extras_require = \
 {'forecast': ['prophet']}
 
 setup_kwargs = {
     'name': 'finstmt',
-    'version': '1.2.2',
+    'version': '1.3.0',
     'description': 'Contains classes to work with financial statement data. Can calculate free cash flows and help project financial statements.',
     'long_description': "\n\n[![](https://codecov.io/gh/nickderobertis/py-finstmt/branch/master/graph/badge.svg)](https://codecov.io/gh/nickderobertis/py-finstmt)\n[![PyPI](https://img.shields.io/pypi/v/finstmt)](https://pypi.org/project/finstmt/)\n![PyPI - License](https://img.shields.io/pypi/l/finstmt)\n[![Documentation](https://img.shields.io/badge/documentation-pass-green)](https://nickderobertis.github.io/py-finstmt/)\n![Tests Run on Ubuntu Python Versions](https://img.shields.io/badge/Tests%20Ubuntu%2FPython-3.8%20%7C%203.9%20%7C%203.10-blue)\n![Tests Run on Macos Python Versions](https://img.shields.io/badge/Tests%20Macos%2FPython-3.8%20%7C%203.9%20%7C%203.10-blue)\n![Tests Run on Windows Python Versions](https://img.shields.io/badge/Tests%20Windows%2FPython-3.8%20%7C%203.9%20%7C%203.10-blue)\n[![Github Repo](https://img.shields.io/badge/repo-github-informational)](https://github.com/nickderobertis/py-finstmt/)\n\n\n#  py-finstmt\n\n## Overview\n\nContains classes to work with financial statement data. Can calculate free cash flows and help project financial statements.\n\n## Getting Started\n\nInstall `finstmt`:\n\n```\npip install finstmt\n```\n\nA simple example:\n\n```python\nfrom finstmt import BalanceSheets, IncomeStatements, FinancialStatements\nimport pandas as pd\n\nbs_path = r'WMT Balance Sheet.xlsx'\ninc_path = r'WMT Income Statement.xlsx'\nbs_df = pd.read_excel(bs_path)\ninc_df = pd.read_excel(inc_path)\nbs_data = BalanceSheets.from_df(bs_df)\ninc_data = IncomeStatements.from_df(inc_df)\nstmts = FinancialStatements(inc_data, bs_data)\n```\n\nSee a\n[more in-depth tutorial here.](\nhttps://nickderobertis.github.io/py-finstmt/tutorial.html\n)\n\n## Links\n\nSee the\n[documentation here.](\nhttps://nickderobertis.github.io/py-finstmt/\n)\n\n## Development Status\n\nThis project is currently in early-stage development. There may be\nbreaking changes often. While the major version is 0, minor version\nupgrades will often have breaking changes.\n\n## Developing\n\nSee the [development guide](\nhttps://github.com/nickderobertis/py-finstmt/blob/master/DEVELOPING.md\n) for development details.\n\n## Author\n\nCreated by Nick DeRobertis. MIT License.\n\n",
     'author': 'Nick DeRobertis',
     'author_email': 'whoopnip@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `finstmt-1.2.2/PKG-INFO` & `finstmt-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finstmt
-Version: 1.2.2
+Version: 1.3.0
 Summary: Contains classes to work with financial statement data. Can calculate free cash flows and help project financial statements.
 License: MIT
 Author: Nick DeRobertis
 Author-email: whoopnip@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

