# Comparing `tmp/sql-scheduler-0.2.5.tar.gz` & `tmp/sql-scheduler-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql-scheduler-0.2.5.tar", last modified: Mon Mar 13 15:51:29 2023, max compression
+gzip compressed data, was "sql-scheduler-0.3.1.tar", last modified: Wed Apr 12 20:03:33 2023, max compression
```

## Comparing `sql-scheduler-0.2.5.tar` & `sql-scheduler-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-03-13 15:51:29.624679 sql-scheduler-0.2.5/
--rw-r--r--   0 henryjones   (501) staff       (20)    35149 2023-02-16 15:18:28.000000 sql-scheduler-0.2.5/LICENSE.md
--rw-r--r--   0 henryjones   (501) staff       (20)    17569 2023-03-13 15:51:29.624314 sql-scheduler-0.2.5/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)    16727 2023-03-09 19:29:18.000000 sql-scheduler-0.2.5/README.md
--rw-r--r--   0 henryjones   (501) staff       (20)      967 2023-03-13 15:26:14.000000 sql-scheduler-0.2.5/pyproject.toml
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2023-03-13 15:51:29.624766 sql-scheduler-0.2.5/setup.cfg
--rw-r--r--   0 henryjones   (501) staff       (20)      718 2023-02-09 21:03:09.000000 sql-scheduler-0.2.5/setup.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-03-13 15:51:29.621294 sql-scheduler-0.2.5/sql_scheduler/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-02-09 21:26:31.000000 sql-scheduler-0.2.5/sql_scheduler/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1098 2023-03-09 18:21:51.000000 sql-scheduler-0.2.5/sql_scheduler/_constants.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1416 2023-02-23 15:50:54.000000 sql-scheduler-0.2.5/sql_scheduler/_helpers.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-02-09 21:03:00.000000 sql-scheduler-0.2.5/sql_scheduler/py.typed
--rwxr-xr-x   0 henryjones   (501) staff       (20)    18873 2023-03-13 15:36:51.000000 sql-scheduler-0.2.5/sql_scheduler/sql_scheduler.py
--rw-r--r--   0 henryjones   (501) staff       (20)    19961 2023-03-13 15:42:35.000000 sql-scheduler-0.2.5/sql_scheduler/sql_task.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-03-13 15:51:29.623803 sql-scheduler-0.2.5/sql_scheduler.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)    17569 2023-03-13 15:51:29.000000 sql-scheduler-0.2.5/sql_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)      428 2023-03-13 15:51:29.000000 sql-scheduler-0.2.5/sql_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2023-03-13 15:51:29.000000 sql-scheduler-0.2.5/sql_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       67 2023-03-13 15:51:29.000000 sql-scheduler-0.2.5/sql_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       24 2023-03-13 15:51:29.000000 sql-scheduler-0.2.5/sql_scheduler.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       14 2023-03-13 15:51:29.000000 sql-scheduler-0.2.5/sql_scheduler.egg-info/top_level.txt
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-04-12 20:03:33.369436 sql-scheduler-0.3.1/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    35149 2023-02-10 19:03:46.000000 sql-scheduler-0.3.1/LICENSE.md
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    17605 2023-04-12 20:03:33.369436 sql-scheduler-0.3.1/PKG-INFO
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    16763 2023-04-12 19:51:56.000000 sql-scheduler-0.3.1/README.md
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1055 2023-04-12 19:52:44.000000 sql-scheduler-0.3.1/pyproject.toml
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       38 2023-04-12 20:03:33.369436 sql-scheduler-0.3.1/setup.cfg
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      718 2023-02-10 16:24:51.000000 sql-scheduler-0.3.1/setup.py
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-04-12 20:03:33.369436 sql-scheduler-0.3.1/sql_scheduler/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      106 2023-04-12 19:49:04.000000 sql-scheduler-0.3.1/sql_scheduler/__init__.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      977 2023-04-12 19:01:35.000000 sql-scheduler-0.3.1/sql_scheduler/_constants.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1766 2023-04-12 16:29:13.000000 sql-scheduler-0.3.1/sql_scheduler/_helpers.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     7617 2023-04-12 19:40:13.000000 sql-scheduler-0.3.1/sql_scheduler/cli.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1281 2023-04-12 19:19:32.000000 sql-scheduler-0.3.1/sql_scheduler/exceptions.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    14096 2023-04-12 19:49:33.000000 sql-scheduler-0.3.1/sql_scheduler/orchestrator.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        0 2023-02-10 16:24:51.000000 sql-scheduler-0.3.1/sql_scheduler/py.typed
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     4377 2023-04-12 19:52:43.000000 sql-scheduler-0.3.1/sql_scheduler/sql_scheduler.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    20531 2023-04-12 19:59:27.000000 sql-scheduler-0.3.1/sql_scheduler/sql_task.py
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-04-12 20:03:33.369436 sql-scheduler-0.3.1/sql_scheduler.egg-info/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    17605 2023-04-12 20:03:33.000000 sql-scheduler-0.3.1/sql_scheduler.egg-info/PKG-INFO
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      507 2023-04-12 20:03:33.000000 sql-scheduler-0.3.1/sql_scheduler.egg-info/SOURCES.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        1 2023-04-12 20:03:33.000000 sql-scheduler-0.3.1/sql_scheduler.egg-info/dependency_links.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       63 2023-04-12 20:03:33.000000 sql-scheduler-0.3.1/sql_scheduler.egg-info/entry_points.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       33 2023-04-12 20:03:33.000000 sql-scheduler-0.3.1/sql_scheduler.egg-info/requires.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       14 2023-04-12 20:03:33.000000 sql-scheduler-0.3.1/sql_scheduler.egg-info/top_level.txt
```

### Comparing `sql-scheduler-0.2.5/LICENSE.md` & `sql-scheduler-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sql-scheduler-0.2.5/PKG-INFO` & `sql-scheduler-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-scheduler
-Version: 0.2.5
+Version: 0.3.1
 Summary: sql-scheduler allows you to easily run a suite of SQL scripts against a Postgres/Redshift database.
 Home-page: https://github.com/henryivesjones/sql-scheduler
 Author: Henry Jones
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: sql,postgres,scheduler,redshift
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -59,25 +59,24 @@
 
 ## Installation
 ```bash
 pip install sql-scheduler
 ```
 ## Configuration
 
-### Required Environment Variables
+### Environment Variables
  - `SQL_SCHEDULER_DDL_DIRECTORY`: An absolute path to the `ddl` directory. EX: `/home/ubuntu/sql/ddl/`
  - `SQL_SCHEDULER_INSERT_DIRECTORY`: An absolute path to the `insert` directory. EX: `/home/ubuntu/sql/insert/`
  - `SQL_SCHEDULER_DSN`: A DSN for connecting to your database in the form: `postgres://user:password@host:port/database?option=value`
-
-### Optional Environment Variables
  - `SQL_SCHEDULER_STAGE`: The default stage (`prod`, `dev`) to run in. Can be overridden by the CLI flag `--dev` or `--prod`. When running in the dev stage a dev schema must be provided, either thru an Environment Variable, or a cli argument.
  - `SQL_SCHEDULER_DEV_SCHEMA`: The schema to replace with when run in the `dev` stage. Can be overridden by the CLI argument `--dev-schema`.
  - `SQL_SCHEDULER_SIMPLE_OUTPUT`: Simplify the output of this program by removing the status message. (If you are running `sql-scheduler` not in the CLI then you probably want to set this to `1`)
  - `SQL_SCHEDULER_CACHE_DURATION`: The length of time for development cache runs to be valid (specified in seconds). Defaults to 6 hours
  - `SQL_SCHEDULER_INCREMENTAL_INTERVAL`: The number of days for the default incremental window (defaults to 14). Incremental windows starts at `00:00:00` 14 days ago and ends at `23:59:59.999` on the current day. The interval can be overridden by setting the `--start` and `--end` cli values.
+ - `SQL_SCHEDULER_CONCURRENCY`: The maximum number of concurrent tasks to be run
 
 ## Common Commands
 
 ### Running all scripts.
 ```bash
 sql-scheduler
 ```
```

### Comparing `sql-scheduler-0.2.5/README.md` & `sql-scheduler-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,25 +39,24 @@
 
 ## Installation
 ```bash
 pip install sql-scheduler
 ```
 ## Configuration
 
-### Required Environment Variables
+### Environment Variables
  - `SQL_SCHEDULER_DDL_DIRECTORY`: An absolute path to the `ddl` directory. EX: `/home/ubuntu/sql/ddl/`
  - `SQL_SCHEDULER_INSERT_DIRECTORY`: An absolute path to the `insert` directory. EX: `/home/ubuntu/sql/insert/`
  - `SQL_SCHEDULER_DSN`: A DSN for connecting to your database in the form: `postgres://user:password@host:port/database?option=value`
-
-### Optional Environment Variables
  - `SQL_SCHEDULER_STAGE`: The default stage (`prod`, `dev`) to run in. Can be overridden by the CLI flag `--dev` or `--prod`. When running in the dev stage a dev schema must be provided, either thru an Environment Variable, or a cli argument.
  - `SQL_SCHEDULER_DEV_SCHEMA`: The schema to replace with when run in the `dev` stage. Can be overridden by the CLI argument `--dev-schema`.
  - `SQL_SCHEDULER_SIMPLE_OUTPUT`: Simplify the output of this program by removing the status message. (If you are running `sql-scheduler` not in the CLI then you probably want to set this to `1`)
  - `SQL_SCHEDULER_CACHE_DURATION`: The length of time for development cache runs to be valid (specified in seconds). Defaults to 6 hours
  - `SQL_SCHEDULER_INCREMENTAL_INTERVAL`: The number of days for the default incremental window (defaults to 14). Incremental windows starts at `00:00:00` 14 days ago and ends at `23:59:59.999` on the current day. The interval can be overridden by setting the `--start` and `--end` cli values.
+ - `SQL_SCHEDULER_CONCURRENCY`: The maximum number of concurrent tasks to be run
 
 ## Common Commands
 
 ### Running all scripts.
 ```bash
 sql-scheduler
 ```
```

### Comparing `sql-scheduler-0.2.5/pyproject.toml` & `sql-scheduler-0.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sql-scheduler"
-version = "0.2.5"
+dynamic = ["version"]
 authors = [
   { name="Henry Jones", email="henryivesjones@gmail.com" },
 ]
 description = "sql-scheduler allows you to easily run a suite of SQL scripts against a Postgres/Redshift database."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text="GPL-3.0-or-later"}
@@ -16,23 +16,27 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
   "asyncpg",
-  "python-dateutil"
+  "python-dateutil",
+  "click>=8"
 ]
 
 keywords = [
   "sql",
   "postgres",
   "scheduler",
   "redshift"
 ]
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
-sql-scheduler = "sql_scheduler.sql_scheduler:main"
+sql-scheduler = "sql_scheduler.cli:entrypoint"
+
+[tool.setuptools.dynamic]
+version = {attr = "sql_scheduler.__version__"}
```

### Comparing `sql-scheduler-0.2.5/setup.py` & `sql-scheduler-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `sql-scheduler-0.2.5/sql_scheduler/_helpers.py` & `sql-scheduler-0.3.1/sql_scheduler/_helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 import os
 from typing import List, Tuple
 
+import click
+
 from ._constants import _SIMPLE_OUTPUT_ENVVAR
 
 _SIMPLE_OUTPUT = bool(os.environ.get(_SIMPLE_OUTPUT_ENVVAR, False))
 
 
 def w_print(content: str, end="\n"):
     if not _SIMPLE_OUTPUT:
         print("\x1b[2K\r", end="")
     print(content, end=end)
 
 
+class Logger:
+    persist_prev: bool
+
+    def __init__(self):
+        self.persist_prev = False
+
+    def out(self, message: str, persist: bool = True):
+        if self.persist_prev:
+            click.echo(message, nl=persist)
+        else:
+            click.echo(f"\x1b[2K\r{message}", nl=persist)
+        self.persist_prev = persist
+
+
 def pad_string(s: str, width: int):
     return f'{s}{" "*(width - len(s))}'
 
 
 def construct_table(headers: List[str], rows: List[tuple], delimiter: str = " | "):
     column_widths = [0 for _ in headers]
     for row in rows + [headers]:
```

### Comparing `sql-scheduler-0.2.5/sql_scheduler/sql_scheduler.py` & `sql-scheduler-0.3.1/sql_scheduler/sql_task.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,583 +1,562 @@
-import argparse
 import asyncio
+import hashlib
 import os
-import shutil
-import sys
+import re
 import time
-from datetime import datetime, timedelta
-from typing import List, Literal, Optional, Set, Tuple
+from datetime import datetime
+from enum import Enum
+from typing import Any, List, Literal, Optional, Set, Tuple, Union
 
-from dateutil import parser as dt_parser
+import asyncpg
 
 from . import _constants
-from ._helpers import _SIMPLE_OUTPUT, construct_table, w_print
-from .sql_task import SQLTask, SQLTaskStatus
+from ._helpers import Logger
+from .exceptions import *
 
 
-def _parse_arguments():
-    parser = argparse.ArgumentParser(
-        epilog=_constants._EPILOG, description=_constants._DESCRIPTION
-    )
-    parser.add_argument(
-        "--dev",
-        action="store_const",
-        const="dev",
-        dest="stage",
-        help="Run SQL tasks in the dev schema. Must also include a dev schema. Overrides the SQL_SCHEDULER_STAGE Envvar.",
-    )
-    parser.add_argument(
-        "--prod",
-        action="store_const",
-        const="prod",
-        dest="stage",
-        help="Run SQL tasks in the prod schema. Overrides the SQL_SCHEDULER_STAGE Envvar.",
-    )
-    parser.add_argument(
-        "--verbose",
-        action="store_true",
-        default=False,
-        dest="verbose",
-        help="Logs all queries run against the database.",
-    )
-    parser.add_argument(
-        "--check",
-        action="store_true",
-        dest="check",
-        default=False,
-        help="Do a check for circular dependency without running any scripts.",
-    )
-    parser.add_argument(
-        "--dev-schema",
-        dest="dev_schema",
-        help="The dev schema to replace schemas with in SQL statements.",
-    )
-    parser.add_argument(
-        "--target",
-        "-t",
-        action="append",
-        dest="targets",
-        help="Specific tasks to be run instead of a complete run.",
-    )
-    parser.add_argument(
-        "--dependencies",
-        action="store_true",
-        default=False,
-        help="Flag to run the upstream dependencies of the given targets",
-    )
-    parser.add_argument(
-        "--no-cache",
-        action="store_true",
-        default=False,
-        dest="no_cache",
-        help="Flag to not use cache for development run. Forces a complete run of dependencies.",
-    )
-    parser.add_argument(
-        "--clear-cache",
-        action="store_true",
-        default=False,
-        dest="clear_cache",
-        help="Clears development cache.",
-    )
-    parser.add_argument(
-        "--refill",
-        action="store_true",
-        default=False,
-        dest="refill",
-        help="Force drop and recreate of all incremental tables.",
-    )
-    parser.add_argument(
-        "--start", dest="start", help="Start date/time for incremental table updates."
-    )
-    parser.add_argument(
-        "--end", dest="end", help="End date/time for incremental table updates."
-    )
-
-    args = parser.parse_args()
-    if args.clear_cache:
-        shutil.rmtree(_constants._CACHE_DIR)
-        sys.exit()
+class SQLTaskDDLFileNotExists(Exception):
+    pass
 
-    start = None
-    if args.start is not None:
-        try:
-            start = dt_parser.parse(args.start)
-        except dt_parser.ParserError:
-            print("Unable to parse --start value.")
-            sys.exit(1)
 
-    end = None
-    if args.end is not None:
-        try:
-            end = dt_parser.parse(args.end)
-        except dt_parser.ParserError:
-            print("Unable to parse --end value.")
-            sys.exit(1)
-
-    if start is None or end is None:
-        incremental_interval = None
-    else:
-        incremental_interval = (start, end)
-
-    stage = args.stage
-    if args.stage is None and args.dev_schema is not None:
-        stage = _constants._STAGE_DEV
-    return (
-        stage,
-        args.dev_schema,
-        args.targets,
-        args.dependencies,
-        args.check,
-        args.no_cache,
-        incremental_interval,
-        args.refill,
-        args.verbose,
-    )
-
-
-def _get_task_parents(task: SQLTask, tasks: List[SQLTask]) -> Set[SQLTask]:
-    if len(task.dependencies) == 0:
-        return {task}
-    parents = {task}
-    for dependency in task.dependencies:
-        parent_task = [
-            _task for _task in tasks if _task.task_id.lower() == dependency.lower()
-        ]
-        if len(parent_task) != 1:
-            print(
-                f"FATAL ERROR: task {task.task_id} has a non-existent dependency {dependency}."
-            )
-            sys.exit(1)
+class SQLTaskInsertFileNotExists(Exception):
+    pass
+
+
+_MULTILINE_COMMENT_REGEXP = re.compile(r"""\/\*[\s\S]*?\*\/""", flags=re.IGNORECASE)
+
+_COMMENT_REGEXP = re.compile(
+    r"""(?<!')--[^\r\n]*?$""", flags=re.IGNORECASE | re.MULTILINE
+)
+
+_FROM_JOIN_REGEXP = re.compile(
+    r"""(?<!delete\s)(?:from|join)\s+(?P<after>"?[\w\d]*?"?\."?[\w\d]*"?)\s*""",
+    flags=re.IGNORECASE,
+)
+_INSERT_REGEXP = re.compile(
+    r'(?P<before>insert\s*into\s*"?)([\w\d]*)(?P<after>"?\."?[\w\d]*"?)',
+    flags=re.IGNORECASE,
+)
+_UPDATE_REGEXP = re.compile(
+    r'(?P<before>update\s*"?)([\w\d]*)(?P<after>"?\."?[\w\d]*"?)', flags=re.IGNORECASE
+)
+
+_CREATE_TABLE_REGEXP = re.compile(
+    r'(?P<before>create\s*table\s*(if)?\s*(not)?\s*(exists)?\s*"?)([\w\d]*)(?P<after>"?\."?[\w\d]*"?)',
+    flags=re.IGNORECASE,
+)
+_DROP_TABLE_REGEXP = re.compile(
+    r'(?P<before>drop\s*table\s*(if)?\s*(not)?\s*(exists)?\s*"?)([\w\d]*)(?P<after>"?\."?[\w\d]*"?)',
+    flags=re.IGNORECASE,
+)
+
+_DELETE_REGEXP = re.compile(
+    r'(?P<before>delete\s+from\s*"?)([\w\d]*)(?P<after>"?\."?[\w\d]*"?)',
+    flags=re.IGNORECASE,
+)
+
+_GRANULARITY_TEST_REGEXP = re.compile(r"granularity:([\w, ]*)", flags=re.IGNORECASE)
+_GRANULARITY_TEST = """
+SELECT {columns}
+FROM "{schema}"."{table}"
+GROUP BY {columns}
+HAVING count(1) > 1
+LIMIT 1;
+""".strip()
+
+_NOT_NULL_TEST_REGEXP = re.compile(r"not_null:([\w, ]*)", flags=re.IGNORECASE)
+_NOT_NULL_TEST = """
+SELECT 1
+FROM "{schema}"."{table}"
+WHERE
+{columns}
+LIMIT 1;
+""".strip()
+
+_RELATIONSHIP_TEST_REGEXP = re.compile(
+    r"relationship: ?([\w_]+ ?= ?[\w_]+\.[\w_]+\.[\w_]+)", flags=re.IGNORECASE
+)
+_RELATIONSHIP_TEST = """
+SELECT 1
+FROM "{schema}"."{table}" AS a
+LEFT JOIN "{r_schema}"."{r_table}" AS b on a."{column}" = b."{r_column}"
+WHERE b."{r_column}" IS NULL
+LIMIT 1;
+""".strip()
+
+_UPSTREAM_COUNT_TEST_REGEXP = re.compile(
+    r"""upstream_count:\s*?"?([\w_\\\/]+?)"?\."?([\w_\\\/]+?)"?\s+?(\d+?)[\s\*]""",
+    flags=re.IGNORECASE,
+)
+
+_COUNT_TEST = """
+SELECT COUNT(1) as count
+FROM "{schema}"."{table}"
+;
+""".strip()
+
+_UPSTREAM_GRANULARITY_TEST_REGEXP = re.compile(
+    r"""upstream_granularity:\s*?"?([\w_\\\/]+?)"?\."?([\w_\\\/]+?)"?\s+([\w_\\\/ ,]+)\*?""",
+    flags=re.IGNORECASE,
+)
+
+_INCREMENTAL_REGEXP = re.compile(r"--sql-scheduler-incremental", flags=re.IGNORECASE)
+
+
+class SQLTaskStatus(Enum):
+    TEST_FAILED = -3
+    UPSTREAM_FAILED = -2
+    FAILED = -1
+    WAITING = 0
+    RUNNING = 1
+    SUCCESS = 2
+    QUEUED = 3
+
+
+class SQLTask:
+    task_id: str
+    ddl_directory: str
+    insert_directory: str
+    logger: Logger
+    verbose: bool = False
+    dependencies: Set[str]
+    status: Literal[
+        SQLTaskStatus.UPSTREAM_FAILED,
+        SQLTaskStatus.FAILED,
+        SQLTaskStatus.WAITING,
+        SQLTaskStatus.TEST_FAILED,
+        SQLTaskStatus.RUNNING,
+        SQLTaskStatus.SUCCESS,
+        SQLTaskStatus.QUEUED,
+    ]
+    stage: Literal["dev", "prod"]
+    dev_schema: Optional[str] = None
+    dsn: str
+    verbose: bool
+    failed_tests: List[str]
+    cache_duration: int
+    cache_filename: str
+    no_cache: bool
+    start_timestamp: float = 0
+    script_duration: Union[float, None] = None
+    test_start_timestamp: Union[float, None] = None
+    test_duration: Union[float, None] = None
+    upstream_test_start_timestamp: Union[float, None] = None
+    upstream_test_duration: Union[float, None] = None
+
+    def __init__(
+        self,
+        ddl_directory: str,
+        insert_directory: str,
+        task_id: str,
+        stage: Literal["prod", "dev"],
+        dev_schema: Optional[str],
+        dsn: str,
+        cache_duration: int,
+        logger: Logger,
+        verbose: bool = False,
+    ):
+        self.task_id = task_id
+        self.ddl_directory = ddl_directory
+        self.insert_directory = insert_directory
+        self.stage = stage
+        self.dev_schema = dev_schema
+        self.dsn = dsn
+        self.cache_duration = cache_duration
+        self.logger = logger
+        self.verbose = verbose
+        self.cache_filename = os.path.join(
+            _constants._CACHE_DIR, f"{self.task_id.lower()}.txt"
+        )
+
+        self.dependencies = self._parse_dependencies()
+        self.incremental = self._is_incremental()
+        self.status = SQLTaskStatus.WAITING
+        self.failed_tests = []
+
+    def get_ddl(self) -> str:
+        ddl_file_path = os.path.join(
+            self.ddl_directory,
+            f"{self.task_id}{_constants._TASK_FILE_ENDING}",
+        )
+        if not os.path.exists(ddl_file_path):
+            raise SQLTaskDDLFileNotExists()
+        with open(ddl_file_path, "r") as f:
+            return f.read()
+
+    def get_insert(self) -> str:
+        insert_file_path = os.path.join(
+            self.insert_directory,
+            f"{self.task_id}{_constants._TASK_FILE_ENDING}",
+        )
+        if not os.path.exists(insert_file_path):
+            raise SQLTaskInsertFileNotExists()
+        with open(insert_file_path, "r") as f:
+            return f.read()
+
+    def _clean_sql_script(self, query: str) -> str:
+        """removes comments from sql scripts"""
+        cleaned_query = _COMMENT_REGEXP.sub("", query)
+        cleaned_query = _MULTILINE_COMMENT_REGEXP.sub("", cleaned_query)
+        return cleaned_query
 
-        parents.update(_get_task_parents(parent_task[0], tasks))
-    return parents
+    def _parse_dependencies(self) -> Set[str]:
+        return set(
+            [
+                table.lower().replace('"', "")
+                for table in _FROM_JOIN_REGEXP.findall(
+                    self._clean_sql_script(self.get_insert())
+                )
+            ]
+        )
 
+    def _is_incremental(self):
+        match = _INCREMENTAL_REGEXP.match(self.get_insert())
+        return match is not None
+
+    def remove_second_class_dependencies(
+        self, first_class_dependencies: Set[str]
+    ) -> None:
+        self.dependencies.intersection_update(first_class_dependencies)
+
+    async def _execute_query(
+        self,
+        query: str,
+        params: List[Any] = [],
+        conn: Optional[asyncpg.Connection] = None,
+        fetch: bool = True,
+    ) -> List[asyncpg.Record]:
+        if conn is None:
+            c = await asyncpg.connect(dsn=self.dsn)
+        else:
+            c = conn
+        if self.verbose:
+            self.logger.out(query)
+        if fetch:
+            results = await c.fetch(query, *params)
+        else:
+            results = await c.execute(query, *params)
+        if conn is None:
+            await c.close()
+        return results
+
+    async def run_granularity_test(self, columns: List[str]):
+        schema, table = self.task_id.lower().split(".")
+        if self.stage == _constants._STAGE_DEV:
+            schema = self.dev_schema
+        results = await self._execute_query(
+            _GRANULARITY_TEST.format(
+                columns=",".join(columns), schema=schema, table=table
+            )
+        )
+        return len(results) == 0, f'granularity_({",".join(columns)})'
 
-def _recursive_circular_check(
-    task: SQLTask, tasks: List[SQLTask], history: List[str] = []
-) -> int:
-    """Return 1 if a circular dependency was found"""
-    if task.task_id.lower() in history:
-        print(f'Circular dependency found between tasks {",".join(history)}.')
-        return 1
-    results = 0
-    for dependency in task.dependencies:
-        parent_task = [
-            _task for _task in tasks if _task.task_id.lower() == dependency.lower()
-        ]
-        if len(parent_task) != 1:
-            print(
-                f"FATAL ERROR: task {task.task_id} has a non-existent dependency {dependency}."
+    async def run_not_null_test(self, columns: List[str]):
+        schema, table = self.task_id.lower().split(".")
+        if self.stage == _constants._STAGE_DEV:
+            schema = self.dev_schema
+        results = await self._execute_query(
+            _NOT_NULL_TEST.format(
+                columns="AND ".join([f"{column} IS NULL " for column in columns]),
+                schema=schema,
+                table=table,
             )
-            sys.exit(1)
-        results += _recursive_circular_check(
-            parent_task[0], tasks, [*history, task.task_id.lower()]
         )
+        return len(results) == 0, f'not-null_({",".join(columns)})'
 
-    return results
+    async def run_relationship_test(self, relationship: str, task_ids: Set[str]):
+        schema, table = self.task_id.lower().split(".")
+        if self.stage == _constants._STAGE_DEV:
+            schema = self.dev_schema
+        column, raw_relationship_column = relationship.replace(" ", "").split("=")
+        r_schema, r_table, r_column = raw_relationship_column.split(".")
+        if (
+            f"{r_schema}.{r_table}".lower() in {task_id.lower() for task_id in task_ids}
+            and self.stage == _constants._STAGE_DEV
+        ):
+            r_schema = self.dev_schema
+        results = await self._execute_query(
+            _RELATIONSHIP_TEST.format(
+                schema=schema,
+                table=table,
+                column=column,
+                r_schema=r_schema,
+                r_table=r_table,
+                r_column=r_column,
+            )
+        )
+        return len(results) == 0, f"relationship_({relationship.replace(' ', '')})"
 
+    async def run_count_test(self, schema: str, table: str, count: int):
+        test_name = f"count_({schema}.{table}_{count})"
 
-def _circular_check(tasks: List[SQLTask]) -> bool:
-    """Return True if Cycle found."""
-    result = 0
-    for task in tasks:
-        result += _recursive_circular_check(task, tasks, history=[])
-    return result > 0
-
-
-def _parse_tasks(
-    ddl_directory: str,
-    insert_directory: str,
-    stage: Literal["prod", "dev"],
-    dev_schema: str,
-    dsn: str,
-    cache_duration: int,
-    no_cache: bool,
-    verbose: bool,
-) -> List[SQLTask]:
-    return [
-        SQLTask(
-            ddl_directory,
-            insert_directory,
-            filename[: -1 * len(_constants._TASK_FILE_ENDING)],
-            stage=stage,
-            dev_schema=dev_schema,
-            dsn=dsn,
-            cache_duration=cache_duration,
-            no_cache=no_cache,
-            verbose=verbose,
+        results = await self._execute_query(
+            _COUNT_TEST.format(schema=schema, table=table)
         )
-        for filename in os.listdir(insert_directory)
-        if filename[-1 * len(_constants._TASK_FILE_ENDING) :]
-        == _constants._TASK_FILE_ENDING
-    ]
-
+        if len(results) != 1:
+            return False, test_name
+        return results[0]["count"] > count, test_name
 
-def _should_start_task(task: SQLTask, tasks: List[SQLTask]) -> bool:
-    task_statuses = {task.task_id.lower(): task.status for task in tasks}
-    if task.status != SQLTaskStatus.WAITING:
-        return False
-    for task_id in task.dependencies:
-        task_status = task_statuses.get(task_id)
-        if task_status in [
-            SQLTaskStatus.UPSTREAM_FAILED,
-            SQLTaskStatus.FAILED,
-            SQLTaskStatus.TEST_FAILED,
-        ]:
-            w_print(
-                f"Marking task {task.task_id.lower()} as UPSTREAM_FAILED due to {task_id} ({task_statuses[task_id].name})"
+    async def run_upstream_granularity_test(
+        self, schema: str, table: str, columns: List[str]
+    ):
+        results = await self._execute_query(
+            _GRANULARITY_TEST.format(
+                columns=",".join(columns), schema=schema, table=table
             )
-            task.status = SQLTaskStatus.UPSTREAM_FAILED
-            return False
-        if task_status in [
-            SQLTaskStatus.WAITING,
-            SQLTaskStatus.RUNNING,
-        ]:
-            return False
-    return True
+        )
 
+        return (
+            len(results) == 0,
+            f'upstream_granularity({schema}.{table} | {",".join(columns)})',
+        )
+
+    def _replace_for_dev(self, query: str, task_ids: Set[str]) -> str:
+        repl = rf"\g<before>{self.dev_schema}\g<after>"
+
+        def repl_fn(match: re.Match):
+            if self.dev_schema is None:
+                raise SQLSchedulerNoDevSchema()
+            schema_table = match.groups()[0].lower().replace('"', "")
+            if schema_table in task_ids:
+                # Should do the replacement
+                _, table = schema_table.split(".")
+                return match.group(0).replace(
+                    match.groups()[0], ".".join((self.dev_schema, table))
+                )
+            return match.group(0)
 
-async def execute(
-    stage: Optional[Literal["dev", "prod"]] = None,
-    dev_schema: Optional[str] = None,
-    targets: Optional[List[str]] = None,
-    dependencies: bool = False,
-    check: bool = False,
-    no_cache: bool = False,
-    incremental_interval: Optional[Tuple[datetime, datetime]] = None,
-    refill: bool = False,
-    verbose: bool = False,
-) -> List[SQLTask]:
-    start_time = time.time()
-    # PARSE STAGE (dev, prod)
-    if stage is None:
-        stage = os.environ.get(_constants._STAGE_ENVVAR, _constants._STAGE_PROD)  # type: ignore
-        if stage not in (_constants._STAGE_PROD, _constants._STAGE_DEV):
-            stage = _constants._STAGE_PROD
-
-    # PARSE CACHE DURATION
-    cache_duration = os.environ.get(
-        _constants._CACHE_DURATION_ENVVAR, _constants._BASE_CACHE_DURATION
-    )
-    try:
-        cache_duration = int(cache_duration)
-    except ValueError:
-        print(
-            f"{_constants._CACHE_DURATION_ENVVAR} is set to an invalid value: {cache_duration}. "
-            f"Must be set to a number. Defaulting to {_constants._BASE_CACHE_DURATION}"
-        )
-        cache_duration = _constants._BASE_CACHE_DURATION
-    if cache_duration <= 0:
-        no_cache = True
-    if not no_cache:
-        os.makedirs(_constants._CACHE_DIR, exist_ok=True)
-
-    # PARSE DEV SCHEMA
-    if dev_schema is None:
-        dev_schema = os.environ.get(_constants._DEV_SCHEMA_ENVVAR, "")
-    if stage == _constants._STAGE_DEV and dev_schema == "":
-        print(
-            f"No dev schema provided when stage is set to dev. {_constants._DEV_SCHEMA_ENVVAR} must be set."
-        )
-        sys.exit(1)
+        updated_query = re.sub(_CREATE_TABLE_REGEXP, repl, query)
+        updated_query = re.sub(_DROP_TABLE_REGEXP, repl, updated_query)
+        updated_query = re.sub(_FROM_JOIN_REGEXP, repl_fn, updated_query)
+        updated_query = re.sub(_DELETE_REGEXP, repl, updated_query)
+        updated_query = re.sub(_INSERT_REGEXP, repl, updated_query)
+        updated_query = re.sub(_UPDATE_REGEXP, repl, updated_query)
+        return updated_query
+
+    def _create_cache_key(self, ddl_script: str, insert_script: str):
+        return f'{hashlib.sha256(ddl_script.encode("utf-8")).hexdigest()}_{hashlib.sha256(insert_script.encode("utf-8")).hexdigest()}'
+
+    def _set_cache(self, ddl_script: str, insert_script: str):
+        with open(self.cache_filename, "w") as cache_file:
+            cache_file.write(self._create_cache_key(ddl_script, insert_script))
+            cache_file.write(",")
+            cache_file.write(f"{time.time()}")
 
-    # PARSE DDL DIR
-    ddl_directory = os.environ.get(_constants._DDL_DIR_ENVVAR)
-    if ddl_directory is None:
-        print(f"No DDL directory provided. {_constants._DDL_DIR_ENVVAR} must be set.")
-        sys.exit(1)
-
-    if not os.path.exists(ddl_directory):
-        print(f"DDL Directory: {ddl_directory} is non-existent.")
-        sys.exit(1)
-
-    # PARSE INSERT DIR
-    insert_directory = os.environ.get(_constants._INSERT_DIR_ENVVAR)
-    if insert_directory is None:
-        print(
-            f"No INSERT directory provided. {_constants._INSERT_DIR_ENVVAR} must be set."
-        )
-        sys.exit(1)
+    def _check_is_cached(self, ddl_script: str, insert_script: str):
+        if not os.path.exists(self.cache_filename):
+            return False
+        with open(self.cache_filename, "r") as cache_file:
+            cache_file_contents = cache_file.read()
+        try:
+            cache_key, cache_set_time = cache_file_contents.split(",")
+            cache_set_time = float(cache_set_time)
+        except:
+            os.remove(self.cache_filename)
+            return False
+        if time.time() - cache_set_time > self.cache_duration:
+            os.remove(self.cache_filename)
+            return False
+        if not self._create_cache_key(ddl_script, insert_script) == cache_key:
+            os.remove(self.cache_filename)
+            return False
+        return True
 
-    if not os.path.exists(insert_directory):
-        print(f"INSERT Directory: {insert_directory} is non-existent.")
-        sys.exit(1)
-
-    # PARSE DSN
-    dsn = os.environ.get(_constants._DSN_ENVVAR)
-    if dsn is None:
-        print(f"No dsn provided. {_constants._DSN_ENVVAR} must be set.")
-        sys.exit(1)
-
-    if incremental_interval is None:
-        incremental_interval_duration = int(
-            os.environ.get(
-                _constants._INCREMENTAL_INTERVAL_ENVVAR,
-                _constants._BASE_INCREMENTAL_DURATION,
-            )
-        )
-        now = datetime.today()
-        incremental_interval_start = datetime(now.year, now.month, now.day) - timedelta(
-            days=incremental_interval_duration
-        )
-        incremental_interval_end = datetime(now.year, now.month, now.day) + timedelta(
-            days=1, milliseconds=-1
-        )
-        incremental_interval = (incremental_interval_start, incremental_interval_end)
+    def _get_analyze(self):
+        schema, table = self.task_id.lower().split(".")
+        if self.stage == _constants._STAGE_DEV:
+            schema = self.dev_schema
+        return f"ANALYZE {schema}.{table};"
+
+    async def execute(
+        self,
+        task_ids: Set[str],
+        incremental_interval: Tuple[datetime, datetime],
+        refill: bool,
+        no_cache: bool,
+    ):
+        self.status = SQLTaskStatus.RUNNING
+        self.start_timestamp = time.time()
+        try:
+            ddl_script = self.get_ddl()
+            insert_script = self.get_insert()
+            if self.incremental:
+                insert_script = insert_script.replace(
+                    "$1",
+                    "'"
+                    + incremental_interval[0].strftime("%Y-%m-%d %H:%M:%S")
+                    + "'::timestamp",
+                ).replace(
+                    "$2",
+                    "'"
+                    + incremental_interval[1].strftime("%Y-%m-%d %H:%M:%S")
+                    + "'::timestamp",
+                )
+            if self.stage == _constants._STAGE_DEV:
+                ddl_script = self._replace_for_dev(ddl_script, task_ids)
+                insert_script = self._replace_for_dev(insert_script, task_ids)
+                if not no_cache and self._check_is_cached(ddl_script, insert_script):
+                    self.logger.out(f"Task {self.task_id.lower()} cached.")
+                    self.status = SQLTaskStatus.SUCCESS
+                    return
+            self.upstream_test_start_timestamp = time.time()
+            upstream_test_futures = []
+
+            upstream_count_matches = _UPSTREAM_COUNT_TEST_REGEXP.finditer(insert_script)
+            for upstream_count_match in upstream_count_matches:
+                schema = upstream_count_match.group(1)
+                table = upstream_count_match.group(2)
+                count = upstream_count_match.group(3)
+                try:
+                    count = int(count)
+                except TypeError:
+                    self.failed_tests.append(
+                        f"upstream_count-{schema}-{table}-count-parse_error"
+                    )
+                    continue
+                except ValueError:
+                    self.failed_tests.append(
+                        f"upstream_count-{schema}-{table}-count-parse_error"
+                    )
+                    continue
+                upstream_test_futures.append(
+                    asyncio.create_task(
+                        self.run_count_test(schema, table, count),
+                        name=f"{self.task_id}-upstream-count-test-{schema}-{table}",
+                    )
+                )
 
-    # PARSE TASKS
-    tasks = _parse_tasks(
-        ddl_directory,
-        insert_directory,
-        stage=stage,
-        dev_schema=dev_schema or "",
-        dsn=dsn,
-        cache_duration=cache_duration,
-        no_cache=no_cache,
-        verbose=verbose,
-    )
-    for task in tasks:
-        task.remove_second_class_dependencies({task.task_id.lower() for task in tasks})
-    circular_dependencies = _circular_check(tasks)
-    if circular_dependencies:
-        print("Circular dependencies found... exiting.")
-        sys.exit(1)
-    if check:
-        print("No circular dependencies found...")
-        return tasks
-    if targets is not None:
-        if dependencies:
-            print(f"Identifying upstream dependencies of {targets}...")
-            subset_tasks: Set[SQLTask] = set()
-            for target in targets:
-                target_task = [_task for _task in tasks if _task.task_id == target]
-                if len(target_task) != 1:
-                    print(f"Target {target} is non-existent.")
-                    sys.exit(1)
-                target_task[0].no_cache = True
-                subset_tasks.update(_get_task_parents(target_task[0], tasks))
-            print(
-                f"Found {len(subset_tasks) - len(targets)} tasks in upstream dependencies."
+            upstream_granularity_matches = _UPSTREAM_GRANULARITY_TEST_REGEXP.finditer(
+                insert_script
             )
-            tasks = list(subset_tasks)
-        else:
-            tasks = [task for task in tasks if task.task_id in targets]
-            for task in tasks:
-                task.no_cache = True
-            if len(tasks) != len(targets):
-                print(
-                    f"Unknown Target: {set(targets) - {task.task_id for task in tasks}}"
-                )
-                sys.exit(1)
-    task_ids = {task.task_id.lower() for task in tasks}
-
-    if any([task.incremental for task in tasks]):
-        start, end = incremental_interval
-        print(
-            f'Incremental tasks will be run with the interval {start.strftime("%Y-%m-%d %H:%M:%S.%f")} -> {end.strftime("%Y-%m-%d %H:%M:%S.%f")}'
-        )
+            for upstream_granularity_match in upstream_granularity_matches:
+                schema = upstream_granularity_match.group(1)
+                table = upstream_granularity_match.group(2)
+                columns = [
+                    col.strip()
+                    for col in upstream_granularity_match.group(3).split(",")
+                ]
+                upstream_test_futures.append(
+                    asyncio.create_task(
+                        self.run_upstream_granularity_test(schema, table, columns),
+                        name=f"{self.task_id}-upstream-granularity-test-{schema}-{table}",
+                    )
+                )
+            if len(upstream_test_futures) > 0:
+                self.logger.out(
+                    f"Running {len(upstream_test_futures)} upstream tests for {self.task_id}."
+                )
+            for test in asyncio.as_completed(upstream_test_futures):
+                result, test_name = await test
+                if not result:
+                    self.failed_tests.append(test_name)
+            self.upstream_test_duration = (
+                time.time() - self.upstream_test_start_timestamp
+            )
+            if len(self.failed_tests) > 0:
+                self.logger.out(
+                    f"Task {self.task_id.lower()} failed {len(self.failed_tests)} upstream tests."
+                )
+                self.status = SQLTaskStatus.TEST_FAILED
+                return
+
+            conn = await asyncpg.connect(dsn=self.dsn)
 
-    # EXECUTION LOOP
-    futures = []
-    try:
-        while True:
-            for task in tasks:
-                if _should_start_task(task, tasks):
-                    w_print(f"Scheduling task {task.task_id.lower()} for execution.")
-                    futures.append(
-                        asyncio.create_task(
-                            task.execute(task_ids, incremental_interval, refill=refill),
-                            name=task.task_id.lower(),
-                        )
+            need_to_create_table = False
+            if self.incremental and refill is False:
+                schema, table = self.task_id.lower().split(".")
+                if self.stage == _constants._STAGE_DEV:
+                    schema = self.dev_schema
+                result = await self._execute_query(
+                    "select 1 from INFORMATION_SCHEMA.tables where table_schema = $1 and table_name = $2 LIMIT 1;",
+                    [schema, table],
+                    conn,
+                )
+                if len(result) == 0:
+                    need_to_create_table = True
+                # check if table exists
+            async with conn.transaction():
+                if not self.incremental or refill is True or need_to_create_table:
+                    await self._execute_query(ddl_script, conn=conn, fetch=False)
+                if self.incremental:
+                    insert_script = insert_script.replace(
+                        "$1",
+                        "'"
+                        + incremental_interval[0].strftime("%Y-%m-%d %H:%M:%S")
+                        + "'::timestamp",
+                    ).replace(
+                        "$2",
+                        "'"
+                        + incremental_interval[1].strftime("%Y-%m-%d %H:%M:%S")
+                        + "'::timestamp",
                     )
-            if not {task.status for task in tasks}.isdisjoint(
-                {SQLTaskStatus.WAITING, SQLTaskStatus.RUNNING}
-            ):
-                num_running_tasks = len(
-                    [1 for task in tasks if task.status == SQLTaskStatus.RUNNING]
-                )
-                num_waiting_tasks = len(
-                    [1 for task in tasks if task.status == SQLTaskStatus.WAITING]
-                )
-                num_completed_tasks = len(
-                    [1 for task in tasks if task.status == SQLTaskStatus.SUCCESS]
-                )
-                num_failed_tasks = len(
-                    [1 for task in tasks if task.status == SQLTaskStatus.FAILED]
-                )
-                num_upstream_failed_tasks = len(
-                    [
-                        1
-                        for task in tasks
-                        if task.status == SQLTaskStatus.UPSTREAM_FAILED
-                    ]
-                )
-                num_failed_test_tasks = len(
-                    [1 for task in tasks if task.status == SQLTaskStatus.TEST_FAILED]
-                )
-                if not _SIMPLE_OUTPUT:
-                    w_print(
-                        f"{num_running_tasks} running. "
-                        f"{num_waiting_tasks} waiting. "
-                        f"{num_completed_tasks} completed. "
-                        f"{num_failed_tasks} failed. "
-                        f"{num_upstream_failed_tasks} "
-                        f"upstream failed. "
-                        f"{num_failed_test_tasks} test failed. "
-                        f"Elapsed time: {timedelta(seconds=int(time.time() - start_time))}",
-                        end="\r",
+
+                await self._execute_query(insert_script, conn=conn, fetch=False)
+                await self._execute_query(self._get_analyze(), conn=conn, fetch=False)
+            await conn.close()
+            self.script_duration = time.time() - self.start_timestamp
+
+            self.test_start_timestamp = time.time()
+            test_futures = []
+            granularity_columns_match = _GRANULARITY_TEST_REGEXP.search(insert_script)
+            if granularity_columns_match is not None:
+                columns = [
+                    column.strip()
+                    for column in granularity_columns_match.group(1).split(",")
+                ]
+                test_futures.append(
+                    asyncio.create_task(
+                        self.run_granularity_test(columns),
+                        name=f"{self.task_id}-granularity-test",
                     )
-                await asyncio.sleep(_constants._EVENT_LOOP_SLEEP)
-                continue
-            return tasks
-    except:
-        pass
-    finally:
-        for task in futures:
-            task.cancel()
-        await asyncio.gather(*futures)
-        w_print("")
-        return tasks
-
-
-def sql_scheduler(
-    stage: Optional[Literal["dev", "prod"]] = None,
-    dev_schema: Optional[str] = None,
-    targets: Optional[List[str]] = None,
-    dependencies: bool = False,
-    check: bool = False,
-    no_cache: bool = False,
-    incremental_interval: Optional[Tuple[datetime, datetime]] = None,
-    refill: bool = False,
-    verbose: bool = False,
-):
-    try:
-        tasks = asyncio.run(
-            execute(
-                stage=stage,
-                dev_schema=dev_schema,
-                targets=targets,
-                dependencies=dependencies,
-                check=check,
-                no_cache=no_cache,
-                incremental_interval=incremental_interval,
-                refill=refill,
-                verbose=verbose,
-            )
-        )
-    except:
-        w_print("")
-        sys.exit(1)
-    if check:
-        return
-    failed_task_ids = []
-    test_failed_tasks = []
-    upstream_failed_task_ids = []
-    for task in tasks:
-        if task.status == SQLTaskStatus.FAILED:
-            failed_task_ids.append(task.task_id.lower())
-        if task.status == SQLTaskStatus.TEST_FAILED:
-            test_failed_tasks.append(task)
-        if task.status == SQLTaskStatus.UPSTREAM_FAILED:
-            upstream_failed_task_ids.append(task.task_id.lower())
-
-    w_print(f"Execution Complete.")
-    print(
-        construct_table(
-            [
-                "task_id",
-                "script duration (s)",
-                "test duration (s)",
-                "upstream test duration (s)",
-            ],
-            [
-                (
-                    task.task_id.lower(),
-                    str(
-                        round(
-                            task.script_duration
-                            if task.script_duration is not None
-                            else -1,
-                            1,
-                        )
-                    ),
-                    str(
-                        round(
-                            task.test_duration
-                            if task.test_duration is not None
-                            else -1,
-                            1,
-                        )
-                    ),
-                    str(
-                        round(
-                            task.upstream_test_duration
-                            if task.upstream_test_duration is not None
-                            else -1,
-                            1,
-                        )
-                    ),
-                )
-                for task in sorted(
-                    filter(
-                        lambda task: task.status
-                        not in (SQLTaskStatus.WAITING, SQLTaskStatus.UPSTREAM_FAILED),
-                        tasks,
-                    ),
-                    key=lambda task: task.start_timestamp,
                 )
-            ],
-        )
-    )
-    if (
-        len(failed_task_ids) + len(test_failed_tasks) + len(upstream_failed_task_ids)
-        == 0
-    ):
-        print(f"All {len(tasks)} tasks run successfully.")
-        return
 
-    print(f"{len(failed_task_ids)} tasks failed:")
-    for failed_task_id in sorted(failed_task_ids):
-        print(f" - {failed_task_id}")
-
-    if len(test_failed_tasks) > 0:
-        print(f"Tasks failed tests:")
-        for test_failed_task in test_failed_tasks:
-            print(
-                f" - {test_failed_task.task_id}: {','.join(test_failed_task.failed_tests)}"
-            )
+            not_null_columns_match = _NOT_NULL_TEST_REGEXP.search(insert_script)
+            if not_null_columns_match is not None:
+                columns = [
+                    column.strip()
+                    for column in not_null_columns_match.group(1).split(",")
+                ]
+                test_futures.append(
+                    asyncio.create_task(
+                        self.run_not_null_test(columns),
+                        name=f"{self.task_id}-not-null-test",
+                    )
+                )
 
-    if len(upstream_failed_task_ids) > 0:
-        print(f"Tasks not run because of upstream failures:")
-        for upstream_failed_task_id in sorted(upstream_failed_task_ids):
-            print(f" - {upstream_failed_task_id}")
-
-    sys.exit(1)
-
-
-def main():
-    (
-        stage,
-        dev_schema,
-        targets,
-        dependencies,
-        check,
-        no_cache,
-        incremental_interval,
-        refill,
-        verbose,
-    ) = _parse_arguments()
-    sql_scheduler(
-        stage=stage,
-        dev_schema=dev_schema,
-        targets=targets,
-        dependencies=dependencies,
-        check=check,
-        no_cache=no_cache,
-        incremental_interval=incremental_interval,
-        refill=refill,
-        verbose=verbose,
-    )
+            relationship_match = _RELATIONSHIP_TEST_REGEXP.findall(insert_script)
+            for relationship in relationship_match:
+                test_futures.append(
+                    asyncio.create_task(
+                        self.run_relationship_test(relationship, task_ids),
+                        name=f"{self.task_id}-relationship-{relationship}-test",
+                    )
+                )
 
+            if len(test_futures) > 0:
+                self.logger.out(
+                    f"Running {len(test_futures)} tests for {self.task_id.lower()}."
+                )
+            for test in asyncio.as_completed(test_futures):
+                result, test_name = await test
+                if not result:
+                    self.failed_tests.append(test_name)
+            self.test_duration = time.time() - self.test_start_timestamp
+
+            if len(self.failed_tests) > 0:
+                self.logger.out(
+                    f"Task {self.task_id.lower()} failed {len(self.failed_tests)} tests."
+                )
+                self.status = SQLTaskStatus.TEST_FAILED
+                return
 
-if __name__ == "__main__":
-    main()
+        except Exception as e:
+            self.logger.out(f"Task {self.task_id.lower()} failed:")
+            self.logger.out(f"TASK_EXCEPTION: {e}")
+            if self.script_duration is None:
+                self.script_duration = time.time() - self.start_timestamp
+            self.status = SQLTaskStatus.FAILED
+            return
+        if self.stage == _constants._STAGE_DEV and not no_cache:
+            self._set_cache(ddl_script, insert_script)
+        self.logger.out(f"Task {self.task_id.lower()} complete.")
+        self.status = SQLTaskStatus.SUCCESS
```

### Comparing `sql-scheduler-0.2.5/sql_scheduler.egg-info/PKG-INFO` & `sql-scheduler-0.3.1/sql_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-scheduler
-Version: 0.2.5
+Version: 0.3.1
 Summary: sql-scheduler allows you to easily run a suite of SQL scripts against a Postgres/Redshift database.
 Home-page: https://github.com/henryivesjones/sql-scheduler
 Author: Henry Jones
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: sql,postgres,scheduler,redshift
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -59,25 +59,24 @@
 
 ## Installation
 ```bash
 pip install sql-scheduler
 ```
 ## Configuration
 
-### Required Environment Variables
+### Environment Variables
  - `SQL_SCHEDULER_DDL_DIRECTORY`: An absolute path to the `ddl` directory. EX: `/home/ubuntu/sql/ddl/`
  - `SQL_SCHEDULER_INSERT_DIRECTORY`: An absolute path to the `insert` directory. EX: `/home/ubuntu/sql/insert/`
  - `SQL_SCHEDULER_DSN`: A DSN for connecting to your database in the form: `postgres://user:password@host:port/database?option=value`
-
-### Optional Environment Variables
  - `SQL_SCHEDULER_STAGE`: The default stage (`prod`, `dev`) to run in. Can be overridden by the CLI flag `--dev` or `--prod`. When running in the dev stage a dev schema must be provided, either thru an Environment Variable, or a cli argument.
  - `SQL_SCHEDULER_DEV_SCHEMA`: The schema to replace with when run in the `dev` stage. Can be overridden by the CLI argument `--dev-schema`.
  - `SQL_SCHEDULER_SIMPLE_OUTPUT`: Simplify the output of this program by removing the status message. (If you are running `sql-scheduler` not in the CLI then you probably want to set this to `1`)
  - `SQL_SCHEDULER_CACHE_DURATION`: The length of time for development cache runs to be valid (specified in seconds). Defaults to 6 hours
  - `SQL_SCHEDULER_INCREMENTAL_INTERVAL`: The number of days for the default incremental window (defaults to 14). Incremental windows starts at `00:00:00` 14 days ago and ends at `23:59:59.999` on the current day. The interval can be overridden by setting the `--start` and `--end` cli values.
+ - `SQL_SCHEDULER_CONCURRENCY`: The maximum number of concurrent tasks to be run
 
 ## Common Commands
 
 ### Running all scripts.
 ```bash
 sql-scheduler
 ```
```

