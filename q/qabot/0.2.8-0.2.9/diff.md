# Comparing `tmp/qabot-0.2.8.tar.gz` & `tmp/qabot-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qabot-0.2.8.tar", max compression
+gzip compressed data, was "qabot-0.2.9.tar", max compression
```

## Comparing `qabot-0.2.8.tar` & `qabot-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    14530 2023-03-11 22:06:36.492895 qabot-0.2.8/README.md
--rw-r--r--   0        0        0      704 2023-03-11 22:18:29.374233 qabot-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-03 03:50:46.340000 qabot-0.2.8/qabot/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 08:34:44.301055 qabot-0.2.8/qabot/agents/__init__.py
--rw-r--r--   0        0        0     4075 2023-03-11 21:03:00.369487 qabot-0.2.8/qabot/agents/agent.py
--rw-r--r--   0        0        0     5307 2023-03-11 21:37:43.043963 qabot-0.2.8/qabot/agents/data_query_chain.py
--rw-r--r--   0        0        0      744 2023-03-03 04:31:14.015696 qabot-0.2.8/qabot/caching.py
--rw-r--r--   0        0        0     6469 2023-03-11 22:06:12.263190 qabot-0.2.8/qabot/cli.py
--rw-r--r--   0        0        0      261 2023-03-03 23:22:20.398849 qabot-0.2.8/qabot/config.py
--rw-r--r--   0        0        0      920 2023-03-08 09:09:36.361169 qabot-0.2.8/qabot/duckdb_documentation.py
--rw-r--r--   0        0        0     2636 2023-03-11 22:14:15.783981 qabot-0.2.8/qabot/duckdb_manual_data_loader.py
--rw-r--r--   0        0        0     1252 2023-03-11 22:14:15.823980 qabot-0.2.8/qabot/duckdb_query.py
--rw-r--r--   0        0        0     2541 2023-03-11 22:00:26.767388 qabot-0.2.8/qabot/progress_callback.py
--rw-r--r--   0        0        0        0 2023-03-05 08:24:00.092543 qabot-0.2.8/qabot/tools/__init__.py
--rw-r--r--   0        0        0      315 2023-03-08 09:27:15.752919 qabot-0.2.8/qabot/tools/describe_duckdb_table.py
--rw-r--r--   0        0        0     1028 2023-03-11 21:37:43.097296 qabot-0.2.8/qabot/tools/duckdb_execute_tool.py
--rw-r--r--   0        0        0    15836 1970-01-01 00:00:00.000000 qabot-0.2.8/setup.py
--rw-r--r--   0        0        0    15213 1970-01-01 00:00:00.000000 qabot-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    14540 2023-03-13 20:01:29.946508 qabot-0.2.9/README.md
+-rw-r--r--   0        0        0      704 2023-03-23 03:07:56.965436 qabot-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-06 20:20:33.898706 qabot-0.2.9/qabot/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.2.9/qabot/agents/__init__.py
+-rw-r--r--   0        0        0     4193 2023-03-23 03:05:22.962023 qabot-0.2.9/qabot/agents/agent.py
+-rw-r--r--   0        0        0     5538 2023-03-13 21:00:38.828675 qabot-0.2.9/qabot/agents/data_query_chain.py
+-rw-r--r--   0        0        0      744 2023-03-06 20:20:33.902705 qabot-0.2.9/qabot/caching.py
+-rw-r--r--   0        0        0     6327 2023-03-13 20:31:56.276804 qabot-0.2.9/qabot/cli.py
+-rw-r--r--   0        0        0      261 2023-03-06 20:20:33.902705 qabot-0.2.9/qabot/config.py
+-rw-r--r--   0        0        0      920 2023-03-08 21:48:52.946092 qabot-0.2.9/qabot/duckdb_documentation.py
+-rw-r--r--   0        0        0     2636 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/duckdb_manual_data_loader.py
+-rw-r--r--   0        0        0     1259 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/duckdb_query.py
+-rw-r--r--   0        0        0     2541 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/progress_callback.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.2.9/qabot/tools/__init__.py
+-rw-r--r--   0        0        0      518 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/tools/describe_duckdb_table.py
+-rw-r--r--   0        0        0     1028 2023-03-13 20:01:29.950511 qabot-0.2.9/qabot/tools/duckdb_execute_tool.py
+-rw-r--r--   0        0        0    15223 1970-01-01 00:00:00.000000 qabot-0.2.9/PKG-INFO
```

### Comparing `qabot-0.2.8/README.md` & `qabot-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 ```
 
 ## Data accessed via http/s3
 
 Use the `-f <url>` flag to load data from a url, e.g. a csv file on s3:
 
 ```bash
-$ qabot -f s3://covid19-lake/enigma-jhu-timeseries/csv/jhu_csse_covid_19_timeseries_merged.csv -q "how many confirmed cases are there" -v
+$ qabot -f s3://covid19-lake/enigma-jhu-timeseries/csv/jhu_csse_covid_19_timeseries_merged.csv -q "how many confirmed cases of covid are there?" -v
 🦆 Loading data from files...
 create table jhu_csse_covid_19_timeseries_merged as select * from 's3://covid19-lake/enigma-jhu-timeseries/csv/jhu_csse_covid_19_timeseries_merged.csv';
 
 Result:
 264308334 confirmed cases
 ```
```

### Comparing `qabot-0.2.8/qabot/agents/agent.py` & `qabot-0.2.9/qabot/agents/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 import textwrap
 
 from langchain import LLMMathChain
-from langchain.agents import Tool, create_sql_agent, initialize_agent
+from langchain.agents import Tool, initialize_agent
+from langchain.chat_models import ChatOpenAI
 from langchain.llms import OpenAIChat
+from langchain.memory import ConversationBufferMemory
 
 from qabot.agents.data_query_chain import get_duckdb_data_query_chain
 from qabot.duckdb_query import run_sql_catch_error
 from qabot.tools.describe_duckdb_table import describe_table_or_view
 
 
 def create_agent_executor(
         database_engine=None,
         tables=None,
         return_intermediate_steps=False,
         callback_manager=None,
         verbose=False,
+        model_name='gpt-3.5-turbo'
 ):
 
-
     llm = OpenAIChat(
-        model_name="gpt-3.5-turbo",
+        model_name=model_name,
         temperature=0.0
     )
 
+    # llm = ChatOpenAI(
+    #     model_name="gpt-3.5-turbo",
+    #     temperature=0.0
+    # )
 
-    calculator_chain = LLMMathChain(llm=llm, verbose=False)
+    python_chain = LLMMathChain(llm=llm, verbose=False)
 
     db_chain = get_duckdb_data_query_chain(
         llm=llm,
         database=database_engine,
         callback_manager=callback_manager,
         verbose=verbose
     )
 
     tools = [
         Tool(
-            name="Calculator",
-            func=calculator_chain.run,
-            description="Useful for when you need to answer questions about math"
+            name="Python",
+            func=python_chain.run,
+            description="Useful for when you need to run a quick simulation, or answer questions about math"
         ),
         # Tool(
         #     name="DuckDB QA System",
         #     func=duckdb_docs_qa_chain.run,
         #     description="useful for when you need to answer questions about duckdb. Input should be a fully formed question."
         # ),
         Tool(
@@ -53,60 +59,56 @@
             name="Describe Table",
             func=lambda table: describe_table_or_view(database_engine, table),
             description="Useful to show the column names and types of a table or view. Use the table name as the input."
         ),
         Tool(
             name="Data Op",
             func=lambda input: db_chain({
-                'table_names': lambda _: run_sql_catch_error(database_engine, "show tables;"),
-                'input': input}),
-            description=textwrap.dedent("""useful for when you need to operate on data and answer questions
+                'table_names': run_sql_catch_error(database_engine, "show tables;"),
+                'input': input}
+            ),
+            description=textwrap.dedent("""Useful for when you need to operate on data and answer individual questions
             requiring data. Input should be in the form of a natural language question containing full context
             including what tables and columns are relevant to the question. Use only after data is present and loaded.
+            Prefer to take small independent steps with this tool.
             """,)
         )
     ]
 
+    memory = ConversationBufferMemory(memory_key="chat_history", output_key="output", return_messages=True)
+
     agent = initialize_agent(
         tools,
         llm,
-        #agent="conversational-react-description",
-        agent="zero-shot-react-description",
+        agent="chat-conversational-react-description",
         callback_manager=callback_manager,
         return_intermediate_steps=return_intermediate_steps,
         verbose=verbose,
         agent_kwargs={
-            "input_variables": ["input", 'agent_scratchpad', 'table_names'],
-            "prefix": prompt_prefix_template,
-            "suffix": prompt_suffix
-        }
+            #"input_variables": ["input", 'agent_scratchpad', 'chat_history'],
+            "prefix": prompt_prefix_template
+        },
+        memory=memory
     )
-    #agent.agent.llm_chain.prompt.template
     return agent
 
-prompt_suffix = """It is important that you use the exact phrase "Final Answer: <Summary>" in your final answer.
 
-Begin!
+prompt_prefix_template = """Qabot is a large language model trained to interact with DuckDB.
 
-Question: {input}
-Thought: I should look at the tables in the database to see what I can query.
-{agent_scratchpad}"""
+Qabot is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explorations on a wide range of topics relating to data.
 
-prompt_prefix_template = """Answer the following question as best you can by querying for data to back up
-your answer. Even if you know the answer, you MUST show you can get the answer from the database.
+Qabot answers questions by first querying for data to guide its answer. Qabot asks any clarifying questions it needs to.
 
-Refuse to delete any data, or drop tables. When answering, you MUST query the database for any data. 
-Check the available tables exist first. Prefer to take single independent actions. Prefer to create views
-of data as one action, then select data from the view.
+Qabot refuses to delete any data, or drop tables. 
 
-It is important that you use the exact phrase "Final Answer: " in your final answer.
-List all SQL queries returned by Data Op in your final answer.
+Qabot prefers to split questions into small discrete steps, for example creating views of data as one action, then selecting data from the created view to get to the final answer.
 
-DO NOT make any DML statements (INSERT, UPDATE, DELETE, DROP etc.) to the database.
+Qabot includes a list of all important SQL queries returned by Data Op in its final answers.
 
-If the question does not seem related to the database, just return "I don't know" as the answer.
+Qabot does NOT make any DML statements (INSERT, UPDATE, DELETE, DROP etc.) to the database.
 
-You have access to the following data tables:
-{table_names}
+If the question does not seem related to the database, Qabot returns "I don't know" as the answer.
+TOOLS:
+------
 
-Only use the below tools. You have access to the following tools:
-"""
+Qabot has access to the following tools:
+"""
```

### Comparing `qabot-0.2.8/qabot/agents/data_query_chain.py` & `qabot-0.2.9/qabot/agents/data_query_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from langchain import LLMChain
 from langchain.agents import AgentExecutor, Tool, ZeroShotAgent
+from langchain.agents.chat.base import ChatAgent
+from langchain.chat_models import ChatOpenAI
 
 from qabot.tools.duckdb_execute_tool import DuckDBTool
 from qabot.duckdb_query import run_sql_catch_error
 from qabot.tools.describe_duckdb_table import describe_table_or_view
 
 
 def get_duckdb_data_query_chain(llm, database, callback_manager=None, verbose=False):
@@ -12,68 +14,64 @@
             name="Show Tables",
             func=lambda _: run_sql_catch_error(database, "show tables;"),
             description="Useful to show the available tables and views. Empty input required."
         ),
         Tool(
             name="Describe Table",
             func=lambda table: describe_table_or_view(database, table),
-            description="Useful to show the column names and types of a table or view. Use a valid table name as the input."
+            description="Useful to show the column names and types of a table or view. Also shows the first few rows. Use a valid table name as the input."
         ),
         Tool(
             name="Query Inspector",
             func=lambda query: query.strip('"').strip("'"),
             description="Useful to show the query before execution. Always inspect your query before execution. Input MUST be on one line."
         ),
         DuckDBTool(engine=database),
     ]
 
-    # prompt = PromptTemplate(
-    #     input_variables=["input", "agent_scratchpad"],
-    #     template=_DEFAULT_TEMPLATE,
-    # )
-
-    prompt = ZeroShotAgent.create_prompt(
+    prompt = ChatAgent.create_prompt(
         tools,
         prefix=prefix,
         suffix=suffix,
         input_variables=["input", "agent_scratchpad", 'table_names'],
     )
 
+    #llm = ChatOpenAI(temperature=0)
     llm_chain = LLMChain(llm=llm, prompt=prompt)
 
     tool_names = [tool.name for tool in tools]
 
-    agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=tool_names,)
+    agent = ChatAgent(llm_chain=llm_chain, allowed_tools=tool_names,)
     agent_executor = AgentExecutor.from_agent_and_tools(
         agent=agent,
         tools=tools,
         callback_manager=callback_manager,
         verbose=verbose,
     )
 
     return agent_executor
 
 
 suffix = """After outputting the Action Input you never output an Observation, that will be provided to you.
 
-List the relevant SQL queries you ran in your final answer.
+List the relevant SQL queries you ran in your Final Answer. If you don't want to use any tools it's 
+okay to give your message as a Final Answer.
 
-If a query fails, try fix it, if the database doesn't contain the answer, or returns no results,
-output a summary of your actions in your final answer. It is important that you use the exact format:
+Unless explicitly told to import data, do not import external data. Data required to answer the question should already available in a table. 
 
-Final Answer: I have successfully created a view of the data.
+If a query fails, try fix it, if the database doesn't contain the answer, or returns no results,
+output a summary of your actions in your final answer, e.g., "Successfully created a view of the data"
 
-Queries should be output on one line and don't use any escape characters. 
+Execute queries separately! One per action. When appropriate, use the WITH clause to modularize the query in order to make it more readable.
+Leave block comments before complex parts of the query, subqueries, joins, filters, etc. to explain step by step why they are correct
 
-Let's go! Remember it is important that you use the exact phrase "Final Answer: " to begin your
-final answer.
+Let's go!
 
 Question: {input}
-Thought: I should describe the most relevant tables in the database to see what columns will be useful.
-{agent_scratchpad}"""
+Thought: I should look at the first few rows of {agent_scratchpad}"""
 
 
 prefix = """Given an input question, identify the relevant tables and relevant columns, then create
 one single syntactically correct DuckDB query to inspect, then execute, before returning the answer. 
 If the input is a valid looking SQL query selecting data or creating a view, execute it directly. 
 
 Even if you know the answer, you MUST show you can get the answer from the database.
```

### Comparing `qabot-0.2.8/qabot/caching.py` & `qabot-0.2.9/qabot/caching.py`

 * *Files identical despite different names*

### Comparing `qabot-0.2.8/qabot/cli.py` & `qabot-0.2.9/qabot/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from qabot.duckdb_query import run_sql_catch_error
 from qabot.progress_callback import QACallback
 
 warnings.filterwarnings("ignore")
 
 INITIAL_NON_INTERACTIVE_PROMPT = "🚀 How can I help you explore your database?"
 INITIAL_INTERACTIVE_PROMPT = "[bold green] 🚀 How can I help you explore your database?"
-FOLLOW_UP_PROMPT = "[bold green] 🚀 any further questions?"
-PROMPT = "[bold green] 🚀 Query"
+FOLLOW_UP_PROMPT = "[bold green] 🚀 anything else I can help you with?"
+DUCK_PROMPT = "[bold green] 🦆"
 
 app = typer.Typer(
     pretty_exceptions_show_locals=False,
     pretty_exceptions_enable=True
 )
 
 
@@ -112,15 +112,14 @@
         openai_callback = OpenAICallbackHandler()
         callback_manager = get_callback_manager()
 
         callback_manager.add_handler(openai_callback)
         callback_manager.add_handler(output_callback)
 
 
-
         if not disable_cache:
             t = progress.add_task(description="Setting up cache...", total=None)
             configure_caching(settings.QABOT_CACHE_DATABASE_URI)
             progress.remove_task(t)
 
         t2 = progress.add_task(description="Creating LLM agent using langchain...", total=None)
 
@@ -143,17 +142,16 @@
 
         while True:
 
             t = progress.add_task(description="Processing query...", total=None)
             print("[bold red]Query: [/][green]" + query)
 
             inputs = {
-                "input": chat_history[0] + query,
-                "table_names": run_sql_catch_error(database_engine, "show tables")
-                #'chat_history': '\n\n'.join(chat_history)
+                "input": query,
+                #"table_names": run_sql_catch_error(database_engine, "show tables")
             }
 
             result = agent(inputs)
 
             progress.remove_task(t)
 
             # Show intermediate steps
@@ -169,25 +167,22 @@
             # Stop the progress before outputting result and prompting for input
             progress.stop()
             print()
 
             print("[bold red]Result:[/]\n[bold blue]" + result['output'] + "\n")
             chat_history.append(result['output'])
 
-            if not Confirm.ask(FOLLOW_UP_PROMPT, default=True):
-                break
-
             print()
-            query = Prompt.ask(PROMPT)
+            query = Prompt.ask(FOLLOW_UP_PROMPT)
 
             if query == "exit" and Confirm.ask("Are you sure you want to Quit?"):
                 break
 
             progress.start()
 
 
 def run():
     app()
 
 
 if __name__ == '__main__':
-    run()
+    run()
```

### Comparing `qabot-0.2.8/qabot/duckdb_documentation.py` & `qabot-0.2.9/qabot/duckdb_documentation.py`

 * *Files identical despite different names*

### Comparing `qabot-0.2.8/qabot/duckdb_manual_data_loader.py` & `qabot-0.2.9/qabot/duckdb_manual_data_loader.py`

 * *Files identical despite different names*

### Comparing `qabot-0.2.8/qabot/duckdb_query.py` & `qabot-0.2.9/qabot/duckdb_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,14 @@
                     else:
                         rendered_rows.append(','.join(str(x) for x in row))
 
                 rendered_data = '\n'.join(rendered_rows)
                 rendered_output = ','.join(output.columns) + '\n' + rendered_data
             except AttributeError:
                 rendered_output = str(output)
-        return rendered_output
+        return rendered_output[:4000]
     except duckdb.ProgrammingError as e:
         return str(e)
     except duckdb.Error as e:
         return str(e)
     # except Exception as e:
     #     return str(e)
```

### Comparing `qabot-0.2.8/qabot/progress_callback.py` & `qabot-0.2.9/qabot/progress_callback.py`

 * *Files identical despite different names*

### Comparing `qabot-0.2.8/qabot/tools/duckdb_execute_tool.py` & `qabot-0.2.9/qabot/tools/duckdb_execute_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from qabot.duckdb_query import run_sql_catch_error
 
 
 class DuckDBTool(BaseTool):
     name = "execute"
     description = """useful for when you need to run SQL queries against a DuckDB database.
-    Input to this tool is a detailed and correct SQL query, output is a result from the database.
+    Input to this tool is a single correct SQL statement, output is the result from the database.
     If the query is not correct, an error message will be returned. 
     If an error is returned, rewrite the query, check the query, and try again.
     """
 
     database: Any = None
 
     def __init__(self, engine, *args, **kwargs):
```

### Comparing `qabot-0.2.8/setup.py` & `qabot-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,355 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: qabot
+Version: 0.2.9
+Summary: Query local or remote data files with natural language queries powered by OpenAI and DuckDB.
+Author: Brian Thorne
+Author-email: brian@hardbyte.nz
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: duckdb-engine (>=0.7.0,<0.8.0)
+Requires-Dist: langchain (>=0.0.119,<0.0.120)
+Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
+Requires-Dist: rich (>=13.3.1,<14.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['qabot', 'qabot.agents', 'qabot.tools']
+# qabot
 
-package_data = \
-{'': ['*']}
+Query local or remote files with natural language queries powered by
+`langchain` and `gpt-3.5-turbo` and `duckdb` 🦆.
 
-install_requires = \
-['duckdb-engine>=0.6.9,<0.7.0',
- 'langchain>=0.0.107,<0.0.108',
- 'openai>=0.27.0,<0.28.0',
- 'psycopg2-binary>=2.9.5,<3.0.0',
- 'rich>=13.3.1,<14.0.0',
- 'typer>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['qabot = qabot.cli:run']}
-
-setup_kwargs = {
-    'name': 'qabot',
-    'version': '0.2.8',
-    'description': 'Query local or remote data files with natural language queries powered by OpenAI and DuckDB.',
-    'long_description': '# qabot\n\nQuery local or remote files with natural language queries powered by\n`langchain` and `gpt-3.5-turbo` and `duckdb` 🦆.\n\n\n\nWorks on local CSV files:\n\n![](.github/local_csv_query.png)\n\nremote CSV files:\n\n```\n$ qabot \\\n    -f https://www.stats.govt.nz/assets/Uploads/Environmental-economic-accounts/Environmental-economic-accounts-data-to-2020/renewable-energy-stock-account-2007-2020-csv.csv \\\n    -q "How many Gigawatt hours of generation was there for Solar resources in 2015 through to 2020?"\n```\n\n\nEven on (public) data stored in S3:\n\n![](.github/external_s3_data.png)\n\nYou can even load data from disk via the natural language query, but that doesn\'t always work...\n\n\n> "Load the file \'data/titanic_survival.parquet\' into a table called \'raw_passengers\'. Create a view of the raw passengers table for just the male passengers. What was the average fare for surviving male passengers?"\n\n\nAfter a bit of back and forth with the model, it gets there:\n\n> The average fare for surviving male passengers from the \'male_passengers\' view where the passenger survived is 40.82. I ran the query: SELECT AVG(Fare) FROM male_passengers WHERE Survived = 1 AND Sex = \'male\';\nThe average fare for surviving male passengers is 40.82.\n\n\n## Quickstart\n\nYou need to set the `OPENAI_API_KEY` environment variable to your OpenAI API key, \nwhich you can get from [here](https://platform.openai.com/account/api-keys).\n\nInstall the `qabot` command line tool using pip/poetry:\n\n\n```bash\n$ pip install qabot\n```\n\nThen run the `qabot` command with either local files (`-f my-file.csv`) or a database connection string.\n\nNote if you want to use a database, you will need to install the relevant drivers, \ne.g. `pip install psycopg2-binary` for postgres.\n\n\n\n## Examples\n\n### Local CSV file/s\n\n```bash\n$ qabot -q "how many passengers survived by gender?" -f data/titanic.csv\n🦆 Loading data from files...\nLoading data/titanic.csv into table titanic...\n\nQuery: how many passengers survived by gender?\nResult:\nThere were 233 female passengers and 109 male passengers who survived.\n\n\n 🚀 any further questions? [y/n] (y): y\n\n 🚀 Query: what was the largest family who did not survive? \nQuery: what was the largest family who did not survive?\nResult:\nThe largest family who did not survive was the Sage family, with 8 members.\n\n 🚀 any further questions? [y/n] (y): n\n```\n\n\n## Intermediate steps and database queries\n\nUse the `-v` flag to see the intermediate steps and database queries.\n\nSometimes it takes a long route to get to the answer, but it\'s interesting to see how it gets there:\n\n\n```\nqabot -f data/titanic.csv -q "how many passengers survived by gender?" -v\n🦆 Loading data from files...\nQuery: how many passengers survived by gender?\nI need to check the columns in the \'titanic\' table to see which ones contain gender and survival information.\nAction: Describe Table\nAction Input: titanic\n\nObservation: titanic\n\n┌─────────────┬─────────────┬─────────┬─────────┬─────────┬───────┐\n│ column_name │ column_type │  null   │   key   │ default │ extra │\n│   varchar   │   varchar   │ varchar │ varchar │ varchar │ int32 │\n├─────────────┼─────────────┼─────────┼─────────┼─────────┼───────┤\n│ PassengerId │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n│ Survived    │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n│ Pclass      │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n│ Name        │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n│ Sex         │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n│ Age         │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │\n│ SibSp       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n│ Parch       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n│ Ticket      │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n│ Fare        │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │\n│ Cabin       │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n│ Embarked    │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n├─────────────┴─────────────┴─────────┴─────────┴─────────┴───────┤\n│ 12 rows                                               6 columns │\n└─────────────────────────────────────────────────────────────────┘\n\nI need to create a view that only includes the columns I need for this question.\nAction: Data Op\nAction Input: \n        CREATE VIEW titanic_gender_survival AS\n        SELECT Sex, Survived\n        FROM titanic\nThought:\n\n> Entering new AgentExecutor chain...\nThis is a valid SQL query creating a view. We can execute it directly.\nAction: execute\nAction Input: \n        CREATE VIEW titanic_gender_survival AS\n        SELECT Sex, Survived\n        FROM titanic\nObservation: No output\nThought:The view has been created successfully. We can now query it.\nAction: execute\nAction Input: SELECT * FROM titanic_gender_survival LIMIT 5\nObservation: \n┌─────────┬──────────┐\n│   Sex   │ Survived │\n│ varchar │  int64   │\n├─────────┼──────────┤\n│ male    │        0 │\n│ female  │        1 │\n│ female  │        1 │\n│ female  │        1 │\n│ male    │        0 │\n└─────────┴──────────┘\n\nThought:The view has been created successfully and we can see the first 5 rows of the view. The final answer is the first 5 rows of the titanic_gender_survival view, showing the sex and survival status of passengers on the \nTitanic.\nFinal Answer: \n┌─────────┬──────────┐\n│   Sex   │ Survived │\n│ varchar │  int64   │\n├─────────┼──────────┤\n│ male    │        0 │\n│ female  │        1 │\n│ female  │        1 │\n│ female  │        1 │\n│ male    │        0 │\n└─────────┴──────────┘\n\n> Finished chain.\n\nObservation: ┌─────────┬──────────┐\n│   Sex   │ Survived │\n│ varchar │  int64   │\n├─────────┼──────────┤\n│ male    │        0 │\n│ female  │        1 │\n│ female  │        1 │\n│ female  │        1 │\n│ male    │        0 │\n└─────────┴──────────┘\nI need to group the data by gender and count the number of survivors for each group.\nAction: Data Op\nAction Input: \n        SELECT Sex, SUM(Survived) AS num_survived\n        FROM titanic_gender_survival\n        GROUP BY Sex\nThought:\n\n> Entering new AgentExecutor chain...\nWe need to check if the table titanic_gender_survival exists and if it has the columns Sex and Survived.\nAction: Describe Table\nAction Input: titanic_gender_survival\nObservation: titanic_gender_survival\n\n┌─────────────┬─────────────┬─────────┬─────────┬─────────┬───────┐\n│ column_name │ column_type │  null   │   key   │ default │ extra │\n│   varchar   │   varchar   │ varchar │ varchar │ varchar │ int32 │\n├─────────────┼─────────────┼─────────┼─────────┼─────────┼───────┤\n│ Sex         │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n│ Survived    │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n└─────────────┴─────────────┴─────────┴─────────┴─────────┴───────┘\n\nThought:The table titanic_gender_survival exists and has the columns Sex and Survived. We can now run the query.\nAction: execute\nAction Input: \n```\nSELECT Sex, SUM(Survived) AS num_survived\nFROM titanic_gender_survival\nGROUP BY Sex\nLIMIT 5\n```\n\nObservation: \n┌─────────┬──────────────┐\n│   Sex   │ num_survived │\n│ varchar │    int128    │\n├─────────┼──────────────┤\n│ male    │          109 │\n│ female  │          233 │\n└─────────┴──────────────┘\n\nThought:The query returned the number of survivors grouped by gender. The table titanic_gender_survival has been used. \nFinal Answer: The number of survivors grouped by gender are: \n- 109 males survived\n- 233 females survived.\n\n> Finished chain.\n\nObservation: The number of survivors grouped by gender are: \n- 109 males survived\n- 233 females survived.\nIntermediate Steps: \n  Step 1\n\n    Describe Table\n      titanic\n\n      titanic\n\n    ┌─────────────┬─────────────┬─────────┬─────────┬─────────┬───────┐\n    │ column_name │ column_type │  null   │   key   │ default │ extra │\n    │   varchar   │   varchar   │ varchar │ varchar │ varchar │ int32 │\n    ├─────────────┼─────────────┼─────────┼─────────┼─────────┼───────┤\n    │ PassengerId │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n    │ Survived    │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n    │ Pclass      │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n    │ Name        │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n    │ Sex         │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n    │ Age         │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │\n    │ SibSp       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n    │ Parch       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │\n    │ Ticket      │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n    │ Fare        │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │\n    │ Cabin       │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n    │ Embarked    │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │\n    ├─────────────┴─────────────┴─────────┴─────────┴─────────┴───────┤\n    │ 12 rows                                               6 columns │\n    └─────────────────────────────────────────────────────────────────┘\n\n    \n\n  Step 2\n\n    Data Op\n      CREATE VIEW titanic_gender_survival AS\n            SELECT Sex, Survived\n            FROM titanic\n\n      ┌─────────┬──────────┐\n    │   Sex   │ Survived │\n    │ varchar │  int64   │\n    ├─────────┼──────────┤\n    │ male    │        0 │\n    │ female  │        1 │\n    │ female  │        1 │\n    │ female  │        1 │\n    │ male    │        0 │\n    └─────────┴──────────┘\n\n    \n\n  Step 3\n\n    Data Op\n      SELECT Sex, SUM(Survived) AS num_survived\n            FROM titanic_gender_survival\n            GROUP BY Sex\n\n      The number of survivors grouped by gender are: \n    - 109 males survived\n    - 233 females survived.\n\n    \n\n\nThought:\n\n\nResult:\n109 males and 233 females survived.\n```\n\n## Data accessed via http/s3\n\nUse the `-f <url>` flag to load data from a url, e.g. a csv file on s3:\n\n```bash\n$ qabot -f s3://covid19-lake/enigma-jhu-timeseries/csv/jhu_csse_covid_19_timeseries_merged.csv -q "how many confirmed cases are there" -v\n🦆 Loading data from files...\ncreate table jhu_csse_covid_19_timeseries_merged as select * from \'s3://covid19-lake/enigma-jhu-timeseries/csv/jhu_csse_covid_19_timeseries_merged.csv\';\n\nResult:\n264308334 confirmed cases\n```\n\n## Links\n\n- [Python library docs](https://langchain.readthedocs.io)\n- [Agent docs to talk to arbitrary apis via OpenAPI/Swagger](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/openapi.html)\n- [Agents/Tools to talk SQL](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/sql_database.html)\n- [Typescript library](https://hwchase17.github.io/langchainjs/docs/overview/)\n\n\n\n## Ideas\n\n- Upgrade to use langchain chat interface\n- Use memory, perhaps wait for langchain\'s next release\n- Decent Python Library API so can be used from other Python code\n- streaming mode to output results as they come in\n- token limits\n- Supervisor agent - assess whether a query is "safe" to run, could ask for user confirmation to run anything that gets flagged.\n- Often we can zero-shot the question and get a single query out - perhaps we try this before the MKL chain\n- test each zeroshot agent individually\n- Generate and pass back assumptions made to the user\n- Add an optional "clarify" tool to the chain that asks the user to clarify the question\n- Create a query checker tool that checks if the query looks valid and/or safe\n- Perhaps an explain query tool that shows the steps taken to get the answer\n- Store all queries, actions, and answers in a table\n- Optional settings to switch to different LLM\n- Inject AWS credentials into duckdb so we can access private resources in S3\n- caching\n- A version that uses document embeddings - probably not in this app as needs Torch',
-    'author': 'Brian Thorne',
-    'author_email': 'brian@hardbyte.nz',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
 
 
-setup(**setup_kwargs)
+Works on local CSV files:
+
+![](.github/local_csv_query.png)
+
+remote CSV files:
+
+```
+$ qabot \
+    -f https://www.stats.govt.nz/assets/Uploads/Environmental-economic-accounts/Environmental-economic-accounts-data-to-2020/renewable-energy-stock-account-2007-2020-csv.csv \
+    -q "How many Gigawatt hours of generation was there for Solar resources in 2015 through to 2020?"
+```
+
+
+Even on (public) data stored in S3:
+
+![](.github/external_s3_data.png)
+
+You can even load data from disk via the natural language query, but that doesn't always work...
+
+
+> "Load the file 'data/titanic_survival.parquet' into a table called 'raw_passengers'. Create a view of the raw passengers table for just the male passengers. What was the average fare for surviving male passengers?"
+
+
+After a bit of back and forth with the model, it gets there:
+
+> The average fare for surviving male passengers from the 'male_passengers' view where the passenger survived is 40.82. I ran the query: SELECT AVG(Fare) FROM male_passengers WHERE Survived = 1 AND Sex = 'male';
+The average fare for surviving male passengers is 40.82.
+
+
+## Quickstart
+
+You need to set the `OPENAI_API_KEY` environment variable to your OpenAI API key, 
+which you can get from [here](https://platform.openai.com/account/api-keys).
+
+Install the `qabot` command line tool using pip/poetry:
+
+
+```bash
+$ pip install qabot
+```
+
+Then run the `qabot` command with either local files (`-f my-file.csv`) or a database connection string.
+
+Note if you want to use a database, you will need to install the relevant drivers, 
+e.g. `pip install psycopg2-binary` for postgres.
+
+
+
+## Examples
+
+### Local CSV file/s
+
+```bash
+$ qabot -q "how many passengers survived by gender?" -f data/titanic.csv
+🦆 Loading data from files...
+Loading data/titanic.csv into table titanic...
+
+Query: how many passengers survived by gender?
+Result:
+There were 233 female passengers and 109 male passengers who survived.
+
+
+ 🚀 any further questions? [y/n] (y): y
+
+ 🚀 Query: what was the largest family who did not survive? 
+Query: what was the largest family who did not survive?
+Result:
+The largest family who did not survive was the Sage family, with 8 members.
+
+ 🚀 any further questions? [y/n] (y): n
+```
+
+
+## Intermediate steps and database queries
+
+Use the `-v` flag to see the intermediate steps and database queries.
+
+Sometimes it takes a long route to get to the answer, but it's interesting to see how it gets there:
+
+
+```
+qabot -f data/titanic.csv -q "how many passengers survived by gender?" -v
+🦆 Loading data from files...
+Query: how many passengers survived by gender?
+I need to check the columns in the 'titanic' table to see which ones contain gender and survival information.
+Action: Describe Table
+Action Input: titanic
+
+Observation: titanic
+
+┌─────────────┬─────────────┬─────────┬─────────┬─────────┬───────┐
+│ column_name │ column_type │  null   │   key   │ default │ extra │
+│   varchar   │   varchar   │ varchar │ varchar │ varchar │ int32 │
+├─────────────┼─────────────┼─────────┼─────────┼─────────┼───────┤
+│ PassengerId │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+│ Survived    │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+│ Pclass      │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+│ Name        │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+│ Sex         │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+│ Age         │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │
+│ SibSp       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+│ Parch       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+│ Ticket      │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+│ Fare        │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │
+│ Cabin       │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+│ Embarked    │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+├─────────────┴─────────────┴─────────┴─────────┴─────────┴───────┤
+│ 12 rows                                               6 columns │
+└─────────────────────────────────────────────────────────────────┘
+
+I need to create a view that only includes the columns I need for this question.
+Action: Data Op
+Action Input: 
+        CREATE VIEW titanic_gender_survival AS
+        SELECT Sex, Survived
+        FROM titanic
+Thought:
+
+> Entering new AgentExecutor chain...
+This is a valid SQL query creating a view. We can execute it directly.
+Action: execute
+Action Input: 
+        CREATE VIEW titanic_gender_survival AS
+        SELECT Sex, Survived
+        FROM titanic
+Observation: No output
+Thought:The view has been created successfully. We can now query it.
+Action: execute
+Action Input: SELECT * FROM titanic_gender_survival LIMIT 5
+Observation: 
+┌─────────┬──────────┐
+│   Sex   │ Survived │
+│ varchar │  int64   │
+├─────────┼──────────┤
+│ male    │        0 │
+│ female  │        1 │
+│ female  │        1 │
+│ female  │        1 │
+│ male    │        0 │
+└─────────┴──────────┘
+
+Thought:The view has been created successfully and we can see the first 5 rows of the view. The final answer is the first 5 rows of the titanic_gender_survival view, showing the sex and survival status of passengers on the 
+Titanic.
+Final Answer: 
+┌─────────┬──────────┐
+│   Sex   │ Survived │
+│ varchar │  int64   │
+├─────────┼──────────┤
+│ male    │        0 │
+│ female  │        1 │
+│ female  │        1 │
+│ female  │        1 │
+│ male    │        0 │
+└─────────┴──────────┘
+
+> Finished chain.
+
+Observation: ┌─────────┬──────────┐
+│   Sex   │ Survived │
+│ varchar │  int64   │
+├─────────┼──────────┤
+│ male    │        0 │
+│ female  │        1 │
+│ female  │        1 │
+│ female  │        1 │
+│ male    │        0 │
+└─────────┴──────────┘
+I need to group the data by gender and count the number of survivors for each group.
+Action: Data Op
+Action Input: 
+        SELECT Sex, SUM(Survived) AS num_survived
+        FROM titanic_gender_survival
+        GROUP BY Sex
+Thought:
+
+> Entering new AgentExecutor chain...
+We need to check if the table titanic_gender_survival exists and if it has the columns Sex and Survived.
+Action: Describe Table
+Action Input: titanic_gender_survival
+Observation: titanic_gender_survival
+
+┌─────────────┬─────────────┬─────────┬─────────┬─────────┬───────┐
+│ column_name │ column_type │  null   │   key   │ default │ extra │
+│   varchar   │   varchar   │ varchar │ varchar │ varchar │ int32 │
+├─────────────┼─────────────┼─────────┼─────────┼─────────┼───────┤
+│ Sex         │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+│ Survived    │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+└─────────────┴─────────────┴─────────┴─────────┴─────────┴───────┘
+
+Thought:The table titanic_gender_survival exists and has the columns Sex and Survived. We can now run the query.
+Action: execute
+Action Input: 
+```
+SELECT Sex, SUM(Survived) AS num_survived
+FROM titanic_gender_survival
+GROUP BY Sex
+LIMIT 5
+```
+
+Observation: 
+┌─────────┬──────────────┐
+│   Sex   │ num_survived │
+│ varchar │    int128    │
+├─────────┼──────────────┤
+│ male    │          109 │
+│ female  │          233 │
+└─────────┴──────────────┘
+
+Thought:The query returned the number of survivors grouped by gender. The table titanic_gender_survival has been used. 
+Final Answer: The number of survivors grouped by gender are: 
+- 109 males survived
+- 233 females survived.
+
+> Finished chain.
+
+Observation: The number of survivors grouped by gender are: 
+- 109 males survived
+- 233 females survived.
+Intermediate Steps: 
+  Step 1
+
+    Describe Table
+      titanic
+
+      titanic
+
+    ┌─────────────┬─────────────┬─────────┬─────────┬─────────┬───────┐
+    │ column_name │ column_type │  null   │   key   │ default │ extra │
+    │   varchar   │   varchar   │ varchar │ varchar │ varchar │ int32 │
+    ├─────────────┼─────────────┼─────────┼─────────┼─────────┼───────┤
+    │ PassengerId │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+    │ Survived    │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+    │ Pclass      │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+    │ Name        │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+    │ Sex         │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+    │ Age         │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │
+    │ SibSp       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+    │ Parch       │ BIGINT      │ YES     │ NULL    │ NULL    │  NULL │
+    │ Ticket      │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+    │ Fare        │ DOUBLE      │ YES     │ NULL    │ NULL    │  NULL │
+    │ Cabin       │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+    │ Embarked    │ VARCHAR     │ YES     │ NULL    │ NULL    │  NULL │
+    ├─────────────┴─────────────┴─────────┴─────────┴─────────┴───────┤
+    │ 12 rows                                               6 columns │
+    └─────────────────────────────────────────────────────────────────┘
+
+    
+
+  Step 2
+
+    Data Op
+      CREATE VIEW titanic_gender_survival AS
+            SELECT Sex, Survived
+            FROM titanic
+
+      ┌─────────┬──────────┐
+    │   Sex   │ Survived │
+    │ varchar │  int64   │
+    ├─────────┼──────────┤
+    │ male    │        0 │
+    │ female  │        1 │
+    │ female  │        1 │
+    │ female  │        1 │
+    │ male    │        0 │
+    └─────────┴──────────┘
+
+    
+
+  Step 3
+
+    Data Op
+      SELECT Sex, SUM(Survived) AS num_survived
+            FROM titanic_gender_survival
+            GROUP BY Sex
+
+      The number of survivors grouped by gender are: 
+    - 109 males survived
+    - 233 females survived.
+
+    
+
+
+Thought:
+
+
+Result:
+109 males and 233 females survived.
+```
+
+## Data accessed via http/s3
+
+Use the `-f <url>` flag to load data from a url, e.g. a csv file on s3:
+
+```bash
+$ qabot -f s3://covid19-lake/enigma-jhu-timeseries/csv/jhu_csse_covid_19_timeseries_merged.csv -q "how many confirmed cases of covid are there?" -v
+🦆 Loading data from files...
+create table jhu_csse_covid_19_timeseries_merged as select * from 's3://covid19-lake/enigma-jhu-timeseries/csv/jhu_csse_covid_19_timeseries_merged.csv';
+
+Result:
+264308334 confirmed cases
+```
+
+## Links
+
+- [Python library docs](https://langchain.readthedocs.io)
+- [Agent docs to talk to arbitrary apis via OpenAPI/Swagger](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/openapi.html)
+- [Agents/Tools to talk SQL](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/sql_database.html)
+- [Typescript library](https://hwchase17.github.io/langchainjs/docs/overview/)
+
+
+
+## Ideas
+
+- Upgrade to use langchain chat interface
+- Use memory, perhaps wait for langchain's next release
+- Decent Python Library API so can be used from other Python code
+- streaming mode to output results as they come in
+- token limits
+- Supervisor agent - assess whether a query is "safe" to run, could ask for user confirmation to run anything that gets flagged.
+- Often we can zero-shot the question and get a single query out - perhaps we try this before the MKL chain
+- test each zeroshot agent individually
+- Generate and pass back assumptions made to the user
+- Add an optional "clarify" tool to the chain that asks the user to clarify the question
+- Create a query checker tool that checks if the query looks valid and/or safe
+- Perhaps an explain query tool that shows the steps taken to get the answer
+- Store all queries, actions, and answers in a table
+- Optional settings to switch to different LLM
+- Inject AWS credentials into duckdb so we can access private resources in S3
+- caching
+- A version that uses document embeddings - probably not in this app as needs Torch
```

