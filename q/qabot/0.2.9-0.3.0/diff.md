# Comparing `tmp/qabot-0.2.9.tar.gz` & `tmp/qabot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qabot-0.2.9.tar", max compression
+gzip compressed data, was "qabot-0.3.0.tar", max compression
```

## Comparing `qabot-0.2.9.tar` & `qabot-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    14540 2023-03-13 20:01:29.946508 qabot-0.2.9/README.md
--rw-r--r--   0        0        0      704 2023-03-23 03:07:56.965436 qabot-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-06 20:20:33.898706 qabot-0.2.9/qabot/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.2.9/qabot/agents/__init__.py
--rw-r--r--   0        0        0     4193 2023-03-23 03:05:22.962023 qabot-0.2.9/qabot/agents/agent.py
--rw-r--r--   0        0        0     5538 2023-03-13 21:00:38.828675 qabot-0.2.9/qabot/agents/data_query_chain.py
--rw-r--r--   0        0        0      744 2023-03-06 20:20:33.902705 qabot-0.2.9/qabot/caching.py
--rw-r--r--   0        0        0     6327 2023-03-13 20:31:56.276804 qabot-0.2.9/qabot/cli.py
--rw-r--r--   0        0        0      261 2023-03-06 20:20:33.902705 qabot-0.2.9/qabot/config.py
--rw-r--r--   0        0        0      920 2023-03-08 21:48:52.946092 qabot-0.2.9/qabot/duckdb_documentation.py
--rw-r--r--   0        0        0     2636 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/duckdb_manual_data_loader.py
--rw-r--r--   0        0        0     1259 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/duckdb_query.py
--rw-r--r--   0        0        0     2541 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/progress_callback.py
--rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.2.9/qabot/tools/__init__.py
--rw-r--r--   0        0        0      518 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/tools/describe_duckdb_table.py
--rw-r--r--   0        0        0     1028 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/tools/duckdb_execute_tool.py
--rw-r--r--   0        0        0    15223 1970-01-01 00:00:00.000000 qabot-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-27 21:19:57.134744 qabot-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5180 2023-04-12 01:17:42.230263 qabot-0.3.0/README.md
+-rw-r--r--   0        0        0      711 2023-04-12 01:18:31.794151 qabot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-04-12 01:11:09.111570 qabot-0.3.0/qabot/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.3.0/qabot/agents/__init__.py
+-rw-r--r--   0        0        0     4277 2023-04-12 01:18:08.098203 qabot-0.3.0/qabot/agents/agent.py
+-rw-r--r--   0        0        0    10550 2023-04-12 00:23:23.064560 qabot-0.3.0/qabot/agents/data_query_chain.py
+-rw-r--r--   0        0        0     1707 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/caching.py
+-rw-r--r--   0        0        0     6390 2023-04-12 01:01:50.420024 qabot-0.3.0/qabot/cli.py
+-rw-r--r--   0        0        0      339 2023-04-11 22:48:01.992987 qabot-0.3.0/qabot/config.py
+-rw-r--r--   0        0        0     3378 2023-03-27 21:34:35.864207 qabot-0.3.0/qabot/duckdb_manual_data_loader.py
+-rw-r--r--   0        0        0     1259 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/duckdb_query.py
+-rw-r--r--   0        0        0     2555 2023-04-12 00:25:15.975882 qabot-0.3.0/qabot/progress_callback.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.3.0/qabot/tools/__init__.py
+-rw-r--r--   0        0        0      518 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/tools/describe_duckdb_table.py
+-rw-r--r--   0        0        0     1027 2023-03-27 21:19:57.138745 qabot-0.3.0/qabot/tools/duckdb_execute_tool.py
+-rw-r--r--   0        0        0     2681 2023-04-11 22:19:46.181702 qabot-0.3.0/qabot/tools/wikidata.py
+-rw-r--r--   0        0        0     5931 1970-01-01 00:00:00.000000 qabot-0.3.0/PKG-INFO
```

### Comparing `qabot-0.2.9/qabot/agents/agent.py` & `qabot-0.3.0/qabot/agents/agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,114 +1,116 @@
 import textwrap
 
 from langchain import LLMMathChain
 from langchain.agents import Tool, initialize_agent
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import OpenAIChat
 from langchain.memory import ConversationBufferMemory
+from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
+from langchain.output_parsers import PydanticOutputParser
+from langchain.tools.human.tool import HumanInputRun
 
 from qabot.agents.data_query_chain import get_duckdb_data_query_chain
 from qabot.duckdb_query import run_sql_catch_error
 from qabot.tools.describe_duckdb_table import describe_table_or_view
+from qabot.tools.wikidata import WikiDataQueryTool
 
 
 def create_agent_executor(
         database_engine=None,
-        tables=None,
         return_intermediate_steps=False,
         callback_manager=None,
         verbose=False,
-        model_name='gpt-3.5-turbo'
+        model_name='gpt-3.5-turbo',
+        allow_wikidata=True,
 ):
 
-    llm = OpenAIChat(
+
+    llm = ChatOpenAI(
         model_name=model_name,
         temperature=0.0
     )
 
-    # llm = ChatOpenAI(
-    #     model_name="gpt-3.5-turbo",
-    #     temperature=0.0
-    # )
-
-    python_chain = LLMMathChain(llm=llm, verbose=False)
+    #python_chain = LLMMathChain(llm=llm, verbose=False)
 
     db_chain = get_duckdb_data_query_chain(
         llm=llm,
         database=database_engine,
         callback_manager=callback_manager,
         verbose=verbose
     )
 
     tools = [
-        Tool(
-            name="Python",
-            func=python_chain.run,
-            description="Useful for when you need to run a quick simulation, or answer questions about math"
-        ),
         # Tool(
-        #     name="DuckDB QA System",
-        #     func=duckdb_docs_qa_chain.run,
-        #     description="useful for when you need to answer questions about duckdb. Input should be a fully formed question."
+        #     name="Python",
+        #     func=python_chain.run,
+        #     description="Useful for when you need to run a quick simulation, or answer questions about math"
         # ),
         Tool(
             name="Show Tables",
             func=lambda _: run_sql_catch_error(database_engine, "show tables"),
-            description="Useful to show the available tables and views. Empty input required."
+            description="Useful to show the locally available database tables and views. Empty input required."
         ),
         Tool(
             name="Describe Table",
             func=lambda table: describe_table_or_view(database_engine, table),
-            description="Useful to show the column names and types of a table or view. Use the table name as the input."
+            description="Useful to show the column names and types of a local database table or view. Use the table name as the input."
         ),
         Tool(
             name="Data Op",
-            func=lambda input: db_chain({
-                'table_names': run_sql_catch_error(database_engine, "show tables;"),
-                'input': input}
-            ),
-            description=textwrap.dedent("""Useful for when you need to operate on data and answer individual questions
-            requiring data. Input should be in the form of a natural language question containing full context
-            including what tables and columns are relevant to the question. Use only after data is present and loaded.
-            Prefer to take small independent steps with this tool.
+            func=lambda query: db_chain({
+                'table_names': run_sql_catch_error(database_engine, "select table_name, table_schema from information_schema.tables;"),
+                'input': query
+            }),
+            description=textwrap.dedent("""Useful to interact with local data tables. 
+            Input should be a natural language question containing full context including what tables and columns are relevant to the question. 
+            Use only after data is present and loaded. Prefer to request small independent steps with this tool.
             """,)
-        )
+        ),
+        HumanInputRun(),
     ]
 
+    if allow_wikidata:
+        tools.append(WikiDataQueryTool())
+
     memory = ConversationBufferMemory(memory_key="chat_history", output_key="output", return_messages=True)
 
     agent = initialize_agent(
         tools,
         llm,
         agent="chat-conversational-react-description",
         callback_manager=callback_manager,
         return_intermediate_steps=return_intermediate_steps,
         verbose=verbose,
         agent_kwargs={
             #"input_variables": ["input", 'agent_scratchpad', 'chat_history'],
             "prefix": prompt_prefix_template
+            #"prompt": prompt
         },
         memory=memory
     )
     return agent
 
 
-prompt_prefix_template = """Qabot is a large language model trained to interact with DuckDB.
+prompt_prefix_template = """You are Qabot, a large language model trained to interact with DuckDB.
 
-Qabot is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explorations on a wide range of topics relating to data.
+Qabot is designed to be able to assist with a wide range of tasks, from answering simple questions to 
+providing in-depth explorations on a wide range of topics relating to data.
 
-Qabot answers questions by first querying for data to guide its answer. Qabot asks any clarifying questions it needs to.
+Qabot answers questions by first querying for data to guide its answer. Qabot responds with clarifying
+questions if the request isn't clear. Qabot first tries to use local tables before
+querying wikidata.
 
-Qabot refuses to delete any data, or drop tables. 
-
-Qabot prefers to split questions into small discrete steps, for example creating views of data as one action, then selecting data from the created view to get to the final answer.
+Qabot prefers to split questions into small discrete steps, creating views of data as one action, then
+selecting data from the created view to get to the final answer.
 
 Qabot includes a list of all important SQL queries returned by Data Op in its final answers.
 
 Qabot does NOT make any DML statements (INSERT, UPDATE, DELETE, DROP etc.) to the database.
 
 If the question does not seem related to the database, Qabot returns "I don't know" as the answer.
+
 TOOLS:
 ------
 
 Qabot has access to the following tools:
 """
```

### Comparing `qabot-0.2.9/qabot/cli.py` & `qabot-0.3.0/qabot/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
 
 @app.command()
 def main(
         query: str = typer.Option("Describe the tables", '-q', '--query', prompt=INITIAL_NON_INTERACTIVE_PROMPT),
         file: Optional[List[str]] = typer.Option(None, "-f", "--file", help="File or url containing data to query"),
         database_uri: Optional[str] = typer.Option(":memory:", "-d", "--database", help="DuckDB Database URI (e.g. '/tmp/qabot.duckdb')"),
-        table: Optional[List[str]] = typer.Option(None, "--table", "-t", help="Limit queries to these tables (can be specified multiple times)"),
-        disable_cache: bool = typer.Option(False, "--disable-cache", help="Disable caching of LLM queries"),
+        disable_cache: bool = typer.Option(True, "--disable-cache", help="Disable caching of LLM queries"),
+        enable_wikidata: bool = typer.Option(False, "-w", "--wikidata", help='Allow querying from wikidata'),
         verbose: bool = typer.Option(False, "-v", "--verbose", help='Essentially debug output'),
 ):
     """
     Query a database using a simple english query.
 
     Example:
         qabot -q "What is the average age of the people in the table?"
@@ -111,29 +111,29 @@
         output_callback = QACallback(progress=progress)
         openai_callback = OpenAICallbackHandler()
         callback_manager = get_callback_manager()
 
         callback_manager.add_handler(openai_callback)
         callback_manager.add_handler(output_callback)
 
-
         if not disable_cache:
             t = progress.add_task(description="Setting up cache...", total=None)
-            configure_caching(settings.QABOT_CACHE_DATABASE_URI)
+            configure_caching(database_engine)
             progress.remove_task(t)
 
         t2 = progress.add_task(description="Creating LLM agent using langchain...", total=None)
 
         agent = create_agent_executor(
             #database_uri=database_uri or settings.QABOT_DATABASE_URI,
             database_engine=database_engine,
-            tables=table,
             return_intermediate_steps=True,
             callback_manager=callback_manager,
             verbose=False,
+            model_name=settings.QABOT_MODEL_NAME,
+            allow_wikidata=settings.QABOT_ENABLE_WIKIDATA and enable_wikidata,
         )
 
         progress.remove_task(t2)
         chat_history = [f"""
         Startup SQL Queries:
         ```
         {executed_sql}
@@ -158,27 +158,28 @@
             if verbose:
                 progress.console.print("[bold red]Intermediate Steps: [/]")
                 for i, (agent_action, action_input) in enumerate(result['intermediate_steps'], 1):
                     print(f"  [bold red]Step {i}[/]")
                     print(textwrap.indent(format_agent_action(agent_action, action_input), "    "))
 
                 print()
-            print("Total tokens", output_callback.total_tokens, f"approximate cost ${output_callback.total_tokens * 0.002/1000}")
+
+            print("Total tokens", output_callback.total_tokens, f"approximate cost in USD: {openai_callback.total_cost}")
 
             # Stop the progress before outputting result and prompting for input
             progress.stop()
             print()
 
             print("[bold red]Result:[/]\n[bold blue]" + result['output'] + "\n")
             chat_history.append(result['output'])
 
             print()
             query = Prompt.ask(FOLLOW_UP_PROMPT)
 
-            if query == "exit" and Confirm.ask("Are you sure you want to Quit?"):
+            if query.lower() in {'q', 'exit', 'quit'} and Confirm.ask("Are you sure you want to Quit?"):
                 break
 
             progress.start()
 
 
 def run():
     app()
```

### Comparing `qabot-0.2.9/qabot/duckdb_manual_data_loader.py` & `qabot-0.3.0/qabot/duckdb_manual_data_loader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 from typing import Tuple
 from urllib.parse import urlparse
+import tempfile
+
 import duckdb
 from duckdb import ParserException, ProgrammingError
+import requests
 
 
 def uri_validator(x):
     try:
         result = urlparse(x)
         return all([result.scheme, result.netloc])
     except:
@@ -62,15 +65,30 @@
 
     try:
         conn.sql(f"create table t_{table_name} as select 1;")
         conn.sql(f"drop table t_{table_name};")
     except (ParserException, ProgrammingError) as e:
         table_name = "data"
 
-    # The SQLAgent doesn't appear to see view's just yet, so we'll create a table instead
+    # try to create a view then fallback to a table if it fails
     use_view = allow_view and is_url
+    try:
+        create_statement = f"create {'view' if use_view else 'table'} '{table_name}' as select * from '{file_path}';"
+        conn.sql(create_statement)
+    except duckdb.IOException as e:
+        # This can occur if the server doesn't send Content-Length headers
+        # We can work around this by downloading the data locally and then
+        # loading it from there. We assume CSV files for now
+        if is_url:
+
+            with tempfile.NamedTemporaryFile(mode='w+b', suffix='.csv', delete=False) as f:
+                r = requests.get(file_path, stream=True)
+                for chunk in r.iter_content(chunk_size=1024):
+                    if chunk:
+                        f.write(chunk)
+                f.flush()
 
-    create_statement = f"create {'view' if use_view else 'table'} '{table_name}' as select * from '{file_path}';"
+                create_statement = f"create table '{table_name}' as select * from read_csv_auto('{f.name}');"
 
-    conn.sql(create_statement)
+        conn.sql(create_statement)
 
     return create_statement
```

### Comparing `qabot-0.2.9/qabot/duckdb_query.py` & `qabot-0.3.0/qabot/duckdb_query.py`

 * *Files identical despite different names*

### Comparing `qabot-0.2.9/qabot/progress_callback.py` & `qabot-0.3.0/qabot/progress_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     #         self.progress.remove_task(self.tool_task_id)
     #         self.tool_task_id = None
 
     def on_agent_action(
         self, action: AgentAction, color: Optional[str] = None, **kwargs
     ):
         """Run on agent requesting an action."""
-        print(f"[{color}]{action.log}[/{color}]")
+        pass
+        #print(f"[{color}]{action.log}[/{color}]")
 
     def on_chain_end(self, outputs, **kwargs):
         super().on_chain_end(outputs, **kwargs)
         if isinstance(outputs, dict) and 'text' in outputs:
             outputs = outputs['text']
             #print(f"[cyan]{outputs}")
```

### Comparing `qabot-0.2.9/qabot/tools/describe_duckdb_table.py` & `qabot-0.3.0/qabot/tools/describe_duckdb_table.py`

 * *Files identical despite different names*

### Comparing `qabot-0.2.9/qabot/tools/duckdb_execute_tool.py` & `qabot-0.3.0/qabot/tools/duckdb_execute_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,12 +23,11 @@
     def _run(self, query: str) -> str:
         #
         query_result = run_sql_catch_error(self.database, query)
         print(f"[pink]{query_result}[/pink]")
         time.sleep(0.2)
         return query_result
 
-
     async def _arun(self, query: str) -> str:
         raise NotImplementedError("DuckDBTool does not support async")
```

