# Comparing `tmp/qabot-0.3.0.tar.gz` & `tmp/qabot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qabot-0.3.0.tar", max compression
+gzip compressed data, was "qabot-0.3.1.tar", max compression
```

## Comparing `qabot-0.3.0.tar` & `qabot-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-03-27 21:19:57.134744 qabot-0.3.0/LICENSE
--rw-r--r--   0        0        0     5180 2023-04-12 01:17:42.230263 qabot-0.3.0/README.md
--rw-r--r--   0        0        0      711 2023-04-12 01:18:31.794151 qabot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      709 2023-04-12 01:11:09.111570 qabot-0.3.0/qabot/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.3.0/qabot/agents/__init__.py
--rw-r--r--   0        0        0     4277 2023-04-12 01:18:08.098203 qabot-0.3.0/qabot/agents/agent.py
--rw-r--r--   0        0        0    10550 2023-04-12 00:23:23.064560 qabot-0.3.0/qabot/agents/data_query_chain.py
--rw-r--r--   0        0        0     1707 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/caching.py
--rw-r--r--   0        0        0     6390 2023-04-12 01:01:50.420024 qabot-0.3.0/qabot/cli.py
--rw-r--r--   0        0        0      339 2023-04-11 22:48:01.992987 qabot-0.3.0/qabot/config.py
--rw-r--r--   0        0        0     3378 2023-03-27 21:34:35.864207 qabot-0.3.0/qabot/duckdb_manual_data_loader.py
--rw-r--r--   0        0        0     1259 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/duckdb_query.py
--rw-r--r--   0        0        0     2555 2023-04-12 00:25:15.975882 qabot-0.3.0/qabot/progress_callback.py
--rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.3.0/qabot/tools/__init__.py
--rw-r--r--   0        0        0      518 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/tools/describe_duckdb_table.py
--rw-r--r--   0        0        0     1027 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/tools/duckdb_execute_tool.py
--rw-r--r--   0        0        0     2681 2023-04-11 22:19:46.181702 qabot-0.3.0/qabot/tools/wikidata.py
--rw-r--r--   0        0        0     5931 1970-01-01 00:00:00.000000 qabot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-27 21:19:57.134744 qabot-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5180 2023-04-12 01:17:42.230263 qabot-0.3.1/README.md
+-rw-r--r--   0        0        0      711 2023-04-12 02:13:50.553282 qabot-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-04-12 01:11:09.111570 qabot-0.3.1/qabot/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.3.1/qabot/agents/__init__.py
+-rw-r--r--   0        0        0     4365 2023-04-12 02:05:45.393093 qabot-0.3.1/qabot/agents/agent.py
+-rw-r--r--   0        0        0    10860 2023-04-12 02:00:21.625211 qabot-0.3.1/qabot/agents/data_query_chain.py
+-rw-r--r--   0        0        0     1707 2023-03-27 21:19:57.138745 qabot-0.3.1/qabot/caching.py
+-rw-r--r--   0        0        0     6471 2023-04-12 02:06:49.481090 qabot-0.3.1/qabot/cli.py
+-rw-r--r--   0        0        0      390 2023-04-12 02:06:49.469090 qabot-0.3.1/qabot/config.py
+-rw-r--r--   0        0        0     3378 2023-03-27 21:34:35.864207 qabot-0.3.1/qabot/duckdb_manual_data_loader.py
+-rw-r--r--   0        0        0     1259 2023-03-27 21:19:57.138745 qabot-0.3.1/qabot/duckdb_query.py
+-rw-r--r--   0        0        0     2555 2023-04-12 00:25:15.975882 qabot-0.3.1/qabot/progress_callback.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.3.1/qabot/tools/__init__.py
+-rw-r--r--   0        0        0      518 2023-03-27 21:19:57.138745 qabot-0.3.1/qabot/tools/describe_duckdb_table.py
+-rw-r--r--   0        0        0     1027 2023-03-27 21:19:57.138745 qabot-0.3.1/qabot/tools/duckdb_execute_tool.py
+-rw-r--r--   0        0        0     2681 2023-04-11 22:19:46.181702 qabot-0.3.1/qabot/tools/wikidata.py
+-rw-r--r--   0        0        0     5931 1970-01-01 00:00:00.000000 qabot-0.3.1/PKG-INFO
```

### Comparing `qabot-0.3.0/LICENSE` & `qabot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/README.md` & `qabot-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/pyproject.toml` & `qabot-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qabot"
-version = "0.3.0"
+version = "0.3.1"
 license = "Apache-2.0"
 description = "Query local or remote data files with natural language queries powered by OpenAI and DuckDB."
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "qabot"}]
 
 [tool.poetry.scripts]
```

### Comparing `qabot-0.3.0/qabot/__init__.py` & `qabot-0.3.1/qabot/__init__.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/qabot/agents/agent.py` & `qabot-0.3.1/qabot/agents/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 def create_agent_executor(
         database_engine=None,
         return_intermediate_steps=False,
         callback_manager=None,
         verbose=False,
         model_name='gpt-3.5-turbo',
+        allow_human_clarification=False,
         allow_wikidata=True,
 ):
 
 
     llm = ChatOpenAI(
         model_name=model_name,
         temperature=0.0
@@ -61,18 +62,20 @@
                 'table_names': run_sql_catch_error(database_engine, "select table_name, table_schema from information_schema.tables;"),
                 'input': query
             }),
             description=textwrap.dedent("""Useful to interact with local data tables. 
             Input should be a natural language question containing full context including what tables and columns are relevant to the question. 
             Use only after data is present and loaded. Prefer to request small independent steps with this tool.
             """,)
-        ),
-        HumanInputRun(),
+        )
     ]
 
+    if allow_human_clarification:
+        tools.append(HumanInputRun())
+
     if allow_wikidata:
         tools.append(WikiDataQueryTool())
 
     memory = ConversationBufferMemory(memory_key="chat_history", output_key="output", return_messages=True)
 
     agent = initialize_agent(
         tools,
```

### Comparing `qabot-0.3.0/qabot/agents/data_query_chain.py` & `qabot-0.3.1/qabot/agents/data_query_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,36 +121,39 @@
 Begin! 
 
 Question: {input}
 {agent_scratchpad}
 """
 
 output_instructions = """
-Your output should be a single valid JSON object with the following keys:
+Your output must be a valid JSON object with the following keys:
 
-
-"type": the type of action to take, should be one of [{tool_names}] or "answer"
+{
+"type": the type of action to take, should be one of [{tool_names}] or "answer".
 "rational": Always think about what to do. Include your plan here.
 "input": The input to the action. Not required when type="answer".
-"result": The result of the action. Only allowed when type="answer". Should be an object with "output" and "query" keys. 
+"result": The final answer to the question when type="answer". Only allowed when type="answer". Should be an object with "output" and "query" keys. 
   The "output" should be a string with the Answer to the initial question. Markdown is supported. "query" should be a single string containing the SQL query used to obtain the answer.
+}
 
+Output 3 new lines after the JSON object.
 
-Output a double newline after your JSON object. The output of the action will be provided.
+Remember you must execute a query before providing an answer. The output of previous actions will be provided to you, only "answer" after querying the data.
 """
 
 
 class CustomOutputParser(AgentOutputParser):
     def get_format_instructions(self) -> str:
         return output_instructions
 
     def parse(self, llm_output: str) -> Union[AgentAction, AgentFinish]:
         try:
             data = CustomLLMResponse.parse_raw(llm_output)
         except pydantic.ValidationError as e:
+            print("format error", e)
             raise OutputParserException from e
 
         # Check if agent should finish
         if data.type == 'answer':
             if data.result and data.result.query:
                 queries = 'SQL Used:\n' + data.result.query
             else:
@@ -199,27 +202,29 @@
     # The list of tools available
     tools: List[BaseTool]
 
     def format_messages(self, **kwargs):
         # Get the intermediate steps (AgentAction, Observation tuples)
         # Format them in a particular way
         intermediate_steps = kwargs.pop("intermediate_steps")
-        thoughts = ""
+        if len(intermediate_steps) == 0:
+            thoughts = "Thought: I should execute a query before giving my answer\n"
+        else:
+            thoughts = ""
         for action, observation in intermediate_steps:
             thoughts += action.log
             thoughts += f"\nObservation: {observation}\nThought: "
 
         # Set the agent_scratchpad variable to that value
         kwargs["agent_scratchpad"] = thoughts
         # Create a tools variable from the list of tools provided
         kwargs["tools"] = "\n".join([f'"{tool.name}": {tool.description}' for tool in self.tools])
         # Create a list of tool names for the tools provided
         kwargs["tool_names"] = ", ".join([tool.name for tool in self.tools])
 
-
         kwargs['output_instructions'] = output_instructions
 
         # TODO probably good to get the updated table names here
         # table_names =
         formatted = self.template.format(**kwargs)
         return [
             HumanMessage(content=formatted)
```

### Comparing `qabot-0.3.0/qabot/caching.py` & `qabot-0.3.1/qabot/caching.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/qabot/cli.py` & `qabot-0.3.1/qabot/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,15 @@
             #database_uri=database_uri or settings.QABOT_DATABASE_URI,
             database_engine=database_engine,
             return_intermediate_steps=True,
             callback_manager=callback_manager,
             verbose=False,
             model_name=settings.QABOT_MODEL_NAME,
             allow_wikidata=settings.QABOT_ENABLE_WIKIDATA and enable_wikidata,
+            allow_human_clarification=settings.QABOT_ENABLE_HUMAN_CLARIFICATION,
         )
 
         progress.remove_task(t2)
         chat_history = [f"""
         Startup SQL Queries:
         ```
         {executed_sql}
```

### Comparing `qabot-0.3.0/qabot/duckdb_manual_data_loader.py` & `qabot-0.3.1/qabot/duckdb_manual_data_loader.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/qabot/duckdb_query.py` & `qabot-0.3.1/qabot/duckdb_query.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/qabot/progress_callback.py` & `qabot-0.3.1/qabot/progress_callback.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/qabot/tools/describe_duckdb_table.py` & `qabot-0.3.1/qabot/tools/describe_duckdb_table.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/qabot/tools/duckdb_execute_tool.py` & `qabot-0.3.1/qabot/tools/duckdb_execute_tool.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/qabot/tools/wikidata.py` & `qabot-0.3.1/qabot/tools/wikidata.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.0/PKG-INFO` & `qabot-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qabot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Query local or remote data files with natural language queries powered by OpenAI and DuckDB.
 License: Apache-2.0
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

