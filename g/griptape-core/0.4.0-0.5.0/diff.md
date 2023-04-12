# Comparing `tmp/griptape_core-0.4.0.tar.gz` & `tmp/griptape_core-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.4.0.tar", max compression
+gzip compressed data, was "griptape_core-0.5.0.tar", max compression
```

## Comparing `griptape_core-0.4.0.tar` & `griptape_core-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.4.0/LICENSE
--rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.4.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.4.0/griptape/__init__.py
--rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.4.0/griptape/core/__init__.py
--rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.4.0/griptape/core/adapters/__init__.py
--rw-r--r--   0        0        0     2385 2023-04-11 16:28:17.823406 griptape_core-0.4.0/griptape/core/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1010 2023-04-08 22:52:20.104416 griptape_core-0.4.0/griptape/core/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.4.0/griptape/core/base_adapter.py
--rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.4.0/griptape/core/base_executor.py
--rw-r--r--   0        0        0     3688 2023-04-11 17:33:25.304240 griptape_core-0.4.0/griptape/core/base_tool.py
--rw-r--r--   0        0        0      533 2023-04-11 16:17:03.307430 griptape_core-0.4.0/griptape/core/decorators.py
--rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.4.0/griptape/core/executors/__init__.py
--rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.4.0/griptape/core/executors/docker_executor.py
--rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.4.0/griptape/core/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.4.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.4.0/griptape/core/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.4.0/griptape/core/utils/__init__.py
--rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.4.0/griptape/core/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.4.0/griptape/core/utils/manifest_validator.py
--rw-r--r--   0        0        0      708 2023-04-11 20:38:38.831174 griptape_core-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.5.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.5.0/griptape/__init__.py
+-rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.5.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.5.0/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-12 20:48:35.984034 griptape_core-0.5.0/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0     1006 2023-04-12 20:48:35.986046 griptape_core-0.5.0/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.5.0/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.5.0/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     3735 2023-04-12 21:11:39.051228 griptape_core-0.5.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      535 2023-04-12 21:11:39.052977 griptape_core-0.5.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.5.0/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.5.0/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.5.0/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.5.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.5.0/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.5.0/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.5.0/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.5.0/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      708 2023-04-12 21:15:59.333234 griptape_core-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.5.0/PKG-INFO
```

### Comparing `griptape_core-0.4.0/LICENSE` & `griptape_core-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.4.0/README.md` & `griptape_core-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape_core-0.4.0/griptape/core/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.5.0/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         )
 
         for action in tool.actions():
             app.add_api_route(
                 f"{self.path_prefix}{action.config['name']}",
                 functools.partial(self.__execute_action, action),
                 methods=["GET"],
-                description=tool.get_action_description(action)
+                description=tool.action_description(action)
             )
 
         return app
 
     def __execute_action(self, action: callable, value: str) -> dict:
         return ast.literal_eval(
             self.executor.execute(action, value.encode()).decode()
```

### Comparing `griptape_core-0.4.0/griptape/core/adapters/langchain_tool_adapter.py` & `griptape_core-0.5.0/griptape/core/adapters/langchain_tool_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @define
 class LangchainToolAdapter(BaseAdapter):
     def generate(self, tool_action: callable) -> langchain.tools.BaseTool:
         tool = tool_action.__self__
 
         # Double up curly brackets for correct f-string parsing in LangChain prompt templates.
-        description = tool.get_action_description(tool_action).replace("{", "{{").replace("}", "}}")
+        description = tool.action_description(tool_action).replace("{", "{{").replace("}", "}}")
 
         def _run(_self, value: str) -> str:
             return self.executor.execute(tool_action, value.encode()).decode()
 
         async def _arun(_self, query: str) -> str:
             raise NotImplementedError("async is not supported")
```

### Comparing `griptape_core-0.4.0/griptape/core/base_tool.py` & `griptape_core-0.5.0/griptape/core/base_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import json
 import os
 from abc import ABC
 from typing import Optional
 import yaml
 from attr import define, fields, Attribute
+from jinja2 import Template
 
 
 @define
 class BaseTool(ABC):
     MANIFEST_FILE = "manifest.yml"
     DOCKERFILE_FILE = "Dockerfile"
     REQUIREMENTS_FILE = "requirements.txt"
@@ -54,14 +55,18 @@
     def abs_file_path(self):
         return os.path.abspath(inspect.getfile(self.__class__))
 
     @property
     def abs_dir_path(self):
         return os.path.dirname(self.abs_file_path)
 
+    @property
+    def schema_template_args(self) -> dict:
+        return {}
+
     def actions(self) -> list[callable]:
         methods = []
 
         for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
             if getattr(method, "is_action", False):
                 methods.append(method)
 
@@ -73,34 +78,32 @@
             return env_var_value
         else:
             return next(
                 (str(getattr(self, f.name)) for f in self.env_fields if f.metadata.get("env") == name),
                 None
             )
 
-    def get_action_name(self, action: callable) -> str:
+    def action_name(self, action: callable) -> str:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
-            schema = action.config["value_schema"].json_schema("ToolActionSchema")
-
             return action.config["name"]
 
-    def get_action_description(self, action: callable) -> str:
+    def action_description(self, action: callable) -> str:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
             schema = action.config["value_schema"].json_schema("ToolActionSchema")
 
             return str.join("\n", [
-                action.config["description"],
+                Template(action.config["description"]).render(self.schema_template_args),
                 f"Input schema: {json.dumps(schema)}"
             ])
 
-    def get_action_value_schema(self, action: callable) -> dict:
+    def action_schema(self, action: callable) -> dict:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
             return action.config["value_schema"].json_schema("ToolInputSchema")
 
     def validate(self) -> bool:
         from griptape.core.utils import ManifestValidator
```

### Comparing `griptape_core-0.4.0/griptape/core/decorators.py` & `griptape_core-0.5.0/griptape/core/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import functools
-from schema import Schema, And, Use
+from schema import Schema
 
 
 def action(config: dict):
     __config_schema().validate(config)
 
     def decorator(func):
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
-            return func(*args, **kwargs)
+        def wrapper(self, *args, **kwargs):
+            return func(self, *args, **kwargs)
 
-        wrapper.is_action = True
         wrapper.config = config
+        wrapper.is_action = True
 
         return wrapper
     return decorator
 
 
 def __config_schema() -> Schema:
     return Schema({
```

### Comparing `griptape_core-0.4.0/griptape/core/executors/docker_executor.py` & `griptape_core-0.5.0/griptape/core/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.4.0/griptape/core/executors/local_executor.py` & `griptape_core-0.5.0/griptape/core/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.4.0/griptape/core/utils/j2.py` & `griptape_core-0.5.0/griptape/core/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.4.0/pyproject.toml` & `griptape_core-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
```

### Comparing `griptape_core-0.4.0/PKG-INFO` & `griptape_core-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

