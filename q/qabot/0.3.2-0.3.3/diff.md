# Comparing `tmp/qabot-0.3.2.tar.gz` & `tmp/qabot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qabot-0.3.2.tar", max compression
+gzip compressed data, was "qabot-0.3.3.tar", max compression
```

## Comparing `qabot-0.3.2.tar` & `qabot-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-03-27 21:19:57.134744 qabot-0.3.2/LICENSE
--rw-r--r--   0        0        0     5039 2023-04-12 02:14:39.645321 qabot-0.3.2/README.md
--rw-r--r--   0        0        0      711 2023-04-12 02:28:41.354245 qabot-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      709 2023-04-12 01:11:09.111570 qabot-0.3.2/qabot/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.3.2/qabot/agents/__init__.py
--rw-r--r--   0        0        0     4365 2023-04-12 02:05:45.393093 qabot-0.3.2/qabot/agents/agent.py
--rw-r--r--   0        0        0    10860 2023-04-12 02:00:21.625211 qabot-0.3.2/qabot/agents/data_query_chain.py
--rw-r--r--   0        0        0     1707 2023-03-27 21:19:57.138745 qabot-0.3.2/qabot/caching.py
--rw-r--r--   0        0        0     6471 2023-04-12 02:06:49.481090 qabot-0.3.2/qabot/cli.py
--rw-r--r--   0        0        0      390 2023-04-12 02:06:49.469090 qabot-0.3.2/qabot/config.py
--rw-r--r--   0        0        0     3378 2023-03-27 21:34:35.864207 qabot-0.3.2/qabot/duckdb_manual_data_loader.py
--rw-r--r--   0        0        0     1339 2023-04-12 02:28:36.278238 qabot-0.3.2/qabot/duckdb_query.py
--rw-r--r--   0        0        0     2555 2023-04-12 00:25:15.975882 qabot-0.3.2/qabot/progress_callback.py
--rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.3.2/qabot/tools/__init__.py
--rw-r--r--   0        0        0      518 2023-03-27 21:19:57.138745 qabot-0.3.2/qabot/tools/describe_duckdb_table.py
--rw-r--r--   0        0        0     1027 2023-03-27 21:19:57.138745 qabot-0.3.2/qabot/tools/duckdb_execute_tool.py
--rw-r--r--   0        0        0     2681 2023-04-11 22:19:46.181702 qabot-0.3.2/qabot/tools/wikidata.py
--rw-r--r--   0        0        0     5790 1970-01-01 00:00:00.000000 qabot-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-27 21:19:57.134744 qabot-0.3.3/LICENSE
+-rw-r--r--   0        0        0     5039 2023-04-12 02:14:39.645321 qabot-0.3.3/README.md
+-rw-r--r--   0        0        0      711 2023-04-12 02:30:40.274395 qabot-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-04-12 01:11:09.111570 qabot-0.3.3/qabot/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.3.3/qabot/agents/__init__.py
+-rw-r--r--   0        0        0     4495 2023-04-12 02:30:40.262395 qabot-0.3.3/qabot/agents/agent.py
+-rw-r--r--   0        0        0    10860 2023-04-12 02:00:21.625211 qabot-0.3.3/qabot/agents/data_query_chain.py
+-rw-r--r--   0        0        0     1707 2023-03-27 21:19:57.138745 qabot-0.3.3/qabot/caching.py
+-rw-r--r--   0        0        0     6471 2023-04-12 02:06:49.481090 qabot-0.3.3/qabot/cli.py
+-rw-r--r--   0        0        0      390 2023-04-12 02:06:49.469090 qabot-0.3.3/qabot/config.py
+-rw-r--r--   0        0        0     3378 2023-03-27 21:34:35.864207 qabot-0.3.3/qabot/duckdb_manual_data_loader.py
+-rw-r--r--   0        0        0     1339 2023-04-12 02:28:36.278238 qabot-0.3.3/qabot/duckdb_query.py
+-rw-r--r--   0        0        0     2555 2023-04-12 00:25:15.975882 qabot-0.3.3/qabot/progress_callback.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.3.3/qabot/tools/__init__.py
+-rw-r--r--   0        0        0      518 2023-03-27 21:19:57.138745 qabot-0.3.3/qabot/tools/describe_duckdb_table.py
+-rw-r--r--   0        0        0     1027 2023-03-27 21:19:57.138745 qabot-0.3.3/qabot/tools/duckdb_execute_tool.py
+-rw-r--r--   0        0        0     2681 2023-04-11 22:19:46.181702 qabot-0.3.3/qabot/tools/wikidata.py
+-rw-r--r--   0        0        0     5790 1970-01-01 00:00:00.000000 qabot-0.3.3/PKG-INFO
```

### Comparing `qabot-0.3.2/LICENSE` & `qabot-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/README.md` & `qabot-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/pyproject.toml` & `qabot-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qabot"
-version = "0.3.2"
+version = "0.3.3"
 license = "Apache-2.0"
 description = "Query local or remote data files with natural language queries powered by OpenAI and DuckDB."
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "qabot"}]
 
 [tool.poetry.scripts]
```

### Comparing `qabot-0.3.2/qabot/__init__.py` & `qabot-0.3.3/qabot/__init__.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/agents/agent.py` & `qabot-0.3.3/qabot/agents/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,42 +36,45 @@
     db_chain = get_duckdb_data_query_chain(
         llm=llm,
         database=database_engine,
         callback_manager=callback_manager,
         verbose=verbose
     )
 
-    tools = [
-        # Tool(
-        #     name="Python",
-        #     func=python_chain.run,
-        #     description="Useful for when you need to run a quick simulation, or answer questions about math"
-        # ),
-        Tool(
-            name="Show Tables",
-            func=lambda _: run_sql_catch_error(database_engine, "show tables"),
-            description="Useful to show the locally available database tables and views. Empty input required."
-        ),
-        Tool(
-            name="Describe Table",
-            func=lambda table: describe_table_or_view(database_engine, table),
-            description="Useful to show the column names and types of a local database table or view. Use the table name as the input."
-        ),
-        Tool(
-            name="Data Op",
-            func=lambda query: db_chain({
-                'table_names': run_sql_catch_error(database_engine, "select table_name, table_schema from information_schema.tables;"),
-                'input': query
-            }),
-            description=textwrap.dedent("""Useful to interact with local data tables. 
-            Input should be a natural language question containing full context including what tables and columns are relevant to the question. 
-            Use only after data is present and loaded. Prefer to request small independent steps with this tool.
-            """,)
-        )
-    ]
+    tools = []
+    # Tool(
+    #     name="Python",
+    #     func=python_chain.run,
+    #     description="Useful for when you need to run a quick simulation, or answer questions about math"
+    # ),
+
+    if database_engine is not None:
+        tools.extend([
+            Tool(
+                name="Show Tables",
+                func=lambda _: run_sql_catch_error(database_engine, "show tables"),
+                description="Useful to show the locally available database tables and views. Empty input required."
+            ),
+            Tool(
+                name="Describe Table",
+                func=lambda table: describe_table_or_view(database_engine, table),
+                description="Useful to show the column names and types of a local database table or view. Use the table name as the input."
+            ),
+            Tool(
+                name="Data Op",
+                func=lambda query: db_chain({
+                    'table_names': run_sql_catch_error(database_engine, "select table_name, table_schema from information_schema.tables;"),
+                    'input': query
+                }),
+                description=textwrap.dedent("""Useful to interact with local data tables. 
+                Input should be a natural language question containing full context including what tables and columns are relevant to the question. 
+                Use only after data is present and loaded. Prefer to request small independent steps with this tool.
+                """,)
+            )
+        ])
 
     if allow_human_clarification:
         tools.append(HumanInputRun())
 
     if allow_wikidata:
         tools.append(WikiDataQueryTool())
```

### Comparing `qabot-0.3.2/qabot/agents/data_query_chain.py` & `qabot-0.3.3/qabot/agents/data_query_chain.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/caching.py` & `qabot-0.3.3/qabot/caching.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/cli.py` & `qabot-0.3.3/qabot/cli.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/duckdb_manual_data_loader.py` & `qabot-0.3.3/qabot/duckdb_manual_data_loader.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/duckdb_query.py` & `qabot-0.3.3/qabot/duckdb_query.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/progress_callback.py` & `qabot-0.3.3/qabot/progress_callback.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/tools/describe_duckdb_table.py` & `qabot-0.3.3/qabot/tools/describe_duckdb_table.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/tools/duckdb_execute_tool.py` & `qabot-0.3.3/qabot/tools/duckdb_execute_tool.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/qabot/tools/wikidata.py` & `qabot-0.3.3/qabot/tools/wikidata.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.2/PKG-INFO` & `qabot-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qabot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Query local or remote data files with natural language queries powered by OpenAI and DuckDB.
 License: Apache-2.0
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

