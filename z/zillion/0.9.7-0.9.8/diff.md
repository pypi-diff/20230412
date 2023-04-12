# Comparing `tmp/zillion-0.9.7.tar.gz` & `tmp/zillion-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillion-0.9.7.tar", last modified: Wed Apr 12 13:15:25 2023, max compression
+gzip compressed data, was "zillion-0.9.8.tar", last modified: Wed Apr 12 17:36:28 2023, max compression
```

## Comparing `zillion-0.9.7.tar` & `zillion-0.9.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 13:15:25.630209 zillion-0.9.7/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.7/AUTHORS.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.7/LICENSE
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 13:15:25.630209 zillion-0.9.7/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-12 13:15:10.000000 zillion-0.9.7/README.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-12 13:15:25.630209 zillion-0.9.7/setup.cfg
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2885 2023-04-12 01:54:36.000000 zillion-0.9.7/setup.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 13:15:25.626209 zillion-0.9.7/zillion/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.7/zillion/configs.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.7/zillion/core.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    69368 2023-04-10 14:08:30.000000 zillion-0.9.7/zillion/datasource.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 13:15:25.630209 zillion-0.9.7/zillion/dialects/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.7/zillion/dialects/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/dialects/conversions.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.7/zillion/dialects/duckdb.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/dialects/mysql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/dialects/postgresql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/dialects/sqlite.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-04-12 12:47:48.000000 zillion-0.9.7/zillion/field.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.7/zillion/model.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    37273 2023-04-12 01:50:57.000000 zillion-0.9.7/zillion/nlp.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    84647 2023-04-12 13:14:09.000000 zillion-0.9.7/zillion/report.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 13:15:25.630209 zillion-0.9.7/zillion/scripts/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/scripts/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.7/zillion/scripts/bootstrap_datasource_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/scripts/json_to_yaml.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1241 2023-04-10 13:55:59.000000 zillion-0.9.7/zillion/scripts/load_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2674 2023-04-12 12:40:39.000000 zillion-0.9.7/zillion/scripts/run_report.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.7/zillion/scripts/yaml_to_json.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.7/zillion/sql_utils.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-12 13:12:51.000000 zillion-0.9.7/zillion/version.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-04 01:10:26.000000 zillion-0.9.7/zillion/warehouse.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 13:15:25.630209 zillion-0.9.7/zillion.egg-info/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 13:15:25.000000 zillion-0.9.7/zillion.egg-info/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      768 2023-04-12 13:15:25.000000 zillion-0.9.7/zillion.egg-info/SOURCES.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-12 13:15:25.000000 zillion-0.9.7/zillion.egg-info/dependency_links.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1080 2023-04-12 13:15:25.000000 zillion-0.9.7/zillion.egg-info/requires.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-12 13:15:25.000000 zillion-0.9.7/zillion.egg-info/top_level.txt
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.354758 zillion-0.9.8/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.8/AUTHORS.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.8/LICENSE
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 17:36:28.354758 zillion-0.9.8/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-12 13:15:10.000000 zillion-0.9.8/README.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-12 17:36:28.354758 zillion-0.9.8/setup.cfg
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2885 2023-04-12 01:54:36.000000 zillion-0.9.8/setup.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.350760 zillion-0.9.8/zillion/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.8/zillion/configs.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.8/zillion/core.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    69368 2023-04-10 14:08:30.000000 zillion-0.9.8/zillion/datasource.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.350760 zillion-0.9.8/zillion/dialects/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.8/zillion/dialects/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/conversions.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.8/zillion/dialects/duckdb.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/mysql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/postgresql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/sqlite.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-04-12 12:47:48.000000 zillion-0.9.8/zillion/field.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.8/zillion/model.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    38893 2023-04-12 17:33:37.000000 zillion-0.9.8/zillion/nlp.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    84745 2023-04-12 17:17:38.000000 zillion-0.9.8/zillion/report.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.354758 zillion-0.9.8/zillion/scripts/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/scripts/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.8/zillion/scripts/bootstrap_datasource_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/scripts/json_to_yaml.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1241 2023-04-10 13:55:59.000000 zillion-0.9.8/zillion/scripts/load_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2674 2023-04-12 12:40:39.000000 zillion-0.9.8/zillion/scripts/run_report.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/scripts/yaml_to_json.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.8/zillion/sql_utils.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-12 17:31:42.000000 zillion-0.9.8/zillion/version.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-12 17:03:08.000000 zillion-0.9.8/zillion/warehouse.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.350760 zillion-0.9.8/zillion.egg-info/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      768 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/SOURCES.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/dependency_links.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1080 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/requires.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/top_level.txt
```

### Comparing `zillion-0.9.7/LICENSE` & `zillion-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/PKG-INFO` & `zillion-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.7
+Version: 0.9.8
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.7/README.md` & `zillion-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/setup.py` & `zillion-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/configs.py` & `zillion-0.9.8/zillion/configs.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/core.py` & `zillion-0.9.8/zillion/core.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/datasource.py` & `zillion-0.9.8/zillion/datasource.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/dialects/conversions.py` & `zillion-0.9.8/zillion/dialects/conversions.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/dialects/duckdb.py` & `zillion-0.9.8/zillion/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/dialects/mysql.py` & `zillion-0.9.8/zillion/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/dialects/postgresql.py` & `zillion-0.9.8/zillion/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/dialects/sqlite.py` & `zillion-0.9.8/zillion/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/field.py` & `zillion-0.9.8/zillion/field.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/model.py` & `zillion-0.9.8/zillion/model.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/nlp.py` & `zillion-0.9.8/zillion/nlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     pass
 
 from sqlalchemy import and_
 from sqlalchemy.schema import CreateTable
 from tlbx import raiseifnot, st, json
 
 from zillion.core import (
+    dbg,
     info,
     warn,
     error,
     zillion_config,
     nlp_installed,
     RollupTypes,
     FieldTypes,
@@ -607,15 +608,15 @@
     (*llm*) - A langchain OpenAI LLM
 
     """
     model = model or zillion_config["OPENAI_MODEL"]
     key = zillion_config["OPENAI_API_KEY"]
     raiseifnot(model and key, "Missing OpenAI API key or model name in zillion config")
     max_tokens = max_tokens or LLM_MAX_TOKENS
-    info(f"Building OpenAI {model} chain with max_tokens={max_tokens}")
+    dbg(f"Building OpenAI {model} chain with max_tokens={max_tokens}")
     openai_class = get_openai_class(model)
     return openai_class(
         model_name=model,
         temperature=0,
         max_tokens=max_tokens,
         request_timeout=request_timeout,
         max_retries=1,
@@ -647,15 +648,15 @@
     """
     llm = llm or build_llm(
         model=model, max_tokens=max_tokens, request_timeout=request_timeout
     )
     return LLMChain(llm=llm, prompt=prompt)
 
 
-TEXT_TO_REPORT_V1 = """You are an expert SQL analyst that takes natural language input and outputs metrics, dimensions, criteria, ordering, and limit settings in JSON format.
+TEXT_TO_REPORT_NO_FIELDS = """You are an expert SQL analyst that takes natural language input and outputs metrics, dimensions, criteria, ordering, and limit settings in JSON format.
 If a relative date is specified, such as "yesterday", replace it with the actual date. The current date is: {current_date}
 
 Generic Example 1:
 
 Input: revenue and sales by date for the last 30 days. Rows with more than 5 sales.
 Output:
 {{
@@ -689,15 +690,15 @@
 
 ----
 Complete the following. Use JSON format and include no other commentary.
 Input: {query}
 JSON Output:"""
 
 
-TEXT_TO_REPORT_V2 = """You are an expert SQL analyst that takes natural language input and outputs metrics, dimensions, criteria, ordering, and limit settings in JSON format.
+TEXT_TO_REPORT_ALL_FIELDS = """You are an expert SQL analyst that takes natural language input and outputs metrics, dimensions, criteria, ordering, and limit settings in JSON format.
 If a relative date is specified, such as "yesterday", replace it with the actual date. The current date is: {current_date}
 
 Supported metrics:
 {metrics}
 
 Supported dimensions:
 {dimensions}
@@ -736,14 +737,58 @@
 }}
 
 ----
 Complete the following. Use JSON format and include no other commentary. Use only supported metrics and dimensions.
 Input: {query}
 JSON Output:"""
 
+TEXT_TO_REPORT_DIMENSION_FIELDS = """You are an expert SQL analyst that takes natural language input and outputs metrics, dimensions, criteria, ordering, and limit settings in JSON format.
+If a relative date is specified, such as "yesterday", replace it with the actual date. The current date is: {current_date}
+
+Supported dimensions:
+{dimensions}
+
+Generic Example 1:
+
+Input: revenue and sales by date for the last 30 days. Rows with more than 5 sales.
+JSON Output:
+{{
+  "metrics": ["revenue", "sales"],
+  "dimensions": ["date"],
+  "criteria": [
+    ["date", ">=", "{thirty_days_ago}"]
+  ],
+  "row_filters": [
+    ["sales", ">", 5]
+]
+}}
+
+Generic Example 2:
+
+Input: show me the top 10 campaigns by revenue yesterday for ad engine Google. Include totals.
+JSON Output:
+{{
+  "metrics": ["revenue"],
+  "dimensions": ["campaign"],
+  "criteria": [
+    ["date", "=", "{yesterday}"],
+    ["ad_engine", "=", "Google"]
+  ],
+  "limit": 10,
+  "order_by": [
+    ["revenue", "desc"]
+  ],
+  "rollup": "totals"
+}}
+
+----
+Complete the following. Use JSON format and include no other commentary.
+Input: {query}
+JSON Output:"""
+
 
 def parse_text_to_report_json_output(output):
     """Parse the output of a chain that produces Zillion args as JSON
 
     **Parameters:**
 
     * **output** - (str) The output of the chain, expected to be valid JSON.
@@ -758,27 +803,29 @@
     try:
         return {k: v for k, v in json.loads(output).items() if v}
     except Exception as e:
         error(f"Error parsing JSON:\n{output}")
         raise
 
 
+# TODO - share code for configs below
+
 PROMPT_CONFIGS = dict(
-    v1=dict(
-        prompt_text=TEXT_TO_REPORT_V1,
+    no_fields=dict(
+        prompt_text=TEXT_TO_REPORT_NO_FIELDS,
         input_variables=["query", "current_date", "yesterday", "thirty_days_ago"],
         context_func=lambda wh: dict(
             current_date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             yesterday=str(datetime.now().date() - timedelta(days=1)),
             thirty_days_ago=str(datetime.now().date() - timedelta(days=30)),
         ),
         parser=parse_text_to_report_json_output,
     ),
-    v2=dict(
-        prompt_text=TEXT_TO_REPORT_V2,
+    all_fields=dict(
+        prompt_text=TEXT_TO_REPORT_ALL_FIELDS,
         input_variables=[
             "query",
             "current_date",
             "yesterday",
             "thirty_days_ago",
             "metrics",
             "dimensions",
@@ -788,14 +835,31 @@
             dimensions=get_dimensions_prompt_str(wh),
             current_date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             yesterday=str(datetime.now().date() - timedelta(days=1)),
             thirty_days_ago=str(datetime.now().date() - timedelta(days=30)),
         ),
         parser=parse_text_to_report_json_output,
     ),
+    dimension_fields=dict(
+        prompt_text=TEXT_TO_REPORT_DIMENSION_FIELDS,
+        input_variables=[
+            "query",
+            "current_date",
+            "yesterday",
+            "thirty_days_ago",
+            "dimensions",
+        ],
+        context_func=lambda wh: dict(
+            dimensions=get_dimensions_prompt_str(wh),
+            current_date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            yesterday=str(datetime.now().date() - timedelta(days=1)),
+            thirty_days_ago=str(datetime.now().date() - timedelta(days=30)),
+        ),
+        parser=parse_text_to_report_json_output,
+    ),
 )
 
 
 def get_field_name_variants(name):
     """Get a list of possible close variants of a field name. This is
     an 80/20 hack to help with fuzzy matching of field names.
 
@@ -920,17 +984,14 @@
         elif k == "limit":
             res[k] = int(v) if v is not None else None
         else:
             raise ValueError(f"Unexpected key {k}")
     return res
 
 
-text_to_report_chain = None
-
-
 def get_fields_prompt_str(fields):
     """Get a string representing names/types of given fields"""
     res = []
     for name, fdef in fields.items():
         type_str = str(fdef.type).lower() if fdef.type else "unknown"
         res.append(f"{name} ({type_str})")
     return "\n".join(res)
@@ -944,15 +1005,15 @@
     return get_fields_prompt_str(warehouse.get_dimensions())
 
 
 class MaxTokensException(Exception):
     pass
 
 
-def text_to_report_params(query, warehouse=None, prompt_version="v1"):
+def text_to_report_params(query, warehouse=None, prompt_version="no_fields"):
     """Convert a natural language input to Zillion report params
 
     **Parameters:**
 
     * **query** - (str) The natural language query to convert.
     * **warehouse** - (Warehouse, optional) The warehouse to map the report params to
     * **prompt_version** - (str) The version of the prompt to use
@@ -968,18 +1029,16 @@
     context = prompt_config["context_func"](warehouse)
     context["query"] = query
     prompt = PromptTemplate(
         input_variables=prompt_config["input_variables"],
         template=prompt_config["prompt_text"],
     )
 
-    global text_to_report_chain
-    if not text_to_report_chain:
-        llm = build_llm(max_tokens=-1)
-        text_to_report_chain = build_chain(prompt, llm=llm)
+    llm = build_llm(max_tokens=-1)
+    text_to_report_chain = build_chain(prompt, llm=llm)
 
     prompt_tokens = text_to_report_chain.llm.get_num_tokens(prompt.format(**context))
     max_tokens = get_openai_model_context_size(text_to_report_chain.llm.model_name)
     if (prompt_tokens + 500) >= max_tokens:
         raise MaxTokensException(f"Prompt is too long: {prompt_tokens} tokens")
 
     llm_start = time.time()
@@ -1024,17 +1083,14 @@
             warn(f"Invalid row in NLP table relationships output: {row}")
             continue
         child_column, parent_column = [x.strip() for x in row.split("->")]
         child_parent[child_column] = parent_column
     return child_parent
 
 
-relationship_chain = None
-
-
 def get_nlp_table_relationships(metadata, table_names):
     """
     Get the NLP table relationships for the given tables. Note: if a table has
     a composite primary key it will be skipped.
 
     **Parameters:**
 
@@ -1063,21 +1119,19 @@
             f"Table: {table_name}\n"
             "Fields:\n"
             f"{chr(10).join(get_column_str(c) for c in table.columns)}"
         )
 
     table_defs_str = "\n\n".join(table_defs)
 
-    global relationship_chain
-    if not relationship_chain:
-        prompt = PromptTemplate(
-            input_variables=["table_defs"],
-            template=NLP_TABLE_RELATIONSHIP_PROMPT,
-        )
-        relationship_chain = build_chain(prompt)
+    prompt = PromptTemplate(
+        input_variables=["table_defs"],
+        template=NLP_TABLE_RELATIONSHIP_PROMPT,
+    )
+    relationship_chain = build_chain(prompt)
 
     llm_start = time.time()
     output = relationship_chain.run(table_defs_str).strip(". -\n\r")
     info(output)
     info(f"LLM took {time.time() - llm_start:.3f}s")
     return parse_nlp_table_relationships(output)
```

### Comparing `zillion-0.9.7/zillion/report.py` & `zillion-0.9.8/zillion/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -2131,20 +2131,25 @@
         * **allow_partial** - (*bool, optional*) Allow partial report results
 
         **Returns:**
 
         * **report** - (*Report*) A report object
 
         """
-        try:
-            # Try the V2 prompt first which includes metrics/dimensions
-            # in the prompt. If that fails, try the V1 prompt.
-            params = text_to_report_params(text, warehouse, prompt_version="v2")
-        except MaxTokensException as e:
-            params = text_to_report_params(text, warehouse, prompt_version="v1")
+
+        params = None
+        prompts = ["all_fields", "dimension_fields", "no_fields"]
+        for prompt in prompts:
+            try:
+                params = text_to_report_params(text, warehouse, prompt_version=prompt)
+                break
+            except MaxTokensException as e:
+                warn(f"Max tokens exceeded, retrying with fallback prompt")
+
+        raiseifnot(params, "Could not parse report params from text: %s" % text)
 
         report_params = map_warehouse_report_params(warehouse, params)
         return Report(
             warehouse,
             **report_params,
             adhoc_datasources=adhoc_datasources,
             allow_partial=allow_partial,
```

### Comparing `zillion-0.9.7/zillion/scripts/bootstrap_datasource_config.py` & `zillion-0.9.8/zillion/scripts/bootstrap_datasource_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/scripts/load_config.py` & `zillion-0.9.8/zillion/scripts/load_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/scripts/run_report.py` & `zillion-0.9.8/zillion/scripts/run_report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/sql_utils.py` & `zillion-0.9.8/zillion/sql_utils.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion/warehouse.py` & `zillion-0.9.8/zillion/warehouse.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion.egg-info/PKG-INFO` & `zillion-0.9.8/zillion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.7
+Version: 0.9.8
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.7/zillion.egg-info/SOURCES.txt` & `zillion-0.9.8/zillion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zillion-0.9.7/zillion.egg-info/requires.txt` & `zillion-0.9.8/zillion.egg-info/requires.txt`

 * *Files identical despite different names*

