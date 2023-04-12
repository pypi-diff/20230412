# Comparing `tmp/zillion-0.9.5.tar.gz` & `tmp/zillion-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillion-0.9.5.tar", last modified: Mon Apr 10 14:09:45 2023, max compression
+gzip compressed data, was "zillion-0.9.6.tar", last modified: Wed Apr 12 01:58:38 2023, max compression
```

## Comparing `zillion-0.9.5.tar` & `zillion-0.9.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.5/AUTHORS.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.5/LICENSE
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 14:09:45.094051 zillion-0.9.5/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-04 15:42:18.000000 zillion-0.9.5/README.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-10 14:09:45.094051 zillion-0.9.5/setup.cfg
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2859 2023-03-31 00:50:17.000000 zillion-0.9.5/setup.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.5/zillion/configs.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.5/zillion/core.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    69368 2023-04-10 14:08:30.000000 zillion-0.9.5/zillion/datasource.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion/dialects/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.5/zillion/dialects/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/conversions.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.5/zillion/dialects/duckdb.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/mysql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/postgresql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/sqlite.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-03-23 18:23:26.000000 zillion-0.9.5/zillion/field.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.5/zillion/model.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    36392 2023-04-04 15:47:25.000000 zillion-0.9.5/zillion/nlp.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    83878 2023-04-03 17:49:18.000000 zillion-0.9.5/zillion/report.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion/scripts/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/scripts/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.5/zillion/scripts/bootstrap_datasource_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/scripts/json_to_yaml.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1241 2023-04-10 13:55:59.000000 zillion-0.9.5/zillion/scripts/load_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2478 2023-04-04 11:18:20.000000 zillion-0.9.5/zillion/scripts/run_report.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/scripts/yaml_to_json.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.5/zillion/sql_utils.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-10 14:09:06.000000 zillion-0.9.5/zillion/version.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-04 01:10:26.000000 zillion-0.9.5/zillion/warehouse.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion.egg-info/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      768 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/SOURCES.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/dependency_links.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1050 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/requires.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/top_level.txt
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 01:58:38.706548 zillion-0.9.6/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.6/AUTHORS.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.6/LICENSE
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 01:58:38.706548 zillion-0.9.6/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-12 01:58:16.000000 zillion-0.9.6/README.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-12 01:58:38.706548 zillion-0.9.6/setup.cfg
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2885 2023-04-12 01:54:36.000000 zillion-0.9.6/setup.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 01:58:38.706548 zillion-0.9.6/zillion/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.6/zillion/configs.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.6/zillion/core.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    69368 2023-04-10 14:08:30.000000 zillion-0.9.6/zillion/datasource.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 01:58:38.706548 zillion-0.9.6/zillion/dialects/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.6/zillion/dialects/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/dialects/conversions.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.6/zillion/dialects/duckdb.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/dialects/mysql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/dialects/postgresql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/dialects/sqlite.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-03-23 18:23:26.000000 zillion-0.9.6/zillion/field.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.6/zillion/model.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    37273 2023-04-12 01:50:57.000000 zillion-0.9.6/zillion/nlp.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    84221 2023-04-12 01:19:40.000000 zillion-0.9.6/zillion/report.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 01:58:38.706548 zillion-0.9.6/zillion/scripts/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/scripts/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.6/zillion/scripts/bootstrap_datasource_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/scripts/json_to_yaml.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1241 2023-04-10 13:55:59.000000 zillion-0.9.6/zillion/scripts/load_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2478 2023-04-04 11:18:20.000000 zillion-0.9.6/zillion/scripts/run_report.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.6/zillion/scripts/yaml_to_json.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.6/zillion/sql_utils.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-12 01:52:09.000000 zillion-0.9.6/zillion/version.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-04 01:10:26.000000 zillion-0.9.6/zillion/warehouse.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 01:58:38.706548 zillion-0.9.6/zillion.egg-info/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 01:58:38.000000 zillion-0.9.6/zillion.egg-info/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      768 2023-04-12 01:58:38.000000 zillion-0.9.6/zillion.egg-info/SOURCES.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-12 01:58:38.000000 zillion-0.9.6/zillion.egg-info/dependency_links.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1080 2023-04-12 01:58:38.000000 zillion-0.9.6/zillion.egg-info/requires.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-12 01:58:38.000000 zillion-0.9.6/zillion.egg-info/top_level.txt
```

### Comparing `zillion-0.9.5/LICENSE` & `zillion-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/PKG-INFO` & `zillion-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.5
+Version: 0.9.6
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.5/README.md` & `zillion-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/setup.py` & `zillion-0.9.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     "duckdb": [
         "duckdb~=0.7.1",
         "duckdb-engine~=0.7.0",
     ],
     "nlp": [
         "langchain==0.0.115",
         "openai==0.27.2",
-        "qdrant-client==0.11.0",
+        "tiktoken==0.3.3",
+        "qdrant-client==1.1.3",
     ],
     "dev": [
         "black",
         "pre-commit",
         "pylint==2.4.4",
         "pytest==7.1.2",
         "pytest-xdist==3.1.0",
```

### Comparing `zillion-0.9.5/zillion/configs.py` & `zillion-0.9.6/zillion/configs.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/core.py` & `zillion-0.9.6/zillion/core.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/datasource.py` & `zillion-0.9.6/zillion/datasource.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/dialects/conversions.py` & `zillion-0.9.6/zillion/dialects/conversions.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/dialects/duckdb.py` & `zillion-0.9.6/zillion/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/dialects/mysql.py` & `zillion-0.9.6/zillion/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/dialects/postgresql.py` & `zillion-0.9.6/zillion/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/dialects/sqlite.py` & `zillion-0.9.6/zillion/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/field.py` & `zillion-0.9.6/zillion/field.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/model.py` & `zillion-0.9.6/zillion/model.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/nlp.py` & `zillion-0.9.6/zillion/nlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from sqlalchemy import and_
 from sqlalchemy.schema import CreateTable
 from tlbx import raiseifnot, st, json
 
 from zillion.core import (
     info,
     warn,
+    error,
     zillion_config,
     nlp_installed,
     RollupTypes,
     FieldTypes,
 )
 
 LLM_MAX_TOKENS = -1
@@ -326,16 +327,25 @@
             # We delay connecting to Qdrant until we need it. This way
             # we can init the API globally without Qdrant necessarily running.
             self.client = None
 
         def connect(self):
             """Connect to Qdrant"""
             host = zillion_config["QDRANT_HOST"]
-            info(f"Connecting to Qdrant at {host}...")
-            self.client = QdrantClient(host=host, port=6333, prefer_grpc=True)
+            info(f"Connecting to Qdrant host: {host}...")
+            if host == ":memory:":
+                self.client = QdrantClient(location=host)
+            elif host.startswith("http") or host in [
+                "localhost",
+                "127.0.0.1",
+                "host.docker.internal",
+            ]:
+                self.client = QdrantClient(host=host, port=6333, prefer_grpc=True)
+            else:
+                self.client = QdrantClient(path=host)
 
         def ensure_client(self):
             """Make sure we have a client. If not, connect to Qdrant."""
             if not self.client:
                 self.connect()
 
         def embed_documents(self, rows):
@@ -375,15 +385,15 @@
                 collection = self.get_collection(collection_name)
                 if collection:
                     info(
                         f"Collection {collection_name} already exists. Skipping creation."
                     )
                     return collection
             except Exception as e:
-                if "Not found" not in str(e):
+                if "not found" not in str(e).lower():
                     raise e
 
             info(f"Creating collection {collection_name}...")
             if sample and vector_size is None:
                 vector_size = len(self.embed_documents([sample])[0])
             elif vector_size is None:
                 vector_size = DEFAULT_VECTOR_SIZE
@@ -555,66 +565,116 @@
     embeddings_api.add_texts(
         collection_name=collection_name, texts=texts, metadatas=metadatas
     )
     info(f"Done in {time.time() - start:3f} seconds.")
     return collection_name
 
 
-def build_chain(
-    prompt, model=None, max_tokens=LLM_MAX_TOKENS, request_timeout=LLM_REQUEST_TIMEOUT
-):
-    """Build a chain using langchain and the OpenAI API.
+def get_openai_class(model=None):
+    """Get the OpenAI class to use for a given model."""
+    model = model or zillion_config["OPENAI_MODEL"]
+    return OpenAI if model == OPENAI_DAVINCI_MODEL_NAME else OpenAIChat
+
+
+def get_openai_model_context_size(model):
+    """Logic copied from langchain since no util exposed"""
+    if model == "text-davinci-003":
+        return 4097
+    elif model == "text-curie-001":
+        return 2048
+    elif model == "text-babbage-001":
+        return 2048
+    elif model == "text-ada-001":
+        return 2048
+    elif model == "code-davinci-002":
+        return 8000
+    elif model == "code-cushman-001":
+        return 2048
+    else:
+        return 4097
+
+
+def build_llm(model=None, max_tokens=None, request_timeout=LLM_REQUEST_TIMEOUT):
+    """Build an LLM using langchain and the OpenAI API.
 
     **Parameters:**
 
-    * **prompt** - (PromptTemplate) The prompt to use.
     * **model** - (str, optional) The OpenAI model to use. Defaults to the model specified in the zillion config.
     * **max_tokens** - (int) The maximum number of tokens to generate.
     * **request_timeout** - (int) The maximum number of seconds to wait for a response from the OpenAI API.
 
     **Returns:**
 
-    (*LLMChain*) - A langchain LLMChain object.
+    (*llm*) - A langchain OpenAI LLM
 
     """
     model = model or zillion_config["OPENAI_MODEL"]
     key = zillion_config["OPENAI_API_KEY"]
     raiseifnot(model and key, "Missing OpenAI API key or model name in zillion config")
     max_tokens = max_tokens or LLM_MAX_TOKENS
     info(f"Building OpenAI {model} chain with max_tokens={max_tokens}")
-    openai_class = OpenAI if model == OPENAI_DAVINCI_MODEL_NAME else OpenAIChat
-    llm = openai_class(
+    openai_class = get_openai_class(model)
+    return openai_class(
         model_name=model,
         temperature=0,
         max_tokens=max_tokens,
         request_timeout=request_timeout,
         max_retries=1,
         openai_api_key=key,
     )
+
+
+def build_chain(
+    prompt,
+    model=None,
+    max_tokens=LLM_MAX_TOKENS,
+    request_timeout=LLM_REQUEST_TIMEOUT,
+    llm=None,
+):
+    """Build a chain using langchain and the OpenAI API.
+
+    **Parameters:**
+
+    * **prompt** - (PromptTemplate) The prompt to use.
+    * **model** - (str, optional) The OpenAI model to use. Defaults to the model specified in the zillion config.
+    * **max_tokens** - (int) The maximum number of tokens to generate.
+    * **request_timeout** - (int) The maximum number of seconds to wait for a response from the OpenAI API.
+    * **llm** - (llm, optional) The LLM to use. Defaults to a new LLM built using the OpenAI API.
+
+    **Returns:**
+
+    (*LLMChain*) - A langchain LLMChain object.
+
+    """
+    llm = llm or build_llm(
+        model=model, max_tokens=max_tokens, request_timeout=request_timeout
+    )
     return LLMChain(llm=llm, prompt=prompt)
 
 
 TEXT_TO_REPORT_V1 = """You are an expert SQL analyst that takes natural language input and outputs metrics, dimensions, criteria, ordering, and limit settings in JSON format.
 If a relative date is specified, such as "yesterday", replace it with the actual date. The current date is: {current_date}
 
-Example inputs and outputs:
+Generic Example 1:
 
 Input: revenue and sales by date for the last 30 days. Rows with more than 5 sales.
 Output:
 {{
   "metrics": ["revenue", "sales"],
   "dimensions": ["date"],
   "criteria": [
     ["date", ">=", "{thirty_days_ago}"]
   ],
   "row_filters": [
     ["sales", ">", 5]
 ]
 }}
 
+Generic Example 2:
+
 Input: show me the top 10 campaigns by revenue yesterday for ad engine Google. Include totals.
 Output:
 {{
   "metrics": ["revenue"],
   "dimensions": ["campaign"],
   "criteria": [
     ["date", "=", "{yesterday}"],
@@ -624,124 +684,117 @@
   "order_by": [
     ["revenue", "desc"]
   ],
   "rollup": "totals"
 }}
 
 ----
+Complete the following. Use JSON format and include no other commentary.
 Input: {query}
 JSON Output:"""
 
-TEXT_TO_REPORT_V2 = """We are going to translate natural language queries into a reporting API call. The python function we will call has a signature and docstring as follows:
-
-```python
-def run_report(
-    metrics=None,
-    dimensions=None,
-    criteria=None,
-    row_filters=None,
-    rollup=None,
-    pivot=None,
-    order_by=None,
-    limit=None,
-):
-    * **metrics** - (*list, optional*) A list of metric names, or dicts in the
-    case of AdHocMetrics. These will be the measures of your report, or the
-    statistics you are interested in computing at the given dimension grain.
-    * **dimensions** - (*list, optional*) A list of dimension names to control
-    the grain of the report. You can think of dimensions similarly to the "group
-    by" in a SQL query.
-    * **criteria** - (*list, optional*) A list of criteria to be applied when
-    querying. Each criteria in the list is represented by a 3-item list or
-    tuple. See `core.CRITERIA_OPERATIONS` for all supported
-    operations. Note that some operations, such as "like", have varying
-    behavior by datasource dialect. Some examples:
-        * ["field_a", ">", 1]
-        * ["field_b", "=", "2020-04-01"]
-        * ["field_c", "like", "%example%"]
-        * ["field_d", "in", ["a", "b", "c"]]
-
-    * **row_filters** - (*list, optional*) A list of criteria to apply at the
-    final step (combined query layer) to filter which rows get returned. The
-    format here is the same as for the criteria arg, though the operations are
-    limited to the values of `core.ROW_FILTER_OPERATIONS`.
-    * **rollup** - (*str or int, optional*) Controls how metrics are rolled up
-    / aggregated by dimension depth. If not passed no rollup will be
-    computed. If the special value "totals" is passed, only a final tally
-    rollup row will be added. If an int, then it controls the maximum depth to
-    roll up the data, starting from the most granular (last) dimension of the
-    report. Note that the rollup=3 case is like adding a totals row to the
-    "=2" case, as a totals row is a rollup of all dimension levels. Setting
-    rollup=len(dims) is equivalent to rollup="all". For example, if you ran a
-    report with dimensions ["a", "b", "c"]:
-        * **rollup="totals"** - adds a single, final rollup row
-        * **rollup="all"** - rolls up all dimension levels
-        * **rollup=1** - rolls up the first dimension only
-        * **rollup=2** - rolls up the first two dimensions
-        * **rollup=3** - rolls up all three dimensions
-        * Any other non-None value would raise an error
-
-    * **pivot** - (*list, optional*) A list of dimensions to pivot to columns
-    * **order_by** - (*list, optional*) A list of (field, asc/desc) tuples that
-    control the ordering of the returned result
-    * **limit** - (*int, optional*) A limit on the number of rows returned
-```
 
+TEXT_TO_REPORT_V2 = """You are an expert SQL analyst that takes natural language input and outputs metrics, dimensions, criteria, ordering, and limit settings in JSON format.
 If a relative date is specified, such as "yesterday", replace it with the actual date. The current date is: {current_date}
 
-Query: {query}
-Python Arguments:"""
+Supported metrics:
+{metrics}
 
+Supported dimensions:
+{dimensions}
 
-TEXT_TO_REPORT_V3 = """We are going to translate natural language queries into a MySQL query. Assume all fields are in a single table called "mytable".
-If a relative date is specified, such as "yesterday", replace it with the actual date. The current date is: {current_date}
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
 
-Query: {query}
-SQL:"""
+----
+Complete the following. Use JSON format and include no other commentary. Use only supported metrics and dimensions.
+Input: {query}
+JSON Output:"""
 
 
-def parse_text_to_report_v1_output(output):
-    """Parse the output of the TEXT_TO_REPORT_V1 chain
+def parse_text_to_report_json_output(output):
+    """Parse the output of a chain that produces Zillion args as JSON
 
     **Parameters:**
 
     * **output** - (str) The output of the chain, expected to be valid JSON.
 
     **Returns:**
 
     (*dict*) - A dict of Zillion report params. Any empty values will be removed.
 
     """
     if not output:
         return None
-    return {k: v for k, v in json.loads(output).items() if v}
-
-
-def parse_text_to_report_v2_output(output):
-    """TODO Parse the output of the TEXT_TO_REPORT_V2 chain, which outputs python arguments"""
-    raise NotImplementedError
-
-
-def parse_text_to_report_v3_output(output):
-    """TODO Parse the output of the TEXT_TO_REPORT_V3 chain, would require sqlparse"""
-    raise NotImplementedError
+    try:
+        return {k: v for k, v in json.loads(output).items() if v}
+    except Exception as e:
+        error(f"Error parsing JSON:\n{output}")
+        raise
 
 
 PROMPT_CONFIGS = dict(
     v1=dict(
         prompt_text=TEXT_TO_REPORT_V1,
-        parser=parse_text_to_report_v1_output,
+        input_variables=["query", "current_date", "yesterday", "thirty_days_ago"],
+        context_func=lambda wh: dict(
+            current_date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            yesterday=str(datetime.now().date() - timedelta(days=1)),
+            thirty_days_ago=str(datetime.now().date() - timedelta(days=30)),
+        ),
+        parser=parse_text_to_report_json_output,
     ),
     v2=dict(
         prompt_text=TEXT_TO_REPORT_V2,
-        parser=parse_text_to_report_v2_output,
-    ),
-    v3=dict(
-        prompt_text=TEXT_TO_REPORT_V3,
-        parser=parse_text_to_report_v3_output,
+        input_variables=[
+            "query",
+            "current_date",
+            "yesterday",
+            "thirty_days_ago",
+            "metrics",
+            "dimensions",
+        ],
+        context_func=lambda wh: dict(
+            metrics=get_metrics_prompt_str(wh),
+            dimensions=get_dimensions_prompt_str(wh),
+            current_date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            yesterday=str(datetime.now().date() - timedelta(days=1)),
+            thirty_days_ago=str(datetime.now().date() - timedelta(days=30)),
+        ),
+        parser=parse_text_to_report_json_output,
     ),
 )
 
 
 def get_field_name_variants(name):
     """Get a list of possible close variants of a field name. This is
     an 80/20 hack to help with fuzzy matching of field names.
@@ -870,57 +923,73 @@
             raise ValueError(f"Unexpected key {k}")
     return res
 
 
 text_to_report_chain = None
 
 
-def text_to_report_params(query, prompt_version="v1"):
+def get_fields_prompt_str(fields):
+    """Get a string representing names/types of given fields"""
+    res = []
+    for name, fdef in fields.items():
+        type_str = str(fdef.type).lower() if fdef.type else "unknown"
+        res.append(f"{name} ({type_str})")
+    return "\n".join(res)
+
+
+def get_metrics_prompt_str(warehouse):
+    return get_fields_prompt_str(warehouse.get_metrics())
+
+
+def get_dimensions_prompt_str(warehouse):
+    return get_fields_prompt_str(warehouse.get_dimensions())
+
+
+class MaxTokensException(Exception):
+    pass
+
+
+def text_to_report_params(query, warehouse=None, prompt_version="v1"):
     """Convert a natural language input to Zillion report params
 
     **Parameters:**
 
     * **query** - (str) The natural language query to convert.
+    * **warehouse** - (Warehouse, optional) The warehouse to map the report params to
     * **prompt_version** - (str) The version of the prompt to use
 
     **Returns:**
 
     (*dict*) - A dict of Zillion report params. The field names extracted are
     not guaranteed to exist in any warehouse or datasource and need to be
     analyzed separately.
 
     """
     prompt_config = PROMPT_CONFIGS[prompt_version]
-    prompt_text = prompt_config["prompt_text"]
-    parser = prompt_config["parser"]
-
-    context = dict(
-        query=query,
-        current_date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-        yesterday=str(datetime.now().date() - timedelta(days=1)),
-        thirty_days_ago=str(datetime.now().date() - timedelta(days=30)),
+    context = prompt_config["context_func"](warehouse)
+    context["query"] = query
+    prompt = PromptTemplate(
+        input_variables=prompt_config["input_variables"],
+        template=prompt_config["prompt_text"],
     )
 
     global text_to_report_chain
     if not text_to_report_chain:
-        prompt = PromptTemplate(
-            input_variables=["query", "current_date", "yesterday", "thirty_days_ago"],
-            template=prompt_text,
-        )
-        text_to_report_chain = build_chain(
-            prompt,
-            model=OPENAI_DAVINCI_MODEL_NAME,
-            max_tokens=1000,
-            request_timeout=LLM_REQUEST_TIMEOUT,
-        )
+        llm = build_llm(max_tokens=-1)
+        text_to_report_chain = build_chain(prompt, llm=llm)
+
+    prompt_tokens = text_to_report_chain.llm.get_num_tokens(prompt.format(**context))
+    max_tokens = get_openai_model_context_size(text_to_report_chain.llm.model_name)
+    if (prompt_tokens + 500) >= max_tokens:
+        raise MaxTokensException(f"Prompt is too long: {prompt_tokens} tokens")
 
     llm_start = time.time()
     output = text_to_report_chain.run(**context).strip(". -\n\r")
     info(f"LLM took {time.time() - llm_start:.3f}s")
-    return parser(output)
+    return prompt_config["parser"](output)
 
 
 NLP_TABLE_RELATIONSHIP_PROMPT = """Given the following tables, what are the suggested foreign key relationships starting from these tables?
 Rules:
 - If there isn't a good option you must skip that table and output nothing.
 - Only include relationships between the tables given below. Do not reference any other tables not in the list.
 - Ignore self-referencing relationships (i.e. a table with a column that references itself)
```

### Comparing `zillion-0.9.5/zillion/report.py` & `zillion-0.9.6/zillion/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,19 @@
     FormulaDimension,
     get_table_fields,
     get_table_field_column,
     FormulaField,
     FIELD_VALUE_CHECK_OPERATIONS,
 )
 from zillion.model import zillion_engine, ReportSpecs
-from zillion.nlp import text_to_report_params, map_warehouse_report_params
+from zillion.nlp import (
+    text_to_report_params,
+    MaxTokensException,
+    map_warehouse_report_params,
+)
 from zillion.sql_utils import (
     sqla_compile,
     get_sqla_criterion_expr,
     to_sqlite_type,
     type_string_to_sa_type,
 )
 
@@ -2118,15 +2122,21 @@
         * **allow_partial** - (*bool, optional*) Allow partial report results
 
         **Returns:**
 
         * **report** - (*Report*) A report object
 
         """
-        params = text_to_report_params(text)
+        try:
+            # Try the V2 prompt first which includes metrics/dimensions
+            # in the prompt. If that fails, try the V1 prompt.
+            params = text_to_report_params(text, warehouse, prompt_version="v2")
+        except MaxTokensException as e:
+            params = text_to_report_params(text, warehouse, prompt_version="v1")
+
         report_params = map_warehouse_report_params(warehouse, params)
         return Report(
             warehouse,
             **report_params,
             adhoc_datasources=adhoc_datasources,
             allow_partial=allow_partial,
         )
```

### Comparing `zillion-0.9.5/zillion/scripts/bootstrap_datasource_config.py` & `zillion-0.9.6/zillion/scripts/bootstrap_datasource_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/scripts/load_config.py` & `zillion-0.9.6/zillion/scripts/load_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/scripts/run_report.py` & `zillion-0.9.6/zillion/scripts/run_report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/sql_utils.py` & `zillion-0.9.6/zillion/sql_utils.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion/warehouse.py` & `zillion-0.9.6/zillion/warehouse.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion.egg-info/PKG-INFO` & `zillion-0.9.6/zillion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.5
+Version: 0.9.6
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.5/zillion.egg-info/SOURCES.txt` & `zillion-0.9.6/zillion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zillion-0.9.5/zillion.egg-info/requires.txt` & `zillion-0.9.6/zillion.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 pre-commit
 psycopg2-binary==2.9.5
 psycopg2-binary~=2.9.5
 pylint==2.4.4
 pymysql~=1.0.2
 pytest-xdist==3.1.0
 pytest==7.1.2
-qdrant-client==0.11.0
+qdrant-client==1.1.3
+tiktoken==0.3.3
 twine==3.1.1
 wheel
 
 [dev]
 black
 pre-commit
 pylint==2.4.4
@@ -61,11 +62,12 @@
 
 [mysql]
 pymysql~=1.0.2
 
 [nlp]
 langchain==0.0.115
 openai==0.27.2
-qdrant-client==0.11.0
+tiktoken==0.3.3
+qdrant-client==1.1.3
 
 [postgres]
 psycopg2-binary~=2.9.5
```

