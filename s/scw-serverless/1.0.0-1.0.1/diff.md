# Comparing `tmp/scw_serverless-1.0.0.tar.gz` & `tmp/scw_serverless-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_serverless-1.0.0.tar", max compression
+gzip compressed data, was "scw_serverless-1.0.1.tar", max compression
```

## Comparing `scw_serverless-1.0.0.tar` & `scw_serverless-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      499 2023-04-11 10:45:16.790571 scw_serverless-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-02-02 17:20:42.069490 scw_serverless-1.0.0/LICENSE
--rw-r--r--   0        0        0     2495 2023-02-02 17:20:42.069490 scw_serverless-1.0.0/README.md
--rw-r--r--   0        0        0     2975 2023-04-11 10:45:16.790571 scw_serverless-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       54 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/app.py
--rw-r--r--   0        0        0     6100 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/cli.py
--rw-r--r--   0        0        0       31 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/__init__.py
--rw-r--r--   0        0        0     5104 2023-04-04 13:54:31.192478 scw_serverless-1.0.0/scw_serverless/config/function.py
--rw-r--r--   0        0        0      138 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/__init__.py
--rw-r--r--   0        0        0      219 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/generator.py
--rw-r--r--   0        0        0     4169 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/serverless_framework.py
--rw-r--r--   0        0        0     7045 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/generators/terraform.py
--rw-r--r--   0        0        0     1247 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/config/route.py
--rw-r--r--   0        0        0       14 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/templates/.gitignore
--rw-r--r--   0        0        0      414 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/templates/serverless.yml
--rw-r--r--   0        0        0      426 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/templates/terraform.tf.json
--rw-r--r--   0        0        0      327 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/config/utils.py
--rw-r--r--   0        0        0     3532 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/dependencies_manager.py
--rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/__init__.py
--rw-r--r--   0        0        0      172 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/backends/__init__.py
--rw-r--r--   0        0        0    11072 2023-03-13 13:34:16.012571 scw_serverless-1.0.0/scw_serverless/deploy/backends/scaleway_api_backend.py
--rw-r--r--   0        0        0      524 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_backend.py
--rw-r--r--   0        0        0     1700 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_framework_backend.py
--rw-r--r--   0        0        0        0 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/gateway/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-04 08:42:26.463081 scw_serverless-1.0.0/scw_serverless/gateway/gateway_api_client.py
--rw-r--r--   0        0        0     2792 2023-04-04 15:50:23.232104 scw_serverless-1.0.0/scw_serverless/gateway/gateway_manager.py
--rw-r--r--   0        0        0     2262 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/logger.py
--rw-r--r--   0        0        0      137 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/triggers/__init__.py
--rw-r--r--   0        0        0     1405 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/triggers/cron.py
--rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/__init__.py
--rw-r--r--   0        0        0      239 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/commands.py
--rw-r--r--   0        0        0     1864 2023-03-14 08:51:57.235841 scw_serverless-1.0.0/scw_serverless/utils/credentials.py
--rw-r--r--   0        0        0      590 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/files.py
--rw-r--r--   0        0        0     1476 2023-02-27 15:17:33.009496 scw_serverless-1.0.0/scw_serverless/utils/loader.py
--rw-r--r--   0        0        0      761 2023-02-02 17:20:42.073490 scw_serverless-1.0.0/scw_serverless/utils/string.py
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 scw_serverless-1.0.0/setup.py
--rw-r--r--   0        0        0     4010 1970-01-01 00:00:00.000000 scw_serverless-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      499 2023-04-11 11:30:00.787325 scw_serverless-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-02-02 17:20:42.069490 scw_serverless-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2495 2023-02-02 17:20:42.069490 scw_serverless-1.0.1/README.md
+-rw-r--r--   0        0        0     2974 2023-04-12 12:07:11.489147 scw_serverless-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/app.py
+-rw-r--r--   0        0        0     6100 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/cli.py
+-rw-r--r--   0        0        0       31 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/__init__.py
+-rw-r--r--   0        0        0     5104 2023-04-04 13:54:31.192478 scw_serverless-1.0.1/scw_serverless/config/function.py
+-rw-r--r--   0        0        0      138 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/__init__.py
+-rw-r--r--   0        0        0      219 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/generator.py
+-rw-r--r--   0        0        0     4169 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/serverless_framework.py
+-rw-r--r--   0        0        0     7045 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/terraform.py
+-rw-r--r--   0        0        0     1247 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/config/route.py
+-rw-r--r--   0        0        0       14 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/templates/.gitignore
+-rw-r--r--   0        0        0      414 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/templates/serverless.yml
+-rw-r--r--   0        0        0      426 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/templates/terraform.tf.json
+-rw-r--r--   0        0        0      327 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/utils.py
+-rw-r--r--   0        0        0     3532 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/dependencies_manager.py
+-rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/__init__.py
+-rw-r--r--   0        0        0      172 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/backends/__init__.py
+-rw-r--r--   0        0        0    11072 2023-03-13 13:34:16.012571 scw_serverless-1.0.1/scw_serverless/deploy/backends/scaleway_api_backend.py
+-rw-r--r--   0        0        0      524 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_backend.py
+-rw-r--r--   0        0        0     1700 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_framework_backend.py
+-rw-r--r--   0        0        0        0 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/gateway/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/gateway/gateway_api_client.py
+-rw-r--r--   0        0        0     2341 2023-04-11 15:47:24.983578 scw_serverless-1.0.1/scw_serverless/gateway/gateway_manager.py
+-rw-r--r--   0        0        0     2262 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/logger.py
+-rw-r--r--   0        0        0      137 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/triggers/__init__.py
+-rw-r--r--   0        0        0     1405 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/triggers/cron.py
+-rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/__init__.py
+-rw-r--r--   0        0        0      239 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/commands.py
+-rw-r--r--   0        0        0     1864 2023-03-14 08:51:57.235841 scw_serverless-1.0.1/scw_serverless/utils/credentials.py
+-rw-r--r--   0        0        0      590 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/files.py
+-rw-r--r--   0        0        0     1476 2023-02-27 15:17:33.009496 scw_serverless-1.0.1/scw_serverless/utils/loader.py
+-rw-r--r--   0        0        0      761 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/string.py
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 scw_serverless-1.0.1/setup.py
+-rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 scw_serverless-1.0.1/PKG-INFO
```

### Comparing `scw_serverless-1.0.0/LICENSE` & `scw_serverless-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/README.md` & `scw_serverless-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/pyproject.toml` & `scw_serverless-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "scw-serverless"
-version = "1.0.0"
+version = "1.0.1"
 description = "Framework for writing serverless APIs in Python, using Scaleway functions and containers."
 authors = ["Scaleway Serverless Team <opensource@scaleway.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/scaleway/serverless-api-project"
 documentation = "https://serverless-api-project.readthedocs.io/en/latest/"
 keywords = ["serverless", "scaleway", "functions", "cloud", "faas"]
 
 # Should be one of:
 # "Development Status :: 3 - Alpha"
 # "Development Status :: 4 - Beta"
 # "Development Status :: 5 - Production/Stable"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Internet",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
```

### Comparing `scw_serverless-1.0.0/scw_serverless/app.py` & `scw_serverless-1.0.1/scw_serverless/app.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/cli.py` & `scw_serverless-1.0.1/scw_serverless/cli.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/config/function.py` & `scw_serverless-1.0.1/scw_serverless/config/function.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/config/generators/serverless_framework.py` & `scw_serverless-1.0.1/scw_serverless/config/generators/serverless_framework.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/config/generators/terraform.py` & `scw_serverless-1.0.1/scw_serverless/config/generators/terraform.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/config/route.py` & `scw_serverless-1.0.1/scw_serverless/config/route.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/dependencies_manager.py` & `scw_serverless-1.0.1/scw_serverless/dependencies_manager.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/deploy/backends/scaleway_api_backend.py` & `scw_serverless-1.0.1/scw_serverless/deploy/backends/scaleway_api_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_backend.py` & `scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/deploy/backends/serverless_framework_backend.py` & `scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_framework_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/gateway/gateway_api_client.py` & `scw_serverless-1.0.1/scw_serverless/gateway/gateway_api_client.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/gateway/gateway_manager.py` & `scw_serverless-1.0.1/scw_serverless/gateway/gateway_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,28 +46,19 @@
         created_functions = self._list_created_functions()
         routed_functions = [
             function
             for function in self.app_instance.functions
             if function.gateway_route
         ]
 
-        # The Gateway deletes routes based on the relative_url,
-        # so we need to cleanup all routes at the start,
-        # otherwise we might accidentally delete a route we previously created.
-        # If it has the same relative_url but different http methods.
-        for function in routed_functions:
-            self.gateway_client.delete_route(function.gateway_route)  # type: ignore
-
         for function in routed_functions:
             if function.name not in created_functions:
                 raise RuntimeError(
                     f"Could not update route to function {function.name} "
                     + "because it was not deployed"
                 )
 
             target = "https://" + created_functions[function.name].domain_name
             function.gateway_route.target = target  # type: ignore
 
         for function in routed_functions:
-            if not function.gateway_route:
-                continue
-            self.gateway_client.create_route(function.gateway_route)
+            self.gateway_client.create_route(function.gateway_route)  # type: ignore
```

### Comparing `scw_serverless-1.0.0/scw_serverless/logger.py` & `scw_serverless-1.0.1/scw_serverless/logger.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/triggers/cron.py` & `scw_serverless-1.0.1/scw_serverless/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/utils/credentials.py` & `scw_serverless-1.0.1/scw_serverless/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/utils/files.py` & `scw_serverless-1.0.1/scw_serverless/utils/files.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/utils/loader.py` & `scw_serverless-1.0.1/scw_serverless/utils/loader.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/scw_serverless/utils/string.py` & `scw_serverless-1.0.1/scw_serverless/utils/string.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.0/setup.py` & `scw_serverless-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 {':python_version < "3.11"': ['typing-extensions>=4.4.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['scw-serverless = scw_serverless.cli:main']}
 
 setup_kwargs = {
     'name': 'scw-serverless',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Framework for writing serverless APIs in Python, using Scaleway functions and containers.',
     'long_description': '# Serverless API Framework\n\n[![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)\n[![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-project/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-project/main)\n\nServerless API Framework is a tool that lets you write and deploy serverless functions in python.\nIt bridges your code with the deployment configuration to make it a breeze to work with serverless functions.\n\nStarts by defining a simple Python function:\n\n```python\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\n\n@app.func(memory_limit=256)\ndef hello_world(event, context):\n    return "Hello World!"\n```\n\nDeploy it with `scw-serverless`:\n\n```console\nscw-serverless deploy app.py\n```\n\n## Quickstart\n\n### Install\n\n```console\npip install scw-serverless\n```\n\nThis will install the `scw-serverless` CLI:\n\n```console\nscw-serverless --help\n```\n\n### Writing and configuring functions\n\nYou can transform your python functions into serverless functions by using decorators:\n\n```python\nimport os\nimport requests\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\nAPI_URL = os.environ["API_URL"]\n\n@app.func(memory_limit=256, env={"API_URL": API_URL})\ndef hello_world(event, context):\n    return requests.get(API_URL)\n```\n\nThe configuration is done by passing arguments to the decorator.\nTo view which arguments are supported, head over to this [documentation](https://serverless-api-project.readthedocs.io/) page.\n\nWhen you are ready, you can deploy your function with the `scw-serverless` CLI tool:\n\n```console\nscw-serverless deploy app.py\n```\n\nThe tool will use your Scaleway credentials from your environment and config file.\n\n## What’s Next?\n\nTo learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).\nIf you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-project/tree/main/examples) to get you started.\n\n## Contributing\n\nWe welcome all contributions.\n\nThis project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.\n\n```console\npre-commit install\n```\n',
     'author': 'Scaleway Serverless Team',
     'author_email': 'opensource@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/scaleway/serverless-api-project',
```

### Comparing `scw_serverless-1.0.0/PKG-INFO` & `scw_serverless-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scw-serverless
-Version: 1.0.0
+Version: 1.0.1
 Summary: Framework for writing serverless APIs in Python, using Scaleway functions and containers.
 Home-page: https://github.com/scaleway/serverless-api-project
 License: MIT
 Keywords: serverless,scaleway,functions,cloud,faas
 Author: Scaleway Serverless Team
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

