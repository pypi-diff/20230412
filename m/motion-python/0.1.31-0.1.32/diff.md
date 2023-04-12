# Comparing `tmp/motion_python-0.1.31.tar.gz` & `tmp/motion_python-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.31.tar", max compression
+gzip compressed data, was "motion_python-0.1.32.tar", max compression
```

## Comparing `motion_python-0.1.31.tar` & `motion_python-0.1.32.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2819 2023-04-11 00:01:27.288007 motion_python-0.1.31/README.md
--rw-r--r--   0        0        0      641 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/api/__init__.py
--rw-r--r--   0        0        0     6702 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/api/models.py
--rw-r--r--   0        0        0     2618 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/cli.py
--rw-r--r--   0        0        0     9885 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/client.py
--rw-r--r--   0        0        0    21630 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/cursor.py
--rw-r--r--   0        0        0     8664 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1348 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/routing.py
--rw-r--r--   0        0        0     3413 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/schema.py
--rw-r--r--   0        0        0    14909 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/store.py
--rw-r--r--   0        0        0     3746 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/task.py
--rw-r--r--   0        0        0     5977 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/trigger.py
--rw-r--r--   0        0        0     1892 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/utils.py
--rw-r--r--   0        0        0     1416 2023-04-11 00:01:46.239987 motion_python-0.1.31/pyproject.toml
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.31/PKG-INFO
+-rw-r--r--   0        0        0     3232 2023-04-12 05:57:39.812966 motion_python-0.1.32/README.md
+-rw-r--r--   0        0        0      641 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/api/__init__.py
+-rw-r--r--   0        0        0     6684 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/api/models.py
+-rw-r--r--   0        0        0     2618 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/cli.py
+-rw-r--r--   0        0        0    10092 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/client.py
+-rw-r--r--   0        0        0    21621 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/cursor.py
+-rw-r--r--   0        0        0     8664 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1348 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/routing.py
+-rw-r--r--   0        0        0     3413 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/schema.py
+-rw-r--r--   0        0        0    14909 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/store.py
+-rw-r--r--   0        0        0     3746 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/task.py
+-rw-r--r--   0        0        0     5977 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/trigger.py
+-rw-r--r--   0        0        0     1892 2023-04-12 05:57:39.820966 motion_python-0.1.32/motion/utils.py
+-rw-r--r--   0        0        0     1544 2023-04-12 05:58:06.745106 motion_python-0.1.32/pyproject.toml
+-rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 motion_python-0.1.32/PKG-INFO
```

### Comparing `motion_python-0.1.31/README.md` & `motion_python-0.1.32/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Motion
 
-[![](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/motion/motion/actions)
+[![motion](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"motion")
+[![docs](https://github.com/dm4ml/motion/workflows/docs/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"docs")
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![GitHub tag](https://img.shields.io/github/tag/dm4ml/motion?include_prereleases=&sort=semver&color=blue)](https://github.com/dm4ml/motion/releases/)
+[![PyPI version](https://badge.fury.io/py/motion-python.svg)](https://badge.fury.io/py/motion-python)
 
 Motion is a framework for building machine learning (ML) applications in Python, designed to give developers **fine-grained control** over **continually-updating** state (e.g., models, indexes, or other data structures).
 
 
 ## Why Motion?
 
 Building production ML applications with reasonable degrees of customization (e.g., fine-tuning on user feedback) can be tedious. First, a developer must set up a database to store their data, data collection pipelines, data preprocessing pipelines, model training pipelines, model serving pipelines, and an interface to interact with the application. To run all pipelines regularly, a developer must also configure and maintain some workflow orchestrator, painstakingly encoding interactions between different pipelines.
```

### Comparing `motion_python-0.1.31/motion/__init__.py` & `motion_python-0.1.32/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/api/api.py` & `motion_python-0.1.32/motion/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,30 +58,30 @@
     @app.get("/get/")
     async def get(args: GetRequest) -> Response:
         cur = app.state.store.cursor()
         res = cur.get(**args.__dict__)
 
         # Check if the result is a pandas df
         if isinstance(res, dict):
-            res = pd.DataFrame(res, index=[0])
+            res = pd.DataFrame([res])
 
         elif not isinstance(res, pd.DataFrame):
             res = pd.DataFrame(res)
 
         return df_to_json_response(res)
 
     @app.get("/mget/")
     async def mget(args: MgetRequest) -> Response:
         cur = app.state.store.cursor()
         res = cur.mget(
             **args.__dict__,
         )
         # Check if the result is a pandas df
         if isinstance(res, dict):
-            res = pd.DataFrame(res, index=[0])
+            res = pd.DataFrame([res])
 
         elif not isinstance(res, pd.DataFrame):
             res = pd.DataFrame(res)
 
         return df_to_json_response(res)
 
     @app.post("/set_python/")
```

### Comparing `motion_python-0.1.31/motion/api/models.py` & `motion_python-0.1.32/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/cli.py` & `motion_python-0.1.32/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/client.py` & `motion_python-0.1.32/motion/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,20 @@
             filter_null (bool, optional): Whether to filter out null values. Filters all records with any null walue for any of the keys requested. Only used in conjuction with include_derived. Defaults to True.
             as_df (bool, optional): Whether to return the result as a pandas dataframe. Defaults to False.
 
 
         Returns:
             pd.DataFrame: The values for the key.
         """
+        if not isinstance(identifiers, list):
+            try:
+                identifiers = list(identifiers)
+            except Exception:
+                raise TypeError("identifiers must be a list or iterable")
+
         args = {
             "relation": relation,
             "identifiers": identifiers,
             "keys": keys,
         }
         args.update(kwargs)
         response = self.getWrapper("/mget/", **args)
@@ -212,15 +218,15 @@
             if isinstance(value, Enum):
                 key_values.update({key: value.value})
 
         # Turn key-values into a dataframe to convert to parquet
         if identifier is None:
             identifier = ""
 
-        df = pd.DataFrame(key_values, index=[0])
+        df = pd.DataFrame([key_values])
         memory_buffer = io.BytesIO()
         df.to_parquet(memory_buffer, engine="pyarrow", index=False)
         memory_buffer.seek(0)
 
         # Create request args
         args = {"args": json.dumps({"relation": relation, "identifier": identifier})}
```

### Comparing `motion_python-0.1.31/motion/cursor.py` & `motion_python-0.1.32/motion/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                     {
                         "identifier": identifier,  # type: ignore
                         "create_at": pd.Timestamp.now(),  # type: ignore
                         "session_id": self.session_id,  # type: ignore
                     }
                 )
                 new_row_dict.update(key_values)
-                new_row_df = pd.DataFrame(new_row_dict, index=[0])
+                new_row_df = pd.DataFrame([new_row_dict])
                 new_row = pa.Table.from_pandas(new_row_df, schema=table.schema)
 
                 # Check schemas match
                 if collections.Counter(new_row.schema.names) != collections.Counter(
                     new_row_df.columns.values
                 ):
                     raise AttributeError(
```

### Comparing `motion_python-0.1.31/motion/entry.py` & `motion_python-0.1.32/motion/entry.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/examples/cooking/dashboard.py` & `motion_python-0.1.32/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/examples/cooking/test.py` & `motion_python-0.1.32/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.32/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.32/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/routing.py` & `motion_python-0.1.32/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/schema.py` & `motion_python-0.1.32/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/store.py` & `motion_python-0.1.32/motion/store.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/task.py` & `motion_python-0.1.32/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/trigger.py` & `motion_python-0.1.32/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/motion/utils.py` & `motion_python-0.1.32/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.31/pyproject.toml` & `motion_python-0.1.32/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.31"
+version = "0.1.32"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -26,39 +26,44 @@
 [tool.poetry.scripts]
 motion = "motion.cli:motioncli"
 
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
 mypy = "^1.1.1"
-coverage = "^7.2.2"
+coverage = {extras = ["toml"], version = "^7.2.3"}
 pre-commit = "^3.2.1"
 types-requests = "^2.28.11.16"
 types-croniter = "^1.3.2.7"
 mkdocs = "^1.4.2"
 mkdocs-terminal = "^4.2.0"
 mkdocs-material = "^9.1.5"
 mkdocstrings = {version="^0.20.0", extras = ["python"] }
 pytkdocs = "^0.16.1"
+linkchecker = "^10.2.1"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.mypy]
 files = "motion"
 mypy_path = "motion"
 warn_return_any = true
 warn_unused_configs = true
 disallow_untyped_defs = true
 exclude = ['motion/tests*']
 ignore_missing_imports = true
 show_error_codes = true
 
+[tool.coverage.run]
+omit = [".*", "*/site-packages/*"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:"
 ]
+fail_under = 100
```

### Comparing `motion_python-0.1.31/PKG-INFO` & `motion_python-0.1.32/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.31
+Version: 0.1.32
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,17 +24,20 @@
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Motion
 
-[![](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/motion/motion/actions)
+[![motion](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"motion")
+[![docs](https://github.com/dm4ml/motion/workflows/docs/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"docs")
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![GitHub tag](https://img.shields.io/github/tag/dm4ml/motion?include_prereleases=&sort=semver&color=blue)](https://github.com/dm4ml/motion/releases/)
+[![PyPI version](https://badge.fury.io/py/motion-python.svg)](https://badge.fury.io/py/motion-python)
 
 Motion is a framework for building machine learning (ML) applications in Python, designed to give developers **fine-grained control** over **continually-updating** state (e.g., models, indexes, or other data structures).
 
 
 ## Why Motion?
 
 Building production ML applications with reasonable degrees of customization (e.g., fine-tuning on user feedback) can be tedious. First, a developer must set up a database to store their data, data collection pipelines, data preprocessing pipelines, model training pipelines, model serving pipelines, and an interface to interact with the application. To run all pipelines regularly, a developer must also configure and maintain some workflow orchestrator, painstakingly encoding interactions between different pipelines.
```

